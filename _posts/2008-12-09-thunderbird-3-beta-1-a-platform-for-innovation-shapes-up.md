---
id: 469
title: 'Thunderbird 3 beta 1 &#8211; a platform for innovation shapes up'
date: 2008-12-09T10:02:21+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "469"
categories:
  - Mozilla
  - MozillaMessaging
  - Open Source
  - Thunderbird
---
Today, we&#8217;re [announcing](http://www.mozillamessaging.com/en-US/thunderbird/3.0b1/) our first beta-quality release since the Thunderbird project was re-energized about a year ago. It&#8217;s exciting to see the first in what will be a series of releases aimed at a broader set of testers make it out the door.

In some ways, this is a typical beta &#8212; we&#8217;ve changed a lot of code since Thunderbird 2, and we need a lot of people to tell us if we&#8217;ve made any boo-boos when fixing bugs. It&#8217;s also a _good_ beta in that we&#8217;ve moved the product forward, in part thanks to new capabilities in the underlying Mozilla platform, which gives us faster performance all around, an add-on manager which will be even more useful for Thunderbird users than for Firefox users. We also have important new mail-specific capabilities, including a new &#8220;autosync&#8221; system that gets Thunderbird to download IMAP message bodies early, so they&#8217;re already there when you need them, and a much faster implementation for deleting and moving IMAP messages, which I can&#8217;t imagine living without at this point. The one-click add-to-addressbook is also an elegant and shameless ripoff of the Firefox bookmarking model, which our alpha users love.

As a result, I feel that even for a first beta, Thunderbird 3 is much better than Thunderbird 2, thanks to a lot of hard work by a motley crew of great contributors worldwide, to whom I&#8217;m very grateful. All that and more is described in the release notes, which I encourage beta testers to read.

However, in some other ways it&#8217;s _far from a typical beta_. In particular, unlike the traditional definition of a beta release, we&#8217;re definitely not done making feature changes, including some pretty significant feature work that we expect will be integrated in Thunderbird 3 in later beta releases, some features that will live as optional add-ons, and some experiments which may end up in later releases of Thunderbird or not, depending on the result of the experiments.

I&#8217;ll talk a bit about some of these upcoming attractions, as I&#8217;m quite excited about them (and some more that will have to wait for another post).

First, the **autoconfig** work, which refers to a complete rethink of the account configuration process in Thunderbird. The account &#8220;wizard&#8221; in Thunderbird made sense in the early days, but over the years it has acquired complexity and lost relevance, as email systems have gotten more complex. Unfortunately, if you&#8217;re lucky enough to have a secure email server, the current Thunderbird user interface unjustly punishes you by making you go through 8 pages of questions and you end up with an account which requires manual tweaks before you can check mail. That&#8217;s not good. To deal with this, we have rethought account configuration completely, and came up with a dialog which, when it lands (becomes available by default), should make account configuration really, really easy. It&#8217;s been hard to come up with an elegant minimal user interface that hides all of the complexities of email configuration, but it&#8217;s worth doing it right.

Next up is **tabs**. Thunderbird 3 has a great opportunity to be basically coming up with a tabbed interface at a time in history where we&#8217;ve learned a lot about how tabs work well or poorly. In Thunderbird 3 beta 1, it&#8217;s a fair bit easier to work with tabs than it was in Thunderbird 2 (although many improvements are planned before the final release). For example, it&#8217;s much easier to create new kinds of tabs (the calendar Lightning add-on makes great use of those, for example, as I show below). One simple example of this is Bryan Clark&#8217;s &#8220;glodabook&#8221; add-on, which is a starting point for exploring new ways of navigating the address book.

[<img src="http://farm4.static.flickr.com/3230/3095046580_bf2d087cee.jpg" alt="Addressbook prototype" width="500" height="230" />](http://www.flickr.com/photos/davidascher/3095046580/ "Addressbook prototype")

Next up is **conversations**. Thunderbird&#8217;s default mode saves emails you send in a &#8220;Sent messages&#8221; folder, and emails you receive filed in other folders, typically decided on a per-message basis by the users (more on that below). This is a fine default strategy, but it can make it hard to find related messages if they&#8217;re not in the same place (e.g. messages that are replies to emails you sent, or messages that are part of a long conversation, some of which is in your archive folders, and some of which is in your inbox). Thunderbird 3 includes a powerful search engine (&#8220;Gloda&#8221;) which is designed to let us efficiently find messages that are related, no matter where they are. In particular, it makes it quick to take a message and &#8220;show it in a conversation context&#8221;. This lets you view the messages you sent interspersed with the messages you received, but also messages from earlier in the conversation which you may have archived. This is still experimental, and not enabled by default in 3.0b1, but early results are very promising:

[<img src="http://farm4.static.flickr.com/3219/3095078638_a4f7314238.jpg" alt="Conversation view" width="500" height="448" />](http://www.flickr.com/photos/davidascher/3095078638/ "Conversation view")

Next up, **search.** Part of the Gloda search engine mentioned above is a powerful full-text search engine, which seems to be working quite well so far. Thunderbird search is already better in 3.0b1 than in 2.0 because we&#8217;re more aggressively downloading emails, and doing a better job of finding the downloaded copies. With the new search engine, we&#8217;ll be able to efficiently do searches like &#8220;show me all messages from bryan mentioning &#8216;conversation&#8217; in the body or the subject&#8221;. And we think we can make that easy for users to discover as well:

First we do autocomplete on existing contacts:

[<img src="http://farm4.static.flickr.com/3039/3095085372_119cf6a0d9_o.png" alt="autocompleting contacts" width="367" height="186" />](http://www.flickr.com/photos/davidascher/3095085372/ "autocompleting contacts")

and then encapsulate them in graphical objects to simplify the display:

[<img src="http://farm4.static.flickr.com/3039/3094256973_330bf18de5.jpg" alt="experimental search results view" width="500" height="229" />](http://www.flickr.com/photos/davidascher/3094256973/ "experimental search results view")

On that topic, one of the design topics we&#8217;re exploring is how to make it easier for users to be smarter about search. Thunderbird has always had very powerful search capabilities, but to use them people have to think like database programmers, which most of us aren&#8217;t. We have some plans there to help people build smart searches based on starting with the simple searches people are used to from the web, using suggested sub-searches based on analyzing their search results. Now that we have the search engine in place, we can start to experiment with many different search models, and see what works best.

The last two screenshots are particularly exciting to me because they demonstrate that we can leverage the foundational bits of Thunderbird, and experiment with new ways of working with messages, without disrupting the user experience that Thunderbird 2 that many users are comfortable with. What&#8217;s equally exciting is that these new ways can themselves be platforms for experimentation, whether by us, or by others. One such experimentation topics is conversation visualization and interaction models. Andrew Sutherland [implemented an add-on](http://www.visophyte.org/blog/2008/11/29/ill-be-wanting-that-latte-machine-now/) that shows thread arcs (here using a view that it out of date by a whole week):

[<img class="alignnone size-medium wp-image-150" title="exptoolbar-visophyte-js-thread-arcs" src="http://www.visophyte.org/blog/wp-content/uploads/2008/11/exptoolbar-visophyte-js-thread-arcs-300x124.png" alt="" width="300" height="124" />](http://www.visophyte.org/blog/wp-content/uploads/2008/11/exptoolbar-visophyte-js-thread-arcs.png)

Thunderbird has always been an interesting experimental playground, because of its open source nature and the add-on model. The technology platform in Thunderbird 3 will make it even more so &#8212; 1) we have better technology that allows new ways to slice the data, 2) as we&#8217;re exploring new features through the use of add-ons ourselves, we find out early what changes we need to make to make the platform more extensible, and 3) because we&#8217;re fully leveraging web technologies, something which is a bit new for Thunderbird. In particular, all of the views above build on some of the most compelling advances in web technology, from the canvas widget to Javascript toolkit-based animations (JQuery for now) and modern CSS features.

Finally, last but not least, the **Lightning** calendaring add-on is moving along great. The Thunderbird+Calendar team has made a lot of progress on tackling the stack of issues that made it hard to integrate into the new Thunderbird codebase. We&#8217;re not done yet, but it&#8217;s looking great:

[<img src="http://farm4.static.flickr.com/3115/3094292059_b099806f0b.jpg" alt="calendar tab" width="500" height="319" />](http://www.flickr.com/photos/davidascher/3094292059/ "calendar tab")

There are some other add-ons that some contributors are working on that I&#8217;ll talk about as they get polished and ready for screenshots.

As always, we love to get ideas for interesting new capabilities we can bring to the platform. We&#8217;re focusing on some of the basic capabilities we think are crucial to solving today&#8217;s mail problems, such as search and message management, but it&#8217;s a huge field, and email users are desperate for innovative ideas.

We&#8217;re identifying way more topics of interest than we have time to tackle, so we&#8217;re hoping to reach out to designers to get a broader set of participants helping us with some of the design challenges of a modern approach to messaging, within the context of Mozilla Labs. More on that soon.

Whether you&#8217;re a designer or an implementor, if you want to build new features on top of the views we&#8217;re building, add new kinds of data to add to our database (twitter, facebook, rss, etc.), or new visualizations, do get in touch.

If you&#8217;re interested in the extensions above, and aren&#8217;t afraid to try out code that changes daily, my recommendation is to use an IMAP server, Shredder (the nightly builds of Thunderbird, which are already different than the beta 1 build), and the extensions at the following locations:

  * [lightning nightlies](http://www.mozilla.org/projects/calendar/lightning/download.html) (see links at the bottom, and check out the [lightning nightly updater](https://addons.mozilla.org/en-US/thunderbird/addon/4623))
  * [exptoolbar](http://clicky.visophyte.org/momo/xpis/) (conversation & search results views)
  * [glodabook](http://clicky.visophyte.org/momo/xpis/) (addressbook)