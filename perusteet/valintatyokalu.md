---
date: "2025-12-13T22:01:00+03:00"
title: "Valintatyökalu"
layout: default
nav_order: 3
parent: Perusteet
---

# Valintatyökalu

{: .figure .figure-right }
![Valintatyökalun kuvake työkalupalkissa](../inkscape-valinta-kuvake.png)

Valintatyökalu on työkalupalkissa ylimpänä ja sitä symboloi nuolikuvake.
Työkalun voi valita myös näppäimistöllä *F1*- tai *s*-näppäintä painamalla.
Valintatyökalulla voi piirtoalueelta valita kohteita yhden tai useampia kerrallaan.
Valitulle kohteelle voi suorittaa erilaisia toimenpiteitä, kuten siirtämisiä,
skaalauksia, kiertoja ja peilauksia.

## Valinta

Kohteen voi valita valintatyökalulla klikkaamalla sitä hiirellä. Jos haluaa
valita yhtä aikaa useampia kohteita, voi ensimmäisen valinnan jälkeen pitää
*Shift*-näppäintä pohjassa ja klikata seuraavia kohteita. Näin klikatut kohteet
lisätään valintaan. Jos näin klikkaa jo valittua kohdetta uudelleen, se poistuu
valinnasta.

Valinta näkyy katkoviivoilla piirrettynä suorakaiteena kaikkien valittujen
kohteiden ympärillä sekä koko valinnan ympärille kulmiin ja reunoihin ilmaantuvina
*skaalauskahvoina*.

{: .figure-medium }
![Esimerkki valitusta kohteesta. Keltainen hymynaama.](../valinta.png)


Yhden tai useamman kohteen voi valita myös painamalla hiiren napin pohjaan
ja piirtämällä hiirellä raahaamalla suorakulmion. Kaikki sen sisään jääneet kohteet
tulevat mukaan valintaan.

{: .figure-large }
![Esimerkki kahdesta yhtä aikaa valitusta kohteesta. Keltainen ja punainen hymynaama.](../valinta-2.png)

## Siirtäminen

Valitun tai valittuja kohteita voi siirtää ottamalla niistä kiinni **hiirellä** ja
raahaamalla ne uuteen paikkaan. Jos raahattaessa pitää *Ctrl*-näppäintä pohjassa,
tapahtuu raahaaminen joko vaaka- tai pystysuoraan. Näin kohde on helppoa saada
pysymään samassa linjassa siirron aikana.

Valittuja kohteita voi siirtää myös käyttämällä näppäimistön **nuolinäppäimiä**.
Pelkästään nuolinäppäintä painamalla kohde siirtyy piirtoalueella noin kahden
pikselin suuruisen matkan valittuun suuntaan. (Tässä pikselillä tarkoitetaan
piirtoalueen koon mukaisia pikseleitä, ei näytön fyysisiä pikseleitä.)
Pitämällä *Shift*-näppäintä pohjassa nuolinäppäintä painettaessa siirrytty matka on pidempi,
eli 20 pikseliä. Vastaavasti, jos nuolinäppäintä painaessa pitää samalla *Alt*-näppäintä pohjassa,
kohde siirtyy normaalia pienemmän matkan, joka riippuu voimassa olevasta zoomauksesta.
Nuolinäppäimillä kohdetta saa siis siirrettyä tarkasti halutun määrän ja hienosäädettyä sijaintia.
Tämä on kätevää erityisesti silloin, kun siirtymä halutaan tehdä saman määrän verran
sekä pysty- että vaakasuunnassa.

## Skaalaaminen

Skaalaaminen tapahtuu ottamalla kiinni valinnan nurkissa tai reunoissa olevista
kaksipäisistä nuolista, *skaalauskahvoista*. Kahvasta vetämällä kohde venyy
(tai kutistuu) haluttuun suuntaan. Oletuksena kohteen mittasuhteet eivät säily
vaan sen muoto saattaa litistyä tai venyä pysty- tai vaakasuunnassa.

{: .figure-large }
![Keltainen hymynaama venytetty sivusuunnassa](../skaalaus.png)

Jos skaalattaessa pidetään samalla
pohjassa *Ctrl*-näppäintä, pysyvät kohteen mittasuhteet lukittuina.

Normaalisti skaalattaessa käytettyä skaalauskahvaa vastakkainen kahva pysyy paikallaan
ja skaalaus tapahtuu näiden kahden kahvan välissä. Jos kuitenkin samanaikaisesti
pidetään *Shift*-näppäintä pohjassa, pysyy valinnan keskipiste paikoillaan ja
skaalaaminen tapahtuu sen ympärillä.

## Kierto ja vääntö

Kiertoa varten valintaa pitää klikata hiirellä toistamiseen. Silloin skaalaamiseen
käytettävät kahvat muuttuvat *kiertokahvoiksi*. Jokainen valitun kohteen klikkaus vaihtaa
tilan skaalauksen ja kierron välillä. Nurkissa olevista kahvoista kiinni
ottamalla voi valintaa kiertää vapaasti mihin kulmaan haluaa. Kierron keskipisteenä
toimii valinnan keskellä oleva "risti-symboli". Jos kierron haluaa tehdä jonkin muun
pisteen ympäri, voi "risti-symbolin" siirtää hiirellä raahaamalla haluamaansa kohtaan.

Jos kiertäessä pitää *Ctrl*-näppäintä pohjassa, kierto tapahtuu portaittain 15 asteen loikilla.

{: .figure-medium }
![Punainen hymynaama kierretty myötäpäivään.](../kierto.png)

Jos kulman kahvojen sijaan ottaa kiinni valinnan sivujen kahvoista, saa niistä vetämällä
väännettyä kuvion vinoon.

{: .figure-medium }
![Punaista hymynaamaa väännetty vinoon kuin kursivoitu.](../vaanto.png)

## Värin ja reunan paksuuden valinta

Valinnan **täyttövärin** voi vaihtaa klikkaamalla ikkunan alareunan väripaletista
halutun värin. Jos klikatessa pitää *Shift*-näppäintä pohjassa, vaihtuu
valinnassa olevien kohteiden **reunan väri**. Värin sijasta voi valita myös
paletin alussa äärimmäisenä vasemmalla olevan ja ruksilla merkityn "**ei väriä**" -vaihtoehdon. Tällöin
valinnasta riippuen objektin täyttö tai reuna muuttuu läpinäkyväksi. Valitut värit
näkyvät ikkunan vasemmassa alakulmassa. Viivan värin vieressä olevaa numeroa
hiiren oikealla nappulalla painamaa klikkaamalla esiin tulevasta valikosta voi
valita reunaviivalle paksuuden.

{: .figure-large }
![Inkscape-ikkunan vasen alakulma](../varit_ja_paksuus.png)


## Objektien pinoaminen

Piirtoalueella olevat objektit ovat aina syvyyssuunnassa jossain järjestyksessä päällekkäin.
Jos objektit ovat piirtoalueella samassa kohdassa, päällä olevat siis peittävät alla olevia
osittain tai kokonaan.

{: .figure-medium }
> ![Hymynaama, reiällinen ympyrä ja kolmio päällekkäin tässä järjestyksessä.](../pinoaminen_1.png)
> ![Kolmio päällimmäisenä ja hymynaama ja ympyrä sen alla.](../pinoaminen_2.png)

Kun objekti on valittuna, voi sen syvyyssuuntaista sijaintia tässä objektien pinossa muuttaa
valintatyökalun asetuspalkin järjestelynapeilla taikka vastaavilla "Kohde"-valikosta löytyvillä
toiminnoilla.

{: .figure-normal }
![Järjestelykuvakkeet: Nosto ylimmäksi, nosto ylös, lasku alas, lasku alimmaksi](../inkscape_jarjestyskuvakkeet.png)

Toiminnoille on olemassa myös kätevät näppäintoiminnot, joiden osaaminen sujuvoittaa ja nopeuttaa
työskentelyä. Valittun objektin voi näillä toiminnoilla siirtää päällimmäiseksi (*Home*), nostaa yhden
askeleen ylemmäs (*Page up*), laskea yhden askeleen alemmas (*Page Down*) ja
siirtää alimmaiseksi (*End*).

## Valintatyökalun asetukset

Valintatyökalun työkalukohtaisissa asetuksissa on joukko käyttöä helpottavia nappeja ja valintoja.

{: .figure-full }
![Valintatyökalun asetuspalkki](../inkscape_valinta-asetukset.png)

Ensimmäinen ryhmä nappeja on joukko pikavalintoja kaikkien piirtoalueella olevien objektien valitsemiseen
tai valinnan poistamiseen. Seuraavassa ryhmässä ovat pikavalinnat 90 asteen kierrolle vasta- ja myötäpäivään
sekä peilauksille pysty- ja vaaka-akselin suhteen. Kolmantena ryhmänä ovat napit, joilla valittua
piirtokohdetta saa siirrettyä objektien pinossa päällimmäiseksi, alimmaiseksi sekä ylös ja alas.

Täytettäviin numerokenttiin on mahdollista suoraan lukuarvot kirjoittamalla siirtää valittu kohde
x- ja y-suunnassa haluttuun kohtaan. Piirtoalueen origo on (oletuksena) vasemmassa yläkulmassa,
koordinaatit kasvavat oikealle ja alas. Syötetty koordinaatti tarkoittaa valitun kohteen vasemman yläkulman
sijaintia suhteessa origoon. Yksiköksi on valittavissa pudotusvalikosta fyysisen
maailman mittayksiköitä, kuten mm, cm tai tuumat, digitaalisia ja painoalan yksiköitä,
kuten [pikselit] (px), [point] (pt) ja [pica] (pc), sekä prosenttiosuus piirtoalueen koon suhteen.

Samoin kohteen leveys ja korkeus ovat myös syötettävissä lukuarvoina. Leveyden ja korkeuden
kenttien välissä oleva **lukkosymboli** kuvaa kohteen mittasuhteiden lukitsemista. Jos lukko on
kiinni, leveyden tai korkeuden muuttaminen muuttaa myös toista samassa suhteessa niin, että
kuvaobjektin mittasuhteet säilyvät.

Asetuspalkin viimeisenä olevat neljä päällä/pois -valintanappia ovat tärkeitä. Niillä
hallitaan sitä, miten piirrosobjektien reunaviivat, kulmien pyöristykset, liukuvärit sekä
täyttökuviot käyttäytyvät, kun objektia skaalataan. Kun kukin näistä on päällä,
vastaavat ominaisuudet säilyvät skaalauksen yhteydessä suhteessa koko objektiin.

Esimerkiksi, jos kuviolla on 2 pikseliä paksu reunaviiva ja se skaalataan mittasuhteiltaan
kaksinkertaiseksi, niin jos reunaviivan suhteet säilyttävä valinta on päällä, myös
reunaviiva skaalautuu kaksinkertaiseksi, eli 4 pikseliä paksuksi. Jos taas asetus ei ole päällä,
reunaviiva pysyy kahdessa pikselissä ja siis pienenee suhteessa muuhun kuvioon.

Oletuksena nämä kaikki neljä asetusta ovat päällä, jolloin skaalaus pitää kuvion täsmälleen saman näköisen,
mutta niiden toiminnasta on hyvä olla tietoinen siltä varalta, että niitä sattuu tarvitsemaan.


{: .exercises }
> Lataa alla oleva SVG-tiedosto (hiiren oikealla napilla "Tallenna kohde levylle")
> ja avaa se Inkscapella. Tiedosto sisältää harjoitustehtäviä, joilla harjoitellaan
> valintatyökalun käyttöä.
> 
> [Harjoitus 2 - Valintatyökalu](/files/harjoitus-02-valinta.svg)
>
> [Harjoitus 3 - Valintatyökalu - Edistyneet](/files/harjoitus-03-valinta_edistynyt.svg)


[pikselit]: https://en.wikipedia.org/wiki/Pixel
[point]: https://en.wikipedia.org/wiki/Point_(typography)
[pica]: https://en.wikipedia.org/wiki/Pica_(typography)