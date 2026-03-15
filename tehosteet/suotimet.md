---
date: "2026-01-31T11:20:00+03:00"
title: "Suotimet"
layout: default
nav_order: 2
parent: Tehosteet ja suotimet
---

# Suotimet

SVG-kuvien tiedostomuotoon kuuluvat osana [suotimet, eli filtterit](https://developer.mozilla.org/en-US/docs/Web/SVG/Reference/Element/filter).
Suodin on erilaisista atomaarisista suodinprimittiveistä
koottu kokoelma. Suodinprimitiivejä ovat esimerkiksi
"[Gauss-sumennus](https://fi.wikipedia.org/wiki/Gauss-sumennus)" ja
"[konvoluutiomatriisi](https://en.wikipedia.org/wiki/Kernel_(image_processing))".
Suodin luodaan määrittelemällä, mitä primitiivisiä suodintoimintoja
kohteelle suoritetaan, minkälaisilla asetuksilla ja missä järjestyksessä.
Samaa määriteltyä ja nimettyä suodinta voidaan käyttää samassa
kuvassa useaan kohteeseen. SVG-kuvia näyttämään kykenevät ohjelmat,
kuten www-selaimet, osaavat suorittaa kuvalle näitä primitiivisiä
toimintoja ja siten myös niistä koostettuja monimutkaisempia suotimia.

Inkscapessa on "Suotimet"-valikossa suuri joukko valmiiksi määriteltyjä
ja alavalikoiksi luokiteltuja suotimia. Suotimen poistaminen objektilta
tapahtuu samasta valikosta.

{: .figure-normal }
![Suotimet-valikko](../inkscape-suotimet-valikko.png)

## Suodingalleria

Samat suotimet löytyvät myös galleriamuotoisesti "Filter Gallery" -ikkunasta.
Galleriassa suotimet on luokiteltu samoin kuin valikossakin, mutta
ne esitetään havainnollistavien kuvakkeiden kanssa.

{: .figure-normal }
![Filter Gallery](../inkscape-suotimet-filter_gallery.png)

Suotimia voidaan soveltaa vektoriobjekteihin, mutta
myös rasterikuvina upotettuihin objekteihin.

Sovelletaan esimerkkinä joitakin suotimia alla olevaan
kukkakuvioon.

{: .figure-medium }
![Värikukka](../inkscape-suotimet-kukka.png)

Seuraavassa suotimet: "Materiaali > 3D Marble", "Pintamateriaalit > Burnt edges",
"Särmät > Combined Lighting", "Ulkonemia > Tuli"

{: .figure-medium-row }
> ![3D Marble](../inkscape-suotimet-3d_marble.png)
> ![Burnt edges](../inkscape-suotimet-burnt_edges.png)
> ![Combined Lighting](../inkscape-suotimet-combined_lighting.png)
> ![Tuli](../inkscape-suotimet-tuli.png)

Osa suotimista avaa dialogin, jossa sille voi valita joukon parametreja.
Esimerkiksi "Heittovarjo"-suotimelle kysytään käytettävä sumennus
sekä x- ja y-suuntainen siirtymä.

{: .figure-normal }
![Heittovarjo-dialogi](../inkscape-suotimet-heittovarjo_dialogi.png)

Lopputuloksena kohteen taustalle tulee varjo.

{: .figure-medium }
![Heittovarjo](../inkscape-suotimet-heittovarjo.png)

Suotimia voi soveltaa myös asiakirjaan upotetuille
kuvaobjekteille. Käytetään esimerkkinä samaa venekuvaa
kuin aiemminkin.

{: .figure-medium }
![Vene lumisessa maisemassa](../vene-01.jpg)

Suotimet: "Kuvan maalaus ja piirto > Vanha postikortti" ja "Kuvan maalaus ja piirto > Öljymaalaus":

{: .figure-medium-row }
> ![Vene lumisessa maisemassa suotimella "vanha postikortti"](../inkscape-suotimet-vanha_postikortti.png)
> ![Vene lumisessa maisemassa suotimella "öljyvärimaalaus"](../inkscape-suotimet-oljyvarimaalaus.png)

## Suodineditori

Suodineditori on työkalu, jolla voi luoda omia tai muokata
valmiita suotimia. Tällä valitaan, mitä primitiivisiä
suotimia käytetään, missä järjestyksessä ja minkälaisilla
asetuksilla.

{: .figure-normal }
![Suodineditori](../inkscape-suotimet-suodineditori.png)
