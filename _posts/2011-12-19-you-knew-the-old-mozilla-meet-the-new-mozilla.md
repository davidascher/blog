---
id: 672
title: You knew the old Mozilla, meet the new Mozilla
date: 2011-12-19T20:05:05+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "672"
categories:
  - Mozilla
---
One of the notable things about working at Mozilla over the last few years right now is that our aims have gotten much more ambitious, but perception moves slower than reality, even among people who spend every working hour working on the project. I&#8217;ve been privileged enough to have a lot of conversations with a lot of people, and to see an evolution in the thinking that motivates our priorities. I&#8217;ve also been unfortunate enough to see and participate in high-emotion conflicts, which emerge from the disconnect between various individuals&#8217; perceived priorities. I&#8217;m hoping that this post can explain the high level reasons for our current initiatives & why they matter, and maybe help get people past short-term conflicts.

### History

For many years, the area that Mozilla needed to focus on was clear: to save the promise of the web, we needed to make a fast and useful browser that didn&#8217;t get in the users&#8217; way, and get lots and lots of people to adopt it. This was (and is) a product play, which implies is that success would be determined by what real people would choose to use based on the real choices in front of them. And the people demanded high quality code, zarro boogs, security, etc., but they mostly demanded compelling experiences that solved their problems. In the case of the browser wars, the outcome has been pretty good for society, if slower than we&#8217;d have liked: standards have evolved, browsers got better and faster, and websites got more interesting (I&#8217;ll note in passing that cross-browser dev work is still way too painful).

### Rethink

While that fight is far from over, we&#8217;re now at a distinct point in the evolution of the web, and Mozilla has appropriately looked around, and broadened its reach. In particular, the browser isn&#8217;t the only strategic front in the struggle to promote and maintain people&#8217;s sovereignty over their online lives. There are now at least three other fronts where Mozilla is making significant investments of time, energy, passion, sweat & tears. They&#8217;re still in their infancy, but they&#8217;re important to understand if you want to understand Mozilla:

The first such effort is, in some ways, &#8220;lower in the stack&#8221; than the browser. We started an ambitious exploration called [Boot to Gecko (B2G)](https://wiki.mozilla.org/B2G), which I don&#8217;t yet understand well enough in detail, but which is clearly trying to ensure that there are realistic options for mobile devices which bake in the right values as low as possible in the stack. As I discussed in my last post, the verticalization of the internet means that we&#8217;re heading towards a world where who you get your phone from will determine way too much about how you can experience the internet. B2G is a bold exploration tackling the operating system layer of that world.

The two other such efforts are higher-level in the stack, specifically in areas which I&#8217;ve been following closely: user identity, and apps. Both of these are spaces where the shape of the real world ergonomics & economics of the internet have managed to completely sneak around the &#8220;traditional&#8221; world view of browsers & websites.

### User-centric Identity on the web

For identity in particular, it&#8217;s now possible to create highly engaging experiences thanks to personalization, but that personalization is by far easiest to achieve by adopting technologies like Facebook Connect, which, while appropriate in some contexts, is inappropriate in many, and highlights how much &#8220;we in the internet&#8221; have failed to address the very real needs of website developers and their users. It&#8217;s taken Mozilla a fair bit of time & experimentation to get to something that feels truly great, but I&#8217;m very bullish on our first big push in this space, which we&#8217;re calling [BrowserID](https://browserid.org/about) for now. The goals of BrowserID are simple:

  * users and websites want to make sign in easy
  * users should be able to choose who their identity provider is
  * websites don&#8217;t want to be beholden to a single identity provider
  * sign in should work everywhere

With BrowserID Mozilla took a bold step, which is still poorly understood even within Mozilla:

  * we built a system that works in all modern browsers
  * we&#8217;re standing up a service to bootstrap the system until identity providers opt in, with the strictest transparency and privacy guarantees we can come up with
  * identity providers can federate it when they want
  * we build on identity concepts which users and developers understand and trust today.
  * we&#8217;re hoping that all browsers provide enhanced user experiences on top of the protocol, but we don&#8217;t need and won&#8217;t wait for their cooperation. This fight will be won by offering something compelling to website developers (and their users!) first.

For Mozilla devs, this is a bit shocking, as we&#8217;re not starting by putting a feature in Firefox first (although we sure hope that Firefox will implement BrowserID before the others!). While I love Firefox, this makes me happy, because in my mind, Mozilla is about making the internet work better for everyone, not just Firefox users, and in this case being browser-neutral is the right strategic play.

Note that Mozilla has always _been_ about making the internet better for everyone, and that&#8217;s what&#8217;s driving e.g. our policy work. Pragmatically, Mozilla is now big enough that I believe we&#8217;ll be more effective if we fight on several fronts at once &#8212; coordination costs are very real, and progress on BrowserID in no way diminishes Firefox&#8217;s value proposition, although they can (and will!) be better together.

### Apps that are _of the web_

The other critical challenge to the web is the rise of Apps, as a mechanism that developers are turning to because it&#8217;s easier to get your apps found & bought, and that users love because it&#8217;s an easier way to experience functionality on mobile devices in particular. And here too, Mozilla has a strong play, which is just starting, but which I believe has legs. We launched a [developer preview of our Apps initiative](https://apps-preview.mozilla.org/), which has the following bold (but doable!) aims:

  * make web technologies the best way to create apps that users can find and install on all devices
  * propose a standard for app purchase and installation that allows many appstores to compete for developers and users, so that developers don&#8217;t have to go through an arbitrary process to reach their audience, and users can choose where they want to get their apps.

There are many more things to say about our Apps effort, but I like to summarize it as teaching the web about the good bits of apps, and teaching apps about the good bits of the web. Right now we&#8217;re watching the sausage being made (something you don&#8217;t see in the Apple and Google kitchens), and it&#8217;s a bit chaotic.  But over time, and by the time it gets into consumer hands, it&#8217;s going to be splendid.

Here too, the goal is complementary to the success of the Firefox browser. And here too, we need so much help, from app developers to help us prioritize features, from web runtime developers to negotiate and implement the APIs that app developers need, and from early adopters to help us iron out the experience (and be forgiving especially in these early days).

### &#8220;Finally!&#8221;

I&#8217;ve been speaking to app & website developers about BrowserID and Apps for a few weeks, and the feedback has been great &#8212; webdevs & entrepreneurs are very aware of the dangers of relying on Facebook, Google, or Apple as the bridges to distribution or users. They desperately want an upgrade to the internet that solves these issues in an infrastructural way, and they are quite aware that Mozilla has a unique position beyond being the makers of Firefox.  Webdevs understand the public benefit charter of Mozilla, and many are keen for us to take on more responsibilities there, and happy to help.

### Culture shock

I expect it&#8217;s not obvious from a distance, but this kind of strategic broadening is hard on a culture. It means that we don&#8217;t have a single way of going after things. It means that others in the project seem to work in directions which don&#8217;t appear to line up with your own. It means that now engineers don&#8217;t just argue with product folks (a tradition in every software organization), but with other engineers with different priorities. It means that it&#8217;s impossible (and frustrating!) to keep track of what everyone is doing. All that is painful, especially as the odds are long in each of these battles, so it&#8217;s natural to want everyone else to drop what they&#8217;re doing and come help you out.

The best advice I have if you find yourself in this kind of culture shock is to first recognize it for what it is: you&#8217;re looking up from something you&#8217;ve been heads-down in, and your world (and your Mozilla!) looks like it&#8217;s changed in surprising ways &#8212; that&#8217;s scary, for limbic-brain kinds of reasons. We all tend to feel this way when we learn about new developments around us that we weren&#8217;t deeply involved with, from SOPA to &#8220;what the kids are up to these days&#8221;. We have to moderate that gut reaction with a bit of brainpower, and realize that just because it makes us uncomfortable, it&#8217;s not necessarily bad. That&#8217;s when the work begins: finding out who is working on whatever it is that&#8217;s making you uncomfortable, and reaching out to them to get looped in. In particular, doing so tends to work better face-to-face, or at least one-on-one. Finding the right people to talk to will take effort and time. It&#8217;s on you to do that work, though, and get informed.  Take the time to understand the history of the change before expressing your unhappiness &#8212; the people involved are likely just as smart as you, and if they&#8217;re Mozillians, they&#8217;re motivated by the same mission.

### Looking forward

So while there&#8217;s tension aplenty, when I think about this new Mozilla, which not only is committed to producing the best possible browser on desktops and phones, but is willing to invest in shaping what mobile devices should and could be like in 5 years, and reaching out of its comfort zone by standing up to internet bullies in critical areas like identity and apps, I&#8217;m pretty proud to be involved.  I&#8217;m confident that 2012 is going to see the emergence of new facets of Mozilla, just as the net needs its particular blend of values, ambition, and pragmatism more than ever.