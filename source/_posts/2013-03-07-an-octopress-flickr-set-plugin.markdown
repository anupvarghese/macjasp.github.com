---
layout: post
title: "An Octopress Flickr Set Plugin"
date: 2013-02-27 16:27
comments: false
categories: [photography, development]
description: "A forked Octopress plugin to display Flickr sets in a page or post"
keywords: "flickr, photos, sets, octopress, posts, plugin, ruby"
---
While I was in the process of setting up and theming this site I envisaged writing a post that documented the migration of my Instagram photos to Flickr{% fn_ref 1 %}, the idea being that I would then embed the newly migrated Flickr photo set in said post on this Octopress powered blog.
<!-- more -->

I wasn't entirely sure whether I'd have to write my own plugin to do so or if I'd be lucky enough to find one already out there and I was thankfully saved the work after coming across a [great little Octopress plugin by tsmango](https://github.com/tsmango/jekyll_flickr_set_tag) that did almost everything I was after, however I felt it could be improved upon so decided to fork the project and make some changes of my own.

- Firstly it returned all photos in a set, the Flickr API can return up to 500 photos at a time and that wouldn't display too well in a blog post, so I've added a new parameter which allows you to configure the amount of photos that are returned by changing the newly created 'per_page:' setting in the _config.yml to a number of your choice.

- Secondly, clicking a photo thumbnail would take you directly to the source image while I personally thought it more sensible if it took you to that individual photos full Flickr page instead, another parameter is required for this called 'user:' in which you enter your own flickr userID. 

Below is the result of those changes and the amended plugin is available to install [from my Github repository](https://github.com/macjasp/jekyll_flickr_set_tag).
<center>{% flickr_set 72157629183418955 %}</center>
<br>
<br>
{% footnotes %}
{% fn %}I scrapped this idea for a post but check out [Flickstagram](http://flickstagram.org/) if you're planning on doing something like this yourself.
{% endfootnotes %}