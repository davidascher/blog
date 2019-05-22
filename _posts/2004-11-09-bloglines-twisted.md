---
id: 46
title: 'Bloglines &#038; Twisted'
date: 2004-11-09T14:44:43+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "46"
categories:
  - Blogging
  - Computing
  - Python
---
Interesting bit found in my webserver access logs:

`209.67.209.74 - - [08/Nov/2004:00:07:32 -0500] "GET /blog/index.cgi/?flav=rss HTTP/1.0" 404 24542 "-" "Twisted PageGetter"`

Googling &#8220;Twisted PageGetter&#8221; confirms that it&#8217;s a spider that comes with Twisted Python. Once more, Python&#8217;s in the web spidering business, this times w/ [bloglines](www.bloglines.com).