---
title: "We need to talk about Arabic!"
subtitle: "A practical critique of  the hostility towards the second most common human writing system built into our quotidian digital infrastructures"
author: Till Grallert
institute: 
    - Humboldt-Universität zu Berlin
    - Methods Innovation Lab (NFDI 4Memory)
date: 2024-03-16
event: "Exploring Epistemic Virtues and Vices"
url: https://tillgrallert.github.io/slides/dh/2024-03-luxembourg/
ORCID: orcid.org/0000-0002-5739-8094
lang: en
bibliography: 
    - /Users/Shared/BachUni/applications/applications.csl.json
    - /Users/Shared/BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /Users/Shared/BachUni/publications/github/pae326271/assets/bibliography/2023_dh-in-practice.csl.json
    - /Users/Shared/BachUni/publications/github/p8fc0a1bd/assets/bibliography/2023_clio-guide.csl.json
slide-level: 2
license: https://creativecommons.org/licenses/by-sa/4.0/
---

<!-- fix the problem with a cross reference to @fig:zakham-ar -->

## Outline

1. Introduction
2. Arabic
2. Multilinguality and linguistic imperialism of socio-technologic infrastructures
3. Arabic textual heritage online

# Introduction
## My research interests 

[... or what I would want to do]{.c_right}

::: columns
:::: column

![Undirected network of authors in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, and *al-Muqtabas*. Colour of nodes: betweenness centrality; size of nodes: number of periodicals; width of edges: number of articles.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_authors_unimodal-n-size_out-degree-n-colour_betweenness-e-colour_grey.png){#fig:network-authors-1}

::::
:::: column

![Directed network of periodicals referenced in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, *al-Muqtabas*, and *al-Zuhūr*](../../assets/sihafa/networks/network_n_periodical-e_referenced-layout_fr-label_Latn.png){#fig:network-mentioned-periodicals-1}

::::
:::

## My research interests

[... or what I would want to do]{.c_right}

![Bootstrap consencus network of stylometric similarity for anonymous articles in *al-Muqtabas* and all attributed articles in the OpenArabicPE data set](../../assets/OpenArabicPE/stylometry/stylo_network-sections-authors_muqtabas-size_degree-colour_louvain.png){#fig:stylo-muqtabas-anonymous}


::: notes

Note how the anonymous articles cluster on the left.

:::


## ... and what I spend my time on
### [Project Jarāʾid](https://projectjaraid.github.io/) (2012--) <br/>Closing the knowledge `<gap/>`

::: columns
:::: column

- Bibliographic record of **all** Arabic periodical titles published between 1798 and 1929
    - websites and open datasets ([TEI/XML](https://tei-c.org/)) for more than 3500 periodicals
    - additional authority files for c.2700 persons, 220 places, 180 libraries
- Unfunded collaboration with Adam Mestyan (Duke), "crowd"-sourcing
- Networking and reconciling existing information: 
    - Integration of holding information from library catalogues such as ZDB, AUB, BnF, HathiTrust
    - Publish everything as Linked Open Data on [Wikidata](https://wikidata.org/)

::::
:::: column

![Periodicals by places of publication. Size of circles corresponds to the number of periodicals. Colour indicates the collection status: known (grün), digitised (blau), reminder (rot).](../../assets/jaraid/map-data-set-periodicals_1789-1929-scatterpie-mena-label_en.png){#fig:holding-stats}

::::
:::

## ... and what I spend my time on
### Open Arabic Periodical Editions ([OpenArabicPE](https://openarabicpe.github.io), 2015--) <br/>Closing the infrastructural `<gap/>`

::: columns
:::: wide

- Digital scholarly editions
    + 6 Arabic magazines from Baghdad, Cairo, Damascus with c.800 issues and more than 9 million words.
    + full text and facsimiles modelled in TEI/XML
    - Bibliographic metadata (MODS, BibTeX, Zotero RDF)
    - Open licenses: [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)
       <!--  - on the article level for the entire corpus plus 2 additional magazines
        - on the issue level for 7 additional newspapers
        - on the title level for 3300+ periodicals (in collaboration with [Project Jarāʾid](https://projectjaraid.github.io)) -->
- Infrastructure:
    + [TEI Boilerplate]((https://github.com/openarabicpe/tei-boilerplate-arabic-editions)): static websites. No need for backend, database or internet connection
    + [GitHub](https://github.com/openarabicpe) / [Zenodo](https://zenodo.org): free hosting and archiving with DOIs
    - [Zotero group](https://zotero.org/groups/openarabicpe) as gateway to search/browse the corpus
- Workflows and tools

::::
:::: narrow

![[Webview of *al-Zuhur* 1(1)](https://openarabicpe.github.io/journal_al-zuhur/tei/oclc_1034545644-i_1.TEIP5.xml)](../../assets/OpenArabicPE/boilerplate_zuhur-v_1-i_1.png){#fig:webview-zuhur}

![[Webview of *al-Muqtabas* 3(2)](https://openarabicpe.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_26.TEIP5.xml)](../../assets/OpenArabicPE/boilerplate_muqtabas-v_3-i_2.png){#fig:webview-muqtabas}

::::
:::

# Background
## Late-Ottoman Eastern Mediterranean <br/>Diversity across the board

::: columns
:::: column

![Map showing the colonial spheres of interest agreed upon by France and UK. Signed by Sir Mark Sykes and Fr[ançois] Georges-Picot, 8 May 1916. Source: @SykesPicot1916Map](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f9/MPK1-426_Sykes_Picot_Agreement_Map_signed_8_May_1916.jpg/1055px-MPK1-426_Sykes_Picot_Agreement_Map_signed_8_May_1916.jpg){#fig:sykes-picot}

::::
:::: column

::: columns
:::: wide

### Languages

+ Administrative: Ottoman, Arabic, Persian
+ Quotidian: Turkic languages, Arabic, Greek, Slavic languages, Armenian, Ladino ...
+ Lithurgic: Arabic, Greek, Armenia, Coptic, Russian, Hebrew ...
+ Educational: Ottoman, Arabic, French, English, Russian ...

### Scripts

+ From right to left:
    * Arabic, Hebrew, Assyrian
+ Fro left to right:
    * Greek, Armenian, Latin, Cyrillic, Coptic

::::
:::: {.narrow .small-font}

### Religions

+ Muslims: Sunni, Shi'ite
+ Christians: div. Orthodox, Eastern Catholic, Western Catholic, Assyrian, Protestant ...
+ Jews: sephardic, ashkenazic
+ Zoroastrians


::: {.small-font}

### Calendars

- Islamic (*hijri*): **lunar**, observed, epoch begins with Muḥammad's exodus from Mecca
- Reformed Julian: **solar**; year begins on 1. January, epoch begins with Christ's birth
- Ottoman fiscal (*mālī*): **lunisolar**; year begins on 1. March, eepoch begins with Muḥammad's exodus from Mecca
- Gregorian: **solar**; year begins on 1. January, epoch begins with Christ's birth
- Jewish: **lunar**; epoch begins with the creation of the world

### Days, hours

- *alla turca*: day begins with sundown, 12 unequal hours each for day and night
- *alle franca*: day begins at midnight. 24 equinoctial hours

:::
::::
:::

::::
:::


::: notes

- this slide could/ should be split into multiple slides with more visual content

:::

<!-- add  slides on the disadvantages in the technical infrastructure -->

## "You are as beautiful as an additional hour of electricity!"

::: columns-3
:::: column

<blockquote class="twitter-tweet" data-partner="tweetdeck"><p lang="ar" dir="rtl">&quot;حبيبتي، انت جميلة، كساعة اضافية من الكهرباء&quot;<br><br>هذا غزل أحد المتظاهرين في ساحة التحرير اليوم.<br>رائعة حقيقة! <a href="http://t.co/KI8sAkY719">pic.twitter.com/KI8sAkY719</a></p>&mdash; aya mansour (\@aya_mansour_11_) <a href="https://twitter.com/aya_mansour_11_/status/627223846244847616?ref_src=twsrc%5Etfw">July 31, 2015</a></blockquote>

::::
:::: column

<blockquote class="twitter-tweet" data-partner="tweetdeck"><p lang="ar" dir="rtl">مريم .. أنتِ جميلة كساعة إضافية من الكهرباء ..<br><br>كتبها عاشق في فلسطين - غزة <a href="https://t.co/W3QvpmaE3O">pic.twitter.com/W3QvpmaE3O</a></p>&mdash; Jawdat Alsaleh (\@JawdatAlsaleh) <a href="https://twitter.com/JawdatAlsaleh/status/879683252184903681?ref_src=twsrc%5Etfw">June 27, 2017</a></blockquote>

::::
:::: column

<blockquote class="twitter-tweet" data-partner="tweetdeck"><p lang="ar" dir="rtl"><a href="https://twitter.com/hashtag/%D8%B3%D8%A3%D9%83%D8%AA%D8%A8_%D8%B9%D9%84%D9%89_%D8%A7%D9%84%D8%AC%D8%AF%D8%A7%D8%B1?src=hash&amp;ref_src=twsrc%5Etfw">#سأكتب_على_الجدار</a><br>أنتِ جميلة كساعة إضافية من الكهرباء <a href="https://t.co/jKpLnnlorR">pic.twitter.com/jKpLnnlorR</a></p>&mdash; A - M .. Syria (\@Azrael90) <a href="https://twitter.com/Azrael90/status/953594519836135436?ref_src=twsrc%5Etfw">January 17, 2018</a></blockquote>

::::
:::

::: notes

- very unequal access to the means of digital production
- 
:::

## "You are as beautiful as an additional hour of electricity!"

::: columns
:::: column

<iframe src="https://data.worldbank.org/share/widget?indicators=EG.ELC.ACCS.ZS&view=map" width='500' height='500' frameBorder='0' scrolling="no" ></iframe>

::::
:::: column

<iframe src="https://data.worldbank.org/share/widget?indicators=IT.NET.BBND.P2&view=map" width='500' height='500' frameBorder='0' scrolling="no" ></iframe>

::::
:::

::: notes

- very unequal access to the means of digital production
- sustainable development goals (SDG) of the UN
- electricity
    + 800 mio have no access
        * almost exclusively in the global south
        * vast majority in subsaharan Africa
    + by 2030 according to projections of the International Energy Agency (IEA): 
        * 600 mio
        * 33 per cent of all Africans
    - access: 
        + 250--500 kWh per year and household
        + less than 14 hours of a 100W lightbulb per day
 - internet
        + 36,6 percent of the world population, or 2,93 billion people do not participate
        + 85 per cent of them live in Africa, South, East and South-East Asia
        + lower speed
        + higher latency
        + higher cost per unit of traffic

:::

## Destruction

::: columns
:::: column

![Meeting room at the [Orient-Institut Beirut](https://orient-institut.org/) damaged by the Beirut Port explosion on 4 August 2020. Source: OIB](../../assets/dh/2020-08-04-oib-damage.jpg){#fig:oib-explosion}

::::
:::: column

![The National Archives of Syria in Damascus the day after their conflagration on 16. July 2023. Source: @aSbHrmAdFAwrkAmAHryqkbyr](https://static.srpcdigital.com/2023-07/256558.jpeg){#fig:archives-dam}

::::
:::

::: notes

- Port explosion on 4 Aug 2020
    + 2750t of ammonium nitrate
    + one of the largest non-nuclear explosions ever
- Conflagration of the Dār al-Wathāʾiq al-Tārīkhiyya in Sūq Sārūjā on 16 July 2023

:::

## Absences and exclusions

::: columns
:::: column

![Global distribution of DH centres. Source: [DH centerNet](http://dhcenternet.org/centers)](../../assets/dh/map_dhcenters.png){#fig:dh-centres}

::::
:::: column

<!-- <iframe src="https://hcommons.social/@dh_potsdam/110696533309515172/embed" width="400" allowfullscreen="allowfullscreen" sandbox="allow-scripts allow-same-origin allow-popups allow-popups-to-escape-sandbox allow-forms"></iframe> -->

![Global distribution of attendees at DH2023 in Graz. Source: [@Potsdam2023GeographyDH2023](https://digitalcourage.social/@dh_potsdam@hcommons.social/110696533594288097)](../../assets/maps/map_dh2023.jpeg){#fig:map-dh2023}

::::
:::

::: notes

- these distributions illustrate the gaps shown before
- access to infrastructures of the digital is limited in the Arabic world
- support for Arabic is limited in the digital
- I should also show a map of migrations showing the massive exodus from the Arabic speaking regions of the world
    + significant brain drain contributes to these absences

:::

# We need to talk about Arabic!
## Arabic

::: columns
:::: column

### Script

- Second most important script after Latin
    + currently used by 14 languages: Arabic, Persian, Urdu, Pashto, Uzbek, Uighur ...

::::
:::: column

### Language

+ Fifth most important language
    * One of six official languages of the United Nations
    * Official language in 26 countries
    * \>420 million speakers
+ Lithurgical language of 1,6 billion Muslims

::::
:::

![Approximate distribution of Arabic script use along current national boundaries [@Nemeth+2017, fig 1.1]](../../assets/maps/map_arabic-script-nemeth-fig_1-1-small.png){#fig:arabic-script}

## Arabic Script Grammar

::: columns
:::: column

+ Written from **right** to left (RTL)
+ Letters (*graphemes*)
    * mostly connected in direction of writing
    * letterform depends of position within the string (*allographs*): [ج جـ ـجـ ـج]{.c_rtl lang="ar"}
    * combination of basic letterforms (*archigraphemes*, Arab. *rasm*) and diacritic marks (*iʿjām*)
- diacritics 
    + reduce semantic ambiguity
    + subject to regional preferences and change of time 
- Vocalisation (*tashkīl*) is **optional** and changes the semantics 

::::
:::: column

![Beginning of @oclc_4770057679-i_13-div_8.d1e1249. Some ligatures are highlighted.](../../assets/dh/arabic-ligatures.png){#fig:zakham-ar}

![Pseudo-rasm of the text in `@fig:zakham-ar`. Automatically generated with @Pohl2022Rasmifize.](../../assets/dh/arabic_rasm.png){#fig:zakham-ar-rasm}

::::
:::

::: notes

- note: 
    + gaps within words
    + tilted base lines
    + ligatures
    + vertical overlap
- "*allograph*"  is Thomas Milo's terminology
- I am showing this in order to demonstrate the epistemic violence exercised by the paradigm of 
    + discrete letters, 
    + the Latin alphabet with its rather small number of letters, 
    + movable type printing
        * magazines become unfeasibly large
            - unwieldy
            - expensive: 
                + more material 
                + more machinery
                + more time for composing
- tilted baselines and vertical overlap of words makes things even more unwieldy
- 
:::

# multilinguality and *linguistic imperialism*
## multilinguality

>Indigenous peoples have the right to revitalize, use, develop and transmit to future generations their histories, languages, oral traditions, philosophies, writing systems and literatures, and to designate and retain their own names for communities, places and persons.

<cite>[@UNDRIP2007, §13]<cite>

::: notes

The human condition, historically, is one of multilinguality. People speak different languages, dialects, sociolects etc. in different contexts: at home, at work, at social gatherings, for worship etc.. Sometimes we share a language with people across geographic distances, just as in this meeting, and sometimes, we do not understand our direct neighbours.

:::

## Linguistic imperialism


>'Linguistic imperialism' is shorthand for a multitude of activities, ideologies, and structural relationships. Linguistic imperialism takes place within an overarching structure of asymmetrical North/ South relations, where language interlocks with other dimensions, cultural (particularly in education, science, and the media), economic and political

<cite>[@Phillipson1997RealitiesAndMyths, 239]</cite>

>The basis for the codes, languages, methodologies, and technical instruments of the digital humanities is English; the written and spoken language of all the main conferences, the most prestigious journals, the institutions that control the discipline, the organizations and international consortia, and the central authorities of knowledge is, with few exceptions, some dialect of British or American English.

<cite>[@Fiormonte+2021+TaxationagainstOverrepresentation, 334-335]</cite>

::: notes

- UNDRIP: United Nations Declaration on the Rights of Indigenous Peoples.
- this  ties back to the map I showed you at the very beginning

:::

## Technical affordances

![Arabic Linotype, 1910s. Source: [@Nemeth+2017, fig. 2.7]](../../assets/dh/arabic-linotype_nemeth-p_46.png){#fig:ar-linotype}

::: notes

- Arabic script is much for challenging for mechanical reproduction than Latin script
- keyboard with 180 keys 
- two magazines  were required for a single Arabic fount

:::

## Encoding characters
### Unicode is awesome ...

::: columns
:::: column

![Supported scripts in Unicode v1.0.0. Currently unsupported scripts. Source: <https://www.worldswritingsystems.org>](../../assets/dh/unicode_1-0-0.png){#fig:unicode-1}

::::
:::: column

![Currently unsupported scripts. Source: <https://www.worldswritingsystems.org>](../../assets/dh/unicode_15-0-0-missing-scripts.png){#fig:unicode-15-missing}

::::
:::


::: notes

- unicode can be traced back to the 1980s
- Unicode has become the dominant encoding standard in the 2000s
- almost universal support across operating systems has been driven by people's fondness of emojis
- Arabic has been part of Unicode since v 1.0.0
- linguisting imperialism
    + consortium: Adobe, Airbnb, Amazon, Apple, Yat, Google, ETCO, Meta, Microsoft, Netflix, SAP and Salesforce
    + character encoding is part of the history of a global hegemonic technology stack  bound up in historically contingent cultural traditions of the Global North. 
    + Mechanically and, later, electronically recording information in scripts other than Latin---particularly complex scripts with a much larger number of graphemes and different writing directions--- was never considered sufficiently important or profitable to be supported out-of-the-box.
    + Character encoding enforces Latin script grammar
        * unicode insufficiently distinguishes between languages and scripts
    + The standard is written in English
    + Current v 15:
        *  we know at least 300 writing systems
        *  127 are currently not encoded

:::

## Unicode is awesome ...

... but standards depend on implementation and software support

### Encoding nightmares

<!-- change this slide to show rendering issues ([@fig:arabic-fail-covid]) AND encoding issues -->

::: columns
:::: wide

![32 variants of encoding "Meccan" ([مكية]{lang="ar"}) [@Milo2014VisuallyMisleading, 4]](../../assets/dh/arabic-script_unicode-example-makkiyya-milo_4.png){#fig:arabic-mecca-1}

::::
:::: narrow

![In-browser search for "[مك]{lang="ar"}" in the Wikidata entry for "Mecca" ([Q5806](https://www.wikidata.org/wiki/Q5806))](../../assets/dh/arabic-script_unicode-example-wikidata_narrow.png){#fig:arabic-mecca-2 height="300px"}

::::
:::

::: notes

- unicode insufficiently distinguishes between languages and scripts
    + violating two of its principles
        * characters not glyphs
        * unification: no duplicates within a script
- yet, rendering depends on software support
    <!-- + see [@fig:arabic-fail-covid] -->


:::

## Unicode is awesome ...

... but standards depend on implementation and software support

### Rendering nightmares

::: columns
:::: wide

<!-- ![@IsasiEtAl2023ModelMultilingual, 19](../../assets/dh/spence-2023-p_19_arabic-failure.png){#fig:spence-arabic-fail} -->

<iframe src="https://fedihum.org/@jomla/112094232400811983/embed" width="400" allowfullscreen="allowfullscreen" sandbox="allow-scripts allow-same-origin allow-popups allow-popups-to-escape-sandbox allow-forms"></iframe>

::::
:::: narrow

This ought to be the **perfect example** (from a £130 book from a major publisher)

>As Ramsey Nasser notes in the overview of his programming language [ب ل ق]{.c_rtl .red lang="ar"} [pre-existing digital techonologies] are almost exclusively based on the ASCII character set

<cite>@IsasiEtAl2023ModelMultilingual, 19</cite>

[ب ل ق]{.c_rtl .red lang="ar"} should have been  [قلب]{.c_rtl .green lang="ar"}

::::
:::

::: notes

- yet, rendering depends on software support
    <!-- + see [@fig:arabic-fail-covid] -->


:::

## Unicode is awesome ...

<!-- [... but standards depend on implementation and software support]{.c_right} -->

... did I mention industry consortia?

>HTML elements all have names that only use ASCII alphanumerics [@HTMLLivingStandard2023, §13.1.2]

::: columns
:::: column

![Rendered HTML with the built-in default CSS for @oclc_4770057679-i_13-div_8.d1e1249. The test file is available [online](https://doi.org/10.5281/zenodo.7781543)](../../assets/dh/arabic_failure-browser.png){#fig:zakham-ar-failure}

::::
:::: column

![HTML-Code for @fig:zakham-ar-failure in Visual Code Studio. By default, non-ASCII characters are visually highlighted](../../assets/dh/html_vscode.png){#fig:html}

::::
:::
::: notes

- Arabic has been part of Unicode since its inception
- yet, software support is a different question, as we have seen 
- HTML5 is a *living standard* maintained by yet another consortium Web Hypertext Application Technology Working Group (WHATWG) 
    + members are leading browser vendors such as Apple, Google, Microsoft and Mozilla
    + all but Mozilla are also members of the Unicode consortium
- `@lang` attribute not used by standard CSS
    + everyone has to add `*[lang="ar"] {direction:rtl;}`

:::


## Bidirectional texts

The mandatory XML declaration `<?xml version="1.0" encoding="UTF-8"?>` sets left-to-right as the base direction.

::: columns
:::: wide

![Bi-directional TEI/XML at the beginning of @oclc_1034545644-i_15-div_1.d2e634. Arrows indicate the reading direction. Numbers indicate reading order.](../../assets/OpenArabicPE/xml_zuhur-v_2-i_4_annotated.png){#fig:bidi-xml}

::::
:::: narrow

![The TEI/XML from @fig:bidi-xml in [oXygen](https://www.oxygenxml.com/)'s  author mode. Styling relies on CSS.](../../assets/OpenArabicPE/oxygen_zuhur-author_small.png){#fig:zuhur-oxygen}

::::
:::
::: notes

- the Oxygen developers added support for Arabic in `@xml:lang` on our suggestion in 2015.
- but only for TEI/XML and not for all RTL languages.

:::

<!-- ## Transliteration, the undead solution of yore

Transliteration into Latin script served the need of colonial administrations and academics with the technological affordances of the time.



::: columns-3
:::: column

### Amīrkā wa ʿulamāʾ al-ʿArab

>Kānat Amīrkā majhūla ʿinda abnāʾ al-qarn al-khāmis ʿashr bi-dalīl an al-muʾarrikhīn fī dhalika al-ʿahd lam yadhkarū ʿanhā siwā akhbār iktishāfihā fī awākhir dhalika al-qarn.

<cite>Transliteration according to the *International Journal of Middle East Studies*</cite>


::::
:::: column

### Amīrkā wa ʿulamāʾ al-ʿarab

>Kānat Amīrkā ma[ǧ]{.red}hūla ʿinda abnāʾ al-qarn al-[ḫ]{.red}āmis ʿa[š]{.red}r bi-dalīl an al-muʾarri[ḫ]{.red}īn fī [ḏ]{.red}alika al-ʿahd lam ya[ḏ]{.red}karū ʿanhā siwā a[ḫ]{.red}bār ikti[š]{.red}āfihā fī awā[ḫ]{.red}ir [ḏ]{.red}alika al-qarn.

<cite>Transliteration according to the *Deutsche Morgenländische Gesellschaft*</cite>

::::
:::: column

### Amīrikā wa-ʻulamāʼ al-ʻArab

>Kānat Amīrikā majhūlah [ʻ]{.red}inda abnā[ʼ]{.red} al-qarn al-khāmis [ʻ]{.red}ashar bi-dalīl an al-mu[ʼ]{.red}arrikhīn fī dhālika al-[ʻ]{.red}ahd lam [ydhkrwā]{.red} [ʻ]{.red}anhā saw[á]{.red} Akhbār [aktshāfhā]{.red} fī awākhir dhālika al-qarn

<cite>Automated ALA-LC transcription into Latin script with the [romanize Arabic demo](http://romanize-arabic.camel-lab.com)</cite>

::::
:::

::: notes

- Depend on input and output **languages**
- Subject to traditions and taste
- Error prone

::: -->

## Transliteration, the undead solution of yore

Transliteration into Latin script served the need of colonial administrations and academics with the technological affordances of the time.

::: columns-3
:::: column

### [مرآة الشرق]{lang="ar"}

The Arabic original

### Meraat al-Sherk

The official transcription provided by the paper's masthead

::::
:::: column

![Front page of *Mirʾāt al-Sharq* #192, 22 Nov. 1922, Jerusalem. Source: [EAP](https://eap.bl.uk/archive-file/EAP119-1-24-1).](https://images.eap.bl.uk/EAP119/EAP119_1_24_1/1.jp2/full/600,/0/gray.jpg){#fig:mirat}

::::
:::: column

### Mirʾāt al-Sharq

Following the system of the *International Journal of Middle East Studies* (IJMES)

### Mirʾāt aš-Šarq

Following the system of the *Deutsche Morgenländische Gesellschaft* (DMG)

### mrMp Alcrq

Buckwalter transliteration

::::
:::

::: notes

- transliteration
    + Depend on input and output **languages**
    - Subject to traditions and taste
    - Error prone
    - if 1:1 grapheme replacement is intended, it becomes unreadable for casual readers
- published by Būlus Shaḥāda in Jerusalem between 1919 and 1938 

:::

# Arabic textual heritage online
## The long tail of ASCII in discovery systems

::: columns-3
:::: column

### [الجنة]{lang="ar"}?

No Arabic script

![Search in [ZDB](https://zdb-katalog.de/list.xhtml?t=الجنة) for "[الجنة]{lang="ar"}"](../../assets/jaraid/zdb_janna-ar.png){#fig:zdb-ar}

::::
:::: column

### al-Ǧanna?

Which Latinized transcription was used?

![Search in [ZDB](https://zdb-katalog.de/list.xhtml?t=al-Ǧanna) for "al-Ǧanna"](../../assets/jaraid/zdb_janna-ar-Latn.png){#fig:zdb-dmg}

::::
:::: column

### Ganna!

What are the normalization rules for the search algorithm?

![Search in [ZDB](https://zdb-katalog.de/list.xhtml?t=Ganna) for "Ganna"](../../assets/jaraid/zdb_janna-ar-Latn-no-al.png){#fig:zdb-functional}

::::
:::

::: notes

- catalogue could be searched in Arabic but the data is missing
- catalogues are historical artefacts
    + digitisation of catalogues: NOT re-cataloguing of original material
        * card catalogue
        * ASCII OPAC
        * automated transcription of the card catalogue
        * human cataloguers depend on the technology they have at hand, which means they might be unable to enter the correct string
        * errors perpetuate
- Latin input is mostly reduced to ASCII
    + Hamza and ʿAyn escape this algorithm on ZDB
- determined article is not automatically removed
- The choices are not transparently documented
- no software on-screen keyboards provided
- additional problems
    + catalogues are inherently local documents
    + aggregated, if at all, on a national level
    + frequently accessible only through Web interfaces and not APIs

:::

<!-- # Digitisation bias -->
## Digitisation bias
### Collection biases perpetuated

::: columns
:::: column

![Periodicals and their holding institutions](../../assets/jaraid/map-data-set-periodical-holdings-med-na_mapped.png){#fig:holding-map}

::::
:::: column

|      periodicals       | --1918 |       | --1929 |               |
|  :-------------------  | ----:  | ----: | ----:  |     ----:     |
|       published        |  2054  |       |  3550  |               |
|     known holdings     |  540   |       |  775   |               |
|       % of total       |        | 26.29 |        | [21.83]{.red} |
|------------------------|--------|-------|--------|---------------|
| digitized              |    156 |       |    233 |               |
| % of total             |        |  7.59 |        | [6.56]{.red}  |
|------------------------|--------|-------|--------|---------------|
| multiple digitisations |     51 |       |     66 |               |
| % of total             |        |  2.48 |        | 1.86          |
| % of digitised         |        | 32.69 |        | [28.33]{.red} |

Table: Periodical holdings and digitization {#tbl:jaraid-holdings}

::::
:::

::: notes

- collection bias is more of a knowledge bias
- While the digitization quote of roughly 50% of titles in collections is surprisingly high, it must be kept in mind that we cannot resolve information on the extent of digitization. Even if only a single issue of hundreds published was digitized, the periodical title will be included in this count.
- 66 periodicals or 28,33% have been digitized by multiple institutions and 21 of this subset by three and more.

:::

## Digitisation bias
### mind the `<gap/>`!

|             | Arabic periodicals (1798--1918) | [WWI as mirrored by Hessian regional papers](https://hwk1.hebis.de) |
|-------------|---------------------------------|---------------------------------------------------------------------|
| community   | c. 420 million Arabic speakers  | c. 6.2 million inhabitants                                          |
| periodicals | 2054 newspapers and journals    | 125 newspapers                                                      |
| digitized   | 156 periodicals                 | 125 newspapers with more than 1.5 million pages                     |
| type        | mostly facsimiles               | facsimiles and full text                                            |
| access      | paywalls, geo-fencing           | open access                                                         |
| interface   | mostly foreign languages only   | local and foreign languages                                         |

Table: Comparison of digitized periodicals between the Global South and the Global North {#tbl:digitisation}


::: columns
:::: column

![Map of Arabic dialects. Source: [reddit](https://www.reddit.com/r/MapPorn/comments/337ws9/arabic_dialects_map_os_2000x1130)](../../assets/maps/lMBwUARaIVBp5EUfx5yp4onMAtfAQsgRevtxTopNl98.png.webp){#fig:map-arabic-dialects}

::::
:::: column

![Map of Hesse in Europe. Source: <https://www.iz.sk/sk/projekty/regiony-eu/DE7>](../../assets/maps/map_hesse-europe.png){#fig:map-hesse}

::::
:::

::: notes

- price of digitisation is part of the equation
- infrastructures of knowledge creation 
- linguistic imperialism embodied in the technology stack

:::

## mind the `<gap/>`!
### Interfaces

![Interface of the [Translatio](https://digitale-sammlungen.ulb.uni-bonn.de/ulbbnioa/periodical/titleinfo/3384757?lang=en) project (Bonn). Facsimile of Arabic original on the left. Yellow = English UI; purple = Arabic metadata in DMG transcription;  green = German metadata](../../assets/OpenArabicPE/translatio_interface-languages_annotated.png){#fig:translatio-interface}

## mind the `<gap/>`!
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

## Quality of metadata

Bibliographic metadata is faulty throughout, mostly unstructured, and subject to *linguistic imperialism*

::: columns
:::: column

![@oclc_4770057679-i_61-div_21.d1e2838 on [Shamela](http://shamela.ws/browse.php/book-26523#page-4046) as it appeared in 2019](https://openarabicpe.github.io/slides/assets/shamela_muqtabas-annotated.png){#fig:muqtabas-6-2-shamela-2}

::::
:::: column

![Facsimile of the same section of @oclc_4770057679-i_61-div_21.d1e2838 from [EAP](https://eap.bl.uk/
)](../../assets/OpenArabicPE/eap119-1-4-5-muqtabas-133_annotated.jpg){#fig:muqtabas-6-2-133-eap-2}

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

## mind the `<gap/>`!
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


## machine-learning approaches to OCR

>For old prints, there's [...] kraken/calamari for coders, Transkribus if you've got money and just want to have the results[,] and OCR-D if you've got an IT department.

<cite>[@Winkler20230307OCR]</cite>

::: columns
:::: narrow

| training set     | *al-Ustādh*        | *al-Muqtabas*    |
| ---------------- | -----------------: | ---------------: |
| words            | 192829             | 11116            |
| lines            | 18732              | 1013             |
| epochs           | 200                | 200              |
| CER train        | 2.01               | 0.07             |
| CER validation   | [**2.09**]{.green} | [**8.40**]{.red} |

Table: Evaluation of my our Transkribus models {#tbl:ocr-ar-ml}

::::
:::: wide

![Transkribus web-app showing results of our model for *al-Ḥasnāʾ* 1(1)](../../assets/OpenArabicPE/transkribus_hasna-v_1-i_1.png){#fig:transkribus-web-app}

::::
:::

::: notes

- models were trained in late 2019 in collaboration with Sinai Rusinek
- results are great (layout recognition still lacking)
    + *al-Muqtabas* model suffers from over-fitting
    + digitised collections need to be re-processed (expensive)
- OpenITI
    + Mellon fund for model training to re-process Arabic-script material on HathiTrust

:::

# Conclusion
## Conclusion

- minimal computing
- be your own tool builder

## Thank you!

- Contributors to [OpenArabicPE](https://openarabicpe.github.io/): Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Daniel Kolland, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Contributors to [Project Jarāʾid](https://projectjaraid.github.io/): Hala Auji, Philippe Chevrant, Marina Demetriadou, Lamia Eid, Stacy Fahrenthold, Ulrike Freitag, Till Grallert, Rana Issa, Nicole Khayat, Peter Magierski, Leyla von Mende, Adam Mestyan, Christian Meier, Daniel Newman, Geoffrey Roper, Sinai Rusinek, Philip Sadgrove, Ola Seif, and Rogier Visser
- Links:
    + Slides: <https://tillgrallert.github.io/slides/dh/2024-03-luxembourg/>
    + Project blog: [https://openarabicpe.github.io](https://openarabicpe.github.io)
    + Papers: <http://digitalhumanities.org/dhq/vol/16/2/000593/000593.html>, <https://doi.org/10/gkhrjr>
    + Mastodon: [\@tillgrallert\@digitalcourage.social](https://digitalcourage.social/@tillgrallert)
    + Email: <till.grallert@hu-berlin.de>

## References {#refs}
