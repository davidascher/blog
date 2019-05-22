---
id: 269
title: 'Lesson learned re: smptlib, hostname and OS X.'
date: 2007-04-27T14:36:26+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2007/04/27/lesson-learned-re-smptlib-hostname-and-os-x/
permalink: /?p=269
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "269"
categories:
  - General
---
To allow Django to send email using smptlib, use _NetInfo Manager_ to create a new _machine_ whose name corresponds to the output of <tt>hostname</tt>, so that <tt>socket.gethostbyname(socket.gethostname())</tt> returns something. (useful for laptops whose local DNS server may not know about their hostname).