---
date: "2026-01-31T11:20:00+03:00"
title: "Tasot"
layout: default
nav_order: 4
parent: Objektit
---

# Tasot

*Tasot* ovat toinen menetelmä objektien ryhmittelemiseen piirtämisen tai
kuvan näyttämisen kannalta loogisiksi kokonaisuuksiksi. Tasoja käytetään
useimmissa kuvankäsittelyohjelmissa riippumatta siitä, piirretäänkö niillä
vektorikuvia vai rasterikuvia.

Tasoilla objektit voidaan ryhmitellä kuin päällekkäin aseteltuina
kalvoina. Esimerkiksi metsämaisemaa esittävässä kuvassta voidaan
taimmaiselle tasolle sijoitella taivas, seuraavalle tasolle puut
ja etummaiselle tasolle eläimiä ja kasveja, kuten tässä [FreeSVG.org](https://freesvg.org)-sivuston
kuvista koostetussa kuvassa.

{: .figure-fulll }
[![Maisemakuva, jossa metsää, jänis, kettu, pensaita ja lintujen muuttoaura](../tasot-maisema.svg)](../tasot-maisema.svg)

Tasot ovat käytännöllisiä erityisesti muokkausvaiheessa, jolloin
tasoja voidaan lukita niin, että vain haluttu taso on muokattavissa.
Silloin vain muokattavalla tasolla olevat kohteet ovat valittavissa
eikä tule vahingossa siirreltyä vääriä kohteita.
Tasoja voidaan myös piilottaa näkyvistä, jolloin on helpompi keskittyä
juuri sillä hetkellä muokattaviin asioihin. Tasojen piilottaminen voi
myös helpottaa piirtämistä, jos kuvassa on niin paljon yksityiskohtia,
että sen käsittely käy tietokoneelle raskaaksi.

Tasot ovat käteviä myös esimerkiksi julisteiden suunnittelussa, jolloin
julisteen taustat, kuvat, otsikot ja tekstit voidaan jaotella omille
tasoilleen.

Tasoista on hyötyä myös, kun samaan piirrokseen piirretään useita
erilaisia näkymiä, jotka sitten viedään erillisiksi rasterikuviksi.
Esimerkiksi alimmaisella tasolla voi olla kuville yhteinen tausta
ja muilla tasoilla vaihtoehtoiset samalla taustalla esitettävät
asiat.

{: .figure-small-row }
> ![Lintukortti 1](../inkscape-tasot-lintukortti1.png)
> ![Lintukortti 2](../inkscape-tasot-lintukortti2.png)
> ![Lintukortti 3](../inkscape-tasot-lintukortti3.png)
> ![Lintukortti 4](../inkscape-tasot-lintukortti4.png)

Eri tasoilla voidaan pitää myös samasta projektista vaihtoehtoiset
toteutukset.

## Tasot ja objektit -dialogi

Tasoja voidaan hallita *Tasot ja Objektit* -dialogilla (Layers and Objects).
Dialogin saa esiin komentopalkin napilla, "Tasot"-valikosta taikka
*Shift-Ctrl-L*-pikanäppäimellä.

{: .figure-normal }
> ![Tasot ja objektit -nappi](../inkscape-tasot-ikoni.png)

Dialogi aukeaa muiden dialogien tapaan oikeaan reunaan telakoituna
ja sen voi halutessaan raahata irralliseksi ikkunaksi.

{: .figure-normal }
> ![Tasot ja objektit -dialogi](../inkscape-tasot-dialogi.png)

Dialogissa tasot ovat listassa päällekkäin siinä järjestyksessä
kuin ne ovat piirroksessa. Päällimmäinen ylimpänä.
Aktiivisena oleva taso on korostettuna.

Uusien tasojen lisääminen tapahtuu vasemman yläkulman plus-ikonilla,
joka oletuksena lisää uuden tason valittuna olevan tason yläpuolelle
ja käyttää tason oletusnimenä aiemman tason nimeä ja yhdellä kasvatettua
lukua. Tasot kannattaa nimetä järkevästi, jotta niiden käyttö on helppoa.

{: .figure-normal }
> ![Lisää uusi taso](../inkscape-tasot-lisaa.png)

Valitun tason voi poistaa roskakori-kuvakkeella. Ylös ja alas päin
olevat nuolet puolestaan siirtävät valittuna olevaa tasoa
pinossa ylemmäs ja alemmas. Tasojen järjestyksen vaihtamiseen voi
Tasot ja Objektit -dialogissa käyttää
myös pikanäppäimiä *Shift-Ctrl-nuoliylös* ja *Shift-Ctrl-nuolialas*, joilla valittu
taso siirtyy askeleen ylös ja alas vastaavasti.

Hieman epäloogisesti ohjelman kohdistuksen ollessa dialogin sijaan piirtoalueen
valitussa kohteessa saman tekevät pikanäppäimet *Shift-Ctrl-PageUp* ja *Shift-Ctrl-PageDown*.

Klikkaamalla tason nimeä hiiren oikealla napilla saa esiin kontekstivalikon,
josta voi valita useampia toimintoja, kuten tason monistamisen
ja tason muuttamisen ryhmäksi.

{: .figure-normal }
> ![Tason kontekstivalikko](../inkscape-tasot-kontekstivalikko.png)

Tästä valikosta valittuna tason lisääminen kysyy erikseen, lisätäänkö
uusi taso nykyisen ylä- vai alapuolelle taikka sen alitasoksi.

{: .figure-normal }
> ![Tason lisäysdialogi](../inkscape-tasot-lisaysdialogi.png)

Kun hiiren vie tason nimen päälle, kunkin tason oikeassa reunassa on kolme
kuvaketta, joilla voi määrätä tason *peittävyydestä*, *näkyvyydestä* ja *lukituksesta*.

{: .figure-normal }
> ![Tason lisäysdialogi](../inkscape-tasot-piilotus_lukitus.png)

Oikeanpuoleisin kuvake on lukko, joka on auki tai kiinni. Kiinni oleva
kuvake tarkoittaa, että taso on lukittu muokkaamiselta.

Oikealta toisena on kuvake, joka on avoin tai suljettu silmä. Kun
silmä on suljettuna, tämä tarkoittaa, että kyseinen taso on poissa
näkyvistä.

Kolmatta kuvaketta klikkaamalla tulee esiin valikko, jolla voi valita
kyseisen tason peittävyyden 0 ja 100 prosentin väliltä, sekä niin sanotun
*sekoitustila*, eli *Blend mode*.

{: .figure-normal }
> ![Tason peittävyys](../inkscape-tasot-peittävyys.png)

Sekoitustilalla tarkoitetaan tapaa, jolla valittu taso yhdistetään sen
alla oleviin tasoihin. Oletuksena oleva *Normal* tarkoittaa, että
taso esitetään alempien päällä normaaliin tapaan kuin läpinäkyvä
kalvo, johon on piirretty peittävä kuva.

Esimerkiksi *Darken* tarkoittaa, että tason objektit tekevät alla
olevaan kuvaan vain tummentavia vaikutuksia. *Lighten* puolestaan
tekee vain vaalentavia vaikutuksia. Näihin toiminnallisuuksiin
kannattaa tutustua kokeilemalla.

Alla esimerkkeinä sekoitustilat *darken*, *lighten*, *difference* ja *luminosity*.

{: .figure-medium-row }
> ![Darken](../inkscape-tasot-blend_darken.png)
> ![Lighten](../inkscape-tasot-blend_lighten.png)
> ![Difference](../inkscape-tasot-blend_difference.png)
> ![Luminosity](../inkscape-tasot-blend_luminosity.png)

## Objektit

Nimensä mukaisesti Tasot ja objektit -dialogi esittää tasojen lisäksi
myös piirroksessa olevat objektit.

Kun tason kohdalta klikkaa sen nimen edessä olevaa kolmiota, avautuu
puurakenteena esiin kaikki tason sisällä olevista objekteista ja niistä
muodostetuista ryhmistä muodostuva sisäkköinen hierarkia.

{: .figure-normal }
> ![Pupu-objekti puurakenteessa](../inkscape-tasot-objekti.png)

Piirroksesta kulloinkin valittu kohde näkyy korostettuna puurakenteessa.

{: .figure-normal }
> ![Pupun silmä puurakenteessa](../inkscape-tasot-objekti_ryhmassa.png)

Tasot ja Objektit -dialogin asetuksista, rataskuvakkeesta esiin tulevasta
valikosta, voi valita, näytetäänkö dialogin listassa tasot ja niiden objektit
vai pelkästään tasot. Valinta "Expand to display selection" tarkoittaa,
että puurakenne avataan aina niin, että piirroksesta valittu kohde
on näkyvissä. Esimerkiksi kohteen ollessa syvällä sisäkkäisessä
ryhmityksessä.

Valittuja kohteita voi siirtää tasojen välillä joko *Tasot*-valikon toiminnoilla
"Siirrä valinta yläpuolella olevalle tasolle" ja "Siirrä valnta alapuolella olevalle tasolle"
taikka pikanäppäimillä *Shift-PageUp* ja *Shift-PageDown*. Kohteita
siirrettäessä tasolta toiselle on huomattavaa, että siirtäminen onnistuu
tällä tavalla myös lukitulle tasolle.

{: .figure-normal }
> ![Tasot-valikko](../inkscape-tasot-valikko.png)
