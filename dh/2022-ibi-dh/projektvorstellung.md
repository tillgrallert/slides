---
title: "Zur Erschließung arabischer Periodika aus spätosmanischer Zeit"
subtitle: "Herausforderungen einer multilingualen und multiskriptoralen Digital History"
author: Till Grallert
affiliation: Digital History Berlin
bibliography: 
    - /BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /BachUni/applications/applications.csl.json
lang: de
date: 2022-01-26
# duration: 30
---


## Zur Erschließung arabischer Periodika aus spätosmanischer Zeit (c.1800--c.1920) <br/>Herausforderungen einer multilingualen und multiskriptoralen Digital History

Till Grallert, @[tillgrallert](https://twitter.com/tillgrallert)

*Digital History* – Offenes Forschungskolloquium  

26 Januar 2022

Folien: [https://tillgrallert.github.io/slides/dh/2022-digital-history-colloquium](https://tillgrallert.github.io/slides/dh/2022-digital-history-colloquium/index.html)

## Übersicht

1. Einführung
2. Mind the `<gap/>`! Digitalität zwischen Heilsversprechen und Realität
3. Mind the `<gap/>`! *Linguistic imperialism*
4. Mind the `<gap/>`! Digitalisierung des Kulturerbes
5. Versuche einer Digital History 
6. Schlussbemerkungen
<!-- 3. Closing the `<gap/>` one step at the time -->

# 1. Einführung
## Spätosmanischer östlicher Mittelmeerraum

:::{.c_width-60}

<!-- ![Das Osmanische Reich, 1893. [@map_ottoman-empire-1893]](../../assets/maps/map_Ottoman-Empire-1893_annotated.jpg){#fig:map-oem} -->

![Die administrative Struktur des Osmanischen Reiches, ca. 1899. AbdurRahman AbdulMoneim, CC BY-SA 4.0, via [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Ottoman_Empire_Administrative_Divisions.png)](https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Ottoman_Empire_Administrative_Divisions.png/2048px-Ottoman_Empire_Administrative_Divisions.png){#fig:map-oem}

:::
:::{.c_width-30}

- Norden: Rumelien und Anatolien
    + ab 14. Jhd. osmanisch
- Süden: *Mashriq* und Ägypten
    + ab 16. Jhd. osmanisch
- Modernisierendes Reich
    + *Tanzimat*: 1838--76
    + Erste konstitutionelle Phase: 1876--78
    + Jungtürkische Revolution: 24. Juli 1908
    + Zweite konstitutionelle Phase: 1908--18 
- Sezessionen, Einfluss europ. Kolonialmächte
    + Muslimisierung
    + Arabisierung

:::


## Arabische Zeitungen und Zeitschriften

:::{.c_width-50}

- Presse als zentraler Agent des Wandels in der Moderne
    + erstes Massenmedium
    + zentrales Medium der literarischen und kulturellen arabischen Renaissance (*nahḍa*)
    + Medium des Sprachwandels
    + zentrale Foren für Verhandlung von Moderne, Nationalismen, Islamismus etc.

:::
:::{.c_width-50}

- Presse bisher vor allem als Quelle genutzt und kaum als Gegenstand untersucht
- Forschung wird dominiert von
    + national(istisch)en Narrativen
    + Verengung auf zwei Orte und wenige <!-- allgemein zugängliche --> Titel
    + impliziten Hypothesen

:::

![Neu gegründete arabisch-sprachige Periodika, 1799--1929](../../assets/jaraid/map-periodicals_World_1855-1929_temp-dist-status-y_5.gif){#fig:map-jaraid}


## Computationelle Periodikastudien

:::{.c_width-50}

![Ungerichtetes Netzwerk der Autor_innen in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas*. Farbe der Knoten: betweenness centrality; Größe der Knoten: Anzahl der Periodika; Breite der Kanten: Anzahl der Artikel.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_authors_unimodal-n-size_out-degree-n-colour_betweenness.png){#fig:network-authors}

:::
:::{.c_width-50}

<!-- ![Orte in Autorenzeilen in *al-Ḥaqāʾiq* (Damaskus)](../../assets/OpenArabicPE/maps/map-oclc_644997575-bylines-middle-east-na_mapped.png){#fig:authors-haqaiq .c_height-50}

![Erscheinungsorte der in *al-Muqtabas* (Kairo und Damaskus) erwähnten Periodika](../../assets/OpenArabicPE/maps/map-oclc_4770057679-referenced-periodicals-med-na_mapped.png){#fig:referenced-periodicals-muqtabas .c_height-50} -->

![Karte der in Autor_innenzeilen erwähnten Orte in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas*](../../assets/OpenArabicPE/maps/map-data-set-bylines-middle-east-na_mapped-bar.png){#fig:map-bylines}

:::

## Computationelle Periodikastudien

:::{.c_width-50}

![Gerichtetes Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas* erwähnten Periodika; nach Ausgaben gewichtet. Größe und Farbe der Knoten: in-degree.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_referenced-periodicals-per-issue_circular-n-size_in-degree.png){#fig:network-periodicals}

:::
:::{.c_width-50}

![Karte der in Autor_innenzeilen erwähnten Orte in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas*](../../assets/OpenArabicPE/maps/map-data-set-referenced-periodicals-med-na_mapped.png){#fig:map-referenced}

:::

## Notwendige Datenbasis

:::{.c_width-30}

### Modellierten Volltext mit Auszeichnung von *Named Entities*

+ z.B. "In ihrer letzten Ausgabe berichtete die Zeitung *al-ʿAṣr al-Jadīd* aus Damaskus, dass ..."
+ (halb)automatische Extraktion basiert auf
    * named entity recognition (NER)
+ Probleme
    * Zustand von OCR und Layout-Erkennung
    * Zustand von NER

:::
:::{.c_width-30}

### Strukturierte bibliographische (Meta)daten auf der Artikelebene

+ z.B. "*Sātisnā* schickte uns diesen Artikel aus *al-Shahbāʾ*"
+ (halb)automatische Extraktion basiert auf
    * Anwesenheit der Information im materiellen Artefakt
    * einem modellierten digitalen Surrogat
+ Probleme
    * Vielfalt von Namensformen

:::
:::{.c_width-30}

### Normdatensätze <!-- zur Disambiguierung und Anreicherung der Daten -->

- *Sātisnā*
    + Pseudonym und Anagram für *Anastās al-Karmilī*, den Herausgeber von *Lughat al-ʿArab* in Bagdad
- *al-Shahbāʾ*, "die Graue"
    + ein Beiname von Aleppo
    + Geokoordinaten: `36.20124, 37.16117`
- Probleme
    + enormes Bias auf den Globalen Norden

:::




## Linguistic imperialism [@Phillipson1997RealitiesAndMyths]: Arabisch

:::{.c_width-50}

### Schrift

- zweithäufigste Schrift <!-- nach lateinischer Schrift -->
    + aktuell für 14 Sprachen verwendet, u.a. Arabisch, Persisch, Urdu, Pashtu.
+ Schriftrichtung von rechts nach links
+ Buchstaben (Grapheme) werden mehrheitlich in Schreibrichtung verbunden und ändern dabei ihre Form (Allographen):  [ج جـ ـجـ ـج]{.c_rtl lang="ar"}
+ Grapheme bestehen aus Basisformen (Archigraphem, *rasm*) und diakritischen Zeichen (*iʿjām*)
* Vokalisierung (*tashkīl*) **kann** hinzugefügt werden und hat Einfluss auf Bedeutung

:::
:::{.c_width-50}

### Sprache

+ fünfthäufigste Sprache
    * eine von sechs Amtssprachen der UN
    + <!-- offizielle --> Amtssprache in 26 Ländern
    * \>420 Mio. Sprechende
+ liturgische Sprache des Islams mit 1,6 Mrd. Gläubigen

:::

![Beispiel: [@oclc_4770057679-i_13-div_8.d1e1249]](../../assets/dh/arabic-script_sample-annotated.png){#fig:arabic-sample-1}

## Arabisch in der Digitalität
### Zum großen Teil <!-- von der digitalen Infrastruktur --> nicht unterstützt

:::{.c_width-50 .c_left}

+ Zeichenkodierung lange Zeit nicht unterstützt
    * <!-- Konsequenz aus dem Buchdruck, Schreibmaschinen etc.:  -->Latinisierte Umschriften
    * "gelehrte" Umschrift vs Praxis des Arabisi
    * Unicode löst das Problem nicht
+ <!-- Notwendige --> Allographen (Verbindungsformen) werden der Rendering Engine überlassen
+ OCR ist nicht funktional*

<!-- + Abstraktion in Buchstaben ist zumindest umstritten
    + Zeichkodierung kann die kulturelle Praxis der Schreibenden nicht abbilden -->

:::
:::{.c_width-50 .c_right}
:::{.c_rtl}

### أميركا وعلماء العرب

[كانت أميركا مجهولة عند ابنآء القرن الخامس عشر بدليل ان المؤرخين في ذلك العهد لم يذكروا عنها سوى اخبار اكتشافها في أواخر ذلك القرن]{.c_rtl lang="ar"}

<cite>[@oclc_4770057679-i_13-div_8.d1e1249]</cite>

:::
:::{.c_ltr}

### Amīrkā wa ʿulamāʾ al-ʿarab

*Kānat Amīrkā majhūla ʿinda abnāʾ al-qarn al-khāmis ʿashr bi-dalīl anna al-muʾarikhīn fī dhalika al-ʿahd lam yadhkarū ʿanhā siwā akhbār iktishāfihā fī awākhir dhalika al-qarn*

Umschrift (IJMES)

:::
:::


## Darstellung <br/>basale Standards werden nicht unterstützt
### Beispiel 1: Werbung (Grafik- und Layout Programme)

:::{.c_width-50}

<!-- Nicht verbunden und von rechts nach links -->

!["Arabische" Werbung Abstand zu halten um sich und andere vor Covid-19 zu schützen, Washentaw County, Health Department. Quelle: [Twitter](https://twitter.com/2awbi2atiye/status/1347351918268489728)](../../assets/dh/ErLBbWwVgAErjHy.jpg){#fig:arabic-fail-covid}

:::
:::{.c_width-50}

<!-- Korrektur -->

![Korrigierte Fassung nachdem Twitternutzer_innen auf die Fehler hinwiesen. Quelle: [Twitter](https://twitter.com/wcpublichealth/status/1347622725469130752)](../../assets/dh/ErO3qtUVkAEUAQ_.jpg){#fig:arabic-fail-covid-corrected}

:::

# Projekte
## Open Arabic Periodical Editions ([OpenArabicPE](https://openarabicpe.github.io), 2015--) <br/>

::: {.c_width-30}

### Ansatz

- Verbindung **vorhandener** Faksimiles und Transkriptionen in einem standardkonformen, offenen Format
- Scraping, Erzeugung, Validierung und Teilen von offenen bibliographischen Metadaten

:::
::: {.c_width-30}

### Ziele

- Validierung und Nutzbarmachung vorhandener Transkriptionen
- Aufbau einer offenen Infrastruktur von Modellen, Workflows, Normdatensätzen
- Unter den **Bedingungen des Globalen Südens**

:::
::: {.c_width-30}

### Prinzipien

- **Etablierte** Werkzeuge und Technologien
- **wenige**, **offene** und **einfache** Formate und Werkzeuge
- **kostenfreie** Platformen ohne lock-in

:::

## [OpenArabicPE](https://openarabicpe.github.io)
### Infrastruktur

:::{.c_width-50}

1. Digitale Editionen, Normdatensätze: [TEI XML](https://tei-c.org/).
1. Offene Lizenzen: [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/) (TEI, MODS, BibTeX), MIT license (XSLT, XQuery)
2. Soziale digitale Editionen, die auf [GitHub](https://github.com/openarabicpe) gehostet sind: <!-- gradually improve transcription and mark-up -->
2. Archivierung auf [Zenodo](https://zenodo.org): DOI für dauerhafte Referenzierbarkeit
3. [Statische Webansichten](https://github.com/openarabicpe/tei-boilerplate-arabic-editions)<!--  (doesn't require a permanent internet connection) -->: Parallele Darstellung von Text und Faksimile.
4. Bibliographische Metadaten sind als öffentliche [Zotero-Gruppe](https://www.zotero.org/groups/openarabicpe) gehostet

:::
:::{.c_width-50}

![[Webansicht von *al-Muqtabas* 6(2)](https://openarabicpe.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_61.TEIP5.xml)](../../assets/OpenArabicPE/boilerplate_muqtabas.png){#fig:webview-muqtabas}

:::

## OpenArabicPE
### Korpus

| Periodikum                                                                    | DOI                                                              | Bände | Ausgaben | Artikel | Wörter  |
| :--------                                                                     | :--                                                              | ----: | ----:    | ----:   | ----:   |
| [al-Ḥaqāʾiq](https://www.github.com/openarabicpe/digital-haqaiq)              | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) | 3     | 35       | 389     | 298090  |
| [al-Ḥasnāʾ](https://www.github.com/openarabicpe/journal_al-hasna)             | [10.5281/zenodo.3556246](https://doi.org/10.5281/zenodo.3556246) | 1     | 12       | 201     | NA      |
| [al-Manār](https://www.github.com/openarabicpe/journal_al-manar)              |                                                                  | 35    | 537      | 4300    | 6144593 |
| [al-Muqtabas](https://www.github.com/tillgrallert/digital-muqtabas)           | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   | 9     | 96       | 2964    | 1981081 |
| [al-Ustādh](https://www.github.com/openarabicpe/journal_al-ustadh)            | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) | 1     | 42       | 435     | 221447  |
| [al-Zuhūr](https://www.github.com/openarabicpe/journal_al-zuhur)              | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) | 4     | 39       | 436     | 292333  |
| [Lughat al-ʿArab](https://www.github.com/openarabicpe/journal_lughat-al-arab) | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) | 3     | 34       | 939     | 373832  |
| **total**                                                                     |                                                                  | 56    | 795      | 9664    | 9311376 |

<!-- Table: Übersicht über das Periodikakorpus {#tbl:openarabicpe-corpus} -->


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

![Karte der in den Autorenzeilen erwähnten Orte für  *al-Muqtabas* (Kairo und Damaskus)](../../assets/OpenArabicPE/maps/map-oclc_4770057679-bylines-middle-east.png){#fig:authors-muqtabas-2}

:::

:::{.c_width-30}

### regional

![Karte der in den Autorenzeilen erwähnten Orte für  *al-Ḥasnāʾ* (Beirut)](../../assets/OpenArabicPE/maps/map-oclc_792756327-bylines-middle-east.png){#fig:authors-hasna}

:::
:::{.c_width-30}

### lokal

![Karte der in den Autorenzeilen erwähnten Orte für  *al-Ḥaqāʾiq* (Damaskus)](../../assets/OpenArabicPE/maps/map-oclc_644997575-bylines-middle-east.png){#fig:authors-haqaiq-2}

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

- Autor_innenzeile: Maryam Zakā aus Saida

```xml
 <byline>
    <placeName ref="oape:place:9 geon:268064">صيدا</placeName>
    <persName ref="oape:pers:2845">مريم زكا</persName>
</byline>
```

- Gazetteer-Eintrag für Saida

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

![Gerichtetes Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas* erwähnten Periodika; nach Ausgaben gewichtet. Größe und Farbe der Knoten: in-degree.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_referenced-periodicals-per-issue_circular-n-size_in-degree.svg){#fig:network-periodicalsß2}

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


## Netzwerkanalyse: erwähnte Periodika
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


+ Das Magazin *al-Zuhūr* aus Kairo 

<!-- ägyptische Zeitschrift -->
```xml
والأصح الدرعية بلام التعريف (راجع <bibl subtype="journal" type="periodical">مجلة <title level="j" ref="oape:bibl:3 oclc:1034545644">الزهور</title> المصرية  <biblScope unit="volume" from="2" to="2">٢</biblScope> :  <biblScope unit="page" from="292">٢٩٢</biblScope></bibl>)
```

+ Die Zeitung *al-Zuhūr* aus Baghdad

<!-- irakische Zeitung -->
```xml
وانتخب <persName>فؤاد أفندي الدفتري البغدادي</persName> و<bibl><editor><persName>نوري أفندي</persName></editor> راس كتاب <textLang otherLangs="ota">القسم التركي</textLang> في <bibl type="periodical" subtype="newspaper">جريدة <title ref="oape:bibl:532">الزهور</title></bibl> البغدادية</bibl> نائبين عن <placeName ref="oape:place:372 geon:94824">كربلاء</placeName>.
```

:::

## 2. Netzwerkanalyse: Autor_innen

:::{.c_width-50}

![Ungerichtetes Netzwerk der Autor_innen in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas*. Farbe der Knoten: betweenness centrality; Größe der Knoten: Anzahl der Periodika; Breite der Kanten: Anzahl der Artikel.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_authors_unimodal-n-size_out-degree-n-colour_betweenness-e-colour_grey.png){#fig:network-authors-2}

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

- Personographie-Eintrag für Père Anastase-Marie de Saint-Elie (Normdatensatz), der sich in den Quellen vornehmlich als *Sātisnā* findet.

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

:::{.c_width-30}

### Forschungsstand

- Die Frage der Autorenschaftsbestimmung ist weitgehend ignoriert worden  <!-- standard accounts don't even mention the issue -->
- Implizite und häufig angenommene Hypothese: die Herausgeber_innen haben alle anonymen Artikel selbst geschrieben

:::
:::{.c_width-30}

![ ](../../assets/clipart/iceberg-2070977_960_720.png){width="100%" height="100%"}

:::
:::{.c_width-30}

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

:::{.c_width-30}

![PCA Kovarianzmatrix für die 100 MFWs in einem Korpus von 165 Ausgaben von *al-Ḥaqāʾiq*, *Lughat al-ʿArab* und *al-Muqtabas*](../../assets/OpenArabicPE/stylometry/comb_muqtabas-haqaiq-lughat_PCA_100_MFWs_Culled_0__PCA__001.png){#fig:pca-halumu-100}

:::
:::{.c_width-30}

- *Lughat al-ʿArab* and *al-Muqtabas* are indistinguishable
- *al-Ḥaqāʾiq* is different
- some issues of *al-Muqtabas* are very different

:::
:::{.c_width-30}

![PCA Kovarianzmatrix für die 100 MFWs in einem Korpus von 165 Ausgaben von *al-Ḥaqāʾiq*, *Lughat al-ʿArab* und *al-Muqtabas*](../../assets/OpenArabicPE/stylometry/comb_muqtabas-haqaiq-lughat_PCA_900_MFWs_Culled_0__PCA__001.png){#fig:pca-halumu-900}

:::

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


# 6. Schlußbemerkungen <br/>Mind the `<gap/>`!
## Mind the `<gap/>`!

:::{.c_width-50}

- bei Forschung/Lehre zu Digitalität
- bei digitaler Forschung/Lehre
- beim Aufbau von Infrastrukturen
- beim Forschungsdatenmanagement
- ...

:::
:::{.c_width-50}

![Graffiti "Du bist so schön, wie eine zusätzliche Stunde Strom", Gaza. Quelle: [Twitter](https://twitter.com/j_zabaneh/status/1366628891817828360)](../../assets/dh/Evc9uxzXEAE8GFw.jpg)
:::

## Danke!

- Beiträger_innen zu Project Jarāʾid: Hala Auji, Philippe Chevrant, Marina Demetriadou, Lamia Eid, Stacy Fahrenthold, Ulrike Freitag, <!-- Till Grallert,  -->Rana Issa, Nicole Khayat, Peter Magierski, Leyla von Mende, Adam Mestyan, Christian Meier, Daniel Newman, Geoffrey Roper, Sinai Rusinek, Philip Sadgrove, Ola Seif, and Rogier Visser
- Beiträger_innen zu OpenArabicPE: Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Beiträger_innen zu OCR: Adam Mestyan, Sinai Rusinek

- Links:
    + Slides: [https://tillgrallert.github.io/slides/dh/2022-digital-history-colloquium](https://tillgrallert.github.io/slides/dh/2022-digital-history-colloquium/index.html)
    + Publikationen: 
        * [@Grallert+2020]
        * [@Grallert2022DHQ]
    + Project URLs: [https://www.github.com/OpenArabicPE](https://www.github.com/OpenArabicPE), [https://openarabicpe.github.io](https://openarabicpe.github.io), 
    + Twitter: @[tillgrallert](https://twitter.com/tillgrallert)
    + Email: <till.grallert@fu-berlin.de>
- Licence: slides and plots are licenced as [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)