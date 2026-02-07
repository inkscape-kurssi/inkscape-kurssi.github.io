---
date: "2026-01-31T11:20:00+03:00"
title: "Tasaaminen"
layout: default
nav_order: 2
parent: Objektit
---

# Tasaaminen

{: .figure .figure-right }
![Tasaa ja jaa -dialogin nappi](../inkscape-tasaus-ikoni.png)

Kuvia piirtäessä tulee usein eteen tilanteita, joissa kohteita
pitää tasata toisiinsa tai koko kuvan suhteen jonkin reunan
tai keskityksen mukaan. Tähän tarkoitukseen Inkscapessa
on *Align and Distribute*, eli *Tasaa ja jaa* -dialogi.
Dialogin voi avata komentopalkissa olevasta napista tai
*Shift-Ctrl-a* -pikanäppäimellä.

{: .figure-normal }
![Tasaa ja jaa -dialogi](../inkscape-tasaus-align.png)


## Kohteiden tasaus

Kohteiden *tasaus* (*align*) tarkoittaa sitä, että valitut objektit asetetaan
keskenään esimerkiksi vasemmasta reunastaan tasan.
Ensimmäinen tärkeä asia tasauksessa on sen valinta, **minkä suhteen
valittuja objekteja tasataan**. Dialogin pudotusvalikosta *Relative to*
voi valita tasauksen vertailukohdaksi *ensimmäiseksi* tai *viimeiksi
valitun kohteen*, *suurimman* tai *pienimmän kohteen*, *koko sivun*,
*koko piirustuksen*, eli kaikki piirtoalueella olevat objektit yhteensä,
taikka *valittujen kohteiden muodostaman alueen*.

{: .figure-normal }
![Minkä suhteen tasataan](../inkscape-tasaus-suhteessa_mihin.png)

Kun tasauksen vertailukohta ja tasattavat objektit on valittu,
voidaan itse tasaus tehdä painamalla halutun tasaustyypin
nappia dialogista.

{: .figure-normal }
![Tasausnapit](../inkscape-tasaus-tasaukset.png)

Tasausten tyypit on jaettu ylärivin vaakasuunnassa ja alarivin pystysuunnassa
tapahtuviin tasauksiin.

Ylärivissä tasaukset ovat:
- Tasaa kohteiden oikea reuna vertailukohdan vasemman reunan kanssa.
- Tasaa kohteiden vasen reuna vertailukohdan vasemman reunan kanssa.
- Tasaa kohteiden keskikohdat vertailukohdan keskikohdan kanssa.
- Tasaa kohteiden oikea reuna vertailukohdan oikean reunan kanssa.
- Tasaa kohteiden vasen reuna vertailukohdan oikean reunan kanssa.
- Tasaa tekstit vasemmasta reunasta.

Alarivissä ovat vastaavat toiminnot, mutta pystysuunnan suhteen.
Vaakasuuntaiset tasaukset eivät muuta kohteiden sijaintia pystysuunnassa
ja pystysuuntaiset eivät koske kohteiden vaakasuuntaiseen sijaintiin.

Nappien kuvakkeet ovat erittäin havainnolliset.

Tasataan esimerkkeinä kuvan kohteita. Valitaan vihreä viisikulmio viimeisenä
ja tasataan muut sen suhteen.

{: .figure-normal }
![Tasattavat kohteet](../inkscape-tasaus-kohteet.png)

Tasataan kohteen ensin vasemman reunan, keskikohdan ja oikean reunan suhteen.

{: .figure-medium-row-vert }
> ![](../inkscape-tasaus-vasen.png)
> ![](../inkscape-tasaus-keski.png)
> ![](../inkscape-tasaus-oikea.png)

Sen jälkeen tasataan kohteet oikeasta reunasta viisikulmion
vasemman reunan tasalle. Ja vasemmasta reunasta viisikulmion oikean reunan
tasalle.

{: .figure-medium-row-vert }
> ![](../inkscape-tasaus-oikea-vasemmalle.png)
> ![](../inkscape-tasaus-vasen-oikealle.png)

Jos tekstikohteet tasataan tekstintasaustoiminnolla, niin tekstiobjektien
ankkuripisteet tasataan sivusuunnassa kohdakkain. Seuraavissa kuvissa
ensimmäisessä tekstit ovat kokonaan tasaamatta.

{: .figure-large }
> ![](../inkscape-tasaus-teksti_tasaamatta.png)

Toisessa kuvassa kaikkien
tekstien tasauksena on vasen tasaus, eli niiden ankkuripiste on tekstin
vasemmassa alakulmassa, ja ne on tasattu tekstitasauksella samaan linjaan.

{: .figure-medium }
> ![](../inkscape-tasaus-teksti_vasen_tasaus.png)

Kolmannessa kuvassa ensimmäinen teksti on
keskitetty, toinen tasattu oikealle ja kolmas vasemmalle. Niiden
ankkuripisteet, eli kussakin tekstissä oleva pieni neliö, ovat pystysuunnassa
samassa linjassa.

{: .figure-large }
> ![](../inkscape-tasaus-teksti_ankkurit.png)

Tasauksen pystysuunnassa toimivat samalla tavalla.
Kohteiden alareuna vertailukohteen yläreunan tasalle ja
yläreuna vertailukohteen alareunan tasalle.

{: .figure-small-row-vert }
> ![](../inkscape-tasaus-kohteet-vert.png)
> ![](../inkscape-tasaus-ala-ylos.png)
> ![](../inkscape-tasaus-yla-alas.png)

Sekä kaikkien kohtedien yläreuna, keskikohta tai alareuna
vertailukohteen vastaavan kohdan kanssa tasaan.

{: .figure-small-row-vert }
> ![](../inkscape-tasaus-yla.png)
> ![](../inkscape-tasaus-keski-vert.png)
> ![](../inkscape-tasaus-ala.png)

Tekstin pystysuunaisessa tasauksessa oleellista on, että
tekstit tasataan tekstin perusviivan mukaan, ei yksittäisten
kirjasinmerkkien mukaan. Tässä esimerkissä kirjainten
"p" ja "y" alaosat menevät tekstin perusviivan alle,
mutta koska tasaus on tehty tekstitasauksena, sitä
ei ole tehty tekstiobjektien alareunan vaan perusviivan
mukaan. Eli toisin sanoen tekstit ovat linjassa
eivätkä pompi.

{: .figure-normal }
> ![](../inkscape-tasaus-teksti_pysty.png)

## Tasajako

Kohteiden *jakamisella* (*distribute*) tarkoitetaan sitä, että
ne asetellaan halutussa suunnassa tasavälein.

{: .figure-large }
> ![Tasajaon toimintanapit](../inkscape-tasaus-jaa.png)

Myös jakamisen toiminnot on dialogissa aseteltu kahteen riviin.
Ylemmässä rivissä vaakasuuntainen ja alemmassa pystysuuntainen jakaminen.

Vaakasuunnassa toiminnot ovat:
- Kohteiden vasemmat reunat tasavälein
- Kohteiden keskipisteet vaakasuunnassa tasavälein
- Kohteiden oikeat reunat tasavälein
- Kohteiden välissä yhtä paljon tilaa
- Tekstien ankkurit tasavälein

Pystysuuntaiset toiminnot ovat vastaavat.

Tarkastellaan esimerkkeinä seuraavien kohteiden jakoa.

{: .figure-medium }
> ![](../inkscape-tasaus-jako_kohteet.png)

Vasemmat reunat tasavälein.

{: .figure-medium }
> ![](../inkscape-tasaus-jaa_vasen.png)

Keskikohdat tasavälein.

{: .figure-medium }
> ![](../inkscape-tasaus-jaa_keski.png)

Oikeat reunat tasavälein.

{: .figure-medium }
> ![](../inkscape-tasaus-jaa_oikea.png)

Kohteiden välillä yhtä paljon tilaa.

{: .figure-medium }
> ![](../inkscape-tasaus-jaa_vali.png)

Tekstien jaossa tekstien ankkuripisteet asetetaan tasavälein.

{: .figure-medium }
> ![](../inkscape-tasaus-jaa_teksti-horiz.png)

## Solmujen tasaus

Edellä olevat tasaukset tehtiin valintatyökalun ollessa käytössä
ja tasaukset olivat erillisten objektien välisiä.
Jos käytössä on solmutyökalu, voidaan tasaustoiminnoilla tasata
myös solmuja samaan linjaan. Joko vaakasuoraan tai pystysuoraan.

{: .figure-normal }
> ![](../inkscape-tasaus-solmut.png)

Ensimmäiseksi pitää taas valita, minkä solmun mukaan tasaus tehdään.

{: .figure-normal }
> ![](../inkscape-tasaus-solmut_minka_mukaan.png)

*Ensimmäiseksi* vai *viimeiseksi valitun*, *valittujen keskiarvon*,
*pienimmän arvon* vai *suurimman arvon* mukaan.

Valitaan kuvasta muutama solmu ja tasataan ne sivusuunnassa samalle
pystysuoralle linjalle viimeisenä valitun ylimmän solmun mukaan.

{: .figure-medium-row-vert }
> ![](../inkscape-tasaus-solmut_alkuperainen.png)
> ![](../inkscape-tasaus-solmut_tasattu-vert.png)
> ![](../inkscape-tasaus-solmut_tasattu-vert-2.png)

Tasaus vaakasuoralle linjalle tapahtuu vastaavasti.

Myös solmuja voi jakaa tasavälein. Joko vaaka- tai pystysuunnassa.

{: .figure-normal }
> ![](../inkscape-tasaus-solmut_jaa.png)

Tasataan vasemmat kärkisolmut tasavälein.

{: .figure-medium-row-vert }
> ![](../inkscape-tasaus-solmut_pystytasaus.png)
> ![](../inkscape-tasaus-solmut_pystytasaus_tehty.png)

## Muita tasauksia

Esiteltyjen lisäksi tasausdialogista löytyy myös muita tasausvälineitä,
joilla voi uudelleenjärjestellä valittuja kohteita esimerkiksi
valintajärjestyksen mukaan, pinojärjestyksen mukaan tai satunnaisesti.

{: .figure-normal }
> ![](../inkscape-tasaus-uudelleenjarjesta.png)

Kohteista voi poistaa päällekkäisyydet jättämällä niiden väliin haluttu
määrä vaaka- ja pystysuuntaista tilaa.

{: .figure-normal }
> ![](../inkscape-tasaus-poista_paallekkaisyydet.png)

Kohteita voi järjestellä ruudukkoon.

{: .figure-normal }
> ![](../inkscape-tasaus-grid.png)

Ja niitä voi asetellä ympyrän muotoon.

{: .figure-normal }
> ![](../inkscape-tasaus-circular.png)

Esimerkiksi:

{: .figure-medium }
> ![](../inkscape-tasaus-circular_kohteet.png)

