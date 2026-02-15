---
date: "2026-01-31T11:20:00+03:00"
title: "Ryhmittely"
layout: default
nav_order: 3
parent: Objektit
---

# Ryhmittely

Vektoripiirrokset koostuvat suorakulmioista, ellipseistä,
kaarista, poluista, teksteistä ja muista alkeisobjekteista.
Monimutkaisemmat piirrokset muodostuvat kuitenkin alkeisobjekteista
koostetuista kompleksisemmista objekteista, joita pitää
voida siirrellä, käännellä ja skaalailla suurempina kokonaisuuksina.
Tätä varten objekteja on mahdollista *ryhmitellä* uusiksi objekteiksi.

Ryhmän luonti tapahtuu valitsemalla ryhmäksi liitettävät kohteet ja
valitsemalla valikosta "Kohde" ja "Ryhmitä" taikka painamalla
komentopalkin kuvaketta "Ryhmitä". Pikanäppäin ryhmän luomiselle
on *Ctrl-G*. Ryhmän purkaminen tapahtuu samoin valikosta "Kohde" ja
"Pura ryhmitys" tai komentopalkin napilla taikka pikanäppäimellä
*Shift-Ctrl-G*.

{: .figure-normal }
![Napit "ryhmitä" ja "pura ryhmitys"](../inkscape-ryhmittely-ikonit.png)

Piirretään esimerkkinä kissan kasvot. Kissan silmä voidaan koostaa
kolmesta ellipsistä

{: .figure-medium }
![Kissan silmä ellipseistä](../inkscape-ryhmittely-silman_osat.png)

Valitaan nämä kolme ellipsiä ja tehdään niistä ryhmä painamalla
pikanäppäintä *Ctrl-G*.

{: .figure-medium }
![Kissan silmä ellipseistä koostettuna ryhmänä](../inkscape-ryhmittely-silma_ryhma.png)

Nyt silmä on yksi ryhmä-objekti, joka sisältää kolme aliobjektia. Kun silmä on valittuna,
myös tilateksti kertoo tämän.

{: .figure-normal }
![Tilatekstinä: "Group of 3 objects in Taso1.](../inkscape-ryhmittely-vihjepalkki.png)

Nyt silmästä voidaan tehdä kopio, koska kissa tarvitsee kaksi silmää.
Painetaan pikanäppäintä *Ctrl-D* ja siirretään monistettu silmä nuolinäppäimillä
paikalleen.

{: .figure-medium }
![Kissan toinen silmä paikalleen](../inkscape-ryhmittely-toinen_silma.png)

Seuraavaksi halutaan varmistaa, että kuvassa kissan silmät ovat symmetrisesti
samalla etäisyydellä nenästä. Siihen voidaan käyttää tasausdialogia, mutta
sitä ennen yhdistetään molemmat silmät uudeksi ryhmäksi.

Valitaan molemmat silmät ja painetaan taas *Ctrl-G*.

{: .figure-medium-row }
> ![Kaksi silmää valittuina](../inkscape-ryhmittely-kaksi_silmaa_valittuina.png)
> ![Kaksi silmää ryhmänä](../inkscape-ryhmittely-kaksi_silmaa_ryhmana.png)

Nyt silmät muodostavat yhdessä yhden objektin, jonka voimme
tasaustyökalulla keskittää symmetrisesti keskelle kissan päätä.
Valitaan kahden silmän ryhmän lisäksi kissan päätä esittävä musta polku.

{: .figure-medium }
![Kaksi silmää ja pää valittuina](../inkscape-ryhmittely-silmat_ja_paa.png)

Koska pää on viimeiseksi valittu objekti, valitaan tasausdialogista
tasaus suhteessa *Viimeksi valittuun* ja toimintona *keskitä*.

{: .figure-medium }
![Tasataan silmäpari keskelle naamaa](../inkscape-ryhmittely-tasaus_keskelle.png)

Lopputuloksena silmät ovat varmasti symmetrisesti.

{: .figure-medium }
![Kaksi silmää ja pää valittuina](../inkscape-ryhmittely-silmat_ja_paa_tasattu.png)

Tässä vaiheessa voidaan purkaa silmien ryhmittely yhteen, koska sitä tarvittiin
vain tasaukseen. Valitaan kaksi silmää sisältävä objekti ja
painetaan *Shift-Ctrl-G*.

Viimeistellään silmät siirtämällä molemmat silmät pinojärjestyksessä vähän
taaemmaksi harmaiden poskien alle pikanäppäimellä *PageDown*.

{: .figure-medium }
![Silmät taaemmaksi pinojärjestyksessä.](../inkscape-ryhmittely-silmien_viimeistely.png)

Lopuksi tehdää korvalle sama kuin tehtiin silmille.
Ensin ryhmitetään kahdesta kaarevasta kolmiosta muodostuva korva yhdeksi
ryhmäobjektiksi.

{: .figure-medium-row }
> ![Korvan kaksi polkuobjektia](../inkscape-ryhmittely-korvan_polut.png)
> ![Korva ryhmä-objektina](../inkscape-ryhmittely-korva_ryhmana.png)

Sen jälkeen kopioidaan, peilataan pystyakselin suhteen, siirretään jonkin matkaa vasemmalle,
ryhmitetään korvat, keskitetään pään suhteen ja puretaan korvien ryhmä.

{: .figure-medium-row }
> ![Kissan korva kopioituna ja peilattuna pystyakselin suhteen](../inkscape-ryhmittely-korvan_peilaus.png)
> ![Kissankorva siirrettynä toiselle puolelle päätä](../inkscape-ryhmittely-korvan_siirto.png)
> ![Kaksi korvaa ryhmiteltyinä yhteen](../inkscape-ryhmittely-korvat_ryhmaksi.png)
> ![Korvaryhmä ja pää valittuina](../inkscape-ryhmittely-korvat_ja_paa.png)

Aivan viimeisenä askeleena valitaan vielä kaikki kissan osat ja ryhmitellään
niistä yksi kissa-objekti.

{: .figure-medium-row }
> ![Kaikki kissan osat valittuina](../inkscape-ryhmittely-kaikki_kissan_osat.png)
> ![Valmis kissa](../inkscape-ryhmittely-kissa_valmis.png)


Lopullinen valmis kissa svg-muotoisena kuvana!

{: .figure-full }
![Kissan kasvot](../kissa.svg)
