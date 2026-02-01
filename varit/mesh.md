---
date: "2026-01-31T11:20:00+03:00"
title: "Mesh-liukuvärit"
layout: default
nav_order: 2
parent: Värityökalut
---

# Mesh-liukuvärit

{: .figure .figure-right }
![Mesh-liukuvärityökalun kuvake työkalupalkissa](../inkscape-mesh-ikoni.png)

*Mesh-liukuvärillä* tarkoitetaan verkkomaisesti toteutettua liukuvärjäystä,
jossa liukuväri ei etene pysäytyspisteiden kautta vain suoraan tai säteittäisesti vaan
pysäytyspisteitä voi olla kuin verkossa solmuja. Niitä luodaan *mesh-liukuvärityökalulla*.

{: .figure-medium-row }
> ![](../inkscape-mesh-suorakulmio.png)
> ![](../inkscape-mesh-tahti.png)

## Mesh-verkon luonti

Mesh-liukuvärejä luotaessa voidaan käyttää lähtökohtana suoraa ruudukkoa
taikka kartioimaisesti pyöreään muotoon aseteltua verkkoa.
Jälkimmäinen on käytännössä toteutettu verkkona, jonka vastakkaiset päät
on kierretty yhteen.

Mesh-liukuvärin asetusvalikosta valitaan, kumpaa tapaa käytetään ja
sovelletaanko liukuvärjäystä täyttöön vai reunaviivaan. Samalla
voidaan valita haluttujen ruudukon rivien ja sarakkeiden määrä jo valmiiksi.
Rivejä ja sarakkeita voi lisätä myös jälkikäteen.

{: .figure-normal }
> ![](../inkscape-mesh-asetuspalkki-tyyppi.png)

Kun valittua kohdetta kaksoisklikataan mesh-työkalulla, siihen lisätään
asetuspalkissa valitun mukainen ruudukko, joka sovitetaan kohteen oman muodon mukaan.

Mesh-verkossa on verkon solmuina kärjellään olevan neliön muotoisia kahvoja, joita voi
siirrellä verkossa haluamaansa paikkaan. Kustakin verkon solmusta lähtee
pyöreällä kahvalla varustetut venytyskahvat kunkin verkon "säikeen" suuntaisesti.
Näillä venytyskahvoilla verkon muotoa, sen taipumista, voidaan säädellä.

Alla olevissa kuvissa ensimmäisessä suorakulmiossa on verkossa vain yksi rivi
ja yksi sarake. Verkon solmut ovat sen kulmissa ja "säikeet" kulkevat pitkin
suorakulmion reunoja. Toisessa kuvassa on 3×3 ruudukko ja kolmannessa kuvassa
3×3 ruudukko on sovitettu ellipsin muotojen mukaan. Kussakin ruudukossa
joka toinen solmu on kohteen alkuperäisellä värillä ja joka toinen valkoinen.

{: .figure-medium-row }
> ![](../inkscape-mesh-1x1ruudukko.png)
> ![](../inkscape-mesh-3x3ruudukko.png)
> ![](../inkscape-mesh-3x3ruudukko_ellipsissa.png)

Nyt mesh-verkon solmuja voidaan siirrellä, niiden venytyskahvoista
voidaan verkkoon luoda kaarevuutta ja verkon solmujen värejä
ja läpinäkyvyyttä voidaan vaihtaa solmukohtaisesti.

Mesh-liukuvärjäys antaa huomattavan paljon lisää vapautta
liukuvärien luomiseen verrattuna pelkkään suoraan ja säteittäiseen
liukuväriin. Monimutkaisen mesh-verkon rakentaminen on toki työläämpää.

## Mesh-verkon muokkaus

Kun mesh-verkkoa muokataan, pitää muistaa, että samalla kohteella
voi olla mesh-liukuväriä sekä täytössä että reunavärissä.
Jos käytössä on molempia, asetuspalkista voi valita, kumman muokkauskahvat
näytetään.

{: .figure-normal }
> ![](../inkscape-mesh-edit_valinta.png)

Asetuspalkin seuraavilla napeilla valitaan, näytetäänkö kahvat, muutetaan
verkon solmujen välisiä säikeitä suoriksi tai bezier-käyriksi taikka
ellipsin mukaisesti symmetrisiksi.

{: .figure-normal }
> ![](../inkscape-mesh-asetuspalkki_janat.png)

Seuraavista napeista ensimmäisellä voidaan valituille verkon solmuille
valita väriksi kohteen alla oleva väri. Esimerkkikuvassa verkon alla on
vihreä suorakulmio, josta väri on otettu.

Toisella napilla puolestaan verkon solmut sovitetaan sen sisältävään laatikkoon.

{: .figure-normal }
> ![](../inkscape-mesh-color_fit.png)

{: .figure-medium-row }
> ![](../inkscape-mesh-colorpick.png)
> ![](../inkscape-mesh-fit-1.png)
> ![](../inkscape-mesh-fit-2.png)

## Kartiomainen mesh-verkko

Jos mesh-verkko luodaan ruudukon sijaan kartiomaisena, saadaan kuvan mukaine
keskipisteen ympärille "kiedottu" verkko.

{: .figure-medium }
> ![](../inkscape-mesh-kartio.png)

Tämä on käytännössä ruudukkoverkko, jonka yläreunan kaikki pisteet ovat
keskipisteessä ja verkko on kiedottu sen ympärille. Seuraavassa kuvassa
tätä on yritetty selventää avaamalla "kiedottua" verkkoa reunasta.

{: .figure-medium }
> ![](../inkscape-mesh-kartio_avattu.png)

Viimeiseinä mesh-työkalun asetuspalkissa on varoitus siitä, että mesh-toiminnallisuus
ei ole vielä valmis standardoidussa svg-määrittelyssä ja se saattaa muuttaa,
sekä pehmennysvalinta, jolla voidaan valita väriliukuun käytettävä algoritmi.

{: .figure-normal }
> ![](../inkscape-mesh-pehmennys.png)
