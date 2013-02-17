---
layout: post
title: "Migrating and Re-sort Your Instagram Photos on Flickr"
date: 2013-02-16 16:27
comments: true
categories: [instagram, flickr, photography]
description: "Migrate your entire Instagram history to Flickr and re-sort by date taken"
keywords: "instagram, flickr, migrate, history, flickstagram, photos, import, sets, sort, date, photostream"
---
The furore caused by [Instagram's changes in Terms and Conditions](http://bits.blogs.nytimes.com/2012/12/17/what-instagrams-new-terms-of-service-mean-for-you/) late last year actually spawned some useful services as a side effect that enable you to migrate your entire Instagram history across to Flickr.

I personally hadn't got in to the habit of importing each new Instagram photo across to Flickr but lately I've been quite keen on doing so, however for the 200+ photos I've uploaded to Instagram in the past 18 months or so it would be a painful, manual exercise to get them across to Flickr and even then they wouldn't show in my Photostream in the order they were originally taken, something I wanted to avoid. Step forward Flickstagram and Flickrstream. 

### Flickstagram
[Flickstagram](http://flickstagram.org) is a really neat little service, in just a few easy steps{% fn_ref 1 %} it enables you to copy your entire Instagram photo history across to Flickr and puts them in a newly created 'Instagram Photos' set. Whats more it maintains comments, retains geotagging data, converts Instagram hashtags to Flickr tags and records the amount of likes you received from Instagram users within the description field{% fn_ref 2 %}.

### Flickrstream
[Flickrstream](http://flickrstream.webzardry.com) provides the second piece of work required, again by providing a nifty yet simple web service{% fn_ref 3 %} whereby you provide the newly created Instagram Photoset ID from your Flickr account and it sets off re-sorting all those newly imported photos by date taken rather than date uploaded. 

Using these two useful web services I now have my Flickr Photostream as if I'd been importing Instagram from day one (as is evident from the set it created in my own account below){% fn_ref 4 %}.
{% flickr_set 72157632736811854 %}


{% footnotes %}
{% fn %} Flickstagram is secure as it uses OAuth for gaining access to your Instagram & Flickr accounts. Once you're finished with the services, simply remove authorisation.
{% fn %} I personally find this a useless feature.
{% fn %} Again, Flickrstream uses the secure OAuth.
{% fn %} This post is partly to show off this particularly lovely [Octopress plugin](https://github.com/tsmango/jekyll_flickr_set_tag) which I've [forked to display a customisable number of photos from the set](https://github.com/macjasp/jekyll_flickr_set_tag).
{% endfootnotes %}