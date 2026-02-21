---
date: "2026-01-31T11:20:00+03:00"
title: "Mittatyökalu"
layout: default
nav_order: 2
parent: Apuvälineet
---

# Mittatyökalu

{: .figure .figure-right }
![Kynätyökalun kuvake työkalupalkissa](../inkscape-mitta-ikoni.png)

*Mittatyökalu* on tarkoitettu auttamaan janojen pituuksien ja
kulmien suuruuksien mittaamisessa. Sen pikanäppäin on *M*.

Kun työkalu on valittuna, ovat sen asetukset valittavissa komentopalkissa.

{: .figure-full }
![Mittaustyökalun asetuspalkki](../inkscape-mitta-palkki.png)

Numeerisesti voidaan valita työkalun mittauksien näyttämiseen
käytettävä kirjasinkoko, tarkkuus, skaalaus sekä siirtymä.
Käytettävä mittayksikkö valitaan pudotusvalikolla.

Skaalauksella tarkoitetaan skaalausta piirroksen koosta johonkin
haluttuun suhteeseen. Esimerkiksi piirros on voitu tehdä
tietyssä millimetrikoossa, mutta se vastaa luonnossa jotain
suurempaa tai pienempää asiaa.

Siirtymällä tarkoitetaan etäisyyttä mitattavasta kohteesta,
jos mittaustulos merkitään piirrokseen näkyviin. Tästä lisää,
kohdassa "Merkitse mitat".

## Etäisyyden mittaaminen

Oletuksena mittaustyökalu näyttää kulloinkin hiiren alla olevan
kohteen oleellisimmat mitat: Leveyden, korkeuden, x-koordinaatin,
y-koordinaatin sekä pituuden. Neljä ensimmäistä ovat samat
tiedot, jotka näkyvät valintatyökalun asetuspalkissa valitulle
kohteelle. Pituus on kohteen reunaviivan yhteenlaskettu pituus.
Esimerkiksi alla olevassa kuvassa suorakulmion piiri.

{: .figure-medium }
![Mittaustyökalu näyttää lukemat kohteen päällä](../inkscape-mitta-hover.png)

*Etäisyyden*, esimerkiksi *janan pituuden*, mittaaminen tapahtuu
painamalla hiiren nappi pohjaan aloituspisteessä ja raahaamalla
mittausjana loppupisteeseen. Kun hiiren napista päästää irti,
mitattu matka jää näkyviin ja mittajanan alku- ja loppupäitä
on mahdollista siirtää vielä tämän jälkeen. Jos hiiren tarttumistoiminto
on päällä, aloitus ja lopetuspisteet napsahtavat automaattisesti
erilaisiin kohtiin, kuten polkujen solmuihin, polkuihin,
polkujen leikkauskohtiin, apuviivoihin riippuen tarttumistoiminnon
asetuksista.

Alla olevissa kuvissa on havainnollistettuna mittajanan raahaaminen,
valmis mittaus sekä mittajanan päätepisteen siirtäminen mittaamaan
suorakulmion sivun sijan sen lävistäjä. Viimeisessä kuvassa nähdään
vaikutus, kun asetuspalkissa kirjasinkokoa muutetaan suuremmaksi.

{: .figure-medium-row }
> ![Etäisyyden mittaaminen: raahaus](../inkscape-mitta-etaisyys-1.png)
> ![Etäisyyden mittaaminen: valmis](../inkscape-mitta-etaisyys-2.png)
> ![Etäisyyden mittaaminen: mittajanan päätepistettä siirretty](../inkscape-mitta-etaisyys-3.png)
> ![Mittalukemat skaalattuina](../inkscape-mitta-etaisyys_skaalattu.png)

## Kulman mittaaminen

*Kulmien suuruuksia* voi mitata samalla työkalulla. Kun muodostetaan mittajana,
työkalu näyttää samalla janan kallistuskulman suhteessa vaakasuoraan.
Huomioitavaa on, että 0 astetta on vaakasuoraan aloituspisteestä oikealle
ja kulman suuruus kasvaa siitä myötäpäivään 180 asteeseen saakka.
Myötäpäivään mentäessä kulmat ovat negatiivisia.

{: .figure-medium }
![Mittajanan kulma suhteessa vaakasuoraan](../inkscape-mitta-kulman_mittaus-1.png)

Jos mittajanaa piirrettäessä, kun hiiren nappi on vielä pohjassa, näpäytetään
*Ctrl*-näppäintä, mittatyökalu lukitsee tämän vertailusuunnaksi vaakasuoran sijaan.
Sen jälkeen mittajanan pään siirtämistä voidaan jatkaa johonkin toiseen suuntaan.
Näin saadaan mitattua minkä tahansa kulman suuruus.

{: .figure-medium }
![Kolmion kärkikulman mittaaminen](../inkscape-mitta-kulman_mittaus-2.png)

## Päällä / pois -napit

Jos mittajana ylittää useita kohteita, niiden reunojen ylityksiin syntyy leikkauspisteitä.
Leikkauspisteet merkitään näkyviin ja mittajanan koko pituuden lisäksi näytetään
myös osajanojen pituudet.

{: .figure-medium }
![Osajanojen pituudet: Ei ensimmäistä ja viimeistä](../inkscape-mitta-janojen_osat-01.png)

### Älä huomioi ensimmäistä ja viimeistä

Oletuksena asetuspalkissa on päällä
asetus *Jätä ensimmäinen ja viimeinen huomiotta* ("Ignore first and last").

{: .figure-normal }
![Jätä ensimmäinen ja viimeinen huomiotta](../inkscape-mitta-ignore_first_and_last.png)

Tämä jättää pois näkyvistä ensimmäisen ja viimeisen pätkän
mitat, eli mittajanan alusta ensimmäiseen leikkauspisteeseen ja viimeisestä leikkauspisteestä
mittajanan loppupäähän. Tätä ominaisuutta käyttämällä voi siis mitata esimerkiksi kahden janan etäisyyden
vain piirtämällä mittajanan niiden yli iman, että tarvitsee saada mittajanan
päitä osumaan juuri täsmälleen viivojen kohdalle.

Jos tämän asetuksen laittaa pois päältä, myös näiden osuuksien sekä koko janan
pituudet näytetään.

{: .figure-medium }
![Osajanojen pituudet: Kaikki osat](../inkscape-mitta-janojen_osat-02.png)

### Mittaa vain valittu

Asetus *Mittaa vain valittu* ("Measure only selected") jättää puolestaan kaikki osajanat merkitsemättä.

{: .figure-normal }
![Mittaa vain valittu -valinta](../inkscape-mitta-vain_valittu.png)

Tämä asetus päällä sama mittaus näyttää tältä.

{: .figure-medium }
![Osajanojen pituudet: Kaikki osat](../inkscape-mitta-janojen_osat-03.png)

### Mittaa kaikki tasot

Jos asetuksista on päällä valinta *Mittaa kaikki tasot*, mittaus koskee
kaikilla tasoilla olevia kohteita, joiden yli mittausjana kulkee.

{: .figure-normal }
![Mittaa kaikki tasot -valinta](../inkscape-mitta-mittaa_kaikki_tasot.png)

Tässä kuvassa alla oleva ympyrä on alemmalla tasolla ja muut piirtokuviot
sen päällä olevalla tasolla. Mittausjanaan tulee merkintä jokaiseen kohtaan,
jossa se leikkaa jonkin polun ja mittajanan jokainen osuus mitataan.

{: .figure-medium }
![Mitataan kaikilla tasoilla](../inkscape-mitta-kaikki_tasot.png)

### Kohteiden väliset etäisyydet

{: .figure-normal }
![Näytä kohteiden väliset etäisyydet -valinta](../inkscape-mitta-between_items.png)

*Näytä kohteiden väliset etäisyydet* ("Show measures between items") -valinnalla
valitaan, näytetäänkö mittauksessa myös kaikkien mittauksen matkalla olevien
kohteiden väliset etäisyydet vai ei.

Alla esimerkkikuvat, joista ensimmäisessä kaikki etäisyydet ovat näkyvissä ja
toisessa näkyy vain etäisyys mittaviivan alusta ensimmäiseen kohteeseen,
etäisyys siitä viimeisen kohteen vastakkaiselle reunalle sekä siitä
mittaviivan loppuun. Lopussa myös koko mittaviivan pituus.

Huomaa, että tässä "Älä huomioi ensimmäistä ja viimeistä" -asetus on pois päältä.

{: .figure-medium-row }
> ![Näytetään etäisyydet](../inkscape-mitta-kohteiden_etaisyydet-1.png)
> ![Ei näytetä etäisyyksiä](../inkscape-mitta-kohteiden_etaisyydet-2.png)

### Näytä piilotetut leikkauspisteet

{: .figure-normal }
![Näytä piilotetut leikkauspisteet -valinta](../inkscape-mitta-show_hidden_intersections.png)

Viimeisenä "päälle / pois" -valintana on *Näytä piilotetut leikkauspisteet*
("Show hidden intersections"), jonka kuvakkeena on suljettu silmä.
Tämä valinta vaikuttaa siihen, mitataanko myös mittajanan leikkauspisteet
sellaisten kuvioiden kanssa, jotka jäävät jonkin toisen piirto-objektin alle piiloon.
Leikkauspisteinä tarkastellaan siis mittajanan ja piirto-objektin reunan leikkauksia,
ei eri piirto-objektien välisiä leikkauksia.

Alla olevissa kuvissa on edellisen kohdan punaiset laatikot peitetty
osittain keltaisella suorakulmiolla ja näkyvissä on sama mittajana.
Kun "Näytä piilotetut leikkauspisteet" on päällä, leikkauspisteet huomioidaan mittauksessa
vaikka ne ovat keltaisen suorakulmion alla. Kun asetus on pois päältä,
vain näkyvissä olevat leikkauspisteet merkitään mittaukseen.

{: .figure-medium-row }
> ![Näytetään piilotetut leikkauspisteet: päällä](../inkscape-mitta-piilotetut_leikkauspisteet-1.png)
> ![Näytetään piilotetut leikkauspisteet: pois](../inkscape-mitta-piilotetut_leikkauspisteet-2.png)

## Toimintanapit

Asetuspalkissa on joukko toimintanappeja.

### Käännä mittaus

{: .figure-normal }
![Ennen kääntöä](../inkscape-mitta-reverse_measure.png)

*Käännä mittaus* ("Reverse measure") -nappi vaihtaa mittajanan suunnan.
Sen alkupää ja loppupää vaihtavat siis paikkaa ja samalla
kulman kärki vaihtuu janan päästä toiseen.

{: .figure-normal }
![Ennen kääntöä](../inkscape-mitta-kaanto-1.png)

{: .figure-normal }
![Käännön jälkeen](../inkscape-mitta-kaanto-2.png)

### Haamumittaus

{: .figure-normal }
![Haamumittauksen nappi](../inkscape-mitta-phantom_measure.png)

Toisinaan on tarve mitata useampaa kohtaa yhtä aikaa.
*Haamumittaus* ("Phantom measure") -toiminnolla, kameranapilla, viimeisimmästä
mittajanasta otetaan "kuva", joka jää piirtoalueelle näkyviin
samalla kun mittatyökalulla voi tehdä uuden mittauksen.

Alla olevassa kuvassa on mitattu keltaisen suorakulmion oikea pystysivu
ja otettu siitä kuva haamumittauksena. Sen jälkeen on aloitettu uusi
mittaus suorakulmion vasemmasta yläkulmasta.

{: .figure-normal }
![Haamumittaus](../inkscape-mitta-haamumittaus.png)

Haamumittauksen saa pois näkyvistä esimerkiksi vaihtamalla
välillä työkalun vaikka valintatyökaluksi.

### Apuviivoiksi

{: .figure-normal }
![Apuviivoiksi-nappi](../inkscape-mitta-apuviivoiksi.png)

Mittatyökalulla mitattuja asioita voidaan muuttaa apuviivoiksi
valitsemalla toiminta *Apuviivoiksi* ("To guides").

Tämä lisää piirtialueelle joukon uusia apuviivoja:
- Vaakasuorat apuviivat mittauksen alku- ja loppupisteeseen
- Pystysuorat apuviivat mittauksen alku- ja loppupisteeseen
- Mittaviivaa pitkin kulkevan apuviivan
- Mittaviivaa vastaan kohtisuorat apuviivat kuhunkin leikkauspisteeseen

Apuviivoilla saadaan siis aikaan ainakin mitatun matkan korkeus ja leveys
sekä tarttumapisteet jokaiseen leikkauspisteeseen.

{: .figure-normal }
![Mittauksesta luodut apuviivat](../inkscape-mitta-apuviivat.png)

### Muunna kohteeksi

{: .figure-normal }
![Muunna kohteeksi](../inkscape-mitta-convert_to_item.png)

Joskus mittaustiedot halutaan lisätä itse kuvaan. Tämä voidaan tehdä
*Muunna kohteeksi* ("Convert to item") -toiminnolla. Tämän
napin painaminen tekee mittajanasta ja sen näyttämistä mitoista
ryhmän piirto-objekteja, joita voidaan sen jälkeen käsitellä
muiden objektien tapaan.

{: .figure-medium-row }
> ![Mittajana muunnettuna piirto-objektien ryhmäksi](../inkscape-mitta-muunna_kohteeksi.png)
> ![Mittajanan kulma muunnettuna piirto-objektien ryhmäksi](../inkscape-mitta-muunna_kohteeksi_kulma.png)

Ryhmästä voi sitten käsin poistaa ylimääräiseksi katsomansa merkinnät.

### Merkitse mitat

{: .figure-normal }
![Merkitse mitat -nappi](../inkscape-mitta-mark_dimensions.png)

Toinen tapa merkitä kuvaan kohteen mittatyökalulla mitattu pituus on
*Merkitse mitat* ("Mark dimensions") -toiminto. Tämä toiminto 
yksinkertaisesti lisää mitatun janan viereen kaksipäisen nuolen ja
sen yläpuolelle janan pituuden mittatyökalussa käytettyinä mittayksikköinä.

Tämän toiminnon yhteydessä mittaustyökalun asetuspalkin "Siirtymä"-asetuksella
on merkitystä. Jos sen arvo on 0, kaksipäinen nuoli piirretään suoraan
mittajanan kohdalle. Kun arvoa kasvatetaan, nuoli ja mittateksti siirtyvät
lukuarvon verran alemmas.

Samoin asetuspalkissa valittu kirjasinkoko vaikuttaa tämän toiminnon luoman
mittatekstin kirjasimen suuruuteen ja skaalaus vaikuttaa tulostuvaan
mittauksen arvoon.

Huomioitavaa on myös, että sillä on merkitystä, mihin suuntaan mittajana
on piirretty. Jos mittateksti tulee ylösalaisin, voi toiminnon peruuttaa
(undo), vaihtaa mittauksen suunnan *käännä mittaus* -toiminnolla ja
merkitä mitat kuvaan uudelleen.

{: .figure-medium-row }
> ![Merkitse mitat: mittatyökalun kanssa](../inkscape-mitta-merkitse_mitat-1.png)
> ![Merkitse mitat: ilman mittatyökalua](../inkscape-mitta-merkitse_mitat-2.png)
> ![Merkitse mitat: suuremmalla "Siirtymä"-arvolla](../inkscape-mitta-merkitse_mitat-3.png)
> ![Merkitse mitat: yläsalaisin](../inkscape-mitta-merkitse_mitat-4.png)

Myös tällä tavalla luotuja piirto-objekteja voi luonnollisestikin mukata
luonnin jälkeen. Muuttaa värejä, viivojen paksuuksia, nuolenpäitä ja siirrellä.