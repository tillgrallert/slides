---
title: "Minimal Computing to the Rescue"
subtitle: "Addressing Our Needs with the People, Tools, and Infrastructures We Have at Hand"
author: Till Grallert
institute: 
    - Humboldt-Universität zu Berlin
    - Methods Innovation Lab (NFDI 4Memory)
    - Scholarly Makerspace
date: 2023-06-27
event: "History, Digitisation, and Archive"
url: https://tillgrallert.github.io/slides/dh/2023-regensburg/
ORCID: orcid.org/0000-0002-5739-8094
lang: de
bibliography: 
    - /Users/Shared/BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /Users/Shared/BachUni/applications/applications.csl.json
slide-level: 2
license: https://creativecommons.org/licenses/by-sa/4.0/
---

<!-- 

- why do we need to be rescued
- what do we need to be rescued from

 -->

# Introduction
## Summary

::: columns-3
:::: column

### Topic

digital and infrastructual divide(s) between the hegemonic, Anglophone North and societies/communities of the Global South with a focus on Arabic as one of the main human languages and scripts

::::
:::: column

### Case study

*Minimal computing* approaches to address the affordances of the digital (or lack thereof) "without the help we cannot get": technological resistance to languages other than English, neo-colonial silencing of the cultural record, complete lack of funds.

::::
:::: column

### Projects

1. Creating knowledge about artefacts: Project Jarāʾid (2011--), a crowd-sourced union list of all Arabic periodicals published before 1930
2. Access to artefacts: Open Arabic Periodical Editions (2015--), a framework for bootstrapped scholarly editions outside the global north

::::
:::

## Overview of today's talk

1. The problem or why do we need rescue

<!-- structure along the workflow:
- knowledge gathering
- digitisation
- publication
 -->

# The problem or why do we need rescue
## digital divide and affordances of the Global South

::: columns
:::: column

- electricty
- internet 
- literacy

::::
:::: column

![Protestor in Baghdad, 31. July 2015, holding sign "darling, you are as beautiful as an additional hour of electricity". Source: [Twitter](https://twitter.com/aya_mansour_11_/status/627223846244847616)](/Users/Shared/BachUni/publications/github/p8fc0a1bd/assets/images/tweet_ 627223846244847616.png){#fig:strom-baghdad}

::::
:::


::: notes

- global north / south
    + not homogenous block but the term has analytical value
    + global north: 
        * hegemonic author of all standards and best practices of the digital
        * owner of the infrastructures
    - global south
        + not the universal other
        + plurality of heterogeneous regions
        * shared experience of constantly negotiating the hegemony of the anglophone global north.
- digital divide
    - electricity
        + 800 mio have no access
        + by 2030: 
            * 600 mio
            * 33 per cent of all Africans
        - access: 
            + 250--500 kWh per year and household
            + less than 14 hours of a 100W lightbulb per day
    - internet
        + 36,6 Prozent der Weltbevölkerung, oder 2,93 Milliarden do not participate
        + 85 per cent of them live in Africa, South, East and South-East Asia
        + lower speed
        + higher latency
        + higher cost per unit of traffic
    - literacy
        + Südasien und Afrika:
            * zwischen 49 und 66 Prozent bei Frauen und 67 bis 80 Prozent bei Männern
        + Interfaces and content is dominated by hegemonial languages and scripts of the Global North

:::

## *linguistic imperialism* and the Absence of Arabic

::: columns
:::: column

- Arabic is one of the major human languages and scripts
- Inadequately supported in the digital realm
    + character encoding: Unicode is not enough!
    + rendering
    + computational methods

::::
:::: column

<!-- ![Interface of the [Translatio](https://digitale-sammlungen.ulb.uni-bonn.de/ulbbnioa/periodical/titleinfo/3384757?lang=en) project (Bonn). Facsimile of Arabic original on the left. Yellow = English UI; purple = Arabic metadata in Latinised transcription;  green = German metadata](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/OpenArabicPE/translatio_interface-languages_annotated.png){#fig:translatio-interface} -->

![Rendered HTML with the built-in default CSS for @oclc_4770057679-i_13-div_8.d1e1249. The test file is available [online](https://doi.org/10.5281/zenodo.7781543)](../../assets/dh/arabic_failure-browser.png){#fig:zakham-ar-failure}

![HTML-Code for @fig:zakham-ar-failure in Visual Code Studio. By default, non-ASCII characters are visually highlighted](../../assets/dh/html_vscode.png){#fig:html}

::::
:::

::: notes

- [@Phillipson1997RealitiesAndMyths]
- Arabic: script and language
    + one of six official languages of the UN
    + spoken by 420 mio people
    + most common script after Latin and chinese
- script
    + right to left
    + connected
    + 
- data: 
    - character encoding -> transliteration
    - automated layout and text recognition
    - data models
    - NER
- interfaces
    + languages of the global north
    + search queries normalised to ASCII

:::

## Digitisation bias
### Collection biases perpatuated

::: columns
:::: column

![Periodicals and their holding institutions](../../assets/jaraid/map-data-set-periodical-holdings-med-na_mapped.png){#fig:holding-map}

::::
:::: column

|      periodicals       | --1918 | --1929 |
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

Table: Periodical holdings and digitization {#tbl:jaraid-holdings}

::::
:::

::: notes

- collection bias is more of a knowledge bias
- While the digitization quote of roughly 50% of titles in collections is surprisingly high, it must be kept in mind that we cannot resolve information on the extent of digitization. Even if only a single issue of hundreds published was digitized, the periodical title will be included in this count.
- 66 periodicals or 28,33% have been digitized by multiple institutions and 21 of this subset by three and more.

:::

## Digitisation biases
### illustrating the divide

|             | Arabic periodicals (1798--1918) | [WWI as mirrored by Hessian regional papers](https://hwk1.hebis.de) |
|-------------|---------------------------------|---------------------------------------------------------------------|
| community   | c. 420 million Arabic speakers  | c. 6.2 million inhabitants                                          |
| periodicals | 2054 newspapers and journals    | 125 newspapers                                                      |
| digitized   | 156 periodicals                 | 125 newspapers with more than 1.5 million pages                     |
| type        | mostly facsimiles               | facsimiles and full text                                            |
| access      | paywalls, geo-fencing           | open access                                                         |
| interface   | mostly foreign languages only   | local and foreign languages                                         |

Table: Comparison of digitized periodicals between the Global South and the Global North {#tbl:digitisation}

## Digitisation biases
### Quality of metadata

Bibliographic metadata is faulty throughout, mostly unstructured, and subject to *linguistic imperialism*

::: columns
:::: column

![@oclc_4770057679-i_61-div_21.d1e2838 on [Shamela](http://shamela.ws/browse.php/book-26523#page-4046) as it appeared in 2019](https://openarabicpe.github.io/slides/assets/shamela_muqtabas-annotated.png){#fig:muqtabas-6-2-shamela}

::::
:::: column

![Facsimile of the same section of @oclc_4770057679-i_61-div_21.d1e2838 from [EAP](https://eap.bl.uk/
)](../../assets/OpenArabicPE/eap119-1-4-5-muqtabas-133_annotated.jpg){#fig:muqtabas-6-2-133-eap}

::::
:::

::: notes

- faulty on shadow libraries and official digitisation efforts
    - publication dates
        + inferred from vol. and issue number: 1 Ṣafar 1329 aH / c. 1 February 1911
        + EAP: March 1911
        + secondary sources: probably delayed by up to four months
    - volume and issue numbers
        + shamela: no.61
        + correct: vol. 6, no. 2
    - pagination:
        + shamela = 45, correct = 133
    - publication place
        + EAP lists Jerusalem
- linguistic imperialism
    + script
    + calendars

:::

## Digitisation biases
### Traditional OCR

>language [is] not currently OCRable.

<cite>Archive.org's item description for [@KurdAli+1923+GharaibAlGharba]</cite>

::: columns
:::: wide


| Font Type          | Sakhr (%)           | ABBYY (%)           | RDI(%)              | Tesseract (%)       |
| -----------------  | -------:            | --------:           | ------:             | -----------:        |
| Traditional Arabic | 48.54               | 67.66               | [**51.88**]{.green} | 47.04               |
| Tahoma             | 10.52               | 69.91               | 26.38               | 38.37               |
| Simplified Arabic  | 52.97               | 67.69               | 44.94               | 46.75               |
| M Unicode Sara     | 36.03               | 59.40               | 25.92               | 33.72               |
| Diwani letter      | [**18.13**]{.red}   | [**18.47**]{.red}   | [**18.13**]{.red}   | [**23.32**]{.red}   |
| DecoType Thuluth   | 36.12               | 37.71               | 24.26               | 32.48               |
| Deco'Type Naskh    | 48.88               | 50.22               | 41.63               | 40.92               |
| Arabic transparent | 51.56               | [**75.19**]{.green} | 46.00               | [**48.61**]{.green} |
| Andalus            | 28.07               | 37.53               | 21.68               | 25.34               |
| AdvertisingBold    | [**57.35**]{.green} | 70.26               | 27.20               | 39.39               |

Table: Evaluation of traditional OCR software for Arabic font types from [@Alghamdi.Teahan+2017+ExperimentalEvaluationArabic, table IV]. Values show percentage of correctly recognised characters {#tbl:ocr-ar-trad}

::::
:::: narrow

<!-- ![*al-Muqtabas* 6 on [HathiTrust](http://hdl.handle.net/2027/njp.32101073250910), quality of the OCR layer (requires US IP)](../../assets/OpenArabicPE/hathi_muqtabas-ocr-3.png) -->
![*al-Bashīr* 9 Jan. 1880 (#487), p.1 on [GPA](https://gpa.eastview.com/crl/mena/newspapers/bshr18800109-01.1.1), quality of the OCR layer](../../assets/OpenArabicPE/gpa_bashir-i_487-p_1_ocr.png){#fig:gpa-ocr}

::::
:::

::: notes

- technical problems
    + layout recognition
    + segmentation
    + text recognition
- what do you do if you have none of the resources mentioned in the toot
- problems with platform providers
    + Unstructured text, no APIs, propriertary interfaces
    + Algorithms and evaluation are kept secret
        *  unknown numbers of *false positives* and *false negatives*

:::

## Digitisation biases
### machine-learning approaches to OCR 

>For old prints, there's [...] kraken/calamari for coders, Transkribus if you've got money and just want to have the results[,] and OCR-D if you've got an IT department.

<cite>[@Winkler20230307OCR]</cite>


| ID      | ground truth    | words   | lines  | epochs  | CER train  | CER validation     |
| ------- | --------------- | ------: | -----: | ------: | ---------: | --------------:    |
| 15946   | *al-Ustādh*     | 192829  | 18732  | 200     | 2.01       | [**2.09**]{.green} |
| 13864   | *al-Muqtabas*   | 11116   | 1013   | 200     | 0.07       | [**8.40**]{.red}   |

Table: Evaluation of my own Transkribus models {#tbl:ocr-ar-ml}


::: notes

- results are great (layout recognition still lacking)
- but digitised collections need to be re-processed (expensive)

:::


## Accessibility
### Catalogue searches

::: columns-3
:::: column

No Arabic script

![Search in [ZDB](https://zdb-katalog.de/list.xhtml?t=الجنة) for "الجنة"](../../assets/jaraid/zdb_janna-ar.png){#fig:zdb-ar}

::::
:::: column

Which Latinized transcription was used?

![Search in [ZDB](https://zdb-katalog.de/list.xhtml?t=al-Ǧanna) for "al-Ǧanna"](../../assets/jaraid/zdb_janna-ar-Latn.png){#fig:zdb-dmg}

::::
:::: column

What are the normalization rules for the search algorithm?

![Search in [ZDB](https://zdb-katalog.de/list.xhtml?t=Ganna) for "Ganna"](../../assets/jaraid/zdb_janna-ar-Latn-no-al.png){#fig:zdb-functional}

::::
:::

::: notes

- catalogue could be searched in Arabic but the data is missing
- Latin input is mostly reduced to ASCII
    + Hamza and ʿAyn escape this algorithm on ZDB
- determined article is not automatically removed

:::

## Accessibility
### Interfaces

![Interface of the [Translatio](https://digitale-sammlungen.ulb.uni-bonn.de/ulbbnioa/periodical/titleinfo/3384757?lang=en) project (Bonn). Facsimile of Arabic original on the left. Yellow = English UI; purple = Arabic metadata in DMG transcription;  green = German metadata](../../assets/OpenArabicPE/translatio_interface-languages_annotated.png){#fig:translatio-interface}

## Accessibility
### copyright regimes, paywalls, and geo fencing

cataloging rules and algorithmic copyright detection cause further inaccessibilities

::: columns
:::: column

![*al-Muqtabas* 6 on [HathiTrust](http://hdl.handle.net/2027/njp.32101073250910) (Original in Princeton) outside the USA](../../assets/OpenArabicPE/hathi_muqtabas-1.png){#fig:hathi-muqtabas-global}

::::
:::: column

![The page from [@fig:hathi-muqtabas-global] with a US-IP](../../assets/OpenArabicPE/hathi_muqtabas-2.png){#fig:hathi-muqtabas-us}

::::
:::


::: notes

Beispiel: unklares Enddatum eines Erscheinungsverlaufs im 20. Jahrhundert wird korrekt als 19uu katalogisiert und dann Copyrightstatus sicherheitshalber als 1999 angenommen.

:::



# Minimal Computing
# A preliminar workflow
## Workflow for bootstrapping
### 1. get the data

- facsimiles
    + link to existing facsimiles, preferably through [IIIF](http://iiif.io)
    + scan your physical artefacts*
- text
    + scrape existing transcriptions
    + use [Transkribus](https://transkribus.eu/), [eScripta](https://escripta.hypotheses.org)/[eScriptorium](https://www.https://escriptorium.fr/) for HTR (with our model trained on 1000+ pages from the OpenArabicPE corpus)

## Workflow for bootstrapping
### 2. save and share the data

- facsimiles: [Internet Archive](https://archive.org) (supports IIIF)
- working copy of everything else: [GitHub](https://github.com/)
- longterm preservation: [Zenodo](https://zenodo.org/)
    + make sure to add [ORCID](https://orcid.org)s for all contributors
- authority data: [Wikidata](https://wikidata.org/)

## Workflow for bootstrapping
### 3. edit the data

- Free, syntax-aware Texteditor with RTL support: [Visual Studio Code](https://code.visualstudio.com) 
- use open, publicly-funded (web)editors, such as [TextGrid Lab](https://textgrid.de/index)
- make use of version control and stable IDs for **transparent authorship attribution**: [GitHub](https://github.com/), [ORCID](https://orcid.org)

## Workflow for bootstrapping
### 4. disseminate the data

- generate static webviews:
    - render XML to HTML on-the-fly in the client's web browser:
        + XSLT1: [TEI Boilerplate](https://github.com/OpenArabicPE/tei-boilerplate-arabic-editions)
        + JavaScript: [CETEICean](https://github.com/TEIC/CETEIcean)
    - [GitHub actions](https://github.com/features/actions) to generate static webpages
- host webviews, project blogs: [gh-pages](https://pages.github.com/) on GitHub, GitLab etc.
- bibliographic database: [Zotero](https://www.zotero.org/groups/openarabicpe/items/)
- full-text search: [Google's programmable search engines](https://cse.google.com/cse?cx=012251040084107011117:jof1v_ejndo)

# OpenArabicPE

# Thank you!
## Thank you!

- Contributors to [OpenArabicPE][openarabicpe_website]: Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Daniel Kolland, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Contributors to [Project Jarāʾid][jaraid_website]: Hala Auji, Philippe Chevrant, Marina Demetriadou, Lamia Eid, Stacy Fahrenthold, Ulrike Freitag, Till Grallert, Rana Issa, Nicole Khayat, Peter Magierski, Leyla von Mende, Adam Mestyan, Christian Meier, Daniel Newman, Geoffrey Roper, Sinai Rusinek, Philip Sadgrove, Ola Seif, and Rogier Visser
- Links:
    + Slides: [https://tinyurl.com/dighis23-grallert](https://tillgrallert.github.io/slides/dh/2023-regensburg/index.html)
    + Project blog: [https://openarabicpe.github.io](https://openarabicpe.github.io)
    + Papers: <http://digitalhumanities.org/dhq/vol/16/2/000593/000593.html>, <https://doi.org/10/gkhrjr>
    + Mastodon: [\@tillgrallert\@digitalcourage.social](https://digitalcourage.social/@tillgrallert)
    + Email: <till.grallert@fu-berlin.de>, <till.grallert@hu-berlin.de>
- Licence: slides and images are licenced as [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

## References {#refs}