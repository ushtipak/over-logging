---
layout: post
title: "Reveal messages with Johnny B pushups"
categories: [css]
---


Motivation and gamification go hand in hand, especially when you're forcing
yourself to do something that should be daily practice

Push-ups, on the other side, are quite healthy

Combine the two, add a bit a of a `display: flex;` to help elements align,
and some JS for fields locking and wrap it with simple number to char
conversion ...

![El Johnny]({{ site.url }}{{ site.baseurl}}/assets/2019-10-12-reveal-messages-with-johnny-b-pushups/johnny-s-signature.png)


# jBravo

Named after Cartoon Network's famous Johnny, lays a project that might help

You "encode" a message of your choice with a bash helper:

{% highlight shell %}
usage: ./jb <message>
{% endhighlight %}

It'll create an HTML with current date and Base64 encoded string as the file
name, containing rows that match each character of given message, with:

  * A placeholder for it's ASCII representation (masked with a dash)
  * Number of completed push-ups (initialized to zero)
  * Number of repetitions needed to complete the daily run (`ord(char)`)
  * EditText and a Button to enter completed sets
  * `date +%F`

Input elements (_type="text" and "submit"_) are by default disabled for all
days except the current one, ensured by `enableToday` being scheduled with
`setInterval`

After midnight, subsequent container is selected and enabled, while the
previous one get frozen permanently, rendering messages useless, if you haven't
completed the target


# Motivation?

Having an option of doing any number of reps, and directly updating it in
the jBravo, will drive you to unveil the letter for that day

Target character is updated with each entered push-up, showing different
results during the training

Try it – checkout the [code](https://github.com/ushtipak/jbravo/), think of
a message that'll hold you for some time and `./jb` it

{% highlight shell %}
$ ./jb '?1337'
$ ls *html
09-10-2019-PzEzMzcK.html
{% endhighlight %}

Fire it up in your favorite browser and start revealing those letters every day

![jBravo]({{ site.url }}{{ site.baseurl}}/assets/2019-10-12-reveal-messages-with-johnny-b-pushups/jbravo-leet-no.png)

