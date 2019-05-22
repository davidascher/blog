---
id: 115
title: Google vs. Rails
date: 2005-05-06T21:22:51+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/?p=115
permalink: /?p=115
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "115"
categories:
  - Web
---
Interesting to see what happens when two &#8220;well-liked&#8221; communities clash.

Background: Google released [a web accelerator](http://webaccelerator.google.com/), which follows the [HTTP specs](http://www.w3.org/DesignIssues/Axioms#state) (AFAICT), but wreaks havoc with a category of Web 2.0-style apps which, for convenience, ignored the part of the spec having to do with the idempotency of GETs (see Sam Ruby on the topic).

This web accelerator, because it runs in the browser, hence as the logged-in user, drills into sites which, while non spec-compliant, were considered &#8220;OK&#8221; because the rest of the web infrastructure (spiders, caching servers, etc.) weren&#8217;t logged in, hence weren&#8217;t exposing the flaw.

Some Ruby on Rails apps by the 37Signals crew was [vulnerable](http://37signals.com/svn/archives2/google_web_accelerator_hey_not_so_fast_an_alert_for_web_app_designers.php), with the web accelerator causing data loss.

Google is following the spec, the Rails folks say [&#8220;yeah, but the world hasn&#8217;t been following the spec for years&#8221;](http://www.loudthinking.com/arc/000454.html). Typical [prescriptive vs. descriptive](http://www.usingenglish.com/articles/prescriptive-descriptive-grammar.html) argument, but in a a community which has stuck to standards over convenience for a decade (in great part in a battle to the death with Microsoft).

It&#8217;s quite a fascinating debate, one that [Sam predicted](http://www.intertwingly.net/blog/2005/03/16/AJAX-Considered-Harmful). Myself, I hope that Google adjusts the program to be less destructive (for the sake of the users) but sticks to the principle of the sanctity of the spec, and that the Rails folks use their considerable smarts to find a way to route around the limitations of the spec.