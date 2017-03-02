---
ID: 5612
post_title: >
  Creating a New Google Analytics Property
  Using Google Tag Manager (GTM)
author: Jessica Ward
post_date: 2015-11-09 07:22:50
post_excerpt: ""
layout: post
permalink: >
  http://mkgmarketinginc.com/creating-a-new-google-analytics-property-using-google-tag-manager-gtm/
published: true
views:
  - "680"
---
Understanding how many people visit your website and what they do when they get there is important for everyone from the part-time blogger to the corporate CEO.
<blockquote>That's where Google Analytics comes into play - a robust, free tool that can help you understand the performance of your website.</blockquote>
This tutorial will help you create a new Google Analytics property using Google Tag Manager (GTM).
<h2>Step 1: Create New Property in Google Analytics</h2>
<ol>
<ol>
	<li>Go to the Admin section of <a href="http://www.google.com/analytics/" target="_blank">Google Analytics</a> and ensure you are in the correct account.</li>
</ol>
</ol>
<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GA-Create-New-Property.png"><img class="aligncenter size-full wp-image-5624" src="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GA-Create-New-Property.png" alt="Google Analytics - Create New Property" width="2846" height="1970" /></a>
<ol>
	<li>Click on Create New Property and complete the form for the new property.</li>
	<li>Make note of the new property Tracking ID -<span style="text-decoration: underline;"><em> designated with UA.</em></span></li>
</ol>
<h2>Step 2: Create New Container in GTM</h2>
<ol>
<ol>
	<li>Login to Google Tag Manager and scroll down to the correct account.</li>
	<li>Click on Create Container and complete the form for the new container.</li>
</ol>
</ol>
<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-Account.png"><img class="aligncenter size-full wp-image-5626" src="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-Account.png" alt="Google Tag Manager - Account" width="2704" height="1208" /></a>
<ol>
	<li>Click on the new container name to update the tags and rules for it.</li>
</ol>
<h2>Step 3: Place GTM Code on Website</h2>
<ol>
<ol>
	<li>In the Admin tab for your new container, click on Install Google tag Manager to get your GTM code.</li>
</ol>
</ol>
<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-Admin.png"><img class="aligncenter size-full wp-image-5633" src="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-Admin.png" alt="Google Tag Manager - Admin" width="2764" height="1970" /></a>
<ol>
	<li>Copy the code and paste it on all pages of your website immediately following the opening tag. For more information on installing the GTM code, visit the <a href="https://developers.google.com/tag-manager/quickstart" target="_blank">GTM Quick Start Guide</a>.</li>
</ol>
<h2>Step 4: Create a New Tag in GTM</h2>
<ol>
<ol>
	<li>In the Container Overview, click on Add a New Tag.</li>
</ol>
</ol>
<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-Container.png"><img class="aligncenter size-full wp-image-5634" src="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-Container.png" alt="Google Tag Manager - Container Overview" width="2758" height="1628" /></a>
<ol>
<ol>
	<li>Complete the form for Google Analytics &gt; Universal Analytics with the GA Tracking ID from Step 1.
<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-GA-Tag-SetUp.png"><img class="aligncenter size-full wp-image-5635" src="http://mkgmarketinginc.com/wp-content/uploads/2015/10/GTM-GA-Tag-SetUp.png" alt="Google Tag Manager - Google Analytics Tag SetUp" width="2764" height="1970" /></a></li>
</ol>
</ol>
Ensure the following settings are enabled
<ol>
<ol>
<ul>
	<li>Display Advertising Features</li>
	<li>Tracking Type is Pageview</li>
</ul>
</ol>
</ol>
&nbsp;
<ol>
	<li>For part four of the form, Fire On, select All Pages and click on Create Tag.</li>
</ol>
<h2>Step 5: Publish Container</h2>
Once you have ensured the first four steps have been completed, click the red publish button in the top right corner of your Google Tag Manager account.
<h2></h2>