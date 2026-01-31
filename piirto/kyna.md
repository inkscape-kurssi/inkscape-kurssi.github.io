---
date: "2026-01-31T11:20:00+03:00"
title: "Kynätyökalu"
layout: default
nav_order: 3
parent: Piirtotyökalut
---

# Kynätyökalu

{: .figure .figure-right }
![Kynätyökalun kuvake työkalupalkissa](../inkscape-kyna-ikoni.png)

*Kynätyökalu* eli *vapaa piirto* on työkalun polkujen piirtämiseen
vapaalla kädellä hiirellä, kosketusnäytöllä tai tietokoneeseen liitetyllä
piirtopöydällä. Työkalun voi valita työkalupalkista tai pikanäppäimellä
*p*.

## Piirtäminen

Hiirellä piirtäminen aloitetaan painamalla hiiren nappi pohjaan jossain
kohtaa piirtoalueella, liikuttamalla hiirtä haluttu reitti ja vapauttamalla
nappi.

Työkalu luo piirretystä reitistä uuden polkuobjektin, jonka varrelle tulee
useita solmuja.

Alla olevista kuvista näkyy, miltä piirtäminen näyttää, minkälainen on
lopputulos ja miltä piirretty polku näyttää solmutyökalulla tarkasteltuna.

{: .figure-medium-row }
> ![Kynällä piirtäminen](../inkscape-kyna-piirtaminen.png)
> ![Kynällä piirretty viiva](../inkscape-kyna-piirto_valmis.png)
> ![Viiva tarkasteltuna solmuina](../inkscape-kyna-solmuina.png)
> ![Jälki täytöllä](../inkscape-kyna-taytolla.png)

Yleensä piirto tapahtuu viimeisimmäksi käytössä olleilla reunan ja täytön
asetuksilla. Jos käytössä on ollut musta reunaviiva ja ei täyttöä, saadaan
musta viiva. Jos taas käytössä on ollut täyttöväri, tulee lopputulokseenkin
täyttö. Nämä voi luonnollisesti muuttaa piirtämisen jälkeen. Väritykset
voi myös valita ennen piirtämistä, kunhan mikään aiempi kohde ei ole
valintahetkellä valittuna.

Samoin kuin viivatyökalulla, valittuna olevaa polkua voi kynällä jatkaa
aloittamalla piirtäminen polun päässä olevasta solmusta.

{: .figure-normal }
![Polun jatkaminen](../inkscape-kyna-jatkaminen.png)

Huomattavaa kynätyökalussa on, että se piirtää reunaviivaa, eli
tasaisella paksuudella olevaa kynän jälkeä.

## Piirtojäljen siloittaminen

Vapaalla kädellä piirretty jälki on helposti vähän vapisevan näköistä
ja polkuun tulee hyvin paljon solmuja. Jos polusta haluaa sileämmän
tai haluaa siihen vähemmin solmuja, voi "Polku"-valikosta valita
toiminnon **"Pelkistä"** tai valita saman toiminnon pikanäppäimellä *Ctrl-L*.

{: .figure-normal }
![Polku-valikon "Pelkistä"](../inkscape-kyna-pelkista.png)

Tämä toiminto yksinkertaistaa polkua poistamalla siitä ylimääräisiä
solmuja. Polku muuttuu hieman, mutta se pyritään pitämään muodoltaan
mahdollisimman samanlaisena.

Alla olevissa kuvissa alkuperäinen kynällä piirretty polku, saman
polun solmut näkyvissä, pelkistetyn polun solmut sekä lopputuloksena
oleva polku ilman, että solmut näkyvät.

{: .figure-medium-row }
> ![Alkuperäinen polku](../inkscape-kyna-pelkista-1.png)
> ![Alkuperäisen polun solmut](../inkscape-kyna-pelkista-2.png)
> ![Pelkistetyn polun solmut](../inkscape-kyna-pelkista-3.png)
> ![Pelkistetty polku](../inkscape-kyna-pelkista-4.png)

Lopputulos on säilyttänyt hyvin alkuperäisen muodon, mutta siitä
on poistunut alkuperäisen "ryppyisyys".

Pelkistystä voi käyttää samaan polkuun myös useasti, jolloin
kuvio alkaa väistämättä muuttua.

## Asetukset

{: .figure-full }
![Kynän asetuspalkki](../inkscape-kyna-asetuspalkki.png)

Kynän asetuspalkista löytyy muutamia käytettäviä asetuksia.
Ensimmäisenä palkissa on valittavissa piirrettävän polun
tyyppi. Nämä ovat jo viivatyökalusta tutut
*bezier-käyrä*, *spiro-polku* ja *spline-polku*. Näistä
kaksi jälkimmäistä tekee tavallista bezier-käyrää
pehmeämpää jälkeä vähemmillä solmuilla.

Neljäs nappi, "Flatten Spiro or SPline LPE", on toiminto,
joka muuntaa spiro- ja spline-polut saman muotoisiksi
tavallisiksi bezier-käyriksi.

Viidentenä nappina on "päälle / pois" -nappi, jolla voi valita
käytettäväksi piirtopöydän paineentunnistusta. Kun tämä kytketään päälle,
valittavaksi tule lisäksi lukuarvoiset minimi ja maksimi paineen
vaikutukselle ja polun päiden muodon valinta.

{: .figure-normal }
![Kynän paineentunnistus päällä](../inkscape-kyna-pressure_sensitive.png)

Paineen tunnistusta käytettäessä kynällä enemmän painettaessa
piirtojälki on paksumpi ja kevyemmin piirrettäessä viivasta tulee ohuempi.

{: .figure-medium-row }
> ![Piirtäminen kynällä paineentunnistuksen kanssa](../inkscape-kyna-pressure-1.png)
> ![Paineentunnistuksella piirretty polku](../inkscape-kyna-pressure-2.png)
> ![Paineentunnistuksella piirretty polku solmuina](../inkscape-kyna-pressure-3.png)

Kuvista näkyy, miten piirtojälki on edelleen polun reunaviiva.
Viivan paksuuden vaihtelu toteutetaan Inkscapessa teknisesti
polun efekteinä.

Asetuksissa lukuarvoinen "Tasoitus" tarkoittaa, miten sileää jälkeä
kynällä pyritään bezier-käyrästä tekemään. Tämän lukuarvon 
mukaisesti piirtojäljelle tehdään valmiiksi edellä kuvailtua pelkistystä.
Jos lukuarvo on pieni, pelkistystä tehdään vähän, eli polulle tulee
paljon sulmuja. Mitä suurempi lukuarvo on, sitä enemmän pelkistystä
tehdään ja sitä vähemmän polulle tulee solmuja.

Alla olevassa kuvassa ylempi viiva on piirretty tasoituksen
arvolla 15 ja alempi arvolla 60.

{: .figure-normal }
![Kynän paineentunnistus päällä](../inkscape-kyna-tasoitus.png)

Viimeiset asetukset, "Shape" ja "Scale", ovat samat kuin [viiva](../viivat/)-työkalussa.