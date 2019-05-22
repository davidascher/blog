---
id: 310
title: A Facebook Story
date: 2007-08-17T16:00:35+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "310"
categories:
  - General
---
I&#8217;ve been quiet lately. One of the reasons is that I&#8217;ve been working hard on a facebook application, which we &#8220;unveiled&#8221; on Wednesday. Now it&#8217;s live (although still alpha), so I have a bit of time to talk about it.

### Why build a facebook app?

We&#8217;re a [technology company](http://activestate.com/). When someone announces a new platform for application development, we naturally poke around it and try to figure it out. In practice, we do that for every platform we can get our hands on. (Note to Apple: when iPhones work in Canada, we&#8217;ll poke around with that too!). For Facebook, it seemed clear that in addition to the groundswell of interest from all kinds of quarters, that just reading the docs wasn&#8217;t going to truly teach us what the F8 platform is like. And I&#8217;m not just saying that because the docs didn&#8217;t match the code! A social platform is different, and requires real users using a real app to teach the developer what works and what doesn&#8217;t.

So we decided that we&#8217;d build the best facebook app we could in a relatively short amount of time. Not a silly little amount of time, because it&#8217;s clear what that leads to &#8212; lots and lots of mostly trivial, ugly, and useless apps. I happened to have a great engineer, a great product designer and a super-talented graphic designer on hand, so we tried to raise the bar (and then we got a great marketer to help out as well).

### What kind of app to build

Figuring out what app fits in a platform is a messy process, at least in our hands. We wanted something that leveraged the social graph which is central to the platform, but we wanted something that provided real value to users. After a fun process of ideation and triage, we zeroed in on an idea which started off as the &#8220;anti-calendar&#8221;. While online calendars focus on when you, the user, have stuff that you have to do, the anti-calendar tells your friends when you are available. That core idea evolved into what we call Up4, which aims to tell your friends that you&#8217;d be interested in (&#8220;up for&#8221;, get it?) something, sometime, somewhere. If you have a Facebook account, [check out the app](http://www.facebook.com/apps/application.php?id=2435391854). If you don&#8217;t, here&#8217;s a screenshot:

![](http://ascher.ca/images/up4_screenshot.png) 

There&#8217;s lots more to say about what apps work in something like Facebook, but the margins on this page are too small.

### How was the app-building experience?

Building the app was a fascinating and frustrating exercise.

From a pure technology point of view, the infrastructure &#8220;kinda works&#8221; (we used [Django](http://www.djangoproject.com) as the back-end, using the really nice [facebook.py module](http://code.google.com/p/pyfacebook/) as the bridge). We hit some simple bugs in the facebook module, but as it was open source, we were able to fix it and get the patches committed. We hits bugs in Facebook, and had to resign ourselves to &#8220;filing&#8221; bugs and then working around them. The biggest beef I have with F8 is that they play fast and loose with standards, meaning that your expectations about HTTP & REST, HTML, CSS and JavaScript have to be checked at the door, since what ends up served to the user&#8217;s browser will be a sometimes mysterious transformation of what your server published. It&#8217;s clear that Facebook both has to deal with a significant security threat, and that it&#8217;s still early in the development of F8.

There was equal fascination and frustration on the product design front. For most of the time we were building the app, using JavaScript outside of iframes was verboten. Iframes are incredibly limiting at well, and naturally making things work in IE also limits what we can do. So while our instinct was to build all kinds of ajaxy goodness, the technical limitations, combined with the general framework of a facebook app forced all kinds of compromises. The very real limits on data sharing and the like also made &#8220;obvious&#8221; features impossible to implement. I&#8217;m sure many of those limitations will fade over time as the Facebook developers figure out how to loosen the restrictions without relaxing security, but for now, it still feels very straight-jackety.

As an application developer, there are a lot of gaps that are both obvious and hard for anyone other than Facebook to fix. For example, testing a social application requires considering what people with different relationships interact with the app. Testing that requires multiple identities. But the terms of service say that you can&#8217;t create multiple identities. Luckily, we have a bunch of people on staff with facebook accounts! It&#8217;s also quite hard to build a test harness which lets you simulate how your app will behave in facebook without building a facebook clone (which was a bit out of scope!). The list goes on.

The most recent and spectacular challenge we had was when our marketing lead, an avid Facebook user, had built a Facebook group to communicate with a group of people who&#8217;d signed up to be our alpha testers. Due to apparent bugs in the group communication mechanisms, he tried to send them each a message to let them know that the app was live and that they should go ahead and start testing it. This promptly triggered a spam filter in facebook, and got his account banned. An appeal with customer service failed miserably (apparently they don&#8217;t seem to even review appeals), and it looked for a while like he had lost his personal Facebook account (with all its data) because he was trying to do his job as a Facebook application developer. Not good. Luckily, friendly folks on the #facebook IRC channel, including a Facebook employee, helped to get that resolved. It did drive home the point that we&#8217;ve all felt that there&#8217;s something problematic about the complete ownership of personal data by Facebook. That control, combined with a hair-trigger banning without warning and a probably overwhelmed appeals process, is scary.

### What&#8217;s the feedback?

The feedback we got from our friends has been great. Even more special is the early feedback we&#8217;re getting from people we don&#8217;t know:

> &#8230; By FAR the best looking application on Facebook. Awesome job! 

> &#8230; I love this app &#8212; it&#8217;s great b/c it actually has the potential to take facebook connections one step further from virual to real, with people being able to be connected on a whim. &#8230; 

and it&#8217;s great to get this kind of feedback from other facebook developers on IRC and in private messages:

> &#8230; your app is awesome  
> &#8230; really nicely designed  
> &#8230; yeah a really slick ui  
> &#8230; seriously, your app is the nicest looking app to date  
> &#8230; great to see people taking the time to put quality like that together rather than just rushing out an app  
> &#8230; very very pretty  
> &#8230; check it out, hands down the nicest looking app to market yet  
> &#8230; Looks nice 🙂  
> &#8230; such a nice looking app needs to be out there 

This feedback goes straight to Luke, our designer, who, as usual, is able to impress people on a glance of his work. We&#8217;ll see how the feedback on usability comes in over the coming weeks, but it&#8217;s a good start!

### Lessons learned

That part will have to wait. Everyone else has already started on in a little friday afternoon celebration of ActiveState&#8217;s tenth anniversary, I&#8217;ve had four hours of sleep, and I&#8217;m going on vacation next week, with only occasional net access. So be kind to the app, don&#8217;t crash the server in my absence except during Norwegian working hours, but do send us feedback via the [app&#8217;s discussion page](http://www.facebook.com/apps/application.php?id=2435391854).