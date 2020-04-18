---
title: "Morse with LEDs on IOT for casual office messaging"
categories: [iot]
---

When a colleague returns from a JS conference and brings back a promotional IOT
piece of hardware, the only thing that makes sense is to build a contraption
that fires LEDs alternately in a way that it can present Morse code, so that we
can send "u suck" memos to each other on the exposed web server

![Neonious Morse LEDs]({{ site.url }}{{ site.baseurl}}/assets/2019-01-24-morse-with-leds-on-iot-for-casual-office-messaging/neonious-morse-leds.jpg)


# Hardware

*Neonious One* is the name of the device and it came pre-patched for the
conference. Attendees were able to access is directly with a utility provided
by the manufactures
([neonious.com/FindMyNeonious](https://www.neonious.com/FindMyNeonious/)),
simply by entering unique 12-digit code of their model, which took them to
gadget's web-based IDE

After the conference, however, factory reset was required
([RTFM](https://www.neonious.com/TPManual)),
if one doesn't want to play with RJ45

{% highlight plaintext %}
me: I'll toss Ethernet cables, won't be needing them
*need cable for initial setup*
me:
{% endhighlight %}
![\*Throws unused RJ45\*]({{ site.url }}{{ site.baseurl}}/assets/2019-01-24-morse-with-leds-on-iot-for-casual-office-messaging/asterisk-throws-unused-rj45-asterisk.jpg)


# Implementation

Sample code will be awaiting in the IDE available on `/neonious/IDE`,
showing how to toggle LEDs, get button press events and fire up a basic server

In our case, message in plain text is passed as a GET:

{% highlight plaintext %}
curl 'http://192.168.3.45/ur_code_is_bad_and_u_should_feel_bad'
{% endhighlight %}


*messageText* is then retrieved from `req.url` and passed on to Morse encoder:

{% highlight plaintext %}
messageMorse = messageText
  .split('')
  .map(function(e) {
    return alphabet[e.toLowerCase()] || '';})
  .join(' ')
  .replace(/ +/g, ' ');
{% endhighlight %}

> neat Morse encode impl from [stackoverflow](https://stackoverflow.com/a/26059399)


Next, encoded message is processed with switch case so that each char is
handled in sequence – dot, dash, pause between parts of the same letter and
pauses between letters and words, with timings from
[Wikipedia](https://en.wikipedia.org/wiki/Morse_code#/media/File:International_Morse_Code.svg)
(ratio of 1 to 3 to 7 for dot, dash and different pauses)

We've created a DNS for convenience, published
[used code](https://github.com/ushtipak/neonious-morse-leds)
and started sending messages

![Morse LEDs in action]({{ site.url }}{{ site.baseurl}}/assets/2019-01-24-morse-with-leds-on-iot-for-casual-office-messaging/u-suck.gif)

`.- -. -.. / - .... . -.-- / .-.. .. ...- . -.. / .... .- .--. .--. .. .-.. -.-- / . ...- . .-. / .- ..-. - . .-.`