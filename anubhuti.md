---
layout: home
title: Anubhuti
permalink: /anubhuti/
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
  .anubhuti-intro {
    padding: 40px 30px;
    background-color: rgba(255, 255, 255, 0.75);
    border-radius: 0px;
    border: none;
    margin-bottom: 40px;
    position: relative;
  }

  .anubhuti-intro::before {
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

  /* Each art as white card */
  .anubhuti {
    margin-bottom: 40px;
    padding: 25px 30px;
    background-color: rgba(255, 255, 255, 0.75);
    border-radius: 0px;
    border: none;
    position: relative;
  }

  .anubhuti::before {
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

  .anubhuti h2 {
    margin-bottom: 4px;
    color: #48474cff;
  }

  .anubhuti h2 a {
    color: #48474cff;
    text-decoration: none;
  }

  .anubhuti h2 a:hover {
    text-decoration: underline;
  }

  .anubhuti .art-contributor {
    margin-top: 2px;
    margin-bottom: 2px;
    color: #666;
    font-size: 0.9em;
  }

  .anubhuti .art-date {
    margin-top: 0;
    margin-bottom: 0;
  }
</style>

<div class="anubhuti-intro">
  <!-- Centered page title -->
  <h1 style="text-align: center; font-weight: bold; color: #a00000; font-size: 56px; margin-bottom: 0px;line-height:1;">
    Anubhuti
  </h1>
  <p style="text-align: center; color: #48474cff; margin-bottom: 0;line-height:1;">
    A Feeling Beyond Words
  </p>
</div>


<!-- List all art -->
{% assign arts = site.anubhuti | sort: "date" | reverse %}

{% for art in arts %}

<div class="anubhuti">
  <h2><a href="{{ site.baseurl }}{{ art.url }}">{{ art.title }}</a></h2>
  {% if art.contributor %}
  <p class="art-contributor">Contributor: {{ art.contributor }}</p>
  {% endif %}
</div>
{% endfor %}