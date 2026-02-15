---
date: "2026-01-31T11:20:00+03:00"
title: "Liukuvärit"
layout: default
nav_order: 1
parent: Värityökalut
---

# Liukuvärit

{: .figure .figure-right }
![Liukuvärityökalun kuvake työkalupalkissa](../inkscape-liukuvari-ikoni.png)

Tasaisten värien lisäksi kohteiden täyttöväriksi sekä reunaväriksi
voidaan valita erilaisia liukuvärjäyksiä, eli gradientteja.
Vaihtoehtoina ovat lineaarinen ja säteittäinen liukuväri. Lisäksi
käytettävissä on myös monimutkaisempi [mesh](../mesh)-liukuvärjäys.

Liukuvärejä voidaan luoda työkalupalkin *Liukuväri*-työkalulla, jonka
pikanäppäin on *G*.

Liukuvärityökalun asetuspalkissa on valittavina liukuvärin tyyppi,
lineaarinen eli suora sekä säteittäinen. Toisena tärkeänä valintana
on, käytetäänkö liukuväriä kohteen täyttöön vai reunaan.

{: .figure-full }
> ![Liukuvärityökalun asetuspalkki](../inkscape-liukuvari-asetuspalkki.png)

## Lineaarinen liukuväri

*Lineaarinen liukuväri tarkoittaa väriliukua, jossa väri vaihtuu
tasaisesti yhden tai useamman värin kautta suoraaviivaisesti
edeten.

Alla olevassa kuvassa on esitetty muutama esimerkki liukuvärien käytöstä
Ensimmäinen suorakulmio on täytetty kahden värin, punaisen ja keltaisen, välisellä
liukuvärillä. Toisessa on liuku läpi koko spektrin punaisesta oranssin, keltaisen,
vihreän, sinisen ja violetin kautta takaisin punaiseen.
Kolmannessa esimerkissä on oranssin ja keltaisen välinen liuku peilauksena
toistuvasti.

Neljännessä suorakulmiossa sateenkaariliuku on laitettu täytön sijaan reunaviivan
väriksi.

{: .figure-medium }
> ![Neljä erilaista lineaarista liukuväriä](../inkscape-varit-lineaarinen_liuku.png)

Lineaarista liukuväriä luotaessa pitää ensimmäiseksi varmistaa, että
sen asetuspalkista on uuden liukuvärin tyypiksi valittuna lineaarinen
eli "suora liukuväri". Toinen tärkeä valittava asia on, sovelletaanko
liukuväriä kohteen täyttöön vai reunaan.

Alla olevassa kuvassa on valittuna suora lineaarinen liuku kohteen täyttöön.

{: .figure-normal }
> ![Suora liuku kohteen täyttöön](../inkscape-liukuvari-tyyppi_ja_kohde.png)

Seuraavaksi liukuvärityökalulla piirretään valittuun kohteeseen
liukuvärin suunta. Painetaan hiiren nappi pohjaan aloituskohdassa, 
vedetään ja päästetään nappi ylös lopetuskohdassa.

{: .figure-medium }
> ![Suora liuku kohteen täyttöön](../inkscape-liukuvari-lineaarinen_luonti.png)

Luotava liukuväri näkyy reaaliaikaisesti luomisen aikana. On myös tärkeää
muistaa valita haluttu kohde ennen liukuvärin tekemistä, jotta se kohdistuu
oikeaan kohteeseen. Oletuksena liukuväri muodostuu kohteessa jo olevasta väristä
täysin läpinäkyvään.

Liu'un aloituspiste näkyy neliökahvana ja lopetuspiste pyöreänä kahvana.
Kumpaakin voi liikuttaa liu'un luomisen jälkeen. Päätepisteiden värit
voi vaihtaa valitsemalla halutun päätepisteen ja sen jälkeen värin.

{: .figure-medium }
> ![Päätepisteen väri vaihdettu läpinäkyvästä punaiseksi](../inkscape-liukuvari-varin_vaihto.png)

Liukua esittävään viivaan voi lisätä *pysähdyspisteitä* eli *stop-pisteitä* joko kaksoisklikkaamalla
haluttua kohtaa hiirellä tai painamalla asetuspalkin plus-nappia.

Lisättyä pysähdyspistettä voi liikutella hiirellä pitkin liukua ja
sille voidaan valita haluttu väri.

{: .figure-medium-row }
> ![](../inkscape-liukuvari-stop_pisteen_lisays-1.png)
> ![](../inkscape-liukuvari-stop_pisteen_lisays-2.png)
> ![](../inkscape-liukuvari-stop_pisteen_lisays-3.png)
> ![](../inkscape-liukuvari-stop_pisteen_lisays-4.png)

Liukuvärityökalun ollessa käytössä, asetuspalkissa on valittavissa pudotusvalikosta
kaikki dokumentissa jo käytössä olevat lukuvärit. Tämän etuna
on se, että jos samaa liukuväriä halutaan käyttää useammassa
kohdassa piirrosta, sitä ei tarvitse määritellä jokaiseen kohtaan
erikseen ja jos liukuväriä haluaa muokata, se muokkautuu samalla
muokkauksella kaikkialle, missä kyseistä liukua on käytetty.

{: .figure-normal }
> ![Päätepisteen väri vaihdettu läpinäkyvästä punaiseksi](../inkscape-liukuvari-pudotusvalikko.png)

Asetuspalkin "Toista"-pudotusvalikosta liu'ulle voi valita toiston tyypin.

Näistä *None*, eli "ei toistoa", tarkoittaa, että kaikki ennen aloituspistettä
on aloituspisteen väristä ja kaikki lopetuspisteen jälkeen on samaa väriä
kuin lopetuspiste.

*Reflected*, eli "peilattu", tarkoittaa, että kun jompi kumpi liu'un
määrittelevän janan pää on saavutettu, siitä jatketaan eteenpäin peilatussa
järjestyksessä yhä uudelleen.

Kolmas vaihtoehto *Direct*, eli suora, tarkoittaa, että liukua toistetaan
ilman peilausta.

Alla esimerkkit liukuväristä ilman toistoa, peilatulla toistolla ja suoralla toistolla.

{: .figure-medium }
> ![Liukuvärin toiston eri tyypit esimerkkeinä](../inkscape-liukuvari-toisto.png)

Pysäytyspisteitä voi valita, siirtää, lisätä ja poistaa myös asetuspalkista.

{: .figure-normal }
> ![Pysähdyspisteiden valinta, lisääminen ja poisto asetuspalkissa](../inkscape-liukuvari-asetuspalkki_stops.png)

Liukuvärin pysähdyspisteitä voi muokata myös "Täyttö ja reunaviiva" -dialogissa.
Huomaa, että nyt täytön tyypiksi on valittuna suora liukuväri.
Kaikki liukuvärin pysäytyspisteet ovat siirreltävissä janalla ja niiden väriä voi
muuttaa vapaasti valitsemalla vasemmalta pysäytyspiste ja oikealta
haluttu värisävy ja peittävyys.

{: .figure-normal }
> ![Liukuvärin muokkaus täyttö ja reunaväri -dialogissa](../inkscape-liukuvari-fill_and_stroke.png)

## Säteittäinen liukuväri

Säteittäinen liukuväri toimii muuten samalla tavalla kuin suora liukuväri,
mutta suoran suunnan sijaan väri muuttuu säteittäisesti keskipisteestä alkaen.

{: .figure-medium }
> ![Esimerkkejä säteittäisestä liukuväristä](../inkscape-liukuvari-sateittainen.png)

Kun säteittäistä liukuväriä luodaan, säädettävissä on neliökahvalla merkitty
liu'un keskipiste ja pyöreillä kahvoilla merkityt kaksi toisiaan vastaan kohtisuoraa
akselia. Akselien pituudet ovat toisistaan riippumattomasti valittavissa,
mutta niiden suunnat ovat toisiinsa lukitut.

{: .figure-medium }
> ![Säteittäisen liukuvärin piirtäminen](../inkscape-liukuvari-sateittainen_piirtaminen.png)

Muuten säteittäisen väriliukuvärin luonti ja muokkaus tapahtuu aivan samoin kuin
suorankin liukuvärin. Säteittäiseksi liukuväriksi voi halutessaan valita saman pudotusvalikosta
valmiiksi jo löytyvän liu'un, jota on käytetty jo jossain muussa kohteessa suorana.
Valinta suoran tai säteittäisen asettelun välillä on kohdekohtainen.

Myös säteittäiseen liukuväriin voi valita samalla tavalla toiston ja peilaavan toiston
kuin suoraan liukuväriin. Samoin säteittäistä toistoa voi käyttää myös reunavärinä.

{: .figure-medium-row }
> ![Säteittäinen toisto peilaamalla](../inkscape-liukuvari-sateittainen_toisto.png)
> ![Säteittäinen toisto peilaamalla reunassa](../inkscape-liukuvari-sateittainen_reuna.png)

Piirretään esimerkkinä liukuvärien käytöstä tämä varjostettu pallo.

{: .figure-medium-row }
> ![Varjostettu sininen pallo](../inkscape-liukuvari-varjostettu_pallo.png)
> ![Varjostettu sininen pallo liukutyökalu näkyvissä](../inkscape-liukuvari-varjostettu_pallo-2.png)
