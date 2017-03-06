---
ID: 4188
title: >
  How to Customize Sidebars in Squarespace
  6 Using CSS
author: KerryGuard
date: 2014-02-25 06:17:44

layout: post
permalink: >
  /how-to-customize-sidebars-in-squarespace6-using-css/
published: true
views:
  - "56"
---
<h3>The Challenge of Using CSS in Squarespace 6</h3> 

<p>Running several blogs under one Squarespace 6 site allows for a lot of reuse; however there are some limitations such as tweaking the sidebar on a per-blog basis that are still challenging for developers to work through.</p>

<h3>The Solution</h3>

<p>A combination of ids and classes in the HTML allows some flexibility in customizing the output, providing you have some basic familiarity with cascading style sheets (CSS).</p>

<p>The simplest option is to add all the elements you need across multiple blogs into a single sidebar and then use the CSS display attribute to hide them by default. You can also selectively show these display attributes for the right blog using display: none and display: block respectively.</p>

<p>Identifying the correct classes can be a little tricky given the almost-random names that Squarespace assigns, but here are the steps to identify these and have them switch as you navigate between the blogs.</p>

<!--more-->

<h4>Locate the CSS Editor</h4>

<ol>
<li>View one of your blogs.</li>
<li>Find the menu bar at the bottom right</li>
<li>Click on the paint brush for style mode</li>
<li>A menu system will push out from the left; scroll to the bottom and click the button that says Custom CSS</li>
<li>An alert will pop up asking if you're sure you want to edit; say yes because you're not overriding visual elements, you're just hiding and displaying certain ones at certain times.</li>
</ol>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/02/Screen-Shot-2014-02-22-at-4.57.01-PM.png" alt="Squarespace 6 Custom CSS Button"/>

<h4>Find and Document the Collection Ids</h4>
<p>When you're in the Squarespace editor, select one of your blogs, and in the url, you'll see the Collection ID</p>

<img src="http://mkgmediagroup.com/wp-content/uploads/2014/02/Screen-Shot-2014-02-22-at-5.03.06-PM.png" alt="Squarespace 6 Collection ID URL"/>

<p>Within the CSS editor in Square Space, note each Collection ID and label with comments. You'll reference these every time you show an element so best to take note now.</p>

<pre>
<code>
/*Sidebars are:
Blog A.collection-52e813a1e4b09717e21eaaaa
Blog B.collection-52e813a3e4b09717e21ebbbb
Blog C.collection-52e813a3e4b09717e21ecccc
*/
</code>
</pre>

<h4>Find the Block IDs</h4>
<p>Make sure your sidebar has all the elements set up. Each blog should show all the elements for the other blogs. It may feel clunky. This is what we're out to fix.</p>
<p>Once all your elements are in place you'll locate the Block Id for each one:</p>
<ol>
<li>Highlight the first element</li>
<li>Right click (on an Mac track pad, click with two fingers)</li>
<li>Select Inspect Element</li>
<li>Go up a few levels within the HTML until you find the div with ID Block</li>
<li>Repeat for all elements you want to show or hide depending on the blog</li>
</ol>
<br>
<img src="http://mkgmediagroup.com/wp-content/uploads/2014/02/Screen-Shot-2014-02-22-at-3.11.08-PM.png" alt="Squarespace 6 ID Block Finder"/>

<h4>Display: None is Your New Best Friend</h4>
<p>Go back to your CSS editor and use the following code to hide all the RSS feeds for each blog.</p>

<pre>
<code>
* RSS sidebar *
#block-e6e370ea67acf3ad6513, /* Blog A RSS */
#block-7c894207de8f679f3ccb, /* Blog B RSS */
#block-5f9c12ebf5cd49212e99 /* Blog C RSS */ {
	display: none;
	}
</code>
</pre>

<h4>Display: Block is Where the Magic Happens</h4>
<p>Remember those Collection IDs you took note of? You'll need those now.</p>
<p>You're simply going to say, when you're on blog A, show element for blog A.</p> 

<pre>
<code>
.collection-52e813a3e4b09717e21eaaaa #block-e6e370ea67acf3ad6513,
.collection-52e813a1e4b09717e21ebbbb #block-7c894207de8f679f3ccb,
.collection-52e813a3e4b09717e21ecccc #block-5f9c12ebf5cd49212e99 {
	display: block;
	}
</code>
</pre>

<h4>Save and Review</h4>
<p>Click save at the bottom of your CSS editor and go review each blog making sure each element is where it should be</p>
<p>I recommend opening an Incognito Window in Chrome (File -> New Incognito Window). This allows you to see your blogs as your readers will.</p>