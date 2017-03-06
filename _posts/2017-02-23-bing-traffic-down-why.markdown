---
layout: post
title: "Why is my Bing traffic down? Four ways to diagnose"
date: 2017-02-23 20:15:10 -0800
categories: seo
---
We get it - everyone uses Google.

Or do they?

In the U.S. (about)[https://www.searchenginejournal.com/august-2016-search-market-share/172078/] 8 out of 10 people typically click over to Google to perform a search</a>.

This leaves a loyal audience of two out of 10 performing a search on Bing or Yahoo.

As an SEO, most clients of ours are concerned with Google. And why shouldn't they be? Typically we see a range of 80-95% of our clients' organic search traffic come from Google. So, rightfully, we're pretty zoned in on Google and what's happening from an <a href="http://www.gsqi.com/marketing-blog/google-algorithm-update-february-7-2017/">algorithm update</a> <em>(shout out to <a href="https://twitter.com/glenngabe/">Glenn Gabe</a> who is my favorite person on the Internet when it comes to giving a detailed look to new algorithm updates)</em> perspective.

But what about if you start seeing some issues with Bing organic traffic?

This post is designed with some specific knowledge in hand to help diagnose any organic search issues you may be having over at Bing / Yahoo.

<em>(Yes, Bing and Yahoo both use the same ranking algorithm.)</em>

Know that it's a separate search algorithm, so things are a little different when it comes to diagnosing why you may be seeing traffic dips or increases.

You should already have your site verified over at <a href="http://www.bing.com/toolbox">Bing Webmaster Tools</a>. If not - what are you waiting for?! It's free, and provides a wealth of information! Several of these tips also rely on tools found in this toolbox.

The following are four ways to diagnose organic search traffic patterns from Bing:
<h2>Deep-Seated Technical Website Issues</h2>
Technical website issues can kill any domain authority that a website has built up as well as stunting domain authority growth for new sites. <a href="https://www.google.com/webmasters/tools">Google Search Console</a> provides some fairly comprehensive technical reporting, from server errors, to duplicate content issues and more.

Bing Webmaster Tools also provides some great technical site reporting. And you should first look at what Bing is reporting as far as 4xx, 5xx errors and all of its error reporting and fixing those first. This is because what Bing reports, you want to fix (duh!).

What we've seen personally is that Bing tends to penalize a bit harsher when it comes to sites that have deep-seated technical issues. Things like uncrawlable AJAX or Javascript. And an issue that I've blogged about before: the <a href="/301-redirect-chains/">d</a><a href="/301-redirect-chains/">readed 301 redirect chain</a>. Usually hard to diagnose. And typically harder to even fix.

To look for redirect chain issues, I typically look at top 301 redirects reported by Bing by # of links they see. Basically - these are your high value URLs that have 301s.

<a href="/wp-content/uploads/2017/02/301-redirects-sorted-by-links.png"><img class="alignnone size-medium wp-image-6062" src="/wp-content/uploads/2017/02/301-redirects-sorted-by-links-205x300.png" alt="Bing Webmaster Tools - 301s sorted by links" width="205" height="300" /></a>

I then start plugging them into a redirect checker tool. My go to is <a href="http://www.redirect-checker.org/">Redirect Checker</a>. I'll sample about 10 or so manually, and then rely on an output from <a href="https://www.screamingfrog.co.uk/redirect-checker/">Screaming Frog SEO Spider</a> to look at site-wide redirect chains that the crawler finds.

I go over <a href="/301-redirect-chains/">how to fix 301 redirects in another post</a>. Suffice to say - it's quite a bit of work untangling the mess, especially if you're seeing four or more. I've seen a six redirect chain before; how many have you seen?

We've seen redirect chain fixes help improve rankings across the board for sites. This is due to fixing up page authority scores, which helps a domain's overall authority.

Know that technical site issues can hurt both in Google and Bing. But we've seen Bing be a bit stingier in regards to shoving down listings in the SERPs that display deep-seated issues.
<h2>Index Explorer = Better Indexation View</h2>
Bing Webmaster Tools' index explorer is awesome. Instead of a list view that Google Webmaster Tools gives, this version from Bing gives you an FTP-like view along with stats based on subfolder or subdomain views.

<a href="/wp-content/uploads/2017/02/bing-webmaster-tools-index-explorer.png"><img class="alignnone size-medium wp-image-6063" src="/wp-content/uploads/2017/02/bing-webmaster-tools-index-explorer-150x300.png" alt="Bing Webmaster Tools Index Explorer" width="150" height="300" /></a>

Instead of a .csv pull, you can easily answer questions such as:
<ul>
 	<li>"Is a specific section of the site being indexed by Bing?"</li>
 	<li>"How many links is my services section of the website receiving?"</li>
 	<li>"How many impressions are my blog posts accruing?"</li>
</ul>
You can access this view for a chosen profile at Reports &amp; Data &gt;&gt; Index Explorer.

Sometimes, you'll find that Bing isn't indexing pages that get traffic over at Google. Otherwise, this tool is a great way to ensure all of your content is included in the Bing index, and has a chance at ranking.
<h2>SEO Reports</h2>
Bing can give you their own SEO recommendations based on any URL in a profile you've verified.

You might be surprised at what they report as being an issue.

Access this tool in Bing Webmaster Tools at Reports &amp; Data &gt;&gt; SEO Reports. Enter a URL and they will tell you if there are any issues and classify each item as low / medium / high priority.


<span style="color: #ff6600;"><span style="text-decoration: underline;"><strong>Test time</strong></span>! Let's see how you do in knowing what Bing deems as<strong> low, medium or high</strong> SEO importance for elements of a web page. Highlight the area after the question to see the answer. <strong>Feel free to leave a comment below with your score out of five</strong>.</span>
<ol>
 	<li><span style="color: #ff6600;">Page is missing meta language information -- <span style="color: #ffffff;">medium priority</span></span></li>
 	<li><span style="color: #ff6600;">The &lt;img&gt; tag does not have an ALT attribute defined -- <span style="color: #ffffff;">low priority</span></span></li>
 	<li><span style="color: #ff6600;">Evaluated size of HTML is estimated to be over 125 KB and risks not being fully cached -- <span style="color: #ffffff;">low priority</span></span></li>
 	<li><span style="color: #ff6600;">The title tag is too short or too long -- <span style="color: #ffffff;">high priority</span></span></li>
 	<li><span style="color: #ff6600;">There are multiple &lt;h1&gt; tags on the page -- <span style="color: #ffffff;">high priority</span></span></li>
</ol>
<span style="color: #ff6600;">How did you score? I got a 2/5 - seriously! You bet I'd put some weight into what Bing reports as a "high priority" item, even if I don't believe it really is.</span>

<h2>Updated SERP Features</h2>
When something changes on the Google search engine result page, the search marketing hivemind goes bananas.

Case in point: a change in the color and style of the "Ad" box for AdWords text ads. <a href="http://www.thesempost.com/google-switches-adwords-ad-tags-outline-style-search-results/">1</a>. <a href="https://www.seroundtable.com/google-green-outlined-adwords-ad-label-23446.html">2</a>. <a href="https://www.seroundtable.com/google-ad-label-confuse-23456.html">3</a>.

With Bing, it's a different story. They roll out changes, additional SERP tools, or completely new SERP features and sometimes there's barely a blip on the radar.

[Case in point: I had been using Bing's Internet speed text result for about a week before it was <a href="http://searchengineland.com/bing-adds-a-internet-speed-test-tool-to-the-search-results-240138">reported by Search Engine Land</a> (c/o <a href="http://www.windowscentral.com/bing-may-be-building-speed-test-widget-within-search-results">Windows Central</a>].

<em>[Sidenote: Lo and behold, Google then started to roll out their own version <a href="https://thenextweb.com/google/2016/06/28/google-making-easy-check-internet-speed-limited-test/#.tnw_UaDm3Qe6">which was covered more extensively</a>.]</em>

The short of it is: you need to gain experience by performing some manual search queries over at Bing to sometimes find new SERP features yourself. Whereas we can rely on news outlets to cover new Google SERP changes, this isn't typically the case for Bing.

Sometimes, drops can be felt due to a change in the SERP.

Look at this carousel result showing for the query "dentists in portland or" -

<a href="/wp-content/uploads/2017/02/bing-organic-carousel.png"><img class="alignnone wp-image-6066 " src="/wp-content/uploads/2017/02/bing-organic-carousel-1024x966.png" alt="Bing organic carousel result" width="804" height="759" /></a>

Grabs up a lot of space, doesn't it?

Imagine if you were the owner of <a href="https://www.doctor-oogle.com/">Doctoroogle.com</a>. Do you think they've seen the impact of this carousel? You bet. Do you think they could have figured out why by simply looking at their web analytics and seen a drop in organic search sessions from Bing? Absolutely not.

So look at the top organic keywords by impressions and clicks both from Google and Bing and do some manual querying yourself. You might be surprised at what you see.
<h2>Conclusion</h2>
Bing is an entirely different animal than Google. Yes, it lacks the overall market share that Google has... but why ignore ~20% of your organic search audience? Follows these initial four steps if you're seeing a downward trend with Bing traffic or even an upward one to help find out why. Apply those lessons over at Google and I'm fairly certain you'll also see a nice bump in traffic over there.

And please - take our fun little Bing SEO priority quiz and let us know how you scored!
