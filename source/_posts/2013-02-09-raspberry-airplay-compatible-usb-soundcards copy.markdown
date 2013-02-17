---
layout: post
title: "Raspberry Pi, Airplay and USB Sound Cards"
date: 2013-02-09 23:23
comments: true
categories: [raspberry pi, airplay, airpi]
description: "A cheap and compatible USB sound card for the Raspberry Pi to use as an AirPlay Receiver"
keywords: "airplay, raspberry pi, usb, sound card, dynamode, airpi, raspian, wheezy, airport express"
---
For a £25 piece of hardware I'm getting a heck of a lot of value from my newly purchased Raspberry Pi, its a powerful piece of tech.

Not only is it now acting as my [Octopress staging server](http://carmo.org.uk/Octopress-on-a-raspberry-pi/) but I now have it performing as an [AirPlay receiver](http://jordanburgess.com/post/38986434391/raspberry-pi-airplay) plugged directly in to my bedroom speakers, something I would normally have had to spend upwards of £70 on if I bought an Apple Airport Express. 

### Compatible USB Sound Cards

<center> {% img https://dl.dropbox.com/u/22370970/blogimages/pi_usb_soundcard.jpg %} Raspberry Pi & Compatible USB Sound Card</center>

It seems the major challenge with the Pi when it comes to audio is the onboard sound card, with it being analog it really isn't up to scratch and has major background hiss and pops with noticeable degradation in sound quality, so finding a compatible USB sound card is essential when wanting to use the Pi for any audio related project.

There's not a huge amount of assurance out there on blogs and forums as to which sound cards are compatible and I personally didn't want to spend a huge amount when taking a punt on finding one, but I took a gamble with a £6 Dynamode 7.1 USB sound card{% fn_ref 1 %} from my local PC World store and with a minimal configuration tweak{% fn_ref 2 %} I've been able to get high quality audio through the Pi and have glorious music streaming from my Apple devices. 

If you're unsure on what sound card to use, or just want something extremely cheap then I can highly recommend the Dynamode. 

{% footnotes %}
{% fn %} [Here's a link to one at Amazon UK](http://www.amazon.co.uk/Dynamode-Channel-USB-Sound-Card/dp/B004FE6UCE).
{% fn %} [There's plenty information around on how to make a USB sound card the default on the Pi](http://elinux.org/RPi_VerifiedPeripherals#USB_Sound_Cards).
{% endfootnotes %}