---
date: "2026-01-31T11:20:00+03:00"
title: "Kuvan avaaminen"
layout: default
nav_order: 1
parent: Kuvatiedostot
---

# Kuvan avaaminen

Kun komentopalkista painetaan "Avaa"-nappia tai "Tiedosto"-valikosta
valitaan vaihtoehto "Avaa...", voi valita normaalilla tiedostonvalintadialogilla
avattavan tiedoston. Pikanäppäin tälle on *Ctrl-O*.

{: .figure-normal }
![Komentopalkin "Avaa"-nappi](../inkscape-avaa-nappi.png)

Inkscape osaa avata oman SVG-tiedostotyyppinsä lisäksi
useita muita tiedostomuotoja, joista osa on
vektorikuvien muotoja ja osa rasterikuvien muotoja.

{: .figure-medium-row }
> ![Inkscapen ymmärtämiä tiedostomuotoja](../inkscape-avaa-tiedostotyypit-1.png)
> ![Inkscapen ymmärtämiä tiedostomuotoja](../inkscape-avaa-tiedostotyypit-2.png)

Inkscapen oma tiedostomuoto on SVG, eli "Scalable Vector Graphics"
ja nämä tiedostot se avaa täydellisesti. Muita vektorigrafiikkamuotoja
ovat esimerkiksi Adobe Illustratorin `*.ai`, AutoCAD:in `*.dxf`,
Corel DRAW:n `*.cdr`, Adoben "Portable Document Format", eli `*.pdf`,
taittoalalla käytetyt "Postscript" `*.ps` ja "Encapsulated PostScript" `*.eps`,
"Windows Metafiles" `*.wmf` sekä joukko muita tiedostotyyppejä.
Nämä Inkscape osaa avata parhaansa mukaan. Toisinaan paremmin, toisinaan
joillain puutteilla.

Lisäksi tuettujen tiedostomuotojen joukossa on rasterikuvien tallennusmuotoja,
kuten `*.jpg`, `*.png`, `*.gif`. Näitä avattaessa luodaan uusi
avattavan kuvan kokoinen asiakirja, johon rasterikuva
tuodaan objektina.

## PDF-tiedosto

Avataan esimerkkinä sample-files.com-sivustolta löytyviä
[PDF-tiedostojen esimerkkejä](https://sample-files.com/documents/pdf/).

Kun avaamme tiedoston `basic-text.pdf`, Inkscape esittää kuvassa olevan
dialogin, jolla se kysyy käyttäjältä tarkempia tietoja, miten tiedosto
halutaan avata.

{: .figure-normal }
![PDF-tiedoston tuonti](../inkscape-avaa-pdf_import.png)

Aivan ensimmäisenä kannattaa huomata dialogin kaksi välilehteä:
*"Internal import"* ja *"Cairo import"*. Näissä on kyse siitä, että
Inkscapella on kaksi keskenään vaihtoehtoista tapaa lukea
PDF-tiedoston sisältö Inkscapen tietorakenteiksi. Ensimmäinen
vaihtoehto on käyttää Inkscapen omaa sisäänrakennettua
menetelmää, eli "Internal import". Toinen vaihtoehto on käyttää
erillistä Cairo-nimistä kirjastoa PDF-tiedoston tulkitsemiseen.
Molemmilla on omat etunsa ja joskus kannattaa vain kokeilla,
kummalla jälki on parempaa.

### Internal import

Inkscapen oma sisäinen menetelmä on suositeltava, sillä se on
monipuolisempi ja avaa PDF-tiedostot paremmin muokattavaan muotoon.
Sisäisessä tuontitavassa käyttäjä voi valita, miten sisältöä tuodaan.
Ensimmäisenä on valinta, **mitkä sivut** halutaan tuoda. Tuodaanko
kaikki sivut vai ainoastaan valitut sivut.

Esikatselunäkymällä voi selata tiedoston sivuja.

Toisena valitaan **syväystapa**, joka kertoo, miten tuotuja sivuja
rajataan. Tarkempaa tietoa vaihtoehdoista löytyy
[Scribus-ohjelmiston wikistä](https://wiki.scribus.net/canvas/PDF_Boxes_:_mediabox,_cropbox,_bleedbox,_trimbox,_artbox).

Kolmantena valitaan, miten tekstejä kirjasintyyppejä käsitellään. Vaihtoehtoina
ovat:

- "Draw missing fonts": Muunnetaan kuviksi kaikki sellaiset tekstit, jotka on kirjoitettu
    käyttöjärjestelmästä puuttuvilla fonteilla.
- "Substitute missing fonts": Korvataan puuttuvilla fonteilla kirjoitetut
    tekstit jollain mahdollisimman sopivalla fontilla.
- "Keep missing fonts' names": Pidetään fonttien nimet entisellään, jolloin
    jollain toisella tietokoneella avattaessa tekstit näkyvät oikein, jos
    tietokoneessa on oikea fontti asennettuna.
- "Delete missing font text": Poistetaan tekstit, jotka on kirjoitettu
    fontilla, joka ei ole käytettävissä.
- "Draw all text": Muutetaan kaikki teksti piirtokuvioiksi.
- "Delete all text": Poistetaan kaikki teksti.

Kohdasta *"List of all PDF fonts"* voi katsoa luettelon kaikista PDF-tiedostossa
käytetyistä fonteista ja niiden mahdollisista korvauksista tai muuttamisista
poluiksi.

*"Precision of approximating gradient meshes"* -valinnalla voi säätää, millä
tarkkuudella mesh-liukuvärit luodaan.

Valinta *"Upota kuvat"* tarkoittaa, että PDF-tiedostossa olevat kuvat
upotetaan suoraan uuteen dokumenttiin sisään upotettuina kuvaobjekteina.
Jos tästä ruudusta poistetaan rasti, kuvatiedostot tallentuvat levylle erillisiksi
tiedostoiksi ja dokumentin kuvaobjekteihin ei tule itse kuvien dataa
vaan viittaus kyseisiin kuvatiedostoihin. Yleensä rasti kannattaa jättää päälle.

*"Import pages"* valinnalla voidaan valita, tuodaanko valitut sivut
Inkscapeen erillisinä sivuina vai tuodaanko ne yhdelle Inkscapen
dokumenttisivulle vierekkäisinä objekteina.

{: .figure-medium }
![PDF-tiedosto avattuna](../inkscape-avaa-pdf_basic_avattuna.png)

Tekstit ovat editoitavia tekstiobjekteja.

{: .figure-normal }
![PDF-tiedosto avattuna](../inkscape-avaa-pdf_basic_avattuna-teksti.png)

Alla olevista kuvista ensimmäisessä monisivuisesta PDF-tiedostosta
on tuotu kaksi sivua asetuksella "Import pages" ja sivut ovat
kahtena erillisenä sivuna.

{: .figure-normal }
![PDF-tiedosto avattuna](../inkscape-avaa-pdf_multipage-1.png)

Toisessa kuvassa ei ole käytetty "Import pages" -asetusta ja
molemmat sivut on tuotu Inkscapeen samalle sivulle vierekkäisinä
objektiryhminä.

{: .figure-normal }
![PDF-tiedosto avattuna](../inkscape-avaa-pdf_multipage-2.png)

### Cairo import

Joissain tilanteissa Inkscapen sisäinen PDF-tuonti ei onnistu
kunnolla ja silloin kannattaa yrittää turvautua Cairo-kirjastolla
tapahtuvaan tuontiin. Tämä on tapa on kuitenkin rajoittuneempi,
sillä se tuo PDF-tiedostosta vain sen ensimmäisen sivun ja
tekstitkään eivät ole välttämättä muokattavaa muotoa vaa
irrallisia kirjaisymboleja. Joidenkin tiedostojen kanssa
tämä on kuitenkin tarpeellinen vaihtoehto.

## Rasterikuvan avaaminen

Kun rasterikuva avataan, sitä varten luodaan uusi asiakirja,
jonka koko on rasterikuvan koko. asiakirjaan lisätään
ainoana objektina kyseinen kuvaobjekti. Ennen kuvan
avaamista käyttäjältä kysytään, miten hän haluaa tuoda
kuvan asiakirjaan.

{: .figure-normal }
![Rasterikuvan tuonti](../inkscape-avaa-rasterikuvan_import.png)

Tämä vaihe on sama kuin [rasterikuvan tuonnissa](../kuvan_tuonti) jo
olemassa olevaan asiakirjaan.