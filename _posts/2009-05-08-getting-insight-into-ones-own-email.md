---
id: 507
title: 'Getting insight into one&#8217;s own email'
date: 2009-05-08T17:07:40+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "507"
categories:
  - Mozilla
  - MozillaMessaging
  - Software
  - Thunderbird
---
Thunderbird knows a lot about your email. After all, it&#8217;s got access to large amounts of data, and builds sophisticated databases so that it can be very responsive, even when dealing with large folders containing thousands of messages. Wouldn&#8217;t it be nice if we could use this information to extract either faster workflow, or even insight into our email habits?

On Tuesday, as he was slogging through some somewhat antique code in the front-end of Thunderbird, Andrew asked whether Thunderbird&#8217;s &#8220;start page&#8221; was what we wanted it to be, which is Andrew-speak for &#8220;this is broken, we should fix it&#8221;. We&#8217;d actually discussed what to do with that page for a long time, but had focused on other, more infrastructure bits for a while. I decided it was time to dust off those plans, and see what we could do.

First, some background. The &#8220;start page&#8221;, which makes a lot of sense in Firefox, never made a huge amount of sense to me in Thunderbird. In particular, it&#8217;s shown only when a folder is selected, and no message is selected. That&#8217;s hardly a logical time to show the (colorful, pretty, but fairly useless) page we show now. Instead, why not show information about the selected folder, and help people who clearly intended to select a folder, so most likely wanted to do something related to that folder!

We could still use a small part of the pane to display interesting news snippets, as a way of keeping users aware of new developments, such as new add-ons that we want to promote, or Mozilla events. In fact, by making that page _useful_, we&#8217;re more likely to get people to read a sentence or two which might change periodically, as opposed to changing a page that is so big, wordy and useless, that I suspect most users are completely blind to it.

A couple of days later, we have an early patch, which feels pretty compelling to me:

  * It summarizes critical data about the folder (name, number of messages, number of unread messages);
  * if you were recently reading that folder, it points out the last message you were reading, so you can quickly find it again;
  * it shows you a few of the messages that are most likely of interest (because they&#8217;re unread or starred);
  * and finally it gives some information about the activity in the folder: a histogram showing activity over the last 52 weeks, and most prolific authors and most active threads during that same period.

For example:</p> 

<div style="text-align:center;">
  <img src="http://farm4.static.flickr.com/3338/3513500353_f4f9af0212.jpg" alt="Folder summary" border="0" width="500" height="350" />
</div>

</a>

The icing on the cake is that if you hover over an author or a thread title, it will highlight when those messages occurred in the histogram (in this case, the &#8220;An alternate take on HTML 5&#8221; thread). Readers of m.d.platform won&#8217;t be surprised at any of the names that show up above!

There are lots of possible additions: Some of the ones we&#8217;ve thought of include:

  * showing how much disk space is used by the folder
  * showing the &#8220;largest&#8221; messages
  * showing the status of autosync/indexing jobs

Note: this hasn&#8217;t been through a visual design phase yet &#8212; the look will change, once [someone who knows what they&#8217;re doing](http://www.andreasn.se/) has a chance to make it nicer! There&#8217;s also a lot of work to do to make sure that it does the right thing for saved searches, smart folders, etc. And yes, we&#8217;ll make it optional, just like the start page is now.

I&#8217;ve been playing with it for only a little bit, and it&#8217;s fascinating how _interesting_ it is to get some data on one&#8217;s email. For example, I more-or-less follow a small-inbox model, where emails don&#8217;t stay in my inbox if I can avoid it &#8212; they get deleted, or archived. As a result, the sparkline for my inbox is:

</p> 

<div style="text-align:center;">
  <img src="http://farm4.static.flickr.com/3414/3514300538_cf76763561.jpg" alt="inbox sparkline" border="0" width="342" height="54" />
</div>

</a>

which isn&#8217;t as short as it should be, telling me pretty quickly that I have some old messages that need attention. It&#8217;ll be interesting to see what else we learn from these kinds of simple personal analytics.

What other kinds of visualizations, summaries, and analysis would you like to see in Thunderbird, or in add-ons?

**[Update]**: I liked the idea that a commenter suggested of showing what tags were in use in the folder, so I had some fun, first with a &#8220;tagpie&#8221;, which proved mostly useless, just like most piecharts; then with a &#8220;tagdots&#8221; small-multiples visualization:

</p> 

<div style="text-align:center;">
  <img src="http://farm4.static.flickr.com/3603/3520824483_aecf18bbff.jpg" alt="tagpies, tagdots, sparklines oh my!" border="0" width="500" height="421" />
</div>

</a>

I don&#8217;t think the tagpie is worth keeping, but the dots are tempting. As an aside, the [Protovis](http://vis.stanford.edu/protovis/) library really is as easy to use as I&#8217;d hoped.