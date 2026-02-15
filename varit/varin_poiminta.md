---
date: "2026-01-31T11:20:00+03:00"
title: "Värin poiminta"
layout: default
nav_order: 3
parent: Värityökalut
---

# Värin poiminta

{: .figure .figure-right }
![Värinpoimintatyökalun kuvake työkalupalkissa](../inkscape-dropper-ikoni.png)

Joskus on tarve poimia kohteelle väri jostain toisesta kohdasta piirustusta.
Tähän sopiva työkalu on *värinpoimintatyökalu* eli *dropper*.
Työkalupalkissa tälle on pipetin näköinen kuvake ja pikanäppäiminä *D* sekä *F7*.

Työkalun käyttö on helppoa. Kohde, jonka väri halutaan muuttaa, on valittuna
ja pomintatyökalulla klikataan piirroksesta sitä kohtaa, jonka väri halutaan
ottaa käyttöön. Jos kohtaa klikataan hiiren napilla, väri tulee valittuna olevan
kohteen täyttöväriksi. Jos taas hiirellä klikataan *Shift*-näppäin pohjassa,
väri tulee valitun kohteen reunaväriksi.

Alla olevissa kuvissa ensimmäisessä hiiri on valittavan värin päällä ennen
klikkaamista. Toisessa hiirellä on klikattu ja väri on poimittu valitun
kohteen, eli tähden täyttöväriksi. Kolmannessa kuvassa on klikattu vihreää
aluetta *Shift* pohjassa ja väri on tullut tähden reunaväriksi.

{: .figure-medium-row }
> ![Hiiri valittavan värin päällä](../inkscape-dropper-valinta-1.png)
> ![Väriä klikattu hiiren napilla ja väri tullut kohteen täytöksi](../inkscape-dropper-valinta-2.png)
> ![Väriä klikattu hiiren napilla Shift pohjassa ja väri tullut kohteen reunaväriksi](../inkscape-dropper-valinta-3.png)

Poimintatyökalu on helppo käyttää ja siinä on hyvin vähän asetuksia.

{: .figure-normal }
> ![Poimintatyökalun asetukset](../inkscape-dropper-asetukset.png)

Ainoat asetukset koskevat peittävyyden käsittelyä, jota varten on
kaksi "päällä / pois" -nappia.

Ensimmäinen, "valitse", tarkoittaa, että jos se on valittuna,
poimintatyökalu huomioi klikattavassa kohdassa olevan peittävyyden
ja poimii myös peittävyystiedon.

Toinen valinta, "käytä", tarkoittaa, että peittävyystietoa myös käytetään
kohteeseen.

Parhaiten toiminta käy ilmi esimerkeillä.

Alla olevissa kuvissa päällä ovat sekä "valitse" että "käytä".
Kun poimintatyökalulla klikataan osittain läpinäkyvää viininpunaista,
tähden väriksi tulee viininpunainen, jossa on sama peittävyys.
Eli poimittiin sekä väri että sen peittävyys ja peittävyyttä
käytettiin. Väripalkeista näkyy valittu väri ja peittävyyden aste.

{: .figure-medium-row }
> ![](../inkscape-dropper-valinta_kayta.png)
> ![](../inkscape-dropper-valinta_kayta-vari.png)

Toisena esimerkkinä tilanne, jossa on valittuna vain "valitse",
mutta ei "käytä"-asetusta.

Nyt valintaan on otettu sekä viininpunainen väri että sen peittävyys,
mutta peittävyystietoa ei ole käytetty vaan se on laitettu 100 prosenttiin.

{: .figure-medium-row }
> ![](../inkscape-dropper-valitse.png)
> ![](../inkscape-dropper-valitse-vari.png)

Kolmantena esimerkkinä on tilanne, jossa sekä "valitse" että "käytä" ovat
pois päältä. ("Käytä" ei edes voi olla päällä, jos "valitse" ei ole päällä.)

Tässä tilanteessa väriä poimittaessa ei ole huomioitu peittävyyttä ollenkaan
vaan on vain poimittu se väri, joka piirtoalueella näkyy. Eli marjapuuron
punainen, joka on seurausta viininpunaisesta, jonka läpi kuultaa taustan valkoinen.
Peittävyys on tässäkin tilanteessa 100 prosenttia.

{: .figure-medium-row }
> ![](../inkscape-dropper-ei_valitse.png)
> ![](../inkscape-dropper-ei_valitse-vari.png)

Otetaan vielä neljäs esimerkki, jossa "valitse" ja "käytä" ovat molemmat
päällä, mutta läpikuultavan kohteen alla ei olekaan tyhjää taustaa
vaan toinen läpinäkymätön kohde. Tässä tapauksessa poimittu väri
on läpikuultavan viininpunaisen ja peittävän yhteisvaikutus ja
peittävyys on niiden yhdessä aikaan saama peittävyys, eli 100 prosenttia.

Tällaisessa tilanteessa, jossa yhteisvaikutus on kokonaan peittävä,
ei valintojen asetuksella ole lopputulokseen vaikutusta.

{: .figure-medium-row }
> ![](../inkscape-dropper-valitse_kayta_tausta.png)
> ![](../inkscape-dropper-valitse_kayta_tausta-vari.png)
