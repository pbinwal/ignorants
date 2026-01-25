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
    background-color: rgba(255, 255, 255, 0.75);
    background-color: transparent;
    border-radius: 0px;
    border: none;
    margin-bottom: 40px;
    position: relative;
  }

  .science-intro::before {
    display: none !important;
  }



  /* Styling for science posts - each gets its own cream card */
  .science-post {
    margin-bottom: 40px;
    padding: 30px;
    background-color: rgba(255, 255, 255, 0.75);
    background-color: transparent;
    font-family: 'EB Garamond', Georgia, serif;
    font-size: 21px;
    border-radius: 0px;
    border: none;
    position: relative;
    display: flex;
    gap: 30px;
    align-items: flex-start;
  }

  .science-post::after {
    display: none !important;
  }



  .science-post-image {
    flex-shrink: 0;
    width: 200px;
  }

  .science-post-text {
    flex: 1;
  }

  .science-post h1 {
    font-size: 32px;
    font-family: 'Montserrat', 'Cardo', serif;
    font-weight: 700;
    margin-bottom: 15px;
    margin-top: 0;
    color: #48474cff;
    line-height: 1.3;
    letter-spacing: 0.04em;
  }

  .science-post img {
    max-width: 100%;
    width: 100%;
    height: auto;
    border-radius: 8px;
    margin: 0;
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

  /* Responsive: stack on mobile */
  @media (max-width: 768px) {
    .science-post {
      flex-direction: column;
    }
    
    .science-post-image {
      width: 100%;
    }
  }

  .science-post-date {
    text-align: right;
    color: #666;
    font-size: 14px;
    font-style: italic;
    margin-top: 10px;
  }
</style>

<div class="science-intro straight-border">
  <!-- Centered page title -->
  <h1 style="text-align: center; font-family: 'Montserrat', 'Cardo', serif; font-weight: 700; color: #700000; font-size: 56px; margin-bottom: 50px; line-height:1; letter-spacing: 0.04em;">
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
  <div class="science-post straight-border">
    <!-- Post image on left -->
    <div class="science-post-image">
      <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
    </div>

    <!-- Post text on right -->
    <div class="science-post-text">
      <!-- Post title -->
      <h1 style="font-family: 'Montserrat', 'Cardo', serif; font-weight: 700; letter-spacing: 0.04em; font-size: 1.1em;">{{ post.title }}</h1>

      <!-- Post excerpt + Read more -->
      <div class="science-post-content">
        {{ post.excerpt }} <a href="{{ post.url | relative_url }}" target="_blank" rel="noopener noreferrer">Read more</a>
      </div>

      <!-- Date at the end -->
      <div class="science-post-date">
        — {{ post.date | date: "%B %-d, %Y" }}
      </div>
    </div>
  </div>
{% endfor %}

