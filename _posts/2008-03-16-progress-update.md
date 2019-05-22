---
id: 400
title: Progress Update
date: 2008-03-16T15:14:24+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "400"
categories:
  - Mozilla
  - MozillaMessaging
  - Software
  - Thunderbird
---
I just realized that I forgot to blog about some of the exciting things going on in Thunderbird land these days.

First, I&#8217;m very happy to announce that another engineer has signed up to work full time on Thunderbird &#8212; Mark Banner, aka Standard8 on IRC. Mark is well known to the Mozilla community, as someone who&#8217;se been a steadfast contributor for years, doing important behind-the-scenes work, especially on the address book &#8212; a part of Thunderbird which I expect will become more important over the next few releases. It&#8217;s great to have Mark on board, even though he&#8217;s not officially starting until next month. One of the projects that Mark will finally have time to push on is to beef up the test automation framework and help drive better test coverage for the codebase, which is a crucial step to allow the refactoring we want to do, and facilitate a more agile development model.

Second, I&#8217;m equally happy to announce that Rick Tessner has joined as a part-time build engineer, helping with build automation, release automation, etc. If you&#8217;re interested in build engineering, I highly recommend reading [John O&#8217;Duinn&#8217;s blog](http://oduinn.com/blog/category/mozilla/). John&#8217;s team has taken on the task of bringing some sanity to the Mozilla build system while Firefox 3 is finishing. To use an analogy my ActiveState colleagues will remember, it&#8217;s like repairing an aircraft fuselage in flight. John&#8217;s team has made great strides in improving build and release automation for Firefox 2 (and 3), and Rick will work with them to improve build and release automation for Thunderbird 2 and 3.

Which brings me to the topic of release planning for security updates, a topic which may be puzzling to people who don&#8217;t follow the process closely. Here&#8217;s how it works, from my newbie perspective.

Mozilla regularly ships security updates to both Firefox and Thunderbird (these days, they&#8217;re called 2.0.0.x), with a schedule which is the result of analyzing:

  * the number and criticality of the security fixes that are available
  * the likelihood of people being impacted (taking into account things like whether the default configurations are vulnerable)
  * the frequency of recent releases (as users get &#8220;update fatigue&#8221; and updating too often may in fact result in more exposure).
  * the unavoidable challenges of scheduling the activities of the people needed to produce a quality release, including developers, build engineers, QA engineers, release managers, localizers, etc.

This is further complicated by the fact that, as of now, there are three product lines which end up relying on many of the same staff, especially in the Build & QA stages (Firefox 2.0.0.x, Firefox 3, and Thunderbird 2.0.0.x). For now, MoCo staff are primarily responsible for the Thunderbird security releases, with great people like Dan Veditz, Sam Sidler, Al Billings, Nick Thomas, and more pushing those through.

What that means in practice is that we have to make some tough choices. For example, there&#8217;s a Firefox 2.0.0.13 release coming up, which fixes some security bugs. Some of those are in the part of the code that is shared with Thunderbird. There will therefore be a matching Thunderbird 2.0.0.13. The only question is when. At the scheduling meeting, it was clear that the ideal scenario (near-simultaneous security releases for Firefox and Thunderbird) was simply impossible, mostly because of resource contention. Some of those resource contentions are due to not enough automation for the Thunderbird release process, and some of it is the consequence of not enough people with the right training &#8212; one of the factors that led to the creation of Mozilla Messaging. After careful weighing of the various options, we all agreed that Thunderbird 2.0.0.13 will have to release [several weeks](http://wiki.mozilla.org/Releases) after Firefox 2.0.0.13. The strange thing is this: everyone on the call was unhappy about it. But I actually feel that the choice was the right one, _given the circumstances_.

For example, some of the security fixes can only be exploited using JavaScript. Because the vast majority of Firefox users have JavaScript enabled (because it&#8217;s the default, because it&#8217;s a key part of the web experience), a Firefox user is more at risk for that kind of issue than a Thunderbird user (Thunderbird doesn&#8217;t ship with JavaScript enabled by default). We could delay releasing Firefox until Thunderbird was ready, in the interest of mitigating the risk of someone using knowledge from the Firefox release to try and attack Thunderbird users. But that would mean leaving over a hundred and fity million users vulnerable. So, applying the correct math, we release Firefox security updates as soon as possible, and Thunderbird security updates as soon as possible. This time, we were hit by the extra whammy that some of the people needed for the Thunderbird build are also doing work that&#8217;s critical to the Firefox 3 release, which itself will boost security on the net. That&#8217;s unfortunate, but I still think we should be proud of these tough choices.

The process that we go through when scheduling these releases is to try to optimize a global metric which I think of as &#8220;public safety&#8221;. And when we do that well, the outcome is one that I can live with because 1) the global metric is the one to pay attention to, and 2) Thunderbird benefits so much from Firefox that any scheduling slight is &#8220;immaterial&#8221; in the grand scheme of things. Even just looking at the (relatively) narrow topic of security, it&#8217;s incredibly valuable to have the ear (and attention, and interest) of security folks like Dan Veditz, who truly care about Thunderbird. Beyond security, Thunderbird gains daily from the improvements in the platform, and even features built &#8220;for&#8221; Firefox 3 like the new download manager will be even more valuable in Thunderbird. The list goes on.

Naturally, living with the best possible schedule given constraints isn&#8217;t \_enough\_, and that&#8217;s why we&#8217;re hiring the best people possible to:

  * reduce the amount of manual work for test, build or release,
  * increase test coverage and code quality, and
  * build out parallel build, QA and release processes for Thunderbird.

Which loops back to Mark and Rick whose work will, in time, help alleviate these issues. Note that while I&#8217;ve primarily talked about the 2.0.0.x security updates, the vast majority of what Rick will do in release automation will be applicable straight away to future Thunderbird 3 releases. Mark Banner&#8217;s test automation work is going to apply to Thunderbird 3 nightly builds, for example.

I&#8217;ll be away from the net for a while, but when I get back I&#8217;ll write a more detailed introduction to the people working on Thunderbird, both staff and contributors.