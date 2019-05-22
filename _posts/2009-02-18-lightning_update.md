---
id: 482
title: Lightning-in-Thunderbird status update
date: 2009-02-18T14:10:28+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "482"
categories:
  - Lightning
  - Mozilla
  - MozillaMessaging
  - Thunderbird
---
For some time, we (the Thunderbird release-drivers) have been exploring how to best integrate calendar functionality into Thunderbird.  Time for an update.

The current plan is to work with the Lightning Add-on community to make a version of it available as an add-on to Thunderbird 3 after we ship later this year.  This is a change from our initial plan of integrating all of Lightning into Thunderbird by default.  Our thinking has evolved based on both technical and product reasons:

  * the calendar team has had a tough time of figuring out how Lightning needed to change to integrate optimally in Thunderbird, in large part because Thunderbird 3 itself has been somewhat of a moving target &#8212; Thunderbird&#8217;s interface model is still shifting, which is certainly hard on add-on developers

  * partially as a result, there&#8217;s a fair amount of work left to do on Lightning before it&#8217;s ready to present as part of the core product.  For example, it&#8217;s not yet possible to selectively enable the task management or calendaring features; the account configuration is a bit too hard to get right for novice users; error messages are still too cryptic &#8212; that sort of thing.

  * looking at Lightning as an addition to the core project, it would represent a lot of new, complex code, with a lot of implied maintenance &#8212; we don&#8217;t have enough developers on hand to be able to take on that commitment at this stage.  See [Philipp&#8217;s post](http://weblogs.mozillazine.org/calendar/2009/02/calendar_project_at_a_critical.html) on this topic for more information, especially if you&#8217;re keen to help out.

  * we try to avoid feature changes in between major releases, and limit minor updates to security fixes.  This would mean that feature changes to Lightning would have to wait for the next major release of Thunderbird.  That would be a real shame.

  * more generally, we recognize that different users need different kinds of calendaring solutions.  Just as there are more and more messaging systems, there is a growing diversity in calendar usage models, such as web calendars, stand alone clients, and calendar and event applications on social networking platforms.

Given all this, we feel the best plan is to take advantage of our add-on ecosystem, to allow a variety of calendaring features to evolve, and to allow Lightning to evolve at whatever pace is best for it, less tied to Thunderbird&#8217;s schedule.  Lightning is by far the most popular and important Thunderbird add-on, and we&#8217;re going to see what we can do to make it better and more successful, both on the development side, as well as on the promotion side.  Also, thanks to Thunderbird 3&#8217;s new add-on manager, it will be easier for users to find and install, which I expect will lead to even greater adoption.

In short: expect a version of Lightning that will work with Thunderbird 3; expect it to have more frequent releases than Thunderbird major release numbers; talk to philipp if you want to help!