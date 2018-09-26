---
layout: post
title: "Count valid words on registration plates with Elixir"
categories: [elixir]
---

Elixir and :observer.start(), since app completion, look like this:

![Elixir: application process tree from :observer]({{ site.url }}{{ site.baseurl}}/assets/2018-09-26-count-valid-words-on-registration-plates-with-elixir/elixir-application-process-tree-from-observer.png)
> Elixir application process tree

Vehicle registration plates of Serbia, since 2011, look like this:

![Exemplary registration plate]({{ site.url }}{{ site.baseurl}}/assets/2018-09-26-count-valid-words-on-registration-plates-with-elixir/exemplary-registration-plate.jpg)
> src: [Wikipedia](https://en.wikipedia.org/wiki/Vehicle_registration_plates_of_Serbia#/media/File:License_plate_of_Serbia,_2014.JPG)

Simple principle of 2 predefined letters (representing larger cities), 3 to 4
numbers and 2 random letters, e.g:

{% highlight plaintext %}
BO 1234 OB
{% endhighlight %}

It's easy to guess where to go from here – how many valid words can we glue
together with these letters – backed with Elixir, poolboy, tiny bit of Go and
Docker, as a tech stack


# Entrée

It's not every day that a new city gets build and grows beyond a certain point
to get it's own 2 letter prefix for registration, but hard-coding existing ones
is still lame

Closest thing to an official list of currently valid Serbian city codes is by
far the [Wikipedia](https://en.wikipedia.org/wiki/Vehicle_registration_plates_of_Serbia)
entry. Fetching purely region IDs from this location requires some code and
either CSS selector or XPath, so Golang and _antchfx/htmlquery_ are called in:

{% highlight golang %}
w := bufio.NewWriter(f)
for _, n := range htmlquery.Find(doc, xPath) {
    _, err := w.WriteString(htmlquery.InnerText(n) + "\n")
    check(err)
}
w.Flush()
{% endhighlight %}


... with XPath being:

{% highlight plaintext %}
"//*[@id=\"mw-content-text\"]/div/table[1]/tbody/tr[*]/td[1]"
{% endhighlight %}

Ancient scrolls, c. 320 BC


# Main course

Having plate codes retrieved as shown above, supported with a list of American
English dictionary words (/usr/share/dict, _wamerican:2018.04.16-1_), poolboy
can be fired up

Elixir playground was bootstrapped via mighty _mix_ and main dish included
_lib/ex_plates/execute.ex_ module, alongside lightweight _worker.ex_

Worker (configured with _{:size, 64}, {:max_overflow, 32}_) is in charge of
ensuring that word being checked indeed starts with 2 letters available in
gathered city codes:

{% highlight elixir %}
def handle_call({word, plate_codes}, _from, state) do
  for plate_code <- plate_codes do
    is_valid = String.starts_with?(String.downcase(word), String.downcase(plate_code))
    if is_valid and not String.contains?(word, "'") do
      IO.puts String.upcase(word)
    end
  end
  {:reply, word, state}
end
{% endhighlight %}


Primary logic, however, lies in mentioned _Execute_ module

Previously prepared _plate_codes_ are loaded as a list (80 2-letter city
prefixes), while the following stream over _wordlist_file_ (_wamerican_ dict)
relies extensively on Elixir's Pipe Operator (taking result of one expression
and passing it on, shell-like)

{% highlight shell %}
$ wc -l < /usr/share/dict/words
102401
{% endhighlight %}


Content of given file (~100k words) is streamed as input to a function that
gets rid of trailing spaces; that output is fed to a _fn_ which filters only 4
chars phrases, which is further the input sent to poolboy workers (generic
pooling lib for Erlang), ones that do the lifting:

{% highlight elixir %}
defmodule Execute do
  @timeout 1000

  def start do
    plate_codes_file = "/tmp/platecodes"
    wordlist_file = "/usr/share/dict/words"

    plate_codes = File.stream!(plate_codes_file) 
                  |> Stream.map(&String.trim/1)
                  |> Enum.to_list

    File.stream!(wordlist_file)
    |> Stream.map(&String.trim/1)
    |> Stream.filter(fn(n) -> String.length(n) == 4 end)      
    |> Stream.map(fn line ->
         Task.async(fn ->
           :poolboy.transaction(
             :worker,
             fn pid -> GenServer.call(pid, {line, plate_codes}) end,
             @timeout
           )
         end)
       end)
    |> Stream.each(fn task -> task |> Task.await(@timeout) end)
    |> Stream.run
  end

end
{% endhighlight %}


# Dessert

Since bootstrapping a working Elixir workstation is not trivial – let's use
Docker

![Ain't nobody got time for Elixir dev]({{ site.url }}{{ site.baseurl}}/assets/2018-09-26-count-valid-words-on-registration-plates-with-elixir/aint-nobody-got-time-for-that.jpg)

{% highlight shell %}
FROM elixir
MAINTAINER ushtipak@gmail.com
RUN apt-get -y update

# prepare and execute platecodes (golang)
WORKDIR /opt/plates/
RUN apt-get install -y git golang
RUN git clone https://github.com/ushtipak/platecodes.git

WORKDIR /opt/plates/platecodes
RUN GOPATH=$HOME/go go get github.com/antchfx/htmlquery
RUN GOPATH=$HOME/go go run platecodes.go

# prepare and execute ex-plates (elixir)
RUN mkdir -p /opt/plates/ex-plates
WORKDIR /opt/plates/ex-plates
COPY . /opt/plates/ex-plates
RUN apt-get install -y wamerican

RUN mix local.hex --force && mix deps.get
RUN mix local.rebar --force
CMD mix run -e "Execute.start"
{% endhighlight %}

Sufficiently understandable, here in action:

![Run Docker, run, "head"]({{ site.url }}{{ site.baseurl}}/assets/2018-09-26-count-valid-words-on-registration-plates-with-elixir/run-docker-run-head.png)

[ ... ]

![Run Docker, run, "tail"]({{ site.url }}{{ site.baseurl}}/assets/2018-09-26-count-valid-words-on-registration-plates-with-elixir/run-docker-run-tail.png)
> Compilation messages excluded, getting the final result


# TL;DR

[Code](https://github.com/ushtipak/ex-plates),
[code](https://github.com/ushtipak/platecodes),
[Docker image](https://hub.docker.com/r/ushtipak/ex-plates/)
– 804 in total

