---
date: "2026-01-31T11:20:00+03:00"
title: "Täyttötyökalu"
layout: default
nav_order: 4
parent: Värityökalut
---

# Täyttötyökalu

{: .figure .figure-right }
![Täyttötyökalun kuvake työkalupalkissa](../inkscape-taytto-ikoni.png)

*Täyttötyökalu* täyttää valittuna värillä yhtenäisiä sujettuja alueita.
Sen pikanäppäin on *u*.

Täyttötyökalu tekee vastaavan kuin rasteripiirto-ohjelmien täyttötyökalu.
Kun sillä klikataan jotain kohtaa piirtoalueesta, haetaan klikkauskohdan
ympäriltä suurin mahdollinen yhtenäinen samaa väriä oleva alue ja
täytetään se valitulla värillä. Ero rasteripiirto-ohjelmien täyttötyökaluun
on siinä, että tämä työkalu ei muuta kuvassa jo olevia kohteita vaan luo
uuden polun, jonka muoto vastaa täytettävää aluetta ja jonka värinä
on käytössä oleva väri. Alla esimerkki, jossa täyttötyökalulla
klikataan punaista aluetta. Kolmannessa kuvassa uutta polkua on
siirretty vähän, jotta sen muoto tulee esiin.

{: .figure-medium-row }
> ![](../inkscape-taytto-kaytto-1.png)
> ![](../inkscape-taytto-kaytto-2.png)
> ![](../inkscape-taytto-kaytto-3.png)

Jos jokin objekti on valittuna, kun täyttötyökalua käytetään,
voidaan *Shift*-näppäintä klikkauksen aikana pohjassa pitämällä
lisätä täytettävä polku valittuun kohteeseen.

{: .figure-full }
> ![Poimintatyökalun asetukset](../inkscape-taytto-asetuspalkki.png)

Esimerkki:

{: .figure-medium-row }
> ![](../inkscape-taytto-kolmio_valittuna.png)
> ![](../inkscape-taytto-klikataan_punaista_vaihdolla.png)

## Asetukset

Täyttötyökalun asetuspalkissa on valittavissa asetukset, joilla
määritetään värin "samuuden" tarkkuus, luotavan uuden polun koko
sekä "välien sulkemista".

{: .figure-full }
> ![Poimintatyökalun asetukset](../inkscape-taytto-asetuspalkki.png)

Ensimmäisenä on pudotusvalikko *"Täytä"*, jolla valitaan, millä tavalla
värien samuus tunnistetaan kuvasta. Oletuksena on valinta "Näkyvät värit",
joka tarkoittaa tavallista tapaa tunnistaa värit samaksi.

Seuraavina vaihtoehtoina ovat "Punainen", "Sininen" ja "Vihreä". 
{: .figure-normal }
> ![Täytön värin tunnistuksen pudotusvalikko](../inkscape-taytto-tayta_pudotusvalikko.png)

Nämä viittaavat värin esitykseen RGB-muodossa, eli punaisena, sinisenä ja vihreänä
komponenttina. Jos täytön menetelmäksi on valittu esimerkiksi "Punainen",
silloin värit katsotaan samoiksi, jos niiden punainen komponentti on sama.

Alla olevissa kuvissa on esimerkki tästä. Kuvan kirkkaan punaisen
ja keltaisen sävyn punaiset komponentit ovat yhtä suuret ja siksi
täyttötyökalun luoma uusi polku peittää molemmat värit.

{: .figure-medium-row }
> ![Punainen nelikulmio ja sen väriasetukset RGB:nä.](../inkscape-taytto-punavari-1.png)
> ![Keltainen ellipsi ja sen väriasetukset RGB:nä.](../inkscape-taytto-punavari-2.png)
> ![Klikkaus täyttötyökalulla punaisen päällä.](../inkscape-taytto-punavari-3.png)
> ![Punainen nelikulmio ja keltainen ellipsi täytetty.](../inkscape-taytto-punavari-4.png)

Sininen ja vihreä väri toimivat samalla tavalla. Valinnat "Sävy",
"Värikylläisyys" ja "Kirkkaus" puolestaan viittaavat värin
HSL-muotoiseen esitykseen ja "Alfa" värin läpinäkyvyyteen.

{: .figure-normal }
> ![Lukuarvoinen asetuskenttä: Raja-arvo](../inkscape-taytto-raja-arvo.png)

Seuraavana asetuksissa oleva lukuarvoinen kenttä *"Raja-arvo"* tarkoittaa
sitä, minkä verran värit voivat heittää klikatun kohdan väristä
niin, että se vielä tulkitaan riittävän samanlaiseksi. Pieni arvo tarkoittaa,
että värin on oltava hyvin lähellä samaa tai täsmälleen sama. Suuremmalla
lukuarvolla riittää, että värit ovat lähes samat.

Alla olevissa kuvissa raja-arvon lukuarvona on 25 ja se riittää
näiden kahden punaisen sävyn samaistamiseen.

{: .figure-medium-row }
> ![Kaksi eri punaisen sävyä.](../inkscape-taytto-raja-arvo-1.png)
> ![Molemmat punaisen sävyt täytetty.](../inkscape-taytto-raja-arvo-2.png)

Seuraavana on lukuarvoinen kenttä *"Kasvata tai kutista"* ja sen yksikkö. Tällä valitaan,
minkä verran täyttömaali "vuotaa" yli rajan. Oletuksena arvo on 0,
jolloin täyttönä luotu polku seuraa alkuperäisten kohteiden rajoja.

{: .figure-normal }
> ![Lukuarvoinen asetuskenttä: Kasvata tai kutista](../inkscape-taytto-kasvata_tai_kutista.png)

Jos lukuarvo on suurempi kuin nolla, luotu polku kasvaa valitun mitan verran kohteiden rajojen yli.
Jos taas lukuarvo on nollaa pienempi, uusi polku pysyy saman verran kohteiden reunojen sisällä.

Alla esimerkit näistä kasvatuksen arvoilla 0, 20px ja -20px.

{: .figure-medium-row }
> ![Täyttö kasvatuksen arvolla 0](../inkscape-taytto-kasvata-0.png)
> ![Täyttö kasvatuksen arvolla 20](../inkscape-taytto-kasvata-20.png)
> ![Täyttö kasvatuksen arvolla -20](../inkscape-taytto-kasvata--20.png)

Viimeisenä asetuksena on pudotusvalikko *"Sulje välit"*.

{: .figure-normal }
> ![Asetus "sulje välit"](../inkscape-taytto-sulje_valit.png)

Tällä asetuksella voidaan säätää, miten pienistä raoista täyttömaali "vuotaa"
läpi. Vaihtoehtoja ovat "None", "Small", "Medium" ja "Large". Asetuksella
"None" maali valuu läpi kaikista pienistäkin raoista. Asetuksella "Small"
täyttöväri ei vuoda pienten rakojen läpi ja arvoilla "Medium" ja "Large"
voidaan valita "tilkittävien" rakojen suuruutta vastaavasti.

Alla olevissa esimerkkikuvissa lokeroiden välissä on eri suuruisia katkoviivoja.
Maali on kaadettu vasemman puoleisimpaan suureen lokeroon.
Ensimmäisessä kuvassa asetuksena on "None" ja maali on vuotanut läpi kaikista
katkoviivojen rei'istä. Seuraavissa kuvissa asetus on ollut "Small", "Medium" ja "Large" ja
niissä aina suuremmat ja suuremmat raot ovat olleet tilkittyinä.

{: .figure-small-row }
> ![Täyttö "sulje välit" -asetuksen arvolla "none"](../inkscape-taytto-sulje_valit-none.png)
> ![Täyttö "sulje välit" -asetuksen arvolla "small"](../inkscape-taytto-sulje_valit-small.png)
> ![Täyttö "sulje välit" -asetuksen arvolla "medium"](../inkscape-taytto-sulje_valit-medium.png)
> ![Täyttö "sulje välit" -asetuksen arvolla "large"](../inkscape-taytto-sulje_valit-large.png)

Tämän asetuksen kanssa on huomattavaa, että piirtoalueen zoomaus vaikuttaa
siihen, mitkä raot tulkitaan pieniksi, keskikokoisiksi ja suuriksi.