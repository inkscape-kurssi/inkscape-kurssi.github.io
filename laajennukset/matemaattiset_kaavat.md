---
date: "2026-03-15T17:30:00+03:00"
title: "Matemaattiset kaavat"
layout: default
nav_order: 5
parent: Laajennukset
---

# Matemaattiset kaavat

Jos Inkscapella halutaan piirtää matematiikan tai fysiikan
havainnollistuskuvia, tulee hyvin nopeasti vastaan
tilanne, että kuvaan pitää saada myös matemaattisia kaavoja.
Tätä varten Inkscapeen löytyy enemmän kuin yksi laajennos.

Oletuksena Inkscapen asennuksessa ovat mukana laajennukset
"Formula (pdflatex)" ja "Formula (typst)". Nimensä mukaisesti
näistä ensimmäinen vaatii toimiakseen, että tietokoneelle
on asennettuna jokin LaTeX-kielen kääntäjä ja toinen vaatii
toimiakseen typst-kielen kääntäjän. Kolmantena vaihtoehtona
on "TexText" -laajennus, joka ei välttämättä tule Inkscapen mukana,
ja joka vaatii myöskin toimiakseen
LaTeX-kääntäjän. "TexText" on näistä kuitenkin suositeltavin,
sillä se mahdollistaa myös kaavojen muokkaamisen.

Nämä kaikki laajennukset löytyvät "Laajennukset"-valikon
"Teksti"-alivalikosta.

## Formula (pdflatex)

"Formula (pdflatex)" -laajennus avaa pienen dialogi-ikkunan,
jossa kysytään luotava kaava LaTeX-kielen mukaisena sekä
kirjasinkoko.

{: .figure-normal }
![Formula (pdflatex)](../inkscape-laajennukset-formula_pdflatex.png)

Kun "Apply"-nappia painetaan, laajennus suorittaa tietokoneelle
asennetun LaTeX-ohjelmiston komennon `pdflatex` ja antaa sille syötteeksi
pyydetyn kaavan sisältävän tiedoston. Komennon tuloksesta laajennus
poimii taitetun kaavan ja tekee siitä ryhmäksi koostetun joukon
polkuja johonkin kohtaa piirtoaluetta. Lopputuloksena oleva kaava
on visuaalisesti kaunis. Ainoana puutteena on, että jos kaavaa
pitää muokata, pitää käytännössä luoda uusi kaavaobjekti.

{: .figure-normal }
![pdflatexilla tuotettu kaava](../inkscape-laajennukset-kaava_pdflatex.png)


## Formula (typst)

Typst on uudempi vaihtoehtoinen tapa kirjoittaa matematiikkaa sisältäviä
asiakirjoja. Typst pyrkii olemaan yksinkertaisempi ja selkeämpi
kuin LaTeX. Joissain tapauksissa LaTeXin matematiikkatuki
on ilmeisesti vielä laajempi.

Jos Typst on asennettuna koneelle, laajennus avaa samantapaisen
dialogin kuin sen LaTeX-versio ja käyttäjältä kysytään kaava
ja kirjasinkoko. Tällä kertaa kaava syötetään Typst-kielen
mukaisessa muodossa.

{: .figure-normal }
![Formula (typst)](../inkscape-laajennukset-formula_typst.png)

Laajennus tuottaa kaavan samaan tapaan kuin sen pdflatex-versio.

{: .figure-normal }
![Typst:illa tuotettu kaava](../inkscape-laajennukset-kaava_typst.png)

Typst-käännintä käytettäessä kannattaa huomioida, että Ubuntu-järjestelmissä
snap-pakettina asennettu Typst voi tuottaa hieman ongelmia
tietoturva-asetustensa vuoksi.


## TexText

[TexText](https://textext.github.io/textext/) on edellisiä selvästi
monipuolisempi lisäosa matemaattisten kaavojen luomiseen
ja muokkaamiseen.

{: .figure-normal }
![TexText](../inkscape-laajennukset-textext_dialogi.png)

TexText sisältää yksinkertaisen tekstieditorin, jossa
on myös synktaksin korostus LaTeX-kaavoille. Kääntäjäohjelmaksi
voi valita joko `pdflatex`-, `xelatex`- tai `luatex`-kääntäjän
sekä uudemmissa versioissa myös `typst`-kääntäjän.

Lopputulosta pystyy esikatselemaan laajennuksen omassa ikkunassa
ennen sen tallentamista asiakirjaan.

{: .figure-normal }
![TexTextillä tuotettu kaava](../inkscape-laajennukset-kaava_textext.png)

TexTextin suurin etu on, että se tallentaa myös käytetyn raakamuotoisen
kaavan tekemäänsä objektiin, joten se kykenee myös avaamaan
kaavan muokattavaksi. Kun TexTextillä luotu objekti on valittuna
ja laajennus käynnistetään uudelleen, kaavaa voi muokata ja tallennus
korvaa aiemman objektin.

Ohjeet TexTextin asentamiseen löytyvät sen [omilta sivuilta](https://textext.github.io/textext).
Ohjeet kuvaavat sen asentamisen niin Windows-, Linux- kuin MacOS-tietokoneeseenkin.
Kaikki vaihtoehdot edellyttävät, että järjestelmään on jo asennettuna
tarvittava LaTeX- tai Typst-kielen kääntäjä.

**Huomio!** Jos Inkscape on asennettuna Ubuntu-järjestelmään
(tai johonkin muuhun Linux-järjestelmään) käyttäen snap- tai flatpak-pakettia,
TexText-laajennuksen käyttäminen ei todennäksisesti onnistu.
Tämä johtuu snap- ja flatpak-paketointien käyttämästä
"hiekkalaatikoinnista", joka estää Inkscapea suorittamasta
ulkopuolisia ohjelmistoja, kuten `pdflatex`ja `typst`.