---
layout: home
title: Science
permalink: /science/
---
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

{% assign sorted_posts = site.science | sort: "date" | reverse %}

{% for post in sorted_posts %}
<div style="margin-bottom: 60px;">

  <!-- Custom date -->
  <p style="font-size: 16px; color: #666; margin-bottom: 10px;">
    {{ post.date | date: "%d %B, %Y" }}
  </p>

  <!-- Post title -->
  <h1 style="font-size: 32px; font-weight: bold; margin-bottom: 20px; color: #1F6BB9;">
    {{ post.title }}
  </h1>

  <!-- Post image -->
  <div style="text-align: left; margin: 20px 0;">
    <img src="{{ post.image | relative_url }}" 
        alt="{{ post.title }}" 
        style="max-width: 200px; width: 50%; height: auto; border-radius: 8px;">
  </div>

  <!-- Post excerpt + Read more -->
  {{ post.excerpt }} <a href="{{ post.url | relative_url }}" target="_blank" rel="noopener noreferrer">Read more</a>

</div>
{% endfor %}

