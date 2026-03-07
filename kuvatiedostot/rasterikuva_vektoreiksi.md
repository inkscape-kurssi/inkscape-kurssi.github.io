---
date: "2026-01-31T11:20:00+03:00"
title: "Rasterikuvan vektorointi"
layout: default
nav_order: 5
parent: Kuvatiedostot
---

# Rasterikuvan vektorointi

Toisinaan tulee vastaan tilanteita, joissa saatavilla on vain rasterikuva
jostain, mikä tavittaisiin mielellään vektorikuvana. Esimerkiksi
logo, joka tarvittaisiin tarkkana ja skaalautuvana.
Tällaisissa tilanteissa tarpeellinen toiminto on rasterikuvan *vektorointi*.

Vektoroinnin voi tehdä joko manuaalisesti taikka käyttämällä
Inkscapen tarjoamaan automaattista työkalua. Huolellinen manuaalinen
työskentely saattaa tuottaa joissain tilanteissa paremman lopputuloksen.
Toisaalta automaattinen työkalu on nopeampi ja varsinkin monimutkaisten
kuvien kanssa huomattavasti helpompi vaihtoehto. Usein paras vaihtoehto
on tehdä vektorointi ensin työkalulla ja sen jälkeen viimeistellä
käsin.

## Jäljitä bittikartta

Tutustutaan ensin *"Jäljitä bittikartta"* -työkaluun ("Trace bitmap").
Aloitetaan tuomalla piirtoalueelle melko pienenä rasterikuvana oleva
harmaasävyinen logo.

{: .figure-normal }
![Harmaasävyinen logo, jossa teksti "LOGO"](../Logo-grayscale-400.png)

Valitaan "Polku"-valikosta valinta "Jäljitä bittikartta...". Sama toiminto
löytyy myös kuvaa hiiren oikealla napilla esiin tulevasta kontekstivalikosta.
Saman dialogin saa esiin myös pikanäppäimellä *Shift-Alt-B*.

{: .figure-normal }
!["Polku"-valikossa valinta "Jäljitä bittikartta..."](../inkscape-trace-valikko.png)

Dialogissa on kolme välilehteä: *Single scan* yksivärisille vektoroinneille,
*Multicolor* monivärisille vektoroinneille ja *Pixel art* erityiseen
pikseligrafiikan luontiin. Tutustutaan näistä kahteen ensimmäiseen.

{: .figure-normal }
!["Jäljitä bittikartta" -dialogi](../inkscape-trace-dialogi.png)

### Single scan

Sincle scan muodostaa kuvasta vain yhden polun. Vaikka alkuperäisessä
kuvassa olisi valkoista ja mustaa, tämä tuottaa siis yhden tumman (mustan)
polun ja muu osa on läpinäkyvää.

Valitaan vektoroitava rasterikuvaobjekti valintatyökalulla.
Jos dialogissa on valittuna kohta "Live updates", näkyy "Preview"-osiossa
esikatselukuva tulevasta vektorikuvasta.

Dialogissa on ensimmäisenä valintana *Tunnistustapa* ("Detection mode"),
jolla valitaan menetelmä, jota käytetään vektorikuvan luomiseen.
Vaihtoehtoina ovat:

- *Brightness cutoff* – Kirkkaudessaan valitun kynnysarvon alle jäävät
    kohdat kuvasta tulkitaan mustaksi.
- *Edge detection* – Kuvasta tunnistetaan tumman ja vaalean väliset reunaviivat.
- *Color quantization* – Kuvasta tunnistetaan useampi tummuussävy ja ne
    vektoroidaan tummuuden mukaan vuorotellen mustiksi ja vaaleiksi (läpinäkyviksi).
- *Autotrace* – Käytetään Autotrace-algoritmia.
- *Centerline tracing* – Piirretään kuhunkin tunnistettuun alueeseen keskiviiva.

{: .figure-normal }
!["Tunnistustapa"-vaihtoehdot](../inkscape-trace-single_scan-detection_mode.png)

Tunnistustavan alapuolella on itse *kynnysarvon* valinta arvosta 0 arvoon 1.
Arvo 0 tarkoittaa täysin mustaa (ei kirkkautta) ja sillä, vain täysin mustat
kohdat muodostavat vektoripolun. Arvo 1 taas tarkoittaa täysin valkoista (täysi kirkkaus)
ja sillä käytännössä koko kuva tulkitaan mustaksi. Näiden arvojen
välillä oleva kynnysarvo määrittää kirkkauden, jota tummemmista kohdista muodostuu
luotava polku.

Alla olevissa kuvissa on alkuperäinen rasterikuvana oleva logo sekä
esikatselunäkymä kynnysarvoilla 0,400 ja 0,700. Näistä jälkimmäinen arvo
ylittää myös vaaleamman harmaan kirkkausarvon. Viimeisessä kuvassa on
laitettu päälle *Negatiivikuva* ("Invert image") -asetus, joka vaihtaa
tumman ja vaalean keskenään.

{: .figure-medium-row }
> ![Alkuperäinen logo rasterikuvana](../Logo-grayscale-400.png)
> ![Esikatselu kynnysarvolla 0,400](../inkscape-trace-cutoff_04.png)
> ![Esikatselu kynnysarvolla 0,700](../inkscape-trace-cutoff_07.png)
> ![Esikatselu "Invert image" -asetus päällä](../inkscape-trace-invert.png)

Muina valittavina parametreina ovat *"Specles"*, *"Smooth corners"* ja
*"Optimize"* sekä niiden lukuarvot. Näistä "Specles"-arvoa kasvattamalla
saadaan vektorointi ohittamaan kuvassa olevat pienet tahrat ja täplät.
"Smooth corners" tasoittaa lopputuloksesta pois teräviä kulmia.
"Optimize"-arvon kasvattaminen pyrkii vähentämään polkuun tulevien solmujen määrää.

Muissa tunnistustavoissa on kussakin oma säätöarvonsa.

{: .figure-normal }
![Edge detection](../inkscape-trace-edge_detection.png)


"Edge detection" -tilassa reunan kynnysarvo ("Edge threshold").

{: .figure-normal }
![Color quantization](../inkscape-trace-color_quantization.png)

"Color quantization" -tilassa värien määrä, eli kuinka moneen kirkkauteen
kuvan värisävyt jaotellaan.

{: .figure-normal }
![Autotrace](../inkscape-trace-autotrace.png)

{: .figure-normal }
![Centerline tracing](../inkscape-trace-centerline_tracing.png)

"Autotracella" ja sitä hyödyntävällä "Centerline tracing" -tilalla
lukumäärä, montako kertaa suodatinta suoritetaan sekä virheiden raja-arvo.

Näillä neljällä lopputulokset tästä harmaasävyisestä kuvasta näyttävät seuraavilta:

{: .figure-normal }
![Tulokset eri tavoilla](../inkscape-trace-single_scan-tulokset.png)


### Multicolor

{: .figure-normal }
!["Multicolor"-välilehti](../inkscape-trace-multicolor.png)

*"Multicolor"*-välilehden toiminta on pääpiirteissään samanlainen kuin
"Single scan" -välilehden, mutta yhden värisävyn sijaan etsitään *"Scans"*-arvolla
määrättyä määrää sävyjä, näistä muodostetaan polut ja yhdistetään samaan
ryhmään.

"Tunnistustapoina" tällä välilehdellä ovat:

- *Brightness steps* – Sävyt tunnistetaan kirkkauden mukaan, kuten "Single scan" -vaihtoehdossa.
    Lopputuloksena on harmaasävyinen kuva, jossa sävyjä on maksimissaan "Scan"-parametrin
    mukainen määrä.
- *Värit* – Tunnistetaan (enintään) "Scan"-parametrin mukainen määrä värejä ja muodostetaan niistä polut.
    Jos alkuperäisessä kuvassa on enemmän värisävyjä, niitä niputetaan yhteen ja keskimääräistetään.
- *Grays* – Muodostetaan harmaasävyinen kuva.
- *Autotrace* – Käytetään erillistä autotrace-algoritmia, joka on hitaampi, mutta toisinaan perusteellisempi.

Käytetään tällä kertaa alkuperäisenä rasterikuvana valokuvaa
Melissa Salmelan piirtämästä joulukortista.

{: .figure-normal }
![Kaksi piirrettyä mustavalkoista kissaa punaisella pohjalla](../kissa-04.jpg)

Tästä kuvasta neljä eri tunnistustapaa tekevät yllä luetellussa järjestyksessä seuraavat
vektorikuvat.

{: .figure-medium-row }
> ![Brightness steps](../kissat_brightness_steps.svg)
> ![Värit](../kissat_varit.svg)
> ![Grays](../kissat_grays.svg)
> ![Autotrace](../kissat_autotrace.svg)

Muita uusia asetuksia tällä "Multicolor"-välilehdellä ovat:

*Tasoita* – Rasterikuvalle tehdään sumennus ennen vektorointia. Esimerkiksi joidenkin
valokuvien kanssa tämä saattaa parantaa lopputulosta poistamalla
tarpeetonta epätasaisuutta.

*Stack*, eli *pinoaminen*, tarkoittaa sitä että ilman tätä asetusta
kukin erivärinen polku peittää vain oman alueensa ja polkujen muodostavat
alueet ovat vierekkäin. Tällöin niiden väliin saattaa jäädä tyhjiä
rakoja, joista tausta paistaa läpi. Jos taas "Stack"-asetus on
valittuna, eri väriset polut pinotaan päällekkäin, jolloin ei
muodostu väliin jääviä rakoja. Havainnollistetaan tätä vektoroimalla
alla oleva rantapallo karkeasti yhdeksällä värisävyllä.

{: .figure-normal }
![Rantapallo](../inkscape-trace-rantapallo.png)

Vasemmalla olevassa kuvassa "Stack"-asetus ei ole ollut päällä
ja oikeassa se on ruksittuna.

{: .figure-normal }
![Varsio ilman "Stack"-asetusta ja sen kanssa](../inkscape-trace-stack_versiot.png)

Alla olevissa kuvissa kummankin vektorikuvan osia on siirrelty hieman
niin, että näkyy, miten alla olevat polut ovat suurempia ja päällä olevat
peittävät alla olevia niin, että väleihin ei jää rakoja.

{: .figure-normal }
![Varsio ilman "Stack"-asetusta ja sen kanssa polut siirreltyinä](../inkscape-trace-stack_siirrelty.png)

Esitetään vielä yhtenä esimerkkinä maisemavalokuva ja siitä tehdyt vektoriversiot.

{: .figure-normal }
![Soutuvene lumisessa maisemassa](../vene-01.jpg)

Vektorikuva 8 värillä:

{: .figure-normal }
![Soutuvene lumisessa maisemassa vektorikuvana kahdeksalla värillä](../vene-8.svg)

Vektorikuva 20 värillä:

{: .figure-normal }
![Soutuvene lumisessa maisemassa vektorikuvana 20 värillä](../vene-20.svg)

Vektorikuva 40 värillä:

{: .figure-normal }
![Soutuvene lumisessa maisemassa vektorikuvana 20 värillä](../vene-40.svg)

## Käsin tehty vektorointi

Jos vektorointi halutaan tehdä käsin, se kannattaa todennäkoisesti
tehdä piirtotyökalulla seuraamalla kuvan ääriviivoja ja luomalla
polku kerrallaan yksi värialue kerrallaan. Parhaan tuloksen
saa yleensä käyttämällä vastaavaa pinoamistekniikkaa kuin
edellä "Stack"-asetuksen esittelyssä. Silloin piirrettyjen
värialueiden välille ei jää tyhjiä rakoja vaan alueet
on pinottuina päällekkäin.

Yksi tapa on seurata seuraavia vaiheita:
1. Asetetaan alkuperäinen rasterikuva taaemmalle tasolle ja lukitaan se.
    Tämän tason läpinäkyvyyttä voidaan tarvittaessa myös säätää, jos ei haluta
    sen olevan taustalla liian kirkkaana.
2. Lisätään päälle uusi taso, johon vektoripiirros piirretään.
3. Kierrätään koko kohteen ääriviivat piirtotyökalulla.
4. Korjaillaan ääriviivat solmutyökalulla siirtelemällä solmuja, kääntelemällä kaarevuuksia
    ja tarvittaessa lisäämällä tai poistamalla solmuja.
5. Rajataan ääriviivojen sisäpuolelta pienempiä eri värisiä alueita.
6. Tarvittaessa monistetaan ulointa ääriviivaa ja otetaan sillä leikkauksia
    muiden alueiden kanssa.
7. Lisäillään alueille sopivia täyttövärejä värivalitsimella alkuperäisestä kuvasta.

Piirtämisen aikana kannattaa hyödyntää eri värisiä ääriviivoja, tyhjää täyttöväriä
ja läpinäkyviä täyttövärejä, jotta on helpompi nähdä, missä alueiden
ääriviivat kulkevat.

Yleensä lopullisiin vektoroituihin kuviin kannattaa käyttää polkuja joissa on käytetty
vain täyttöväriä ja jätetty reunaväri pois. Tällä tavalla muodot
ja värit on yleensä helpompi hallita. Jos kuvassa on selkeitä viivoja, nämä
todennäköisesti kannattaa piirtää viivoina, mutta jossain vaiheessa muuttaa
myös täytetyiksi poluiksi "Reunaviiva poluksi" -toiminnolla.

{: .figure-normal }
![Kissan ääriviivojen piirtämistä piirtotyökalulla](../inkscape-trace_kasin-kissan_aariviivat.png)

Lopullinen käsin vektoroitu kissa.

{: .figure-full }
![Käsin vektoroitu kissa](../kissa-kasin.svg)

Käsin vektoroimalla lopputulos on yksinkertaisempi. Laatu riippuu siitä, miten paljon
kuvaa jaksaa muokata.

Käsin vektoroinnissa myös maaliämpäri on hyödyllinen työkalu. Alla oleva kuva on
vektoroitu käyttämällä maaliämpäriä eri värialueisiin erilaisilla kynnysarvoilla,
yhdistelemällä samaa väriä olevia alueita unionilla ja liittämällä maaliämpärin
luomiin polkuihin kynällä piirrettyjä alueita sekä pinoamalla värialueet sopivasti.

{: .figure-full }
![Maaliämpärillä vektoroidut kissat](../kissat_maaliamparilla.svg)
