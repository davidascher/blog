---
id: 850
title: 'First pyblosxom plugin: draft mode'
date: 2004-09-20T04:00:00+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/?p=17
permalink: /?p=850
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "17"
categories:
  - General
---
I like to be able to tweak the content of entries without having to worry  
about whether these changes will affect someone&apos;s RSS feed. Since Pyblosxom  
doesn&apos;t have a real &#8220;staging&#8221; model for posts, I wrote this plugin which  
lets me see draft posts using (very weak) password protection, and then  
&apos;turn them on&apos; simply by renaming the file (i.e. `mv draft-foo.txt<br />
foo.txt`). [Enjoy.](/software/pyblosxom/draft.py)