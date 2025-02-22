---
title: Using Google Search Console to effortlessly monitor small hobby projects (or big ones!)
image: /assets/images/2023/google-search-console.png
tags:
    - Google Search Console
    - Web
---

Like a lot of developers, I've somehow ended up with a collection of mini-projects online that require no maintenance, are missing a few features, but still get some Google traffic. I used to use Google Analytics for this, but I've been really, really impressed by [Google Search Console](https://search.google.com/search-console)!

## What is Google Search Console?

Google Search Console is a simple (and free) service to track how a site is doing from Google's perspective. This obviously includes how highly ranked the site appears in results, but it also includes a lot more!

For example, are there any errors found following links? Are any pages giving conflicting metadata around canonical URLs? Are any pages loading too slowly?

All of these factors factor into Google's search algorithm, as they are symptoms of a high quality site. As such, following recommendations to improve your site's Google listing... also improves the quality in general!

Google themselves [describe it as](https://support.google.com/webmasters/answer/9128668?hl=en&sjid=5299712260308016178-EU):
> Google Search Console is a free service offered by Google that helps you monitor, maintain, and troubleshoot your site's presence in Google Search results. You don't have to sign up for Search Console to be included in Google Search results, but Search Console helps you understand and improve how Google sees your site.

## Why use it?

There are a *lot* of reasons to try out Google Search Console, even before getting into the actual [features](#what-features-does-it-have)!

### Simple

I don't get on with Google Analytics. I get lost, I find it impossible to manage multiple sites, and get lost in trying to filter... dimensions... audiences... funnels. [Google Search Console](https://search.google.com/search-console) has drastically less data, but surfaces it in an extremely usable and helpful way.

Usability can be somewhat subjective, but given the drastically smaller userbase of this platform, I get the feeling that Google's designers have been more "free" to make changes. Below is the main overview, it instantly surfaces the 3 things I likely care about most:
1. How many users are visiting my site?
2. How many of my pages is Google listing?
3. How high quality are my pages?

I'll dive into each page in [the features section](#what-features-does-it-have), here's how it looks:

[![](/assets/images/2023/googlesearchconsole-overview-thumbnail.png)](/assets/images/2023/googlesearchconsole-overview.png)

### Automatic subdomain verification

If you have verified a domain property (by adding a DNS record), adding a new subdomain requires no additional work. Just adding the subdomain sets it up, ready for tracking, since Google knows you own the entire domain.

[![](/assets/images/2023/googlesearchconsole-verification-thumbnail.png)](/assets/images/2023/googlesearchconsole-verification.png)

This means the overall site stats are visible, whilst individual project sites can be dived into easily. I have ended up adding every domain I'm actively working on to Google Search Console, it's very satisfying seeing random old projects experience traffic surges (due to [proactive emails](#proactive-emails--achievements)).

[![](/assets/images/2023/googlesearchconsole-sites-thumbnail.png)](/assets/images/2023/googlesearchconsole-sites.png)

### No code needed

Yep, no JavaScript needed. Your site's code is completely untouched, there's no security risks, there's no increase in page load time, none of the downsides of other tracking solutions.

Since Google owns Google Search (obviously...) and the Google indexing bot, Google Search Console is merely surfacing some of the data they have already collected. 

As such, the only technical work needed is adding the DNS record to prove domain ownership, so that Google is comfortable sharing the data with you (see [how to set it up](#how-to-set-it-up)).

### Proactive emails & achievements

I am very confident that Google Analytics etc has the ability to set up emails for spikes in traffic. With Google Search Console however, it's all already there. 

For example, I recently added [my settlers manual](https://settlers.jakelee.co.uk) to Google Search Console, then a few days ago received an email letting me know it had received 80 users from Google Search! Obviously these aren't big numbers, but as it's a small project I haven't touched in years, I would never have thought to check the analytics without this achievement notification.

[![](/assets/images/2023/googlesearchconsole-email-thumbnail.png)](/assets/images/2023/googlesearchconsole-email.png)

Clicking the link in this email also lets you view historical achievements, useful for an instant look at how consistent the site's growth it.

[![](/assets/images/2023/googlesearchconsole-achievements-thumbnail.png)](/assets/images/2023/googlesearchconsole-achievements.png)

### Monthly summaries

If your project is your main source of income, or you spend a lot of time on it, then you'll probably be checking the analytics daily. However, for a small project you did in a weekend a few years ago? It's unnecessary.

This is where Google Search Console's monthly emails are such a helpful feature. They provide a very high level view of how your site is doing, and I always give them a quick skim-read when they arrive.

I won't show all the detail (the screenshot would be very long!), but the monthly emails include:
1. The number of clicks, views, and pages with first impressions this month.
2. The top growing & performing pages this month (and how many clicks they received).
3. The top growing & performing queries used to find your site.
4. What type of device, country, and type of Google search the user found your site via.

This is extremely helpful data, all without any code being added to your site! I find the information on growing & performing pages to be an especially interesting snapshot into why people are visiting your site.

[![](/assets/images/2023/googlesearchconsole-content-thumbnail.png)](/assets/images/2023/googlesearchconsole-content.png)

Finally, the "insights" feature lets you know which search queries you are in the top 5 results for, growing content, clicks per month, etc. For my site, it shows that despite all my high effort technical posts... people just want to read about gaming!

[![](/assets/images/2023/googlesearchconsole-insights-thumbnail.png)](/assets/images/2023/googlesearchconsole-insights.png)

### Quality monitoring

Google looks at your site regularly, to ensure their search results are up-to-date. If the site is added to Google Search Console, whenever it experiences something *weird* that dissuades it from showing your page in results, you'll receive an email.

This could be anything from a page not being found, a redirect, conflicting meta tags, or duplicate content. Most of these "issues" aren't actually errors, but they are potential problems that are worth looking into. For example, on my sites I have hundreds of unindexed pages due to:
* Search results pages (correctly) stating the main search page should be indexed instead.
* `http://` pages that (correctly) state `https://` is the main source of the content.
* Old URLs that broke when I moved away from Wordpress' `/year/month/day/title` URL format to my current `/title`.

[![](/assets/images/2023/googlesearchconsole-unindexed-thumbnail.png)](/assets/images/2023/googlesearchconsole-unindexed.png)

These alerts have been pretty useful when I've accidentally broken something on one of my sites without realising, such as [incorrectly stating my site should be HTTP](https://blog.jakelee.co.uk/jekyll-github-pages-https/)!

### No limitations / upselling

Nice and simple, the service is completely free and unlimited. Thousands of pages? Hundreds of domains? All free!

Since Google *wants* you to improve your site to provide better search results, the free service they're providing is mutually beneficial.

## What features does it have?

Okay, so I've run through why I use Google Search Console. But what features are actually included in the site? Here's all the options in the sidebar:

### Overview

[![](/assets/images/2023/googlesearchconsole-overview-thumbnail.png)](/assets/images/2023/googlesearchconsole-overview.png)

As already mentioned, the main overview screen shows performance, indexed pages, and overall experience. "[Enhancements](https://developers.google.com/search/docs/appearance/structured-data/search-gallery)" are also supported, but I don't use them so can't comment.

There's also a "URL inspection" feature that shows you how Google Search views a specific page, and when it last updated. I use this feature to submit my new articles manually, since re-indexing can be requested.

[![](/assets/images/2023/googlesearchconsole-urlinspection-thumbnail.png)](/assets/images/2023/googlesearchconsole-urlinspection.png)

### Performance

This section is the most similar to more traditional analytics tools, as it provides detailed information on search queries, pages, countries, devices, etc.

The "pages" tab is especially interesting, since it shows the most popular pages across your site. Clicking each page lets you look at the search queries used to find it. Neat!

[![](/assets/images/2023/googlesearchconsole-performance-thumbnail.png)](/assets/images/2023/googlesearchconsole-performance.png)

There's also a page providing similar information on visitors from Google's "Discover" feature but... these numbers have always been extremely low for me.

### Indexing

The indexing section provides information on why pages are or aren't indexed (see [quality monitoring](#quality-monitoring)).

It also has a few useful but niche utilities:
1. Video pages, to help your site show up in Google Video results.
2. Sitemaps, to help the Google indexing robot find content. I especially like that multiple sitemaps can be added, useful for subdomains!
3. Removals, where you can request [Google hides some of your content](https://support.google.com/webmasters/answer/9689846#make_permanent) (usually for privacy reasons).

### Experience

Google Search Console also provides basic data on how quickly your pages are loading, how visible they are on mobile devices, whether they can use HTTPS, and similar concerns. This is a surprisingly helpful tool, and has helped me discover that various layouts have been broken on smaller devices.

Whilst this data is split into "Page experience", "Core web vitals", "Mobile usability", and "HTTPS", the first page provides a perfectly sufficient view of all sections:

[![](/assets/images/2023/googlesearchconsole-experience-thumbnail.png)](/assets/images/2023/googlesearchconsole-experience.png)

### Security & Manual Actions

I don't know what these are! I have never had any issues detected, which can only be a good thing.

### Misc

Finally, we have "Links", which provides a great overview of internal & external links. For example, most of my visitors come from Reddit, or Google, followed by GitHub. Since my main sites all link to each other via the top bar, this data is unfortunately somewhat inaccurate!

Additionally, due to Reddit's pagination URLs any successful post on there will look like it has been linked to from thousands of different URLs.

[![](/assets/images/2023/googlesearchconsole-links-thumbnail.png)](/assets/images/2023/googlesearchconsole-links.png)

Under "Settings" there's also fairly standard options to invite other users or services, update your URL, export all your data, etc.

## How to set it up?

1. Go to [Google Search Console](https://search.google.com/search-console).
2. Click "Add property".
3. Add the DNS record to your site (I did it via a Cloudflare integration).
4. You're done!

There's also a short but sweet [series of guides from Google](https://support.google.com/webmasters/answer/10267942) that provide an overview of everything Google Search Console can do. 

## Downsides of Google Search Console

Okay, so yes, despite being a massive fan of Google Search Console for the last year or so, it's not perfect. 

### Mysterious data sources

I don't quite understand how Google Search Console can show which sites link to mine, but it can! I assumed the tool would only be able to show me Google search related data, but apparently not.

Due to this mysterious data acquisition, I only really pay attention to the parts that focus on Google Search or my pages themselves. Perhaps it is linked to my Google Analytics?

### Basic data

Whilst I really appreciate the data that is being surfaced, it's always going to be limited. From search data alone you can't gain the user journey / funnel information that most analytics systems provide.

Personally I think this is a very fair trade-off for being entirely free, irreplaceable (since nobody else has Google's data), and requiring no code changes at all.

### Not realtime

Recently I had a massive spike in views for one of my articles (the [Need for Speed Unbound tips](https://jakelee.co.uk/need-for-speed-unbound-tips/)). However, I only found out about it when I reached a new 28-day record a week or so later. Whilst this didn't have any direct impact, it did leave me feeling like I was stuck viewing aggregated past data, which is a bit less exciting than something more realtime.

## Conclusion

In conclusion, I've no idea why [Google Search Console](https://search.google.com/search-console) isn't more widely used!

Whilst it isn't perfect, it's such a simple and easy to use tool that there seems to be no reason not to use it in combination with more comprehensive tools. Given the zero maintenance it requires and zero impact it has on my site's users, I'll definitely be staying subscribed to the emails.

Since Google doesn't directly make any revenue from it, I do understand why it isn't promoted very heavily at all. However, I'm pretty confident any users of it will gain a bit of goodwill towards Google & Google Search, so surely that makes it worth the effort?

