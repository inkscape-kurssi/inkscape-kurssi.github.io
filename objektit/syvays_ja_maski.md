---
date: "2026-01-31T11:20:00+03:00"
title: "Syväys ja maski"
layout: default
nav_order: 5
parent: Objektit
---

# Syväys ja maski

Syväyksessä ja maskissa on kyse siitä, että yhdellä objektilla
määritellään ja rajataan toisen objektin näkyvyyttä.

Molemmat toiminnot löytyvät "Kohde"-valikosta.
Tarkastellaan niiden toimintaa esimerkeillä.

## Syväys

Syväyksellä tarkoitetaan jonkin kuvan tai muun objektin rajaamista
ja irroittamista taustastaan. Inkscapessa syvääminen tapahtuu
kahden objektin yhteistyönä. Ensimmäinen objekti on itse
syvättävä kuva, josta halutaan rajata tai leikata jokin
osa irti. Toinen objekti on polku, joka määrää rajauksen
reunaviivan.

Aloitetaan esimerkki valitsemalla syvättävä kuvaobjekti ja
polkuobjekti, jota käytetään tekemään rajaus.

{: .figure-normal }
![Syvättävä kuva ja rajaukseen käytettävä polku](../inkscape-syvays-objektit.png)

Asetellaan objektit pääällekkäin niin, että rajaava polku on kuvan päällä
siten kuin rajaus halutaan tehdä. Valitaan molemmat objektit.

{: .figure-normal }
![Syvättävä kuva ja rajaukseen käytettävä polku päällekkäin ja valittuina](../inkscape-syvays-objektit_paallekkain.png)

Valitaan "Kohde"-valikosta vaihtoehto "Syväys" ja sen alta "Set Clip".
Tämän pikanäppäin on *Ctrl-M*. Kuvankäsittelyohjelmissa
termi "Clip" tarkottaa yleensä rajaamista tai leikkaamista rajoja myöten.

{: .figure-normal }
![Syväyksen asettaminen](../inkscape-syvays-valikko.png)

Tämä toiminto asettaa kuvalle "rajauspolun" ("clip-path"), ja nyt siitä näkyy
vain polun sisälle jäävä osuus. Kaikki sen ulkopuolelle jäävä leikkautuu pois.

{: .figure-normal }
![Kuvasta rajattu sydämen muotoinen alue.](../inkscape-syvays-syvatty.png)

Syväys on mahdollista vaihtaa myös käänteiseksi, jolloin kuvasta jääkin
näkyviin rajatun alueen ulkopuoli. Tällä tavalla voidaan esimerkiksi
tehdä kuvaan "reikä", josta näkyy läpi jotain taustalla olevaa.

Tämä tapahtuu saman valikon valinnalla "Set Inverse Clip".

{: .figure-normal }
![Syväyksen asettaminen käänteiseksi](../inkscape-syvays-valikko_kaanteinen.png)

Ja lopputulos näyttää tässä tapauksessa tältä.

{: .figure-normal }
![Käänteinen syväys](../inkscape-syvays-kaanteinen.png)

Käytössä olevan syväyksen voi poistaa saman valikon valinnalla "Release Clip".

{: .figure-normal }
![Syväyksen poistaminen](../inkscape-syvays-valikko_poisto.png)

Tämä poistaa syväyksen ja palauttaa käytetyn polun näkyviin erillisenä objektina.


# Maski

Maskilla tarkoitetaan kuvankäsittelyssä yleensä mustavalkoista kuviointia,
jolla määritellään, mitkä osat varsinaisesta kuvasta ovat läpinäkyviä
ja mitkä peittäviä. Inkscapessa maskin käyttö tapahtuu samaan tapaan
kuin syväyksen käyttö. Maskin toteuttamiseen tarvitaan kaksi objektia.
Ensimmäinen objekti on varsinainen kuva, johon maskia sovelletaan
ja toinen objekti on itse maski.

Käytetään esimerkkeinä vastaavia objekteja kuin syväyksessä.
Muutetaan rajaukseen käytetty polku maskiksi täyttämällä
se mustavalkoisella väriliu'ulla.

{: .figure-normal }
![Kuva, johon maskia käytetään, ja maskina toimiva polku](../inkscape-maski-objektit.png)

Asetellaan objektit halutulla tavalla päällekkäin, maski päällimmäisenä.
Valitaan molemmat objektit.

{: .figure-normal }
![Kuva, johon maskia käytetään, ja maskina toimiva polku päällekkäin](../inkscape-maski-objektit_paallekkain.png)

Maskin asettaminen tapahtuu aivan samoin kuin syväyksenkin, eli
"Kohde"-valikon kohdasta "Maski" ja "Set Mask".

{: .figure-normal }
![Maskin asettaminen valikosta](../inkscape-maski-valikko.png)

Lopputuloksena maski sekä rajaa kuvan että asettaa sille läpinäkyvyyden
niin, että kaikki, mikä oli maskissa täysin mustaa, on täysin läpinäkyvää
ja kaikki, mikä oli maskissa täysin valkoista, on täysin peittävää.

Mustan ja valkoisen välillä olevat sävyt määräävät vastaavasti
läpinäkyvyyden näiden kahden ääripään väliltä.

Inkscapessa maski voi olla myös värillinen. Peittävyys ja läpinäkyvyys
määräytyy värin tummuuden mukaan.

{: .figure-normal }
![Maski käytössä](../inkscape-maski-maskattu.png)

Samoin kuin syväyksen kanssa, myös maskin voi laittaa käänteisenä.
Silloin maskin ulkopuoli pysyy kokonaan näkyvissä. Itse maskin
alueeseen tämä ei vaikuta vaan musta tarkoittaa edelleen läpinäkyvää
ja valkoinen peittävää.

{: .figure-normal }
![Maski käänteisenä](../inkscape-maski-kaanteinen.png)

Havainnollistetaan läpinäkyvyyttä vielä laittamalla kuvan taustalle punainen
taustapalkki, joka näkyy kuvasta läpi.

{: .figure-normal }
![Maski ja tausta](../inkscape-maski-tausta.png)

Vastaavasti kuin syväyksellä, maskin poistaminen tapahtuu
valitsemalla "Kohde"-valikosta "Maski" ja "Release Mask".

Näytetään vielä sama hieman monimutkaisemmalla maskilla.

{: .figure-medium-row }
> ![Maskissa sisäkköisiä sydämiä eri suuntiin menevillä väriliu'uilla](../inkscape-maski-monimutkaisempi.png)
> ![Maski käytössä](../inkscape-maski-monimutkaisempi_maskattu.png)
