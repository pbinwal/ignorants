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
    background-color: rgba(255, 255, 255, 0.75);
    background-color: transparent;
    border-radius: 0px;
    border: none;
    margin-bottom: 40px;
    position: relative;
  }

  .prose-intro::before {
    content: "";
    position: absolute;
    top: -4px;
    left: -4px;
    right: -4px;
    bottom: -4px;
    border: 6px solid #3a3a3a;
    pointer-events: none;
    filter: url(#watercolor);
  }

  /* Each poem as white card */
  .prose-poem {
    margin-bottom: 60px;
    padding: 25px 30px;
    background-color: rgba(255, 255, 255, 0.75);
    background-color: transparent;
    border-radius: 0px;
    border: none;
    position: relative;
    font-family: 'EB Garamond', Georgia, serif;
    font-size: 21px;
  }

  .prose-poem::before {
    content: "";
    position: absolute;
    top: -4px;
    left: -4px;
    right: -4px;
    bottom: -4px;
    border: 6px solid #3a3a3a;
    pointer-events: none;
    filter: url(#watercolor);
  }

  .prose-poem h2 {
    margin-bottom: 4px;
    color: #48474cff;
  }

  .prose-poem h2 a {
    color: #48474cff;
    text-decoration: none;
  }

  .prose-poem h2 a:hover {
    text-decoration: underline;
  }

  .prose-poem .poem-date {
    margin-top: 0;
    margin-bottom: 0;
  }
</style>

<div class="prose-intro straight-border">
  <!-- Centered page title -->
  <h1 style="text-align: center; font-family: 'Montserrat', 'Cardo', serif; font-weight: 700; color: #700000; font-size: 56px; margin-bottom: 0px; line-height:1; letter-spacing: 0.04em;">
    Flow
  </h1>
  <p style="text-align: center; color: #48474cff; margin-bottom: 0; line-height:1;">
    A Curation of Poetry and Prose
  </p>
</div>

<!-- List all poems -->
{% assign poems = site.prose | sort: "date" | reverse %}

{% for poem in poems %}
<div class="prose-poem straight-border">
  <h2 style="font-family: 'Montserrat', 'Cardo', serif; font-weight: 700; letter-spacing: 0.04em; font-size: 1.1em;"><a href="{{ poem.url | relative_url }}">{{ poem.title }}</a></h2>
  <p class="poem-date">{{ poem.date | date: "%d %B %Y" }}</p>
</div>
{% endfor %}
