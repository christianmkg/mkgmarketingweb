---
ID: 5424
post_title: 'QA Optimizely Experiments: A 3-Step Guide'
author: Mike Krass
post_date: 2015-04-27 06:59:47
post_excerpt: ""
layout: post
permalink: >
  http://mkgmarketinginc.com/qa-optimizely-experiments/
published: true
views:
  - "2246"
---
<h1>How do you QA your A/B testing experiments?</h1>
When we first tried out <a href="http://optimizely.com" target="_blank">Optimizely</a>, an A/B testing tool, all we thought we had to do was to navigate to the 'Preview' option of the experiment variation and take a quick peak to QA the experiment.
<blockquote><em>Wrong!!!!!!</em></blockquote>
Over the years, we've learned that the good-old-fashioned preview feature is only one of three different ways to perform quality assurance checks on your A/B testing experiments.
<h2>Enter: The 3 Step QA Process</h2>
As we have built and refined our own <a title="Conversion Rate Optimization" href="http://mkgmarketinginc.com/case-studies/conversion-rate-optimization/" target="_blank">conversion rate optimization</a> process over the past three years, we discovered there were three critical step to QA Optimizely experiments.

Those steps are...
<ol>
	<li>Viewing an experiment in the Preview pane</li>
	<li>Testing across multiple browsers and OS's</li>
	<li>Using a Force Parameter to load a paused experiment on a live staging URL</li>
</ol>
In order for an experiment to be cleared for takeoff, our QA process dictated that it needed to pass all three steps in our QA process from a minimum of <em>two </em>different members of the <a href="http://mkgmarketinginc.com" target="_blank">MKG</a> team.

That being said, here is the order of operations we follow each time we QA an experiment.
<h2>Step #1: The Preview Pane</h2>
This is probably the easiest step in the process: Using the preview feature within your experiment.

<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/04/Preview-feature-of-Optimizely.png"><img class="alignleft size-full wp-image-5449" src="http://mkgmarketinginc.com/wp-content/uploads/2015/04/Preview-feature-of-Optimizely.png" alt="Preview feature of Optimizely" width="209" height="70" /></a>

&nbsp;

&nbsp;

&nbsp;

When we click on 'Preview', we're really looking for a few things:
<ol>
	<li>Design: How does my design look? Sometimes this can change from the small-screen editor view to the blown up browser view that your site visitors will see.</li>
	<li>Interaction: Do all the links click through, videos play, and interactive elements of the page operate as they should?</li>
</ol>
You can watch me mess around with the Preview feature at the 1:05 mark in the video below:

https://youtu.be/b8m7nRobED8?t=1m4s

Once you have checked the design and interaction within Preview, it's time to move on to the Cross Browser Testing step.
<h2>Step #2: Checking Experiments Across Browsers &amp; Operating Systems</h2>
Did you know that Optimizely has a partnership with <a href="http://crossbrowsertesting.com" target="_blank">crossbrowsertesting.com</a> that makes their tool <i>free </i>for you?

Yup, that little link there!

<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/04/cross-browser-and-OS-testing-.png"><img class=" size-full wp-image-5450 aligncenter" src="http://mkgmarketinginc.com/wp-content/uploads/2015/04/cross-browser-and-OS-testing-.png" alt="cross browser and OS testing" width="442" height="308" /></a>

&nbsp;

Before Optimizely plugged that feature into the experiment editor, we used to have to load up a few virtual machines in Parallels Desktop, fire up every version of Internet Explorer, Firefox, Chrome and Safari across both Windows <em>and </em>Mac in order to get a feel for how our experiment would render across browsers and operating systems.
<blockquote><em>No more I say!</em></blockquote>
When you click on the cross-browsing testing option, you'll be taken to a web page that looks a little something like this (give it about 2 minutes to load):

<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/04/Screengrabs-from-Cross-Browser-Testing.com_.png"><img class="alignleft size-full wp-image-5451" src="http://mkgmarketinginc.com/wp-content/uploads/2015/04/Screengrabs-from-Cross-Browser-Testing.com_.png" alt="Screengrabs from Cross Browser Testing.com" width="1012" height="685" /></a>

When we review the experiment across browsers and OS's, we look for a few things:
<ol>
	<li>Mobile versus Desktop: How does this experiment render across both mobile and desktop devices? Oftentimes, we'll scrap the mobile version of the experiment <em>or </em>create a specific experiment <em>only for mobile devices.</em></li>
	<li>Design versus Code: A regular issue we run into is that we used the 'Move &amp; Rearrange' feature in the editor to move a button or block of text around the page. This will render differently across different browsers and OS's. Check your intended design versus the code output that browsers interpret for site visitors.</li>
	<li>Windowed versus Full Page: The windowed view is essentially your 'above the fold' look at the experiment. Full page allows you to see the entire page, which is obviously better if you made changes deeper into the page.</li>
	<li>Pro Tip: Completely <strong>ignore Windows Vista and XP </strong>screenshots. For reasons unknown to me, those two versions of Windows absolutely destroy your design. Fortunately for you, not many people still use <a href="http://www.worldstart.com/how-many-people-still-use-vista/" target="_blank">Vista or XP</a> :-)</li>
</ol>
One last word to the wise: There is a super handy 'download zipped screenshots' link at the bottom of the screenshot panel. We sometimes download these screenshots in order to pass them along to a client for approval or simply keep for our own QA-ing records.

<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/04/download-linked-screenshots-cbt.com_.png"><img class="alignleft size-full wp-image-5452" src="http://mkgmarketinginc.com/wp-content/uploads/2015/04/download-linked-screenshots-cbt.com_.png" alt="download linked screenshots cbt.com" width="547" height="343" /></a>

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;
<h2></h2>
<h2>Step #3: Using the force parameter</h2>
This is a trick that the Optimizely support team mentioned to us in a recent Optiverse Q&amp;A session.
<blockquote><em>In essence, a force parameter allows you to force yourself to see a specific variation, even when it's paused.</em></blockquote>
You can read their <a href="https://help.optimizely.com/hc/en-us/articles/200107480),?flash_digest=39641d7993daea802bd898606f6b0378f4be5f94" target="_blank">official documentation on that process here,</a> and we've outlined the steps to use the force parameter to perform QA below.

<strong>Step 1: Enable Force Parameter in your Optimizely Account</strong>

Navigate to "Settings", then "Privacy" and then un-check the box marked "Disable the Force Variation Parameter" and hit the blue "Save" button.

By default, this feature is not available in your Optimizely account. And for good reason! If anybody was wise enough to use a force parameter, they could look at all of the experiments you have built in Optimizely even if you did not publish them.

<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/04/Force-URL-Parameter-in-Optimizely-2.png"><img class=" size-full wp-image-5454 aligncenter" src="http://mkgmarketinginc.com/wp-content/uploads/2015/04/Force-URL-Parameter-in-Optimizely-2.png" alt="Force URL Parameter in Optimizely - 2" width="801" height="563" /></a>

<strong>Step 2: Firing a Paused Experiment into a Live Staging Link</strong>

Alright, now you've got Optimizely all set up to allow you to use force parameters.

So what does this actually look like?

A force parameter is comprised of three elements:
<ol>
	<li>Simple match experiment URL: This is the URL the experiment is running on</li>
	<li>?optimizely_xEXPERIMENTID: The specific experiment ID</li>
	<li>=VARIATIONID: The variation you want to fire. Using a tab system, Optimizely counts from left to right; from 0 to 1 to 2 to 3 ... As a rule of thumb, your original is always variation zero.</li>
</ol>
Wait ... what???

It'll look a little something like this:

<a href="http://mkgmarketinginc.com/wp-content/uploads/2015/04/sample-force-parameter-URL.png"><img class="alignleft size-full wp-image-5456" src="http://mkgmarketinginc.com/wp-content/uploads/2015/04/sample-force-parameter-URL.png" alt="sample force parameter URL" width="574" height="74" /></a>

&nbsp;

&nbsp;

Step-by-step, here is how you'll find the force parameter for your experiment.
<ol>
	<li>Open a tab in your browser and enter the simple match URL that you are experimenting on into the address bar.</li>
	<li>In a separate tab, log into Optimizely and choose an experiment.</li>
	<li>Go into 'Editor' mode.</li>
	<li>Click on 'Options' dropdown on the far right and find 'Diagnostic' report.</li>
	<li>Once you click on 'Diagnostic', you'll see a 9-digit 'Experiment ID' number. Write that down.</li>
	<li>Choose the variation you'd like to see. Is it a simple A/B test? Then variation zero is your original, and variation 1 is represented by the number 1.</li>
	<li>Compile your force parameter URL and, opening a third tab in your browser, enter it into the address bar and hit enter.</li>
</ol>
If this is a bit confusing, you're not alone. It took me quite some time to get used to this process. That's why we recorded this process :-)

<iframe src="https://www.youtube.com/embed/b8m7nRobED8" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
<h2>There you have it!</h2>
This is our three-step process to ensure every single conversion optimization experiment we launch is properly QA'd before hitting the 'Start' button.

Out of curiosity, how do the conversion marketers reading this post perform quality control checks on A/B testing activity?