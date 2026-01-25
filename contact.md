---
layout: home
title: Contact
permalink: /contact/
---

<style>
  /* Remove main card background */
  main {
    background-color: transparent !important;
  }
</style>
<link rel="stylesheet" href="{{ '/assets/css/handwritten.css' | relative_url }}">

<!-- Page container -->
<div class="straight-border" style="background-color: transparent; color: #000000; padding: 50px 20px; font-family: 'EB Garamond', Georgia, serif; font-size: 21px; max-width: 900px; margin: 40px auto; border-radius: 0px; border: none; position: relative;">
<div style="position: relative; z-index: 1;">

  <!-- Title -->
  <h1 style="text-align: center; font-family: 'Montserrat', 'Cardo', serif; font-weight: 700; color: #700000; font-size: 48px; margin-bottom: 20px; letter-spacing: 0.04em;">
    Contact
  </h1>

  <!-- Photo -->
<div style="text-align: center; margin-bottom: 30px;">
  <img src="{{ '/assets/images/PB_photo.jpg' | relative_url }}"
       alt="Profile Photo"
       loading="lazy"
       style="width: 220px; height: auto; border-radius: 12px;">
</div>


<!-- Email -->
  <p id="greeting" style="text-align: center; font-size: 28px; color: #48474c; margin-bottom: 10px; font-weight: bold; transition: all 0.3s; font-family: 'Chathura', sans-serif;">
    <span id="hello-word" style="color: #cbc104ff; font-family: 'Chathura', sans-serif; font-size: 1.6em;">Hello</span>
    <span style="font-family: 'Chathura', sans-serif; font-size: 1.6em; margin-left: 0.5em;">fellow human!</span>
  </p>
  <script>
    const greetings = [
    'Hello',
    'Namaskaram',
    'Hola',
    'Bonjour',
    'Ciao',
    'Hallo',
    'Olá',
    'Привет',
    '你好',
    'こんにちは',
    '안녕하세요',
    'مرحبا',
    'שלום',
    'Shalom',
    'ਸਤਿ ਸ੍ਰੀ ਅਕਾਲ',
    'สวัสดี',
    'Xin chào',
    'Hei',
    'Hej',
    'Ahoj',
    'Γειά σου',
    'Selam',
    'Merhaba',
    'Sawubona',
    'Salam',
    'Szia',
    'Sveiki',
    'Tere',
    'Halo',
    'Mingalaba',
    'Kamusta',
    'Salve',
    'Dzień dobry',
    'God dag',
    'Dia dhuit',
    'Aloha',
    'Sannu',
    'Habari',
    'Jambo',
    'Bula',
    'Malo e lelei',
    'Talofa',
    'Kia ora',
    'Sain baina uu',
    'Saluton',
    'Zdravo',
    'Pozdrav',
    'Moien',
    'Terve',
    'Labas',
    'Dobrý den',
    'Cześć',
    'Bok',
    'Dobar dan'
  ];

    const helloWord = document.getElementById('hello-word');
    let greetIndex = 0;
    helloWord.textContent = greetings[0];
    setInterval(() => {
      greetIndex = (greetIndex + 1) % greetings.length;
      helloWord.textContent = greetings[greetIndex];
    }, 700);
  </script>
  <!-- Email -->
  <p class="handwritten" style="text-align: center;">
    I am a PhD student at the Institute for Neurobiology, University of Tuebingen, Germany.<br>
    You can reach me at—
  </p>

  <p style="text-align: center; font-size: 1.3em; font-weight: bold; font-family: 'Chathura', sans-serif;">
    <a href="mailto: ignorants.pb@gmail.com" style="color: #000000; text-decoration: none; font-family: 'Chathura', sans-serif; font-size: 1.3em;">
      ignorants.pb@gmail.com
    </a>
  </p>

</div>
</div>
