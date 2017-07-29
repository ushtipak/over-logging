---
layout: post
title: "AWS Lambda colleague name generator"
categories: [aws, lambda]
---

Our _original_ colleague's name was Tomislav or Miroslav, I believe

Time passed since he started receiving daily *slav names upon arrival in the office...
Why? Noone remembers exactly, but after a few days, it was obvious that the
process needed to be automated

Good friend of mine created music "artist" name generator and shared it with
the world as a legendary <a href="http://polumenta.zardina.org/" target="_blank">
Polumenta generator</a>. He <a href="https://github.com/vl4dimir/polumenta"
 target="_blank">open-sourced</a> it, so shameless code stealing was obviously
the way to go

Script was Python-ized with minor adjustment of adding another ponderized last
character, before necessary "слав" ending, based on distribution of actual
names of it's kind. Base64 from indexed 1-bit palette image was supplied along
– all ready for FaaS


# AWS Lambda

Creating a λ function is trivial – from given _hello-world_ example, without
initial trigger, apply <a href="https://github.com/ushtipak/shiftoslav/blob/master/shiftoslav.py"
 target="_blank">code</a> gently

![AWS Lambda code]({{ site.url }}/assets/aws-lambda-code.png)

Based on above `lambda_handler` function name – and the fact we're using Python –
here is the overview of configuration options

{% highlight yaml %}
Runtime: Python 3.6
Handler: lambda_function.lambda_handler
Role: Choose an existing role
Existing role: service-role/polygon-shiftoslav
Description: Generate Shift-O-Slav name

Memory (MB): 128 MB
Timeout: 3s
DLQ Resource: None
VPC: no VPC
Enable active tracing: [ ]
KMS key: (default) aws/lambda
{% endhighlight %}

In order to verify that function returns correct JSON with name and UTF-8 chars,
use empty curly brackets for _Input test event_ and validate output

{% highlight json %}
{
  "name": "Гомеслав"
}
{% endhighlight %}


# AWS API Gateway

In order to have an URL to invoke the function from, GET request method
integration is needed. By default API Gateway returns JSON, so making it
present HTML requires a bit of extra work

Three out of four pillars of non-intuitive method execution setup (_Method
Re{quest,sponse}_, _Integration Re{quest,sponse}_) need to be tweaked in
order to achieve that

![AWS API gateway method execution]({{ site.url }}/assets/aws-api-gateway-method-execution.png)

Changes on the _Integration Request_ are basic

{% highlight yaml %}
Integration type: Lambda Function
Use Lambda Proxy integration: [ ]
Invoke with caller credentials: [ ]

Body Mapping Templates:
  Request body passthrough:
    When no template matches the request Content-Type header
{% endhighlight %}

_Integration Response_, however, demands more alteration. Within HTTP 200
response set _Content-Type_ and define body mapping so that function return
is parsed as part of HTML

{% highlight yaml %}
Lambda Error Regex: default
Content handling: Passthrough

Header Mappings:
  Content-Type:
    'text/html; charset=utf-8'

Body Mapping Templates:
  application/json:
    #set($inputRoot = $input.path('$'))
    <!doctype html>
        <meta charset=utf-8>
        <head><title>ShiftOSlav</title></head>
        <body><center>
            <p><img src="data:image/png;base64, iVBORw0KGgoAAAAN [ ... ]
                         5wAAAABJRU5ErkJggg==" alt="Shift-O-Slav" />
            <p><h1>$inputRoot.name</h1>
            </center></body></html>
{% endhighlight %}

> Content-Type is entered **with** single quotes and all JSON fields from
lambda are accessed via `inputRoot._`

![AWS API gateway integration response]({{ site.url }}/assets/aws-api-gateway-integration-response.png)

Last step before hitting _Actions / Deploy API_ is adding "Content-Type" within
_Method Response_ and modifying response body for HTTP 200

{% highlight yaml %}
Response Headers for 200:
  Name: Content-Type

Response Body for 200:
  Content type: application/json
  Models: Empty
{% endhighlight %}


# Shift-O-Slav

Entry point for the function can now be found under _Invoke URL_ on the
_Stages editor_, after API has been succesfully deployed.
All that's left is to enjoy fresh FaaS
<a href="https://o5bsrqjdtl.execute-api.us-east-1.amazonaws.com/live"
 target="_blank">Shift-O-Slav name generator</a>

![Shift-O-Slav]({{ site.url }}/assets/shift-o-slav.png)

