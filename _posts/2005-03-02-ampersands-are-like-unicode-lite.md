---
id: 83
title: Ampersands are like Unicode lite
date: 2005-03-02T17:58:24+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "83"
categories:
  - General
---
.flickr-photo { border: solid 2px #000000; }  
.flickr-yourcomment { }  
.flickr-frame { text-align: left; padding: 3px; }  
.flickr-caption { font-size: 0.8em; margin-top: 0px; }

<div class="flickr-frame">
  <a href="http://www.flickr.com/photos/davidascher/5779187/" title="photo sharing"><img src="http://photos4.flickr.com/5779187_cd70d6ecb3.jpg" class="flickr-photo" alt="" /></a><br /> <br /> <span class="flickr-caption"><a href="http://www.flickr.com/photos/davidascher/5779187/">ampersand</a>, originally uploaded by <a href="http://www.flickr.com/people/davidascher/">David Ascher</a>.</span>
</div>

<p class="flickr-yourcomment">
  Ampersands, as I&#8217;ve mentioned before, are really nice letters &#8212; they have a great typographical history, they&#8217;re wonderfully flexible creative outlets for font designers, and they&#8217;re quite useful to the writer.
</p>

However, they sure do get in the way of a lot of code, especially when it comes to HTML and XML toolchains. I&#8217;ve had problems with ampersands in titles of Flickr photos (fixed now AFAICT), and just now hit a problem when trying to export my Bloglines blogroll as an OPML file, as shown here (more correctly, Firefox&#8217;s well-formedness checker complained that the OPML file wasn&#8217;t valid XML).

I&#8217;m thinking that [Sam](http://www.intertwingly.net/blog/2005/03/01/Yahoo-Search-and-I18n) should add an ampersand to his [Iñtërnâtiônàlizætiøn](http://intertwingly.net/stories/2004/04/14/i18n.html) hint, maybe that would help in the long run&#8230;

This post includes another common problem spot, a double-hyphen (one of my typographic tics), which routinely breaks XML processing streams. We&#8217;ll see how this one goes through&#8230;