---
id: 301
title: MacFUSE and sshfs great even with no UI
date: 2007-06-25T17:09:19+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "301"
categories:
  - General
---
Gozer pointed me to a neat way to do development on an linux box from my mac, which is to use [MacFUSE](http://code.google.com/p/macfuse/) and the included sshfs program. It mounts the remote drives as a volume on my mac, and Komodo just edits is as if it&#8217;s a local file. Works great.

It would be nice if there was a tiny bit more UI to sshfs, so that, say, it told you when it successfully mounted the remote drive, but it&#8217;s amazing what UI failings one will tolerate of free software that works as advertised.