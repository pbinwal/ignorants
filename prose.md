---
layout: home
title: Poetry and Prose
permalink: /prose/
---

<style>
  /* Remove main card background */
  main {
    background-color: transparent !important;
    box-shadow: none !important;
  }
  
  main::before {
    display: none !important;
  }

  /* Intro section */
  .prose-intro {
    padding: 40px 30px;
    background-color: rgba(255, 255, 255, 0.85);
    border-radius: 20px;
    margin-bottom: 40px;
  }

  /* Each poem as white card */
  .prose-poem {
    margin-bottom: 40px;
    padding: 25px 30px;
    background-color: rgba(255, 255, 255, 0.85);
    border-radius: 20px;
  }

  .prose-poem h2 {
    margin-bottom: 4px;
  }

  .prose-poem .poem-date {
    margin-top: 0;
    margin-bottom: 0;
  }
</style>

<div class="prose-intro">
  <!-- Centered page title -->
  <h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 0px; line-height:1;">
    Flow
  </h1>
  <p style="text-align: center; color: #48474cff; margin-bottom: 0; line-height:1;">
    A Curation of Poetry and Prose
  </p>
</div>

<!-- List all poems -->
{% assign poems = site.prose | sort: "date" | reverse %}

{% for poem in poems %}
<div class="prose-poem">
  <h2><a href="{{ poem.url | relative_url }}">{{ poem.title }}</a></h2>
  <p class="poem-date">{{ poem.date | date: "%d %B %Y" }}</p>
</div>
{% endfor %}
