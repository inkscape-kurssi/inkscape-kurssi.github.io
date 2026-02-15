---
date: "2026-01-31T11:20:00+03:00"
title: "Apuviivat"
layout: default
nav_order: 1
parent: Apuvälineet
---

# Apuviivat

Piirtäessä tarvitaan toisinaan erilaisia apuviivoja, jotka eivät
ole osa varsinaista piirrosta, mutta joita käytetään piirtämisen
apuna kohdistamaan erilaisia kohteita.

Inkscapessa on tarjolla muutamia erilaisia apuviivoja sekä visuaaliseen
kohdistamiseen että automaattiseen kohdalle "napsahtamiseen". Tärkeimmät
apuviivoja koskevat asetukset löytyvät piirtoasiakirjan asetuksista,
joita pääsee muokkaamaan "Asiakirjan ominaisuudet" -dialogissa.
Dialogi aukeaa joko "Tiedosto"-valikon kohdasta "Asiakirjan ominaisuudet"
tai komentopalkin napilla taikka pikanäppäimellä *Shift-Ctrl-D*.

{: .figure-normal }
> ![Asiakirjan ominaisuudet -nappi](../inkscape-apuviivat-dokumentin_asetukset_ikoni.png)

Dialogissa on erilliset välilehdet apuviivoille ja ruudukoille.
Tarkastellaan ensin ruudukkojen käyttöä.

## Ruudukot

*Ruudukko*, eli *grid*, on koko piirtoalueen peittävä toistuva apuviivojen muodostama
verkko, joka auttaa kohdistamaan kohteita säännönmukaisille etäisyyksille toisistaan.

Kun "Asiakirjan ominaisuudet" -dialogista valitaan näkyville "Ruudukot"-välilehti,
siellä ei ole vielä yhtään ruudukkoa, jos niitä ei ole vielä käytetty.
Vaihtoehtoina on lisätä uusi ruudukko joka on jotain kolmesta tyypistä:
"Suorakulmainen" (Rectangular), "Aksonometrinen" (Axonometric) tai "Modulaarinen" (Modular).

{: .figure-normal }
> ![Asiakirjan ominaisuudet -dialogin ruudukot-välilehti](../inkscape-apuviivat-ruudukot_dialogi.png)

Samassa piirtokuvassa voi olla yhtä aikaa määriteltynä useita ruudukkoja
ja voidaan valita, mitkä niistä ovat käytössä ja mitkä näkyvissä.

Kaikkien käytössä olevien ruudukkojen näyttämistä ja piilottamista
saa helposti vaihdettua pikanäppäimellä *Shift-#*.

### Suorakulmainen ruudukko

Lisätään aluksi suorakulmainen ruudukko.

{: .figure-normal }
> ![Asiakirjan ominaisuudet -dialogin ruudukot-välilehti](../inkscape-apuviivat-ruudukot_suorakulma.png)

Ruudukosta voi valita, onko se käytössä, näkyvissä,
kiinnitetäänkö kohteita vain kulloinkin näkyvillä oleviin apuviivoihin ja näytetäänkö
viivojen sijaan vain pisteet apuviivojen leikkauskohdissa.

Varsinaisista ruudukon ominaisuuksista voi määritellä käytettävän mittayksikön, esimerkiksi
millimetrit, ensimmäisen ruudun aloituksen x- ja y-suunnassa vasemmasta yläkulmasta,
viivojen välin suuruuden x- ja y-suunnassa, pääruudukon ja alaruudukon värit sekä sen,
kuinka monen viivan välein piirretään pääruudukon viivat. Pääruudukolla tarkoitetaan
hieman paksumpia ja mahdollisesti eri värillä piirrettyjä apuviivoja. Vastaavaan tapaan
kuin millimetripaperissa on pienempiä tiheämpiä viivoja millimetrin välein ja paksumpia
viivoja senttimetrin välein.

Ruudukon tasauksesta voi valita, mistä kohtaa ruudukon piirtäminen alkaa. Kohdistetaanko
ruudukko esimerkiksi vasempaan yläkulmaan vai levittäytyykö se piirtoalueen yli
keskeltä alkaen. Tämä on pikavalinta, joka vaikuttaa "aloitus"-asetukseen.

{: .figure-medium-row }
> ![Ruudukko tasattu alkamaan vasemmasta yläkulmasta](../inkscape-apuviivat-ruudukot-kulma.png)
> ![Ruudukko näkyvissä vain pisteinä](../inkscape-apuviivat-ruudukot-pisteet.png)
> ![Ruudukko zoomattuna](../inkscape-apuviivat-ruudukot-zoomattu.png)
> ![Ruudukko zoomattuna. Pääruudukko punaisena, alaruudukko sinisenä](../inkscape-apuviivat-ruudukot-paa_ja_ala.png)

Ruudukon avulla piirrettäessä valitaan haluttu tarttumistapa Inkscapen ikkunan oikeassa yläkulmassa olevasta
tarttumisvalikosta.

{: .figure-normal }
> ![Tarttumisvalikko](../inkscape-apuviivat-ruudukot-tarttuminen.png)

Tässä valikossa on monta valintaa sille, mihin kaikkiin piirroksen osiin kulloinen
piirtotyökalu *tarttuu* (*snap*) ja onko tarttuminen ylipäätään sallittua.
Ruudukon kannalta olennaiset valinnat ovat *Ruudukot* ja sen alla oleva *Ruudukon viivat* (Grid Lines).
Kun ne ovat valittuina, kaikki piirtotyökalut sekä valintatyökalulla ja solmutyökalulla tapahtuvat
siirtämiset napsahtavat, eli tarttuvat, ruudukon risteyksiin sekä ruudukon viivoihin.

Alla olevissa kuvissa ensin piirretään polku, jonka solmupisteet ovat ruudukon
risteyksissä. Sitten siirretään suorakulmiota, joka siirrettäessä tarttuu
napsahtaen ruudukkoon. Kolmanneksi siirretään polun solmuja ruudukon
risteyksistä toisiin. Neljännessä kuvassa on zoomattu lähemmäs ja nähdään,
että solmun siirtäminen tarttuu tässä tilanteessa ruudukon risteysten
lisäksi myös itse ruudukon viivoihin.

{: .figure-medium-row }
> ![Piirtäminen](../inkscape-apuviivat-ruudukot-piirtaminen.png)
> ![Siirtäminen](../inkscape-apuviivat-ruudukot-siirtaminen.png)
> ![Solmun siirtäminen](../inkscape-apuviivat-ruudukot-solmun_siirtaminen.png)
> ![Viivaan tarttuminen](../inkscape-apuviivat-ruudukot-viivaan_tarttuminen.png)

### Aksonometrinen ruudukko

Toinen ruudukon tyypin vaihtoehto on *aksonometrinen* ruudukko, joka koostuu
suorakulmaisten apuviivojen sijaan toisiinsa nähden 60 asteen kulmissa
olevista apuviivoista ja neliön muotoisten ruutujen sijaan ne muodostavat
tasasivuisia kolmioita.

{: .figure-normal }
> ![Aksonometrisen ruudukon asetukset](../inkscape-apuviivat-ruudukot-aksonometrinen-asetukset.png)


Tätä ruudukkoa voidaan hyödyntää [aksonometristen][Axonometry]-kaavioiden
piirtämiseen. Niillä voidaan esittää kolmiulotteisia kappaleita
ilman perspektiivivaikutelmaa niin, että kaikkien kolmen akselin
suuntaiset etäisyydet ovat samassa suhteessa.

{: .figure-medium-row }
> ![Aksonometrinen ruudukko](../inkscape-apuviivat-ruudukot-aksonometrinen.png)
> ![Aksonometrinen ruudukko](../inkscape-apuviivat-ruudukot-aksonometrinen_laatikko.png)


### Modulaarinen ruudukko

Kolmas ruudukon tyyppi on *modulaarinen*. Se luo ruudukon, joka koostuu
suorakulmaisista "laatikoista", joiden väliiin voidaan määritellä
*väli* (gap) ja *marginaali* (margin).

{: .figure-normal }
> ![Modulaarisen ruudukon asetukset](../inkscape-apuviivat-ruudukot-modular-asetukset.png)

Tässä pari esimerkkiä:

{: .figure-medium-row }
> ![Modulaarinen ruudukko ilman marginaalia](../inkscape-apuviivat-ruudukot-modular.png)
> ![Modulaarinen ruudukko marginaalilla](../inkscape-apuviivat-ruudukot-modular_margin.png)

Tätä ruudukkoa voidaan käyttää esimerkiksi erilaisten korttien suunnittelemiseen.

## Omat apuviivat

Piirtoalueelle voi lisätä myös omia apuviivoja raahaamalla ne esiin piirtoalueen
reunalla olevasta mitta-asteikosta. Hiirellä otetaan kiinni mitta-asteikosta
ja raahaamalla vedetään esiin apuviiva. Vasemman reunan asteikosta
raahaamalla saadaan pystysuoria apuviivoja ja yläreunan asteikosta
vaakasuoria apuviivoja. Diagonaalit apuviivat saadaan vedettyä esiin
piirtoalueen kulmista.

{: .figure-medium-row }
> ![Vedetään pystysuora apuviiva esiin](../inkscape-apuviivat-oma-pysty.png)
> ![Vedetään vaakasuora apuviiva esiin](../inkscape-apuviivat-oma-vaaka.png)
> ![Vedetään diagonaali apuviiva esiin](../inkscape-apuviivat-oma-swne.png)
> ![Vedetään toiseen suuntaan diagonaali apuviiva esiin](../inkscape-apuviivat-oma-senw.png)

"Asiakirjan ominaisuudet" -dialogin "Apuviivat"-välilehdellä voi valita,
näytetäänkö omat apuviivat, ovatko ne lukittuina niin, etteivät ne siirry
vahingossa, mitkä niiden värit normaalisti ja siirrettäessä.

Lisäksi sieltä voidaan lisätä apuviivat sivun kullekin reunalle
sekä poistaa kaikki apuviivat.

{: .figure-normal }
> ![Apuviivojen asetukset](../inkscape-apuviivat-oma-asetukset.png)

[Axonometry]: https://en.wikipedia.org/wiki/Axonometry