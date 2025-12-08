---
layout: home
title: Anubhuti
permalink: /anubhuti/
---

<style>
  /* Less space between art title and date */
  .anubhuti h2 {
    margin-bottom: 4px;
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

  /* More space between each art block */
  .anubhuti {
    margin-bottom: 35px;
  }
</style>

<!-- Centered page title -->
<h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 0px;line-height:1;">
  अनुभूति
</h1>
<p style="text-align: center; color: #48474cff; margin-bottom: 5px;line-height:1;">
  Anubhuti: Featured artwork
</p>


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