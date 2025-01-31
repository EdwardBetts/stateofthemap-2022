---
layout: page-with-toc
#title: Venue &amp; Transportation
title: Venue
headings: "conference-venue,getting-to,sights"
---

<h2 class='space-bottom1' id='conference-venue'>Venue</h2>

State of the Map 2022 will take place at the University of Florence. It was founded in 1321 and It's one of the oldest in Italy. It cooperates with International research institutions and welcomes students and teachers all over the world, promoting research, study programmes and conferences.

The conference is going to take place in the Morgagni Campus (Careggi District, Address: Viale Giovan Battista Morgagni 40, 50127 Firenze). The Centro Didattico Morgagni is a learning centre opened in 2005 with a multifunctional building for Firenze University. It houses lecture halls, meeting rooms and an auditorium. Around the full height central hall face several rooms, with good internet connection and all the needed facilities.

<div id="map" style="height:420px; width:100%"></div>

<h2 class='space-bottom1' id='getting-to'>Getting To Florence</h2>

<h3>By Train</h3>

Florence is a major stop on the Italian high speed rail network. It's easy to reach via [direct connections](https://direkt.bahn.guru/?origin=8300151) from many cities in Italy, [sleeper trains](https://www.nightjet.com/en/reiseziele/italien/florenz) from Munich or Vienna, and from many [international](https://www.seat61.com/international-trains/trains-from-Florence.htm) stations via transfer connections.


<h3>By Plane</h3>

[Florence Airport (Aeroporto di Firenze-Peretola)](https://en.wikipedia.org/wiki/Florence_Airport) provides air connections to various airports in Europe. The airport is in the outskirts of the city. A [tram](https://www.aeroporto.firenze.it/en/the-passengers/transport/tramway.html) connects it to the city center in about 20 minutes.

[Pisa International Airport (Aeroporto Internazionale di Pisa)](https://en.wikipedia.org/wiki/Pisa_International_Airport) is also nearby and offers additional connections you might like to consider. The city center of Florence is reachable from Pisa International Airport in 70 to 90 minutes by frequently running local trains.

<h2 class='space-bottom1' id='sights'>Florence – Sights and Attractions</h2>

Florence (Italian: Firenze) is a popular tourist destination because of its high density of important historic, cultural, religious and artistic sights. The city is known as the <em>cradle of the Renaissance</em> and hosts world-famous attractions like the <em>Galleria degli Uffizi</em>, the <em>Duomo</em>, <em>Ponte Vecchio (Old Bridge)</em> or the <em>Palazzo Vecchio</em>. The historic centre of Florence is recognized as a World Heritage Site by the UNESCO. For further information about the city and its surroundings, head over to [FOSS4G's conference website](https://2022.foss4g.org/tourism.php) or the [official tourist website of the City of Florence](https://www.feelflorence.it/en).



<script>
  document.addEventListener('DOMContentLoaded', function() {
    var map = L.map('map').setView([43.79, 11.25], 13);
    L.control.scale().addTo(map);
    L.tileLayer('{{ site.map_tiles.url}}', {
      attribution: '{{ site.map_tiles.attribution }}',
      maxZoom: {{ site.map_tiles.maxZoom}}
    }).addTo(map);
    map.scrollWheelZoom.disable();
    L.marker([43.80104, 11.24515], {icon: L.icon({
      iconUrl: "{{ "/img/logo/sotm_2022-logo.svg" | prepend: site.baseurl }}",
      iconSize: [40, 40],
      iconAnchor: [20, 20]
    })}).bindPopup("<h3>Centro Didattico Morgagni</h3><p>Conference Venue. <a href='https://www.openstreetmap.org/?mlat=43.80104&mlon=11.24516#map=18/43.80104/11.24516' target='_blank'>Open location on osm.org</a>.</p>").addTo(map);
  }, false);
</script>
