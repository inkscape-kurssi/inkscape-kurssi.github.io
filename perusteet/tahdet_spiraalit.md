---
date: "2026-01-17T15:49:00+03:00"
title: "Tähdet, spiraalit ja laatikot"
layout: default
nav_order: 6
parent: Perusteet
---

# Tähdet, monikulmiot, spiraalit ja laatikot

{: .figure .figure-right }
![Tähti ja ja monikulmio -, laatikko- ja spiraali-työkalujen ikonit työkalupalkissa](../inkscape_tahti-ikoni.png)

Tähdet ja monikulmiot sekä spiraalit toimivat työkaluina vastaavalla tavalla kuin suorakulmiot ja
ellipsit. Laatikkotyökalulla voidaan lisäksi piirtää kolmiulotteiselta näyttäviä
kappaleita.

Myös nämä työkalut löytyvät Inkscapen vasemman reunan työkalupalkista heti
suorakulmioiden ja ellipsien alapuolelta.

## Tähdet ja monikulmiot

Samalla työkalulla voidaan piirtää sekä *tähtiä* että *säännöllisiä monikulmioita*.
Työkalun pikanäppäin on *\**, eli asteriski, eli tähti.
Tällä työkalulla valitaan ensin työkalun asetuspalkista, kumpaa kuviotyyppiä,
tähtiä vai monikulmioita, halutaan piirtää ja sen jälkeen kulmien tai sakaroiden
määrä.

{: .figure .figure-full }
![Tähdet ja monikulmio -työkalun asetuspalkki](../inkscape-tahti-asetukset.png)

Kuvion tyypin valinnan jälkeen piirtäminen tapahtuu jälleen painamalla hiiren nappi pohjaan,
raahaamalla ja päästämällä nappi ylös. Piirtäminen alkaa kuvion keskipisteestä
ja päättyy yhteen monikulmion kulmaan taikka tähden sakaraan. Kuvion asento
ja koko määräytyy siitä, mihin piirtäminen päättyy. Jos piirtäessä pidetään
pohjassa *Ctrl*-näppäintä, kuvion asento lukittuu 15 asteen kulmien välein.
Tämä helpottaa kuvion piirtämistä tiettyy säännölliseen asentoon.

{: .figure .figure-medium-row }
![Oranssi 5-kulmio](../inkscape-monikulmio-piirros.png)
![Keltainen 5-sakarainen tähti](../inkscape-tahti-piirros.png)


Piirtämisen jälkeen voidaan vielä vaihtaa valitun kuvion tyyppiä valitsemalla
työkalun asetuspalkista. Monikulmio muuttuu tähdeksi, jonka sakarat ovat siellä,
missä monikulmion kärjet olivat, ja tähti muuttuu vastaavasti monikulmioksi.

Samoin työkalupalkista on mahdollista vaihtaa piirtämisen jälkeen myös
kulmien ja sakaroiden määrää.

Monikulmiossa on yhdessä kuvion kulmassa **neliön muotoinen kahva**, jota siirtämällä
kuvion asentoa ja kokoa voidaan muokata.

Tähdessä näitä kahvoja on kaksi. Niistä **toinen on tähden yhden sakaran kärjessä**
ja **toinen kahden kärjen välissä olevassa kulmassa**. Sakaran kärjessä olevaa
kahvaa liikuttamalla tähteä voi pyörittää ja kärjen terävyyttä lisätä tai
vähentää. Sakaroiden välissä olevan kulman kahvasta liikuttamalla tähti puolestaan
saadaan muodoltaan vinoksi. Tällä tavalla voidaan piirtää vaikka sirkkelin terä.

Muutettasessa monikulmion tai tähden muotoa kahvoja siirtämällä voidaan *Ctrl*-näppäintä
pohjassa pitämällä estää kahvan siirtyminen kiertosuunnassa, jolloin vain
kulman etäisyys keskipisteestä muuttuu. Tämä helpottaa esimerkiksi tähden
terävyyden muokkaamista ilman, että sen asento muuttuu tai se kiertyy sirkkelin teräksi.

{: .figure .figure-medium-row }
![Tähti, jossa on pitkät terävät sakarat.](../inkscape-tahti-terava.png)
![Tähti, jonka sakarat ovat vinossa.](../inkscape-tahti-vino.png)

## Asetuspalkki

Asetuspalkissa monikulmioilla ja tähdillä on osittain samat ja osittain toisistaan
poikkeavat asetukset. Kuvion tyypin vaihtonapit, kulmien määrän valinta,
pyöristysasetus sekä sekoitusasetus ovat yhteiset.

{: .figure .figure-full }
![Tähdet ja monikulmiot -työkalun asetuspalkki](../inkscape-tahti-asetukset.png)

*Pyöristys* muuntaa monikulmion tai tähden sivut kaareviksi ja kulmat pyöreiksi.
Positiivinen arvo "pullistaa" kuviota tehden kuvion pehmeämmän näköiseksi. Negatiivinen arvo
puolestaan kaartaa sivut sisään päin tehden kulmista ja sakaroista "silmukoita".

{: .figure .figure-small-row }
![Pyöristetty 5-kulmio](../inkscape-monikulmio-pyorea.png)
![Pyöristetty 5-sakarainen tähti](../inkscape-tahti-pyorea.png)
![Sisään päin pyöristetty 5-kulmio, jonka kulmista on tullut lenkit](../inkscape-monikulmio-pyorea-negatiivinen.png)
![Sisään päin pyöristetty 5-sakaranien tähti, jonka sakaroista ja sisäkulmista on tullut lenkit](../inkscape-tahti-pyorea-negatiivinen.png)


*Sekoitus* satunnaistaa molemmissa kuvioissa kulmien suuruutta ja sijaintia jonkin verran,
jolloin kuviot eivät ole täysin säännöllisiä.

{: .figure .figure-small-row }
![5-kulmio, joka ei ole säännöllinen](../inkscape-monikulmio-sekoitus.png)
![5-sakarainen tähti, jonka sakarat ovat keskenään erilaiset](../inkscape-tahti-sekoitus.png)

Tähdessä on lisäksi asetus *syvyydelle* (Spoke Ratio), joka tarkoittaa sakaroiden välissä olevan
pisteen etäisyyttä tähden keskipisteestä suhteessa sakaroiden kärkien etäisyyteen keskipisteestä.
Oletuksena syvyyden arvo on 0,5. Mitä lähemmäs nollaa tämän arvon muuttaa, sen
lähemmäs tähden keskipistettä sakaroiden välit menevät ja sitä pidempiä sakarat
ovat suhteellisesti. Jos taas arvo lähenee lukua 1, lähenee n-sakarainen tähti
2n-kulmiota.

Alla esimerkkinä tähdet, joiden syvyyksien arvot ovat 0,190; 0,400; 0,650 ja 1,000.

{: .figure .figure-small-row }
![5-sakarainen tähti, jonka syvyys on 0,190. Erittäin terävät sakarat.](../inkscape-tahti-spoke-019.png)
![5-sakarainen tähti, jonka syvyys on 0,400. Normaalit sakarat.](../inkscape-tahti-spoke-040.png)
![5-sakarainen tähti, jonka syvyys on 0,650. Vähän pullealta näyttävä tähti.](../inkscape-tahti-spoke-065.png)
![5-sakarainen tähti, jonka syvyys on 1,000. Tähti on muuttunut 10-kulmioksi.](../inkscape-tahti-spoke-100.png)

Asetuspalkin viimeisenä kohtana on molemmilla kuviotyypeillä peruutusnappi, jolla
kuvion voi nollata alkuasetuksiinsa.


## Spiraali

*Spiraalityökalu* tuottaa nimensä mukaisesti spiraalin. Sen pikanäppäin on *I*. Piirtäminen alkaa
hiiren klikkauksella spiraalin keskipisteestä ja päättyy hiiren napin nostamiseen
spiraalin ulkoreunalla.

{: .figure .figure-medium-row }
![Musta spiraaliviiva, joka alkaa keskeltä ja kiertää kolme kierrosta](../inkscape-spiraali-piirros.png)

Spiraalin asetuspalkista voidaan valita spiraaliin haluttu *kierrosten* määrä,
kierrosten *poikkeama* sekä spiraalin *sisin säde*.

{: .figure .figure-full }
![Spiraalityökalun asetuspalkki](../inkscape-spiraali-asetukset.png)

*Poikkeamalla* tarkoitetaan spiraalin kierrosten välistä tiheyden eroa spiraalin keskellä
ja ulkoreunalla. Arvo 1 tarkoittaa, että kierrokset ovat tasavälein koko spiraalin matkalla.
Lukua 1 pienemmillä arvoilla spiraalin kierrokset ovat ulkoreunalla tiheämmin kuin keskellä
ja lukua 1 suuremmilla arvoilla spiraalin sisäosa on tiheä ja ulkokehät harvempia.

Alla esimerkkinä spiraaleja, joissa kaikissa on 14 kierrosta, mutta poikkeaman arvoina:
0,100; 0,300; 0,700; 1,000; 1,500 ja 3,100.

{: .figure .figure-small-row }
![Spiraali poikkeamalla 0,100. Kaikki kasautuneena ulkokehälle.](../inkscape-spiraali-poikkeama-010.png)
![Spiraali poikkeamalla 0,300. Painottunut enemmän ulkoreunaan kuin sisään.](../inkscape-spiraali-poikkeama-030.png)
![Spiraali poikkeamalla 0,700. Vain vähän painottunut ulkoreunalle.](../inkscape-spiraali-poikkeama-070.png)
![Spiraali poikkeamalla 1,000. Spiraalin kierrosten välit ovat tasaiset koko matkalla.](../inkscape-spiraali-poikkeama-100.png)
![Spiraali poikkeamalla 1,500. Vähän painottunut sisukseen.](../inkscape-spiraali-poikkeama-150.png)
![Spiraali poikkeamalla 3,100. Painottunut vahvasti spiraalin keskukseen.](../inkscape-spiraali-poikkeama-310.png)

Spiraalin *sisin säde* on oletuksena nolla, mikä tarkoittaa, että spiraali alkaa
aivan keskeltä. Jos tämän säteen arvoa kasvattaa, alkaa näkyvä spiraali kauempaa
spiraalin keskipisteestä. Arvo on suhtessa spiraalin koko kokoon, eli lähellä lukua
1 oleva arvo tarkoittaa, että spiraali alkaa läheltä sen ulkokehää.

Alla esimerkit säteen arvoilla 0; 0,200; 0,500 ja 0,750.

{: .figure .figure-small-row }
![Spiraali alkaa aivan keskeltä.](../inkscape-spiraali-sade-0.png)
![Spiraali alkaa 0,2 säteen etäisyydeltä keskeltä.](../inkscape-spiraali-sade-02.png)
![Spiraali alkaa puolivälin etäisydeltä keskeltä.](../inkscape-spiraali-sade-05.png)
![Spiraali alkaa läheltä ulkokehää.](../inkscape-spiraali-sade-075.png)

Kierrosten määrää ja sisintä sädettä voi muokata myös ottamalla hiirellä kiinni
spiraalin niitä vastaavien päiden kahvoista ja "kerimällä" spiraaliin lisää tai
vähemmän kierroksia liikuttamalla spiraalin päätä keskipisten ympäri.


## Laatikko

*Laatikkotyökalulla* voi luoda kolmiulotteisilta näyttäviä laatikkokappaleita.
Työkalun pikanäppäin on *Shift-F4*.
Luodulla laatikolla on kahdeksan kulmaa ja kolme perspektiivin katoamispistettä.
Katoamispisteet voi valita joko äärellisiksi taikka äärettömiksi, jolloin
laatikon yhdensuuntaisia esittävät sivut ovat myös piirroksessa samansuuntaisilla
suorilla.

{: .figure .figure-medium }
![Piirtoalueella sininen varjostettu kolmiulotteinen laatikko ja pystysuuntaiset apuviivat sekä kaksi katoamispistettä ja niihin suuntaavat apuviivat](../inkscape-laatikko.png)

Laatikkotyökalua voi käyttää joko laatikoiden piirtämiseen taikka perspektiiviä
sisältävän piirroksen apuviivojen ja -kuvioiden piirtämiseen.

Laatikon asetuspalkista voi lukita haluamansa akselien suunnat yhdensuuntaisiksi
tai jättää ne avoimiksi. Oletuksena on "tavallinen" tilanne, jossa pystysuorat (y)
laatikon reunat on lukittu yhdensuuntaisiksi ja kahden muun suunnan sivut
kohtaavat kahdessa katoamispisteessä.

{: .figure .figure-full }
![Laatikko-työkalun asetuspalkki](../inkscape-laatikko-asetukset.png)

Lukitsemalla kaikki suunnat käyttämään yhdensuuntaisia viivoja ilman katoamispisteitä,
voidaan piirtää niin sanottuja [isometristä projektiota][isometrinen projektio] käyttäviä kuvia.
Isometrisiä projektioita käytetään usein havainnepiirroksissa, matematiikassa sekä
esimerkiksi peleissä, joissa halutaan poistaa perspektiivin vaikutus kappaleiden kokoon.

{: .figure .figure-medium }
![Kolme isometrisesti piirrettyä laatikkoa.](../inkscape-laatikko-isometrinen.png)

Laatikkotyökalun käyttö avautuu parhaiten kokeilemalla ja harjoittelemalla.

[isometrinen projektio]: https://fi.wikipedia.org/wiki/Isometrinen_projektio