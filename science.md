---
layout: home
title: Science
permalink: /science/
---

<style>
  /* Styling for science posts */
  .science-post {
    margin-bottom: 15px;
    padding-bottom: 15px;
    border-bottom: 1px solid #e0e0e0;
  }

  .science-post:last-child {
    border-bottom: none;
  }

  .science-post h1 {
    font-size: 32px;
    font-weight: bold;
    margin-bottom: 15px;
    color: #1F6BB9;
    line-height: 1.3;
  }

  .science-post img {
    max-width: 200px;
    width: 50%;
    height: auto;
    border-radius: 8px;
    margin: 15px 0;
  }

  .science-post-content {
    font-size: 20px;
    line-height: 1.6;
    margin-bottom: 0;
  }

  .science-post-content p {
    margin: 0 0 0 0 !important;
    padding: 0 !important;
    font-size: 20px !important;
  }

  .science-post-content a {
    font-size: 20px;
  }

  .science-post-date {
    text-align: right;
    color: #666;
    font-size: 14px;
    font-style: italic;
    margin-top: 10px;
  }
</style>

<!-- Centered page title -->
<h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 50px; line-height:1;">
  The 3AM Page
</h1>
<p style="text-align: left; font-weight:bold; font-size: 28px; color: #48474cff; margin-bottom: 5px; line-height:1;">
  Why 3AM?
</p>

<!-- Why 3AM text -->
<p style="text-align: left; color: #48474cff; font-size: 20px; margin-bottom: 75px; line-height:1.5;">
  Partly because the name sounded like a really good one when it first occurred to me at 4 (and not 3) AM in the morning.
  Partly because 3 AM stands for <i>An Article A Month</i>— more or less.
</p>

<div style="border-top: 1px solid #e0e0e0; margin-bottom: 15px;"></div>

{% assign sorted_posts = site.science | sort: "date" | reverse %}

{% for post in sorted_posts %}
  <div class="science-post">
    <!-- Post title -->
    <h1>{{ post.title }}</h1>

    <!-- Post image -->
    <div style="text-align: left;">
      <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
    </div>

    <!-- Post excerpt + Read more -->
    <div class="science-post-content">
      {{ post.excerpt }} <a href="{{ post.url | relative_url }}" target="_blank" rel="noopener noreferrer">Read more</a>
    </div>

    <!-- Date at the end -->
    <div class="science-post-date">
      — {{ post.date | date: "%B %-d, %Y" }}
    </div>
  </div>
{% endfor %}

