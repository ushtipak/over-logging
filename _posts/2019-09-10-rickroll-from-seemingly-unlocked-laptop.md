---
layout: post
title: "Rickroll from seemingly unlocked laptop"
categories: [python, xflock]
---


At work we have a tendency of sending highly inappropriate content from other
colleagues laptops, if they forget to lock them

If you have similar, neat working environment – and want to have fun with the
lurkers that await for a unprotected computer – fetch
[never-gonna](https://raw.githubusercontent.com/ushtipak/never-gonna/master/astley.py)
script and start it before leaving your machine

Python code with bindings to Tk GUI simply shows an image of your like, one
that resembles unlocked desktop (i.e. IDE with opened project or some emails)
and actually locks screen with xflock4 on any keyboard or mouse event, showing
our dear Astley in a genuine
[rick-rolling](https://en.wikipedia.org/wiki/Rickrolling) fashion


# Proper Rickrolling

Correct image is important, so here is how to get the most prominent Astley
representation – retrieve the signature song in best video quality and extract
a recognizable photo for the lock screen

{% highlight plaintext %}
youtube-dl https://www.youtube.com/watch?v=dQw4w9WgXcQ -f 137
ffmpeg -ss 00:00:04 -i _-dQw4w9WgXcQ.mp4 -vframes 1 -q:v 2 never-gonna.jpg
{% endhighlight %}

> Fetch 1920x1080 mp4 and acquire 4th sec frame

![Rick Astley]({{ site.url }}{{ site.baseurl}}/assets/2019-09-10-rickroll-from-seemingly-unlocked-laptop/never-gonna.jpg)


# Rollout

Dev setup involved XFCE, Mint and light-locker, but the code can be used
in any DE / screensaver combination

Fetch py [code](https://github.com/ushtipak/never-gonna),
install tkinter (e.g., `sudo apt-get install python3-tk`) and Pillow
(`pip install -r requirements.txt`) and ensure lightdm-gtk packages are in
place

{% highlight plaintext %}
liblightdm-gobject-1-0:amd64
lightdm
lightdm-gtk-greeter
lightdm-settings
{% endhighlight %}

Fire up `lightdm-settings`, choose Mr Rick for the background, toggle
`Draw user backgrounds`, update HONEYPOT and XFLOCK in `astley.py` and enjoy
subtle jesting

![LightDM Settings]({{ site.url }}{{ site.baseurl}}/assets/2019-09-10-rickroll-from-seemingly-unlocked-laptop/lightdm-settings.png)
⮕ ![Never Gonna IRL]({{ site.url }}{{ site.baseurl}}/assets/2019-09-10-rickroll-from-seemingly-unlocked-laptop/irl.gif)

