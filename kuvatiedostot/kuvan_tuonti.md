---
date: "2026-01-31T11:20:00+03:00"
title: "Kuvan tuonti"
layout: default
nav_order: 2
parent: Kuvatiedostot
---

# Kuvan tuonti

Kuvan tuonti tarkoittaa jonkin kuvatiedoston
tuomista uutena objektina jo olemassa olevaan Inkscape-asiakirjaan.

Kuvan tuonnin voi tehdä kolmella tavalla. Tiedostonvalintadialogin
voi avata komentopalkin "Tuo"-napilla, jonka kuvakkeessa nuoli osoittaa
sisään asiakirjaan, taikka "Tiedosto"-valikosta kohdasta "Tuo...".
Tuonnin pikanäppäin on *Ctrl-I*.

{: .figure-medium }
![Rasterikuvan tuonti napilla](../inkscape-import-nappi.png)

{: .figure-medium }
![Rasterikuvan tuonti valikosta](../inkscape-import-valikko.png)

Kolmantena vaihtoehtona on tiedoston raahaaminen tiedostonhallintasovelluksesta
ja pudottaminen Inkscapen piirtoalueelle.

Riippuen tiedostomuodosta käyttäjältä kysytään hieman erilaisia
asioita tuonnin yhteydessä. Katsotaan esimerkkeinä SVG-, PDF- ja
rasterikuvan tuonti.

## SVG-tuonti

{: .figure-normal }
![SVG-kuvan tuonnin dialogi](../inkscape-import-svg.png)

Ensimmäiseksi kysytään, minkälaiseksi sisällöksi SVG-kuva
halutaan tuoda asiakirjaan. Vaihtoehtoina ovat:

- "Lisää SVG kuva editoitavana objektina nykyiseen tiedostoon" – Tämä
    vaihtoehto lisää tuotavan SVG-kuvan sisällön uutena ryhmänä.
- "Add SVG as new page(s) in the current file" – Tämä vaihtoehto
    lisää SVG-tiedoston sisällön uusina sivuina.
- "Embed the svg file in an image tag (not editable in this document)" –
    Tällä SVG-kuva lisätään kokonaisena kuvana, jonka osia ei voi muokata
    tässä asiakirjassa.
- "Link the SVG-file in on image tag (not editable in this document)" – 
    Tämä lisää SVG-kuvan kokonaisena kuvana, kuten edellinenkin vaihtoehto,
    mutta lisäksi kuva on linkitetty viittauksena erilliseen kuvatiedostoon.
    Tällainen linkitys voi rikkoontua helposti, jos tiedostoja siirretään
    levyllä paikasta toiseen tai toiselle tietokoneelle.
- "Open SVG image as separate document" – Tämä vaihtoehto muuttaa tuonnin
    avaamiseksi uuteen asiakirjaan.

Seuraavana vaihtoehtona on tuotavan kuvan esittämiseen käytettävä pistetiheys,
"DPI for rendered SVG".

Kolmantena renderöintimoodi, joka kertoo kuvana upotettavan tai linkitettävän
objektin piirtotavan.

Useimmiten oletusvaihtoehdot ovat halutut.

{: .figure-medium }
![SVG-kuva tuotuna](../inkscape-import-svg_kuva.png)

Tuodusta kuvasta riippuen se saattaa olla kooltaan liian suuri tai pieni
ja se kannattaa skaalata sopivan kokoiseksi. Skaalatessa on hyvä
muistaa pitää *Ctrl*-näppäin pohjassa, jotta kuvasuhde säilyy.

## PDF-kuvan tuonti

PDF-tiedoston tuonnissa käyttäjälle näytetään sama dialogi kuin
PDF-tiedostoa avattaessa.

{: .figure-normal }
![PDF-tiedoston tuonti](../inkscape-import-pdf.png)

Jos dialogissa valitaan "Import Pages", niin PDF-tiedoston sivut lisätään
asiakirjaan uusina sivuina.

{: .figure-medium }
![PDF-tiedoston tuonti sivuina](../inkscape-import-pdf_import_pages.png)

Jos tämä kohta ei ole valittuna, sivujen sisällöt tuodaan yhtenä
ryhmäobjektina, jonka sisällä on kunkin sivun sisältö omana ryhmänään.
Nämä objektit voi skaalata ja sijoitella asiakirjan alkuperäiselle sivulle.

{: .figure-medium }
![PDF-tiedoston tuonti objekteina](../inkscape-import-pdf_as_groups.png)

## Rasterikuvan tuonti

Rasterikuvaa, eli esimerkiksi JPG-, PNG-, WEBP- tai GIF-kuvaa tuotaessa
esitetään käyttäjälle sama dialogi kuin niiden avaamisen yhteydessä.
Tämä on luonnollista, sillä avaaminen on käytännössä vain
kuvan kokoisen uuden asiakirjan luonti ja rasterikuvan tuonti siihen.

{: .figure-normal }
![Rasterikuvan tuonti](../inkscape-avaa-rasterikuvan_import.png)

Ensimmäisenä kysymyksenä on kuvan tuonnin tyyppi *"Image Import Type"*.
Tässä vaihtoehtoina ovat *Upota* ja *Linkitä*. Näiden erona
on se, että upotettaessa kuvan koko data luetaan sisään
Inkscapeen ja kirjaimellisesti upotetaan sisään luotavaan
kuvaobjektiin. Tämä kasvattaa tallennettavan tiedoston tiedostokokoa,
mutta varmistaa, että kuva on aina asiakirjassa mukana.

Linkitys tarkoittaa sitä, että rasterikuva on edelleen omana
tiedostonaan ja siihen vain viitataan tiedoston nimellä.
Tämä vaihtoehto toimii niin kauan, kuin sekä asiakirja
että kuvatiedosto sijaitsevat samassa paikassa, mutta jos
Inkscapella luotu tiedosto siirretään esimerkiksi toiselle
tietokoneelle, linkitys katkeaa. Samoin käy, jos linkitetyn
rasterikuvatiedoston sijaintia siirretään.

Toisena valintana on kuvan tulostustarkkuus, eli "*Image DPI*"
(DPI = Dots Per Inch). Oletusvaihtoehtona on "From file", eli
käytetään samaa pistettä tuumalla -tarkkuutta, joka on
tallennettuna rasterikuvaan.

Kolmantena valintana on "*Kuvan renderöintimoodi*", eli
miten SVG-tiedostoon upotettu kuva piirretään näytölle.
Vaihtoehtoina ovat "None", eli automaattinen piirtotapa,
"Smooth", eli kuvan laatua optimoiva hitaampi tapa, sekä
"Blocky", joka optimoi nopeuden kuvan pehmeyden kustannuksella.

{: .figure-normal }
![Tuotu rasterikuva](../inkscape-import-jpg.png)

Vektorikuvaan kuvaobjektiksi tuotu rasterikuva on edelleen
rasterikuva eikä se ole muokattavissa vektorikuvien
muokkauskeinoilla. Sen tarkkuus on myös edelleen
rasterikuvan kiinteä tarkkuus.

Sille voidaan kuitenkin tehdä muita operaatioita, kuten
[rajaus halutun vektoriobjektin](../../objektit/syvays_ja_maski) mukaan.

{: .figure-normal }
![Tuotu rasterikuva](../inkscape-import-rasteri_clip.png)

Kuvaobjekteille voidaan käyttää myös erilaisia suotimia.

{: .figure-normal }
![Tuotu rasterikuva](../inkscape-import-raster_suodin.png)

