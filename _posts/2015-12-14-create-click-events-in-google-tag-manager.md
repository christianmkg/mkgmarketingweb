---
ID: 5676
post_title: 'The 121 Second Guide to Create &#038; Deploy Click Events in Google Tag Manager'
author: Mike Krass
post_date: 2015-12-14 07:02:42
post_excerpt: ""
layout: post
permalink: >
  /create-click-events-in-google-tag-manager/
published: true
views:
  - "706"
enclosure:
  - |
    /wp-content/uploads/2015/12/google-tag-manager-mkg-marketing-inc-create-click-class-trigger.mp4
    11586096
    video/mp4
    
  - |
    /wp-content/uploads/2015/12/google-tag-manager-mkg-marketing-inc-create-click-event-tag.mp4
    1654949
    video/mp4
    
---
<h2>The 121 Second Guide to Create &amp; Deploy Click Events in Google Tag Manager</h2>
It's taken a few years, but with Google Tag Managers v2 release we've begun to see more documentation about how to properly deploy tag, create triggers and variables and generally make use of Google Tag Manager (GTM).
<blockquote>
<p class="p1">This guide will teach you how to deploy a Click Event in GTM that reports into your Google Analytics.</p>
</blockquote>
<p class="p1">Common use cases for this implementation include:</p>

<ul>
	<li class="p1">Tracking key button clicks on a website</li>
	<li class="p1">Tracking where users tap on their screen on mobile devices</li>
</ul>
<h2>Step 1: Create a Click Event Trigger in Google Tag Manager</h2>
<p class="p1">TL;DR Click the image below to watch a 72 second video below to learn how to create a click event trigger.</p>
[video width="2542" height="1280" mp4="/wp-content/uploads/2015/12/google-tag-manager-mkg-marketing-inc-create-click-class-trigger.mp4"][/video]
<p class="p1">For the purpose of this tutorial, let's assume that you want to create a Google Analytics event <em>that fires every single time </em>somebody clicks on the big orange 'Contact' button on our website.</p>
<p class="p1">Your first step in this process is to find the Click Class. Follow these three steps:</p>

<ul>
	<li class="p1">Open up the Chrome browser</li>
	<li class="p1">Right click on the element you want to track - in this case our orange Contact button - and click 'Inspect Element'</li>
	<li class="p1">Chrome DevTools will pop up and you'll see a  named Class. Copy that name.</li>
</ul>
Now that you've got your Click Class handy, you'll want to navigate back to Google Tag Manager.
<ul>
	<li>Select 'Triggers'</li>
	<li>'New' (big red button)</li>
	<li>Name your trigger "GA - Contact Button Clicks"</li>
	<li>Select 'Click' as your event type in step 1</li>
	<li>Targets dropdown should be set to 'Just Links'</li>
	<li>Leave the 'Wait for Tags' and 'Check Validation' alone and click 'Continue'</li>
	<li>In Step 3, Enable when should be set to 'Click Classes' contains [insert Click Class here from your Inspect Element step above]</li>
	<li>Finally in step 4, fire on URL matches RegEx (regular expression) .* to fire on all pages of your website.</li>
</ul>
<h2>Step 2: Create a Tag in Google Tag Manager</h2>
<p class="p1">Think of your Trigger as the first domino - it is the catalyst that sparks change down the line. It tells your <em>Tag </em>that it needs to fire when certain conditions are met.</p>
<p class="p1">So now it's time to make that Tag!</p>
<p class="p1">TL;DR Watch the 49 second by clicking on the photo below to learn to make an Event Tracking tag in Google Analytics.</p>
[video width="1996" height="1244" mp4="/wp-content/uploads/2015/12/google-tag-manager-mkg-marketing-inc-create-click-event-tag.mp4"][/video]
<ol>
	<li class="p1">Navigate to Tags option on the lefthand side</li>
	<li class="p1">Click 'New'</li>
	<li class="p1">Select 'Google Analytics'</li>
	<li class="p1">Choose 'Universal Analytics'</li>
	<li class="p1">Input your Tracking ID - I have mine saved as a variable so ignore the {{gaProperty}} text you see in the screengrab</li>
	<li class="p1">Configure tag type in the Track Type dropdown. Select 'Event'</li>
	<li class="p1">Category, Action and Label are for your own convenience. Name them something that will remind you what is being reported in Google Analytics.</li>
	<li class="p1">Finally at Step 4, 'Fire On', scroll over to the 'More' option and select the Trigger we created earlier</li>
	<li class="p1">Finish up by clicking the blue 'Create Tag' button</li>
</ol>
<h2>Step 3: Debugging and Quality Assurance (QA)</h2>
Use the preview mode provided by GTM to see the tags fire. Secondary debugging tool is the Chrome DevTools extension (Command + Option + I on a Mac).

Voila! There you have it :)
<p class="p1"></p>