---
date: "2026-01-31T11:20:00+03:00"
title: "Joukko-operaatiot"
layout: default
nav_order: 5
parent: Piirtotyökalut
---

# Joukko-operaatiot

*Joukko-operaatioilla*, eli *Boolen-operaatioilla* tarkoitetaan
polkuobjekteille tehtäviä operaatioita, joissa polun sisäosille
tehdään joukko-opista tuttuja toimintoja. Operaatioihin osallistuvat
kohteet voivat olla myös esimerkiksi ellipsejä tai suorakulmia.
Ne muunnetaan automaattisesti poluiksi ennen operaation suorittamista.
Inkscapen **"Polku"**-valikosta löytyvät seuraavat toiminnot. Käytetään esimerkkinä
kahta päällekkäin olevaa polkuobjektia, joille toiminnot tehdään.

{: .figure-normal }
> ![Keltainen ellipsi ja punainen suorakulmio päällekkäin. Mustat reunaviivat](../inkscape-joukot-kaksi_kohdetta.png)

## Yhdiste eli unioni

Joukko-opissa *yhdiste* eli *unioni* tarkoittaa operaatiota, joka yhdistää
kahden joukon alkiot yhteen. Kahden polun unioni tuottaa
uuden polun, jonka sisäosana ovat molempien polkujen sisäosat.
Yhdisteen pikanäppäimenä on *Ctrl-+*. (control plus)

Eli edellä olevien polkujen yhdiste on:

{: .figure-normal }
> ![Ellipsi ja suorakulmio on yhdistetty yhdeksi kuvioksi](../inkscape-joukot-unioni.png)

Huomattavaa on, että unionissa valitut kohteet yhdistetään alimpaan kohteeseen ja
uusi kohde perii täytön ja reunan värit alimmalta valitulta kohteelta.

## Erotus

*Erotus* tarkoittaa, että alemmasta valitusta kohteesta poistetaan sen päällä olevan
kohteen osuudet. Kohteita täytyy olla valittuna täsmälleen kaksi kappaletta.
Päällä olevasta kohteista ei jää mitään jäljelle. Erotuksen pikanäppäin on
*Ctrl- -*. (control miinus)

{: .figure-normal }
> ![Ellipsistä on poistettu suorakulmion osat, jotka ovat sen päällä](../inkscape-joukot-erotus.png)

## Leikkaus

Joukko-opissa *leikkaus* (englanniksi "intersection") tarkoittaa kaikkia niitä osia, jotka ovat
kohteille yhteisiä. Inkscapessa leikkaukseen voi osallistua
useita kohteita yhtä aikaa. Jäljelle jäävä kuvio on se osuus, joka
on kaikille kohteille yhteinen. Leikkauksen pikanäppäin on *Ctrl-\**. (control tähti)

{: .figure-normal }
> ![Ellipsin ja suorakulmion päällekkäin osuvat osuudet eli leikkaus](../inkscape-joukot-leikkaus.png)

## Poisto

*Poisto* on leikkaukselle vastakkainen operaatio. Siinä lopputuloksena
on kuvio, jossa ovat ne osat valituista kohteista, jotka eivät ole päällekkäin.
Siis kuin kohteiden unioni, josta on poistettu niiden leikkaus.
Tai kuin kohteista molemmin päin otetut erotukset yhdistettyinä.
Poiston pikanäppäin on *Ctrl-^*. (control hattu)

{: .figure-normal }
> ![Ellipsin ja suorakulmion ei päällekkäin osuvat osuudet eli poisto](../inkscape-joukot-poisto.png)

Poiston kanssa on kuitenkin syytä huomioida, että jos se tehdään useamman kohteen
kanssa, päällekkäisistä osista lasketaan parillisuuden mukaan, mitkä osat jäävät
ja mitkä eivät. Osat, joissa on vain yhtä kohdetta päällekkäin jäävät.
Osat, joissa on kahta kohdetta päällekkäin poistetaan. Osat, joissa on kolmea
kohdetta jäävät taas jäljelle. Jos kohteita olisi useampia, parittomat jätetään
ja parilliset päällekkäisyydet poistetaan.

{: .figure-medium-row }
> ![Ellipsi ja kaksi suorakulmiota osittain päällekkäin](../inkscape-joukot-kolme_kohdetta.png)
> ![Kolmen kohteen välinen poisto](../inkscape-joukot-poisto-3.png)


## Jako

Inkscapessa *jako* tarkoittaa alemman kohteen jakamista osiin sen mukaan, mitkä
osat ovat päällekkäin toisen kohteen kanssa ja mitkä eivät.
Käytännössä siis kohteille tehdään sekä erotus että leikkaus ja molemmat
jäävät jäljelle erillisinä uusina polkuina.

Voidaan myös ajatella, että päällimmäisen kohteen reunaviiva leikkaa alemman
kohteen kahteen osaan. Jaon pikanäppäimenä on *Ctrl-/*. (control jakoviiva)

{: .figure-normal }
> ![Ellipsi on jaettu kahteen osaan suorakulmion mukaisesti](../inkscape-joukot-jako.png)


## Polun leikkaus

*Polun leikkaus* voi suomenkielisenä käännöksenä helposti sekoittua edellä olevaan
leikkaukseen. Tämä kuitenkin tarkoittaa tilannetta, jossa leikattaan kuin veitsellä tai saksilla
polku osiin. (englanniksi "cut") Tässä toiminnossa päällimmäinen kohde
leikkaa alemman kohteen reunaviivan osiin. Tämä eroaa edellä olevasta jaosta
siinä, jaossa ositetaan täyttöosaa, polun leikkauksessa vain reunaviivaa.
Pikanäppäimenä *Ctrl-Alt-/*.

{: .figure-normal }
> ![Ellipsin reunaviiva on jaettu kahteen osaan suorakulmion mukaisesti](../inkscape-joukot-polun_leikkaus.png)

# Shape Builder -työkalu

{: .figure .figure-right }
![Shape Builder -työkalun kuvake työkalupalkissa](../inkscape-shapebuilder-ikoni.png)

Joukko-operaatioiden muodostamiseen löytyy myös erillinen työkalu, *Shape Builder*,
joka on työkalupalkissa ja jonka pikanäppäin on *X*.

Kun Shape Builder käynnistetään, se sumentaa piirtoalueen ja antaa
merkitä valituista kohteista hiirellä niiden päällekkäin osuvista 
tai ei päällekkäisistä osista, mitkä halutaan ottaa mukaan ja mitä
ei.

{: .figure-medium-row }
> ![Shape Builderin valintanäkymä](../inkscape-shapebuilder-1.png)
> ![Hiiri yhdenosan päällä](../inkscape-shapebuilder-2.png)
> ![Valittuna yksi osa ja hiiri toisen osan päällä](../inkscape-shapebuilder-3.png)
> ![Kaksi osaa valittuina](../inkscape-shapebuilder-4.png)

Shape Builderin asetuspalkissa on valinta, lisätäänkö vai poistetaanko
osia ja napit valinnan hyväksynnälle tai perumiselle. Lisäksi 
palkissa on säätö sumennuksen voimakkuudelle sekä valinta sille,
jätetäänkö alkuperäiset kohteet operaation jälkeen piirtoalueelle
vai poistetaanko ne.

{: .figure-medium }
> ![Shape Builderin asetuspalkki](../inkscape-shapebuilder-asetukset.png)

Yllä oleva valinta tuottaa alla olevan kuvan mukaisen lopputuloksen.
Huomaa, että toisin kuin joukko-operaatioissa, lopputuloksena ei ole
yksi path-objekti vaan jokainen kohde on erillinen objekti, jolla on
oma värityksensä.

{: .figure-medium }
> ![Shape Builderin tulos](../inkscape-shapebuilder-valmis.png)


# Polku-operaatiot

Esitellään tässä yhteydessä vielä samassa "Path"-valikossa olevat
"polkuoperaatiot", jotka eivät ole varsinaisia joukko-operaatiota,
vaan muita poluille tehtäviä toimintoja.

Käytetään näille operaatioille esimerkkinä seuraavia kolmea
kohdetta.

{: .figure-normal }
> ![Keltainen ympyrä ja vihreä sekä oranssi suorakulmio](../inkscape-polut-kolme_kohdetta.png)

## Yhdistä

*Yhdistä*-toiminto, jonka pikanäppäin on *Ctrl-K*, yhdistää useamman polun
yhdeksi poluksi. Kun kohteet on yhdistetty yhdeksi poluksi, niille ei voi enää
määrätä erilaisia värejä ja niitä ei voi liikuttaa toisistaan erillään.
Ne ovat saman polun osia.

Kuvassa yhdistetty polku, joka on perinyt päällimmäisen kohteen värit. Toisessa
kuvassa ovat näkyvissä polun kaikki solmut ja viivat.

{: .figure-medium-row }
> ![Kohteet yhdistetty yhdeksi poluksi](../inkscape-polut-yhdista-1.png)
> ![Kohteet yhdistetty yhdeksi poluksi ja solmut ovat näkyvissä](../inkscape-polut-yhdista-2.png)

## Katkaise

*Katkaise* on edeliselle yhdistämiselle vastakkainen operaatio. Se irrottaa samassa
polussa olevat alipolut omiksi path-objekteikseen, joita voidaan käsitellä erikseen
ja määrätä niille erilaiset värit ja reunaviivan ominaisuudet.

Katkaisun pikakomento on *Shift-Ctrl-K*.

{: .figure-normal }
> ![Alipolut katkaistu erillisiksi path-objekteiksi](../inkscape-polut-katkaise.png)

## Split path

*Split Path* on hyvin saman tapainen toiminto kuin katkaise, mutta sen ero
on siinä, että vain alipolut, jotka eivät ole päällekkäin, erotetaan
omiksi objekteikseen. Esimerkiksi alla olevassa kuvassa ympyrä ja suurempi
suorakulmio ovat päällekkäin, joten ne ovat pysyneet samana polku-objektina,
mutta niistä erillään oleva pienempi suorakulmio on erotettu erilliseksi
objektiksi.

Tämä toiminnallisuus voi olla hyödyllinen esimerkiksi erotettaessa
poluksi muunnetusta tekstistä kirjaimia erillisiksi objekteiksi.

Pikanäppäimenä tälle toiminnolle on *Shift-Ctrl-Alt-K*.

{: .figure-normal }
> ![Ei päällekkäin olevat lipolut katkaistu erillisiksi path-objekteiksi](../inkscape-polut-split_path.png)

## Fracture

*Fracture*-toiminto murtaa valituista kohteista päällekkäin olevat osuudet
irti omiksi polku-objekteiksi. Esimerkiksi alla olevassa kuvassa
keltainen näkyvä osuus ympyrästä on yksi objekti, ympyrän ja
vihreän suorakulmion leikkaus on muuttunut yhdeksi objektiksi ja
loput vihreästä suorakulmiosta on oma objektinsa.

Toiminnon pikanäppäin on *Ctrl-Alt-F*.

{: .figure-normal }
> ![Fracturella päällekkäiset osat murrettu irti toisistaan.](../inkscape-polut-fracture.png)

## Flatten

*Flatten*-toiminto muuttaa kaikki valittujen kohteiden osat erillisiksi polkuobjekteiksi.
Alla olevassa kuvassa osia on siirretty hieman, jotta niiden erillisyys näkyy.
Kaikki polkujen sisäosat on irroitettu reunaviivoista, reunaviivat on muutettu
niitä ympäröiviksi poluiksi ja yhden kohteen ollessa toisen alla siitä ja sen reunaviivasta
ovat jääneet jäljelle vain näkyvillä olleet osuudet. Pikanäppäin tälle on *Shift-F*.

Tämän toiminnon jälkeen mikään objekteista ei ole enää toisen alla.

{: .figure-normal }
> ![Flatten irrottanut kaikki näkyvät osat erikseen.](../inkscape-polut-flatten.png)


{: .exercises }
> Lataa alla olevat SVG-tiedostot (hiiren oikealla napilla "Tallenna kohde levylle")
> ja avaa ne Inkscapella. Tiedostot sisältää harjoitustehtäviä, joilla harjoitellaan
> joukko-operaatioden ja polkuoperaatioiden käyttöä.
> 
> [Harjoitus - Joukko-operaatiot](/files/harjoitus-joukko-operaatiot.svg)
>
> [Harjoitus - Polkuperaatiot](/files/harjoitus-polkuoperaatiot.svg)
