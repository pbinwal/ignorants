---
layout: home
title: Poetry and Prose
permalink: /prose/
---

<style>
  /* Less space between poem title and date */
  .prose-poem h2 {
    margin-bottom: 4px;
  }

  .prose-poem .poem-date {
    margin-top: 0;
    margin-bottom: 0;
  }

  /* More space between each poem block */
  .prose-poem {
    margin-bottom: 35px;
  }
</style>

<!-- Centered page title -->
<h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 0px; line-height:1;">
  Flow
</h1>
<p style="text-align: center; color: #48474cff; margin-bottom: 5px; line-height:1;">
  A Curation of Poetry and Prose
</p>

<!-- List all poems -->
{% assign poems = site.prose | sort: "date" | reverse %}

{% for poem in poems %}
<div class="prose-poem">
  <h2><a href="{{ poem.url | relative_url }}">{{ poem.title }}</a></h2>
  <p class="poem-date">{{ poem.date | date: "%d %B %Y" }}</p>
</div>
{% endfor %}
