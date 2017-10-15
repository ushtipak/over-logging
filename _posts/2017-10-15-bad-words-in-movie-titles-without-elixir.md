---
layout: post
title: "Bad words in movie titles without Elixir"
categories: [python, elixir]
---

Intention was to use Erlangs successor, the mighty
[potion of youth](https://elixir-lang.org/ "potion of youth"), for creating
alternative movie name titles – ones gone bad

Idea was quickly rendered obsolete though, upon realization that both fetching
and processing original titles took about 30 seconds in total with Python,
with similar number of lines of code as the processing time elapsed


# Phase one: Collect underpants

Learning new language with arbitrary challenges of implementing sorting
algorithms, doing simple IO or fetching web data is shiny equivalent of
writing _hello world_, compile, run... Doesn't give you the right feeling
of wielding a new programming asset

So the first part of _let's-have-more-interesting-learning-experience_ was
collecting and normalizing all available movie titles from the web.
Before going straight to Elixir, data was scraped with Python as a code
reference to build from

List of movies got crawled from wikipedia, year 1900 onward with only "English
speaking originated" films targeted. Python's BeautifulSoup and threading
module scraped data in about 20 seconds for all existing titles, ever,
rendering implementation of this step trivial in Elixir

{% highlight python %}
bs = BeautifulSoup(urlopen(Request(
    url, headers={'User-Agent': 'Mozilla/5.0'})), "html.parser")

for table in bs.findAll("table", {"class": "wikitable"}):
    for row in table.findAll("tr"):
        cells = row.findAll("td")
        if cells:
            movies.append(cells[0].find(text=True))
{% endhighlight %}

Bad words dictionaries, on the other hand, can be retrieved from multiple sources.
In this case a bit cleansed version of 
[badwords-list](https://github.com/web-mech/badwords-list "badwords-list") was
used, having ones with digits and special characters removed

Second, and frankly, more prominent, task was to go through all words in all
movie titles and find permutations and variations close to words from _bad_
dictionary and create new movie titles in lightning way. Elixir is awesome
when it comes to CPU utilization, so independent  entries going through a
custom algorithm to find close characters looked promising

Again, for the POC, a few lines of Python were written, since having
pseudo-code or preferably a working algorithm in any familiar language makes
moving to a new programming environment much easier

"Problem" arose when naively optimized Py code processed all titles in just a
few seconds, even with _Global Interpreter Lock_, delivering fine results

{% highlight plaintext %}
original: A Small Town Girl
     bad: A Balls Town Girl

original: Mission: Impossible
     bad: Pissin Impossible

original: The Widow's Investment
     bad: The Dildos Investment

original: Honest Hutch
     bad: Horniest Buttmuch

original: Fun at a Children's Party
     bad: Fun Twat a Children's Party

original: Puppet Master 5: The Final Chapter
     bad: Puppet Masterbate 5: The Anal Chapter

original: The Little Snob
     bad: The Titties Nob

original: That Was Then... This Is Now
     bad: That Ass Then... Shit Is Now
{% endhighlight %}


# The Wolf of Balls Street

Implementing all this in Elixir now felt like forcing oneself to watch all episodes
of [Parks and Recreation](http://www.imdb.com/title/tt1266020/ "Parks and Recreation")
only to cover scenes with Ron Swanson – hence the new plan – bootstrap a
[Karpathy RNN](https://github.com/karpathy/char-rnn "Karpathy RNN")
to spin up ideas for real life use cases to learn Elixir on

