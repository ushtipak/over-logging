---
layout: post
title: "Bootstrap Karpathy RNN"
categories: [ml, char-rnn]
---

There are plenty of resources on Machine Learning and Neural networks, and many
interactive [playgrounds](http://playground.tensorflow.org "TensorFlow playground")
where you can learn and test out ML concepts. If you still need references
before going further – check out the [basics](http://bfy.tw/G9FC "ML basics")

Recurrent neural networks (RNNs), present a artificial NN type in which units
go through a directed cycle, allowing dynamic change of arbitrary sequences
with it's internal memory

Traditional (feed-forward) neural networks treat all inputs and outputs as
independent pieces, which, most of the time, is not the case. Imagine predicting
next character in a word without knowing the preceding one

That's where RNNs come in place, with output of subsequent task directly
dependent of the previous

![ML meeting]({{ site.url }}{{ site.baseurl }}/assets/2018-01-16-bootstrap-karpathy-rnn/ml-meeting.png)

This IO coupling allows RNNs to thrive in handwriting and speech recognition,
in addition to being able to easily train character-level language models

The last part, in layman's terms – if we feed RNN with bunch of text, it'll
model probability distribution of each character in a sequence, allowing us
to create new text snippets, char by char


# Karpathy RNN

When you mix [Torch](http://torch.ch/ "Torch framework") framework and
[Lua](https://www.lua.org/about.html "Lua programming language") code,
good things happen

Mr Andrej Karpathy nicely documented everything in his
[blog](https://karpathy.github.io/2015/05/21/rnn-effectiveness/ "Karpathy blog"),
shared [code](https://github.com/karpathy/char-rnn "Karpathy char RNN on GitHub")
behind it and provided detailed guide on how to prepare and work with his
RNN implementation

Karpathy's blog post covers awesome examples of the effectiveness of his
neural network, accompanied by general guidelines on backpropagation, operating
on sequences of vectors, as well as speeding things up with CUDA on nVIDIA GPUs

Bootstrapping whole enchilada, however, is a bit time consuming and ain't
promptless, so let's automate things a bit


# The bootstrap

[setup-rnn.sh](https://github.com/ushtipak/rnn-bootstrap/blob/master/setup-rnn.sh "RNN bootstrap script")
to the rescue – installing required system packages, fetching everything Torch
related, removing user inquiry from install, retrieving Lua modules
and finally cloning Karpathy's char-rnn repo

Script is designed with 4 initial distros provided by Amazon EC2 in mind:
* Amazon Linux
* SUSE Linux Enterprise Server
* Red Hat Enterprise Linux
* Ubuntu Server

Linux versions and AMIs on which bootstrap was tested, respectably:
* 2017.09.1 (32cf7b4a)
* 12 SP3 (6bc56f13)
* 7.4 (223f945a)
* 16.04 LTS (1ee65166)

On any of these flavors, bootstrap is an oneliner that grabs code from GH and
orchestrates everything needed for char-rnn: 

{% highlight plaintext %}
curl https://raw.githubusercontent.com/ushtipak/rnn-bootstrap/master/setup-rnn.sh | sudo bash
{% endhighlight %}

Other distros, ones not using apt, yum or zypper, can still use boostrap
script by simply adding a flag `./setup-rnn.sh --ommit-dependency-installation`
and the list of system packages required will be displayed on start of it's run 

In any case, after 40-ish bash script completes it's run, Torch framework is
installed in `/opt/torch/`, while the repo ends up in `/opt/rnn-karpathy`

![RNN bootstrap]({{ site.url }}{{ site.baseurl }}/assets/2018-01-16-bootstrap-karpathy-rnn/rnn-bootstrap.png)


# Digits

In order to be consistent and have credible numbers, bootstrap was performed
three times on each of the four _default_ EC2 Linux flavors

![RNN bootstrap on 4 distros]({{ site.url }}{{ site.baseurl }}/assets/2018-01-16-bootstrap-karpathy-rnn/rnn-bootstrap-on-all-four-distros-side-by-side.png)
> upper left to lower right: Amazon, SUSE, RHEL, Ubuntu

Two things are interesting here – time to prepare everything and time to first
processed sample, and here is how distributions stack up:

|                              |||| install |||| checkpoint |
|                              ||||---------||||------------|
| Amazon Linux                 ||||   00:14 ||||      00:06 |
| SUSE Linux Enterprise Server ||||   00:04 ||||      03:13 |
| Red Hat Enterprise Linux     ||||   00:05 ||||      03:15 |
| Ubuntu Server                ||||   00:05 ||||      03:04 |

![RNN bootstrap times]({{ site.url }}{{ site.baseurl }}/assets/2018-01-16-bootstrap-karpathy-rnn/rnn-bootstrap-times.png)
> sherpa blue – bootstrap time; olive – processing first checkpoint

Given times are average of 3 VMs being bootstrapped and finalized processing
1000 cycles, when 1st checkpoint is created

While the bootstrap time varied between 4 and 14 minutes, initial checkpoint
generation lasted between 6 minutes in case of Amazon Linux and ranged between
184 and 195 mins for the remaining three

All instances in test were, of course, identical. 12x t2.micro VMs with same
amount of RAM, vCPUs and storage \(1/1/EBS\)

Checkpoint times are way off chart!

For some reason, Torch runs miraculously slow on all EC2 instance flavors
(not including AWS Marketplace), except Amazon Linux, which is again based
on RHEL, so something is a bit &#x1f41f;y here. Either optimizations Amazon
made are astonishing, or they favor their distro over competition,
resource-wise, under the hood

Any way you prefer, Amazon Linux, in spite of slower bootstrap, is the logical
choice when it comes to char-rnn training, with cycles up to 10x faster than
the rest


# Playtime

Post bootstrap, all that remains is to aim a terminal to `/opt/rnn-karpathy/`,
provide a text source in `data/` subdir (remove `tinyshakespeare/` too) and
fire up `sudo th train.lua -gpuid -1`

Console will display train loss, epoch and cycle duration and this is a great
time to thank the `screen` command and step away from the server, since
modeling will take some time

Processing duration differs based on the dataset size, but for a very rough
estimate – `input.txt` [1.06 MB], from char-rnn repo, on Amazon Linux instance
type t2.micro – takes about 24 hours to complete

![RNN checkpoint files]({{ site.url }}{{ site.baseurl }}/assets/2018-01-16-bootstrap-karpathy-rnn/rnn-checkpoint-files.png)

Amid modeling, assuming you're anxious to see preliminary results, start
another console and examine latest checkpoint file, as soon as cycles round up
on 1k. Head to `/opt/rnn-karpathy/cv` and sample with
`sudo th sample.lua cv/* -gpuid -1`

If, however, want to test pre-provided input right away and generate some of
the Kind Richards paragraphs, Andrej neatly provided beforementioned
`data/tinyshakespeare/input.txt`

Here is the complete rundown on a fresh VM:

{% highlight plaintext %}
curl https://raw.githubusercontent.com/ushtipak/rnn-bootstrap/master/setup-rnn.sh | sudo bash
cd /opt/rnn-karpathy/
sudo th train.lua -gpuid -1
sudo th sample.lua cv/$(ls cv/ -1t | head -1) -gpuid -1
{% endhighlight %}

4 lines and about a day later, last command will provide output similar to:

![RNN sampling]({{ site.url }}{{ site.baseurl }}/assets/2018-01-16-bootstrap-karpathy-rnn/rnn-sampling.png)

RNN, much fun, very wow
