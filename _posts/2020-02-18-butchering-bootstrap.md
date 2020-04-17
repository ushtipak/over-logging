---
title: "Butchering bootstrap"
categories: [bootstrap, reactjs]
---


Bootstrap is awesome!

Together with Mrs Wify – a website for parents with kids was made, utilizing it's responsiveness and mobile-first approach

![Uno reverse]({{ site.url }}{{ site.baseurl}}/assets/2020-02-18-butchering-bootstrap/uno-reverse.png)
> She did all the coding, I gave motivational speeches and shoulder massage

*However*, a neat, "Leap", theme that was used as a base, conveyed 14k+ lines in `theme.css` and a 3+ MB ballast in `assets/js`

Results of Google's Lighthouse, after initial rollout, were beyond acceptable (w/ simulated throttling):

* Performance: 2
* Accessibility: 95
* Best Practices: 86
* SEO: 100


# Step 1: Remove unused CSS

All tested tools broke something on the page – PurifyCSS, UnCSS, UnusedCSS ...

Ended up manually removing unused CSS blocks with Chrome's code coverage

![Kill me now meme]({{ site.url }}{{ site.baseurl}}/assets/2020-02-18-butchering-bootstrap/polly-kill-me-now.jpg)
> src: [Know Your Meme](https://knowyourmeme.com/photos/508168-kill-me)

## Outcome

CSS trimmed down to 5961 lines (~42%); at long last – 378 in total


# Step 2: JS libs cleanup

In begging, it was pure abundance:

{% highlight shell %}
dist/assets/js$ ls -1 | wc -l
34
dist/assets/js$ du -sh .
3,5M	.
{% endhighlight %}

A bunch of scripts were unused, but apparently required (removal of `twitterFetcher` resulted in killing of parallax)

![WTF am I reading meme]({{ site.url }}{{ site.baseurl}}/assets/2020-02-18-butchering-bootstrap/js-removal.jpg)
> src: [Imgflip](https://imgflip.com/memegenerator/)

Solution was to rewrite what was actually needed

## Outcome

{% highlight shell %}
dist$ du -sh assets/js/
8,0K	assets/js/
{% endhighlight %}


# Step 3: CDN up

Arise Digital Ocean's Spaces with `Restricted File Listing` CDN:

![Digital Ocean Spaces]({{ site.url }}{{ site.baseurl}}/assets/2020-02-18-butchering-bootstrap/do-spaces.png)
> AWS S3-compatible object storage

... and a quick Gzip in Nginx w/ Terraform:

{% highlight terraform %}
  provisioner "remote-exec" {
    inline = [
      "sed -i 's/# gzip_/gzip_/g' /etc/nginx/nginx.conf",
      "systemctl reload nginx.service",
    ]
{% endhighlight %}

## Outcome

Combined with previous improvements – Lighthouse performance jumped to 90+


# Step 4: Next.js

Good friend suggested: "go with N**E**xtJS, everyone is switching!"

![Mr. Trololo]({{ site.url }}{{ site.baseurl}}/assets/2020-02-18-butchering-bootstrap/mr-trololo.jpg)

Few tutorials later and we were ready to migrate

Once we met again, he said: "nah, don't use Next, N**U**xt.js is now the way to go, it uses Vue instead of React"

## Outcome

We're no longer friends


# Step 5: Back to React

4-5 components, Axios, a simple backend and off we go

## Outcome

{% highlight shell %}
$ npm run build

> gdesadecom@0.1.0 build /home/m/cpeople/workspace-wileecoyote/gdesadecom/pquark
> react-scripts build

Creating an optimized production build...
Compiled successfully.
{% endhighlight %}


# In the End

It's starts with:

* 15+ private repos
  * 7 rendered obsolete
* 8+ tools
  * Go (backend)
  * ReactJS and Flexbox (WYSIWYG)
  * rclone (CDN)
  * Terraform (blue / green deploy)
  * Ansible (UAT deploy)
  * Python (automated tweets)
  * bash (glue around)

... I tried so hard and got so far:

* 5 days in
  * 100% Bootstrap
* 3 months in
  * 0% Bootstrap


... but – It doesn't even matter:

![Lighthouse stats]({{ site.url }}{{ site.baseurl}}/assets/2020-02-18-butchering-bootstrap/lighthouse-stats.jpg)
> Butchering complete

