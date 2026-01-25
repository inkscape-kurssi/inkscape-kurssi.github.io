---
date: "2026-01-25T18:18:17+03:00"
title: "Polun muokkaaminen"
layout: default
nav_order: 2
parent: Piirtotyökalut
---

# Polun muokkaaminen

{: .figure .figure-right }
![](../inkscape-nodetool-ikoni.png)

Jo olemassa olevia polkuja voi muokata **solmutyökalulla** (node tool), joka on työkalupalkissa
heti valintatyökalun alapuolella. Solmutyökalun voi hiiren lisäksi valita pikanäppäimillä *n* ja *F2*.

## Solmujen valinta ja siirtäminen

Kun solmutyökalu on käytössä, aktiiviseksi valitussa polku-objektissa ovat kaikki sen solmut näkyvissä
pieninä neliön muotoisina siirtokahvoina. Jos solmun kulma ei ole pyöristetty, neliö on kärjellään, ja
jos kyseisen solmun kulma on pyöristetty, siirtokahvan neliö on vaakasuunnassa.

{: .figure-medium-row }
> ![](../inkscape-nodetool-objekti.png)
> ![](../inkscape-nodetool-siirto.png)
> ![](../inkscape-nodetool-valinta.png)
> ![](../inkscape-nodetool-siirto2.png)

Solmusta voi ottaa kiinni hiirellä ja sen voi raahata haluamaansa kohtaan. Useampia solmuja
voi valita yhtä aikaa aktiiviseksi "piirtämällä" hiirellä niiden yli suorakaiteen. Kaikki
suorakaiteen sisään jäävät solmut tulevat valituksi. Solmuja voi valita myös yksitellen
hiirellä klikkaamalla. Klikkaus valitsee kyseisen solmun ja klikkaus *Shift*-nappi pohjassa
lisää uuden solmun valintaan tai poistaa sen siitä.

Jos useampi solmu on yhtä aikaa valittuna, solmusta kiinni ottaminen ja siirtäminen siirtää
kaikkia valuttuja solmuja yhtä aikaa.

Valittuja solmuja voi siirtää myös näppäimistöltä nuolinäppäimillä samoin kuin valintatyökalulla
pystyi siirtämään kokonaisia objekteja. Pelkkä nuolinäppäimen painaminen siirtää solmua vähän.
*Shift* ja nuolinäppäin siirtää solmua kymmenkertaisesti. *Alt*-näppäin pojassa nuolilla siirtäminen
on puolestaan pientä hienosäätöä. Nuolinäppäimillä siirtoja voi siis tehdä paljon
hiirtä tarkemmin ja täsmällisemmin. Tämä on käyttökelpoista esimerkiksi silloin, jos halutaan
siirtää useampia solmuja yhtä suuria etäisyyksiä eri suuntiin.

Yksi hyödyllinen pikanäppäin toiminto on myös *Ctrl-a*, jolla saa nopeasti valittua kaikki
aktiiviseen polkuun tai polkuihin kuuluvat solmut.

Lisäksi on hyödyllistä tietää, että kahden solmun välistä viivaa klikkaamalla työkalu
valitsee molemmat viivan päissä olevat solmut.


## Kulmien ja viivojen pyöristys

Jos polusta valitaan solmu, jota vastaava kulma on pyöristetty, näkyvät siirtokahvan
ympärillä myös pyöreät "venytyskahvat", joilla kulman muotoa voidaan muokata siirtämällä ja venyttämällä.
Jos solmuun ei liity näitä kahvoja, ne saa esiin ottamalla solmusta kiinni hiirellä ja vetämällä
*Shift*-näppäin pohjassa viivan suuntaan. Molempien viivojen suuntaan lähtevät kahvat
ovat venytettävissä erikseen.

{: .figure-medium-row }
> ![](../inkscape-nodetool-kahva.png)
> ![](../inkscape-nodetool-kahva-2.png)
> ![](../inkscape-nodetool-kahva-3.png)
> ![](../inkscape-nodetool-kahva-4.png)

Solmujen väliin jäävän viivan muotoa voi pyöristää ja venyttää myös ottamalla
hiirellä kiinni suoraan viivasta ja venyttämällä sitä haluamallaan tavalla.

{: .figure-medium-row }
> ![](../inkscape-nodetool-viiva-1.png)

## Asetuspalkki

{: .figure-full }
> ![](../inkscape-nodetool-asetukset.png)

Solmutyökalun asetuspalkissa on paljon toimintoja. Käydään niitä läpi vaiheittain.

## Solmujen lisääminen ja poistaminen

Asetuspalkin ensimmäiset napit liittyvät solmujen ja viivojen lisäämiseen, poistamiseen
sekä yhdistelyyn. Nappien kuvakkeet esittävät hyvin, mitä kustakin napista tapahtuu.
Solmujen poistoja ja lisäyksiä voi tehdä joko palkin nappuloiden kautta tai suoraan polkuun.

{: .figure-normal }
> ![](../inkscape-nodetool-lisayspoisto.png)

Uusien **solmujen lisääminen** polkuun tapahtuu helposti klikkaamalla polun viivaa siitä kohdasta,
johon uuden solmun haluaa lisätä. Polun muoto pysyy entisellään, mutta halutuun kohtaan
ilmestyy uusi solmu. Vastaavasti ylimääräisen **solmun voi poistaa** valitsemalla sen ja
painamalla *Del*-näppäintä tai *Backspace*-näppäintä.

Toinen tapa lisätä solmuja on valita polusta haluttu viiva tai viivat valitsemalla sen päätepistinä
olevat solmut. Tämän jälkeen asetuspalkin "plus"-nappia painamalla kyseiseen väliin ilmaantuu uusi
solmu. Suoralla viivalla uusi solmu tulee puoleen väliin. Kaarevalla viivalla sijainti voi olla
painottunut.

Vastaavasti palkin "miinus"-napin painaminen poistaa valitut solmut.

{: .figure-medium-row }
> ![](../inkscape-nodetool-objekti.png)
> ![](../inkscape-nodetool-lisays.png)
> ![](../inkscape-nodetool-poisto.png)

Palkin seuraava nappi tarkoittaa kuvakkeensa mukaisesti toimintoa, joka **yhdistää polun kaksi
avoimen pään solmua yhdeksi solmuksi**. Uusi yhdistetty solmu tulee kahden valitun solmun puoliväliin,
joten kappaleen muoto luonnollisestikin muuttuu.

{: .figure-medium-row }
> ![](../inkscape-nodetool-yhdista-1.png)
> ![](../inkscape-nodetool-yhdista-2.png)

Seuraava nappi tekee myös kuvakkeensa mukaisen toiminnon, eli **katkaisee polun valitun solmun kohdalta**.
Käytännössä yhdestä solmusta tulee kaksi polun päättösolmua, jotka ovat samassa kohdassa.
Katkaisun jälkeen mikään ei näytä muuttuneen, mutta jos näistä kahdesta solmusta valitsee toisen ja
siirtää sitä, tulee katkaisukohta näkyviin, kuten alla olevissa kuvissa.

{: .figure-medium-row }
> ![](../inkscape-nodetool-katkaise-1.png)
> ![](../inkscape-nodetool-katkaise-2.png)

Seuraavat kaksi nappia myöskin sulkevat ja katkaisevat polun valittujen solmujen kohdalta, mutta
erona on se, että polun sulkemista ei tehdä yhdistämällä valitut solmut yhdeksi vaan **yhdistämällä
solmut uudella viivalla**. Vastaavasti katkaiseminen tehdään päinvastoin **poistamalla solmujen välillä oleva viiva**.

{: .figure-medium-row }
> ![](../inkscape-nodetool-yhdista-3.png)
> ![](../inkscape-nodetool-yhdista-4.png)

Kun polusta poistetaan viivoja solmujen väliltä, on hyvä tehdä huomio, että samassa polussa voi
olla useita avoimia päitä. Polun ei siis tarvitse olla suljettu tai vain yksi murtoviiva alkusolmusta
loppusolmuun. Se voi koostua useista murtoviivoista tai suljetuista osista. Tärkeää on myös ymmärtää,
että koska kyseessä on yksi useammasta osasta koostuva polku, sillä voi olla vain yksi täyttöväri,
viivan väri ja yksi viivan paksuus. Tästä aiheesta lisää myöhemmin.

{: .figure-medium-row }
> ![](../inkscape-nodetool-polku_osissa.png)
> ![](../inkscape-nodetool-polku_osissa-2.png)


## Solmujen pehmennys

Asetuspalkin seuraavat napit liittyvät solmujen kohdalle tuleviin kulmiin ja kaariin.
Niillä määrätään solmun tyyppi, joka voi olla **kulma**, **pehmennetty**, **symmetrinen**
tai **automaattinen**.

{: .figure-normal }
> ![](../inkscape-nodetool-solmujen_kulmat.png)

Solmun tyyppinä **kulma** esitetään kärjellään olevalla siirtokahvalla ja se tarkoittaa, että
solmun molemmat "venytyskahvat" ovat siirrettävissä itsenäisesti, jolloin kulmasta voidaan
tehdä juuri niin terävä ja kaartuva kuin piirtäjä haluaa.

{: .figure-medium-row }
> ![](../inkscape-nodetool-kulma-1.png)
> ![](../inkscape-nodetool-kulma-2.png)

**Pehmennetty** solmu esitetään siirtokahvalla, jonka neliö on vaakasuorassa. Pehmennetyssä
solmussa sen venytyskahvat ovat vastakkaisiin suuntiin. Kun toista kahvaa siirretään, toisen
suunta muuttuu samalla. Tämä tekee polun suunnan muuttumisesta solmun kohdalla pehmeän ja sileän.
Venytyskahvojen pituudet ovat kuitenkin toisistaan riippumattomat, eli solmuun "tulevan" ja "lähtevän"
viivan kaarevuudet voivat olla erilaiset.

{: .figure-medium-row }
> ![](../inkscape-nodetool-pehmennetty-1.png)
> ![](../inkscape-nodetool-pehmennetty-2.png)

Solmun kolmas tyyppi on **symmetrinen**, joka esitetään myös vaakasuoralla neliökahvalla.
Symmetrisyys tarkoittaa sitä, että vastakkaissuuntaisuuden lisäksi venytyskahvojen
pituudet ovat myös yhtä suuret. Kun toista venytetään, toinen seuraa perässä.
Polun kaarevuus solmun kohdalla siis sileän lisäksi myös symmetrinen "tulevaan" ja "lähtevään" suuntaan.

{: .figure-medium-row }
> ![](../inkscape-nodetool-symmetrinen-1.png)
> ![](../inkscape-nodetool-symmetrinen-2.png)

Solmun neljäs tyyppi, **automaattinen**, pyrkii nimensä mukaisesti säilyttämään
solmun sileyden myös silloin, kun muita solmuja siirrellään. Automaattinen solmu
esitetään pyöreällä siirtokahvalla. Kun solmu on merkitty automaatiseksi, sen viereisiä
solmuja siirrettäessä automaattisen solmun venytyskahvat kääntyvät automaattisesti
niin, että pehmennys pyrkii säilymään. Automaattisen solmun venytyskahvat ovat näkyvissä
ja niistä näkee venytysten suuruuden ja suunnan, mutta jos venytyskahvoja käyttää,
solmu siirtyy automaattisesta tilasta tavalliseksi pehmennetyksi solmuksi.

{: .figure-medium-row }
> ![](../inkscape-nodetool-automaattinen-1.png)
> ![](../inkscape-nodetool-automaattinen-2.png)

## Venytysten poisto ja lisäys

Asetuspalkin seuraavat kaksi nappia liittyvät solmujen venytyskahvojen lisäämiseen ja poistamiseen.

{: .figure-normal }
> ![](../inkscape-nodetool-suoristus.png)

Jos kahden solmun välinen viiva on kaareva ja se halutaan suoristaa,
tämä tapahtuu valitsemalla kyseinen viiva, eli sen molemmat päätysolmut, ja painamalla suoran
viivan nappia. Tämä käytännössä poistaa viivan päissä olevista solmuista venytyskahvat.

Jos taas suoraan viivaan halutaan lisätä päihin venytyskahvat, se voidaan tehdä valitsemalla
viivan päätysolmut ja painamalla kaarevan viivan nappia. Saman voi toki tehdä jo edellä
mainituilla tavoilla, eli *Shift*-vetämällä solmusta tai vetämällä itse viivasta.

{: .figure-medium-row }
> ![](../inkscape-nodetool-suoristus-1.png)
> ![](../inkscape-nodetool-suoristus-2.png)


## Live Path Effect

**Live Path Effect** on erikoistoiminto, joka voidaan lisätä polulle erillisestä napista.

{: .figure-normal }
> ![](../inkscape-nodetool-lpe-ikoni.png)

Sen käyttäminen
valittuna olevalle polulle lisää kunkin solmun kahvojen viereen ylimääräisen pienen kahvan.
Tällä kahvalla polkuun voi lisätä kulmanpyöristysefektin, joka säilyy kulman
ominaisuutena vaikka solmuja liikutellaan. Tämä on erilainen pyöristys kuin
venytyskahvoilla saavutettava ja tähän kannattaa tutustua kokeilemalla.

{: .figure-medium-row }
> ![](../inkscape-nodetool-lpe-1.png)
> ![](../inkscape-nodetool-lpe-2.png)
> ![](../inkscape-nodetool-lpe-3.png)
> ![](../inkscape-nodetool-lpe-4.png)


## Objekti poluksi

Kaikki piirto-objektit eivät ole polkuja. Muita objektityyppejä ovat esimerkiksi
aiemmin tutustutut suorakulmiot ja ellipsit sekä myöhemmin käsiteltävät
tekstit. Muilla objektityypeillä on omat piirto-ominaisuutensa ja etunsa, mutta
toisinaan ne voidaan haluta muuntaa poluiksi. Tätä varten solmutyökalun
asetuspalkissa ovat kaksi seuraavaa toimintoa.

{: .figure-normal }
> ![](../inkscape-nodetool-poluksi-ikoni.png)

Näistä ensimmäinen muuntaa muuta tyyppiä olevat **objektit poluiksi**.
Kun valintatyökalu on käytössä, alareunan vihjepalkissa
näkyy tekstinä valitun piirto-objektin tyyppi. Alla olevassa ensimmäisessä kuvassa
näkyy, että valittuna on suorakulmio, jonka kulmat on pyöristetty.
Toisessa kuvassa käyttöön on valittu solmutyökalu, jolloin suorakaiteen ominaisuuksien
kahvat ovat tulleet näkyviin. Solmutyökalulla voi muokata myös suorakaiteita.
Kolmannessa kuvassa on painettu asetuspalkin "muuta poluksi" -painiketta ja suorakaide
on muttunut vastaavan muotoiseksi poluksi, jossa on kuusi solmua.
Neljännessä kuvassa on vielä otettu valintatyökalu käyttöön, jolloin vihjepalkki vahvistaa,
että kyseessä on nyt polku.

{: .figure-medium-row }
> ![](../inkscape-nodetool-poluksi-1.png)
> ![](../inkscape-nodetool-poluksi-2.png)
> ![](../inkscape-nodetool-poluksi-3.png)
> ![](../inkscape-nodetool-poluksi-4.png)

Kun suorakulmio on muunnettu poluksi, sitä ei voi enää käsitellä suorakulmiona. Se on
menettänyt suorakulmion rajoitteet ja sitä voidaan muokata tästä lähtien polkuobjektin
vapaudella.

Toinen poluksi muuntava toiminto on **viivat poluiksi**. Tämän työkalun käytössä on kyse
nimensä mukaisesti siitä, että piirretty viiva muutetaan itsensä reunapoluksi.
Tämän tarkoitus käy ehkä parhaiten ilmi alla olevista kuvista. Ensimmäisessä on
polku, joka koostuu kahdesta solmusta ja niiden välisestä paksusta punaisesta ja
kaarevasta viivasta. Toisessa kuvassa tämän polun viiva on muutettu poluksi, jolloin
viivasta onkin tullut uuden polun sisäosa. Uusi polku seuraa vanhan ääriviivoja ja
viivan väri on vaihtunut uuden polun täyttöväriksi. Uudella polulla ei ole nyt
ääriviivoja vaan pelkkä täyttöväri. Tämä on toisinaan hyvin käyttökelpoinen
muunnos.

{: .figure-medium-row }
> ![](../inkscape-nodetool-stroketopath-1.png)
> ![](../inkscape-nodetool-stroketopath-2.png)
