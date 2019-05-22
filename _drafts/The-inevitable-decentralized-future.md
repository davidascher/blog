---
id: 729
title: The inevitable decentralized future?
date: 2012-08-14T22:08:03+00:00
author: David Ascher
layout: post
guid: http://blog.ascher.ca/?p=729
permalink: /?p=729
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "729"
categories:
  - Uncategorized
---
In a recent blog post, I bemoaned what I saw as a gloomy future for the internet, whereby new, &#8220;better&#8221; walled gardens are being built by excedingly well-run and ruthless corporations, all driven to turn us all into eyeballs, ARPUs, and other insulting and dehumanizing labels.

It&#8217;s easy to look around and see threats to the democratic, equalizing, open, boiling internet of yore. We see them in ever-increasing centralization of product strategies, the death of open APIs, the ever expanding scope and ambition of The Giants, and the ever deepening and broadening capabilities of soulless companies beholden to Wall Street. But that&#8217;s depressing, so let&#8217;s not dwell too much on that, even if that brings Evgeny Morozov&#8217;s wrath.

Instead, I want to point out two long term trends which I choose to believe have disruptive power in the face of these current trends, and which are energizing me.

1. Moore&#8217;s law and phase transitions

The first trend has to do with the strange implications of Moore&#8217;s laws and economic thresholds. As I&#8217;ve talked about in various talks for a few years now, we&#8217;ve seen a huge shift in how cost models have shifted how we think about &#8220;building an Internet feature&#8221;.

. In the last 15 years, rapid decreases in the cost structures of software creation, massive changes in the size of the addressable market, and the emergence of monetization platforms have all conspired to jolt our view of how innovation can happen on the internet. I rememer an organism so incredibly expensive as a whole that \_of course\_ it had to be a multi-party, standards-negotiating, collaborative effort. These days, any &#8220;rich kid with a trust fund&#8221; or even a passing connection to some risk-tolerant financiers can reasonably say &#8220;I know, I&#8217;ll build this thing for the Internet, and it will be global; no federation, no standards &#8211; that way we&#8217;ll move fast and retain control.&#8221; This shift has had many positive outcomes, from the obvious resulting acceleration of innovation to the less obvious increase in the role of design. It&#8217;s also paid for a lot of mortgages and groceries. But it&#8217;s also undermined the economic underpinnings of the Internet as a \_commons\_, to be tended in concert.

To be more precise: it&#8217;s now positively cheap to build a cloud based service that accumulates enormous quantities of data \_for all possible users (!)\_, to process that data so as to mine it for money, and to adjust the product offering daily until the product either fails fast or becomes profitable at scale. As a result, many people are doing it, and doing so with no public benefit or even multi-party approach in mind. There is ample financing to feed that system, and enough high-value exits typically from acquisitions that we have a fairly efficient source of new features for the silos. I think that&#8217;s all well understood, at least on Wall Street.

What&#8217;s been bubbling in my mind in the last few months is that I wonder if we&#8217;re on the cusp of a different phase transition, due to a continuation in the shifts in the cost of &#8220;feature creation&#8221;. And this one feels like it could have even deeper societal impact.

After talking to people who know a lot more about these things than I do, I&#8217;ve come to believe that the operating cost of running a service for a very small number of users, managing a very small amount of data, is getting so low that it&#8217;s hard to come up with a consumer good that has an equivalent price. I expect that within a small number of years, the cost of a latte or a Big Mac will cover many years of operating costs for such an app (assuming competence all around).

[Technical note: imagine a fully loaded optimally-sized server running well-written node.js-or-equivalent servers intelligently sharing a not-particularly-sophisticated datastore on commodity hardware. Or imagine a plug computer.]

Let&#8217;s assume for a minute that there are compelling features that users would love, and which fit in an environment that doesn&#8217;t require BigData or BigCompute. As an example, imagine a personal address book with a simple API &#8212; a few hundred records, some simple access control logic, nothing fancy. Data and access that&#8217;s important to an individual, and which even today resists fitting in any silo, be it Facebook, LinkedIn or any other. There are, I&#8217;ll posit, other such interesting pesonal features (or, as we call them today, apps) worth building &#8212; remember: the criterion isn&#8217;t whether they&#8217;re fundable, or can be commercially successful, but whether they provide meaningful value to individuals.

We know enough about the economic impact of open source, dynamic languages, and the power of 1 coder + 1 designer, to imagine a world where these applications are very cheap to produce, especially if we can start to leverage the \_global\_ creative class. Exhibit one: the Apple and Android appstores.

Those apps are then things which a very small team can create, distribute for free, and whose operating costs are measured in cents/user \_and decentralized\_. What&#8217;s exciting about that concept is that we can look beyond traditional business models to finance them. We end up in an economic regime where the question is not &#8220;how to maximize profit&#8221; but &#8220;how to finance access&#8221;. And in that regime, depending on the app, many models seem insanely reasonable, from the street-level &#8220;I&#8217;ll pay for the hosting of this app for everyone in my kids&#8217; school&#8221; to financing by government (neightborhood, city, province, state), and even medium-sized non-profits can envision acting on national or global scales. On a per-citizen basis, it&#8217;s a lot cheaper than roads, medicines, or even school lunches.

In other words, &#8220;the means of production&#8221; have become so cheap, and the modes of distribution so instantaneous, that the operating cost of an app is negligible. We still have to find ways to compensate the creative work, but it need not be through charging users directly, or even selling user&#8217;s data to third parties. If the goal isn&#8217;t primarily financial reward, then many more models become viable. 

Kickstarter is the example du jour for alternative funding models, but my point here is that we can decentralize the operating costs of cloud apps, not just the source of funds. Your average kickstarter project defers the question of how the &#8220;thing&#8221; is financed, but most of the ones I&#8217;ve seen still require either significant concentration of capital, which begets concentration of control. It need not be that way. 

Note that I&#8217;m not arguing against the traditional investor / corporate / customer model of creating utility &#8212; simply wondering whether we might not be on the cusp of an explosion in viable outlets for all of the creative minds out there who aren&#8217;t well suited for the traditional model.

2. And then there&#8217;s topology

If we think of apps as decentralized, linked units of computation+data, then many interesting effects seem possible. 

First, it&#8217;s hard to believe that the world wants applications that are as monocultural as they appear to be in 2012. Facebook blue, Google white, Apple shiny and Metro squares? That&#8217;s the menu? Surely there are myriad user benefits that would result from having apps that are developed by people who understand how they rather than how north-americans think; apps with data that&#8217;s topologically close to them, rather than in some faraway server farms in a country subject to jurisdictions that the users have no influence over? Platforms that understand problems that are deeply local?

There too, I think there are interesting trends which could turn out well for humanity. Specifically, as connectivity gets better, people&#8217;s expectations of what kinds of realtime communications are available will result in a clash with the desire for centralization of data-at-rest. As technologies like Skype and Facetime become more mainstream, I&#8217;m seeing a shift where people used to see them as alternatives to much more expensive modes of communication (from long distance calls to airplane rides), and now simply incorporating them into their daily life. As that happens, I claim that a majority of the bandwidth usage will come from topologically near nodes. And that usage pattern will strengthen the drive of peer-to-peer network models, rather than hub & spoke models. Like Arend Naylor, I like to believe that the advent of WebRTC is one of the potentially most disruptive additions to the web platform, although I&#8217;m the first to admit that I don&#8217;t yet understand how it will surface in real apps.