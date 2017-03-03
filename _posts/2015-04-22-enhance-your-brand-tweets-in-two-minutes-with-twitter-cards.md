---
ID: 5439
post_title: >
  Enhance your brand tweets in two minutes
  with Twitter Cards
author: Kerry Guard
post_date: 2015-04-22 13:11:52
post_excerpt: ""
layout: post
permalink: >
  /enhance-your-brand-tweets-in-two-minutes-with-twitter-cards/
published: true
views:
  - "925"
---
<p>A client recently asked if there was a way to share an image with their Twitter posts through JetPack. I read a few documents to understand my options:</p>

<a href="https://dev.twitter.com/cards/types/summary-large-image" target="_blank" data-behavior="truncate">https://dev.twitter.com/cards/types/summary-large-image</a>

<a href="https://dev.twitter.com/cards/cms-integration#plugin_yoast" target="_blank" data-behavior="truncate">https://dev.twitter.com/cards/cms-integration#plugin_yoast</a>

<p>But at the end of the day I just felt overwhelmed and more confused than ever, so I went back to the original issue...</p>

<p>Share an image on Twitter along with the post. The post was already rendering the title and description, it was just missing an image and in the first piece of documentation there was code that read:</p>

<code>&lt;meta name="twitter:card" content="summary_large_image"&gt;</code>
<code>&lt;meta name="twitter:site" content="@nytimes"&gt;</code>

<p>So all I did was change "@nytimes" to "@mkgmarketinginc" and drop both tags in the &lt;head&gt; of our website and now, if you go to <a href="https://cards-dev.twitter.com/validator">Twitter Card Validator</a> and put in the url to this post you'll see that we are now sharing the image.</p>

<img src="/wp-content/uploads/2015/04/Screen-Shot-2015-04-16-at-1.57.26-PM.png" alt="Twitter Card Meta Description" />

<p>Leave JetPack to create the meta title and description and these added tags will add the image.</p>

<img src="/wp-content/uploads/2015/04/Screen-Shot-2015-04-16-at-1.59.10-PM.png" alt="Twitter Card Validator" />

<p>Easy peasy lemon squeezy.</p>
<p>Leave me a comment if you have any questions.</p>