---
date: "2026-01-31T11:20:00+03:00"
title: "Kuvan tallentaminen"
layout: default
nav_order: 3
parent: Kuvatiedostot
---

# Kuvan tallentaminen

Kuvan tallennukseen on useampi vaihtoehto. Jos tiedostolla on jo
nimi ja se halutaan **tallentaa samalla nimellä**, voidaan painaa
komentopalkin tallennusnappia, valita "Tiedosto"-valikosta
"Tallenna" tai painaa pikanäppäintä *Ctrl-S*.

{: .figure-normal }
![Tallennusnappi](../inkscape-tallenna-nappi.png)

Jos tiedostolla ei ole vielä nimeä tai se halutaan **tallentaa
uudella nimellä**, pitää valita "Tallenna"-valikosta "Tallenna nimellä..."
tai painaa pikanäppäintä *Shift-Ctrl-S*.

Kolmantena vaihtoehtona on "Tallena"-valikon "Tallenna kopio..." ja
sen pikanäppäin *Shift-Ctrl-Alt-S*. Tämä tarkoittaa, että
tiedostosta **tallennetaan kopio toisella nimellä**, mutta avoimen
asiakirjan nimenä pysyy edelleen aiempi tiedostonimi.

Yleensä onkin järkevintä tehdä varsinaisen muokkausversion
tallennukset Inkscapen omalla SVG-tiedostomuodolla ja tallentaa
esimerkiksi julkaistavaksi tarkoitetut PDF-versiot erikseen
kopioina. Näin muokattavassa versiossa säilyvät aina kaikki
Inkscapen käytössä hyödylliset ominaisuudet, kuten tasot ja
apuviivat.

{: .figure-medium }
![Tallenna-valikko](../inkscape-tallenna-valikko.png)

Tallennettaessa vaihtoehtoisia tiedostomuotoja löytyy useita.
Ne ovat pääasiassa vektorigrafiikkamuotoja, mutta joukossa
on muutama muunkinlainen vaihtoehto.

{: .figure-medium }
![Tallennustiedostomuodot](../inkscape-tallenna-tiedostomuodot.png)

Oletuksena on "Arvaa tiedostopätteestä", joka päättelee tiedostonimeen
kirjoitetusta päätteestä halutun muodon.

Tärkeimpiä tallennusmuotoja ovat:

## Inkscape-SVG

SVG-tiedostomuoto, jonka dataan on lisättynä joitain
Inkscapen omia metatietoja ja attribuutteja, kuten tiedot
kuvassa käytetyistä tasoista, sivuista, apuviivastoista ja erinäisistä muista
määrittelyistä.

## Standardi SVG

Tämä tiedostomuoto on standardi SVG-tiedosto, eli "plain svg", josta puuttuvat
Inkscapelle ominaiset lisätiedot. Näiden lisätietojen puuttuminen
tarkoittaa, että kun tällainen tiedosto avataan uudelleen
Inkscapeen, se ei sisällä enää esimerkiksi tietoa piirtämisen
apuna käytetyistä tasoista ja apuviivoista.

Tämä tiedostomuoto on tärkeä esimerkiksi tuotantosovellutuksiin 
tarkoitetuissa SVG-tiedostoissa, esimerkiksi verkkosivuilla, kuten Wikipediassa.

Myös piirtäjän oman tietoturvan kannalta voi olla hyvä tallentaa
julkaistavaksi tarkoitetut SVG-tiedostot tässä muodossa, sillä
Inkscape-SVG saattaa toisinaan sisältää myös tietoa esimerkiksi
piirroksesta vietyjen rasterikuvien tiedostopoluista.

## Pakatut SVG-muodot

Sekä Inkscape-SVG:stä että standardista SVG:stä on mahdollista tallentaa
myös Gzip-algoritmilla pakattuja versioita. SVG itsessään on
pelkkä tekstitiedosto, joten pakattuna se vie selvästi vähemmän tilaa.

Kaikki ohjelmat eivät kuitenkaan osaa näyttää pakattuja SVG-tiedostoja.

## Optimoitu SVG

Tämä vaihtoehto pyrkii riisumaan tallennettavasta SVG-tiedostosta kaikkea
mahdollista ylimääräistä ja optimoimaan sen tiedostokoon mahdollisimman
pieneksi. Tallennettaessa käyttäjältä kysytään dialogilla tarkemmat
vaihtoehdot.

{: .figure-medium }
![Optiomoitu SVG -dialogi](../inkscape-tallenna-svg_optimoitu-1.png)

Dialogin ensimmäisellä välilehdellä olevilla valinnoilla voi määrätä,
monenko merkitsevän numeron tarkkuudella koordinaatit tallennetaan,
lyhennetäänkö värikoodit ja käytetäänkö CSS-määrittelyiden sijaan
vastaavia XML-attribuutteja.

Ryhmien litistäminen ("Collapse groups") tarkoittaa, että tallennettavasta
tiedostosta poistetaan kuvan esittämisen kannalta tarpeettomat ryhmittelyt.
Ryhmien luonti samanlaisille attribuuteille puolestaan säästää tilaa
ryhmittelemällä samanlaisia attribuutteja, esimerkiksi saman viivan 
ja täytön värin, sisältävät piirto-objektit samaan ryhmään ja
määrittelemällä attribuutin koko ryhmälle kerralla.

"Keep editor data" -valinta estää tallennusta poistamasta
esimerkiksi tekijänoikeustietoja. "Keep unreferenced definitions"
puolestaan jättää tiedostoon esimerkiksi sellaiset liukuvärien
määrittelyt, joita ei ole kuvassa käytetty. Normaalisti nämä
kaksi vaihtoehtoa on pois päältä, mikä tuottaa pienemmän tiedoston.

"Work around renderer bugs" yrittää varmistaa, että joissain
SVG-kuvia näyttävissä ohjelmissa olevat tunnetut bugit
eivät tule näkyviin.

{: .figure-medium }
![Optiomoitu SVG -dialogi](../inkscape-tallenna-svg_optimoitu-2.png)

Toisella välilehdellä voi merkitä poistettavaksi XML-määrittelyitä,
metadatat sekä kommentit.

Rasterikuvien upottaminen ("Embed raster images") tarkoittaa, että
mahdollisesti linkitetyt viittaukset rasterikuviin muutetaan
tiedoston sisään upotetuksi dataksi, mikä on useimmissa tapauksissa
tärkeä.

"Enable viewboxing" mahdollistaa kuvan katseltavan osuuden
geometrian sisällyttämisen tiedostoon. Tämä on usein hyödyllinen
verkkosivuihin upotettavissa SVG-kuvissa.

"Pretty-printing" -ominaisuudet määrittelevät, käytetäänkö
tallennettavassa tiedostossa rivinvaihtoja ja koodin sisennyksiä.
Tämä voi olla hyödyllistä, jos ihmisen on tarkoitus tarkastella
SVG-koodin tekstiä. Muussa tapauksessa tämän formatoinnin
laittaminen pois päältä säästää vielä jonkin verran tilaa.

{: .figure-medium }
![Optiomoitu SVG -dialogi](../inkscape-tallenna-svg_optimoitu-3.png)

Viimeisellä välilehdellä voi poistaa SVG:n elementeistä tarpeettomat
id-tiedot sekä lyhentää tarvittavia.

## PDF-tiedosto

PDF-tiedostoksi tallentaminen kannattaa yleensä tehdä "Tallenna kopio..."
vaihtoehtona, jolloin muokattavana oleva tiedosto pysyy
Inkscapen omassa SVG-muodossa.

PDF-tiedostoksi tallennettaessa käyttäjältä kysytään myös
joitakin valintoja erillisellä dialogilla.

{: .figure-normal }
![PDF-tallennuksen dialogi](../inkscape-tallenna-pdf.png)

Tallennettavana PDF-tiedoston versiona kannattaa yleensä
pitää "PDF 1.5", ellei ole jotain painavaa syytä muuttaa tätä.

Käyttätarkoituksesta riippuen tekstin tallennuksessa voi käyttää
jotain vaihtoehdoista:

- *"Embed fonts"* - Käytettyjen kirjasintyyppien upottaminen
    mukaan PDF-tiedostoon varmistaa, että tiedoston vastaanottaja
    kykenee katselemaan sitä riippumatta siitä, mitä fonttitiedostoja
    hänellä on koneelleen asennettuna.
- *"Convert text to paths"* – Tämä tarkoittaa, että kaikki tekstit
    muunnetaan poluiksi. Tämä voi olla jossain tilanteessa tarpeen,
    jos halutaan varmistua, että tekstit tulostuvat oikein riippumatta
    siitä, onko tulostajalla käytettävissään teksteihin käytetyt fontit.
    Tämän vaihtoehdon miinuspuolena on, että tämän jälkeen PDF-tiedoston
    kaikki tekstit ovat polkuja eikä niitä voi enää muokata tekstinä
    eikä lukijaohjelmassa voi tehdä tekstihakuja. Tämä on siis yleensä
    järkevää vain suoraan tulostuksiin menevissä versioissa.
- *"Omit text in PDF and create LaTeX file"* – Tämä vaihtoehto on
    tarpeen vain tilanteissa, joissa PDF-muotoinen kuva halutaan lisätä
    LaTeX-dokumenttiin. Tässä vaihtoehdossa tekstit tallennetaan erilliseen
    LaTeX-muotoiseen tiedostoon.

*Rasteroivat suodintehosteet* tarkoittaa, että Inkscapen suotimilla tehdyt
tehosteet muunnetaan PDF:ksi tallennettaessa rasterikuviksi.

*"Resolution for rasterization (dpi)"* tarkoittaa rasteroitavien osuuksien
resoluutioon käytettävää "Dots Per Inch" (pisteitä tuumalla) arvoa.

Lopuksi on mahdollisuus valita, kompensoidaanko kuvassa pyöristyksistä
aiheutuvia mahdollisia virheitä.

## Desktop Cutting Plotter (DXF)

Tiedostot, jotka päättyvät `*.dxf`-päätteeseen, ovat AutoCad-ohjelmiston
tiedostomuotoja, joita käytetään paljon myös erilaisten laserleikkureiden,
vinyylileikkureiden ja plottereiden kanssa.

## PostScript ja Encapsulated PostScript

Näistä kahdesta tiedostomuodosta EPS on lähinnä yksittäisten kuvien ja
PS monisivuisten tulostettavien dokumenttien esittämiseen. Näitä käytetään
usein erityisesti taittoalalla sekä LaTeX-dokumenttien kuvien esittämiseen.
EPS-tiedostossa, kuten SVG-tiedostossa, voi olla sekä vektorigrafiikkaa
että sisään upotettua rasterigrafiikkaa.

Jos kulkaisuun tarvitaan kuva EPS-muodossa, Inkscape on yksi hyvä tapa
muuntaa vektorimuotoinen kuva EPS-tiedostoksi.

## GIMP-paletti

[GIMP-paletti](https://docs.gimp.org/3.0/en/gimp-concepts-palettes.html) ei ole itse kuva vaan tiedosto, joka sisältää kokoelman
RGB-värejä. Tiedostomuoto on alkujaan GIMP-kuvankäsittelyohjelman
tapa tallentaa ja ladata paletteja. Myös Inkscape pystyy käyttämään
tässä tiedostomuodossa tallennettuja paletteja.

Kun Jokin piirros "tallennetaan" GIMP-palettina, käytännössä tallennetaan
siis kokoelma värejä, joita voidaan käyttää myöhemmin Inkscapessa,
GIMPissä tai jossain muussa samaa tiedostomuotoa tukevassa ohjelmassa.

## LaTeX PSTricks-makroilla

Tämä tallennusmuoto tallentaa kuvan tekstitiedostoon sarjana
LaTeX-taitto-ohjelman PSTricks-paketin piirtokomentoja.

Yleensä PSTricks-komentoja käytetään esimerkiksi matematiikan
tieteellisissä julkaisuissa erilaisten kaavioiden ja havainnollistusten
piirtämiseen. Monet piirtävät niitä käsin komentoja kirjoittamalla,
mutta tämä tallennustapa mahdollistaa PSTricks-kuvien piirtämisen
graafisesti Inkscapella.


## OpenDocument Piirros (ODG)

ODG-on tiedostomuoto, joka on määritelty OpenDocument-standardissa
ja joka on LibreOfficen Draw-piirto-ohjelman oma tallennusmuoto.

Tallennus ei ole aina kovin onnistunut ja SVG-kuvientuominen
LibreOfficen Draw -ohjelmaan suoraan onkin yleensä suositeltavampaa.