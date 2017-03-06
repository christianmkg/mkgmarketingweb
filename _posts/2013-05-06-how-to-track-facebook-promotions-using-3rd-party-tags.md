---
ID: 2607
title: >
  How to Track Facebook Promotions Using
  3rd Party Tags
author: KerryGuard
date: 2013-05-06 10:27:44

layout: post
permalink: >
  /how-to-track-facebook-promotions-using-3rd-party-tags/
published: true
seo_title:
  - >
    How to Track a Facebook Promotions Using
    3rd Party Tags
seo_description:
  - >
    A Step-by-Step Guide Describing How to
    Track Facebook Promotions Using 3rd
    Party Tags
seo_keywords:
  - >
    Shortstack, Facebook Promotion Pages,
    Charles Proxy, Web Debugger
views:
  - "127"
---
<h2><em></em>"Can we track our marketing efforts if we drive traffic to a Facebook Promotion page?"</h2>
Recently, one of our clients asked to drive <em><strong>ALL</strong></em>Â their digital marketing efforts, tracked by 3rd party tags, to a Facebook Promotion page.

In remembering what <a title="How to be a Good Digital Marketing Partner" href="http://kerryguard.com/how-to-be-a-good-digital-marketing-partner/">Don Draper said two weeks ago in Mad Men</a>, about saying yes when they should have said no, our initial gut instinct was to tell the client:
<blockquote>Absolutely not. With the way conversion tracking is set up right this minute, we cannot track performance on that Facebook Promotion page.</blockquote>
Instead, we took a step back to test whether or not their 3rd party tags could be tracked through a Facebook Promotion Page.
<h2>Ask Questions</h2>
<span style="line-height: 1.5em;">Before we provide a solution to a client we first made sure we understood all the moving parts out of our control, in this case the only piece we didn't control was the Facebook page and how it was built.</span>

By simply asking, "How is this built? Are you using a specific program or writing it from scratch with HTML &amp; CSS?" We got a very simply response from our client that they were using <a title="Shortstack" href="http://shortstack.com">Shortstack</a>,Â <span style="line-height: 1.5em;">a free application to easily build Facebook Pages for promotions, sign-ups, photo contests, etc.</span>
<h2>Research</h2>
By having this information we were able to quickly look at any documentation Shortstack had on 3rd party tracking. The only <a title="Short Stack Help" href="http://help.shortstackapp.com/main-menu/mastering-shortstack/advanced-widget-programming/#TrackingReferrals">page</a> we found was in regards to trackingÂ referrals, but to track those we'd still need to implement 3rd party tags.

<span style="line-height: 1.5em;">So we decided the best research is hands on research so we created a Shortstack account with a fake promotion to run a conversion test.</span>
<h2>Trial &amp; Error</h2>
By creating our own account we were able to walk through the user flow and see where the sign-up is confirmed. Â In this case the only change was a simple copy addition, that simply said,
<blockquote>Thank you for your submission</blockquote>
Because it wasn't aÂ separateÂ landing page we weren't sure we were going to be able to track conversions at all. Before we gave up all hope and turn to our client to say no, we quickly walked one of our developers through the process he's said to place an image tag after the thank you copy.

After digging further into the functionality of Shortstack we were able to do just that.

<span style="line-height: 1.5em;"><span style="color: #443322; font-family: Asap, Verdada, Arial, Helvetica, sans-serif; font-size: 24px; line-height: 1.2em;">Follow These 4 Steps to Track Your Own Facebook Promotions Using 3rd Party Conversion Tags</span></span>

In staying with the Shortstack Facebook Promotion page application, follow the steps below:
<h2>Step #1: Sign in to Shortstack</h2>
<h2><span style="line-height: 1.5em;">Â </span></h2>
<a style="font-size: 14px; line-height: 1.5em;" href="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.09.07-PM.png"><img class="aligncenter size-full wp-image-2628" alt="Shortstack.com Sign In Page" src="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.09.07-PM.png" width="1114" height="675" /></a>
<h2>Step #2: Open The Promotion Page App</h2>
<span style="line-height: 1.5em;">Open your App that houses the promotion you need to track. In our case, "Fake It 'Til You Make It" is the test application we created.</span>

<a style="font-size: 14px; line-height: 1.5em;" href="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.11.50-PM.png"><img class="aligncenter size-full wp-image-2629" alt="Screen Shot 2013-04-26 at 3.11.50 PM" src="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.11.50-PM.png" width="1073" height="337" /></a>
<h2>Step #3: Edit the Promotion</h2>
<span style="line-height: 1.5em;">Under 'edit widgets', click the pencil icon for Promotion.</span>

<a style="font-size: 14px; line-height: 1.5em;" href="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.13.06-PM.png"><img class="aligncenter size-full wp-image-2630" alt="Short Stack Editor" src="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.13.06-PM.png" width="1302" height="678" /></a>
<h2>Step #3: Implement Image Tag</h2>
<ul>
	<li><span style="line-height: 1.5em;">Scroll down to "Override Labels, Messages, and Other Text"</span></li>
	<li><span style="line-height: 1.5em;">Replace "Thank you for your submission" with: Thank you for your submission &lt;img src="//www.googleadservices.com/pagead/conversion/<span style="color: #ff0000;">xxxxxxx</span>/?value=0&amp;amp;label=<span style="color: #ff0000;">xxxxxxxxxxxx</span>&amp;amp;guid=ON&amp;amp;script=0" style="height:1;Â  width:1"/&gt;</span></li>
</ul>
<a style="font-size: 14px; line-height: 1.5em;" href="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.15.30-PM.png"><img class="aligncenter size-full wp-image-2632" alt="Screen Shot 2013-04-26 at 3.15.30 PM" src="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.15.30-PM.png" width="1166" height="519" /></a>
<h2>Step #4: QA Test to Confirm Tracking is Operation</h2>
<span style="line-height: 1.5em;">We use the </span><a style="font-size: 14px; line-height: 1.5em;" href="http://www.ghostery.com/">Ghostery Plugin</a><span style="line-height: 1.5em;"> for Firefox &amp; Chrome which allows us to see the conversion pixel fires in the purple box at the top right of our browser.</span>

<a style="font-size: 14px; line-height: 1.5em;" href="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.21.25-PM.png"><img class="aligncenter size-full wp-image-2633" alt="3rd Party Tracking Facebook Promotion" src="http://mkgmediagroup.com/wp-content/uploads/2013/04/Screen-Shot-2013-04-26-at-3.21.25-PM.png" width="1448" height="905" /></a>