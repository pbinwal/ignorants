---
layout: home
title: Blossom
date: 2026-01-18
contributor: Jayesh Bhatt
---

<!-- Full page styling -->
<div style="background-color: transparent; color: #000000; min-height: 100vh; padding: 50px 20px; font-family: 'Noto Sans Devanagari', Georgia, serif;">

  <!-- Centered title -->
  <h1 style="text-align: center; font-weight: bold; color: #a00000; margin-bottom: 20px;">
    {{ page.title }}
  </h1>

  <p style="text-align: center; color: #000000; margin-top: 5px; font-family: 'Noto Sans Devanagari', Georgia, serif; font-size: 1.2em;">
  The blossoming of a flower, <br>
  Though impalpable at first,<br>
  Is unmissable when does,<br>
  The fragrance delight.<br>
  <br>
  And so bit by bit,<br>
  Does the seeker blossom,<br>
  Intangible at first,<br>
  But unmistakable in the end.<br>
  </p>
  <!-- Custom image -->
  <div style="text-align: center; margin-bottom: 20px;">
    <img src="{{ site.baseurl }}/assets/images/blossom.jpg"
         alt="Artwork" 
         style="max-width: 100%; height: auto; border-radius: 10px;">
  </div>



  <!-- Contributor info -->
  <p style="text-align: right; color: #000000; margin-top: 5px; font-family: 'Noto Sans Devanagari', Georgia, serif; font-size: 1.2em;">
    Illustration by: Jayesh Bhatt
  </p>
   <!-- Date at the bottom, right -->
  <p style="text-align: right; color: #000000; margin-top: 40px; font-family: 'Noto Sans Devanagari', Georgia, serif;">
    — {{ page.date | date: "%-d" }} January, {{ page.date | date: "%Y" }}
  </p>
</div>


