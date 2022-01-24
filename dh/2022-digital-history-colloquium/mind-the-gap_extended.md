---
title: "Mind the `<gap/>`!"
subtitle: "Digital Humanities und das kulturelle Erbe des Globalen Südens"
author: Till Grallert
affiliation: Orient-Institut Beirut
bibliography: /BachUni/applications/applications.csl.json
lang: de
date: 2021-03-04
duration: 25
---


## Title slide

Till Grallert, Orient-Institut Beirut (OIB), @[tillgrallert](https://twitter.com/tillgrallert)

Probevortrag

Slides: [https://tillgrallert.github.io/slides/dh/2021-mind-the-gap](https://tillgrallert.github.io/slides/dh/2021-mind-the-gap/index.html)

## Übersicht des Probevortrages

1. Mind the `<gap/>`!
2. Closing the `<gap/>` one step at the time

# 1. Mind the `<gap/>`! Zwischen Heilsversprechen und Realität
## Zwischen Heilsversprechen und Realität

::: {.c_width-50 .c_left}

### egalitäres Heilsversprechen

- jede kann ohne Unterschied teilhaben
- uneingescheränkter Zugang zum Wissen der Welt

### Normative Grundlagen

- Wissen = Daten = Verständnis
- mehr Wissen = besseres Verständnis
- Solutionism, Technokratie

:::
::: {.c_width-50 .c_right}

### ernüchternde Realtität

- universale, wenn auch unterschiedliche Ausschlußerfahrungen

### Elefant in the room

- Digitalität wird als **voraussetzungslos** verstanden

:::

## Metaphermaschinen

::: {.c_width-50 .c_left}

- Digitalität **simuliert** Vertrautheit und Stasis
    + Metaphern
    + semantische Modelle
- Digitalität ist hochgradig ephemer und wird kontinuierlich remediiert

:::
::: {.c_width-50 .c_right}

![Google docs](../..//assets/dh/google-docs.png){#fig:google-docs}

:::

## Mind the `<gap/>`! Zugangsvorraussetzungen

...  müssen explizit gemacht werden!

::: {.c_width-50 .c_left}

### technisch

+ Hardware: aktuell
+ Strom: kontinuierlich
+ Internet: schnell und stabil
+ Software

:::
::: {.c_width-50 .c_right}

### kulturell

+ Sprach- und Schriftkenntnisse
+ Vertrautheit mit den Metaphern
+ Vertrautheit mit semantischen Modellen

:::

## Mind the `<gap/>`! Zwischen Globalem Norden und Globalem Süden

::: {.c_width-50 .c_left}

### Globaler Norden

- Hegemon
- Autor der technischen und kulturellen Standards der Digitalität

:::
::: {.c_width-50 .c_right}

### Globaler Süden

- nicht homogen, kein universeller "Anderer"
- Vielzahl heterogener Regionalitäten
- gemeinsame Erfahrung der konstanten Auseinandersetzung mit dem Hegemon

:::

|                 |   Globaler Norden    |    Globaler Süden    |
+-----------------+----------------------+----------------------+
| Hardware        | Designer             | Benutzer             |
| Software        | Designer             | Benutzer             |
| Standards       | Designer             | Benutzer             |
| Schrift/Sprache | lokal                | fremd                |
| Finanzierung    | reichlich, lokal     | eingeschränkt, fremd |
| Instituionen    | reichlich            | eingeschränkt        |
| Internet        | schnell, verlässlich | langsam, unbeständig |
| Elektrizität    | verlässlich          | unbeständig          |

## Digital Humanities als Teil des Globalen Nordens

![Globale Verteilung von [DH Zentren](http://dhcenternet.org/centers)](../../assets/maps/map_dhcenters.png)

## technische Zugangsvorraussetzungen


+--------------------+------------------------------------------+--------------------------------+
|                    |                 Weltweit                 |            Libanon             |
+====================+==========================================+================================+
| Computer Hardware  | - Internetcafé                           |                                |
|                    | - Telefon                                |                                |
+--------------------+------------------------------------------+--------------------------------+
| Stomversorgung     | + 2018: 89,6%                            | - 3h/ Tag reg. Stromausfall    |
|                    | + Afrika: 20 Länder unter 43%            | - teure Generatorenabonnements |
+--------------------+------------------------------------------+--------------------------------+
| Internetverbindung | + 2019: knapp 4 Mrd. Menschen (c.51,4 %) | - 15 Mbps für ein Institut     |
|                    |                                          | - mobil: 60 USD für 20 GB      |
+--------------------+------------------------------------------+--------------------------------+
| Software           | + Trend zu Abo-Modellen                  |                                |
+--------------------+------------------------------------------+--------------------------------+


<!-- 40 MB für einen Scan dauern mit 15 Mbps rechnerisch 21,33 Sek für den Download. Aber über VPN oder vor Ort teilen sich diese Leitung 20-40 Leute -->
<!-- außerdem fliege ich alle 200-300 MB aus dem SharePoint Volume -->

# Nicht-lateinische Schriften und Sprachen des Globalen Südens
## Ungleicher Zugang nach Sprache

### Englischkenntnisse sind <!-- für die Teilhabe --> unabdingbar

:::{.c_width-50 .c_left}

Englisch ist die Lingua Franca und Basis der technischen Infrastruktur

- Beispiel: CSS

```css
body {
    background: white;
    color: black;
}
```

- Beispiel: R

```R
library(tidyverse)
setwd("/path/to/folder/")
load("oape_stats.rda")
المجلات <- c("4770057679", "644997575", "472450345", "792756327")
المشار.اليها <- المشار.اليها %>%
    filter(source.id.oclc %in% المجلات)
write.table(المشار.اليها, file = "csv/oape_stats.csv", row.names = FALSE, quote = TRUE, sep = ",")
```

:::
:::{.c_width-50 .c_right}

Schriften und Sprachen des Globalen Nordens sind der Hegemon der Interfaces

![[Translatio Bonn](https://digitale-sammlungen.ulb.uni-bonn.de/ulbbnioa/periodical/titleinfo/3384757?lang=en): Englisches Interface (gelb), Arabisch in deutscher Umschrift (lila), Deutsch (grün).](../../assets/OpenArabicPE/translatio_interface-languages_annotated.png){#fig:translatio-interface}

:::

## Arabisch

:::{.c_width-50 .c_left}

### Schrift

- zweithäufigste Schrift <!-- nach lateinischer Schrift -->
+ aktuell für 14 Sprachen verwendet, u.a. Arabisch, Persisch, Urdu, Pashtu.
+ Schriftrichtung von rechts nach links
+ Buchstaben werden mehrheitlich in Schreibrichtung verbunden und ändern dabei ihre Form:  [ج جـ ـجـ ـج]{.c_rtl}
+ Präferenz für Ligaturen

:::
:::{.c_width-50 .c_right}

### Sprache

+ fünfthäufigeste Sprache
    * eine von sechs Amtssprachen der UN
    + <!-- offizielle --> Amtssprache in 26 Ländern
    * \>420 Mio. Sprechende
+ liturgische Sprache des Islams mit 1,6 Mrd. Gläubigen

:::

![Beispiel: "Amerika und die arabischen Gelehrten". [*al-Muqtabas* 2(1)](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_13.TEIP5.xml#div_8.d1e1249)](../../assets/dh/arabic-script_sample-annotated.png){#fig:arabic-sample}

## Arabisch in der Digitalität
### Zum großen Teil <!-- von der digitalen Infrastruktur --> nicht unterstützt

+ Character encoding kann die kulturelle Praxis der Schreibenden nicht abbilden
+ Abstraktion in Buchstaben / Gleichsetzung von Graphemen mit Buchstaben ist zumindest umstritten
+ Notwendige Verbindungsformen der Buchstaben werden der Rendering Engine überlassen
+ OCR ist nicht funktional

<!-- hello Java, I am looking at you! -->
<!-- add screenshot of tweet writing Arabic in Latin -->

## Arabische Schrift: Character encoding
### Unicode is awesome but ...

:::{.c_width-50 .c_left}

<!-- - Vor Unicode lange Zeit gar nicht unterstützt -->
- Unicode ist ein <!-- in Mountain View ansässiges --> Industriekonsortium <!-- mit US-Dominanz -->
    + Full members: Adobe, Apple, Facebook, Google, IBM, Microsoft, Netflix, SAP, Salesforce, **Sultanat von Oman**
- Encodings <!-- sind politische Entscheidungen und --> folgen Sprachen, nicht Schriften
- OS, Browser etc. normalisieren die Varianz nicht.
<!-- - Notwendige Verbindungsformen der Buchstaben werden der Rendering Engine überlassen -->
- Folge: Volltextsuchen sind nicht aussagekräftig

:::
:::{.c_width-50 .c_right}

![32 Varianten von "mekkanisch" (مكية). Quelle: Thomas Milo *Patterns of confusability* 2014.](../../assets/dh/arabic-script_unicode-example-makkiyya.png){#fig:arabic-mecca-1}

![Browsersuche nach "مك" im Wikidataeintrag für Mekka ([Q5806](https://www.wikidata.org/wiki/Q5806))](../../assets/dh/arabic-script_unicode-example-wikidata_narrow.png){#fig:arabic-mecca-2 height="300px"}

:::

## Rendering: basale Standards werden nicht unterstützt

### Beispiel 1: Werbung (Grafik- und Layout Programme)

:::{.c_width-50 .c_left}

<!-- Nicht verbunden und von rechts nach links -->

!["Arabische" Werbung Abstand zu halten um sich und andere vor Covid-19 zu schützen, Washentaw County, Health Department. Quelle: <https://twitter.com/2awbi2atiye/status/1347351918268489728>](../../assets/dh/ErLBbWwVgAErjHy.jpg){#fig:arabic-fail-covid}

:::
:::{.c_width-50 .c_right}

<!-- Korrektur -->

![Korrigierte Fassung nachdem Twitternutzer_innen auf die Fehler hinwiesen. Quelle: <https://twitter.com/wcpublichealth/status/1347622725469130752>](../../assets/dh/ErO3qtUVkAEUAQ_.jpg){#fig:arabic-fail-covid-corrected}

:::

<!-- ![Die schwedischen Liberalen in ihrer Selbstbeschreibung (franz., arab.). Quelle: https://pbs.twimg.com/media/DmB222GXoAEyBux](../../assets/dh/DmB222GXoAEyBux.jpg)   -->

## Rendering: basale Standards werden nicht unterstützt
### Beispiel 2: Webbrowser und HTML 5

Das browsereigene CSS ignoriert das HTML5 Attribut `@lang` und stellt Arabisch linksbündig dar

:::{lang="ar"}
كانت أمريكا مجهولة عند أبناء القرن الخامس عشر بدليل أن المؤرخين في ذلك العهد لم يذكروا عنها سوى أخبار اكتشافها في أواخر ذلك القرن غير أن كلام ايراتوستينيس واسترابون اليونانيين اللذين عُنيا بفن الجغرافيا بنحو ٢٠٠ سنة ق. م. يستدل منه على أن القدماء كانوا يتحدثون بوجود قارة مجهولة في أيامهم.
:::

:::{.c_width-30}
![Chrome](../../assets/dh/html5-lang_ar-chrome-2.png){#fig:arabic-fail-chrome}
:::

:::{.c_width-30}
![Firefox](../../assets/dh/html5-lang_ar-firefox-2.png){#fig:arabic-fail-firefox}
:::

:::{.c_width-30}
![Safari](../../assets/dh/html5-lang_ar-safari-2.png){#fig:arabic-fail-safari}
:::

# Digitalisierung des Kulturerbes
## Digitalisierung des Kulturerbes

:::{.c_width-50 .c_left}

### Erfassung

Digitalisierung ist **teuer**: public-private partnerships, private vendors

+ Findet primär im Globalen Norden statt
+ Kuratorische Entscheidungen
    + Sammlung
    + Katalogisierung
    + Digitalisierung
+ Technische Entscheidungen
    * Workflows, Modelle, Ontologien des Nordens
+ Wirtschaftliche Entscheidungen
    * Outsourcing

:::
:::{.c_width-50 .c_right}

### Bereitsstellung

Platformen zur Maximierung des Gewinns

+ Proprietäre Interfaces
+ Datensilos ohne APIs
+ Bezahlschranken
+ geo-fencing

:::

## Digitalisierung des Kulturerbes

![Karte von in Worldcat und ArUC erfassten Beständen der Zeitschrift *al-Muqtabas*](../../assets/OpenArabicPE/maps/map-holdings_al-muqtabas-vol_1-9.png){#fig:map-global-holdings}

## Digitalisierung des Kulturerbes: Bezahlschranken und Geo-fencing

:::{.c_width-50 .c_left}

![*al-Muqtabas* 6 auf [HathiTrust](http://hdl.handle.net/2027/njp.32101073250910) außerhalb der USA](../../assets/OpenArabicPE/hathi_muqtabas-1.png){#fig:hathi-muqtabas-global}

:::
:::{.c_width-50 .c_right}

![*al-Muqtabas* 6 auf [HathiTrust](http://hdl.handle.net/2027/njp.32101073250910) mit US IP](../../assets/OpenArabicPE/hathi_muqtabas-2.png){#fig:hathi-muqtabas-us}

:::

## Digitalisierung des Kulturerbes: OCR Schichten

:::{.c_width-50 .c_left}

![OCR Schicht für *al-Muqtabas* 6 auf [HathiTrust](http://hdl.handle.net/2027/njp.32101073250910) (mit US IP)](../../assets/OpenArabicPE/hathi_muqtabas-ocr-3.png)

:::
:::{.c_width-50 .c_right}

![OCR Schicht für *al-Bashīr* 9 Jan. 1880 (#487), S.1 auf [GPA](https://gpa.eastview.com/crl/mena/newspapers/bshr18800109-01.1.1)](../../assets/OpenArabicPE/gpa_bashir-i_487-p_1_ocr.png)

:::



<!-- hier muss noch was zu den verscheidenen Gaps hin -->

## Mind the `<gap/>`

- Infrastruktur
- Werkzeuge
- Wissen

# 3. Closing the `<gap/>`: mein Beitrag zu den *digital commons*
# 3.1 <!-- Wissenslücke/  -->Knowledge gap: Project Jarāʾid (2012--)
## [Project Jarāʾid](https://projectjaraid.github.io/)

<!-- - Addressiert den **knowledge gap** mit einer Webseite und offenen Datensätzen (TEI XML). -->

:::{.c_width-50 .c_left}

- Bibliographische Erfassung sämtlicher arabischer Periodika seit ihrer Entstehung um 1800 bis 1930.
    + Webseite und offene Datensätzen (TEI XML)
    + Normdatensätze für c.2700 Personen, 220 Orte, 180 Bibliotheken u.ä.
- Kollaboration mit Adam Mestyan (Duke)

:::
:::{.c_width-50 .c_right}

![Neu gegründete arabisch-sprachige Periodika, 1799--1929](../../assets/jaraid/map-jaraid_1850-1929_world.gif){#fig:map-jaraid}

:::

## [Project Jarāʾid](https://projectjaraid.github.io/)
### Wissenslücke -> Digitalisierungslücke

:::{.c_width-50 .c_right}
![In Project Jarāʾid erfasste Periodika](../../assets/jaraid/jaraid_holdings_pie-3.png){#fig:jaraid-stats}
:::

:::{.c_width-50 .c_left}

|                  | number  | %     |
| ---------------- | ------: | ----: |
| Periodika        | 3269    |       |
| in Bibliotheken  | 747     | 22.85 |
| digitalisiert    | 145     | 4.44  |

<!-- Table: In Project Jarāʾid erfasste Periodika {#tbl:jaraid-stats} -->
:::

# 3.2 Infrastructural gap: Open Arabic Periodical Editions (OpenArabicPE, 2015--) <!-- digitisation bias  -->
## corpus building: [Open Arabic Periodical Editions](https://openarabicpe.github.io)

1. Ideen:
    - Verbindung **vorhandener** Faksimiles und Transkriptionen in einem standardkonformen, offenen Format
    - Scraping, Erzeugung, Validierung und Teilen von offenen bibliographischen Metadaten
2. Ziele
    + **Validierung** der Transkriptionen
    + Iterative und kollaborative **Verbesserungen** der Editionen
    + Alles soll dauerhaft **zitierbar** und **verlinkbar** sein
    + Verbesserte Zugänglichkeit und Nachnutzung durch **offene Lizenzen**
3. Prinzipien
    - Weiternutzung **vorhandener** und **etablierter** Werkzeuge und Technologien
    - Präferenz für **offene** und **einfache** Formate und Werkzeuge

## corpus building: [Open Arabic Periodical Editions](https://openarabicpe.github.io)

:::{.c_width-50 .c_left}

1. Digitale Editionen: TEI XML.
1. Offene Lizenzen: [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/) (TEI, MODS, BibTeX), MIT license (XSLT, XQuery)
2. Soziale digitale Editionen, die auf [GitHub](https://github.com/openarabicpe) gehostet sind: <!-- gradually improve transcription and mark-up -->
2. Veröffentlichungen werden auf [Zenodo](https://zenodo.org) archiviert: DOI für dauerhafte Referenzierbarkeit
3. [Statische Webansichten](https://github.com/openarabicpe/tei-boilerplate-arabic-editions)<!--  (doesn't require a permanent internet connection) -->: Parallele Darstellung von Text und Faksimile.
4. Bibliographische Metadaten sind als öffentliche [Zotero-Gruppe](https://www.zotero.org/groups/openarabicpe) gehostet

:::
:::{.c_width-50 .c_right}

![[Webansicht von *al-Muqtabas* 6(2)](https://openarabicpe.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_61.TEIP5.xml)](../../assets/OpenArabicPE/boilerplate_muqtabas.png){#fig:webview-muqtabas}

:::

## OpenArabicPE: Korpus

| Periodikum                                                                        | DOI                                                              | Bände | Ausgaben | Artikel | Wörter   | Wörter/Artikel |
| :--------                                                                         | :--                                                              | ----: | ----:    | ----:    | ----:   | ----:             |
| [al-Ḥaqāʾiq](https://www.github.com/openarabicpe/digital-haqaiq)              | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) | 3     | 35       | 389      | 298090  | 832.66            |
| [al-Ḥasnāʾ](https://www.github.com/openarabicpe/journal_al-hasna)             | [10.5281/zenodo.3556246](https://doi.org/10.5281/zenodo.3556246) | 1     | 12       | 201      | NA      | NA                |
| [al-Manār](https://www.github.com/openarabicpe/journal_al-manar)                  |                                                                  | 35    | 537      | 4300     | 6144593 | 1437.73           |
| [al-Muqtabas](https://www.github.com/tillgrallert/digital-muqtabas)           | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   | 9     | 96       | 2964     | 1981081 | 873.34            |
| [al-Ustādh](https://www.github.com/openarabicpe/journal_al-ustadh)                | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) | 1     | 42       | 435      | 221447  | 582.21            |
| [al-Zuhūr](https://www.github.com/openarabicpe/journal_al-zuhur)                  | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) | 4     | 39       | 436      | 292333  | 695.09            |
| [Lughat al-ʿArab](https://www.github.com/openarabicpe/journal_lughat-al-arab) | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) | 3     | 34       | 939      | 373832  | 485.21            |
| **total**                                                                         |                                                                  | 56    | 795      | 9664     | 9311376 |                   |

Table: Übersicht über das Periodikakorpus {#tbl:openarabicpe-corpus}


# 3.3 Tool gap: OCR/HTR für arabische Periodika (2019--)
## Traditionelle Ansätze

- Ziel: Buchstaben- und Worterkennung
- Ansatz: Segmentierung, Erkennung
- Probleme:
    + Buchstaben werden **mehrheitlich** in Schreibrichtung verbunden
    + Positionsabhängige Buchstabenformen
    + Ambivalente Buchstabenformen
    + Präferenz für Ligaturen ![](../../assets/dh/arabic-script_sample_short.png)
- Resultat:

![Evaluierung von OCR Software für Arabisch, [@Alghamdi.Teahan+2017+ExperimentalEvaluationArabic, table IV]](../../assets/dh/arabic-ocr_alghamdi-2017-table-iv_annotated.png){#fig:alghamdi-2018-table-4}

## Neue Ansätze mit maschinellem Lernen

- Ansatz: Word spotting und Lernen
- Vorteile:
    + Segmentierung nicht notwendig
    + Eingabe- und Ausgabeschrift müssen nicht die gleiche sein
    + Offene Software
- Nachteile
    + Training benötigt potentiell sehr umfangreiches Ground Truth
    + Training von Schrift- und Sprachmodellen für jeden Font
    + Rechenintensiv

## Experiment: OCR für arabische Periodika

- Kollaboration mit Sinai Rusinek (Haifa)
- Software: Transkribus, Tesseract 4
- Ground Truth: OpenArabicPE Korpus
- Probleme:
    + Komplexes Layout
    + Software nimmt Links-nach-rechts als Leserichtung an
- Resultat:

| ID      | based on   | ground truth    | words   | lines  | epochs  | CER train  | CER validation        |
| ------- | ---------- | --------------- | ------: | -----: | ------: | ---------: | --------------:       |
| 15946   |            | *al-Ustādh*     | 192829  | 18732  | 200     | 2.01       | [2.09]{style="color:green;"} |
| 13864   |            | *al-Muqtabas*   | 11116   | 1013   | 200     | 0.07       | 8.40                  |
| 25211   | 15946      |                 | 5987    | 604    | 100     | 0.09       | 6.19                  |


## Experiment: Transkribus

:::{.c_width-50 .c_left}

![Transkribus: Evaluation des Modells #13864](../../assets/dh/transkribus/evaluation-modell_OpenArabic1.png){#fig:transkribus-evaluation}

:::
:::{.c_width-50 .c_right height="100%"}

![Seite aus dem Validierungssample mit "komplexem" Layout, *al-Muqtabas* 1(1), S.19](../../assets/dh/transkribus/oclc_4770057679-v_1-img_019.tif){#fig:muqtabas-1-1-19}

:::


# 4. Closing the `<gap/>`: digitale Methoden
# SIHAFA: Mapping the late Ottoman Ideosphere of the Eastern Mediterranean through Computational Approaches to its Periodical Press (2021?--)

## SIHAFA

:::{.c_width-30}

### Ziele:

+ systematische Erforschung der spätosmanischen arabischen Presse *at scale*
+ Entwicklung/Evaluation von digitalen Methoden
+ Hinterfragung etablierter Forschungsnarrative
+ Etablierung von "Arab Periodical Studies"

:::
:::{.c_width-30}

### Fragen

+ Wer sind die zentralen Akteure (Personen, Periodika) in diesem diskursiven Feld?
+ Wie sind Periodika produziert worden? Wie ist Autorenschaft zu denken?
+ Welche Rolle spielt *text reuse*? Wie reisten Texte, Themen, Genres?
+ Wie hat sich die Sprache der Moderne im multilingualen, imperialen Raum etabliert?

:::
:::{.c_width-30}

### Methoden

+ Netzwerkanalyse
+ stilometrische Autorenschaftbestimmung
+ historische GIS
+ Layoutanalyse
+ Topic modelling
+ Word embeddings

:::

## 1. Historisches GIS: Typologie der Periodika <!-- CUT -->

Hypothese: geographische Herkunft von Artikeln in einem Periodikum erlaubt Rückschlüsse über seine Bedeutung

:::{.c_width-30}

### trans-regional

![Karte der in den Autorenzeilen erwähnten Orte für  *al-Muqtabas* (Kairo und Damaskus)](../../assets/OpenArabicPE/maps/map-oclc_4770057679-bylines-middle-east.png){#fig:authors-muqtabas}

:::

:::{.c_width-30}

### regional

![Karte der in den Autorenzeilen erwähnten Orte für  *al-Ḥasnāʾ* (Beirut)](../../assets/OpenArabicPE/maps/map-oclc_792756327-bylines-middle-east.png){#fig:authors-hasna}

:::
:::{.c_width-30}

### lokal

![Karte der in den Autorenzeilen erwähnten Orte für  *al-Ḥaqāʾiq* (Damaskus)](../../assets/OpenArabicPE/maps/map-oclc_644997575-bylines-middle-east.png){#fig:authors-haqaiq}

:::


## Historisches GIS
### Voraussetzungen: Daten

:::{.c_width-50}

- Erste Quellen: OpenArabicPE
- Auszeichnung von Orten im modellierten Volltext
    + Autor_innenzeilen
    + Rezensionen
    + Probleme: kein funktionales arabisches NER
- Normdatensätze für die Disambiguierung und Anreicherung von Daten
    + Georeferenzierte Orte
    + Probleme: Mangel an historischen Ortsverzeichnissen (gazetteer)

:::
:::{.c_width-50}

```xml
 <byline>
    <placeName ref="oape:place:9 geon:268064">صيدا</placeName>
    <persName ref="oape:pers:2845">مريم زكا</persName>
</byline>
```

```xml
<place type="town" xml:id="place_9">
    <placeName type="simple">Saida</placeName>
    <placeName xml:lang="ar-Latn-x-ijmes">Ṣaydā</placeName>
    <placeName xml:lang="en">Sidon</placeName>
    <placeName xml:lang="ar">صيدا</placeName>
    <location>
        <geo>33.55751, 35.37148</geo>
    </location>
    <idno type="url">http://en.wikipedia.org/wiki/Sidon</idno>
    <idno type="geon">268064</idno>
    <idno type="oape">9</idno>
</place>
```

:::

## 2. Netzwerkanalyse: erwähnte Periodika

:::{.c_width-60 .c_left}

![Gerichtetes Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas* erwähnten Periodika; nach Ausgaben gewichtet. Größe und Farbe der Knoten: in-degree.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_referenced-periodicals-per-issue_circular-n-size_in-degree.svg){#fig:network-periodicals}

:::
:::{.c_width-30}

### Ziel

- empirische Überprüfung von Hypothesen
- Entscheidungshilfe für Digitalisierung

### Erste Ergebnisse

* hauptsächlich selbstreferentiell
* Typologie: Grad der Weltzugewandtheit
* Kernnetzwerk:
    * Überraschende Mitglieder
    - Hochgradig geographisch konzentriert <!-- (10 Orte) -->
<!--     - Bestätigt den Forschungsschwerpunkt auf Kairo und Beirut -->

:::


## Netzwerkanalyse: erwähnten Periodika
### Voraussetzungen: Daten

:::{.c_width-50}

- Erste Quellen: OpenArabicPE, Project Jarāʾid, OCR
- Auszeichnung aller Erwähnungen von Periodika im modellierten Volltext
    + semi-automatisch (regex): folgt dem Muster "Zeitung ABC", "Zeitschrift DEF"
    + Probleme: kein funktionales arabisches NER
- Normdatensätze für die Disambiguierung und Anreicherung von Daten
    + Bibliographie
    + Probleme: geringe Quote in vorhandenen Normdatensätzen

:::
:::{.c_width-50}
<!-- Zwei Ausschnitte, die verschiedene Periodika mit dem gleichen Titel (*al-Zuhūr*) erwähnen. -->

<!-- ägyptische Zeitschrift -->
```xml
والأصح الدرعية بلام التعريف (راجع <bibl subtype="journal" type="periodical">مجلة <title level="j" ref="oape:bibl:3 oclc:1034545644" xml:id="title_16.d2e2291">الزهور</title> المصرية  <biblScope unit="volume" from="2" to="2">٢</biblScope> :  <biblScope unit="page" from="292">٢٩٢</biblScope></bibl>)
```

<!-- irakische Zeitung -->
```xml
وانتخب <persName>فؤاد أفندي الدفتري البغدادي</persName> و<bibl><editor><persName>نوري أفندي</persName></editor> راس كتاب <textLang otherLangs="ota">القسم التركي</textLang> في <bibl type="periodical" subtype="newspaper">جريدة <title ref="oape:bibl:532">الزهور</title></bibl> البغدادية</bibl> نائبين عن <placeName ref="oape:place:372 geon:94824">كربلاء</placeName>.
```

:::

## 2. Netzwerkanalyse: Autor_innen

:::{.c_width-50}

![Ungerichtetes Netzwerk der Autor_innen in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas*. Farbe der Knoten: betweenness centrality; Größe der Knoten: Anzahl der Periodika; Breite der Kanten: Anzahl der Artikel.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_authors_unimodal-n-size_out-degree-n-colour_betweenness-e-colour_grey.png){#fig:network-authors}

:::
:::{.c_width-50}

### Ziel

- empirische überprüfung von Hypothesen
- Forschungsleitend für *close reading*

### Erste Ergebnisse

<!-- * Nur wenige Knoten sind von relativer Bedeutung (14 von 319) -->
* Sehr begrenzte Überschneidung zwischen Periodika aus der gleichen Stadt
* Kernnetzwerk:
    - praktisch nicht in der Forschung abgebildet
    - Überraschende Zusammensetzung: viele Iraker (6), wenige Syrer (2), wenige Christen (2)

:::

## Netzwerkanalyse: Autor_innen
### Voraussetzungen: Daten

:::{.c_width-50}

- Erste Quellen: OpenArabicPE, Project Jarāʾid
- Strukturierte bibliographische Daten
    + semi-automatisch auf Basis der Editionen
    + manuelle Erfassung
    + Probleme: viele Abkürzungen, vielfältige Namensformen
- Normdatensätze für die Disambiguierung und Anreicherung von Daten
    + Lebensdaten
    + Werke in Bibliothekskatalogen
    + Probleme: geringe Quote in vorhandenen Normdatensätzen

:::
:::{.c_width-50}

```xml
<person>
    <persName><roleName type="pseudonym">ساتسنا</roleName></persName>
    <persName><roleName type="pseudonym">أمكح</roleName></persName>
    <persName><roleName type="pseudonym">فهر الجابري</roleName></persName>
    <persName><roleName type="rank">الأب</roleName> <forename>أنستاس</forename> <forename>ماري</forename> <surname><addName type="nisbah">الكرملي</addName></surname></persName>
    <persName><forename>أنستاس</forename> <forename>ماري</forename> <addName type="nisbah">الألياوي</addName> <surname><addName type="nisbah">الكرملي</addName></surname></persName>
    <persName><forename>بطرس</forename> <addName type="nasab">بن <forename>جبرائيل</forename></addName> <forename>يوسف</forename> <surname>عواد</surname></persName>
    <idno type="VIAF">39370998</idno>
    <idno type="oape">227</idno>
    <idno type="wiki">Q4751824</idno>
    <birth><date source="viaf" when="1866-08-05">1866-08-05</date> in <placeName ref="oape:place:216 geon:98182">Baghdad</placeName></birth>
    <death><date source="viaf" when="1947-01-07">1947-01-07</date> in <placeName ref="oape:place:216 geon:98182">Baghdad</placeName></death>
</person>
```

:::

## Problem: Das Netzwerk der Autor_innen umfasst nur 17% aller Artikel

![ ](../../assets/clipart/iceberg-2070977_960_720.png){width="100%" height="100%"}

## Autorenschaftsbestimmung

:::{.c_width-50}

### Forschungsstand

- Die Frage der Autorenschaftsbestimmung ist weitgehend ignoriert worden  <!-- standard accounts don't even mention the issue -->
- Implizite und häufig angenommene Hypothese: die Herausgeber_innen haben alle anonymen Artikel selbst geschrieben

:::
:::{.c_width-50}

### Probleme

- Hypothese ist nicht überprüft
- Wir kennen gar nicht die Namen aller potentiellen Kandidat_innen <!-- (siehe Project Jarāʾid) -->
- Es ist sehr unwahrscheinlich, dass alles von einer Person verfasst wurde <!-- Autor als Funktion, nicht als Person zu denken -->

:::

## 3. Stilometrie zur Autorenschaftsbestimmung

- **komparative** Methode:
    + Vergleich **stylistischer Merkmale** (*most frequent words* MFWs) liefert ein nummerisches Abstandsmaß (Verschiedenheit)
    + Selbstvalidierung: Abstimmung der Ergebnisse mehrerer Iterationen mit verschiedenen Anzahlen von MFWs
- Ist bis jetzt nicht auf arabische Texte angewendet worden
- Herausvorderungen:
    + abhängig von der Zusammensetzung des Korpus
    + Texte müssen eine Mindestlänge haben

## Stilometrie: erste Experimente
### Falsifizierung der Hypothese

:::{.c_width-60 .c_left}

![Figure: *bootstrap consensus network* von Artikeln in *al-Muqtabas* (Länge >= 5000 Wörter, 100--1000 MFWs). Farbe:  *modularity group*](../../assets/OpenArabicPE/stylometry/stylo_oape-p3a6afa20_articles-w_5000-modularity_1-label_authors.svg){#fig:stylometry-muqtabas-w5000}

<!-- modularity group: members of the group have more connections among themselves than with other (groups of) nodes -->

:::
:::{.c_width-30}

- Stilometrie funktioniert für arabische Periodika
- <!-- Erfolgreich identifizierte  -->Signale für
    + Autorenschaft
    + Herausgeberschaft
    + Übersetzung
- Zusätzliches (Sub)-signal
    + Genre
<!-- - Falsifizierung der Hypothese: es gibt einen anonymen Autor, der nicht der Herausgeber ist -->

:::

<!-- - chunking/sampling beeinflusst die Ergebnisse
    + Anzahl der stylistische Merkmale: mehrere Iterationen stimmen ab
    + Textlänge: Minimum von 4000-5000 Wörtern für signifikante Ergebnisse -->

## Layoutanalyse

# Conclusio
## take home messages