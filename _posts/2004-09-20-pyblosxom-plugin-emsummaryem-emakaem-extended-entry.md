---
id: 757
title: 'Pyblosxom plugin: summary (aka extended entry)'
date: 2004-09-20T04:00:00+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/?p=12
permalink: /?p=757
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "12"
categories:
  - Blogging
  - Python
---
A missing feature of Pyblosxom was the &apos;extended entry&apos; capability that several other blogging systems have. Continuing in my experiment with Pyblosxom, [a second plugin](/software/pyblosxom/summary.py) for Pyblosxom, which comes in at a whopping 32 lines of code (a sign of a decent architecture!).

The markup is relatively simple, and seems to be compatible with the various entry parsers (textile, ReST, etc.):

<pre>Entry title
    (((
    This is the summary
    )))
    This is the full entry.
</pre>

[summary.py](/software/pyblosxom/summary.py)