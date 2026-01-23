---
layout: home
title: Science
permalink: /science/
---

<style>
  /* Remove main card background for science page */
  main {
    background-color: transparent !important;
    box-shadow: none !important;
  }
  
  main::before {
    display: none !important;
  }

  /* Intro section with cream background */
  .science-intro {
    padding: 40px 30px;
    background-color: rgba(255, 255, 255, 0.85);
    border-radius: 20px;
    margin-bottom: 40px;
    position: relative;
  }

  .science-intro::before {
    content: "";
    position: absolute;
    top: -10px;
    left: -10px;
    right: -10px;
    bottom: -10px;
    background: linear-gradient(135deg, 
      rgba(232, 190, 145, 0.2), 
      rgba(215, 175, 135, 0.18),
      rgba(200, 160, 120, 0.15));
    border-radius: 25px;
    z-index: -1;
    filter: blur(25px);
  }

  /* Styling for science posts - each gets its own cream card */
  .science-post {
    margin-bottom: 40px;
    padding: 30px;
    background-color: rgba(255, 255, 255, 0.85);
    border-radius: 20px;
    position: relative;
  }

  .science-post::before {
    content: "";
    position: absolute;
    top: -10px;
    left: -10px;
    right: -10px;
    bottom: -10px;
    background: linear-gradient(135deg, 
      rgba(232, 190, 145, 0.2), 
      rgba(215, 175, 135, 0.18),
      rgba(200, 160, 120, 0.15));
    border-radius: 25px;
    z-index: -1;
    filter: blur(25px);
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

<div class="science-intro">
  <!-- Centered page title -->
  <h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 50px; line-height:1;">
    The 3AM Page
  </h1>
  <p style="text-align: left; font-weight:bold; font-size: 28px; color: #48474cff; margin-bottom: 5px; line-height:1;">
    Why 3AM?
  </p>

  <!-- Why 3AM text -->
  <p style="text-align: left; color: #48474cff; font-size: 20px; margin-bottom: 0; line-height:1.5;">
    Partly because the name sounded like a really good one when it first occurred to me at 4 (and not 3) AM in the morning.
    Partly because 3 AM stands for <i>An Article A Month</i>— more or less.
  </p>
</div>

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

