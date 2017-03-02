---
ID: 4954
post_title: 'How Twitter Generated 10x Visitors from SEO: Our Thoughts'
author: Kerry Guard
post_date: 2014-11-12 16:32:20
post_excerpt: ""
layout: post
permalink: >
  http://mkgmarketinginc.com/how-twitter-generated-10x-visitors-from-seo-thoughts/
published: true
views:
  - "263"
---
<p>Not sure if you read the news, but <a href="http://searchengineland.com/twitter-seo-more-visitors-208160" target="_blank">Twitter recently announced</a> that they "made a change earlier this year to ensure that search engines like Google and Bing could better access 50,000 popular hashtag pages" and due to this change have had a return of 10x of organic search traffic to those pages.</p>

<p><strong>10x!</strong></p>

<p>That's 100 instead of 10. 1,000 instead of 100. But in Twitter's case, the traffic impact is:</p>

<p>75,000,000 instead of 7,500,000.</p>

<p>WOW! What an extra zero that is!</p>

<p>Naturally, the company didn't say what they did to increase traffic to their most popular 50,000 hashtag pages... so we did some digging. And while we can't say what exactly lead to this big increase, we have a couple of hypotheses.</p>

<!--more-->

<p><h2>Hypothesis #1: a simple Robots.txt change</h2></p>

<p>I love robots.txt files. This is a public-facing file that taps into the psyche of a website's SEO. Looking through Twitter.com's robots.txt file, I found an interesting command:</p>

<p><a href="http://mkgmediagroup.com/wp-content/uploads/2014/11/twitter-robots-txt-file.png"><img src="http://mkgmediagroup.com/wp-content/uploads/2014/11/twitter-robots-txt-file.png" alt="twitter robots txt file contents" width="542" height="510" class="aligncenter size-full wp-image-4956" /></a></p>

<p>Unfortunately, I can't see a historical look at what this robots.txt file had before Twitter got this 10x boost... but those two "allow commands" are almost marching orders for search engines to go to those subdomains and crawl that content. I wonder if making this simple change to their robots.txt file helped guide spiders to these subfolders whereas previously twitter was just hoping that search engines would crawl these two money content spots.</p>

<p><h2>Hypothesis #2: Google being Google</h2></p>

<p>If you do a search for #cometlanding on Google, you'll see this result on the search engine result page (SERP):</p>

<p><a href="http://mkgmediagroup.com/wp-content/uploads/2014/11/hashtag-comet-landing.png"><img src="http://mkgmediagroup.com/wp-content/uploads/2014/11/hashtag-comet-landing.png" alt="twitter hashtag cometlanding #cometlanding" width="926" height="160" class="aligncenter size-full wp-image-4957" /></a></p>

<p>Additionally, if you perform other hashtag+words searches, you'll find similar results for twitter that resemble that same structure of:</p>

<p><strong>Title tag</strong>: Tweets about (hashtag) hashtag on Twitter</p>
<p><strong>Meta description</strong>: The latest and best Tweets on (hashtag). Read what people are saying and join the conversation.</p>

<p>Sniffs like templatized recs for all hashtag pages, which is entirely A-OK. What doesn't really check out is that meta description tag... specifically: it appears nowhere in the page code. No actual meta description in place for each hashtag page and certainly not that text.</p>

<p>So where is it coming from?</p>

<p>Well, think of it this way: Google is in the business of giving users the best search engine experience possible. Why? Because a happy Google searcher equals a returning Google search user. Perhaps Google knows that whenever someone is searching for #SOMETHING, they're looking for a hashtag on twitter. Wouldn't be the craziest thing in the world to think. So perhaps Google has some kind of rule in place to always look to add that snippet in search results because they believe it gives the correct context to the user on the content for the twitter hashtag page. Maybe a bit of a tinfoil hat thought here, but when you don't find references to this phrase in the code, you have to start reaching for the hat.</p>

<p><h2>Hypothesis #3: Addition of link rel="search"</h2></p>

<p>A rel=search tag is a way for site owners to instruct how a browser could create a URL to search the current site for any given keyword. In the case of a Twitter hashtag page, the command they use is:</p>

<p><a href="http://mkgmediagroup.com/wp-content/uploads/2014/11/twitter-rel-search-tag.png"><img src="http://mkgmediagroup.com/wp-content/uploads/2014/11/twitter-rel-search-tag-1024x58.png" alt="twitter rel=search tag on hashtag pages" width="1024" height="58" class="aligncenter size-large wp-image-4958" /></a></p>

<p>To quickly deconstruct this order, basically, the code is saying to go to this URL to construct the page in a way search engines can understand: https://twitter.com/opensearch.xml.</p>

<p>Now if we go to that page, we see some commands that are given on how to construct the URL based on the search, specifically the URL structure. We could go down the rabbit hole here, but in doing some thinking, wondering if somehow in there twitter has provided templatized recs on how to return a meta description snippet based on the search query / hashtag used.</p> 

<p>What do you think? What ideas do you have that lead Twitter to increase their traffic to these popular hashtag pages 10x fold? Would love to hear them!</p>