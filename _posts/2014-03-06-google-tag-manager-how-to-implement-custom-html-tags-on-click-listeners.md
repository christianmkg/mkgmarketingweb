---
ID: 4259
title: 'Google Tag Manager: How to Implement Custom HTML Tags on Click Listeners'
author: Kerry Guard
date: 2014-03-06 06:56:57

layout: post
permalink:
  /google-tag-manager-how-to-implement-custom-html-tags-on-click-listeners/
published: true
views:
  - "732"
---
<p>For all it's wonder and glory, there's one thing missing from the Google Tag Manager product.</p>

<blockquote><em>Detailed Q&A forums!</em></blockquote>

<p>We utilize Google Tag Manager (GTM) for the majority of our clients; it reduces the number of IT requests put in to engineering, helps us securely manage marketing tags across the entirety of our clients' websites, and ensures that we don't slow down our client's website with too many marketing tags.</p>

<p>But for the life of us, we cannot figure out why there isn't more troubleshooting assistance from Google (Google Product forums and elsewhere) available to loyal users of this product like ourselves.</p>

<!--more-->

<p>That being said, we've decided to create Google Tag Manager University -- any time we run into a problem and find a solution to a GTM issue we'll blog about it on our site.</p>

<p>Today's issue revolves around ...</p>

<h3>How to Implement a 3rd Party HTML Tag on to a Click Listener</h3>

<p>For starters, let's define a click listener:</p>

<ul>
	<li>Part of the event listener library of functions within Google Tag Manager, an event listener allows marketers to tag website actions without bothering engineering</li>
	<li>A click listener specifically allows marketers to track clicks (buttons, links, etc) on a single page</li>
</ul>

<p>Now, the issue with implementing a custom HTML tag on a click listener is that it's actually a three step process that isn't entirely clear until you've gone through it a few times.</p>

<p>Those steps are:</p>

<ol>
	<li>Create a click listener with properly formatted firing rules</li>
	<li>Create a custom HTML tag tag and drop in your 3rd party HTML or image source code</li>
	<li>Create a tag version and publish it live to the web</li>
</ol>

<h3>How to create a click listener in GTM</h3>

<p>Let's visually walk through the steps to creating a click listener in Google Tag Manager.</p>

<H4>Step 1: After logging in to your Google Tag Manager account, click the icon that reads 'create' and select 'tag'.</h4>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/1.-1.2-google-tag-manager-create-tag.png" alt="google tag manager create tag"/>

<h4>Step 2: Name your click listener</h4>

<p>Give your click listener a name that will help remind everybody what you are measuring. It's better to be too specific than not specific enough!</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/name-click-listener-event-listener-tag-google-tag-manager.png"/>

<h4>Step 3: Select the tag type</h4>

<p>There will be an empty menu for a drop down labeled 'Tag Type'. Click on that drop down menu and scroll down to Event Listener >> Click Listener.</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/3-event-listener-google-tag-manager.png" alt="event listener google tag manager"/>

<h4>Step 4: Create a firing rule</h3>

<p>A firing rule tells this tag when to activate itself -- how should it know to record an activity on your website without a firing rule?</p>

<p>Hover to the top right part of your new tag screen and click on 'add rule'.</p>

<p>This will pop up a check box that allows you to select from existing rules or to create a new firing rule. For this example, we'll create a new rule to fire the tag when somebody reaches 'http://xyz.com', our clients website.</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/create-new-firing-rule-google-tag-manager.png" alt="create new firing rule google tag manager"/>

<p>One thing to note: you might want to uncheck the box that reads 'check validation' but leave 'wait for tags' checked.</p>

<p>Then, you simply need to hit 'save' to save that tag you just created.</p>

<p>Voila! You have created a click listener tag!</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/save-google-tag-manager-tag.png" alt="save google tag manager tag"/>

<h3>How to create and implement a custom HTML tag to fire 3rd party code snippets</h3>

<h4>Step 1: Create a new click tag</h4>

<p>At your account's home screen, navigate to the red 'new' button and click on 'tag'. This will get you started to create that custom HTML tag you'll need to properly fire your 3rd party code.</p>

<h4>Step 2: Create a custom HTML tag</h4>

<p>After you get to the 'new tag' screen, you'll want to name your custom HTML tag. Following that process, click on the 'tag type' drop down and select 'custom HTML tag'.</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/2.2-create-custom-HTML-tag.png" alt="create custom HTML tag"/>

<h4>Step 3: Drop in 3rd party code snippet</h4>

<p>Now it's time to drop in your 3rd party code. Remember, if it's a Javascript snippet you'll want to add script open and close elements appropriately.</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/step-3-drop-in-third-party-code-snippet.png" alt="google tag manager third party code snippet"/>

<h4>Step 4: Add the correct firing rule to the custom HTML tag</h4>

<p>This is perhaps one of the most important steps; you need to add the following firing two conditions as a firing rule to get your tag to work.</p>

<p>Those conditions are:</p>

{% raw %}
<pre>
<code>
{{event}} equals gtm.linkClick
{{element url}} contains "<EXAMPLE: USE URL OF YOUR OWN WEBPAGE>"
</code>
</pre>
{% endraw %}

<p>This rule tells your tag to fire every time someone clicks on a link whose href contains the string of your link destination.</p>

<p>In our case, that would be "EXAMPLE: USE URL OF YOUR OWN WEBPAGE", although you all know that it should be a properly formatted URL such as 'http://xyz.com'</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/step-4-create-firing-rule.png" alt="Google Tag Manager Firing Rule gtm.linkClick"/>


<h4>Last steps to implement this rule</h4>

<p>Last but not least, you'll need to do create a new version of all these tags.</p>

<p>At the home screen, click on 'create a new version':</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/google-tag-manager-create-container-version.png" alt="google tag manager create container version"/>

<p>Now, you'll need to publish your container so that tag and it's attached rules actually go live on the web.</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/03/7-publish-google-tag-manager-container.png" alt="publish google tag manager container"/>

<h3>There you have it!</h3>

<p>Using a de-bugging tool like <a href="https://chrome.google.com/webstore/detail/tag-assistant-by-google/kejbdjndbnbjgmefkgdddjlbokphdefk?hl=en" target="_blank">Google Tag Assistant</a> (Chrome browser extension) or <a href="https://www.ghostery.com/" target="_blank">Ghostery</a> (Chrome/Firefox browser extension), you should be able to navigate through your site, click on the link you just created a rule for and watch the click listener and 3rd party code snippet fire.</p>

<p>For those who are more inclined to watching this via video, I've actually gone through and recorded myself doing these tasks in the video below.</p>

<p><iframe width="853" height="480" src="//www.youtube.com/embed/AEtFV3Ipklw?rel=0" frameborder="0" allowfullscreen></iframe></p>

<h3>Share any questions, comments or concerns in our comments sections below!</h3>
