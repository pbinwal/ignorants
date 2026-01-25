---
layout: home
title: IgnoRants
permalink: /ignorants/
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
  .rant-intro {
    padding: 40px 30px;
    background-color: rgba(255, 255, 255, 0.75);
    background-color: transparent;
    border-radius: 0px;
    border: none;
    margin-bottom: 40px;
    text-align: center;
    position: relative;
  }

  .rant-intro::before {
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

  /* Each rant as white card */
  .rant {
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

  .rant::before {
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

  .rant-content {
    font-size: 18px;
    line-height: 1.6;
    margin-bottom: 0;
    white-space: pre-line;
  }

  .rant-content p {
    margin: 0 0 0 0 !important;
    padding: 0 !important;
  }

  .rant-date {
    text-align: right;
    color: #666;
    font-size: 14px;
    font-style: italic;
    margin-top: 0;
  }
</style>

<div class="rant-intro straight-border">
  <h1 style="font-family: 'Montserrat', 'Cardo', serif; font-weight: 700; color: #700000; font-size: 56px; margin-bottom: 0; line-height:1; letter-spacing: 0.04em;">
    IgnoRants
  </h1>
</div>

<div style="max-width: 700px; margin: 0 auto;">
  {% assign ignorants_posts = site.IgnoRants | sort: "date" | reverse %}
  {% for post in ignorants_posts %}
    <div class="rant straight-border">
      <div class="rant-content">
        {{ post.content }}
      </div>
      <div class="rant-date">
        — {{ post.date | date: "%B %-d, %Y" }}
      </div>
    </div>
  {% endfor %}
</div>
