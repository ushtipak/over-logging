---
title: "\"What is my purpose?\" (aka Debian on ROG G20AJ)"
categories: [debian]
---

Bought an _Asus ROG_ desktop with a plan to use it as a development workstation
_and_ a gaming computer. Potential reboots between the two OSes were solved by
placing _Debian_ inside a virtual machine, with half of total RAM and host CPUs

After some time, we (me, myself and _moi_) unanimously agreed that Alt-tabbing
was not practical in this scenario so 2 worlds needed to be fully separated

Q: _What is my purpose?_

A: _You are a development workstation_

![What is my purpose]({{ site.url }}{{ site.baseurl }}/assets/2017-08-31-what-is-my-purpose-aka-debian-on-rog-g20aj/what-is-my-purpose.png)

Strangely enough, it turned out that dual booting _G20AJ_ is not that easy

_Debian netinst_ or any fully fledged installation with DE wouldn't boot. _Mint_
behaved the same (both _LMDE2_ and _Sonya_), alongside _Fedora_, _{,K}Ubuntu_
and even _PCLinuxOS_ (_'member finest GPU support? ... I 'member_)

Irrelevant of the image preparation method (burning onto a CD or writting to a
USB in a few different ways, just to be sure), display always went blank.
Welcome screen was indeed visible, but after choosing any of the boot options
– _Elsa_ emerged

2^6 different UEFI configurations were tested, HDMI cable magic was exercised
and even the sturdy VGA HD-15 tried it's luck. All options were tried out
– fallbacks, "safe boots", forced CPU gfx, _realloc_, _noacpi_,
_n{vidia,ouveau}.modeset_, the catch-all _nomodeset_...

After everything failed and reading the cries from users in similar situation
came to a grinding halt, it was obvious that an alternative
_there-is-a-way-I-told-you-so_ solution needs to come forth – let's install a
_server distribution_ and migrate away from it!


# Brave New World

Man with no Linux choose _Ubuntu Server_ as a host for future abandonment

Installation was simple, "framebuffer safe", and login prompt quickly appeared.
For a few minutes, at least, before being completely overwritten with _Sid_

In order to migrate from this temporary distro to a _Debian Testing_ one needs
to update _sources.list_

{% highlight plaintext %}
deb http://deb.debian.org/debian testing main contrib non-free
{% endhighlight %}

Public key needs to be imported, so that new packages can be fetched; and plain
_dist-upgrade_ fails with package inconsistencies, so here is the long list
of commands needed to summon a new _Debian_

{% highlight plaintext %}
gpg --keyserver pgpkeys.mit.edu --recv-key 7638D0442B90D010
gpg -a --export 7638D0442B90D010 | apt-key add -
apt-get dist-upgrade -f
apt-get autoremove
{% endhighlight %}

Reboot and enjoy

There is always a way, even if it takes 3 days of hair.pull()

{% highlight plaintext %}
root@phoenix-person:~# lshw | grep ASUS -B 1 \
> | sed 's/ //g' | awk -F"(" '{print $1}' | sort -n | uniq
--
product:G20AJ
vendor:ASUSTeKCOMPUTERINC.
root@phoenix-person:~# cat /etc/issue
Debian GNU/Linux buster/sid \n \l
{% endhighlight %}

