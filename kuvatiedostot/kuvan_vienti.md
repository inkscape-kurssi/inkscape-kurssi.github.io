---
date: "2026-01-31T11:20:00+03:00"
title: "Kuvan vienti"
layout: default
nav_order: 4
parent: Kuvatiedostot
---

# Kuvan vienti

*Kuvan vieminen* (export) tarkoittaa koko kuvan tai jonkin
sen osan tallentamista erilliseen kuvatiedostoon.

{: .figure-normal }
![Vie-nappi](../inkscape-export-nappi.png)

Vientidialogi tulee esiin painamalla komentopalkin "Open Export" -nappia
tai valitsemalla "Tiedosto"-valikosta "Export"-vaihtoehto.
Toiminnon pikanäppäin on *Shift-Ctrl-E*.

Alla olevissa kuvissa ensimmäisessä on valittuna koko kuvasta
pupu ja toinen kuva on tämän valinan osuus vietynä png-tiedostoksi.

{: .figure-medium-row }
> ![Pupu valittuna kuvasta](../inkscape-export-valittu_pupu.png)
> ![Pupu vietynä kuvasta](../inkscape-export-pupu.png)

Avattu "Vie"-dialogi näyttää tältä:

{: .figure-normal }
!["Vie"-dialogi](../inkscape-export-dialogi.png)

Dialogista on valittuna ylimpänä *"Single File"* -välilehti, jolla
tehdään vienti yhteen tiedostoon. Seuraavalla rivillä tehdään
valinta, halutaanko viedä koko asiakirja, sivu, tehty valinta
vai koordinaattien mukaan valittu oma rajaus.

Kuvan koko määritetään pikseleinä leveys- ja korkeussuunnassa
taikka vaihtoehtoisesti valitsemalla haluttu DPI-arvo.
Vietävän kuvan mittasuhteet pysyvät aina oikeana, eli yhden
kentän muuttaminen vaikuttaa vastaavasti kaikkiin muihin kenttiin.

Rastiruudulla *"Export Selected Only"* tarkoittaa, että jos tässä
on rasti, vientiin ei tule mukaan muuta kuin valitut objektit
vaikka niiden taustalla tai edessä olisi muita objekteja.
Jos taas rastia ei ole, valittujen objektien lisäksi kuvaan
tulee mukaan myös kaikki muu, mikä näkyy valinnan muodostamassa
suorakaiteessa.

*"Backround Color"* -valinnalla voidaan määrätä taustan väri.
Oletuksena tausta on läpinäkyvä.

Lopuksi valitaan luotavan tiedoston nimi ja sijainti sekä tiedostotyyppi.
Suurin osa tiedostotyypeistä on rasterimuotoisia (PNG, JPG, TIFF, WEBP),
mutta mukana on myös vektorimuotoiset Inkscape SVG, puhdas SVG ja PDF.
Osalle tiedostotyypeistä on lisäksi valittavissa asetuksia, kuten
pakkauksen tyyppiä tai fonttien upotus.

{: .figure-normal }
!["Vie"-tiedostomuodot](../inkscape-export-tiedostomuodot.png)

Esimerkissä samaan SVG-tiedostoon on piirretty joukko
[shakkinappuloita](https://freesvg.org/low-poly-chess-pieces)
ja sieltä halutaan viedä ratsu erilliseen PNG-tiedostoon
jotain käyttöä varten.

{: .figure-normal }
![Valkoiset shakkinappulat](../inkscape-export-shakkinappulat_export.png)

Lopputuloksena on kuva pelkästä ratsusta läpinäkyvällä taustalla.

{: .figure-normal }
![Ratsu erikseen vietynä](../inkscape-export-ratsu.png)

Viennin jälkeen muokattava SVG-tiedosto kannattaa tallentaa,
sillä Inkscape-SVG-tiedostoon tallentuvat myös viimeisimmät
viennin yhteydessä käytetyt asetukset. Eli seuraavalla kerralla
muutoksia tehdessä viennin saa helposti tehtyä samaan tiedostoon.

Jos kuvasta halutaan viedä kerralla kaikki shakkinappulat, voidaan
ottaa käyttöön dialogin *"Batch Export"*-välilehti.

{: .figure-normal }
![Valkoiset shakkinappulat](../inkscape-export-batch_export.png)

Tällä välilehdellä vietäviksi voidaan valita *Valinta*, *Tasot* (Layers)
tai *Sivut* (Pages). Kun piirroksesta valitaan kaikki shakkinappulat,
ne viedään jokainen erilliseen tiedostoon sen sijaan, että
vietäisiin niistä yhdessä koostuva yksi kuva, kuten "Single File" -välilehdellä.

Kuvan esimerkissä tiedostoille on annettu prefiksiksi "export" ja suffiksiksi "shakki".
Näiden lisäksi tiedostojen nimissä käytetään esikatselukuvissakin näkyviä objektien
id-nimiä. Esimerkiksi ratsun kuvan tiedostonimeksi tulee siis
`export_g522_shakki.png`.

Lisäksi "Batch Export" -välilehdellä voidaan lisätä useampi samanaikainen
vienti napilla "Add Export". tämä tarkoittaa, että esimerkiksi shakkinappuloista
voidaan yhdellä kertaa tehdä sekä PNG- että SVG-muotoiset tiedostot.
Tämä helpottaa tilannetta, jossa samoista objekteista pitää aina
muutosten jälkeen luoda versiot useissa tiedostomuodoissa tai
erilaisilla kokoasetuksilla.

{: .figure-normal }
![Useampi vienti](../inkscape-export-add_export.png)

Samalla tavalla "Batch Export" -välilehdellä vienti voidaan tehdä
kokonaisille tasoille tai sivuille.