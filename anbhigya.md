---
layout: home
title: Anbhigya
permalink: /anbhigya/
---

<style>
  /* Less space between poem title and date */
  .anbhigya-poem h2 {
    margin-bottom: 4px;
  }

  .anbhigya-poem .poem-date {
    margin-top: 0;
    margin-bottom: 0;
  }

  /* More space between each poem block */
  .anbhigya-poem {
    margin-bottom: 35px;
  }
</style>

<!-- Centered page title -->
<h1 style="text-align: center; font-weight: bold; color: #000; font-size: 56px; margin-bottom: 0px;line-height:1;">
  अनभिज्ञ
</h1>
<p style="text-align: center; font-size: 20px; color: #48474cff; margin-bottom: 5px;line-height:1;">
  कविता संग्रह
</p>

<!-- List all poems -->
{% assign poems = site.anbhigya | sort: "date" | reverse %}

{% for poem in poems %}
<div class="anbhigya-poem">
  <h2><a href="{{ poem.url | relative_url }}">{{ poem.title }}</a></h2>
  <p class="poem-date">{{ poem.date | date: "%d %B %Y" }}</p>
</div>
{% endfor %}
