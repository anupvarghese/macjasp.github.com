---
layout: post
title: "Dynamic DNS Updater for CloudFlare"
date: 2013-03-24 19:42
comments: false
categories: [cloudflare, dyndns, development]
description: "A bash script to automatically update CloudFlare with a dynamically assigned IP address"
keywords: "raspberry pi, cloudflare, dyndns, dynamic dns, dns, bash, script, network, static ip, dynamic ip, ip"
---
Over the weekend I decided to move hosting of this blog from Github Pages to the Raspberry Pi that resides in the bedroom of my home{% fn_ref 1 %}. The site has always been protected by the impressive [CloudFlare](http://www.cloudflare.com/) but that protection is even more critical now I've made that change, it does however present a particular challenge around dynamically assigned IP addresses that ISP's dish out on consumer broadband and fibre networks.
<!-- more -->
<center>{% img https://dl.dropbox.com/u/22370970/blogimages/cloudflare.png %}</center>
CloudFlare needs to be kept informed of the currently assigned IP address that the Pi is sitting behind and although they do offer an API and [a dyndns client](http://robertianhawdon.me.uk/2012/07/17/fixing-ddclient-to-work-with-cloudflare/), it's a little troublesome to get working so I decided the best approach would be a simple bash script.

{% gist 5252855 %}

The script runs perfectly on a Raspberry Pi and all it needs is a simple alteration to include your own domain, CloudFlare Username and API key, then add it to a cron job and it will keep your CloudFlare DNS up to date with the currently assigned dynamic IP at an interval of your choosing{% fn_ref 2 %}.

Any support, issues, comments or feedback are always welcome by getting in touch on [Twitter](http://twitter.com/macjasp).
<br>
<br>
{% footnotes %}
{% fn %}<del>The static pages of this Octopress blog are being served by [Nginx](http://nginx.org/en/) and performance is admirable on the Raspberry Pi.</del> I had to change hosting back to Github Pages after some weird sleeping issues the Pi was experiencing.
{% fn %}I currently have mine set to update CloudFlare every 55 minutes.
{% endfootnotes %}