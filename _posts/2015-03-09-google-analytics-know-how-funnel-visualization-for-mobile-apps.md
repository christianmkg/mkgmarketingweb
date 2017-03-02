---
ID: 5224
post_title: 'Google Analytics Know How: Funnel Visualization for Mobile Apps'
author: Mike Krass
post_date: 2015-03-09 06:28:04
post_excerpt: ""
layout: post
permalink: >
  http://mkgmarketinginc.com/google-analytics-know-how-funnel-visualization-for-mobile-apps/
published: true
views:
  - "1987"
---
[soundcloud url="https://api.soundcloud.com/playlists/86675120" params="color=ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false" width="100%" height="450" iframe="true" /]

<em>For the TL;DR crowd: This podcast explores Google Analytics to find out where mobile app users drop off in the purchase process. Listen to the audio above or skim through the excerpt and transcript below for more detailed information.</em>
<h1>Google Analytics Know How: Finding Out Where Users Drop Off in Mobile App Purchases with a Funnel Visualization Snapshot</h1>
A few weeks back I hosted the inaugural Google Analytics meet up at <a href="http://nextspace.us?utm_source=mkgmarketinginc" target="_blank">NextSpace</a>, a co-working space based in San Francisco. As an active Google Analytics practitioner, I was interested in meeting up with non-practioneers to hear their use cases and questions about Google Analytics.

This initial meet up spawned a few really solid topics (more on those in a later post), but the one that we'll discuss today came from Carlos, an iOS developer here in San Francisco:
<blockquote><strong><em>Can I figure out where my app users drop off in the mobile checkout process?</em></strong></blockquote>
Luckily for Carlos, the short answer is <span style="text-decoration: underline;"><strong>YES</strong></span>. Using a Funnel Visualization report (example below), you can figure out at exactly what steps users dropped out of your purchase funnel.

<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/03/Google-Analytics-Funnel-Vizualization-Report.png"><img class="alignnone wp-image-5228 size-large" src="http://mkgmarketinginc.com/wp-content/uploads/2015/03/Google-Analytics-Funnel-Vizualization-Report-1024x446.png" alt="Google Analytics Funnel Vizualization Report" width="1024" height="446" /></a>

It's pretty simply to wire up this report:
<ol>
	<li>Navigate to Conversions"</li>
	<li>Expand the "Goals" option</li>
	<li>Click on "Funnel Visualization"</li>
</ol>
Voila!

For those interested in the full transcript, read along below:
<h3>Transcript of Google Analytics meet up</h3>
<em>Liz: I'm Liz. I work for a hotel company, and we use Google Analytics exclusively for all of our traffic, and seeing our customer's path, clicking.</em>

<em>Scott: I'm Scott. I work at Razorfrog Web Design. We use Google Analytics to optimize sites, look at page feed, and that kind of stuff.</em>

<em>Max: I work with Scott. I'm Max. We use it for all our clients, some 150 various accounts that we're looking at right now, some much more than others. I'm trying to make sense of it for them, on their behalf, trying to look through it on our behalf, just where we can make improvements, for pages, and conversions, and goals. A lot more for our own site, with goal tracking, and Dropbox, and forms, and those units and things.</em>

<em>Carlos: Hi, I'm Carlos. I'm a developer. I installed it, and I want to know more.</em>

<em>Steven: I'm Steven. I'm a co-founder for a company called [inaudible 00:01:06], and we use Google Analytics for tracking, and here to learn how to use it more.</em>

<em>Natalie: I'm Natalie, and I don't know anything about Google Analytics. I'm here to eat my lunch and listen to the sound of Mike's voice.</em>

<em>Jen: Me too.</em>

<em>Mike: Eat lunch. That's going in the meeting minutes. Eat lunch and listen to Mike. Jen seconds. All right.</em>

<em>Jen: We're the cheerleaders.</em>

<em>Steve: Hi I'm Steve. I'm currently taking some tech courses, but looking to do some development shortly. We just want to learn more about Google Analytics, details and specifics.</em>

<em>Rob: I'm Rob; I'm the founder of Senior Care Web Business. We use Google Analytics for user acquisition, where people are coming from, which channels have ROI. And then also conversion tracking, and what percentage of people are buying something, and where they are coming from so that we can make smarter business decisions. [pause] And eat my sandwich.</em>

<em>Mike: Well, if we want to just start by just addressing use cases, I think Carlos had one out of the gate.</em>

<em>Carlos: Yep.</em>

<em>Mike:  So, I think Carlos your initial question was like, "Where do people drop off?" And in Google Analytics, there in the goals section you can do a funnel visualization. So, you can start from anywhere. But we should start from e-commerce.</em>

<em>Max: And you can make lots of them and save them all?</em>

<em>Mike: Yes.</em>

<em>Carlos: So you can basically decide what pages you are tracking at the go?</em>

<em>Mike: Well, Google Analytics, as long as you deploy it on your entire site, or the app, it will grab anything. So you can pick a page here. It just starts at like an index or an entrance. So in reality this is like the homepage. This is our client's homepage.</em>

<em>And there's not much in this goal, because you just basically go from the homepage to trial. And either you make it or you don't. So, you can see here that this shows about 40,000 people, or about a fourth, a little more than a fourth, just drop off. And they end up dropping off to just an exit the website, they make it to checkout but they don't go all the way. They end up going to a product page, a different product page.</em>

<em>So you can do this. This is probably a better funnel. Here we go. This is what it would look like for a shopping cart, so you can see the entrance here on the left. And then it's PD, this is our product pages and then they actually get into the cart. So it shows 10% of people make it to the cart.</em>

<em>And then there's individual phases. So a great thing here to see is that 98, almost 99% of people make it from the cart entrance to their billing info. And then you see the drop-off.</em>

<em>Max: If people wanted to check out, but then they change their minds when they're entering billing.</em>

<em>Mike: Yeah. So that's how we use this for this client is to call out those drop-offs. It's really tangible for this client because with 31,000 drop-offs, their product costs 80 bucks a month, or 80 bucks. So they're leaving $2.5 million on the table in the last month.</em>

<em>So we're not saying you're going to get all of that, because that's never possible, but you could at least get some of it.</em>

<em>Natalie: That's a lot!</em>

<em>[chuckles]</em>

<em>Mike: Yeah. So that's a good example of the question you had, Carlos.</em>

<em>Carlos: Mm-hmm. That absolutely completely answered that.</em>

<em>Mike: And you can do that all these goals that are set up are the same types of goals you can set up for mobile devices.</em>

<em>Carlos: Mm-hmm.</em>

<em>Mike: So, you can set up those goals for in-app purchases, [pause] you know, downloads, anything like that.</em>

&nbsp;