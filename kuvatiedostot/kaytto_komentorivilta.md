---
date: "2026-01-31T11:20:00+03:00"
title: "Käyttö komentoriviltä"
layout: default
nav_order: 6
parent: Kuvatiedostot
---

# Käyttö komentoriviltä

Sen lisäksi, että Inkscapella voidaan piirtää kuvia graafisesti,
sitä on mahdollista käyttää myös komentoriviltä käsin.
Komentoriviä käyttämällä on mahdollista esimerkiksi muuntaa
tiedostoja tyypistä toiseen ja viedä osia tiedostosta
"Vie"-toiminnolla.

Komentorivin hyödyllisyys tulee esiin siinä, että näin
Inkscapen voima voidaan skriptauksella integroida osaksi
jotain suurempaa prosessia.

Esimerkiksi Inkscapella voidaan piirtää yhteen asiakirjaan
jonkin pelin kortit taikka nappulat ja automatisoida
yksittäisten korttitiedostojen luonti ilman, että niitä tarvitsee
viedä käsin jokaisen muokkauksen jälkeen.

## Koko kuvan vienti

Komentorivillä komento alkaa aina ohjelman nimellä, eli ensimmäisenä on
`inkscape`. Sen jälkeen tulee välilyönnillä eroteltuna joukko erilaisia
optioita ja niiden argumentteja sekä lopuksi avattavan tiedoston nimi
taikka useamman tiedoston nimet.

Käsitellään esimerkkinä seuraavaa SVG-kuvaa.

{: .figure-medium }
![Vektorikuva keltaisesta linnusta](../lintu1.svg)

Seuraava komento avaa SVG-kuvan `lintu1.svg` ja
vie sen tiedostoksi `lintu1.png`. Luotavan kuvan leveydeksi (width)
asetetaan 200 pikseliä.

```bash
inkscape -o lintu1.png -w 200 lintu1.svg
```

Optiot voi komentorivillä antaa myös pidemmässä muodossa.

```bash
inkscape --export-filename=lintu1.png --export-width=200 lintu1.svg
```

Molemmilla tavoilla lopputuloksena on 200 pikseliä leveä PNG-kuva.

{: .figure-normal }
![Vektorikuva keltaisesta linnusta](../lintu1.png)

Inkscapelle voi antaa vietäväksi myös useampia SVG-kuvia kerralla.

```bash
inkscape --export-type=png -w 200 lintu1.svg lintu2.svg lintu3.svg lintu4.svg
```

Tämä komento kertoo vietävien kuvien tyypiksi `png` ja leveydeksi 200 pikseliä.
Käsiteltäviä kuvia on nyt neljä kappaletta. Luotavien PNG-kuvien
nimiksi otetaan alkuperäisten SVG-kuvien nimet, mutta `png`-päätteellä.

{: .figure-normal-row }
> ![Vektorikuva keltaisesta linnusta](../lintu1.png)
> ![Vektorikuva ruskeasta linnusta](../lintu2.png)
> ![Vektorikuva vaaleanpunaisesta linnusta](../lintu3.png)
> ![Vektorikuva sinisestä linnusta](../lintu4.png)


## Kuvan osan vienti

Tarkastellaan seuraavaksi SVG-tiedostoa, jossa on shakkilaudan kaikkien
nappuloiden kuvat vektorikuvina.

{: .figure-medium }
![Shakkinappulat](../shakki.svg)

Varmistetaan, että kukin nappula on SVG-tiedostossa nimettynä, jotta
niihin voidaan viitata komentorivillä.

{: .figure-normal }
![Shakkinappulat SVG:nä ja kukin nappula nimetynä](../inkscape-cli-shakkinappulat.png)

"Tasot ja Objektit" -dialogista nähdään, että kutakin nappulaa edustavalle
objektiryhmälle on annettu kuvaavat nimet. Lisätään ryhmille vielä vastaavat
nimet niiden ID:iksi. Valitaan esimerkiksi musta kuningatar, valitaan valikosta
"Kohde" ja "Kohteen ominaisuudet" tai pikanäppäin *Shift-Ctrl-O*.

{: .figure-normal }
![Mustan kuningattaren ominaisuudet](../inkscape-cli-kohteen_ominaisuudet.png)

Vaihdetaan kunkin nappulan ominaisuuksiin kyseisen ryhmän ID:ksi nappulan
nimi. Nyt SVG-tiedoston lähdekoodissa on kyseisten ryhmien `<g>`-tageissa
`id`-attribuutti, jonka arvona on kyseisen nappulan nimi.

```xml
  <g
     id="musta_kuningatar"
     transform="matrix(0.31655,0,0,0.31655,1288.1446,402.61781)"
     inkscape:label="musta_kuningatar">
    <path
       id="path5428"
       style="color:#000000;fill:#000000;stroke:#525252;stroke-width:0.19909"
       d="m -1952.8,-1199.4 c -17.1,0 -30.9,13.8 -30.9,30.9 0,2.1 0.2,4.2 0.6,6.2 h -99.8 c -1.6,0.4 -2,1.3 -1.6,2.8 l 50.2,175.83 h 11.9 c -2.5,3.36 -4.1,7.52 -4.2,12.03 -0.2,7.87 4.1,14.65 10.5,18 h -5.3 c -11.2,0 -20.4,9.04 -20.7,20.25 -0.2,8.92 5.4,16.44 13.3,19.16 h -7.5 c -13.4,0 -24.4,10.77 -24.7,24.16 -0.3,13.38 10.2,24.18 23.6,24.18 h 16.4 c 29.6,28.44 9.6,225.89 -17.9,246.41 -2,1.79 -2.7,1.1 -3.2,2.78 l -1.3,56.94 c -16.9,0.3 -30.6,13.95 -31,30.87 -0.3,12.08 6.3,22.51 16.3,27.6 h -18.7 c -1.5,0 -2.8,1.22 -2.8,2.75 l -1.4,62 c -0.1,1.52 1.2,2.75 2.7,2.75 h 252.2 c 1.5,0 2.8,-1.23 2.8,-2.75 l 1.4,-62 c 0,-1.53 -1.2,-2.75 -2.7,-2.75 h -21 c 10.2,-5.09 17.2,-15.52 17.5,-27.6 0.4,-16.54 -12.2,-29.97 -28.5,-30.84 l 1.3,-56.97 c 0,-0.65 -0.2,-1.25 -0.6,-1.72 -20,-15.99 -56.4,-216.44 -29.3,-247.03 -0.1,-0.15 -0.1,-0.29 -0.2,-0.44 h 14.6 c 13.4,0 24.4,-10.8 24.7,-24.18 0.3,-13.39 -10.3,-24.16 -23.7,-24.16 h -9.7 c 8,-2.72 13.9,-10.24 14.1,-19.16 0.2,-11.21 -8.6,-20.25 -19.8,-20.25 h -5.4 c 6.6,-3.35 11.2,-10.13 11.4,-18 0.1,-4.51 -1.3,-8.67 -3.7,-12.03 h 13.4 l 50.3,-175.83 c 0.4,-1.7 -0.1,-2.8 -2,-2.8 h -101.3 c 0.4,-2 0.6,-4.1 0.6,-6.2 0,-17.1 -13.8,-30.9 -30.9,-30.9 z" />
...
```

Nyt voidaan komentoriviltä käsin viedä SVG-kuvasta vain haluttu objekti
uuteen tiedostoon.

```bash
inkscape --export-id=musta_ratsu -o musta_ratsu.png -w 100 shakki.svg
```

Myös ID:n mukaan vietäessä voidaan viedä samalla kertaa useampi
kuva luettelemalla useampi ID. ID:t kirjoitetaan lainausmerkkien
sisään luettelona puolipisteillä eroteltuina. Tiedostojen nimeksi laitetaan aluperäisen
tiedoston nimi ilman päätettä, alaviiva ja sen perään vietävän kohteen
ID sekä valitun tiedostotyypin pääte. Esimerkiksi `shakki_musta_lahetti.png`.

```bash
inkscape --export-id="valkoinen_lahetti;musta_lahetti;valkoinen_torni;musta_torni" --export-type=png -w 50 shakki.svg
```

Tuloksena on neljä kuvaa.

{: .figure-normal }
> ![Valkoinen lähetti](../shakki_valkoinen_lahetti.png)
> ![Musta lähetti](../shakki_musta_lahetti.png)
> ![Valkoinen torni](../shakki_valkoinen_torni.png)
> ![Musta torni](../shakki_musta_torni.png)

Jos SVG-kuvassa on useita objekteja ja kuvaan halutaan vain yksi
ID:llä valittu objekti ilman esimerkiksi taustalla
olevia objekteja, komentoon voidaan lisätä `--export-id-only`, joka
varmistaa että kuvaan ei tule muita samalla alueella olevia
kohteita.

{: .figure-normal }
> ![Lintukortti](../lintukortit.svg)

```bash
inkscape --export-id="keltainen_lintu" --export-type=png -w 100 lintukortit.svg
inkscape --export-id-only --export-id="keltainen_lintu" --export-type=png -w 100 lintukortit.svg
```

Edellä olevista komennoista ensimmäinen vie tiedostoon keltaisen linnun
sekä sen takana olevan siniset taivaan. Jälkimmäinen vain linnun ilman taivasta.

{: .figure-normal }
> ![Lintu taivaalla](../lintukortit_keltainen_lintu.png)
> ![Lintu ilman taivasta](../lintukortit_keltainen_lintu_vain.png)

## Kuvan vienti koordinaateilla

Vietävän alueen voi määritellä myöskin suoraan koordinaatteina
optiolla `--export-area=x0:y0:x1:y1`. Tässä `x0` ja `y0` ovat
vietävän alueen vasemman yläkulman koordinaatit ja `x1` sekä `y1`
alueen oikean alakulman koordinaatit. Origo on kuvan vasemmassa
yläkulmassa ja koordinaatit kasvavat oikealle ja alas.

```bash
inkscape --export-area=30:40:230:140 -o lintu-alue.png lintukortit.svg
```

Yllä oleva komento tuottaa kuvan:

{: .figure-normal }
> ![Koordinaateilla leikattu viety kuva](../lintu-alue.png)


## Vienti muihin tiedostomuotoihin

Viedään linktukortin kuva [PDF-tiedostoksi](../lintu.pdf) ja [EPS-tiedostoksi](../lintu.eps):

```bash
inkscape -o lintu.pdf lintukortit.svg
inkscape -o lintu.eps lintukortit.eps
```

## Muut optiot

Lisää komentorivitoiminnoista voi opiskella englanniksi
[dokumentaatiosta](http://wiki.inkscape.org/wiki/index.php/Using_the_Command_Line).

Kaikki Inkscapen komentorivioptiot saa esiin optiolla `--help`:

```bash
inkscape --help

Usage:
  org.inkscape.Inkscape [OPTION…] file1 [file2 [fileN]]

Process (or open) one or more files.

Help Options:
  -?, --help                                  Show help options
  --help-all                                  Show all help options
  --help-gapplication                         Show GApplication options
  --help-gtk                                  Show GTK+ Options

Application Options:
  -V, --version                               Tulosta Inkscape:n versionumero
  --debug-info                                Print debugging information
  --system-data-directory                     Print system data directory
  --user-data-directory                       Print user data directory
  --list-input-types                          List all available input file extensions
  --app-id-tag                                Create a unique instance of Inkscape with the application ID 'org.inkscape.Inkscape.TAG'
    
Tuo tiedosto:                        
  -p, --pipe                                  Read input file from standard input (stdin)
  -n, --pages=PAGE[,PAGE]                     Page numbers to import from multi-page document, i.e. PDF
  --pdf-poppler                               Use poppler when importing via commandline
  --pdf-font-strategy=STRATEGY                How fonts are parsed in the internal PDF importer [draw-missing|draw-all|delete-missing|delete-all|substitute|keep]
  --convert-dpi-method=METHOD                 Method used to convert pre-0.92 document dpi, if needed: [none|scale-viewbox|scale-document]
  --no-convert-text-baseline-spacing          Do not fix pre-0.92 document's text baseline spacing on opening
    
View tiedosto:                       
  -o, --export-filename=FILENAME              Output file name (defaults to input filename; file type is guessed from extension if present; use '-' to write to stdout)
  --export-overwrite                          Overwrite input file (otherwise add '_out' suffix if type doesn't change)
  --export-type=TYPE[,TYPE]*                  File type(s) to export: [svg,png,ps,eps,pdf,emf,wmf,xaml]
  --export-extension=EXTENSION-ID             Extension ID to use for exporting
    
Vie geometria:                       
  -C, --export-area-page                      Vietävä alue on sivu
  -D, --export-area-drawing                   Vietävä alue on koko piirustus (sivukokoa ei huomioida)
  -a, --export-area=x0:y0:x1:y1               Area to export in SVG user units
  --export-area-snap                          Snap the bitmap export area outwards to the nearest integer values
  -d, --export-dpi=DPI                        Resoluutio bittikarttooille ja rasteroitaville suotimille; oletusarvo on 96
  -w, --export-width=LEVEYS                   Bittikarttan leveys pikseleinä (ohittaa --export-dpi)
  -h, --export-height=KORKEUS                 Bittikarttan leveys pikseleinä (ohittaa --export-dpi)
  --export-margin=MARGIN                      Margin around export area: units of page size for SVG, mm for PS/PDF
    
Viennin asetukset:                   
  --export-page=all|n[,a-b]                   Page number to export
  -i, --export-id=OBJECT-ID[;OBJECT-ID]*      ID(s) of object(s) to export
  -j, --export-id-only                        Hide all objects except object with ID selected by export-id
  -l, --export-plain-svg                      Poista Inkscape kohtaiset SVG ominaisuudet
  --export-ps-level=LEVEL                     Postscript taso (2 tai 3); Oletusarvo on 3
  --export-pdf-version=VERSION                PDF version (1.4 or 1.5); default is 1.5
  -T, --export-text-to-path                   Muunna kaikki teksti poluiksi tallennettaessa (PS, EPS, PDF ja SVG)
  --export-latex                              View teksti erillisenä LaTeX-tiedostona (PS, EPS, PDF ja SVG)
  --export-ignore-filters                     Renderöi kohteet ilman suotimia niiden rasteroinnin sijaan (PS, EPS ja PDF)
  -t, --export-use-hints                      Use stored filename and DPI hints when exporting object selected by --export-id
  -b, --export-background=VÄRI                Bittikartan taustaväri (mikä tahansa SVG:n ymmärtämä väri)
  -y, --export-background-opacity=ARVO        Bittikartan taustan peittävyys. (joko välillä 0,0 - 1,0 tai 1 - 255)
  --export-png-color-mode=COLOR-MODE          Color mode (bit depth and color type) for exported bitmaps (Gray_1/Gray_2/Gray_4/Gray_8/Gray_16/RGB_8/RGB_16/GrayAlpha_8/GrayAlpha_16/RGBA_8/RGBA_16)
  --export-png-use-dithering=false|true       Force dithering or disables it
  --export-png-compression=LEVEL              Compression level for PNG export (0 to 9); default is 6
  --export-png-antialias=LEVEL                Antialias level for PNG export (0 to 3); default is 2
    
Query object/document geometry:      
  -I, --query-id=OBJECT-ID[,OBJECT-ID]*       ID(s) of object(s) to be queried
  -S, --query-all                             Print bounding boxes of all objects
  -X, --query-x                               X coordinate of drawing or object (if specified by --query-id)
  -Y, --query-y                               Y coordinate of drawing or object (if specified by --query-id)
  -W, --query-width                           Width of drawing or object (if specified by --query-id)
  -H, --query-height                          Height of drawing or object (if specified by --query-id)
    
Edistynyt tiedostojen käsittely:     
  --vacuum-defs                               Poista käyttämättömät määritykset asiakirjan <defs>-osiosta
  --select=OBJECT-ID[,OBJECT-ID]*             Valitut kohteet: pilkuilla erotelty ID-tunnusten luettelo
                                          
  --actions=ACTION(:ARG)[;ACTION(:ARG)]*      List of actions (with optional arguments) to execute
  --action-list                               List all available actions
  --actions-file=FILENAME                     Use a file to input actions list
    
Käyttöliittymä:                      
  -g, --with-gui                              With graphical user interface (required by some actions)
  --batch-process                             Close GUI after executing all actions
                                          
  --shell                                     Start Inkscape in interactive shell mode
  -q, --active-window                         Use active window from commandline
  --display=DISPLAY                           X display to use


Esimerkit:
  Export input SVG (in.svg) to PDF (out.pdf) format:
        inkscape --export-filename=out.pdf in.svg
  Export input files (in1.svg, in2.svg) to PNG format keeping original name (in1.png, in2.png):
        inkscape --export-type=png in1.svg in2.svg
  See 'man inkscape' and http://wiki.inkscape.org/wiki/index.php/Using_the_Command_Line for more details.
```