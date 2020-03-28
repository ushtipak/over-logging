---
layout: post
title: "Terraform Minecraft server"
categories: [terraform, minecraft]
---


Since we're stuck at home – lets bootstrap a Minecraft server to play with our friends

![Terraform Minecraft server]({{ site.url }}{{ site.baseurl}}/assets/2020-03-28-terraform-minecraft-server/terraform-minecraft-server.png)


# @app.before_first_request

You'll need Terraform and a DigitalOcean API key

{%highlight plaintext %}
$ git clone -q https://github.com/ushtipak/terraform-minecraft-server.git
$ cd terraform-minecraft-server/
$ ./init.sh
> retrieve server [1.15.2]
> initialize terraform

Initializing the backend...

Initializing provider plugins...
- Checking for available provider plugins...
- Downloading plugin for provider "digitalocean" (terraform-providers/digitalocean) 1.15.1...

Terraform has been successfully initialized!

You may now begin working with Terraform. Try running "terraform plan" to see
any changes that are required for your infrastructure. All Terraform commands
should now work.

If you ever set or change modules or backend configuration for Terraform,
rerun this command to reinitialize your working directory. If you forget, other
commands will detect it and remind you to do so if necessary.

> usage

echo export DO_PAT="XXXXXXXXXXXXXXXXXXXXXXXXX"
terraform apply                             \
  -var "do_token=${DO_PAT}"                 \
  -var "pub_key=$HOME/.ssh/XXXXXXXXXX.pub"  \
  -var "pvt_key=$HOME/.ssh/XXXXXXXXXX"      \
  -var "ssh_fingerprint=XX:XX:XX:XX:XX:XX:XX"
{% endhighlight %}


# @app.route("/start")

Export your DO token, populate vars and Terraform up

{%highlight plaintext %}
$  export DO_PAT=░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
$ terraform apply                            \
>   -var "do_token=${DO_PAT}"                \
>   -var "pub_key=$HOME/.ssh/░░░░░░░░░░.pub" \
>   -var "pvt_key=$HOME/.ssh/░░░░░░░░░░"     \
>   -var "ssh_fingerprint=░░:░░:░░:░░:░░:░░:░░:░░:░░:░░:░░:░░:░░:░░:░░:░░"

[ ... ]

digitalocean_droplet.minecraft_server: Creation complete after 2m17s [id=186492531]

Apply complete! Resources: 1 added, 0 changed, 0 destroyed.

Outputs:

minecraft-server = 157.230.░░░.░░░
{% endhighlight %}


# @app.route("/stop")

After playing, fire up the `wrapup` to retrieve generated world,
so that it can be (automatically) synced with new server in the future

{%highlight plaintext %}
m@mrmeeseeks:~/live-test/terraform-minecraft-server$ ./wrapup.sh
wrapup start
  rollback [saves/world-2020-03-28-13-32-53-968197585]
  archived [!]
  ip [167.71.░░░.░░░]

[ ... ]

total size is 3,664,223  speedup is 1.00
all done \o/
{% endhighlight %}


Finally:

![Terraform destroy]({{ site.url }}{{ site.baseurl}}/assets/2020-03-28-terraform-minecraft-server/terraform-destroy.jpg)
> src: [Imgflip](https://imgflip.com/memegenerator/)

