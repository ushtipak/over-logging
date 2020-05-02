---
title: "Design logo in a complicated way"
categories: [whitespace]
---


After nearly 3 years and 7 times the amount of posts, _Over Logging_ finally got a logo

![2 logos]({{ site.url }}{{ site.baseurl}}/assets/2020-05-01-design-logo-in-a-complicated-way/2logos.png)

> (code && human) \|\| (code && code)


Two designs stayed until the very end – left one, made in Inkskape "by hand",
based on an idea from [Hatchful](https://hatchful.shopify.com/), and a
programmatically created one, on the right

Both used Ethan Schoonover's [Solarized](https://ethanschoonover.com/solarized/)
color scheme to be easier on the eyes


# The right way

There are numerous tools that'll help you create a logo

Choose a style (e.g. modern, energetic) and industry (tech, sports, arts), enter desired
name and optionally a slogan – and pick one of the dozens generated in your behalf

However, no matter how nice they might look, logos should stand for something,
and not just be a random representation (oh the irony)


![Alternative logo]({{ site.url }}{{ site.baseurl}}/assets/2020-05-01-design-logo-in-a-complicated-way/alternative-logo.png)

> alternative Pac-Man inspired logo


Although the onion-style logo looked ok, it didn't _mean_ anything

_However_, writing the blog name with an esoteric programming language
and having that code somehow converted to a SVG _did_


# The wrong way

[Whitespace programming language](https://en.wikipedia.org/wiki/Whitespace_%28programming_language%29)
has only three valid chars:

* Space
* Tab
* Line feed

Rudimentary as it is, Whitespace still allows stack manipulation sufficient for
printing out "Over Logging" in a few lines:

{% highlight plaintext %}
[Space][Space][Space]
[Space][Space][Space][Tab][Space][Tab][Space]
[Space][Space][Space][Tab][Tab][Space][Space][Tab][Tab][Tab]
[Space][Space][Space][Tab][Tab][Space][Tab][Tab][Tab][Space]
[Space][Space][Space][Tab][Tab][Space][Tab][Space][Space][Tab]
[Space][Space][Space][Tab][Tab][Space][Space][Tab][Tab][Tab]
[Space][Space][Space][Tab][Tab][Space][Space][Tab][Tab][Tab]
[Space][Space][Space][Tab][Tab][Space][Tab][Tab][Tab][Tab]
[Space][Space][Space][Tab][Space][Space][Tab][Tab][Space][Space]
[Space][Space][Space][Tab][Space][Space][Space][Space][Space]
[Space][Space][Space][Tab][Tab][Tab][Space][Space][Tab][Space]
[Space][Space][Space][Tab][Tab][Space][Space][Tab][Space][Tab]
[Space][Space][Space][Tab][Tab][Tab][Space][Tab][Tab][Space]
[Space][Space][Space][Tab][Space][Space][Tab][Tab][Tab][Tab]

[Space][Space]
[Space]
[Space]
[Tab][Space][Tab]
[Tab]
[Space][Space]
[Space]


[Space][Space][Tab]
[Space]
{% endhighlight %}

> [real chars](https://raw.githubusercontent.com/ushtipak/wspaced-over-logging/master/over-logging.ws)
are replaced with named fields for clarity


The actual logo was made by a more [straightfoward code](https://raw.githubusercontent.com/ushtipak/wspaced/master/main.go)
that used _WS_ script as input to draw spaces and tabs (as squares and
rectangles) on a SVG canvas with configurable props (i.e. ratio of \t to [ ])

So to summarize:

![Profit]({{ site.url }}{{ site.baseurl}}/assets/2020-05-01-design-logo-in-a-complicated-way/profit.jpg)

> src: [Imgflip](https://imgflip.com/memegenerator/)
