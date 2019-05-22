---
id: 362
title: Thunderbird and Institutional users
date: 2007-11-20T17:00:01+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "362"
categories:
  - Enterprise
  - France
  - MailCo
  - Mozilla
  - Thunderbird
---
During my trip to Paris last week, I met with a set of representatives from public sector institutions which are deploying Thunderbird to large sets of users, as part of a larger (and long-term) move towards open source and open standards. It was fascinating to find out what their goals were, what they&#8217;d been able to achieve, what hurdles they were still facing, and how we might be able to work together.

### User control vs. centralized responsibility

In enterprises, people expect their IT department to help them if they have problems using the software they use for work. Especially if the IT told them to use Thunderbird, that means that the same IT department has to be able to support it, in the local language, using customized, organization-specific documentation. In that kind of scenario, it&#8217;s seen as important that the IT department has the right level of control over exactly what version of Thunderbird is in use. Many of the things that make both Firefox and Thunderbird wonderful consumer products end up inadvertently making it harder for those IT administrators to support it. Auto-update, which is key to keeping the web safe and any desktop application up to date especially with security fixes but also with continuous improvement, is a possible time-bomb for the people handling support in large installations. The ability for end-users to install extensions which solve a need they have as individuals, if it breaks core functionality in the product, and results in calls to tech support, end up hurting the product.

I like these topics because I think that while on the surface they seem like points of conflict between the end-user focus of Mozilla products and enterprise deployments, longer term I see opportunities for progress on both &#8220;sides&#8221;.

  * The AUS technologies that Mozilla built to support updating hundreds of millions of users at once can be redeployed inside enterprises to give them the control they need and facilitating faster update cycles. 
  * The support concerns that IT managers have about extensions aren&#8217;t that different than the concerns the Firefox team probably has about possible &#8220;rogue&#8221; extensions, and together I suspect both groups can help each other. 
  * Improving the configuration experience for Thunderbird will help the home user as much as the IT administrator. 

Annoyingly for me, when these institutions distribute Thunderbird, the update-checking mechanism is deliberately disabled as part of a global security policy, meaning that not only do bug fix releases like last week&#8217;s [2.0.0.9](http://www.mozilla.com/en-US/thunderbird/2.0.0.9/releasenotes/) don&#8217;t reach those users, but I have no way of even guessing how many such users there are! This makes understanding user trends like total user population, the speed at which users upgrade, etc., much harder.

### The power of extensions

Extensions are great. Everyone says it, and they&#8217;re usually referring to Firefox extensions. But I believe the potential power of extensions is even greater in the world of messaging than in the world of the web. Browsers are made to interact with websites, most of which try _very hard_ to make the experience be the same across browsers. Firefox extensions, in some way, fight the dominant mode of the web. In a messaging client, however, extensions can work hand-in-hand with server-side technology, or the sometimes very idiosyncratic needs of a specific organization. I was shown several fascinating Thunderbird extensions implementing CRM-like features, global account management features, integration with custom calendaring software, specialized mail handling, etc. In these organizations, the email client is deeply customized to fit the local needs, and the Mozilla platform&#8217;s story on extensibility is unbeatable. There are definite issues in the Thunderbird extensions story, but there are also low-hanging fruit there.

### Pre-configuration and mass deployment

If you think Thunderbird is hard to configure right now (I do), imagine being responsible for configuring 80,000 desktops for non-technical users! There are some [systems](http://kb.mozillazine.org/Configuration_utilities_for_administrators) in place already, but I understand there are still issues that make it a challenge to deploy Thunderbird in such large installations. This is likely more problematic for Thunderbird than for Firefox, as there are more environmental settings involved in email than in web browsing. Indeed, several of these enterprises deploy Thunderbird but not Firefox, countering the notion that Firefox is always the &#8220;lead&#8221;.

### Opportunities for peer-help and a Thunderbird consultant market

If last week&#8217;s conversations are any indication, there are likely hundreds of individuals responsible for hundreds of thousands and maybe soon millions of Thunderbird installations, and yet they likely don&#8217;t know each other. One of them may even have solved a problem that the others are struggling with, or don&#8217;t yet know they&#8217;ll have. Today, it&#8217;s hard for these people to find each other. That&#8217;s a problem we should be able to solve, using basic tools like Wikis and a dedicated mailing list/newsgroup.

Another opportunity is that institutional users tend to have core competencies which don&#8217;t include writing Thunderbird patches or extensions. There are, however, a growing number of small and not-so-small service companies which are learning how to do that better and better. There&#8217;s a market gap there, especially as MailCo itself is not likely to build custom extensions, for example. Given that my number one goal is to facilitate adoption of Thunderbird, I want to facilitate the creation of a market for custom Thunderbird extensions, and for fixes to bugs which may be urgent for some but which we may not get to soon enough. If you&#8217;re interested in either side of that marketplace, let me know.

### The debate is different

More specifically, the people I talked to represent a new type of customer for me. Thanks to years of evangelism by people like [Tristan Nitot](http://standblog.org/blog/), I didn&#8217;t have to argue for releasing code under compatible open source licenses, or for working hard to avoid the need for forks. Even more interesting is the fact that in North America, when I describe what I&#8217;m up to, the most common first question is &#8220;but how will you make money?&#8221;, while at least in one big meeting with lots of people, _no one asked_. The people I talked to were more interested in the non-financial aspects of the Mozilla endeavor. That money is being made is fine, but one gets the feeling that it&#8217;s not a particular point of interest by users or pride by community members. Knowing that Mozilla is willing to take on fights that no one else is willing to take on, _that&#8217;s_ inspiring and exciting, and worth taking some risks for.

### Next Steps

The single most common complaint I heard regarding Mozilla&#8217;s handling of Thunderbird is not enough communications. Communications about everything from the roadmap (on my plate), the APIs for extensions (FUEL for Thunderbird anyone?), the wiki, the strategy to change the world, and more. I agree wholeheartedly, even with the criticism that I should blog more. Mea culpa, will try to do more in the coming weeks.