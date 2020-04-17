---
title: "Static website on S3 and away from WordPress"
categories: [aws, s3, wordpress]
---

A few friends of mine and myself are running a office share type of place,
quite nice, I'd say. Plenty of parking space, free coffee, tea and table tennis,
and people seem to like it

We had a landing page in WordPress, since, although all of us are in IT,
we suck at design, so creating something on our own was out of the question.
WP itself was not the problem, of course. It does an excellent job in providing
a solid base with a healthy ecosystem of plugins and themes

Problem arose when we moved from a hosted instance of a cloud provider to a
dedicated WP "all-around hosting solution" from a large web hosting company –
and we haven't been carefully reading the small print

Story was quite awesome when we initially transfered our WP site. Neat price of
just 12 bucks for a year and no one had to regularly patch underlying Debian,
Nginx, MySQL – it was all part of the pitch. However, after twelve months passed,
we received a new yearly bill that was closer to 90 bucks!

It's not a big deal, we tend to earn some money from the business, but this
thing was a 7x price increase, for no extra benefit. Therefore, it was
irritating and unfair, so we decided to move our landing page away from this
tyranny and redo it in the same time

For the task of rebuilding the page, we used a free tool called
[Mobirise](https://mobirise.com "Mobirise") and patched up a
fine single page in a few hours. A few pictures here and there, pricing model
with benefits of different tiers, location and other ways of reaching us, all
sprinkled with a parallax or two, since everyone seems to like these today

Site was responsive and easily packed in a tar.gz for distribution, and now back
on a regular VM instance in the cloud. Although we were now paying about a 70%
of dedicated WP hosting price for the cloud VM, and had to do all the maintenance
on our own, we were more than satisfied in moving away from the vultures

From there, we decided to go one step further and transfer everything to Amazon
S3, and below is the brief outline of how to achieve that in a quick fashion


# Up and away

We're using _quickstart-website_ bootstrap from AWS in order to speed up content
upload, but we're not relying on _CloudFront_ or _Route 53_ which go alond with.
Latter is related to DNS setup, while most rely on their domain provider, and
the CF part is about enabling HTTPS over S3 and distributing content
geographically. In case of our office share business, neither was needed, but
if you require any of above, use URL from _CloudFront_ as your domain's CNAME
and enjoy

We'll be creating a separate user for hosting as a good practice to distinguish
projects, users and permissions. Uploading website content will be next, followed
up with disabling automatically created _CloudFront_ distribution(s). Bucket
replication with permissions, policies, and _Static website hosting_ setup
follows and last step is simply pointing your domain to S3 bucket via a CNAME
and happily reloading


## IAM

* Go to
[console.aws.amazon.com/iam](https://console.aws.amazon.com/iam "console.aws.amazon.com/iam")
  * Make a note of IAM users sign-in link, for logging with non-root account

* Create user
  * Check _Programmatic access_ and _AWS Management Console access_
  * Set a password and uncheck _Require password reset_

* Attach policies
  * Add **AmazonS3FullAccess** and **CloudFrontFullAccess**

![AWS IAM user permissions]({{ site.url }}{{ site.baseurl }}/assets/2017-06-28-static-website-on-s3-and-away-from-wordpress/aws-iam-permissions.png)

> Write down Access key ID and **Secret access key**, since latter won't be
available for retrieval afterwards


## Host a static website

* Login with new user and go to
[console.aws.amazon.com/quickstart-website](https://console.aws.amazon.com/quickstart-website "console.aws.amazon.com/quickstart-website")

* Select _Your website_
  * Upload your entire site in ZIP

![AWS Host a static website]({{ site.url }}{{ site.baseurl }}/assets/2017-06-28-static-website-on-s3-and-away-from-wordpress/aws-static-website.png)

> We're neatly skipping separate file upload to S3 which requires more time to
setup via AWS CLI


## Disable CloudFront

* Go to
[console.aws.amazon.com/cloudfront](https://console.aws.amazon.com/cloudfront "console.aws.amazon.com/cloudfront")

* Disable and delete distributions
  * If reduntant distributions have been created, select one and choose delete
  * Perform _Disable_ action on the remaining (or single one) and follow that up with deletion

![AWS CloudFront distributions]({{ site.url }}{{ site.baseurl }}/assets/2017-06-28-static-website-on-s3-and-away-from-wordpress/aws-cloudfront-distributions.png)

> Disabling might take time, keep track of it's status


## Replicate bucket

* Go to
[console.aws.amazon.com/s3](https://console.aws.amazon.com/s3 "console.aws.amazon.com/s3")
  * Select your new, automatically created bucket

* Mark all objects and select _Copy_

![AWS AWS S3 object copy]({{ site.url }}{{ site.baseurl }}/assets/2017-06-28-static-website-on-s3-and-away-from-wordpress/aws-s3-object-copy.png)

* Create a new bucket with *identical* name as your website
  * Select original bucket to copy settings from
  * Enable read for _Object{s, permissions}_ for _Everyone_ in _Manage public permissions_
  * Paste objects with _More_ / _Paste_

> If you want to cover both {,www.} – create other bucket and enable
Redirect requests to original one


## Bucket propagation

* From same, newest bucket, select _Static website hosting_ from _Properties_
  * Choose _Use this bucket to host a website_ and set index (_index.html_ in most cases)
  * Note the _Endpoint_ link in the first line

![AWS AWS S3 hosting endpoint]({{ site.url }}{{ site.baseurl }}/assets/2017-06-28-static-website-on-s3-and-away-from-wordpress/aws-s3-hosting-endpoint.png)

* Select _Bucket Policy_ from _Permissions_ tab
  * Create policy to allow object get, per AWS
    [reference](http://docs.aws.amazon.com/AmazonS3/latest/dev/HostingWebsiteOnS3Setup.html "reference")

    {% highlight json %}
    {
        "Version": "2012-10-17",
        "Statement": [
            {
                "Sid": "PublicReadGetObject",
                "Effect": "Allow",
                "Principal": "*",
                "Action": "s3:GetObject",
                "Resource": "arn:aws:s3:::_____/*"
            }
        ]
    }
    {% endhighlight %}

> Update _Resource_ with your bucket / domain name

![AWS AWS S3 hosting endpoint]({{ site.url }}{{ site.baseurl }}/assets/2017-06-28-static-website-on-s3-and-away-from-wordpress/aws-s3-bucket-policy.png)

> Note that buket policy Versions cannot be arbitrary, but predefined
[values](https://aws.amazon.com/blogs/security/back-to-school-understanding-the-iam-policy-grammar/ "values")


## CNAME the endpoint

* Update DNS record within your domain provider
  * Set retrieved endpoint as a CNAME record
  * (Optionally) add {,www.} as another


# Takeaways

Distributed web-based storage is good, read the small prints and stay in school

