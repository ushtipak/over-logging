---
title: "The Tealhinator (occupation by RNN)"
categories: [ml, char-rnn]
---

Becoming a Pinter, Garner, Pepytatil Nurse, Chief Infospation Officer or
Tealhinator, as a career choice, seems to be completely fine in the eyes of a
Recurrent Neural Network

The context? Generating new occupations based on existing ones


# Wiki fetch

In order to get existing job titles – Wikipedia was consulted

At start, plan was to write a crawler, but the idea was remised in favor of
a more "cavalier"
[code](https://github.com/ushtipak/rnn-playground/blob/master/fetch-occupations.py "fetch-occupations code")
that utilizes MediaWiki API

To retrieve all known professions, URL walk through initial
[lists of occupations](https://en.wikipedia.org/wiki/Lists_of_occupations "Lists of occupations")
is required. Titles from second level are subsequently fetched, and the special
ones (e.g. _Category:_, _Talk:_) or references to nested lists are removed

{% highlight plaintext %}
import json
import urllib.request

base_url = 'https://en.wikipedia.org/w/api.php?' \
           'action=query&format=json&prop=links&pllimit=500&titles='


def get_links(title):
    resp = json.loads(urllib.request.urlopen(
        base_url + title.replace(" ", "%20"), timeout=10).read(
    ).decode().rstrip())["query"]["pages"]
    return resp[[k for k in resp.keys()][0]]["links"]


for l1 in get_links("Lists of occupations"):
    for l2 in get_links(l1["title"]):
        if not any(c in l2["title"] for c in [":", "List"]):
            print(l2["title"])
{% endhighlight %}

> Handling exceptions (i.e. JSONDecodeError, {URL,HTTP}Error) is barbarically
neglected

The output? First level salvage returns 14 categories (scientific, healthcare,
artistic...), while the second one, final set of all known job
titles, barely gets to 865


# The RNN

In order to mash things up and model a probability distribution – Recurrent
Neural Network implementation from
[Andrej Karpathy](https://karpathy.github.io/2015/05/21/rnn-effectiveness/ "Andrej Karpathy RNN")
(director of AI @ Tesla) was used

Since we've already prepared code to bootstrap Karpathy's RNN
[before](https://ushtipak.github.io/over-logging/ml/char-rnn/2018/01/16/bootstrap-karpathy-rnn.html "Bootstrap Karpathy RNN"),
next step was merely
[gluing](https://github.com/ushtipak/rnn-playground/blob/master/gimme-an-occupation.sh "gluing code")
it to abovementioned Python code for getting input data

Based on the previous experience, _Amazon Linux_ distribution was used (~7-11x
faster processing than remaining _default_ EC2 distros), now in the updated
flavor of AL2

{% highlight plaintext %}
echo -n "> bootstrap rnn ... "
curl -s https://raw.githubusercontent.com/ushtipak/rnn-bootstrap/master/setup-rnn.sh | bash >/dev/null 2>&1
rm /opt/rnn-karpathy/data/tinyshakespeare/ -rf && echo done

echo -n "> fetch occupations from wikipedia ... "
amazon-linux-extras install python3 >/dev/null 2>&1
curl -s https://raw.githubusercontent.com/ushtipak/rnn-playground/master/fetch-occupations.py | python3 > /opt/rnn-karpathy/data/input.txt && echo done

echo -n "> train a model ... "
cd /opt/rnn-karpathy
th train.lua -data_dir /opt/rnn-karpathy/data -rnn_size 128 -batch_size 2 -num_layers 3 -dropout 0.6 -gpuid -1 >/dev/null 2>&1 && echo done

echo "> generate occupations ..."
sudo th sample.lua cv/$(ls cv/ -1t | head -1) -gpuid -1

echo "all done \o/"
{% endhighlight %}


# The ∑

Machine Learning and Neural networks thrive on large input datasets, while
we're dealing with less than 1k records here. Hence, in order to make the most
of it, we're forced to heavily tweak and try various arrangements of hidden
layers, dropouts, RNN and batch sizes

On more than a dozen _t2.medium_ instances with _Amazon Linux 2_ planted, after 
multiple train setups tested, three configurations yielded the most:

| rnn_size | num_layers | batch_size | dropout |
|----------|------------|------------|---------|
|      256 |          5 |          1 |     0.5 |
|      128 |          4 |          2 |     0.5 |
|      128 |          3 |          2 |     0.6 |

Automated job title generation on a new VM, with last row's parameters for RNN,
can be triggered via:

{% highlight plaintext %}
$ curl -s https://raw.githubusercontent.com/ushtipak/rnn-playground/master/gimme-an-occupation.sh | sudo bash
{% endhighlight %}

... producing output of:

![Occupations generated on fresh VM.png]({{ site.url }}{{ site.baseurl }}/assets/2018-02-02-the-tealhinator-occupation-by-rnn/occupations-generated-on-fresh-vm.png)

In all variations, however, generated titles were mostly random. Roughly 10% is
meaningful, which is, having in mind dreadfully terse input, quite expected:

* Runter
* Uthoratist
* Pimicityer
* Newtor
* Phailic Onsinter
* Chestacge Corinner
* Stogh Cliter
* Orertricion Director
* Staeler
* Meddermaderog
* Elergogoot Nursing
* Werhine Pance Thayerist
* Amcrofiin Araryst
* Mashor
* Perecoty Danncer
* Fomiatrilian
* Futhion Suncyror
* Rodugion Mesigner
* Makeniatar
* Chief Buctunel Officer
* Cledus Tanagerer
* Photlac
* Garner
* Pecsion Monicer
* Totrulical Technician
* Ipestralocist
* Foltinist
* Partiol Apant
* Twipo
* Corpossere
* Rushyr
* Sealoet
* Mathor Crale
* Remianecetist
* Pepytatil Nurse
* Dontor Operation
* Dytor Padmer
* Chenm Efficistrator
* Soal Stater
* Tant Daster
* Chief Vart Officer
* Dontore Designer
* Foafer
* Pinter
* Stile Enminderent Aderator
* Gereuttapher
* Aptoroteg
* Bare Telhanicalisirsitc
* Bathuder
* Mirk-tomkar
* Srelhor
* Chief Rimensiol Officer
* Olmhicastor

Still, [author's](https://www.linkedin.com/in/milos-knezevic-43179028/ "author's Linkedin profile")
Linkedin job position is updated with one from the headline – who knows,
_Tealhinator_ might become highly demanded position in close future

