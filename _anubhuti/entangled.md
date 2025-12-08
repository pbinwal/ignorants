---
layout: home
title: Entangled 
date: 2024-12-06
contributor: Jayesh Bhatt
---

<!-- Full page styling -->
<div style="background-color: #ffffff; color: #000000; min-height: 100vh; padding: 50px 20px; font-family: 'Noto Sans Devanagari', Georgia, serif;">

  <!-- Centered title -->
  <h1 style="text-align: center; font-weight: bold; color: #000000; margin-bottom: 20px;">
    {{ page.title }}
  </h1>

  <!-- Custom image -->
  <div style="text-align: center; margin-bottom: 20px;">
    <img src="{{ site.baseurl }}/assets/images/entangled.jpg"
         alt="Artwork" 
         style="max-width: 100%; height: auto; border-radius: 10px;">
  </div>



  <!-- Contributor info -->
  <p style="text-align: right; color: #000000; margin-top: 5px; font-family: 'Noto Sans Devanagari', Georgia, serif; font-size: 1.2em;">
    Contributor: Jayesh Bhatt
  </p>
  <!-- Date at the bottom, right -->
  <p style="text-align: right; color: #000000; margin-top: 40px; font-family: 'Noto Sans Devanagari', Georgia, serif;">
    — {{ page.date | date: "%-d" }} December, {{ page.date | date: "%Y" }}
  </p>
</div>


