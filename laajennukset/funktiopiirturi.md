---
date: "2026-03-15T17:30:00+03:00"
title: "Funktiopiirturi"
layout: default
nav_order: 4
parent: Laajennukset
---

# Funktiopiirturi

"Funktiopiirturi", eli "Function Plotter", on laajennus, jota
voidaan käyttää matemaattisten funktioiden kuvaajien piirtämiseen.
Funktiopiirturi vaatii syötteekseen suorakulmion, jota se käyttää
piirtoalueen pohjana.

{: .figure-normal }
![Funktiopiirturi](../inkscape-laajennukset-funktiopiirturi-1.png)

Laajennuksessa valitaan x- ja y-suuntaiset rajat koordinaatistolle.
Vaakasuuntaisen akselin voi määritellä myös piin monikertoina.
Näytteenottotaajuus, eli "Number of samples" määrää, montako
lukuarvoa piirrettävällä välillä lasketaan. Tämä kannattaa valita
riittävän suureksi ja riippuen piirrettävästä funktiosta.
Esimerkiksi funktiota "x·sin(3x)" piirrettäessä kannattaa valita
käytettäväksi pariton luku, jotta arvo lasketaan myös keskellä,
eli kohdassa x=0.

Alla esimerkki funktion "x·sin(3x)" kuvaajasta, joka on piirretty
liian pienellä näytteiden määrällä, arvolla 10. Piirrettävä funktio pomppii
oikeasti niin nopeasti ylös ja alas, että tämä kuvaaja ei ole
pystynyt esittämään sen todellista kulkua.

{: .figure-normal }
![Funktiopiirturi](../inkscape-laajennukset-funktiopiirturi-2.png)

Seuraavassa kuvassa puolestaan arvo on ollut 30 ja piirturi on
osannut piirtää kuvaajan muuten oikein, mutta koska arvo on ollut
parillinen, funktion arvoa ei ole laskettu kohdassa x=0 ja
siksi kuvaaja ei kulje täysin origon kautta.

{: .figure-normal }
![Funktiopiirturi](../inkscape-laajennukset-funktiopiirturi-3.png)

Kun näytteiden määräksi valitaan 31, saadaan myös origo paikoilleen.

{: .figure-normal }
![Funktiopiirturi](../inkscape-laajennukset-funktiopiirturi-4.png)

Pienellä ulkoasun muokkauksella, eli koordinaatistoruudukon lisäämisellä
ja värien valinnalla saadaan ulkoasuksi esimerkiksi tällainen.

{: .figure-normal }
![Funktiopiirturi](../koordinaatisto-xsin3x.svg)

Samaa koordinaatistopohjaa voidaan luonnollisesti käyttää useampien
funktioiden kanssa, jos käytetään saman kokoista suorakulmiota
ja samoja asetuksia.
