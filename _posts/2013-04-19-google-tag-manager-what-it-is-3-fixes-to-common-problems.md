---
ID: 2541
post_title: 'Google Tag Manager: What It Is &#038; 3 Fixes to Common Problems'
author: Kerry Guard
post_date: 2013-04-19 06:00:52
post_excerpt: ""
layout: post
permalink: >
  http://mkgmarketinginc.com/google-tag-manager-what-it-is-3-fixes-to-common-problems/
published: true
seo_title:
  - 'Google Tag Manager: What It Is & 3 Fixes to Common Problems | MKG Media Group'
seo_description:
  - >
    Read about what Google Tag Manager is,
    three fixes to common problems users
    tend to have with the product, and to
    see if using GTM is something you should
    do.
ppw:
  - >
    http://mkgmediagroup.com/wp-content/uploads/2013/04/tags.jpg
views:
  - "3016"
---
<p>We here at MKG Media Group are big fans of deploying Google Tag Manager on our clients' websites.</p>

<p>First, if you're unfamiliar with what Google Tag Manager (GTM) is, this is how Google describes their product:</p>

<p><em>"Google Tag Manager makes it easy for marketers to add and update website tags -- including analytics, remarketing, and more & with just a few clicks, and without bugging the IT folks."</em></p>

<p>Sounds pretty sweet, right? It is! GTM code acts as a tag management system that places a "container" tag on your web page. Once in place, you're able to specify rules as to when you want specific pieces of code to show up in the container, such as:</p>

<ol>
	<li>Set up rules that have Google Analytics code fire on every page of a website</li>
	<li>Set up a rule that lets AdWords conversion code fire whenever someone hits a "thank you" page.</li>
</ol>

<p><strong>Hashtag done</strong></p>

<p>However, <em>things aren't so cut and dry with GTM</em>. The support documentation is lacking in some critical areas. The following are some answers to questions those who are thinking of using GTM might have that Google doesn't have any support documentation around.</p>

<h3>Using Google Tag Manager on HTTPS pages</h3>
<p>If you're going to be placing GTM code on a secure web page (https), then you'll need to make a small tweak to your Google Tag Manager code in order for it to work.</p>

<p>There are two instances in the Google Tag Manager code that starts with "src=". Change the following "//www" to "https://www" for both.</p>

<p>This will then allow the GTM container code to accurately display on a secure web page.</p>

<h3>I use MediaMind Ad Server and wish to use GTM to deploy that code. Can I?</h3>

<p>Yes you can... but you need to tweak two lines of code.</p>

<p>First, you need to place the code in a custom image tag. This is an option you can select when creating a new tag. Then copy / paste the code that was given to you from MediaMind. Now, you'll need to replace this line of code:</p>

<p><em>document.write('&lt;scr'+'ipt src="HTTP://bs.serving-sys.com/BurstingPipe/ActivityServer.bs?cn=as&amp;ActivityID=XXXXX&amp;rnd=' + ebRand + '"&gt;');</em></p>

<p>With this line of code:</p>

<p><em>jQuery.getScript("HTTP://bs.serving-sys.com/BurstingPipe/ActivityServer.bs?cn=as&amp;ActivityID=XXXXX&amp;;rnd=" + ebRand);</em></p>

<p>Do know you need to place the correct ActivityID (which I have as XXXXX in the examples) in the tweaked line of code in order to track the desired activity.</p>

<h3>How can I easily check if GTM is installed properly?</h3>
<p>We like two specific Chrome extensions: Google Tag Assistant and Ghostery. The pros &amp; the cons are:</p>

<ol>
	<li><span style="line-height: 1.5em;">Google Tag Manager will only report on Google-specific code</span></li>
	<li><span style="line-height: 1.5em;">Ghostery will report on a whole slew of different code types, including beacons, advertising tags, privacy trackers and widgets</span></li>
</ol>

<p>You can find Google Tag Assistant <a href="https://chrome.google.com/webstore/detail/tag-assistant-by-google/kejbdjndbnbjgmefkgdddjlbokphdefk?hl=en" target="_blank">here</a> and Ghostery <a href="https://chrome.google.com/webstore/detail/ghostery/mlomiejdfkolichcflejclcbmpeaniij?hl=en" target="_blank">here</a>.</p>

<h3>Should I look to deploy GTM for my own / clients' websites?</h3>
<p>Yes and no. If you fall under the following scenarios, we would recommend looking to use GTM:</p>
<ul>
	<li><span style="line-height: 14px;">Running paid search and are using conversion codes</span></li>
	<li>Running a retargeting or remessaging program (get tags on specific pages with burn pixels to stop remarketing to customers who have already converted)</li>
	<li>Have a possible need of adding code to a client's website in the future</li>
</ul>
<p>If you have any questions, we've certainly built up quite a bit of knowledge about GTM and are happy to help. Feel free to contact me (social media links below) or comment on this blog post.</p>