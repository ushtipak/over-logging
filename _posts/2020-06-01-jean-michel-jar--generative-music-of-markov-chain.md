---
title: "Jean-Michel Jar: generative music of Markov chain"
categories: [ml, java]
---


[Jean-Michel Jarre](https://en.wikipedia.org/wiki/Jean-Michel_Jarre)
is a great composer, known for beautiful instrumentals

His surname resembles Java class package format, so it only makes sense to use
[Markov chain](https://en.wikipedia.org/wiki/Markov_chain) to generate records that
resemble his music in Java

![IDE w/ jmichel]({{ site.url }}{{ site.baseurl}}/assets/2020-06-01-jean-michel-jar--generative-music-of-markov-chain/jmichel.png)


# import org.jfugue.pattern.Pattern;

The simplest way of transcribing notes is from a `*.mid` file

Since we're dealing with MIDI input, playing and saving generated notes,
[JFugue](http://www.jfugue.org/), _Music Programming for Java_, is used here

Jean-Michel's [Oxygène (Part IV)](https://www.youtube.com/watch?v=N4oSXmnkPUU)
has by far the most recognizable theme, and is publicly available in mentioned form

Transcribed into a note pattern, it's 46 element array is used for ML train


# Andrey Markov

Predicting items in a chain is based on a [simple principle](https://setosa.io/ev/markov-chains/):
probability of each event depends solely on the previous ones

In contrary to most machine learning algorithms – Markov chain doesn't
require copious amounts of input, hence permutations from note pattern are sufficient:

{% highlight plaintext %}
C6q R/0.16666666666666607 G5T. R/0.036458333333333925 EB5I R/0.040104166666667496 G5/0.203125 R/0.04843749999999858 C5/0.5833333333333334 RH C6Q R/0.16666666666666607 G5T. R/0.036458333333333925 EB5I R/0.040104166666667496 G5/0.203125 R/0.04843749999999858 C5/0.5833333333333334 RH BB5Q R/0.16666666666666607 A5T. R/0.036458333333333925 G5I R/0.040104166666667496 A5/0.203125 R/0.04843749999999858 D5/0.5833333333333334 R/0.5078125 A5/0.1234375 R/0.02083333333333215 G5/0.0484375 R/0.0442708333333357 F5/0.12083333333333333 R/0.0390625 C5/0.4817708333333333 R/0.11093749999999858 A5/0.140625 R/0.014062500000001421 G5/0.052083333333333336 R/0.04322916666666643 F5/0.11197916666666667 R/0.02708333333333357 C5/0.45208333333333334 R/0.16145833333333215
{% endhighlight %}

Regained pattern is split into words slice and a field map of
`String: ArrayList<String>` is populated with each word:
  * if *previous* word has been joined before – current one is added to it's array
  * otherwise – a key (preceding word) is created with mapping to current one

There is no subsequent for the last word, of course, so the key with longest
value array is added as it's value

A random note from theme is selected as the initial link and the ensuant ones are
chained based on the probability of the last one, up to the desired length

E.g:

{% highlight plaintext %}
C5/0.5833333333333334 RH C6Q R/0.16666666666666607 A5T. R/0.036458333333333925 G5I R/0.040104166666667496 G5/0.203125 R/0.04843749999999858 C5/0.5833333333333334 RH C6Q R/0.16666666666666607 A5T. R/0.036458333333333925 EB5I R/0.040104166666667496 A5/0.203125 R/0.04843749999999858 C5/0.5833333333333334 RH C6Q R/0.16666666666666607 A5T. R/0.036458333333333925 EB5I R/0.040104166666667496 A5/0.203125 R/0.04843749999999858 C5/0.5833333333333334 RH C6Q R/0.16666666666666607 A5T. R/0.036458333333333925 G5I R/0.040104166666667496 G5/0.203125 R/0.04843749999999858 C5/0.5833333333333334 RH C6Q R/0.16666666666666607 G5T. R/0.036458333333333925 G5I R/0.040104166666667496 G5/0.203125
{% endhighlight %}

Different...

![But same]({{ site.url }}{{ site.baseurl}}/assets/2020-06-01-jean-michel-jar--generative-music-of-markov-chain/but-same.jpg)
> src: [Flickr](https://www.flickr.com/photos/lesterchan/18233447992)


[Code](https://github.com/ushtipak/jean-michel-jar) is available to dissect
alongside a few generated analogues to the famous theme:

{% include markov.html %}

