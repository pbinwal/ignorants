---
layout: home
title: Finding sun above the clouds 
date: 2026-01-06
---

<!-- Lightbox Modal -->
<div id="imageModal" style="display: none; position: fixed; z-index: 9999; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9); cursor: pointer;" onclick="closeModal()">
  <span style="position: absolute; top: 20px; right: 35px; color: #f1f1f1; font-size: 40px; font-weight: bold;">&times;</span>
  <img id="modalImage" style="margin: auto; display: block; max-width: 90%; max-height: 90%; position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%);">
</div>

<script>
function openModal(imgSrc) {
  document.getElementById('imageModal').style.display = 'block';
  document.getElementById('modalImage').src = imgSrc;
}

function closeModal() {
  document.getElementById('imageModal').style.display = 'none';
}

// Close modal on ESC key
document.addEventListener('keydown', function(event) {
  if (event.key === 'Escape') {
    closeModal();
  }
});
</script>

<!-- Full page styling -->
<div style="background-color: #ffffffff; color: #000000ff; min-height: 100vh; padding: 50px 20px; font-family: 'Noto Sans Devanagari', Georgia, serif;">

  <!-- Centered title -->
  <h1 style="text-align: center; font-weight: bold; color: #000000ff; margin-bottom: 40px; font-size: 36px;">
    {{ page.title }}
  </h1>

  <!-- Centered text -->
  <div style="text-align: left; line-height: 2;">
  Somewhere on the runway of the airport of Valencia, I turned 24 ( I was born in the afternoon, I've been told). As I stared out of the window of the Ryanair aircraft I was now aboard, waiting for it to take off, it struck me that Ryanair narrowly missed being a palindrome by not replacing the <em>i</em> with a <em>y</em>. Or the <em>y</em> with an <em>i</em>— though <em>Ryan</em> wouldn't have been too happy then, I think. I chuckled to myself thinking that this is exactly the kind of dumb awakening that would, I hope, form the spirit of this blog.<br>
  <br>
  <div style="float: right; margin: 0 0 20px 20px; max-width: 45%; text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/ryanair.jpg"
       alt="Ryanair" 
       style="width: 100%; height: auto; border-radius: 10px; cursor: pointer;"
       onclick="openModal('{{ site.baseurl }}/assets/images/ryanair.jpg')">
  <p style="font-size: 1em; color: #666; margin-top: 5px;">Ryanair</p>
</div>
  As the aircraft sprinted ahead on the runaway before taking off, I found myself thinking of Bernoulli and his principle, as I have caught myself doing very often on flights. But these thoughts were quickly interrupted by the feeling of water trickling down on me and the stranger seated next to me from the overhead cabin as the airplane tilted and took off, reaching for the clouds. Perhaps somebody had stowed off a leaky bottle in the cabin above. We shrugged it off and exchanged a smile. The trickling stopped as the aircraft straightened itself.<br>
  <br>
  As we soared above the kingdom of clouds, we were treated to a view of a clear sky. <em>Sunlight, at last</em>, I thought. Four days ago, I had flown to Valencia in the hopes of spending a few leisurely days with lots of sunshine in the Spanish city that boasts of about three-hundred days of sunshine every year. But my days there had not exactly been leisurely, and it was on my flight back home that I was finally greeted with clear blue skies. Just days before my trip, I had signed up for a three week meditation program that required about 80 minutes of commitment each morning, which meant waking up at 5 am to meditate while I was in Spain, so that I could still leave early enough to stick to my planned itinerary. But for this, I had no regrets.<br>
  <br>
  <div style="float: left; margin: 0 20px 20px 0; max-width: 45%; text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/marseille_perhaps.jpg"
       alt="Marseille, perhaps" 
       style="width: 100%; height: auto; border-radius: 10px; cursor: pointer;"
       onclick="openModal('{{ site.baseurl }}/assets/images/marseille_perhaps.jpg')">
  <p style="font-size: 1em; color: #666; margin-top: 5px;">Marseille, perhaps</p>
</div>
  Sometime midway during the flight, the skies cleared further and looking out of the window, one could see a port city. <em>Marseille, perhaps</em>, I thought because we had flown over it on our way to Valencia. The ports of the sprawling city welcomed us from afar. Overlooking the sea from thousands of feet above, one could see little specks of ships on their way to the harbour. Some six hundred years ago, a ship that had looked very different had sailed from Marseille to the Spanish coast, carrying in it certain pieces of iron chains that I had just seen in the Valencian Cathedral the previous afternoon. History says that when King Alfonso V of what was then the kingdom of Aragon had attacked Marseille, he had brought back to Spain remnants of the iron links that had protected the entrance of the old port from enemy naval ships. The chains had been donated to the Valencian Cathedral by the king and even today, their remains are displayed in the <em>Capilla del Santo Cáliz</em> (Chapel of the Holy Chalice) in <em>Catédral de Valencia</em>, bearing testimony to his victory in Marseille as he had intended.<br>
  <div style="clear: both;"></div>
  <br>
  <div style="float: right; margin: 0 0 20px 20px; max-width: 45%; text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/valencia_cathedral.jpg"
       alt="Catédral de Valencia" 
       style="width: 100%; height: auto; border-radius: 10px; cursor: pointer;"
       onclick="openModal('{{ site.baseurl }}/assets/images/valencia_cathedral.jpg')">
  <p style="font-size: 1em; color: #666; margin-top: 5px;">Catédral de Valencia</p>
</div>
  But I reminded myself that the iron chains, though massive, are not the main attraction of the Capilla in question. As the name suggests, the <em>Capilla del Santo Cáliz</em> houses what is believed to be the Holy Chalice that Jesus himself used in the Last Supper. The cup itself, I had learnt, is made of agate, a beautiful translucent silica stone and dates back a little under two thousand years, but it is propped on a gold stand that was a later addition in the 11th Century. Apart from the holy grail and the chains from Marseille in the same chapel, the cathedral also houses the left arm of Saint Vincent the Martyr, the patron saint of Valencia who was martyred by the Romans for refusing to give up his Christian faith.<br>
  <div style="clear: both;"></div>
  <br>
  <div style="text-align: center; margin-bottom: 20px; display: flex; justify-content: center; gap: 15px; flex-wrap: wrap;">
    <div style="width: 45%;">
      <img src="{{ site.baseurl }}/assets/images/holy_chalice.jpg"
           alt="The Holy Chalice in Capilla del Santo Cáliz" 
           style="width: 100%; height: auto; border-radius: 10px; cursor: pointer;"
           onclick="openModal('{{ site.baseurl }}/assets/images/holy_chalice.jpg')">
      <p style="font-size: 1em; color: #666; margin-top: 5px;">The Holy Chalice in Capilla del Santo Cáliz</p>
    </div>
    <div style="width: 45%;">
      <img src="{{ site.baseurl }}/assets/images/hand_of_martyr.jpg"
           alt="Severed arm of Saint Vincent the Martyr" 
           style="width: 100%; height: auto; border-radius: 10px; cursor: pointer;"
           onclick="openModal('{{ site.baseurl }}/assets/images/hand_of_martyr.jpg')">
      <p style="font-size: 1em; color: #666; margin-top: 5px;">Severed arm of Saint Vincent the Martyr</p>
    </div>
  </div>
  Soon, the landscape beneath us changed dramatically as one began to see the lofty snow-covered peaks of the Alps. While the many houses and buildings of Marseille or whatever towns and cities we had flown over had seemed like minuscule specks, barely distinguishable from one another from that altitude, the mountains towered over everything else. Their snow-capped peaks rose well above the low clouds that surrounded them, mocking everything that our species has ever created. As some of us on board delighted in the landscape beneath us, and others snored on, the pilot graciously let us know that somewhere among the many crests and troughs outside our windows, it was possible to see Mont Blanc, the tallest mountain of the Alps. At a height of 4808 m, Mont Blanc is nearly 6 times the height of Burj Khalifa, easily paling the tallest known structure ever built by humans. And what are mountains but tiny wrinkles on the surface of earth? (Turns out if the earth were the size of a tennis ball, Mount Everest would be less than half a mm— so small that one would barely feel it when running over a finger!) And what is earth but just another planet in the Milky Way, and what is our galaxy but just one of the many hundreds of billions (trillions?) of galaxies that might exist in our universe? Maybe Austen was onto something when she wrote— <em>What are men, to rocks and mountains?</em><br>
  <br>
  <div style="float: left; margin: 0 20px 20px 0; max-width: 45%; text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/alps.jpg"
       alt="View of the Alps as seen from my free window seat" 
       style="width: 100%; height: auto; border-radius: 10px; cursor: pointer;"
       onclick="openModal('{{ site.baseurl }}/assets/images/alps.jpg')">
  <p style="font-size: 1em; color: #666; margin-top: 5px;">View of the Alps as seen from my free window seat</p>
</div>
  At some point the pilot announced that we would be flying over Zurich. But the cloud cover was too thick to see anything, and so the world below us lay shrouded in mystery. With few cities or mountains to see outside now, my mind wandered to the rocks I had admired two days ago on the cliffs of Cala Moraig in Costa Blanca, the white coast of Spain. Once a part of the sea bed, the cliffs had gradually emerged from the sea, all the while being sculpted by the skillful hands of the sea waves and winds. Perhaps the most dramatic formation on the Moraig beach is the <em>Cova del Arcs</em>, an arched cave made of rugged limestone typical of the area. While I had arrived early on the beach to try and photograph the sunrise from the cave, the clouds had had other plans. In any case, the beauty of the geology of the area and the gleaming turquoise waters could not be marred by the whims of the weather. There were less than five people on the beach at that time of the day— visiting it during the off-season had been a nice idea after all, even though it had meant fighting off the allure of going for a dip in the crystal clear waters as they would have been too cold to swim. And so, I had chosen to hike the cliff route from Moraig to Cala Llebeig instead. It would be an understatement to call the views spectacular, perhaps a few pictures could do some justice.<br>
  <div style="clear: both;"></div>
  <br>
  <div style="text-align: center; margin-bottom: 20px; display: flex; justify-content: center; gap: 10px; flex-wrap: wrap; align-items: flex-start;">
    <div style="width: 32%;">
      <img src="{{ site.baseurl }}/assets/images/sea_moraig_to_llebeig.jpg"
           alt="Looking down at the sea on the hike from Moraig to Llebeig" 
           style="width: 100%; height: 350px; object-fit: cover; border-radius: 10px; cursor: pointer;"
           onclick="openModal('{{ site.baseurl }}/assets/images/sea_moraig_to_llebeig.jpg')">
      <p style="font-size: 1em; color: #666; margin-top: 5px;">View of the sea on the hike from Moraig to Llebeig</p>
    </div>
    <div style="width: 32%;">
      <img src="{{ site.baseurl }}/assets/images/moraig_cave.jpg"
           alt="Cova del Arcs, Cala Moraig" 
           style="width: 100%; height: 350px; object-fit: cover; border-radius: 10px; cursor: pointer;"
           onclick="openModal('{{ site.baseurl }}/assets/images/moraig_cave.jpg')">
      <p style="font-size: 1em; color: #666; margin-top: 5px;">Cova del Arcs, Cala Moraig</p>
    </div>
    <div style="width: 32%;">
      <img src="{{ site.baseurl }}/assets/images/seagull_llebeig.jpg"
           alt="Seagull, Cala Llebeig" 
           style="width: 100%; height: 350px; object-fit: cover; border-radius: 10px; cursor: pointer;"
           onclick="openModal('{{ site.baseurl }}/assets/images/seagull_llebeig.jpg')">
      <p style="font-size: 1em; color: #666; margin-top: 5px;">Seagull, Cala Llebeig</p>
    </div>
  </div>
  I am no geology buff, but ever since taking Earth Science 101s in the first few semesters of university, I've had a certain sense of reverence towards the discipline. As I had marvelled at the dramatic limestone cliffs on the hike between Cala Moraig and Cala Llebeig, the reverence had been reinforced by the realisation that in these cliffs lay hundreds of thousands, possibly millions of years of earth's history compressed into tens of metres. On this scale, the entirety of a human life is but a speck— too small to see, too fleeting to leave an imprint. Indeed modern humans wouldn't even have existed as a species for the majority of time when these rocks had formed. In every moment of pride and conceit I experience, perhaps this is something I shall remind myself. <em>Perhaps we all should.</em>

   <!-- Date at the bottom, right -->
  <p style="text-align: right; color: #000000ff; margin-top: 40px; font-family: 'Noto Sans Devanagari', Georgia, serif;">
    — {{ page.date | date: "%B %-d, %Y" }}
  </p>
  </div>
</div>


