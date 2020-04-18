---
title: "Pigeon Facts as a Service"
categories: [bash]
---

Friend is into pigeons, so the only thing that makes sense is to buy a domain
with his name and create a **PFaaS** (Pigeon-Facts-as-a-Service), so that he
can flaunt in front of his other, pigeon loving friends


# Means of production

Although there are plenty of frameworks that could be used to bootstrap REST
API, Bash shell with `nc` was chosen, based on it's supreme benchmarks

![Netcat benchmark]({{ site.url }}{{ site.baseurl}}/assets/2019-03-10-pigeon-facts-as-a-service/netcat-benchmark.png)

> Connections during time – constant output (1) from `nc`, no fluctuations


Netcat is handling the routing, with responses passing through a FIFO pipe

{% highlight plaintext %}
cat "${PFAAS_PIPE}" | nc -n -l -p ${PFAAS_PORT} > >(
  while read l; do
    # [ ... ]
  done
)
{% endhighlight %}


Facts are read from a separate file and fed into an array that is used to show
either a random or a specific fact (`/api/fact/{id}`)

{% highlight plaintext %}
IFS=,$'\n' read -d '' -a FACTS < ${PFAAS_FACTS}
# [ ... ]
id=$RANDOM
let "id %= ${#FACTS[@]}"
fact="${FACTS[${id}]}"
{% endhighlight %}


After a GET request is parsed (and optional fact ID retrieved), either the
target fact or a random one will be JSON marshaled and returned to the client


# Obligatory benchmark

Apache Bench shows neat results for one user / one request at a time,
expectedly breaking when either consecutive requests (`nc` is not fond of
RFC 2616's "Connection: close") or concurrent ones appear

{% highlight plaintext %}
$ ab -n 1 -c 1 -k -H "Content-Type: application/json" \
                   http://localhost:1805/api/fact/ | tail -n+15 | head -4
Concurrency Level:      1
Time taken for tests:   0.015 seconds
Complete requests:      1
Failed requests:        0
{% endhighlight %}


> Apache Bench – 1 req

{% highlight plaintext %}
$ ab -n 2 -c 1 http://localhost:1805/api/fact/ > /dev/null
apr_socket_recv: Connection refused (111)
{% endhighlight %}

> Anything above one (w/o increasing concurrency level)


# Pigeon facts to go

[Code](https://github.com/ushtipak/pfaas) and a complementary
[Docker image](https://hub.docker.com/r/ushtipak/pfaas) are available, if you
prefer to have it running on-prem

For those that simply want to expand their vast pigeon knowledge, feel free to
checkout a random fact on friend's
[PFaaS](http://pfaas.nenadcolovic.com:1805/api/facts)

If you get an error, another user is accessing it, try in a sec

![PFaaS in action]({{ site.url }}{{ site.baseurl}}/assets/2019-03-10-pigeon-facts-as-a-service/pfaas-in-action.gif)
