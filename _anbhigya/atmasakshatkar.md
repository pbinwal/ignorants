---
layout: home
title: आत्मसाक्षात्कार 
date: 2025-11-21
---

<!-- Full page styling -->
<div style="background-color: #000000ff; color: #ffffffff; min-height: 100vh; padding: 50px 20px; font-family: 'Noto Sans Devanagari', Georgia, serif;">

  <!-- Centered poem title -->
  <h1 class="poem-title" style="text-align: center; font-weight: bold; color: #ffffffff; margin-bottom: 0px;">
    {{ page.title }}
  </h1>

   <!-- Custom image below poem -->
  <div style="text-align: center; margin-top: 2px; margin-bottom: 20px;">
    <img src="{{ site.baseurl }}/assets/images/eyes.png"
        alt="Custom illustration" 
        style="max-width: 100px; width: 100%; height: auto; border-radius: 10px;">
  </div>

  <!-- Centered poem text -->
  <div style="text-align: center; line-height: 2;">
    एक कक्ष है, दो खिड़कियाँ, <br>
    उन पर टंगा एक आवरण, <br>
    पीछे खड़ा झाँके कोई, <br>
    है कौन, आता न स्मरण |<br>
    <br>
    परछाई-सी संसार की, <br>
    पढ़ती है जब मध्य आवरण, <br>
    चलचित्र सी प्रतीत हो, <br>
    करती है मुग्ध ,वह ये मन | <br>
    <br>
    दर्शक नज़ारा देखता, <br>
    विकृत ही क्यों न हो छवि,<br>
    छाया न पूर्ण सत्य है,<br>
    सोचा नहीं उसने कभी |<br>
    <br>
    जब से खुली हैं खिड़कियाँ, <br>
    तबसे टंगा है आवरण, <br>
    तबसे तमाशा चल रहा, <br>
    चलता है जीवन से मरण | <br>
    <br>
    एक दिन हटाकर आवरण, <br>
    पूछा मैंने तू कौन है? <br>
    भाये तुझे चलचित्र क्यों, <br>
    हाँ बोल, अब क्यों मौन है ? <br>
    <br>
    पर क्या यह मायाजाल था,<br>
    उस ओर भी था जो खड़ा,<br>
    मैं ही था, जाना यह मैंने,<br>
    और आत्मसाक्षात्कार हुआ |<br>

  <!-- Date at the bottom, right -->
  <p class="poem-date" style="text-align: right; color: #ffffff; margin-top: 40px; font-family: 'Noto Sans Devanagari', Georgia, serif;">
    — {{ page.date | date: "%-d" }} नवंबर, {{ page.date | date: "%Y" }}
  </p>

</div>
    