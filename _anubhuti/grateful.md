---
layout: home
title: Grateful
date: 2025-12-30
contributor: Jayesh Bhatt
---

<!-- Full page styling -->
<div style="background-color: transparent; color: #000000; min-height: 100vh; padding: 50px 20px; font-family: 'Noto Sans Devanagari', Georgia, serif;">

  <!-- Centered title -->
  <h1 style="text-align: center; font-weight: bold; color: #2c5f7d; margin-bottom: 20px;">
    {{ page.title }}
  </h1>

  <p style="text-align: center; color: #000000; margin-top: 5px; font-family: 'Noto Sans Devanagari', Georgia, serif; font-size: 1.2em;">
  When nothing of me remains in me, <br>
  Then all I am— is gratefulness alone.
  </p>
  <!-- Custom image -->
  <div style="text-align: center; margin-bottom: 20px;">
    <img src="{{ site.baseurl }}/assets/images/grateful.jpg"
         alt="Artwork"
         loading="lazy"
         style="max-width: 100%; height: auto; border-radius: 10px;">
  </div>



  <!-- Contributor info -->
  <p style="text-align: right; color: #000000; margin-top: 5px; font-family: 'Noto Sans Devanagari', Georgia, serif; font-size: 1.2em;">
    Illustration by: Jayesh Bhatt
  </p>
   <!-- Date at the bottom, right -->
  <p style="text-align: right; color: #000000; margin-top: 40px; font-family: 'Noto Sans Devanagari', Georgia, serif;">
    — {{ page.date | date: "%-d" }} December, {{ page.date | date: "%Y" }}
  </p>
</div>


