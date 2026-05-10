---
date: "2026-01-30T12:33:00+03:00"
title: "Tekstin asettelu"
layout: default
nav_order: 2
parent: Teksti
---

# Tekstin asettelu

Usein ilmenee tarvetta asetella tekstiä muutenkin kuin vain
irrallisina sanoina tai tekstilaatikkoina.

Teksti saatetaan haluta kulkemaan jotain tiettyä reittiä, vaikka
kaarevaa polkua. Se saatetaan haluta jonkin muun kuvion sisään
tai kulkemaan palstalta toiselle. Näihin löytyvät Inkscapesta
tarvittavat toiminnot.

## Teksti polulle

Tarkastellaan tilannetta, jossa teksti "Kettu juoksi yli järven"
halutaan asetella kaarevalle polulle.

{: .figure-normal }
![Teksti ja polku](../inkscape-teksti-teksti_ja_polku.png)

Valitaan ensin teksti ja sitten polku, jolle teksti halutaan ja lopuksi
"Teksti"-valikosta kohta "Aseta polulle".

{: .figure-normal }
![Teksti-valikossa "Aseta polulle"](../inkscape-teksti-valikosta_teksti_polulle.png)

Seurauksena teksti asettuu polulle alkaen polun alkupäästä, koska teksti oli
vasemmalle tasattu.

{: .figure-full }
![Teksti polulla alkaen polun alusta](../inkscape-teksti-teksti_polulla-1.png)

Jos teksti halutaankin keskelle polkua, pitää aloittaa alusta. Ennen tekstin
asettamista polulle, valitaan tekstiobjekti ja tekstityökalulla valitaan
sille keskitetty asettelu. Keskitetty asettelu näkyy myös valitussa
tekstiobjektissa, kun tekstityökalu on käytössä, pienenä neliönä keskellä tekstiä.
Tämä pieni neliö on objektin *"ankkuri"*, eli se kohta, josta se on kiinnitetty
piirtoalueeseen. Kullakin objektilla on aina ankkuri. Vasemmalle keskitetyn
tekstin ankkuri on vasemmassa alakulmassa, oikealle keskitetyn oikeassa alakulmassa.

{: .figure-full }
![Teksti "Kettu juoksi yli järven" keskitettynä](../inkscape-teksti-kettu_keskitetty.png)

Nyt tehdään polulle asettaminen uudelleen ja huomataan, että keskitetyn tekstin
ankkuri asettuu keskelle polkua.

{: .figure-full }
![Teksti keskellä polkua](../inkscape-teksti-teksti_polulla-2.png)

Tekstin sijaintia polulla voidaan hienosäätää tekstityökalulla "kerning"-asetuksilla
joko asetuspalkin hienosäätövalikosta tai nuolinäppäimillä.

Asetetaan tekstikursori tekstin alkuun ja painetaan *Alt*-näppäin pohjassa *nuolta
ylöspäin*. Silloin kaikki kursorin jäkeen tuleva teksti siirtyy paikaltaan
ylöspäin. Vastaavasti tekstiä voidaan siirtää omalta paikaltaan alas, oikealle ja
vasemmalle.

{: .figure-medium-row }
> ![Teksti keskellä polkua nostettuna](../inkscape-teksti-teksti_polulla-3.png)
> ![Teksti keskellä polkua laskettuna ja siirrettynä oikealle](../inkscape-teksti-teksti_polulla-4.png)

Tehdyt hienosäädöt voi nollata asetusvalikosta:

{: .figure-normal }
![Tekstin hienosäätöasetukset numeerisina](../inkscape-teksti-kerning.png)

Jos tekstin haluaakin kulkemaan polun toista puolta, voi valita polun ja
"Polku"-valikosta kohdan "Käännä". Tämä vaihtaa polun kulkusuunnan
päinvastaiseksi. Eli polun entinen alkupiste muuttuukin päätepisteeksi ja
päinvastoin.

{: .figure-normal }
![Tekstin polun toisella puolella](../inkscape-teksti-teksti_polulla-5.png)

Jos näkyviin halutaan vain kaareva teksti ilman polkuviivaa, voidaan valita
polku ja ottaa siltä pois reunaväri. Silloin polku on edelleen olemassa
piirtoalueella, mutta se ei näy, koska sillä ei ole reuna- eikä täyttöväriä.

{: .figure-normal }
![Pelkkä kaareva teksti](../inkscape-teksti-teksti_polulla-6.png)

Polun muotoa voidaan myös muokata, jolloin teksti seuraa polun uutta muotoa.

{: .figure-normal }
![Teksti muokatulla polulla](../inkscape-teksti-teksti_polulla-7.png)

Teksti voidaan luonnollisesti asetella myös muilla objekteille, kuten
ympyrälle tai monikulmiolle.

{: .figure-medium-row }
> ![Teksti ympyrällä](../inkscape-teksti-teksti_ympyralla.png)
> ![Teksti pentagonilla](../inkscape-teksti-teksti_pentagonilla.png)


## Teksti kehykseen

Tekstiobjektin sisällön voi sijoittaa toiseen piirto-objektiin, esimerkiksi
ympyrään, ellipsiin, suorakulmioon tai vapaaseen polkukuvioon.

Ensin valitaan sijoitettava teksti, sen jälkeen valitaan kuvio, johon se
halutaan sijoittaa ja lopuksi "Teksti"-valikosta kohta "Vie kehykseen".
Pikanäppäin tälle toiminnolle on *Alt-W*.

Tämä toiminto asettelee tekstin toisen objektin sisään niin, että se
myötäilee objektin reunoja. Sisällä oleva teksti on edelleen muokattavaa
ja muotoiltavaa tekstiä. Jos objektia, jonka sisään teksti on sijoitettu,
muokataan, teksti rivittyy muutoksen mukaan uudelleen.

**Huomattavaa:** Kannattaa varmistaa, että tekstiobjekti on sivulla
kehysobjektin päällä. Jos nämä ovat väärässä järjestyksessä, kehys
peittää tekstin näkyvistä. Objektien järjestystä voi vaihtaa vielä
tekstin kehykseen viennin jälkeenkin.

{: .figure-medium-row }
> ![Tekstilaatikko ja ympyrän sektori valittuina](../inkscape-teksti-teksti_ja_sektori.png)
> ![Teksti aseteltuna sektorin sisään](../inkscape-teksti-teksti_sektorissa.png)
> ![Teksti aseteltuna sektorin sisään ja lisätään tilaa tekstin ympärille](../inkscape-teksti-teksti_sektorissa-padding.png)
> ![Teksti aseteltuna sektorin sisään ja sektoria on muotoiltu](../inkscape-teksti-teksti_sektorissa-muokattu.png)


## Teksti palstoissa

Kun teksti sijoitetaan kehykseen, kehyksiä voi olla useampia. Tämä mahdollistaa
tekstin juoksuttamisen palstalta toiselle.

Alla olevissa kuvissa esitetään, miten sivulle on luotu kolme suorakaidetta
tarvittaviksi palstoiksi sekä tekstilaatikko, jossa on haluttu teksti.

Ensin valitaan teksti sekä kaikki kolme palstalaatikkoa halutussa järjestyksessä.
Sen jälkeen valitaan "Teksti"-valikosta kohta "Vie kehykseen". Tämä asettaa tekstin
kulkemaan laatikosta toiseen palstoina. Lopuksi lisätään tekstityökalulla tekstille
vähän tyhjää tilaa ympärille. Viimeinen vaihe ei ole tarpeen, jos laatikot
ovat esimerkiksi valkoisia ja niiden välissä on jo valmiiksi riittävästi tilaa.

{: .figure-medium-row }
> ![Tekstilaatikko ja kolme suorakulmiota valittuina](../inkscape-teksti-teksti_ja_laatikot.png)
> ![Teksti aseteltuna suorakulmioihin palsoiksi](../inkscape-teksti-teksti_laatikoissa.png)
> ![Teksti aseteltuna palsoihin ja lisätään tilaa tekstin ympärille](../inkscape-teksti-teksti_laatikoissa-padding.png)
> ![Teksti aseteltuna palstoihin valmiina](../inkscape-teksti-teksti_laatikoissa-valmis.png)


{: .exercises }
> Lataa alla oleva SVG-tiedosto (hiiren oikealla napilla "Tallenna kohde levylle")
> ja avaa se Inkscapella. Tiedosto sisältää harjoitustehtäviä, joilla harjoitellaan
> tekstin asettelua polulle ja kehykseen.
> 
> [Harjoitus - Tekstin asettelu](/files/harjoitus-tekstiasettelu.svg)
