---
date: "2026-03-21T21:45:00+03:00"
title: "Matemaattisia havainnekuvia"
layout: default
nav_order: 1
parent: Sovelluksia
---

# Matemaattisia havainnekuvia

Inkscape on käyttökelpoinen työkalu myös matematiikan tehtävien
havainnekuvien piirtämiseen. Kuvia voi piirtää niin
opettaja, opiskelija kuin oppimateriaalin tuottajakin.

Havainnekuvat ovat yleensä pelkistettyjä ja pyritään tekemään
selkeiksi. Inkscapen etuna on myös mahdollisuus piirtää kuvia
tarvittaessa tarkan täsmällisesti.

Piirretään esimerkkeinä muutamia kuvia eri aiheista.

## Geometria

"Vieruskulmien summa on aina 180° eli &alpha; + &beta; = 180°."

Piirretään vaakasuora sininen jana ja sen keskipisteestä alkava
toinen jana. Piirretään punaisella reunaviivalla oleva ympyrä,
jonka keskipiste on janojen leikkauspisteessä. Muutetan
ympyrä kaareksi siirtämällä sen pyöreitä kahvoja.
Monistetaan kaari ja siirretään sen päätepisteet toisen kulman
kohdalle pyöreillä kahvoilla. Suurennetaan kaaren sädettä
siirtämällä neliökahvaa. Monistetaan kaari ja suurennetaan
sen sädettä, jotta saadaan samaan kulmaan toinen samanlainen,
mutta suuremmalla säteellä oleva kaari.

{: .figure-small-row }
> ![](../inkscape-matematiikka-kulman_ympyra.png)
> ![](../inkscape-matematiikka-kulman_kaari.png)
> ![](../inkscape-matematiikka-toinen_kulma-1.png)
> ![](../inkscape-matematiikka-toinen_kulma-2.png)

Näiden vaiheiden suorittamisessa on suureksi hyödyksi,
kun tarttuminen pisteisiin, siis janan keskipisteeseen ja
päähän, on päällä. Ympyrä kannattaa piirtää pitämällä
pohjassa sekä *Shift*- että *Ctrl*-näppäimiä. Näistä
*Shift* tarkoittaa, että piirtäminen aloitetaan ympyrän
keskipisteestä ja *Ctrl* auttaa saamaan aikaan ellipsin
sijaan ympyrän.

Lopuksi käytetään TexText-lisäosaa ja lisätään sillä
kulmien nimet &alpha; ja &beta; Kuvaan on lisätty
myös taustalle valkoinen suorakulmio, jotta
sillä on helppo rajata tiedostoksi vietävän SVG-kuvan
koko. Samalla saadaan vähän tyhjää tilaa janojen
ympärille ja varmistetaan, että tausta on valkoinen
eikä läpinäkyvä.

{: .figure-normal }
![Vieruskulmat](../inkscape-matematiikka-vieruskulmat.svg)

Havainnollistetaan ja nimetään ympyrään liittyviä osia,
janoja ja suoria. Keskipistettä kuvaavan ruksin voi tehdä
piirtämällä janan, monistamalla sen, kääntämällä toisen janan
90 astetta ja yhdistämällä janat ryhmäksi. Keskelle
ympyrää sen saa tasaustyökalulla tasaamalla keskelle
ympyrää vaaka- ja pystysuunnassa.

Janat piirretään viivatyökalulla ja käytetään tarttumisasetusta,
jolloin janojen päät on helpompi saada osumaan kehälle.
Kaarae saa monistamalla ympyrän ja muuttamalla sen kaareksi.

Lopuksi lisätään pisteiden nimet ja selitetekstit
tekstityökalulla. Tekstien värit saa samoiksi kuin
janat käyttämällä värinpoimintatyökalua.

Värien kanssa on hyvä muistaa, että janoissa on käytössä
reunaväri, teksteissä täyttöväri.

{: .figure-medium-row }
> ![Ympyrä ja keskipiste](../inkscape-matematiikka-ympyra_ja_keskipiste.png)
> ![Ympyrä ja janat sekä kaari](../inkscape-matematiikka-ympyra_ja_janat.png)
> ![Ympyrän osat nimettyinä](../inkscape-matematiikka-ympyra_nimetty.png)

Alla on vielä lopputulos SVG-kuvaksi vietynä tiedostona.

{: .figure-medium }
![Ympyrä ja siihen liittyviä osia nimettyinä](../inkscape-matematiikka-ympyra_nimetty.svg)

Jos kuva sisältää tekstiä ja sitä halutaankäyttää
SVG-muodossa, on hyvä muistaa, että
silloin kannattaa koettaa valita kirjasintyypiksi,
jokin sellainen fontti, joka todennäköisimmin löytyy kuvaa
katselevalta. Jos kyseistä fonttia ei löydy, se
yritetään korvata jollain muulla ja ei ole täysiä takeita
siitä, että esimerkiksi kirjasinkoko pysyy samanlaisena.

Toinen vaihtoehto on muuttaa tekstit poluiksi ennen
kuvan viemistä SVG-tiedostoksi. Tämä varmistaa, että
teksti näkyy oikein, mutta vaikeuttaa kuvan muokkaamista
myöhemmin.


## Koordinaatisto

Matematiikassa piirretään usein pisteitä ja kuvaajia koordinaatistoon.
Siksi kannattaakin piirtää kerralla hyvä koordinaatistopohja ja
uudelleenkäyttää sitä yhtenäisen ilmeen saamiseksi.

{: .figure-large }
![Koordinaatisto](../inkscape-matematiikka-koordinaatisto.svg)

Koordinaatiston piirtämisessä kannattaa hyödyntää tarttumisasetusta
sekä Inkscapen ruudukkoa, joiden avulla koordinaatistosta
saa täsmällisen.

{: .figure-large }
![Yhtälön y=x+3 kuvaaja koordinaatistossa](../inkscape-matematiikka-kuvaaja.svg)


## 3D-kappaleet

"Ympyräkartion vaippa muodostuu ympyräsektorin osasta, jonka kaaren pituus on kartion
pohjaympyrän piiri (2&pi;r) ja säde s."

Piirretään havainnollistava kuva. Aloitetaan ympyrän muotoisesta pohjasta.

{: .figure-medium }
![Ympyräkartion pohja](../inkscape-matematiikka-ympyrakartion_pohja.png)

Piirretään seuraavaksi kolmio, jonka kärjet ovat ellipsin puoliakseleiden kolmessa
päätepisteessä. Tarttumistoiminto auttaa kärkipisteiden kohdentamisessa.


{: .figure-medium }
![Kartion piirtäminen aloitettu](../inkscape-matematiikka-ympyrakartion_kartio-1.png)

Siirretään kartion huippu paikalleen ylemmäs. Pidetään *Ctrl*-näppäin pohjassa,
jotta piste ei siirry sivusuunnassa. Vaihtoehtoisesti pisteen voi siirtää
ylös nuolinäppäimellä.

{: .figure-medium }
![Kartion huippu ylös](../inkscape-matematiikka-ympyrakartion_kartio-2.png)

Monistetaan pohja ja otetaan sen ja kolmion unioni, jolloin saadaan alla oleva kuvio.

{: .figure-medium }
![Yhdistetään kartio ja pohja](../inkscape-matematiikka-ympyrakartion_kartio-3.png)

Monistetaan kartion pohja, muutetaan sen reunaksi musta katkoviiva ja poistetaan täyttö.
Muutetaan ellipsi kaareksi, jolloin saadaan pohjan takareuna näkymään katkoviivana.

{: .figure-medium }
![Yhdistetään pohjan takareuna katkoviivana](../inkscape-matematiikka-ympyrakartion_kartio-4.png)

Lisätään kuvaan korkeusjana, pohjan säde ja merkki suoralle kulmalle.

{: .figure-medium }
![Lisätään korkeusjana, säde ja suorankulman merkki](../inkscape-matematiikka-ympyrakartion_kartio-5.png)

Piirretään ympyrä, jonka keskipisteenä on kartion huippu ja säteenä kartion sivujanan pituus.

{: .figure-medium }
![Kartion sivujanan suuruinen ympyrä](../inkscape-matematiikka-ympyrakartion_kartio-6.png)

Muunnetaan ympyrä sektoriksi esittämään kartion vaippaa, joka on kierretty
auki.

{: .figure-medium }
![Kartion sivujanan suuruinen ympyrä](../inkscape-matematiikka-ympyrakartion_kartio-7.png)

Kun vielä lisätään TexTexillä tarvittavat merkinnät ja kaavat, saadaan lopullinen kuva.

{: .figure-large }
![Kartion vaipan ja pohjan yhteispinta-ala](../inkscape-matematiikka-ympyrakartion_kokonaispinta-ala.svg)
