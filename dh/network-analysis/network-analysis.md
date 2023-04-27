---
title: "Metapher und Methode"
panel: "Der Netzwerkbegriff und arabische Zeitschriftenforschung"
author: 
	- Till Grallert
    - Yvonne Albers
institute: 
    - Humboldt-Universität zu Berlin
    - Freie Universität Berlin
date: 2023-04-27
event:
url: https://tillgrallert.github.io/slides/dh/network-analysis/index.html
ORCID: orcid.org/0000-0002-5739-8094
lang: de
bibliography: 
    - /Users/Shared/BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /Users/Shared/BachUni/applications/applications.csl.json
slide-level: 2
license: https://creativecommons.org/licenses/by-sa/4.0/
---

# Der Netzwerkbegriff und arabische Zeitschriftenforschung <br/> -------> <br/>Historische Netzwerkanalyse als Zugang zu einer systematischen Periodikaforschung


## Plan

::: columns
:::: column

![Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, *al-Muqtabas* und *al-Zuhūr* erwähnten Periodika.](../../assets/sihafa/networks/network_n_periodical-e_referenced-layout_fr-label_Latn.png){#fig:network-mentioned-periodicals-1}

::::
:::: column

1. Netzwerkanalyse
2. Fallstudie: Rezeption anderer Periodika
    - Set-up
    - Ergebnisse
3. Schlußbemerkungen

::::
:::

::: notes

1. Einführung:
    - [x] Netzwerkanalyse
    - [ ] arabische Periodika
        - teilweise momentan in der Fallstudie enthalten
2. Fallstudie: Rezeption anderer Periodika. Periodika als Netzwerke
    - Set-up
    - Ergebnisse
3. Fallstudie: Netzwerkanalyse als Methode. Stylometrie?
3. Schlußbemerkungen

:::

# Netzwerkanalyse<br/> in der Periodikaforschung
## Periodika als relationales Medium


- Jede Ausgabe repräsentiert ein Netzwerk von **Texten** und **Menschen** (und Orten)
- Jeder Titel repräsentiert ein Netzwerk von **Menschen** (und Orten)
- Periodika existieren im Plural beziehen sich aufeinander
- historische Periodika existieren in einem Sammlungszusammenhang

## Forschungsfragen

- Was sind die wichtigsten Knoten (Autor_innen, Periodika, Orte etc.) im diskursiven Feld der Presse?
- Rezeptionsgeschichte:
    + Wer hat was, wo und wann gelesen (und darüber geschrieben)?
- Produktionsgeschichte:
    + Wie wurden Periodika produziert?
    + Wer verfasste die mehrheitlich anonymen Texte?
    + Wie hoch ist die Wiederverwertungsrate und wie "reisten" Texte?

# Netzwerkanalyse<br/> Hintergrund
## Netzwerkanalyse

Statistische Analyse der Beziehungen (**Kanten**) zwischen Entitäten (**Knoten**)

::: columns
:::: column

![Gerichtetes Netzwerk aller in [*al-Muqtabas* 1(12), 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_12.TEIP5.xml) erwähnter Periodika. Größe und Farbe der Knoten: *weighted degree*.](../../assets/OpenArabicPE/networks/al-muqtabas-v_1-i_12-n_periodicals-e_ref.png){#fig:network-muqtabas-1-12_1}

::::
:::: column

### Modalität

- Unimodal: nur eine Art von Knoten, z.B. Periodika
- Multimodal: verschiedene Arten von Knoten, z.B. Periodika und Personen

### Zentralität von Knoten

- Anzahl und Stärke der Verbindungen
- Länge des Weges zu allen anderen Knoten
- Verbindungen zwischen Clustern

::::
:::

::: notes

- Knoten und Kanten
- Unimodal: 
    + nur eine Art von Knoten
    + verschiedenste Arten von Kanten
        * Beziehungen zwischen Periodika
        * Beziehungen zwischen Menschen
        * Beziehungen zwischen Orten

:::

## Netzwerkanalyse

::: columns
:::: column-30

### Cluster

- Gruppen von Knoten, die untereinader mehr verbunden sind als mit anderen Knoten

### Dichte

- Grad der Verbundenheit
        
::::
:::: column-60

![Ungerichtetes Netzwerk aller in [*al-Muqtabas* 1(12), 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_12.TEIP5.xml) erwähnter Periodika. Kanten und Farbe der Knoten: Sprache. Größe der Knoten: *weighted degree*.](../../assets/OpenArabicPE/networks/al-muqtabas-v_1-i_12-n_periodicals-e_lang.png){#fig:network-muqtabas-1-12_2}

::::
:::

::: notes

- statistische Aussagen über Dichte, Clustering, Wichtigkeit von Knoten

:::

## Netzwerkanalyse

![Gerichtetes Netzwerk aller in [*al-Muqtabas* 1(12), 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_12.TEIP5.xml) erwähnter Periodika. Knoten: Größe = betweenness centrality; Farbe = weighted degree. Kanten: blau = erwähnt; pink = gleiche Sprache; grau = gleicher Publikationsort.](../../assets/OpenArabicPE/networks/al-muqtabas-v_1-i_12-n_periodicals-e_ref-lang-loc.png){#fig:network-muqtabas-1-12_3}

## Netzwerkanalyse

Grafiken sind nicht ausreichend und potenziell irreführend

::: columns
:::: column-60

![Netzwerk der Herausgerber_innen sämtlicher arabischer Periodika, 1800--1929. Größe der Knoten: betweenness centrality](../../assets/OpenArabicPE/networks/network_project-jaraid_people-titles-n-size_betweenness-centrality.svg){#fig:network-editors}

::::
:::: column-30

- Was ist das für ein Netzwerk?
    + 2702 Knoten: Mitarbeiter_innen
    + 608 Kanten: Zusammenarbeit an einem Periodikum
    + Dichte: sehr gering
- Zeigt es sehr begrenzte Zusammenarbeit?
- Zeigt es die falschen Beziehungen?
- Welche Rolle spielt der Datensatz?

::::
:::

# Arabische Periodika {data-background-image="../../assets/OpenArabicPE/front-pages_strip.png" data-background-size="90%"}
## Arabische Periodika

::: columns
:::: column

- Presse als zentraler Agent des Wandels in der Moderne
    + erstes Massenmedium
    + zentrales Medium der literarischen und kulturellen arabischen Renaissance (*nahḍa*)
    + Medium des Sprachwandels
    + zentrale Foren für Verhandlung von Moderne, Nationalismen, Islamismus etc.

::::
:::: column

- Presse bisher vor allem als Quelle genutzt und kaum als Gegenstand untersucht
- Forschung wird dominiert von
    + national(istisch)en Narrativen
    + Verengung auf zwei Orte und wenige <!-- allgemein zugängliche --> Titel
    + impliziten Hypothesen

::::
:::

![Neu gegründete arabisch-sprachige Periodika, 1799--1929](../../assets/jaraid/map-periodicals_World_1855-1929_temp-dist-status-y_5.gif){#fig:map-jaraid}

## Arabische Periodika

::: columns
:::: column

![Titelseite von *al-Quds* #331, 10 Januar 1913](../../assets/OpenArabicPE/front-pages/al-quds-v_5-i_331_annotated.jpg){#fig:al-quds}

::::
:::: column

- Grün: Osmanischer Halbmond mit drei Sternen und Slogan der jungtürkischen Revolution von 1908 "Freiheit, Gleichheit, Brüderlichkeit"
- Blau: Französischer Titel
- Rot: Datumszeile mit drei Kalendern
    + Reformierter julianischer K.: 28. Dezember 1912
    + Gregorianischer K.: 10 Januar 1913
    + Islamischer K.: 2 Ṣafar 1331

::::
:::

<!-- ![Titelseiten von *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *al-Iqbāl*, *al-Maḥabba*, *al-Ahrām*, *al-Muqtaṭaf* und *al-ʿAṣr al-Jadīd*](../../assets/OpenArabicPE/front-pages_strip.png){#fig:front-pages .c_height-30} -->

# Fallstudie <br/>Netzwerk der erwähnten Periodika
## Periodika-Netzwerke

- Frage: welche Periodika werden besonders viel rezepiert?
- Wie: wir zählen sämtliche Erwähnungen von Periodika in allen Periodika (wirklich)
- Zweck:
    + Erweiterung unseres Wissens über Periodika
    + Überprüfung bestehender Trends in der Forschung
    + Überprüfung der Signifikanz des eigenen Korpus
    + Hilfestellung für zukünftige Digitalisierungsprojekte
- Benötigte Daten:
    - Modellierter, digitaler **Volltext** mit Auszeichnung von *named entities* (Periodikatitel)
    - **Normdatensätze** zur Disambiguierung und Anreicherung

::: notes

- Das ist offensichtliche Netzwerkforschung

:::

## Vorhandene Daten?

*Survival* und *collection biases* führen zu *digitisation bias*

::: columns
:::: column

|       Periodika        | --1918 | --1929 |
|------------------------|--------|--------|
| published              |   2054 |   3550 |
| known holdings         |    540 |    775 |
| % of total             |  26.29 |  21.83 |
|------------------------|--------|--------|
| digitized              |    156 |    233 |
| % of total             |   7.59 |   6.56 |
|------------------------|--------|--------|
| multiple digitizations |     51 |     66 |
| % of total             |   2.48 |   1.86 |
| % of digitized         |  32.69 |  28.33 |

::::
:::: column

![Publikationsorte arabischer Periodika bis 1929. Größe der Kreise: Anzahl der Titel. Farbe zeigt den Sammlungsstatus an: unbekannter Verbleib (rot), bekannte Sammlungen (grün und blau), digitalisiert (blau).](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/jaraid/map-data-set-periodicals_1789-1929-scatterpie-mena-label_en.png){#fig:holding-stats}

![In Katalogen dokumentierte Sammlungen arabischer Periodika bis 1929](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/jaraid/map-data-set-periodical-holdings-global-north-na_mapped.png){#fig:holding-map}

::::
:::

::: notes

- we only know of collections that have been catalogued
    + 775 of 3550 titles, c. 20%
- predominantly localed in the Global North
- digitisation is expensive and mundane sources in "foreign" languages do not matter
    + 233 or 6,5% digitised
- uncoordinated efforts
    + 66 titles or c. 30% have been digitised multiple times

:::

## Vorhandene Daten!

- [Open Arabic Periodical Editions][openarabicpe_website]: Modellierter Volltext ([TEI XML](http://www.tei-c.org)), Normdaten ([TEI XML](http://www.tei-c.org))
- [Project Jarāʾid][jaraid_website] (mit Adam Mestyan): bibliographische Metadaten für 3300+ Periodika ([MODS](http://www.loc.gov/standards/mods/), [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework), [BibTeX](http://www.bibtex.org/Format/))

| Periodical                                                        | Place           | Dates[^tb1] | Vol.s   | No.s   | Words       | Articles | with author | Authors | DOI                                                              |
| -------------------------------                                   | ---------       | --------    | ------: | ----:  | ----:       | ------:  | ------:     | ------: | --------------                                                   |
| [al-Ḥaqāʾiq][haqaiq_git]                                          | Damascus        | 1910--13    | 3       | 35     | 298090      | 389      | **41.90**   | 104     | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) |
| [al-Ḥasnāʾ][hasna_git] | Beirut          | 1909--11    | 1       | 12     |             | 201      |             |         |                                                                  |
| [al-Muqtabas][muqtabas_git]                                       | Cairo, Damascus | 1906--18    | **9**   | **96** | **1981081** | **2964** | 12.72       | 140     | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   |
| [al-Ustādh][ustadh_git]                                           | Cairo           | 1892--93    | 1       | 42     | 221447      | 435      | 5.52        | 8       | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) |
| [al-Zuhūr][zuhur_git]                                             | Cairo           | 1910--13    | 4       | 39     | 292333      | 436      | **41.51**   | 112     | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) |
| [Lughat al-ʿArab][lughat_git]                                     | Baghdad         | 1911--14    | 3       | 34     | 373832      | 939      | 16.19       | 53      | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) |
| **total**                                                         |                 |             | 21      | 258    | 3166783     | 5163     |             |         |                                                                  |

Table: Das verwendete "[Open Arabic Periodical Editions][openarabicpe_website]" Corpus  {#tbl:openarabicpe-corpus}

[^tb1]: The current cut-off date is 1918.

[muqtabas_git]: https://github.com/OpenArabicPE/journal_al-muqtabas
[haqaiq_git]: https://github.com/OpenArabicPE/journal_al-haqaiq
[lughat_git]: https://github.com/OpenArabicPE/journal_lughat-al-arab
[ustadh_git]: https://github.com/OpenArabicPE/journal_al-ustadh
[zuhur_git]: https://www.github.com/openarabicpe/journal_al-zuhur
[hasna_git]: https://www.github.com/openarabicpe/journal_al-hasna

## Vorhandene Daten

::: columns
:::: column

### Modellierter Volltext

Aus ["al-Shaykh Ibrāhīm al-Yāzijī", *al-Muqtabas* 1(12), Jan. 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_12.TEIP5.xml#div_15.d1e2443)

```xml
<p xml:lang="ar">هبط مصر في شتاء <date when="1897">سنة <num value="1897">١٨٩٧</num></date> لإنشاء مجلة علمية وطبع معجم عربي كان عني بتأليفه منذ سنين ولكن خانته الأقدار فرأى ما كان يسمعه عن نهضة مصر العلمية مبالغاً فيه وأن <pb ed="shamela" n="n12-p50"/> سوق العلم والأدب كاسدة لا لإقبال عليها فأصدر أولاً <bibl subtype="journal" type="periodical">مجلة <title level="j" ref="oape:bibl:11 oclc:792754974">البيان</title></bibl> سنة بمعاونة <persName ref="oape:pers:2817">الدكتور زلزل</persName> ثم أصدر وحده <bibl subtype="journal" type="periodical">مجلة <title level="j" ref="oape:bibl:27 oclc:1034555409">الضياء</title></bibl> فدامت مطردة الصدور إلى صيف هذه السنة وقد شحنها من عرائس أفكاره وتحقيقاته اللغوية وأماليه الأدبية ما لو كتب بغير هذا اللسان لأعجب به أهله وكبروا مثل مقالات اللغة والعصر ولغة الجرائد وأغلاط العرب وأغلاط المولدين وطبع في العهد الأخير كتاب نجعة الرائد في اللغة ولم يوفق إلى طبع معجمه لأسباب أهمها قلة النصير والظهير.</p>
```

::::
:::: column

### Normdaten

Für die erwähnte Zeitschrift *al-Bayān* (oclc:792754974)

```xml
<biblStruct oape:frequency="monthly" subtype="journal" type="periodical">
   <monogr>
        <title level="j" xml:lang="ar">البيان</title>
        <title level="j" type="sub" xml:lang="ar">مجلة علمية أدبية طبية صناعية</title>
        <idno type="oape">11</idno>
        <idno type="OCLC">792754974</idno>
        <editor> 
            <persName ref="oape:pers:2808 viaf:64154472" xml:lang="ar"><forename>ابراهيم</forename> <surname><addName type="nisbah">اليازجي</addName></surname></persName> </editor>
        <editor>
            <persName ref="oape:pers:2817 viaf:57953733" xml:lang="ar"> <forename>بشارة</forename> <surname>زلزل</surname></persName> </editor>
        <textLang mainLang="ar"/>
        <imprint>
            <date from="1897-03-01" to="1898"/>
            <pubPlace><placeName ref="oape:place:226 geon:360630" xml:lang="ar">القاهرة</placeName></pubPlace>
        </imprint>
   </monogr>
</biblStruct>
```

::::
:::

## Vorhandene Daten

Übersetzung von ausgezeichnetem Volltext und Normdaten in Netzwerkdaten

::: columns
:::: column

### Knoten-Tabelle

| id |   name  | name.transliterated |    type    |
|----|---------|---------------------|------------|
|  9 | المقتبس | al-Muqtabas         | periodical |
| 11 | البيان  | al-Bayān            | periodical |
| 27 | الضياء  | al-Ḍiyāʾ            | periodical |

::::
:::: column 

### Kanten-Tabelle

| source | target |    date    | place |   type   |
|--------|--------|------------|-------|----------|
|      9 |     11 | 1907-01-16 | Cairo | directed |
|      9 |     27 | 1907-01-16 | Cairo | directed |

::::
:::


## Netzwerk erwähnter Periodika

::: columns
:::: wide

![Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, *al-Muqtabas* und *al-Zuhūr* erwähnten Periodika. Größe und Farbe der Knoten: *in-degree*. Kanten: gewichtet nach Anzahl der Ausgaben.](../../assets/sihafa/networks/network_n_periodical-e_referenced-layout_fr-label_Latn.png){#fig:network-mentioned-periodicals-2}

::::
:::: narrow

1. *al-Muqtabas* macht die meisten Verweise
2. Alle Zeitschriften sind selbstreferentiell
1. Nur wenige Knoten sind von relativer Bedeutung (101 von 613)
    - Hochgradig geographisch zentralisiert (10 Orte)
    - Überraschende Mitglieder

::::
:::

::: notes

+ Gesamtnetzwerk: 613 Periodika
    * *al-Muqtabas* macht die meisten Verweise auch nach Abzug seines größeren Umfangs
    * 512 Periodika (83.52 %) von nur einer Zeitschrift erwähnt
    * 421 Periodika (68.68 %) in einer einzigen Ausgabe erwähnt
+ Kernnetzwerk: 
    * 101 Periodika in mehr als einer Zeitschrift erwähnt
    * 8 Periodika in 4 Zeitschriften erwähnt
    * 21 Periodika in 3 Zeitschriften erwähnt
    * 72 Periodika in 2 Zeitschriften erwähnt
    + "Überraschende" Mitglieder
        * Eingestellte Periodika: *al-Jinān* (1876--86), *al-Ḍiyāʾ* (1898--1906)
        * Ausländische Titel: 
            - Paris: *Le Temps*, *Revue des Revues* and *Revue du Monde Musulman*
            - London: *The Times*
:::

## Kernnetzwerk

::: columns
:::: wide

![Kernnetzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, *al-Muqtabas* und *al-Zuhūr* erwähnten Periodika. Größe und Farbe der Knoten: *in-degree*. Kanten: gewichtet nach Anzahl der Ausgaben.](../../assets/sihafa/networks/network_n_periodical-e_referenced-core-layout_fr-label_Latn.png){#fig:network-mentioned-periodicals-core}

::::
:::: narrow

1. Nur wenige Knoten sind von relativer Bedeutung (101 von 662)
5. Hochgradig geographisch zentralisiert (10 Orte)
6. Bestätigt den Fokus auf Kairo und Beirut (8 von 9)
6. Überraschende Mitglieder

::::
:::

::: notes

Kernnetzwerk: 
    * 101 Periodika in mehr als einer Zeitschrift erwähnt
        - Sprachen
            + Arabisch: 89
            + Französisch: 8
            + Englisch: 3
            + Osmanisch: 1
    * 8 Periodika in 4 Zeitschriften erwähnt
        - *al-Manār*, *al-Hilāl* and *al-Ḍiyā* aus Kairo
        - *al-Muqtabas* aus Kairo/ Damaskus
        - *al-Muqtaṭaf* aus Beirut / Kairo
        - *al-Mufīd*, *Ḥadīqat al-Akhbār* aus Beirut
        - *al-Athār* aus Zahle
        - The centrality of the three Cairene periodicals, *al-Manār*, *al-Muqtaṭaf*, *al-Hilāl*, which were all published by Syrian immigrants, tentatively confirms standard narratives of the Arabic press
        * The remaining five, however, do not figure prominently in scholarly literature.
    * 21 Periodika in 3 Zeitschriften erwähnt
    * 72 Periodika in 2 Zeitschriften erwähnt
    + "Überraschende" Mitglieder
        * Eingestellte Periodika: *al-Jinān* (1876--86), *al-Ḍiyāʾ* (1898--1906)
        * Ausländische Titel: 
            - Paris: *Le Temps*, *Revue des Revues* and *Revue du Monde Musulman*
            - London: *The Times*

:::

## Kernnetzwerk

|       title.Latn       | in-degree | in-degree (weighted by issue) | lang |     location    |
|------------------------|-----------|-------------------------------|------|-----------------|
| al-Muqtabas            |         4 |                            67 | ar   | Cairo, Damascus |
| al-Mufīd               |         4 |                            12 | ar   | Beirut          |
| al-Āthār               |         4 |                             5 | ar   | Zahle           |
| al-Ḍiyāʾ               |         4 |                            13 | ar   | Cairo           |
| al-Manār               |         4 |                            19 | ar   | Cairo           |
| al-Hilāl               |         4 |                            25 | ar   | Cairo           |
| Ḥadīqat al-Akhbār      |         4 |                             7 | ar   | Beirut          |
| al-Muqtaṭaf            |         4 |                            17 | ar   | Beirut, Cairo   |
| al-Zuhūr               |         3 |                            28 | ar   | Cairo           |
| Lughat al-ʿArab        |         3 |                            32 | ar   | Baghdad         |
| al-Ḥasnāʾ              |         3 |                            11 | ar   | Beirut          |
| Sūriyya                |         3 |                             3 | ar   | NA              |
| al-Waṭan               |         3 |                             6 | NA   | NA              |
| al-Naṣīr               |         3 |                             4 | NA   | NA              |
| al-Ḥuqūq               |         3 |                             4 | ar   | Mount Lebanon   |
| al-ʿAṣr al-Jadīd       |         3 |                             4 | ar   | Damascus        |
| al-Kulliyya            |         3 |                             3 | ar   | Beirut          |
| al-Waṭan               |         3 |                             4 | ar   | Beirut          |
| Lisān al-ʿArab         |         3 |                             3 | ar   | NA              |
| al-Ikhāʾ               |         3 |                             3 | ar   | Hama            |
| al-ʿIrfān              |         3 |                            11 | ar   | Sidon           |
| al-Ḥaqīqa              |         3 |                             4 | ar   | Beirut          |
| al-Ṭabīb               |         3 |                             4 | ar   | NA              |
| al-Insāniyya           |         3 |                             4 | NA   | NA              |
| Le Temps               |         3 |                            12 | fr   | Paris           |
| al-Ittiḥād al-ʿUthmānī |         3 |                             5 | ar   | Beirut          |
| al-Mashriq             |         3 |                            15 | ar   | Beirut          |
| al-Muʾayyad            |         3 |                            19 | NA   | Cairo           |
| The Times              |         3 |                             8 | en   | London          |

## Kernnetzwerk

::: columns
:::: column

| Rang | Sprache | Titel |
|------|---------|-------|
|    1 | ar      |    89 |
|    2 | fr      |     8 |
|    3 | en      |     3 |
|    4 | ota     |     1 |

::::
:::: column

| Rang |    Ort     | Titel |
|------|------------|-------|
|    1 | Beirut     |    27 |
|    2 | Cairo      |    18 |
|    3 | Damascus   |    10 |
|    4 | Paris      |     7 |
|    5 | NA         |     5 |
|    6 | Alexandria |     4 |
|    7 | Baghdad    |     4 |
|    8 | Istanbul   |     3 |
|    9 | Hama       |     2 |
|   10 | Homs       |     2 |

::::
:::

## Geographische Netzwerke
### Internationale Zeitschriften

![1462 in *al-Muqtabas* erwähnte Periodka](../../assets/OpenArabicPE/maps/map-oclc_4770057679-referenced-periodicals-all-source-na_mapped.png){#fig:map-periodicals-muqtabas}

## Geographische Netzwerke
### Lokale und regionale Zeitschriften

::: columns
:::: column

![100 in *al-Ustādh* erwähnte Periodka](../../assets/OpenArabicPE/maps/map-oclc_1036721166-referenced-periodicals-all-source-na_mapped.png){#fig:map-periodicals-ustadh}

![187 in *Lughat al-ʿArab* erwähnte Periodka](../../assets/OpenArabicPE/maps/map-oclc_472450345-referenced-periodicals-all-source-na_mapped.png){#fig:map-bylines-lughat}

::::
:::: column

![85 in *al-Ḥaqāʾiq* erwähnte Periodka](../../assets/OpenArabicPE/maps/map-oclc_644997575-referenced-periodicals-all-source-na_mapped.png){#fig:map-periodicals-haqaiq}

::::
:::

# Schlußbemerkungen
## Netzwerkanalyse

- Kann wichtige Einblicke geben, die durch *close reading* nicht möglich sind.
- Hilft vorhandene Corpora zu evaluieren und Digitalisierungen zu priorisieren 
- Ist aufwendig und die Datenbasis kann nur kollaborativ erschlossen werden.

::: columns
:::: column

What most people think I do

![@fig:network-mentioned-periodicals-2: Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, *al-Muqtabas* und *al-Zuhūr* erwähnten Periodika.](../../assets/sihafa/networks/network_n_periodical-e_referenced-layout_fr-label_Latn.png)

::::
:::: column

What I actually do

1. Daten vorbereiten
    - Digitalisieren
    - Daten modellieren
    - entity recognition
    - entity disambiguation
    - Daten bereinigen
    - ein bisschen mehr Daten bereinigen
    - ...
    - noch mehr Daten bereinigen
2. Netzwerkanalyse
    - Daten transformieren
    - natürlich wieder Daten bereinigen
    - analysieren
    - visualisieren

::::
:::

## Danke!

- Beiträger_innen zu [OpenArabicPE][openarabicpe_website]: Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Daniel, Kolland, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Beiträger_innen zu [Project Jarāʾid][jaraid_website]: Hala Auji, Philippe Chevrant, Marina Demetriadou, Lamia Eid, Stacy Fahrenthold, Ulrike Freitag, Till Grallert, Rana Issa, Nicole Khayat, Peter Magierski, Leyla von Mende, Adam Mestyan, Christian Meier, Daniel Newman, Geoffrey Roper, Sinai Rusinek, Philip Sadgrove, Ola Seif, and Rogier Visser
- Links:
    + Folien: [https://tinyurl.com/2023-grallert-network](https://tillgrallert.github.io/slides/dh/network-analysis/index.html)
    + Projektblog: <https://openarabicpe.github.io>
    + Papers: <http://digitalhumanities.org/dhq/vol/16/2/000593/000593.html>, <https://doi.org/10/gkhrjr>
    + Mastodon: \@[tillgrallert@digitalcourage.social](https://digitalcourage.social/@tillgrallert)
    + Email: <till.grallert@fu-berlin.de>, <till.grallert@hu-berlin.de>
- Lizenz: Folien und Plots sind unter [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/) lizensiert

# Weitere Netzwerke
## Autor_innenzeilen
### Lokale und regionale Zeitschriften

::: columns
:::: column

<!-- ![Orte in Autor_innenzeilen, *Lughat al-ʿArab*](../../assets/OpenArabicPE/maps/map-oclc_472450345-bylines-all-source-na_mapped.png){#fig:map-bylines-lughat} -->
![Orte in Autor_innenzeilen, *al-Ḥaqāʾiq*](../../assets/OpenArabicPE/maps/map-oclc_644997575-bylines-all-source-na_mapped.png){#fig:map-bylines-haqaiq}

::::
:::: column

![Orte in Autor_innenzeilen, *al-Ḥasnāʾ*](../../assets/OpenArabicPE/maps/map-oclc_792756327-bylines-all-source-na_mapped.png){#fig:map-bylines-hasna}

::::
:::

## Autor_innenzeilen
### Internationale Zeitschriften

![Orte in Autor_innenzeilen, *al-Muqtabas*](../../assets/OpenArabicPE/maps/map-oclc_4770057679-bylines-all-source-na_mapped.png){#fig:map-bylines-muqtabas}


[openarabicpe_website]: https://openarabicpe.github.io
[jaraid_website]: https://projectjaraid.github.io