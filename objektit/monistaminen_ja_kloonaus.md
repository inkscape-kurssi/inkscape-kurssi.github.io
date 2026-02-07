---
date: "2026-01-31T11:20:00+03:00"
title: "Monistus ja kloonaus"
layout: default
nav_order: 1
parent: Objektit
---

# Monistus ja kloonaus

Kun piirto-alueella on jokin objekti, siitä saatetaan haluta
useita kopioita. Kopioiden luomiseen on olemassa kaksi tapaa
jotka eroavat toisistaan siinä, tehdäänkö kopiointi
kertaluonteisesti niin, että objektit ovat tämän jälkeen
itsenäisesti muokattavia, vai halutaanko niiden välillä pitää
kytkös niin, että yhtä muokattaessa toinenkin muuttuu.

## Monistaminen

Objektista voi tehdä toisen täsmälleen samanlaisen kopion
muistakin ohjelmista tutulla tavalla: "kopioi" ja "liitä".
Nämä löytyvät "Muokkaa"-valikosta ja niiden pikanäppäiminä
ovat tutut *Ctrl-c* ja *Ctrl-v*. Tuttu "Leikkaa" toiminto,
jonka pikanäppäin on *Ctrl-x*, toimii myös.

Liittäminen tapahtuu hiiren osoittimen kohdalle niin, että
osoitin on keskellä uutta objektia.

Inkscapessa on kuitenkin myös nopeampi tapa *monistaa*
objekti. "Muokkaa"-valikosta löytyvä komento "Monista"
tekee valituista objekteista välittömästi kopion samaan
paikkaan, jossa alkuperäinen on ja valitsee sen.
Tämän pikanäppäin on *Ctrl-d*, joka tulee sanasta "duplicate".

Monistaminen löytyy myös yläreunan komentopalkista.

{: .figure-normal }
> ![Komentopalkin napit](../inkscape-duplikaatti-napit.png)

Monistamisen etuna objektin kopiointiin on se, että
kopio sijaitsee samassa paikassa kuin alkuperäinen, jolloin
se voidaan siirtää esimerkiksi nuolinäppäimillä tarkasti.
Myös useampien kopioiden luonti ja sijoittelu on helppoa
monistamalla.

{: .figure-medium-row }
> ![Alkuperäinen hymynaama](../inkscape-duplikaatti-alkuperainen.png)
> ![Alkuperäinen hymynaama ja siitä monistetut kolme kopiota](../inkscape-duplikaatti-4_kopiota.png)
> ![Neljä alkuperäistä hymynaama](../inkscape-duplikaatit-4_alkuperaista.png)
> ![12 hymynaama](../inkscape-duplikaatit-12_hymynaamaa.png)

Kolmas keino tehdä kopioita objektista on *välilyönnin* painaminen
samalla, kun objektia siirretään valintatyökalulla. Tämä "pudottaa"
siirrettävästä objektista kopion siihen kohtaan, jossa ollaan.

{: .figure-normal }
> ![Siirron matkalla pudotettuja hymynaaman kopioita](../inkscape-duplikaatti-pudotus.png)

Luodut kopiot ovat kaikki toisistaan irrallisia objekteja, joita voidaan muokata kutakin
erikseen.

{: .figure-normal }
> ![Alkuperäinen hymynaama sekä venytetty ja värjätty kopio.](../inkscape-duplikaatti-muokkaus.png)

## Kloonit

*Kloonaus* on toinen tapa tehdä kopio alkuperäisestä objektista.
Kloonauksessa alkuperäisen objektin ja sen kloonin välillä säilyy kytkös.
Alkuperäisen objektin muokkaaminen muokkaa myös sen kloonia.
Myös *"Kloonaa"* löytyy "Muokkaa"-valikosta ja sen pikanäppäin on *Alt-d*.

Myös kloonaaminen ja sen purku löytyvät komentopalkista.

{: .figure-normal }
> ![Komentopalkin napit](../inkscape-duplikaatti-napit.png)

Alla olevissa kuvissa ensimmäisessä on alkuperäinen hymynaama ja sen klooni.
Toisessa venytetään alkuperäistä ja kolmannessa myös klooni on saanut saman
venytetyn muodon. Neljännessä alkuperäiseen on lisätty nenä, joka on
ilmestynyt myös kloonille.

{: .figure-medium-row }
> ![Alkuperäinen ja kloonattu hymynaama](../inkscape-klooni-alkuperainen_ja_klooni.png)
> ![Venytetään alkuperäistä](../inkscape-klooni-alkuperaisen_venytys.png)
> ![Myös klooni on venynyt](../inkscape-klooni-venytetyt.png)
> ![Alkuperäiseen on lisätty nenä](../inkscape-klooni-nena_lisatty.png)

Huomattavaa on, että kloonin muuttaminen ei vaikuta alkuperäiseen. Eli, jos
esimerkiksi kloonin kokoa muutetaan, silloin alkuperäinen ja klooni ovat
eri kokoiset, mutta jos nyt muutetaan alkuperäistä, siihen tehdyt muutokset
heijastuvat taas klooniin.

Seuraavissa kuvissa on ensin muunnettu kloonin hymynaaman koko pienemmäksi
ja muoto pyöreämmäksi. Alkuperäinen on edelleen venynyt. Kun alkuperäinen
muotoillaan taas pyöreäksi, kloonin muoto muuttuu samassa suhteessa.

{: .figure-medium-row }
> ![](../inkscape-klooni-pienennetty_klooni.png)
> ![](../inkscape-klooni-klooni_seuraa.png)

Kloonaus on erityisen kätevää silloin, jos kuvassa pitää olla useita samanlaisia
objekteja ja niitä halutaan muokata piirtämisen aikana.
Jos tällaisessa tilanteessa tehtäisiin monistamalla esimerkiksi
30 kappaletta samanlaisia objekteja ja sitten objektia haluttaisiinkin
muuttaa, pitäisi sama muutos tehdä jokaiseen kopioon taikka poistaa
ne ja tehdä kopiointi uudelleen.

**Huomioitavaa!** Jos klooneja monistetaan, ne ovat myös alkuperäisen
objektin klooneja. Siis samanlaisia kuin klooni, josta ne monistetaan.

## Asettamaton väri

Jossain tilanteessa voi olla järkevää tehdä alkuperäisestä objektista
pohja, joka ei ole mukana itse kuvassa vaan vain mallina,
jonka klooneja varsinaisessa kuvassa mukana olevat objektit ovat.
Alkuperäinen voidaan vaikka siirtää piirtoalueella valkoisen varsinaisen
kuva-alueen ulkopuolelle pois näkyvistä.

Jos klooneihin halutaan erilaisia värejä, tällöin kannattaa alkuperäisen
objektin vastaavaksi väriksi valita "asettamaton", eli "unset fill".
Tämän voi tehdä vasemman alakulman täyttövärin päältä hiiren
oikealla napilla tulevalla valikolla. Asettamaton vaihtoehto on
käytettävissä sekä täyttövärille että reunavärille.

{: .figure-normal }
> ![Valitaan täyttöväriksi "asettamaton".](../inkscape-klooni-unset_fill.png)

Asettamaton väri näkyy mustana.

{: .figure-normal }
> ![Hymynaaman täyttövärinä "asettamaton".](../inkscape-klooni-asettamaton_vari.png)

Nyt, koska täyttöväri on asettamaton, voidaan klooneissa vastaava täyttöväri
tai reunaväri valita vapaasti ja niitä voidaan venytellä ja skaalata
halutulla tavalla.

{: .figure-normal }
> ![Väritetyt kloonit.](../inkscape-klooni-varitetyt_kloonit.png)

Koska kloonit ovat yhä kytköksissä alkuperäiseen objektiin, alkuperäisen
muokkaaminen muotoilee myös kloonit.

{: .figure-normal }
> ![Alkuperäistä objektia on muotoiltu.](../inkscape-klooni-varitetyt_kloonit-muokattu.png)

## Linkityksen purkaminen

Kytköksen alkuperäisen ja kloonatun objektin välillä voi myös purkaa.
Tämä tarkoittaa sitä, että linkityksen purkamisen jälkeen klooni
muuttuu tavalliseksi kopioksi, joka ei enää seuraa alkuperäiselle
objektille tehtyjä muutoksia. Purkaminen löytyy komentopalkista ja
"Muokkaa"-valikon "Kloonaa"-alavalikosta. Sen voi tehdä myös pikanäppäimellä
*Shift-Alt-d*.

{: .figure-normal }
> ![Komentopalkin napit](../inkscape-duplikaatti-napit.png)


## Laattakloonaus

Kun halutaan luoda kerralla useita kloonattuja kopioita ruudukon muotoon,
voidaan "Muokkaa"-valikon "Kloonaa"-alavalikosta valita "Luo laattaklooneja".
Tämä avaa dialogin, josta voi valita, montako riviä ja saraketta klooneja
luodaan sekä lukuisia eri välilehdeille jaoteltuja asetuksia, miten
kloonit luodaan.

{: .figure-medium-row }
> ![](../inkscape-klooni-laattaklooni-1.png)
> ![](../inkscape-klooni-laattaklooni-2.png)
> ![](../inkscape-klooni-laattaklooni-3.png)
> ![](../inkscape-klooni-laattaklooni-4.png)
> ![](../inkscape-klooni-laattaklooni-5.png)
> ![](../inkscape-klooni-laattaklooni-6.png)
> ![](../inkscape-klooni-laattaklooni-7.png)

Esimerkiksi ensimmäinen välilehti "Symmetria" antaa valita, minkälaisia
symmetriaoperaatioita (siirto, kierto, peilaus, siirtopeilaus) klooneille
tehdään. Toinen välilehti "Siirto" määrittelee sarakkeittain ja
riveittän tehtävät siirrot mahdollisine satunnaistuksineen.
Kolmannella välilehdellä voi muokata kloonien kokojen muutosta
sarakkeiden ja rivien mukaan.

Esimerkkikuvassa vasemman yläkulman hymynaama on kloonattu
6×6-ruudukoksi niin, että oikealle mentäessä jokaisessa
sarakkeessa korkeutta on venytetty 10 % edellisestä
ja jokaisessa rivissä alas mentäessä leveyttä on venytetty
10 % edellisestä.

{: .figure-normal }
> ![Komentopalkin napit](../inkscape-klooni-laattaklooni_6x6.png)
