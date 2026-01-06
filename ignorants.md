---
layout: home
title: IgnoRants
permalink: /ignorants/
---

<style>
  /* Less space between post title and date */
  .ignorants h2 {
    margin-bottom: 4px;
  }

  .ignorants .post-date {
    margin-top: 0;
    margin-bottom: 0;
  }

  /* More space between each post block */
  .ignorants {
    margin-bottom: 35px;
  }
</style>

<!-- Centered page title -->
<h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 0px;line-height:1;">
  IgnoRants
</h1>

<div class="ignorants">
  {% for post in site.IgnoRants %}
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
  {% endfor %}
</div>
