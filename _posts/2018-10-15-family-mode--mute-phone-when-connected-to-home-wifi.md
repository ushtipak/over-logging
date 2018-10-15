---
layout: post
title: "Family Mode | Mute phone when connected to home WiFi"
categories: [android]
---

Title pretty much explains it – when your Android phone is connected to a
marked WiFi network, app will disable the ringer

Why? The kids might be sleeping

So, in short:

{% highlight plaintext %}
if (kid.count >= 1) && (kid.averageAge <= 5) && (you.hasAndroidPhone): continue
{% endhighlight %}

Idea is simple and comes from personal preference of not wanting anyone to ring
me up when I'm home and potentially wake my kids, if they might be sleeping

So the logic is trivial – when I enter _mi casa_, phone connects to my home
WiFi, Android's BroadcastReceiver sends `android.net.wifi.STATE_CHANGE` and
Family Mode plainly enables silent stance. Once out of the range of home
wireless, same broadcast message is sent and app puts the ringer back on


# Endless features

Well, three, to be precise: mark SSID you're currently connected to, manage
saved ones and toggle service functionality

![Family Mode: Mark and manage SSIDs]({{ site.url }}{{ site.baseurl}}/assets/2018-10-15-family-mode--mute-phone-when-connected-to-home-wifi/family-mode-mark-and-manage.jpg)

Same and infinitely more can be achieved with professional apps like
[Automate](https://play.google.com/store/apps/details?id=com.llamalab.automate)
and [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm),
but this was more of a 
[_lets-make-a-lightweight-app-on-my-own_](https://github.com/ushtipak/family-mode/)
sort of a thing

![Family Mode: Toggle service]({{ site.url }}{{ site.baseurl}}/assets/2018-10-15-family-mode--mute-phone-when-connected-to-home-wifi/family-mode-toggle.jpg)
> service disabled == ringer enabled; and vice-versa

