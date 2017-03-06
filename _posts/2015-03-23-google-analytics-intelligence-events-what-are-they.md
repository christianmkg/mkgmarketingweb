---
ID: 5293
title: 'Google Analytics: What are Intelligence Events?'
author: Mike Krass
date: 2015-03-23 06:40:22

layout: post
permalink: >
  /google-analytics-intelligence-events-what-are-they/
published: true
views:
  - "1299"
---
[soundcloud url="https://api.soundcloud.com/tracks/196505160" params="color=ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false" width="100%" height="166" iframe="true" /]

<em>For the TL;DR crowd: This podcast explores the <span style="text-decoration: underline;">intelligence events feature of Google Analytics</span>. Listen to the audio above or skim through the excerpt and transcript below for more detailed information.</em>
<h1>Google Analytics Intelligence Events: What are These Reports?</h1>
As we mentioned in our post last week, <a href="/google-analytics-know-how-funnel-visualization-for-mobile-apps/" target="_blank">Google Analytics Funnel Visualization Reports for Mobile Apps</a>, we hosted a Google Analytics meet up at our co-working space and got a really lively conversation going between Google Analytics practitioners and relative newbies.

Today's topic came from Max, a front-end web developer at Razor Frog web design:
<blockquote><strong><em>What is the intelligence events feature? Do any Google Analytics users actually look at this?</em></strong></blockquote>
First and foremost, let's define what intelligence events are straight from the Google support answers forum:

<a href="/wp-content/uploads/2015/03/definition-google-analytics-intelligence-events.png"><img class=" size-full wp-image-5294 aligncenter" src="/wp-content/uploads/2015/03/definition-google-analytics-intelligence-events.png" alt="definition google analytics intelligence events" width="666" height="152" /></a>

&nbsp;

In plain English: intelligence events allow you to set up custom alerts when significant changes happen on your website.

A few use cases that we have implemented for our clients:
<ol>
	<li>Revenue Spikes/Dips: For our clients that use the e-commerce tracking provided by Google Analytics, it's nice to know situations when revenue spikes or dips. We can set up automated email alerts and, if you configure your inbox correctly, these can actually push through as text messages to your mobile phone.</li>
	<li>Segmented Traffic Spikes/Dips: We like to look at search engine traffic to our clients' websites <em>every single week.</em> We have found it's handy to set up a weekly intelligence event to fire if our search engine traffic has dropped, as it allows us to diagnose the problem that week instead of waiting to pull down SEO performance at the end of the month and letting performance possibly slide any further.</li>
</ol>
Now, here's how to set up an intelligence event.
<h2>Intelligence Events: Video &amp; Step-by-Step Set Up</h2>
For the purpose of this exercise, I'm going to set up an intelligence event on our old website (retired circa January 2015) to monitor search engine traffic.

<iframe src="https://www.youtube.com/embed/ECZQmIByj5Y" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

For those who don't want to watch the video, here are the steps outlined directly from Google Analytics support forum.
<ol class="spaced-list">
	<li>Select the <strong>Reporting</strong> tab.</li>
	<li>Navigate to any one of the <strong>Intelligence Events</strong> reports (<strong>Overview</strong>, <strong>Daily</strong>, <strong>Weekly</strong>, or <strong>Monthly Events</strong>).</li>
	<li>Above the table there is a tab labeled <strong>Custom Alerts</strong>, click on that</li>
	<li>Next, you'll want to click <strong>Manage Custom Events </strong>and then, at the next screen, click the red <strong>+NEW ALERT</strong> button</li>
	<li><em>Alert name</em>: Enter a name for the alert.
<em>Apply to</em>: Select the reporting views to which you want to apply the alert.
<em>Period</em>: Select the frequency at which the alert can be generated (Day, Week, Month).
<em>Send me an email when this alert triggers</em>: Select this checkbox if you want to receive an email when the alert is generated. If you want other people to also receive email, open the <em>other email addresses</em> menu, click
Click <em>Set up your mobile phone</em> to enter your mobile phone number.
<em>Alert Conditions</em>:
<ul>
	<li><em>This applies to</em>: Select the dimension to which the alert applies.</li>
	<li><em>Alert me when</em>: Select the metric to which the alert applies, the condition that generates the alerts (e.g., Is less than, Is greater than), and enter the value for the condition (e.g., Is less than <em>20</em>).</li>
</ul>
</li>
</ol>
And there you have it! Your very own intelligence event is set up.
<h2>Any other questions?</h2>
If you have any other questions, feel free to give me a shout directly over Twitter! Reach me at <a href="http://twitter.com/mikekrass" target="_blank">twitter.com/mikekrass</a>
<h3>Transcript of Google Analytics meet up on Intelligence Events</h3>
<em>Max: For so many of our clients the dashboards are blank.</em>

<em>Mike: Yeah. [laughs]</em>

<em>Max: Like when you have 3 million visits it's much more fun to look through all the data.</em>

<em>Mike: Yeah, I picked this on purpose. Yeah. [laughs]</em>

<em>Max: It actually works.</em>

<em>Mike: Yeah. Do you guys at Razorfrog use real-time at all?</em>

<em>Max: A little bit.</em>

<em>Scott: It's like, "Oh, someone's on the desktop version of our site right now." Or, "Who's on hold?" Or, "Where are they coming from?"  </em>

<em>Steve: It's cool, but I don't have any real uses for it, personally.</em>

<em>Max: I use it for a bitcoin app, and I thought it was cool just to see people around the world using it, but no use for it really besides entertainment.</em>

<em>Mike: Do you use this at all?</em>

<em>Rob: Yeah, it was one of those things, kind of cool, but it's hard to draw any conclusions from any of the sites to this...</em>

<em>Mike: Yeah, the only way we use it at all is to QA things, primarily e-commerce, or any kind of tracking links to our site. You can go into real-time and look at conversions for example. And if I was testing something, say I made a new goal or something wasn't working in Google Analytics, I'd load up real-time on my second monitor and just watch it. And then I'd run through the conversion process and see if it popped or not.</em>

<em>Max: Yeah, it's a lot easier when you have a lot of traffic.</em>

<em>Mike: Yeah. [laughs] Yeah, because GA, normally the data that is ingested and then displayed is about three or four or five hours behind. And that's based on Pacific Time too. So sometimes when you need to QA something, it doesn't behoove you to wait six hours. You want to see if it worked right now. [laugh]  </em>

<em>Liz, you had a GA meeting this morning, didn't you?</em>

<em>Liz: No.</em>

<em>Mike: Okay.</em>

<em>Liz: Yes, sir. [laughter]</em>

<em>Mike: I'm trying to set you up.</em>

<em>Rob: Yeah, I use it for QA-ing like that too, but other use cases, just testing whether or not those pages are tagged or you can use that. I've been questioning whether it has a tag on it or not, you can just go there and you can see.</em>

<em>Male: Should it come up or not?</em>

<em>Mike: Yeah. It's in the content section; you see all these URL's that just jump up.</em>

<em>Steven: So I interviewed with some company, I don't remember what it was, but they used the real-time. They had it on a TV up a wall, and they would watch it, and that's how they would know if their site was down. They just look over, and all of a sudden...[laughter], "Oh no, we've got to go fix the site."</em>

<em>Rob: That's one way.</em><em><strong><strong> </strong></strong></em>

<em>Mike: It's like a good down detector?</em>

<em>Steven: Yeah. [laughs]</em>

<em>Female: I was going to say, it would be interesting to look at it during a cyber sale, or something like Cyber Monday or Black Friday.</em>

<em>Rob: Mm-hmm, yeah, definitely. That would be cool.</em>

<em>Mike: Especially for e-commerce you want to make sure the second that something went down you'd want to know.</em>

<em>Female: Yeah. Totally.</em>

<em>Mike: You wouldn't want to wait for a couple of minutes and then realize that you were missing out on sales.</em>

<em>Jen: we can really benefit from real?</em>

<em>Liz: Yeah, we have. [laughs]</em>

<em>Mike: You guys have some downages?</em>

<em>Natalie: Not lately, but...</em><em><strong><strong> </strong></strong></em>

<em>Natalie: ...there has been. It always seems to happen on a holiday, though, so...[laughs].</em>

<em>Liz: Not as much since we got the new websites.</em>

<em>Male: Never want to use it.</em>

<em>Max: Yeah. It only goes down when people use it. </em>