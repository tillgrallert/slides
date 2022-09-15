---
title: "Historische Netzwerkanalyse als Zugang zu einer systematischen Periodikaforschung"
panel: "Arab Periodical Studies: Neue Ansätze zu Einer Kulturwissenschaftlichen Zeitschriftenforschung"
event: "#DOT2022"
author: 
	- Till Grallert
institute: Humboldt-Universität zu Berlin
date: 2022-09-12 
ORCID: orcid.org/0000-0002-5739-8094
lang: en-GB
bibliography: 
    - /Users/Shared/BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /Users/Shared/BachUni/applications/applications.csl.json
slide-level: 2
---

## Plan

::: columns
:::: column

![Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas* erwähnten Periodika.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_referenced-periodicals-per-issue_circular-n-size_in-degree.svg)

::::
:::: column

1. Netzwerkanalyse
2. Fallstudie: Rezeption anderer Periodika
    - Set-up
    - Ergebnisse
3. Schlußbemerkungen

::::
:::

# Netzwerkanalyse
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


## Netzwerkanalyse

- Was: Statistische Analyse der Beziehungen (**Kanten**) zwischen Entitäten (**Knoten**)

::: columns
:::: column

![Gerichtetes Netzwerk aller in [*al-Muqtabas* 1(12), 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_12.TEIP5.xml) erwähnter Periodika. Größe und Farbe der Knoten: *weighted degree*.](../../assets/OpenArabicPE/networks/al-muqtabas-v_1-i_12-n_periodicals-e_ref.png){#fig:network-muqtabas-1-12_1}

::::
:::: column

### Zentralität von Knoten

- Anzahl und Stärke der Verbindungen
- Länge des Weges zu allen anderen Knoten
- Verbinungen zwischen Clustern

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

![Netzwerk aller in [*al-Muqtabas* 1(12), 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_12.TEIP5.xml) erwähnter Periodika. Knoten: Größe = betweenness centrality; Farbe = weighted degree. Kanten: blau = erwähnt; pink = gleiche Sprache; grau = gleicher Publikationsort.](../../assets/OpenArabicPE/networks/al-muqtabas-v_1-i_12-n_periodicals-e_ref-lang-loc.png){#fig:network-muqtabas-1-12_3}

## Netzwerkanalyse

Grafiken sind nicht ausreichend und potenziell irreführend

::: columns
:::: column-60

![Netzwerk der Herausgerber_innen sämtlicher arbischer Periodika, 1800--1929. Größe der Knoten: betweenness centrality](../../assets/OpenArabicPE/networks/network_project-jaraid_people-titles-n-size_betweenness-centrality.svg){#fig:network-editors}

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

## Vorhandene Daten?

Kombinationen von *survival*, *collection* und *digitisation biases*

::: columns
:::: column-60

![Bekannte Sammlungen und Digitalisate arabischer Periodika bis 1929 nach Publikationsort](../../assets/jaraid/map-example_sf_mena_en-status_scatterpie.png){#fig:map-holdings-summary}

::::
:::: column-30

![In Katalogen dokumentierte Sammlungen arabischer Periodika bis 1929](../../assets/jaraid/map-data-set-periodical-holdings-med-na_mapped.svg){#fig:map-holdings-catalogues}

::::
:::

## Vorhandene Daten!

- [Open Arabic Periodical Editions](https://openarabicpe.github.io/): Modellierter Volltext ([TEI XML](http://www.tei-c.org)), Normdaten ([TEI XML](http://www.tei-c.org))
- [Project Jarāʾid](https://projectjaraid.github.io/) (mit Adam Mestyan): bibliographische Metadaten für 3300+ Periodika ([MODS](http://www.loc.gov/standards/mods/), [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework), [BibTeX](http://www.bibtex.org/Format/))

| Periodical                                                        | Place           | Dates[^tb1] | Vol.s   | No.s   | Words       | Articles | with author | Authors | DOI                                                              |
| -------------------------------                                   | ---------       | --------    | ------: | ----:  | ----:       | ------:  | ------:     | ------: | --------------                                                   |
| [al-Ḥaqāʾiq][haqaiq_git]                                          | Damascus        | 1910--13    | 3       | 35     | 298090      | 389      | **41.90**   | 104     | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) |
| [al-Ḥasnāʾ][hasna_git] | Beirut          | 1909--11    | 1       | 12     |             | 201      |             |         |                                                                  |
| [al-Muqtabas][muqtabas_git]                                       | Cairo, Damascus | 1906--18    | **9**   | **96** | **1981081** | **2964** | 12.72       | 140     | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   |
| [al-Ustādh][ustadh_git]                                           | Cairo           | 1892--93    | 1       | 42     | 221447      | 435      | 5.52        | 8       | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) |
| [al-Zuhūr][zuhur_git]                                             | Cairo           | 1910--13    | 4       | 39     | 292333      | 436      | **41.51**   | 112     | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) |
| [Lughat al-ʿArab][lughat_git]                                     | Baghdad         | 1911--14    | 3       | 34     | 373832      | 939      | 16.19       | 53      | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) |
| **total**                                                         |                 |             | 21      | 258    | 3166783     | 5163     |             |         |                                                                  |

Table: Das verwendete "[Open Arabic Periodical Editions](https://openarabicpe.github.io/)" Corpus  {#tbl:openarabicpe-corpus}

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

Aus ["*al-Shaykh Ibrāhīm al-Yāzijī", *al-Muqtabas* 1(12), Jan. 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_12.TEIP5.xml#div_15.d1e2443)

```xml
<p xml:lang="ar">هبط مصر في شتاء <date when="1897">سنة <num value="1897">١٨٩٧</num></date> لإنشاء مجلة علمية وطبع معجم عربي كان عني بتأليفه منذ سنين ولكن خانته الأقدار فرأى ما كان يسمعه عن نهضة مصر العلمية مبالغاً فيه وأن <pb corresp="file:../epub/26523/OEBPS/xhtml/P686.xhtml" ed="shamela" n="n12-p50"/> سوق العلم والأدب كاسدة لا لإقبال عليها فأصدر أولاً <bibl subtype="journal" type="periodical">مجلة <title level="j" ref="oape:bibl:11 oclc:792754974">البيان</title></bibl> سنة بمعاونة <persName ref="oape:pers:2817">الدكتور زلزل</persName> ثم أصدر وحده <bibl subtype="journal" type="periodical">مجلة <title level="j" ref="oape:bibl:27 oclc:1034555409">الضياء</title></bibl> فدامت مطردة الصدور إلى صيف هذه السنة وقد شحنها من عرائس أفكاره وتحقيقاته اللغوية وأماليه الأدبية ما لو كتب بغير هذا اللسان لأعجب به أهله وكبروا مثل مقالات اللغة والعصر ولغة الجرائد وأغلاط العرب وأغلاط المولدين وطبع في العهد الأخير كتاب نجعة الرائد في اللغة ولم يوفق إلى طبع معجمه لأسباب أهمها قلة النصير والظهير.</p>
```

::::
:::: column

### Normdaten

Für die erwähnte Zeitschrift *al-Bayān*

```xml
<biblStruct oape:frequency="monthly" subtype="journal" type="periodical">
  <monogr>
        <title level="j" xml:lang="ar">البيان</title>
        <title level="j" type="sub" xml:lang="ar">مجلة علمية أدبية طبية صناعية</title>
        <idno type="oape">11</idno>
        <idno type="jid" xml:lang="ar">161</idno>
        <idno type="OCLC">792754974</idno>
        <editor source="../../oclc_165855925/tei/oclc_165855925-v_1.TEIP5.xml#p_1303.d2e14065"> 
            <persName ref="oape:pers:2808 viaf:64154472" xml:lang="ar"><forename>ابراهيم</forename> <surname><addName type="nisbah">اليازجي</addName></surname></persName> </editor>
        <editor source="../../oclc_165855925/tei/oclc_165855925-v_1.TEIP5.xml#p_1303.d2e14065">
            <persName ref="oape:pers:2817 viaf:57953733"> <forename>بشارة</forename> <surname>زلزل</surname></persName> </editor>
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

# Ergebnisse <br/>Erwähnte Periodika
## Erwähnte Periodika

::: columns
:::: column-60

![Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas* erwähnten Periodika. Größe und Farbe der Knoten: *in-degree*. Kanten: gewichtet nach Anzahl der Ausgaben.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_referenced-periodicals-per-issue_circular-n-size_in-degree.svg){#fig:network-mentioned-periodicals}

::::
:::: column-30

1. *al-Muqtabas* macht die meisten Verweise
2. Alle Zeitschriften sind selbstreferentiell
1. Nur wenige Knoten sind von relativer Bedeutung (44 von 465)
5. Hochgradig geographisch zentralisiert (10 Orte)
6. Bestätigt den Fokus auf Kairo und Beirut (8 von 9)
6. Überraschende Mitglieder

::::
:::

::: notes

+ Gesamtnetzwerk: 465 Periodika
    * *al-Muqtabas* macht die meisten Verweise auch nach Abzug seines größeren Umfangs
    * 421, 90% von nur einer Zeitschrift erwähnt
    * 344 Periodika in einer einzigen Ausgabe erwähnt
    * 335 Periodika in einem einzigen Artikel erwähnt
+ Kernnetzwerk: 44 Periodika
    * 9 Periodika in 3 Zeitschriften erwähnt
        * *al-Manār*, *al-Muqtaṭaf*, *al-Hilāl* and *al-Ḍiyā* from Cairo
        * *al-Muqtabas* aus Cairo/ Damaskus
        * *al-Mufīd*, *al-Waṭan* and *al-Ḥaqīqa* from Beirut
        * *al-Ḥuqūq* from Mt. Lebanon
        * The centrality of the three Cairene periodicals, *al-Manār*, *al-Muqtaṭaf*, *al-Hilāl*, which were all published by Syrian immigrants, tentatively confirms standard narratives of the Arabic press
        * The remaining six, however, do not figure prominently in scholarly literature.
    + "Überraschende" Mitglieder
        * Eingestellte Periodika: *al-Jinān* (1876--86), *al-Ḍiyāʾ* (1898--1906)
        * Ausländische Titel: 
            - Paris: *Le Temps*, *Revue des Revues* and *Revue du Monde Musulman*
            - London: *The Times*
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

![@fig:network-mentioned-periodicals: Netzwerk der in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab* und *al-Muqtabas* erwähnten Periodika.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_referenced-periodicals-per-issue_circular-n-size_in-degree.svg)

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

- Beiträger_innen zu OpenArabicPE: Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Beiträger_innen zu Project Jarāʾid: Hala Auji, Philippe Chevrant, Marina Demetriadou, Lamia Eid, Stacy Fahrenthold, Ulrike Freitag, Till Grallert, Rana Issa, Nicole Khayat, Peter Magierski, Leyla von Mende, Adam Mestyan, Christian Meier, Daniel Newman, Geoffrey Roper, Sinai Rusinek, Philip Sadgrove, Ola Seif, and Rogier Visser
- Links:
    + Folien: [https://tinyurl.com/dot2022-grallert-periodicals](https://tillgrallert.github.io/slides/dh/2022-dot-periodicals/index.html)
    + Projektblog: [https://openarabicpe.github.io](https://openarabicpe.github.io)
    + Papers: <http://digitalhumanities.org/dhq/vol/16/2/000593/000593.html>, <https://doi.org/10/gkhrjr>
    + Twitter: \@[tillgrallert](https://twitter.com/tillgrallert)
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