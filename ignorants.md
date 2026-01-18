---
layout: home
title: IgnoRants
permalink: /ignorants/
---

<style>
  /* Styling for rants */
  .rant {
    margin-bottom: 15px;
    padding-bottom: 8px;
    border-bottom: 1px solid #e0e0e0;
  }

  .rant:last-child {
    border-bottom: none;
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

<!-- Centered page title -->
<h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 40px; line-height:1;">
  IgnoRants
</h1>

<div style="max-width: 700px; margin: 0 auto;">
  {% for post in site.IgnoRants reversed %}
    <div class="rant">
      <div class="rant-content">
        {{ post.content }}
      </div>
      <div class="rant-date">
        — {{ post.date | date: "%B %-d, %Y" }}
      </div>
    </div>
  {% endfor %}
</div>
