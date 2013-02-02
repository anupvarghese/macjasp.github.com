---
layout: post
title: "Octopress on a Raspberry Pi"
date: 2013-02-01 11:10
comments: true
categories: [octopress, raspberry pi]
---
<center>{% img https://dl.dropbox.com/u/22370970/blogimages/RaspberryPi.jpg %}</center>
My Raspberry Pi turned up this week which was greeted with much enthusiasm in my household (only by me, I hasten to add).

I've been tempted to get my hands on one for a while now and with my recent dive in to Octopress it was justification enough to purchase as it gives me a small, lightweight, low powered yet always on server that I can access from my iOS devices and have the ability to update content and play with the layout and plugins, generate and push to Github without having to keep my MacBook Pro powered on 24-7.

It's a super little device and I'll be hacking the hell out of it in the coming months, however in terms of this post and what I've had time to play with to date, installing Octopress has been the initial test of the Pi's power and flexibility.

### Installation
Erik Minkel has an [extremely useful blog post](http://www.erikminkel.com/2012/12/17/host-your-own-jekyll-based-blog-on-a-raspberry-pi/) on how to get Octopress up and running on a Raspberry Pi and it's highly recommended reading if that's what you plan to do, the only issue I personally came across when following the instruction was at the point I attempted a Rake Generate when I hit an error which failed to generate the Octopress blog.

>LoadError: cannot load such file -- openssl

Turns out the install of Ruby Version Manager (rvm) and it's OpenSSL dependancy was the issue, for me I had to replace the 

{% codeblock %}
rvm install 1.9.3 --with-openssl-dir=$HOME/.rvm/usr
{% endcodeblock %}
with
{% codeblock %}rvm install 1.9.3 --with-openssl-dir=$HOME/.rvm/usr/ssl{% endcodeblock %}

The ssl path specifically being where my openssl.cnf resides. I'm unsure if it's related to the latest version of Raspbian Wheezy or not but I followed the steps pretty much to the letter, however once that was cracked Octopress was up and running like a dream on the Pi.

### Github
Migrating the existing Octopress installation from my MacBook Pro across to the Pi was far more straightforward with another good post from [James Saan](http://jamessann.com/2013/01/17/using-octopress-on-multiple-machines-for-mac-os-x/).

His post points out that he had to perform a bundle install at the end, I found I didn't have to go that far, simply setting up Github on the Pi, pushing the latest source from the MBP to Github then cloning and checking out the source back to the Pi was enough to then perform a 'Rake Generate' & 'Rake Deploy'.

I'm now playing with Apps that will allow me to manage the Pi and the Octopress blog while mobile, which I'll share my findings of in a future post.