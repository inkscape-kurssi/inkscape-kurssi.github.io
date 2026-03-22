---
date: "2026-03-22T20:37:00+03:00"
title: "Polun koko"
layout: default
nav_order: 6
parent: Piirtotyökalut
---

# Polun koko

Polkuna piirretyn ääriviivan kokoa halutaan joskus *laajentaa*
tai *supistaa*. Tällä ei tarkoiteta objektin skaalaamista vaan
sen reunaviivojen siirtämistä ulommas tai sisemmäs saman
verran joka kohdassa. Tämä ei säilytä kuvion muotoa.

Alla on esimerkki alkuperäisestä kättä esittävästä kuvasta
sekä sama kuva laajennettuna ja supistettuna.

{: .figure-small-row }
> ![Punainen käsi](../inkscape-koko-kasi.png)
> ![Punainen käsi laajennettu](../inkscape-koko-kasi_laajennettu.png)
> ![Punainen käsi supistettu](../inkscape-koko-kasi_supistettu.png)

Kun nämä kuvat asetetaan päällekkäin eri värisinä, nähdään
ehkä vielä selvemmin, miten laajennus ja supistus ovat
muuttaneet polkua.

{: .figure-medium}
![Kolme eri kokoa päällekkäin](../inkscape-koko-kasi_koot.png)

Laajentaminen paisuttaa kuviota samalla pyöristäen muotoa.
Supistaminen puolestaan terävöittää muotoja. Molemmat hukkaavat
yksityiskohtia, mutta voivat soveltua varsinaisen kuvion korostamiseen.

## Supistaminen ja laajentaminen

Supistaminen ja laajentaminen löytyvät molemmat "Polku"-valikosta.

{: .figure-normal}
![Supistaminen ja laajentaminen valikossa](../inkscape-koko-valikko.png)

Supistamisen pikänäppäin on *Ctrl-(* ja laajentamisen *Ctrl-)*.
Suomalaisella näppäimistöllä nämä tarkoittavat käytännössä
*Ctrl-Shift-8* ja *Ctrl-Shift-9*.

Laajentamista voidaan käyttää tehokeinona esimerkiksi ääriviivojen
korostamiseksi.

{: .figure-normal}
![Mustavalkoinen kissa](../inkscape-koko-kissa-1.png)

Valitaan kuvasta kissan musta ääriviiva, monistetaan se ja
käytetään siihen "Laajenna"-toimintoa.

{: .figure-medium-row}
> ![Mustavalkoinen kissa mustalla laajennetulla ääriviivalla](../inkscape-koko-kissa-2.png)
> ![Mustavalkoinen kissa valkoisella reunalla](../inkscape-koko-kissa-3.png)

Toinen esimerkki laajentamisen käytöstä voisi olla esimerkiksi alla
olevan kartan tapaan etäisyyksiä esittävän tasa-arvokäyrästön
luominen.

{: .figure-normal}
![Kartta](../inkscape-koko-kartta.svg)


## Dynaaminen koko

Supistaminen ja laajentaminen muuttavat polun ääriviivaa 
askelittain. Jos ääriviivaa halutaan muuttaa portaattomasti,
voidaan käyttää *dynaaminen koko* -vaihtoehtoa. Sen pikanäppäin
on *Ctrl-J*.

Tämä toiminto lisää polkuun kahvan, jota siirtämällä polun koko
laajenee tai supistuu juuri sen verran kuin kahvaa on siirretty.

{: .figure-medium-row}
> ![Tähti](../inkscape-koko-tahti.png)
> ![Tähti ja dynaamisen koon kahva](../inkscape-koko-tahti_kahva.png)
> ![Tähti ja dynaaminen koon muuntaminen](../inkscape-koko-tahti_dynaaminen.png)

Sopivasti polkua monistamalla, pinoamalla ja laajentamalla tai supistamalla
saadaan aikaa korostuksia.

{: .figure-normal}
> ![Tähti ja useita eri kokoisia reunoja](../inkscape-koko-tahti_monistettu.png)

## Linkitetty koko

Tavallisen supistamisen ja laajentamisen sekä dynaamisen koon muuttamisen
heikkona puolena on se, että jos alkuperäistä polkua muutetaan,
siitä tehdyt laajennetut tai supistetut kopiot eivät enää vastaa alkuperäistä.
Jos muokattavuus on tarvittava ominaisuus, voidaan käyttää
toimintoa *linkitetty koko*, jonka pikanäppäin on *Ctrl-Alt-J*.

Tämä toiminto on hyödyllinen esimerkiksi, jos halutaan ympäröidä tekstiä
ääriviivoilla. Otetaan esimerkiksi seuraava lihavoitu "Inkscape"-teksti.

{: .figure-normal}
> ![Punainen teksti "Inkscape"](../inkscape-koko-inkscape.png)

Valitaan tekstiobjekti ja valitaan "Polku"-valikosta "Linkitetty koko".

Tämä luo alkuperäisestä objektista poluksi muunnetun kopion, jolla on
samanlainen kokoa muuttava kahva kuin "dynaaminen koko" -toiminnossa.
Uusi objekti on alkuperäisen alla.

{: .figure-normal}
> ![Punainen teksti "Inkscape" ja linkitetyn koon kahva](../inkscape-koko-linkitetty_koko.png)

Kun uuden objektin kokoa muutetaan ja täyttö- sekä reunaväri valitaan sopivasti,
saadaan tekstille aikaiseksi hieno kehystys.

{: .figure-normal}
> ![Punainen teksti "Inkscape" ja linkitetyn objektin laajennus](../inkscape-koko-linkitetty_laajennus.png)

Linkitetyn koon varsinainen etu on se, että luotu objekti on kytköksissä
alkuperäiseen objektiin ja alkuperäisen muokkaaminen vaikuttaa
myös linkitettyyn objektiin.

{: .figure-normal}
> ![Punainen teksti "Inkscape!" muokattu ja linkitetty laajennus seuraa](../inkscape-koko-linkitetty_muokattu.png)

Linkitettyä koon muokkausta voidaan toki tehdä myös muille objekteille kuin
vain tekstille, linkitettyjä objekteja voidaan luoda useampia ja niitä
voidaan siirrellä riippumatta alkuperäisestä objektista.

{: .figure-medium-row }
> ![](../inkscape-koko-linkitetty_tahti.png)
> ![](../inkscape-koko-linkitetty_tahti-muokattu.png)
> ![](../inkscape-koko-linkitetty_tahti-siirretty.png)

Linkitetyllä koolla tehtyjä linkitettyjä objekteja voi käyttää,
myös varjoefektin luomiseen. Nyt varjo muuttuu, kun tekstiä editoidaan.

{: .figure-normal}
> ![Punainen teksti "Inkscape" ja sille linkityksen avulla luotu varjo](../inkscape-koko-linkitys_varjo.png)
