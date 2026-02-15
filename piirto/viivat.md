---
date: "2026-01-17T18:14:00+03:00"
title: "Viivatyökalu"
layout: default
nav_order: 1
parent: Piirtotyökalut
---

# Viivatyökalu

{: .figure .figure-right }
![Viivatyökalun ikoni työkalupalkissa](../inkscape-viiva-ikoni.png)

Piirtotyökaluista ehkä yleiskäyttöisin on *viivatyökalu* (Pen Tool),
jolla voi piirtää avoimia tai suljettuja polkuja, jotka koostuvat
suorista tai kaarevista viivoista.

{: .figure-medium }
> ![Esimerkkinä erilaisia viivatyökalulla piirrettyjä murtoviivoja, kaarevia viivoja, avoimia ja suljettuja](../viivat-esimerkki.svg)

Kukin käyrä, eli *polku* koostuu piirtoalueella olevista pisteistä, eli *solmuista* (node)
ja niitä yhdistävistä *viivoista*, eli kaarista (edge). Viivat ovat aina kahden pisteen välillä
ja samaan pisteeseen voi kytkeytyä korkeintaan kaksi viivaa.

## Polku suorista janoista

Aloitetaan piirtämällä viiva-työkalulla polku, jonka kaikki viivat ovat suoria.

Valitaan viivatyökalu joko klikkaamalla työkalupalkista tai pikanäppäimellä *B*.
Polun piirtäminen alkaa klikkaamalla hiiren napilla halutusta kohdasta
piirtoaluetta ja jatkamalla klikkauksilla jokaisessa kohdassa, johon halutaan
uusi solmu. Kun kaikki halutut solmut ovat paikoillaan, klikataan hiiren oikealla
napilla tai painetaan *Enter*-näppäintä, mikä päättää polun piirtämisen.

{: .figure-medium-row }
> ![Viivatyökalulla piirtäminen](../inkscape-viiva-piirto.png)
> ![Valmis viiva, jonka reunaviiva on musta ja täyttö vaaleanpunainen](../inkscape-viiva-valmis.png)

Huomaa, että piirtämisen aikana lukitut viivat näkyvät sinisenä ja punaisena
näkyvä viiva on vasta piirrettävänä oleva seuraava viiva.

Kun polun piirtäminen päätetään, sen täytöksi tulee valittuna oleva väri ja
reunaviivan väriksi ja paksuudeksi vastaavasti valittuna olevat asetukset.

Polun piirtämisen voi päättää myös klikkaamalla sen viimeinen piste hiiren vasemmalla napilla
samaan kohtaan kuin sen aloituspiste. Silloin lopputuloksena saadaan suljettu polku.
Suljetun polun saa aikaiseksi myös päättämällä piirtämisen *Shift-Enter* -näppäinyhdistelmällä
pelkän *Enter*-näppäimen sijaan. Silloin polun ensimmäinen ja viimeinen piste yhdistetään
suoralla janalla.

{: .figure-medium-row }
> ![Polun piirtämisen päättäminen klikkaamalla aloituspistettä](../inkscape-viiva-piirto-suljettu.png)
> ![Valmis suljettu polku](../inkscape-viiva-valmis-suljettu.png)

On hyvä muistaa, että ikkunan alareunassa väripaletin alla oleva vihjepalkki antaa aina
ajantasaisen ohjeen siitä, mitä ollaan tekemässä ja millä pikanäppäimillä voi
muokata käytössä olevan työkalun toimitaa. Alla olevassa kuvassa vihjepalkissa kerrotaan,
että ollaan piirtämässä janaa, jonka kulma on tällä hetkellä -9,29° ja pituus 7,04 mm.
Lisäksi muistutetaan, että *Ctrl*-näppäintä painamalla kulma lukittuu tasavälein ja
että polun piirtämisen voi päättää *Enter*- tai *Shift-Enter*-näppäilyillä.

{: .figure-full }
> ![Inkscapen alareunan väripaletti ja vihjeteksti](../inkscape-viiva-vihjepalkki.png)

## Kaarevat polut

Polusta voi tehdä suorista janoista koostuvan sijaan kaarevan "venyttämällä" jokaisen
välipisteen kohdalla. Kun välipiste luodaan hiirellä klikkaamalla, ei päästetäkään
hiiren napista irti vaan pidetään se pohjassa ja venytetään esiin tulevaa pyöreää
kahvasaa vetämällä polulle pyöristystä solmun kohdalle.

{: .figure-medium-row }
> ![Polun piirtäminen. Kolmannen solmun kohdalla venytetäänkin kahvasta.](../inkscape-viiva-kaareva-1.png)
> ![Jatketaan piirtämistä](../inkscape-viiva-kaareva-2.png)
> ![Neljännen solmun kohdalla venytetään taas kahvoista.](../inkscape-viiva-kaareva-3.png)
> ![Valmis suljettu polku](../inkscape-viiva-kaareva-4.png)

Piirtotyökalulla polkua piirrettäessä pisteen molempien puolien kahvat toimivat symmetrisesti,
eli pisteen kohdalle polkuun tulee samanlainen kaarevuus kumpaankin siitä lähtevään
polun osaan. Myöhemmin opetellaan, miten näitä pyöristyskahvoja voidaan siirrellä jälkikäteen
tarkemmin *solmutyökalulla*.


## Polun jatkaminen

Kun viivatyökalulla on piirretty avoin polku, sitä on mahdollista jatkaa klikkaamalla
työkalulla polun toista päätä ja jatkamalla uusien solmujen luomista.
Piirtämisen voi päättää normaaliin tapaan joko jättämällä polun avoimeksi tai
sulkemalla sen.

{: .figure-medium-row }
> ![Valmiin valitun polun toisesta päästä on jatkettu piirtämistä.](../inkscape-viiva-jatko-1.png)
> ![Piirtäminen päätetään valmiin polun toiseen päähän.](../inkscape-viiva-jatko-2.png)
> ![Valmis polku, jossa alkuperäisen avoimen polun päät on yhdistetty murtoviivalla yhdeksi suljetuksipoluksi.](../inkscape-viiva-jatko-3.png)

## Solmujen kohdistaminen

Viivoja piirtäessä on toisinaan tarpeen saada uuden polun solmu osumaan
täsmälleen samaan pisteeseen kuin aiemman polun solmu. Tässä auttaa, jos
ominaisuus nimeltä *tarttuminen* (*snap*) on päällä. Tämän ominaisuuden
voi kytkeä päälle Inkscapen oikeasta yläkulmasta.

{: .figure-medium }
> ![Tarttumisnappi klikattuna päälle. Kuvakkeena magneetti.](../inkscape-viiva-snap.png)

Tämä toiminto on kuvakkeensa mukaisesti kuin magneetti, joka napauttaa 
piirtotyökalun kiinni jo olemassa olevaan solmuun, kun sellainen osuu
lähelle hiiren kohdistinta. Solmujen lisäksi piirtotyökalu tarttuu myös
solmujen välissä olevaan viivaan tai käyrään, mikä helpottaa siistien
kuvien piirtämistä.

{: .figure-medium-row }
> ![Uuden polun piirtäminen napsahtaa kiinni aiemman polun solmuun.](../inkscape-viiva-snap-node.png)
> ![Uuden polun piirtäminen napsahtaa kiinni aiemman polun viivaan.](../inkscape-viiva-snap-path.png)

## Asetuspalkki

Viivatyökalun asetuspalkista voi valita työkalun toimintatilan.
Ensimmäinen tila on *tavallinen bezier-polku*. Sen jälkeen tulevat
*Spiro-polku*, *BSpline-polku*, *suorat viivalohkot* sekä *kohtisuorat janat*.

{: .figure-full }
> ![Viivatyökalun asetuspalkki](../inkscape-viiva-palkki.png)

Ensimmäinen tila toimii, kuten edellä on kuvattu. *Spiro-tilassa* polku muodostuu
ympyrän kaarista, jotka kulkevat luotujen solmujen kautta.

{: .figure-medium-row }
> ![Spiro-viivan piirtäminen](../inkscape-viiva-spiro-1.png)
> ![Spiro-viivan piirtäminen](../inkscape-viiva-spiro-2.png)
> ![Spiro-viivan piirtäminen](../inkscape-viiva-spiro-3.png)
> ![Valmis suljetu Spiro-viiva](../inkscape-viiva-spiro-4.png)

*BSpline-polut* on toinen tapa piirtää polkuja pyöristetyillä kulmilla.
Lisää bsplinestä voi kulea [Wikipediasta][Wikipedia-bspline]. Parhaiten sen
toiminta varmasti avautuu kokeilemalla.

{: .figure-medium-row }
> ![BSpline-polun piirtäminen](../inkscape-viiva-bspline-1.png)
> ![BSpline-polun piirtäminen](../inkscape-viiva-bspline-2.png)
> ![BSpline-polun piirtäminen](../inkscape-viiva-bspline-3.png)
> ![Valmis suljettu BSpline-polku](../inkscape-viiva-bspline-4.png)

*Suorat viivalohkot* toimivat muuten samoin samoin kuin tavallinen bezier-polku,
mutta sen kulmia ja viivoja ei voi piirron aikana pyöristää vaan niistä tulee
automaattisesti kärkiä ja suoria.

{: .figure-medium-row }
> ![Suoran viivapolun piirtäminen](../inkscape-viiva-suora-1.png)
> ![Valmis suljettu suorista lohkoista koostuva polku](../inkscape-viiva-suora-2.png)

*Kohtisuorilla janoilla* piirtäminen on puolestaan rajoitettua niin, että kuhunkin
solmuun muodostuu suora kulma.

{: .figure-medium-row }
> ![Kohtisuorilla janoilla piirtäminen](../inkscape-viiva-kohtisuora-1.png)
> ![Valmis kohtisuorilla janoilla piirretty suljettu polku](../inkscape-viiva-kohtisuora-2.png)

Asetuspalkin *Shape*-valinnalla voi valita muodon, jota piirrettävälle viivalle käytetään.
*Scale*-lukuarvo määrää käytettävänmuodon kokoskaalan.

{: .figure-medium }
> ![Shape- ja scale-asetukset viivatyökalun asetuspalkissa](../inkscape-viiva-shape-valikko.png)

Alla olevassa esimerkissä on piirrettynä kolme viivaa asetuksilla "Triangle in", "Triangle out" ja "Ellipsi".

{: .figure-medium }
> ![Kolme viivaa triangle in -, triangle out - ja ellipsi-shape-asetuksella](../inkscape-viiva-shape-esimerkki.png)



## Viivat ja käyrät SVG:ssä

Inkscapea käytettäessä ei ole välttämätöntä tietää, miten SVG-tiedostomuodossa
polut esitetään, mutta joillekin lukijoille tämä tieto voi olla valaisevaa.

SVG-tiedostoissa vapaamuotoiset käyrät esitetään `<path>`-elementteinä
joissa käyrän osat voivat olla suoria, kaaria tai bezier-käyriä.
Käyrän kulku kuvataan sarjana komentoja, joilla polkua piirtävää "kynää" voi
siirtää (**m**, **M**) tai piirtää suoria viivoja (vaaka: **h**, **H**, pysty: **v**, **V**,
vino: **l**, **L**), kaaria (**a**, **A**) sekä bezier-käyriä (**s**, **S**, **c**, **C**).
Komennoilla voi myös käskeä yhdistämään päätepiste piirron aloituspisteeseen (**z**).

{: .example-title }
> SVG-esimerkki
>
> ```xml
> <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="100" height="100" viewBox="0 0 100 100">
>     <path stroke="black" fill="#ffcc00" stroke-width="1"
>           d="M20 10
>             h20
>             v10
>             l30 20
>             s10 5 -20 10
>             c-10 -10 -20 -10 -30 0
>             a5 10 -20 1 1 -10 -30
>             z">
>     </path>
> </svg>
> ```

Ylläoleva svg-kuva näyttää tältä:

{: .figure-medium }
> ![Esimerkkikuva path-elementtinä piirretystä kuvasta](../path-elementti.svg)


Lisää SVG-kuvien piirtämisestä kirjoittamalla suoraan `<path>`-elementtejä voi opiskella
[Mozillan tutoriaalista][moz-path]. Bezier-käyrien teoriaan tutustumisen voi aloittaa
[Wikipediasta][Wikipedia-bezier].



[moz-path]: https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorials/SVG_from_scratch/Paths
[Wikipedia-bezier]: https://en.wikipedia.org/wiki/B%C3%A9zier_curve
[Wikipedia-bspline]: https://en.wikipedia.org/wiki/B-spline