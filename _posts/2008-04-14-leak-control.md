---
id: 413
title: Leak control!
date: 2008-04-14T22:08:44+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "413"
categories:
  - Mozilla
  - Thunderbird
---
Thunderbird work is all about leaks these days, of various kinds:

  * A [study at CMU](http://www.cs.cmu.edu/~vitor/cutonce/userStudy.html) to test [an extension](http://www.cs.cmu.edu/~vitor/cutonce/cutOnce.html) that suggests people you might have forgotten to include in an email, and whether you might be leaking something to people you didn&#8217;t intend to include (via [Shawn Wilsher](http://shawnwilsher.com/archives/150)), 
  * A [related post](http://dutherenverseauborddelatable.wordpress.com/2007/11/01/mls-for-thunderbird-or-o-gosh-perhaps-i-shouldnt-have-sent-confidential-info-to-a-public-mailing-list/) I&#8217;ve been meaning to refer to for a while from David Teller about adding MLS (multi-level security) to Thunderbird.
  * Only linguistically related work from Mark Banner on adding metrics to [detect memory leaks](http://ccgi.standard8.plus.com/blog/archives/9) in the Mail/News code that Thunderbird relies on.