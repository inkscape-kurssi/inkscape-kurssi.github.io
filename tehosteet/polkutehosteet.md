---
date: "2026-01-31T11:20:00+03:00"
title: "Polkutehosteet"
layout: default
nav_order: 1
parent: Tehosteet ja suotimet
---

# Polkutehosteet

Polkutehosteet muttavat polun ulkoasua. Tehoste voidaan
lisätä polulle "Polku"-valikosta kohdasta "Polkutehosteet...",
jonka pikanäppäin on *Ctrl-&*. Tehoste voidaan myös liittää
toisesta kohteesta kopioituna. Samasta valikosta löytyy
myös tehosteen poistaminen.

Aloitetaan yksinkertaisella esimerkillä. Valitaan tehostettavaksi
yksinkertainen neljän solmun polku.

{: .figure-medium }
![Nelikulmainen polku](../inkscape-polkutehosteet-polku.png)

Valitaan "Polkutehosteet...", jolloin aukeaa "Polkutehosteet"-dialogi.

{: .figure-normal }
![Polkutehosteet-dialogi](../inkscape-polkutehosteet-dialogi.png)

Polulle voi valita tehosteen pudotusvalikosta.

{: .figure-normal }
![Polkutehosteet-dialogin pudotusvalikko](../inkscape-polkutehosteet-dialogin_pudotusvalikko.png)

Valitaan tehosteeksi ensimmäisenä vaihtoehtona oleva "Corners", eli "Kulmat".

{: .figure-normal }
![Polku ja valitun "Kulmat"-tehosteen asetukset](../inkscape-polkutehosteet-kulmat.png)

Nyt polkuun on sovellettuna "Kulmat"-tehoste oletusasetuksilla, jotka eivä käytännössä tee vielä mitään.
Polkuun on ilmestynyt kunkin solmun lähelle pieni piste. Kahva, jolla tehosteen toimintaa
voidaan säätää. Tehdään muutokset kuitenkin tehosteen lomakkeesta. Lisätään parametrin
"Säde" arvoksi 10 pikseliä. Tämä pyöristää kaikkia kulmia niin, että niiden säteeksi tulee 10.

{: .figure-normal }
![Polku ja valitun "Kulmat"-tehosteen asetukset: Kulmien säde 10 px](../inkscape-polkutehosteet-kulmat-10.png)

Polun kunkin kulman pyöristystä voidaan lisäksi muokata käsin kahvoja hiirellä
raahaamalla.

{: .figure-normal }
![Polun kulmia on säädetty käsin solmukohtaisesti.](../inkscape-polkutehosteet-kulmat-epasymmetrinen.png)

Käytännössä Inkscape pitää tallessa alkuperäisen polun ja näyttää
käyttäjälle tehosteella muokatun version polusta. Jos tehoste poistetaan,
polku palautuu alkuperäiseen muotoonsa.

Kun Inkscape tallentaa kuvion SVG-tiedostoon, tallennetaan
näytettävä lopputulos standardin mukaisena polkuna, jonka myös
muut ohjelmat osaavat näyttää, sekä sen lisäksi alkuperäisenä
polkuna ja Inkscapen ymmärtämänä tehostemäärittelynä. Näin
kuva näkyy oikein kaikilla ohjelmilla ja Inkscape osaa jatkaa
muokkausta alkuperäisessä muodossa.

Tehosteita voi olla yhtä aikaa käytössä useampia ja ne sovelletaan
kohteeseen siinä järjestyksessä kuin ne ovat "Polkutehoste"-dialogissa.

Lisätään samalle polulle "Slice"-tehoste, joka jakaa polun kahteen osaan.

{: .figure-normal }
![Polussa yhtä aikaa sekä "kulmat"- että "slice"-tehoste](../inkscape-polkutehosteet-kulmat_ja_slice.png)

Jos tehosteiden järjestyksen vaihtaa raahaamalla tehosteen kohdalla olevasta kahvasta,
on lopputulos erilainen. Nyt polkuun sovelletaan ensin "slice"-tehoste ja vasta sen jälkeen
kulmat pyöristävä "kulmat"-tehoste.

{: .figure-normal }
![Polussa yhtä aikaa sekä "slice"- että "kulmat"-tehoste toisessa järjestyksessä](../inkscape-polkutehosteet-kulmat_ja_slice-2.png)

Kunkin tehosteen kohdalla olevilla hallintanapeilla voi kytkeä tehosteen päälle tai pois (silmä),
poistaa tehosteen (roskakori), monistaa, siirtää, litistää, asettaa oletukseksi, asettaa suosikiksi
sekä raahata toiseen kohtaan. Litistämisellä tarkoitetaan sitä, että tehosteiden luomat
muunnokset tehdään suoraan polkuun. Tämän jälkeen ei ole enää olemassa erikseen
alkuperäistä polkua ja siihen tehtyjä irrallisia tehosteita vaan vain muutettu polku.

Kokeillaan muutamaa muuta polkutehostetta. Tehosteita on niin monta,
että lukija voi kokeilla loppuja itse.

Piirretään Suomen lipun mittasuhteissa oleva sininen risti ja
alltoileva viiva.

{: .figure-normal }
![Siniristi Suomen lipun mittasuhteissa](../inkscape-polkutehosteet-siniristi_ja_polku.png)

Valitaan viiva ja lisätään sille "Pattern Along Path" -tehoste.

{: .figure-normal }
![Pattern Along Path -tehoste](../inkscape-polkutehosteet-pattern_along_path.png)

Seuraavaksi valitaan sininen risti, kopioidaan se (*Ctrl-C*) ja valitaan uudelleen
alltoviiva. Nyt voidaan tehosteen asetuksissa klikata
"Pattern source" -kohdassa leikepöydän kuvaa. Tämä liittää kopioidun ristin
"lähdekuvioksi", joka toistetaan polulla. Lopputuloksena on
aaltoviivan mukaisesti aaltoileva risti.

{: .figure-normal }
![Aaltoileva risti](../inkscape-polkutehosteet-aaltoileva_risti.png)

Jos sama toistetaan sekä suorakaiteelle että ristille ja valitaan
niille sopivat värit, saadaan tehtyä alkeellinen liehuva lippu.

{: .figure-normal }
![Liehuva Suomen lippu](../inkscape-polkutehosteet-liehuva_lippu.png)

Hieman paremman ja helpomman lopputuloksen saa aikaan käyttämällä
"Lattice Deformation" -tehostetta. Tämän voi kohdistaa kokonaiseen
polusta muodostettuun ryhmään, esimerkiksi lipun kuvaan.

{: .figure-normal }
![Lattice deformation -tehoste ja Suomen lippu](../inkscape-polkutehosteet-lattice_deformation.png)

Yllä olevassa kuvassa lipun muodostavaan kahden polun ryhmään on lisätty "Lattice Deformation" -tehoste.
("Hilavääristymä")
Kun työkaluksi vaihtaa solmutyökalun, tulee esiin 5×5 hila, jonka solmuja voi siirrellä
ja siten "vääristää" polun ulkoasua.

{: .figure-normal }
![Hilan pisteiden siirto](../inkscape-polkutehosteet-lattice_deformation-2.png)

Ja lopputulos:

{: .figure-normal }
![Toinen liehuva Suomen lippu](../inkscape-polkutehosteet-liehuva_lippu-2.png)

Kokeillaan vielä "Solmu"-, eli "Knot"-tehostetta.

Aloitetaan piirtämällä kaksi keskenään ristiin piirrettyä ellipsiä ja yhdistämällä
ne yhdeksi poluksi. Tämä voidaan tehdä esimerkiksi piirtämällä ensin yksi
pystysuuntainen ellipsi, monistamalla se ja kääntämällä 90 astetta. Sen jälkeen
yhdistämällä ne yhdeksi poluksi (*Ctrl-K*) ja lopuksi kääntämällä saatua kuviota
45 astetta. Lopputuloksena on seuraava kuvio:

{: .figure-normal }
![Kaksi ristiin piirrettyä ellipsiä](../inkscape-polkutehosteet-solmu-1.png)

Nyt valitaan polkutehosteeksi "Knot", eli "Solmu". Lopputuloksena
onkuvio, jossa jokaisen viivojen risteyksen kohdalla toinen viiva katkeaa
risteämisen ajaksi. Tehosteen asetuksista voi valita esimerkiksi
katkoksen pituuden.

{: .figure-normal }
![Kaksi ristiin piirrettyä ellipsiä](../inkscape-polkutehosteet-solmu-2.png)

Tehdään sama tehoste säännölliselle viisikulmiolle, jonka kulmille
on laitettu negatiivinen pyöristys.

{: .figure-medium-row }
> ![Viisikulmainen solmu ilman tehostetta](../inkscape-polkutehosteet-solmu-3.png)
> ![Viisikulmainen solmu tehosteen kanssa](../inkscape-polkutehosteet-solmu-4.png)

Ottamalla esiin solmutyökalun, voi vielä tarkemmin määritellä, mikä
viiva menee missäkin risteyksessä yli ja mikä ali. Solmutyökalun
ollessa aktiivinen yksi risteyksistä on merkitty "kiertonuolella",
joka symboloi viivojen järjestystä risteyksessä. Tiloja on kolme:
"vastapäivään" (yksi viiva päällä), "myötäpäivään" (toinen viiva päällä)
ja "ei kumpikaan" (molemmat viivat näkyvissä). Tila vaihtuu klikkaamalla
risteyskohdassa olevaa kahvaa. Kahvan voi raahata seuraavan
risteyskohdan päälle ja hallita sen risteämisjärjestystä.

{: .figure-medium-row }
> ![Vastapäivään](../inkscape-polkutehosteet-solmu_suunta-1.png)
> ![Myötäpäivään](../inkscape-polkutehosteet-solmu_suunta-2.png)
> ![Ei kumpikaan](../inkscape-polkutehosteet-solmu_suunta-3.png)
> ![Seuraava risteys](../inkscape-polkutehosteet-solmu_suunta-4.png)
