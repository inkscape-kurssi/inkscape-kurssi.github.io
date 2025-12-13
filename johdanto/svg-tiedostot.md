---
date: "2025-12-13T11:45:00+03:00"
title: "SVG-tiedostot"
parent: Johdanto
nav_order: 2
layout: default
---

# Mikä on SVG-tiedosto?

SVG, eli Scalable Vector Graphics on [W3C]-järjestön ylläpitämä [standardi][W3C-svg]
erityisesti verkossa käytettävälle vektorigrafiikalle.

Inkscape-ohjelma käyttää tätä tiedostomuotoa omana oletustallennusmuotonaan ja
ohjelman toiminnallisuus pyritään toteuttamaan vastaamaan standardin
mahdollistamia ominaisuuksia.

SVG-tiedostomuodossa käytetty kieli kuuluu xml-kielten perheeseen. Siinä erilaiset
kuvaelementit esitetään erityyppisillä tageilla (esimerkiksi: `<path>` ja `<circle>`)
ja niiden ominaisuudet, kuten viivan paksuus ja väri, näiden tagien ominaisuuksina, eli attribuutteina
(esimerkiksi: `<path stroke-width="2" stroke="#a00">`).

Www-sivuilla SVG-kuvia voi käyttää useammallakin tavalla. Niitä voidaan näyttää
muiden kuvatiedostojen tapaan `<img>`-tagilla. Koska SVG sisältyy osana HTML5-standardiin,
SVG-koodi voidaan kirjoittaa myös suoraan HTML5-tiedoston sisään sellaisenaan.
Lisäksi niitä voidaan käyttää muiden kuvien tavoin taustakuvina sivun CSS-tyylien määrityksissä.

Kun SVG-kuvaa käytetään upotettuna koodina suoraan HTML-koodin seassa, sen tagien
ominaisuuksia voi muokata sivuston CSS-säännöillä aivan samaan tapaan kuin minkä
tahansa HTML-elementin ominaisuuksia. Kun kuvan osille annetaan vielä `class`-attribuutilla
sopivia luokkia, on CSS-määrityksillä helppoa esimerkiksi teemoittaa sivustolla
käytetyt kuvakkeet halutun tyylisiksi. CSS-sääntöjä voidaan käyttää myös kuvan
ominaisuuksien animointiin esimerkiksi hiiren osuessa kuvan päälle.

{: .example-title }
> SVG-esimerkki
>
> ```xml
> <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="100" height="100" viewBox="0 0 30 30">
>     <circle cx="15" cy="15" r="12" fill="#fc0" stroke="black" stroke-width="1"></circle>
>     <ellipse cx="11.3" cy="13" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse>
>     <ellipse cx="18.7" cy="13" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse>
>     <path fill="none" stroke="black" stroke-width="1" d="M10 19.5 c3 3 7 3 10 0"></path>
> </svg>
> ```

{: .figure-small }
> <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="100" height="100" viewBox="0 0 30 30"><circle cx="15" cy="15" r="12" fill="#fc0" stroke="black" stroke-width="1"></circle><ellipse cx="11.3" cy="13" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse><ellipse cx="18.7" cy="13" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse><path fill="none" stroke="black" stroke-width="1" d="M10 19.5 c3 3 7 3 10 0"></path></svg>




SVG-kuvien piirtäminen kirjoittamalla suoraan SVG-kieltä on työlästä.
Siksi SVG-kuvat piirretään yleensä jollakin niitä tuottamaan kykenevällä piirto-ohjelmalla, kuten Inkscapella.
Jos SVG-kuvia haluaa piirtää kirjoittamalla suoraan SVG-kieltä, voi sitä
opiskella esimerkiksi [W3schools]-sivustolla tai Mozillan [MDN-sivustolla][MDN-svg].






[W3C]: https://www.w3.org/
[W3C-svg]: https://www.w3.org/Graphics/SVG/
[W3schools]: https://www.w3schools.com/graphics/svg_intro.asp
[MDN-svg]: https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial
