---
date: "2026-01-15T13:20:00+03:00"
title: "Reunaviivat ja täyttö"
layout: default
nav_order: 4
parent: Perusteet
---

# Reunaviivat ja täyttö

Vektorikuvissa kuvien alkeiskuviot koostuvat kuvion **reunaviivasta** (stroke) ja sen **täytöstä** (fill) 
eli "sisäpuolesta". Molemmille voi toisistaan riippumatta määritellä erilaisia ominaisuuksia, kuten värin.

## Reunaviiva

Reunaviiva voi olla avoin tai suljettu. Jos se on avoin, se alkaa jostain
pisteestä, ja päättyy johonkin pisteeseen. Jos reunaviiva puolestaan on suljettu,
se alkaa samasta pisteestä, johon se myös päättyy. Kuvio voi myös koostua useammasta
kuin yhdestä avoimesta tai suljetusta käyrästä.

{: .figure-small-row }
> ![](../kayra-ei_tayttoa.svg)
> ![](../kayra-taytto.svg)
> ![](../kayra-ei_tayttoa-yhtenainen.svg)
> ![](../kayra-taytto-yhtenainen.svg)
> ![](../kayra-ei_tayttoa-monta.svg)
> ![](../kayra-taytto-monta.svg)

Ympyrä ja nelikulmio ovat esimerkkejä kuvioista, joiden reunaviivat ovat suljettuja.
Ellipsin tai ympyrän (vajaa) kaari sekä spiraali ovat puolestaan esimerkkejä
avoimista kuvioista.

{: .figure-small-row }
> ![](../ympyra.svg)
> ![](../suorakaide.svg)
> ![](../lohko.svg)
> ![](../kaari-taytetty.svg)
> ![](../spiraali.svg)
> ![](../tahti.svg)

Reunaviivalle voidaan määrätä ominaisuuksia, kuten **väri**, **paksuus**, **viivan tyyppi**
(esimerkiksi yhtenäinen viiva, katkoviiva tai pisteviiva), **kulmien pyöristystapoja**,
**viivan päätteitä** sekä **aloitus-, lopetus- ja välikuvioita** (esimerkiksi nuolenpäitä).

{: .figure-medium-row }
> ![](../viivat.svg)


## Täyttö

Täyttö tarkoittaa kuvion reunaviivan sisäpuolelle jäävää pintaa.
Jos reunaviiva on avoin, menee täytön rajana reunaviivan alkupisteestä
sen loppupisteeseen kulkeva kuvitteellinen suora jana. Tälle sisäosalle voidaan
määrätä haluttu **täyttöväri**, **liukuvärjäys** (lineaarinen, säteittäinen, mesh)
tai muunlainen täyttö, esimerkiksi **kuviointi**.

{: .figure-small-row }
> ![](../taytto-vari.svg)
> ![](../taytto-liuku-lineaarinen.svg)
> ![](../taytto-liuku-sateittainen.svg)
> ![](../taytto-liuku-mesh.png)
> ![](../taytto-kuvio.svg)

Se, mikä puoli on reunaviivan sisäpuoli on selkeää yleensä silloin, jos
reunaviiva ei leikkaa itseään. Palataan myöhemmin siihen, miten sisäpuoli ja
sen täyttö määritellään, kun reunaviiva tekee itseään leikkaavan silmukan.

## Väri

Kuvion täyttö- ja reunavärien nykyiset arvot näkyvät ikkunan vasemmassa
alakulmassa. Jos kuviolla on reunaväri, näkyy sen oikealla puolella myös
reunan paksuus lukuarvona.

{: .figure-large }
![](../varit_ja_paksuus.png)

Valitun kuvion **täyttöväri valitaan** klikkaamalla ikkunan alareunan väripaletista
haluttua väriä. Jos useampi kuvio on yhtä aikaa valittuna, niiden kaikkien
täyttöväri vaihtuu samalla kertaa.

Valittuna olevalle kuviolle **reunaviivan väri valitaan** väripaletista
klikkaamalla haluttua väriä näppäimistön *shift*-näppäin pohjassa. Tämä toimii
muuten aivan samoin kuin täyttövärinkin valinta.

Jos kuviolle ei haluta täyttö- tai reunaväriä, voidaan se poistaa valitsemalla
väriksi paletin vasemmassa reunassa punaisella ruksisymbolilla merkitty
**"Ei mitään"**.

## Viivan paksuus

Reunaviivan paksuudelle löytyy pikavalinta ikkunan vasemmasta alakulmasta.
Klikkaamalla viivan paksuuden lukuarvoa esittävää numeroa hiiren oikealla
napilla esiin ponnahtaa valikko, jossa ovat valittavissa yleisimmin käytetyt
viivanpaksuuden lukuarvot sekä mittayksiköt.

{: .figure-small }
![](../inkscape-viivanpaksuus.png)

## Täyttö ja reunaviiva -dialogi

Laajemman näkymän täytön ja reunan värien sekä muiden ominaisuuksien muokkaamiseen
saa ottamalla esiin **"Täyttö ja reunaviiva"** -dialogin. Tämä tapahtuu joko yläreunan komentopalkista
taikka kaksoisklikkaamalla nykyisen värin ilmaisinta ikkunan vasemmassa alakulmassa.
Pikanäppäin tälle näkymälle on *shift+ctrl+F*.

{: .figure-large }
![](../inkscape-nappi-tayttojaviiva.png)

Täyttö ja reuna -dialogissa on kolme välilehteä, joista ensimmäinen käsittelee
täyttövärin valintaa, toinen reunavärin valintaa ja kolmas reunan tyyliä.

{: .figure-medium-row }
![](../inkscape-taytto.png)
![](../inkscape-viivanvaritys.png)
![](../inkscape-viivantyyli.png)


### Värit

Värivalinnat ovat samanlaisia sekä täytölle että reunalle. Valintoina ovat:
"ei väriä", "tasainen väri", "suora liukuväri", "säteittäinen liukuväri",
"mesh liukuväri", "kuviointi", "swatch" sekä "asettamaton".

Näistä "ei väriä" sekä "tasainen väri" ovat suoraviivaisimmat. Muihin palataan
myöhemmin. Tasaisen värin voi valita erilaisilla värienvalintatyökaluilla, joista
**HSL**-muoto on ehkä selkein. Lyhenne tulee sanoista:

- **Hue**, eli *sävy* (punaisesta kaikkien sateenkaaren värien kautta takaisin punaiseen, 0–360)
- **Saturation**, eli *kylläisyys* (harmaasta täysin kirkkaaseen värisävyyn, 0–100)
- **Luminance**, eli *kirkkaus* (mustasta valitun värin kautta valkoiseen, 0–100)

{: .figure-large }
![](../inkscape-taytto.png)

Tässä muodossa väri valitaan siis valitsemalla kolme arvoa lukuarvoa.
Ensimmäisenä värin **sävy** spektristä, joka käy sateenkaaren tavoin värit punaisesta oranssin, keltaisen,
vihreän, sinisen ja violetin kautta takaisin punaiseen. Arvo vastaa väriympyrän kulmaa alkaen 0:sta
360:een asteeseen.

Toisena värin **kylläisyys**, eli arvo, joka kertoo, onko väri lähempänä harmaata vai "puhdasta" murtamatonta väriä.
Tämän arvo kulkee 0:sta (harmaa) täyteen arvoon 100 (puhdas väri).

Kolmas arvo kertoo värin **kirkkauden**, joka käy äärimmäisenä vasemmalla olevasta
täysin mustasta valitun värin kautta äärimmäisenä oikealla olevaan täysin valkoiseen.
Tämänkin arvot ovat väliltä 0–100.

Neljäntenä värille valittavana arvona on vielä valittavissa **Alpha**, eli värin
*peittävyys*.  Tällä ominaisuudella arvo 0 tarkoittaa täysin läpinäkyvää ja
arvo 100 täysin peittävää väriä.

### Viivan tyyli

Viivan tyyli -välilehdellä on valittavissa useampi viivan ulkoasuun vaikuttava
valinta, joista yksinkertaisin on viivan paksuus. Paksuus on valittavissa
numeroarvon ja mittayksikön avulla.

{: .figure-large }
![](../inkscape-viivantyyli.png)

**"Kuvio"** (*Dashes*) tarkoittaa sitä, onko reunaviiva tasainen vai jonkinlainen katko- tai
pisteviiva. Valittavana on useampi erilainen vaihtoehto. Kuvion yhteydessä valittavissa
oleva lukuarvo **"Siirtymä"** viittaa siihen, mistä kohtaa toistuvaa kuviota sen käyttö alkaa.
**"Pattern"**-tekstikentän avulla voi luoda oman katkoviivakuvion. Kuvan esimerkin "4 1"
tarkoittaa kuviota, jossa neljän yksikön pituista viivaa seuraa yhden yksikön pituinen katko
ja tämä kuvio toistuu koko reunaviivan pituudelta.

**"Markers"**-valinnalla voi valita viivan alku-, keski- sekä loppupisteisiin erityiset
merkkikuviot. Yleisimpiä käyttötarkoituksia ovat esimerkiksi viivan päihin tulevat
nuolenpäät taikka leikkauskohtaa osoittavaan katkoviivaan matkan varrelle tulevat
saksikuviot.

Muita viivan tyylivalintoja ovat kulmien liitostyyli (viisto, pyöreä, terävä), viivan
päiden tyyli (litteä, pyöreä, neliö) sekä järjestys, jossa täyttö, viiva sekä merkinnät
piirretään näkyviin.

### Sumennus ja peittävyys

Samassa dialogissa on alareunassa lisäksi valittavissa arvot kuvion sumennukselle ja
peittävyydelle.

{: .figure-large }
![](../inkscape-sumennus-peitto.png)

Sumennus on oletuksena nolla, eli kuvio on terävä. Jos tätä arvoa kasvattaa,
muuttuu koko kuvio arvon kasvaessa sumeaksi. Alla esimerkkinä sama tähti
sumennuksen arvoilla 0, 16, 35 ja 50.

{: .figure-small-row}
> ![](../taytto-vari.svg)
> ![](../sumennus-tahti16.svg)
> ![](../sumennus-tahti35.svg)
> ![](../sumennus-tahti50.svg)

Peittävyys on puolestaan oletuksena 100 % ja tarkoittaa, että kuviosta ei näy
läpi. Mitä pienemmäksi tämän arvon muuttaa, sitä enemmän kuvion läpi näkyy sen
alla olevia muita kuvioita tai taustaa. Arvo 0 tarkoittaa, että kuvio on täysin
läpinäkyvä, eli näkymätön.

Alla esimerkkinä kuvat, joissa keltaisen tähden peittävyys on saanut arvot
100, 80, 50, 20, 5 ja 0.

{: .figure-small-row}
> ![](../opacity-tahti100.svg)
> ![](../opacity-tahti80.svg)
> ![](../opacity-tahti50.svg)
> ![](../opacity-tahti20.svg)
> ![](../opacity-tahti5.svg)
> ![](../opacity-tahti0.svg)

Kannattaa huomata, että kuviolle voi määrätä kolmea erilaista peittävyyttä:
täyttövärin peittävyys, reunavärin peittävyys ja kuvion kokonaispeittävyys.
