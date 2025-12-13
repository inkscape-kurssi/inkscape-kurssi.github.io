---
dat: "2025-12-13T10:00:00+03:00"
title: "Vektorikuvat"
parent: Johdanto
nav_order: 1
layout: default
---

# Mikä on vektorikuva?

Ennen ohjelman käytön opettelua on syytä tutustua hiukan käsitteistöön.
Inkscape on ohjelma, jolla piirretään sekä muokataan *vektorikuvia* ja
ohjelman opettelun aloittamisessa onkin tärkeitä ymmärtää, mikä vektorikuvissa
on olennaista ja miten ne eroavat *rasterikuvista*, joita piirretään tai
muokataan monilla muilla ohjelmilla, kuten [Gimpillä][Gimp] tai Photo Shopilla.

Tutustutaan ensin rasterikuvan käsitteeseen, jotta saadaan parempi käsitys siitä, miten
vektorikuvat eroavat esimerkiksi valokuvista.


Rasterikuva
============

{: .figure-small.figure-right }
![](../../images/raster-b.svg)

[Rasterikuvat][Pikseligrafiikka] eli pikselikuvat eli bittikarttakuvat ovat kuvatyyppi,
jota ovat esimerkiksi normaalit digitaalisella kameralla otetut valokuvat tai
skannerilla skannatut kuvat.
Ne koostuvat ruudukon muotoon asetelluista neliön muotoisista
erivärisistä kuvapisteistä eli *rastereista* eli [*pikseleistä*][Pikseli].

{: .highlight }
> - Rasterikuva on ruudukko, jolla on aina **tietty koko**, esimerkiksi 800&times;500 pikseliä.  
  (ruudukon sarakkeiden määrä kertaa rivien määrä)
> - Kuva on tallennettu tietona ruudukon kunkin **ruudun väristä**.
> - Kuvan muokkaaminen tarkoittaa kuvassa olevien kuvapisteiden värin muuttamista.
> - Rasterikuvat soveltuvat erityisesti **valokuviin** sekä muihin paljon "epäsäännöllisyyttä" sisältäviin kuviin.
> - Tallennusmuotoja: bmp, jpg, png, gif, webp, raw


Voidaan ajatella, että rasterikuvilla esitetyt kuviot eivät ole oikeastaan
kyseisiä kuvioita vaan joukko pikseleitä, jotka on asetelty sellaiseen järjestykseen,
että ne yhdessä näyttävät halutulta kuviolta.
Siis esimerkiksi, jos rasterikuvassa on ympyrältä näyttävä kuvio,
paljastaa lähempi tarkastelu, että todellisuudessa kuvassa onkin joukko
sopivan värisiä kuvapisteitä, jotka on aseteltu ympyrän muotoon. Läheltä tarkasteltuna
ja suurennettuna pikseleiden kulmikas muoto tulee esiin ja kuva alkaa "palikoitua" sekä näyttää
"legomaiselta".

Alla muutama erikokoinen hymynaama alkuperäisessä koossaan sekä skaalattuina
saman kokoisiksi. Kun pienet kuvat on skaalattu suuremmiksi, näkyy niiden
koostuminen "palikoista".

| Kuva                                    | Koko            | Tiedostokoko | Samankokoisina (100&times;100) |
|:---------------------------------------:|-----------------|-------------:|:--------------------------------------------:|
|![10&times;10](../../images/smiley-10.png)    | 10&times;10     |        321 t | ![10&times;10](../../images/smiley-10-100.png)    |
|![30&times;30](../../images/smiley-30.png)    | 30&times;30     |       1161 t | ![30&times;30](../../images/smiley-30-100.png)    |
|![60&times;60](../../images/smiley-60.png)    | 60&times;60     |       2609 t | ![60&times;60](../../images/smiley-60-100.png)    |
|![100&times;100](../../images/smiley-100.png) | 100&times;100   |       4752 t | ![100&times;100](../../images/smiley-100.png)     |
|[2000&times;2000](../../images/smiley-2000.png)| 2000&times;2000|     125432 t | ![2000&times;2000](../../images/smiley-100.png)   |

Rasterikuvien palikkamaista koostumusta voidaan häivyttää tekemällä kuvasta
tarkempi, eli kasvattamalla ruudukon kokoa. Esimerkiksi kokoa 4000&times;3000
oleva kuva on selvästi tarkempi kuin 1000&times;750 kokoinen kuva, koska suuremmalla määrällä kuvapisteitä pystytään kuvaan tekemään enemmän yksityiskohtia. Tarkemmassa
kuvassa on enemmän *informaatiota* ja informaation suurempi määrä tarkoittaa
luonnollisesti myös suurempaa tiedostokokoa, koska tallennettavia pikseleitä on
enemmän. Esimerkiksi 4000&times;3000-kokoisessa kuvassa on kertolaskun mukaisesti
12 miljoona pikseliä, eli *12 megapikseliä*. Esimerkiksi digikameroiden ja
puhelimien mainoksissa kerrotuissa megapikselilukemissa on kyse juuri tästä.
Millä tarkkuudella olevia kuvia kamera kykenee ottamaan. Kuvatiedoston kokoon
vaikuttaa luonnollisesti myös käytettävissä olevien värisävyjen määrä.
Valokuvissa on käytettävissä tyypillisesti noin 16 miljoonaa väriä.

{: .figure-large }
> ![](../../images/kissa.jpg)
> Valokuvat sisältävät paljon epäsäännöllisyksiä ja värisävyjä. Rasterikuvamuodot soveltuvat hyvin valokuvien tallentamiseen.

Kuvioiden koostuminen kuvapisteistä tarkoittaa myös sitä, että kuvaa muokattaessa
täytyy itse kuvion sijasta muokata sitä esittäviä pisteitä. Esimerkiksi ympyrää
siirrettäessä pitää siis siirtää sitä esittäviä kuvapisteitä. Tämä ei ole aina helppoa,
jos kuvassa on jotain muutakin sisältöä, jota ei ole tarkoitus muuttaa.


Vektorikuva
============

{: .figure-small.figure-right }
![](../../images/vector-b.svg)

Toisin kuin rasterikuva, [vektorikuva][Vektorikuva] ei koostu kuvapisteistä vaan
se sisältää tiedot erilaisista geometrisista kuvioista sekä niiden (matemaattisista) ominaisuuksista.
Esimerkiksi, jos kuvassa on ympyrä, on siitä tyypillisesti tallennettu tiedot
sen keskipisteen sijainnista, säteen pituudesta, mahdollisen reunaviivan
paksuudesta, reunaviivan väristä sekä ympyrän täyttöväristä. Monikulmiosta puolestaan
on tallennettu tiedot kärkipisteiden sijainneista järjestyksessä, viivan paksuus,
viivan väri sekä täyttöväri.

{: .highlight }
> - Vektorikuva on aina **tarkka** koosta riippumatta.
> - Kuva on tallennettu **tietoina kuvassa olevien kappaleiden ominaisuuksista**, ei kappaleiden kuvina.<br>
  (kappaleen ominaisuuksia: sijainti, suunta, suuruus, pituus, paksuus, väri,...)
> - Vektorikuva **säilyttää muokattavuuden**.
> - Sopii erityisesti säännöllisiin ja selkeisiin **piirtokuviin ja kaavioihin**.
> - Tallennusmuotoja: svg, pdf, ps, eps, wmf


Vektorikuvassa on siis tallennettuna itse kuvion tiedot, ei vain
sen esitys jonkin kokoisena "ruudukkoesityksenä". Koska vektorikuvatkin
lopulta aina näytetään jossain mediassa, siis esimerkiksi näytöllä
tai paperille tulostettuna, ne käytännössä aina muunnetaan katselua varten
rasterikuvaksi. Näytöllä vektorikuva muunnetaan näytön pieniksi valopikseleiksi
ja paperilla tulostuksen tai painon mustepisteiksi. Erona rasterikuviin on siis
se, että vektorikuva voidaan aina näytettäessä, jopa suurempaan kokoon skaalattaessa,
näyttää kyseisen median parhaalla mahdollisella tarkkuudella.

Alla sama hymynaamaa esittävä vektorikuva skaalattuna eri kokoihin.

| Kuva                                    | Koko            | Tiedostokoko | Samankokoisina |
|:---------------------------------------:|-----------------|-------------:|:--------------------------------------------:|
|![10x10](../../images/smiley-vector-10.svg) | 10&times;10     |        492 t | ![10&times;10](../../images/smiley-vector-100.svg)    |
|![30x30](../../images/smiley-vector-30.svg) | 30&times;30     |        492 t | ![10&times;10](../../images/smiley-vector-100.svg)    |
|![60x60](../../images/smiley-vector-60.svg) | 60&times;60     |        492 t | ![10&times;10](../../images/smiley-vector-100.svg)    |
|![100x100](../../images/smiley-vector-100.svg) | 100&times;100|        494 t | ![10&times;10](../../images/smiley-vector-100.svg)    |
|![300x300](../../images/smiley-vector.svg) | 300&times;300    |        494 t | ![10&times;10](../../images/smiley-vector-100.svg)    |
|[2000&times;2000](../../images/smiley-vector-2000.svg) | 2000&times;2000    |        496 t | ![10&times;10](../../images/smiley-vector-100.svg)    |

Taulukon hymynaama koostuu ympyrästä, kahdesta ellipsistä ja yhdestä kaarevasta
viivasta. Alla on kuvan vektorimuotoisen SVG-tiedoston sisältö, josta voidaan
nähdä, miten kuva on tallennettu luettelemalla kuvan osien ominaisuudet.

```xml
<svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="300" height="300" viewBox="0 0 30 30">
    <circle cx="15" cy="15" r="12" fill="#fc0" stroke="black" stroke-width="1"></circle>
    <ellipse cx="11.3" cy="13" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse>
    <ellipse cx="18.7" cy="13" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse>
    <path fill="none" stroke="black" stroke-width="1" d="M10 19.5 c3 3 7 3 10 0"></path>
</svg>
```

Koska vektorikuvien piirtämiseen käytetään geometrisia kuvioita ja muotoja, ne soveltuvat
erityisesti piirroskuviin, joissa on selkeitä ääriviivoja ja jotka koostuvat erilaisista
viivoista ja väripinnoista.

{: .figure-large }
![](../../images/sitikka.svg)

Suurempana näytettävää kuvaa varten ei tallenneta enempää tietoa, koska samat
kuviot vain piirretään suuremmassa koossa, joten vektorikuva
säästää tilaa sitä enemmän, mitä suuremmasta kuvasta on kyse. Hymiöesimerkissä
tiedostokokojen pieni ero johtuu vain siitä, että kuvan näyttökoko on tallennettu kuvaan
itseensä `width`- ja `height`-attribuutteina, joiden pituus vaihtelee kahdesta
merkistä ("10") neljään merkkiin ("2000").

Vektorigrafiikassa objekteja voi ryhmitellä monimutkaisemmiksi kokonaisuuksiksi, muuttaa niiden värejä, skaalata, peilata, kiertää, järjestellä ja pinota eri järjestyksiin.

{: .figure-medium }
![](../../images/cars.svg)

Lisäksi, koska kuvassa olevia kuviota ei tallennettaessa muuteta niiden
pikseliesitykseksi, säilyvät niiden ominaisuudet helposti muokattavina.
Esimerkiksi kuvassa oleva ellipsi on helposti siirrettävissä vain muuttamalla
tietoa sen keskipisteen sijainnin koordinaateista. Samoin hymynaaman väri voidaan vaihtaa
vaikka punaiseksi korvaamalla keltaista sävyä tarkoittavan värikoodin `#fc0`
punaisella sävyllä `#f66`. Viivan paksuus vaihtuu muuttamalla `stroke-width`-attribuutin
arvoa.

{: .figure-medium }
![](../../images/smiley-vector-100-modified.svg)

```xml
<svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="100" height="100" viewBox="0 0 30 30">
    <circle cx="15" cy="15" r="12" fill="#f66" stroke="black" stroke-width="1"></circle>
    <ellipse cx="11.3" cy="10" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse>
    <ellipse cx="20" cy="13" rx="1.7" ry="2.5" fill="white" stroke="black" stroke-width="1"></ellipse>
    <path fill="none" stroke="black" stroke-width="3" d="M10 19.5 c3 3 7 3 10 0"></path>
</svg>
```

Vektorikuvan muokattavuus perustuu juuri siihen, että kuvakokonaisuus koostuu
objekteista (olioista), joita voi muokata siirtämällä, skaalaamalla, kiertäämällä,
väriä vaihtamalla sekä ryhmittelemällä ja järjestämällä/pinoamalla eri järjestykseen
toisiinsa nähden.

Vektorikuva soveltuu erityisen hyvin piirtokuviin, kaavioihin, karttoihin sekä
muihin kuviin, jotka koostuvat selkeistä säännöllisistä (matemaattisista) käyristä
ja kuvioista sekä tasavärisistä tai liukuvärisistä pinnoista. Kuitenkin esimerkiksi
valokuvissa on tyypillisesti niin paljon epäsäännöllisyyksiä ja erilaisia
värisävyjä, että niiden tallentamiseen rasterikuvat sopivat yleensä
huomattavan paljon paremmin.



[Pikseli]: https://fi.wikipedia.org/wiki/Pikseli
[Pikseligrafiikka]: https://fi.wikipedia.org/wiki/Bittikarttagrafiikka
[Vektorikuva]: https://fi.wikipedia.org/wiki/Vektorigrafiikka
[SVG]: https://fi.wikipedia.org/wiki/SVG
[Gimp]: https://gimp.org