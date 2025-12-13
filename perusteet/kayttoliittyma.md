---
date: "2025-12-13T14:30:00+03:00"
title: "Käyttöliittymä"
layout: default
nav_order: 1
parent: Perusteet
---

# Käyttöliittymä

Kun Inkscape käynnistetään, sille avautuu yksi ikkuna. Ikkunan jokaisessa reunassa
on erilaisia työkaluja ja onkin hyvä heti aluksi opetella, mistä löytyy mitäkin.
Käydään lyhyesti läpi ohjelman ikkunassa näkyvän käyttöliittymän osat.

## Piirtoalue ja sivu

Inkscapen käyttöliittymässä ikkunan keskellä on piirtoalue ja siinä suorakaiteen
muotoinen rajattu alue eli sivu. Sivun koko ja muoto ovat valittavissa asetuksista.
Oletuksena se on pystysuuntaisen A4-paperin muotoinen ja kokoinen. Piirto-objekteja
on mahdollista sijoittaa piirtoalueelle myös merkityn sivun ulkopuolelle, mutta
tallennettua kuvaa tarkastellessa, esimerkiksi verkkosivulla, vain sivun sisäpuoli on näkyvissä.

{: .figure-full }
> ![](../inkscape_ui.png)
> Inkscapen käyttöliittymän osat ovat ikkunan reunoilla.

## Valikko

Ikkunan yläreunassa on ohjelman valikko, josta löytyvät normaalit tiedosto- ja
muokkausvalinnat sekä lukuisia muita toimintoja.

Piirtoalueen ympärillä ikkunan eri reunoilla on joukko nappulapaneleja ja dialoginäkymiä.

## Komentopalkki

Ikkunan yläreunassa heti valikon alapuolella on komentopalkki, jossa on
pikavalintoja joillekin usein tarvittaville toiminnoille, kuten tiedostojen
avaamiselle ja tallentamiselle. Nämä toiminnot löytyvät pääsääntöisesti myös
valikosta eri kohdista, mutta tästä palkista ne ovat kätevästi saatavilla.
Näitä toimintoja ovat esimerkiksi uuden tiedoston luonti, tiedoston
avaus ja tallentaminen, kopiointi, leikkaus, liittäminen sekä kumoustoiminnot.

Samasta palkista on avattavissa esiin myös erinäisiä *dialoginäkymiä*, kuten
täytön ja reunan asetukset, tasot, tasausasetukset sekä piirtoalueen asetukset.

## Työkalurivi

Työkalurivi on ikkunan vasemmassa reunassa pystysuuntaisesti oleva rivi nappuloita.
Näillä valitaan kulloinkin käytössä oleva työkalu. Työkalut ovat järjestyksessä
ylhäältä alaspäin:

- Valitse ja muunna kohteita
- Muokkaa polun solmuja
- Luo muotoja boolean työkalulla (uudemmissa versioissa)
- Luo suorakulmioita ja neliöitä
- Luo ympyröitä, ellipsejä ja kaaria
- Luo tähtiä ja monikulmioita
- Luo 3D-laatikoita
- Luo spiraaleja
- Piirrä suoria ja Bézier-viivoja
- Piirrä viivoja käsivaraisesti
- Piirrä kalligrafisia tai sivellinviivoja
- Luo ja muokkaa tekstikohteita
- Luo ja muokkaa liukuvärejä
- Luo ja muokkaa mesh-verkkoja
- Poimi värit kuvasta
- Täytä suljettuja alueita
- Muokkaa kohteita veistämällä tai maalaamalla
- Suihkuta valittuja kohteita sprayn tapaan
- Poista polut
- Luo liittimiä
- LPE-työkalu. Luo geometrisia muotoja (uudemmissa versioissa)
- Mittaustyökalu
- Lähennä ja loitonna

Lähes kaikille työkalulle on lisäksi pikanäppäin, jolla sen voi valita nopeasti näppäimistöllä.
Pikanäppäimen näkee työkaluvihjeenä, kun hiiren vie työkalun napin päälle. Esimerkiksi
valintatyökalun voi ottaa käyttöön nopeasti painamalla näppäimistön **s**-näppäintä.

Kullekin työkaluista on asetuksissa joitakin työkalukohtaisia asetuksia, joita
pääsee muokkaamaan kaksoisnapauttamalla työkalun kuvaketta.

## Työkalukohtaiset asetukset ja toiminnot

Piirtoalueen yläpuolella olevan palkin sisältö vaihtuu sen mukaan, mikä työkalu kulloinkin
on valittuna. Siellä ovat nähtävillä kuhunkin työkaluun liittyvät valinnat, asetukset
ja toiminnot. Esimerkiksi valintatyökalun ollessa käytössä, tässä palkissa ovat
muun muassa piirtoalueelta valitun kohteen sijainnin koordinaatit ja koko sekä
toiminnot kohteen peilaamiselle ja kiertämiselle.

{: .figure-full }
![](../inkscape_valinta-asetukset.png)

Tekstityökalulle täältä löytyvät
puolestaan esimerkiksi kirjasimen (fontin) valinta, kirjasimen koko ja kirjasimen tyyli
(lihavointi, kursivointi).

{: .figure-full }
![](../inkscape_teksti-asetukset.png)

Kullekin työkalulle valintoja on useita ja niiden merkityksiin voi tutustua parhaiten
lukemalla niiden työkaluvihjeet sekä kokeilemalla.

## Väripaletti ja tilarivi

Ikkunan alareunassa on esillä väripaletti, josta piirroksen eri kohteille voi valita
reuna- ja täyttövärin. Hiiren vasen klikkaus värin päällä vaihtaa kyseisen värin
valitun kohteen täyttöväriksi. Hiiren vasen klikkaus näppäimistön *shift*-näppäin
painettuna vaihtaa valitun kohteen reunavärin.

{: .figure-full }
![](../inkscape_varipaletti.png)

Jos paletissa on paljon värejä, on se vieritettävissä joko pysty- tai sivusuunnassa,
riippuen Inkscapen versiosta tai asetuksista. Paletin
oikean reunan napista voi valita tarjolla olevista paleteista haluamansa värivalikoiman.

{: .figure-small }
![](../inkscape_palettivaihtoehdot.png)


Paletin alapuolella on tilarivi, jossa ovat nähtävillä parhaillaan valitun
kohteen täyttö- ja reunaväri, kohteen peittävyys prosentteina, pikavalintoja
tasoasetuksille sekä tila- ja vihjeteksti.

Tila- ja vihjeteksti kertoo jatkuvasti, minkälainen kohde on valittuna tai
mitä toimintoja käytössä olevalla työkalulla voi tehdä.

{: .figure-full }
![](../inkscape_vari_ja_vihje.png)

## Kohdistusvalinnat

Ikkunan reunassa äärimmäisenä oikealla ylhäällä ovat kohdistus- eli tartuntavalinnat.

{: .figure-small }
![](../inkscape_snapping.png)

Näillä valinnoilla voi valita monipuolisesti, miten piirtokohteet ja niiden
pisteet siirrettäessä ja skaalattaessa "takertuvat" tai "napsahtavat" muihin
kohteisiin, kohteiden solmupisteisiin, piirtoalueen reunoihin, koordinaatiston
ruudukon pisteisiin ynnä muihin piirtoalueen kohtiin. Asetukset ovat "päälle/pois"
valintoja. Erilaiset tavat kohdistaa kohteita helpottavat niiden sijoittamista täsmällisesti
toisiinsa nähden. Magneettia esittävästä napista tarttumisominaisuuden
voi laittaa päälle tai kokonaan pois päältä.

## Telakoidut dialogit

Lisäksi ikkunan oikeaan reunaan, piirtoalueen viereen,
on mahdollista avata erilaisia dialoginäkymiä telakoituna. Tämä tarkoittaa sitä,
että dialoginäkymät on mahdollista irrottaa omiksi pieniksi ikkunoikseen taikka
kiinnittää (telakoida) pääikkunan reunaan. Tällaisia dialogeja ovat esimerkiksi
tasonäkymä, täyttö- ja viiva-asetukset sekä objektien tasaus.
