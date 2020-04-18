---
title: "T-Shirt design vote backed by Android and Golang"
categories: [android, golang]
---

When you work at IT company where things like competing in a 16 meter freestyle
swimming race in a kiddy size pool occur, interesting ideas tend to surface

We were planning on throwing an after-work beer day in a backyard of our office
building, celebrating the
[International Beer Day](https://en.wikipedia.org/wiki/International_Beer_Day),
and decided to promote our company’s new t-shirt design

Just 24 hours away from the party start, we’ve realized that, since we're
already inviting a bunch of friends over, why not allow them to vote for a
t-shirt design they like best and have that one eventually printed in a
larger series

As some of us do have the ability to overcomplicate simple things efficiently,
we've reckoned writing some code to back the voting process


# Bundle

Plan was quite straightforward – have a tablet (which we had lying around the
office not doing much) to show two colors without any context in full screen
(immersive), representing the two t-shirt designs, add 10 seconds cooldown
between votes (so that tipsy people with butter fingers won't spam their
favorite design recklessly), have that vote marshaled and sent to a server that
runs a simple API written in Golang, one that accepts POST requests, validates
them over Basic Auth (never enough security for a crucial project like this),
counts votes, adds some potentially interesting text to it and sends that
bundle as a tweet, only to be displayed on Twitter feed running on a TV mounted
near the beforementioned tablet and neatly placed between the two hanged
t-shirt prototypes


![Expectation]({{ site.url }}{{ site.baseurl
}}/assets/2018-09-10-t-shirt-design-vote-backed-by-android-and-golang/bundle-expectation.png)
> Expectation


# Ex{planations,cuses,ceptions}

As mentioned, the nutshell of the idea was conceived one day before the party,
but actual development started about _2 Minutes to Midnight_ on the very same
day, so tomorrow on the T-day, we've realized we were lacking dev status for
our company's Twitter account, which would grant us their API access...

Also, due to time constraints, code quality of our solution was shitty
(_if there was more time – it would still be shitty..._ OH SHUT UP!)

Getting approval from Twitter apparently isn't something one gets on short
notice (we've tried), so we were forced to take the alternate route


![Expectation]({{ site.url }}{{ site.baseurl
}}/assets/2018-09-10-t-shirt-design-vote-backed-by-android-and-golang/bundle-reality.png)
> Reality


Twitting part (alongside additional content fetch) on Golang side was replaced
with direct HTML templating – thankfully, A Wild colleague / friend Appears –
Mr [Nemanja C](https://github.com/nemanjacosovic "Nemanja C's GitHub profile"),
Frontend dev and UX design guru jumped in and orchestrated entire UI part of
the app

Since t-shirt designs had a retro 80's throwback, we've decided that the best
way to present results would be with an era appropriate, fighting style layout
– a VS-like screen with a animated 'Thank you' appearing after each vote,
alongside a slightly enlarged t-shirt that has more votes

All patched up – running behind npm's _live-server_ with iptables re-routing
(live-server doesn't take kindly to port 80, and it would be lame to reside on
something like 3000), hence –

{% highlight plaintext %}
iptables -t nat -A PREROUTING -i eth0 -p tcp \
  --dport 80 -j REDIRECT --to-port 8080
{% endhighlight %}


# After all the beer

All systems are a go!


![Tablet IRL]({{ site.url }}{{ site.baseurl
}}/assets/2018-09-10-t-shirt-design-vote-backed-by-android-and-golang/tablet-irl.jpg)
> Choose wisely


![Tablet Screenshot]({{ site.url }}{{ site.baseurl
}}/assets/2018-09-10-t-shirt-design-vote-backed-by-android-and-golang/tablet-screenshot.jpg)
> Screenshot of 3 secs post vote


![IRL Frontend]({{ site.url }}{{ site.baseurl
}}/assets/2018-09-10-t-shirt-design-vote-backed-by-android-and-golang/irl-frontend.jpg)
> Frontend IRL


![IRL Backend]({{ site.url }}{{ site.baseurl
}}/assets/2018-09-10-t-shirt-design-vote-backed-by-android-and-golang/irl-backend.jpg)
> Backend IRL


Vote was a success (after a few beers we like to believe that it was) and it
did produce a winner


![Vote results]({{ site.url }}{{ site.baseurl
}}/assets/2018-09-10-t-shirt-design-vote-backed-by-android-and-golang/vote-results.jpg)
> Go Yellow Matori!


Two of us responsible for the entire shebang patted ourselves on the backs,
gave each other a high five and destroyed all evidence this ever happened

Except [Android](https://github.com/ushtipak/t-shirt-brodown) code...
and [frontend](https://github.com/nemanjacosovic/HLV-matoridev-tshirt-vote)
code... aaand [Golang](https://github.com/ushtipak/broadway) code... sigh

