---
title: "We need to talk about Arabic!"
subtitle: "A practical critique of the hostility towards the second most common human writing system built into our quotidian digital infrastructures"
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

# Introduction
## My research interests 
### ... or what I would want to do

::: columns
:::: column

![Undirected network of authors in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, and *al-Muqtabas*. Colour of nodes: betweenness centrality; size of nodes: number of periodicals; width of edges: number of articles.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_authors_unimodal-n-size_out-degree-n-colour_betweenness-e-colour_grey.png){#fig:network-authors-1}

::::
:::: column

![Directed network of periodicals referenced in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, *al-Muqtabas*, and *al-Zuhūr*](../../assets/sihafa/networks/network_n_periodical-e_referenced-layout_fr-label_Latn.png){#fig:network-mentioned-periodicals-1}

::::
:::

<!-- ## My research interests

[... or what I would want to do]{.c_right}

![Bootstrap consencus network of stylometric similarity for anonymous articles in *al-Muqtabas* and all attributed articles in the OpenArabicPE data set](../../assets/OpenArabicPE/stylometry/stylo_network-sections-authors_muqtabas-size_degree-colour_louvain.png){#fig:stylo-muqtabas-anonymous}


::: notes

Note how the anonymous articles cluster on the left.

::: -->


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
    - Publish everything as Linked Open Data on [Wikidata](https://w.wiki/9UDd)

::::
:::: column

<!-- ![Periodicals by places of publication. Size of circles corresponds to the number of periodicals. Colour indicates the collection status: known (grün), digitised (blau), reminder (rot).](../../assets/jaraid/map-data-set-periodicals_1789-1929-scatterpie-mena-label_en.png){#fig:holding-stats} -->

![Periodicals by places of publication. Size of circles corresponds to the number of periodicals. Colour indicates the number of new titles per period.](../../assets/jaraid/map-periodicals_World_1855-1929_temp-dist-status-y_5.gif){#fig:history-arab-press}

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
    * letterform depends on position within the string (*allographs*): [ج جـ ـجـ ـج]{.c_rtl lang="ar"}
    * combination of basic letterforms (*archigraphemes*, Arab. *rasm*) and diacritic marks (*iʿjām*)
- diacritics 
    + reduce semantic ambiguity
    + subject to regional preferences and change of time 
- Vocalisation (*tashkīl*) is **optional** and changes the semantics 

::::
:::: column

![Beginning of @oclc_4770057679-i_13-div_8.d1e1249. Some ligatures are highlighted.](../../assets/dh/arabic-ligatures.png){#fig:zakham-ar}

![Pseudo-rasm of the text in @fig:zakham-ar. Automatically generated with @Pohl2022Rasmifize.](../../assets/dh/arabic_rasm.png){#fig:zakham-ar-rasm}

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
## multilinguality and *linguistic imperialism*

>Indigenous peoples have the right to revitalize, use, develop and transmit to future generations their histories, languages, oral traditions, philosophies, writing systems and literatures, and to designate and retain their own names for communities, places and persons.

<cite>[@UNDRIP2007, §13]<cite>

::: notes

The human condition, historically, is one of multilinguality. People speak different languages, dialects, sociolects etc. in different contexts: at home, at work, at social gatherings, for worship etc.. Sometimes we share a language with people across geographic distances, just as in this meeting, and sometimes, we do not understand our direct neighbours.

:::


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

- we talked about the situatedness of knowledge production and path dependencies
- Arabic script is much for challenging for mechanical reproduction than Latin script
- keyboard with 180 keys 
- two magazines  were required for a single Arabic fount

:::

## Encoding characters
### Unicode is awesome ...

... but many contemporary and historical human writing systems are not supported even in its latest iteration.

::: columns
:::: column

![Supported scripts in Unicode v1.0.0. Source: <https://www.worldswritingsystems.org>](../../assets/dh/unicode_1-0-0.png){#fig:unicode-1}

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

This ought to be the **perfect example**:

>As Ramsey Nasser notes in the overview of his programming language [ب ل ق]{.c_rtl .red lang="ar"} [pre-existing digital techonologies] are almost exclusively based on the ASCII character set

<cite>[@IsasiEtAl2023ModelMultilingual, 19]</cite>

[ب ل ق]{.c_rtl .red lang="ar"} should have been  [قلب]{.c_rtl .green lang="ar"}

::::
:::

::: notes

- yet, rendering depends on software support
- example from a £130 book from a major publisher
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
| community   | c. **420 mio.** Arabic speakers  | c. **6.2 mio.** inhabitants                                          |
| periodicals | 2054 newspapers and journals    | 125 newspapers                                                      |
| digitized   | [156]{.red} periodicals                 | [125]{.green} newspapers with more than 1.5 million pages                     |
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



::: columns
:::: column

![*al-Muqtabas* 6 on [HathiTrust](http://hdl.handle.net/2027/njp.32101073250910) (Original in Princeton) outside the USA](../../assets/OpenArabicPE/hathi_muqtabas-1.png){#fig:hathi-muqtabas-global}

cataloguing rules and algorithmic copyright detection cause further inaccessibilities

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
## build the digital commons **we need** <br/>with what **we have** at hand

::: columns
:::: narrow

1. Do it yourself
    - but not alone
2. keep it simple
    - for the sake of the people and spaceship earth
3. there will be a future

::::
:::: wide

>Contemporary research instrumentation in our field, from natural language processing to network analysis, involves complex mechanisms. Their inner workings often lie beyond the full comprehension of the casual user. **To use such tools well, we must, in some real sense, understand them better than the tool makers**. At the very least, we should know them well enough to comprehend their biases and limitations. 

<cite>[@Tenen2016BluntInstrumentalism, 85]</cite>

>this implies learning how to produce, disseminate, and preserve digital scholarship ourselves, **without the help we can’t get**, even as we fight to build the infrastructures we need at the intersection of, with, and beyond institutional libraries and schools.

<cite>[@Gil+2016, 29]</cite>


::::
:::

## Thank you!

- Contributors to [OpenArabicPE](https://openarabicpe.github.io/): Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Daniel Kolland, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Contributors to [Project Jarāʾid](https://projectjaraid.github.io/): Hala Auji, Philippe Chevrant, Marina Demetriadou, Lamia Eid, Stacy Fahrenthold, Ulrike Freitag, Till Grallert, Rana Issa, Nicole Khayat, Peter Magierski, Leyla von Mende, Adam Mestyan, Christian Meier, Daniel Newman, Geoffrey Roper, Sinai Rusinek, Philip Sadgrove, Ola Seif, and Rogier Visser

::: columns
:::: column

- Links:
    + Slides: <https://tillgrallert.github.io/slides/dh/2024-03-luxembourg/>
    + Project blog: [https://openarabicpe.github.io](https://openarabicpe.github.io)
    + Papers: <http://digitalhumanities.org/dhq/vol/16/2/000593/000593.html>, <https://doi.org/10/gkhrjr>
    + Mastodon: [\@tillgrallert\@digitalcourage.social](https://digitalcourage.social/@tillgrallert)
    + Email: <till.grallert@hu-berlin.de>


::::
:::: column

<svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="328" height="328" viewBox="0 0 328 328" shape-rendering="crispEdges"><rect x="0" y="0" width="328" height="328" fill="#fff"></rect><path fill="#000" d="M32 32h8v8H32V32M40 32h8v8H40V32M48 32h8v8H48V32M56 32h8v8H56V32M64 32h8v8H64V32M72 32h8v8H72V32M80 32h8v8H80V32M112 32h8v8H112V32M136 32h8v8H136V32M160 32h8v8H160V32M176 32h8v8H176V32M184 32h8v8H184V32M192 32h8v8H192V32M208 32h8v8H208V32M216 32h8v8H216V32M240 32h8v8H240V32M248 32h8v8H248V32M256 32h8v8H256V32M264 32h8v8H264V32M272 32h8v8H272V32M280 32h8v8H280V32M288 32h8v8H288V32M32 40h8v8H32V40M80 40h8v8H80V40M104 40h8v8H104V40M112 40h8v8H112V40M120 40h8v8H120V40M152 40h8v8H152V40M160 40h8v8H160V40M168 40h8v8H168V40M176 40h8v8H176V40M240 40h8v8H240V40M288 40h8v8H288V40M32 48h8v8H32V48M48 48h8v8H48V48M56 48h8v8H56V48M64 48h8v8H64V48M80 48h8v8H80V48M96 48h8v8H96V48M112 48h8v8H112V48M128 48h8v8H128V48M152 48h8v8H152V48M184 48h8v8H184V48M192 48h8v8H192V48M208 48h8v8H208V48M216 48h8v8H216V48M240 48h8v8H240V48M256 48h8v8H256V48M264 48h8v8H264V48M272 48h8v8H272V48M288 48h8v8H288V48M32 56h8v8H32V56M48 56h8v8H48V56M56 56h8v8H56V56M64 56h8v8H64V56M80 56h8v8H80V56M96 56h8v8H96V56M104 56h8v8H104V56M112 56h8v8H112V56M120 56h8v8H120V56M128 56h8v8H128V56M160 56h8v8H160V56M168 56h8v8H168V56M176 56h8v8H176V56M184 56h8v8H184V56M200 56h8v8H200V56M208 56h8v8H208V56M224 56h8v8H224V56M240 56h8v8H240V56M256 56h8v8H256V56M264 56h8v8H264V56M272 56h8v8H272V56M288 56h8v8H288V56M32 64h8v8H32V64M48 64h8v8H48V64M56 64h8v8H56V64M64 64h8v8H64V64M80 64h8v8H80V64M96 64h8v8H96V64M112 64h8v8H112V64M120 64h8v8H120V64M128 64h8v8H128V64M136 64h8v8H136V64M160 64h8v8H160V64M176 64h8v8H176V64M192 64h8v8H192V64M200 64h8v8H200V64M208 64h8v8H208V64M224 64h8v8H224V64M240 64h8v8H240V64M256 64h8v8H256V64M264 64h8v8H264V64M272 64h8v8H272V64M288 64h8v8H288V64M32 72h8v8H32V72M80 72h8v8H80V72M96 72h8v8H96V72M128 72h8v8H128V72M136 72h8v8H136V72M144 72h8v8H144V72M152 72h8v8H152V72M160 72h8v8H160V72M168 72h8v8H168V72M184 72h8v8H184V72M192 72h8v8H192V72M224 72h8v8H224V72M240 72h8v8H240V72M288 72h8v8H288V72M32 80h8v8H32V80M40 80h8v8H40V80M48 80h8v8H48V80M56 80h8v8H56V80M64 80h8v8H64V80M72 80h8v8H72V80M80 80h8v8H80V80M96 80h8v8H96V80M112 80h8v8H112V80M128 80h8v8H128V80M144 80h8v8H144V80M160 80h8v8H160V80M176 80h8v8H176V80M192 80h8v8H192V80M208 80h8v8H208V80M224 80h8v8H224V80M240 80h8v8H240V80M248 80h8v8H248V80M256 80h8v8H256V80M264 80h8v8H264V80M272 80h8v8H272V80M280 80h8v8H280V80M288 80h8v8H288V80M96 88h8v8H96V88M112 88h8v8H112V88M128 88h8v8H128V88M144 88h8v8H144V88M152 88h8v8H152V88M184 88h8v8H184V88M200 88h8v8H200V88M216 88h8v8H216V88M224 88h8v8H224V88M32 96h8v8H32V96M48 96h8v8H48V96M56 96h8v8H56V96M64 96h8v8H64V96M72 96h8v8H72V96M80 96h8v8H80V96M136 96h8v8H136V96M168 96h8v8H168V96M184 96h8v8H184V96M208 96h8v8H208V96M216 96h8v8H216V96M224 96h8v8H224V96M240 96h8v8H240V96M248 96h8v8H248V96M256 96h8v8H256V96M264 96h8v8H264V96M272 96h8v8H272V96M72 104h8v8H72V104M96 104h8v8H96V104M112 104h8v8H112V104M136 104h8v8H136V104M160 104h8v8H160V104M168 104h8v8H168V104M176 104h8v8H176V104M184 104h8v8H184V104M216 104h8v8H216V104M240 104h8v8H240V104M248 104h8v8H248V104M264 104h8v8H264V104M272 104h8v8H272V104M288 104h8v8H288V104M40 112h8v8H40V112M64 112h8v8H64V112M72 112h8v8H72V112M80 112h8v8H80V112M136 112h8v8H136V112M144 112h8v8H144V112M152 112h8v8H152V112M168 112h8v8H168V112M176 112h8v8H176V112M200 112h8v8H200V112M208 112h8v8H208V112M224 112h8v8H224V112M232 112h8v8H232V112M256 112h8v8H256V112M272 112h8v8H272V112M280 112h8v8H280V112M48 120h8v8H48V120M88 120h8v8H88V120M96 120h8v8H96V120M112 120h8v8H112V120M120 120h8v8H120V120M136 120h8v8H136V120M160 120h8v8H160V120M192 120h8v8H192V120M256 120h8v8H256V120M264 120h8v8H264V120M272 120h8v8H272V120M40 128h8v8H40V128M64 128h8v8H64V128M80 128h8v8H80V128M96 128h8v8H96V128M144 128h8v8H144V128M160 128h8v8H160V128M168 128h8v8H168V128M200 128h8v8H200V128M208 128h8v8H208V128M216 128h8v8H216V128M232 128h8v8H232V128M248 128h8v8H248V128M256 128h8v8H256V128M264 128h8v8H264V128M280 128h8v8H280V128M288 128h8v8H288V128M48 136h8v8H48V136M64 136h8v8H64V136M88 136h8v8H88V136M104 136h8v8H104V136M120 136h8v8H120V136M136 136h8v8H136V136M168 136h8v8H168V136M176 136h8v8H176V136M184 136h8v8H184V136M200 136h8v8H200V136M208 136h8v8H208V136M240 136h8v8H240V136M280 136h8v8H280V136M288 136h8v8H288V136M40 144h8v8H40V144M48 144h8v8H48V144M72 144h8v8H72V144M80 144h8v8H80V144M96 144h8v8H96V144M104 144h8v8H104V144M112 144h8v8H112V144M120 144h8v8H120V144M152 144h8v8H152V144M160 144h8v8H160V144M176 144h8v8H176V144M184 144h8v8H184V144M192 144h8v8H192V144M200 144h8v8H200V144M224 144h8v8H224V144M232 144h8v8H232V144M240 144h8v8H240V144M256 144h8v8H256V144M264 144h8v8H264V144M272 144h8v8H272V144M280 144h8v8H280V144M64 152h8v8H64V152M72 152h8v8H72V152M104 152h8v8H104V152M112 152h8v8H112V152M120 152h8v8H120V152M128 152h8v8H128V152M184 152h8v8H184V152M200 152h8v8H200V152M208 152h8v8H208V152M224 152h8v8H224V152M232 152h8v8H232V152M240 152h8v8H240V152M256 152h8v8H256V152M264 152h8v8H264V152M272 152h8v8H272V152M32 160h8v8H32V160M56 160h8v8H56V160M64 160h8v8H64V160M80 160h8v8H80V160M112 160h8v8H112V160M136 160h8v8H136V160M152 160h8v8H152V160M168 160h8v8H168V160M192 160h8v8H192V160M208 160h8v8H208V160M224 160h8v8H224V160M232 160h8v8H232V160M248 160h8v8H248V160M256 160h8v8H256V160M288 160h8v8H288V160M56 168h8v8H56V168M88 168h8v8H88V168M96 168h8v8H96V168M120 168h8v8H120V168M144 168h8v8H144V168M168 168h8v8H168V168M184 168h8v8H184V168M192 168h8v8H192V168M200 168h8v8H200V168M216 168h8v8H216V168M232 168h8v8H232V168M240 168h8v8H240V168M248 168h8v8H248V168M264 168h8v8H264V168M272 168h8v8H272V168M288 168h8v8H288V168M40 176h8v8H40V176M48 176h8v8H48V176M56 176h8v8H56V176M64 176h8v8H64V176M72 176h8v8H72V176M80 176h8v8H80V176M88 176h8v8H88V176M144 176h8v8H144V176M152 176h8v8H152V176M168 176h8v8H168V176M176 176h8v8H176V176M200 176h8v8H200V176M208 176h8v8H208V176M224 176h8v8H224V176M240 176h8v8H240V176M248 176h8v8H248V176M256 176h8v8H256V176M272 176h8v8H272V176M280 176h8v8H280V176M48 184h8v8H48V184M120 184h8v8H120V184M136 184h8v8H136V184M184 184h8v8H184V184M200 184h8v8H200V184M248 184h8v8H248V184M256 184h8v8H256V184M264 184h8v8H264V184M272 184h8v8H272V184M280 184h8v8H280V184M288 184h8v8H288V184M56 192h8v8H56V192M80 192h8v8H80V192M88 192h8v8H88V192M96 192h8v8H96V192M112 192h8v8H112V192M120 192h8v8H120V192M128 192h8v8H128V192M144 192h8v8H144V192M152 192h8v8H152V192M160 192h8v8H160V192M176 192h8v8H176V192M200 192h8v8H200V192M208 192h8v8H208V192M216 192h8v8H216V192M224 192h8v8H224V192M248 192h8v8H248V192M256 192h8v8H256V192M264 192h8v8H264V192M32 200h8v8H32V200M48 200h8v8H48V200M56 200h8v8H56V200M64 200h8v8H64V200M72 200h8v8H72V200M88 200h8v8H88V200M96 200h8v8H96V200M104 200h8v8H104V200M112 200h8v8H112V200M120 200h8v8H120V200M144 200h8v8H144V200M152 200h8v8H152V200M184 200h8v8H184V200M192 200h8v8H192V200M208 200h8v8H208V200M240 200h8v8H240V200M248 200h8v8H248V200M264 200h8v8H264V200M272 200h8v8H272V200M288 200h8v8H288V200M32 208h8v8H32V208M48 208h8v8H48V208M72 208h8v8H72V208M80 208h8v8H80V208M88 208h8v8H88V208M96 208h8v8H96V208M128 208h8v8H128V208M136 208h8v8H136V208M144 208h8v8H144V208M160 208h8v8H160V208M192 208h8v8H192V208M200 208h8v8H200V208M208 208h8v8H208V208M224 208h8v8H224V208M232 208h8v8H232V208M256 208h8v8H256V208M272 208h8v8H272V208M280 208h8v8H280V208M32 216h8v8H32V216M48 216h8v8H48V216M64 216h8v8H64V216M72 216h8v8H72V216M88 216h8v8H88V216M104 216h8v8H104V216M112 216h8v8H112V216M136 216h8v8H136V216M144 216h8v8H144V216M176 216h8v8H176V216M184 216h8v8H184V216M200 216h8v8H200V216M224 216h8v8H224V216M248 216h8v8H248V216M264 216h8v8H264V216M272 216h8v8H272V216M280 216h8v8H280V216M32 224h8v8H32V224M48 224h8v8H48V224M56 224h8v8H56V224M64 224h8v8H64V224M72 224h8v8H72V224M80 224h8v8H80V224M88 224h8v8H88V224M112 224h8v8H112V224M120 224h8v8H120V224M136 224h8v8H136V224M168 224h8v8H168V224M184 224h8v8H184V224M192 224h8v8H192V224M208 224h8v8H208V224M224 224h8v8H224V224M232 224h8v8H232V224M240 224h8v8H240V224M248 224h8v8H248V224M256 224h8v8H256V224M288 224h8v8H288V224M96 232h8v8H96V232M136 232h8v8H136V232M160 232h8v8H160V232M176 232h8v8H176V232M184 232h8v8H184V232M192 232h8v8H192V232M224 232h8v8H224V232M256 232h8v8H256V232M272 232h8v8H272V232M280 232h8v8H280V232M288 232h8v8H288V232M32 240h8v8H32V240M40 240h8v8H40V240M48 240h8v8H48V240M56 240h8v8H56V240M64 240h8v8H64V240M72 240h8v8H72V240M80 240h8v8H80V240M112 240h8v8H112V240M128 240h8v8H128V240M136 240h8v8H136V240M152 240h8v8H152V240M160 240h8v8H160V240M168 240h8v8H168V240M176 240h8v8H176V240M192 240h8v8H192V240M200 240h8v8H200V240M216 240h8v8H216V240M224 240h8v8H224V240M240 240h8v8H240V240M256 240h8v8H256V240M272 240h8v8H272V240M280 240h8v8H280V240M32 248h8v8H32V248M80 248h8v8H80V248M96 248h8v8H96V248M112 248h8v8H112V248M128 248h8v8H128V248M136 248h8v8H136V248M152 248h8v8H152V248M160 248h8v8H160V248M192 248h8v8H192V248M200 248h8v8H200V248M216 248h8v8H216V248M224 248h8v8H224V248M256 248h8v8H256V248M264 248h8v8H264V248M272 248h8v8H272V248M280 248h8v8H280V248M288 248h8v8H288V248M32 256h8v8H32V256M48 256h8v8H48V256M56 256h8v8H56V256M64 256h8v8H64V256M80 256h8v8H80V256M96 256h8v8H96V256M104 256h8v8H104V256M112 256h8v8H112V256M120 256h8v8H120V256M128 256h8v8H128V256M144 256h8v8H144V256M152 256h8v8H152V256M168 256h8v8H168V256M192 256h8v8H192V256M224 256h8v8H224V256M232 256h8v8H232V256M240 256h8v8H240V256M248 256h8v8H248V256M256 256h8v8H256V256M264 256h8v8H264V256M280 256h8v8H280V256M288 256h8v8H288V256M32 264h8v8H32V264M48 264h8v8H48V264M56 264h8v8H56V264M64 264h8v8H64V264M80 264h8v8H80V264M96 264h8v8H96V264M128 264h8v8H128V264M168 264h8v8H168V264M192 264h8v8H192V264M216 264h8v8H216V264M224 264h8v8H224V264M232 264h8v8H232V264M256 264h8v8H256V264M264 264h8v8H264V264M272 264h8v8H272V264M288 264h8v8H288V264M32 272h8v8H32V272M48 272h8v8H48V272M56 272h8v8H56V272M64 272h8v8H64V272M80 272h8v8H80V272M96 272h8v8H96V272M104 272h8v8H104V272M112 272h8v8H112V272M120 272h8v8H120V272M136 272h8v8H136V272M160 272h8v8H160V272M176 272h8v8H176V272M200 272h8v8H200V272M208 272h8v8H208V272M240 272h8v8H240V272M248 272h8v8H248V272M264 272h8v8H264V272M272 272h8v8H272V272M32 280h8v8H32V280M80 280h8v8H80V280M112 280h8v8H112V280M120 280h8v8H120V280M128 280h8v8H128V280M136 280h8v8H136V280M176 280h8v8H176V280M200 280h8v8H200V280M232 280h8v8H232V280M240 280h8v8H240V280M256 280h8v8H256V280M264 280h8v8H264V280M272 280h8v8H272V280M32 288h8v8H32V288M40 288h8v8H40V288M48 288h8v8H48V288M56 288h8v8H56V288M64 288h8v8H64V288M72 288h8v8H72V288M80 288h8v8H80V288M96 288h8v8H96V288M104 288h8v8H104V288M120 288h8v8H120V288M128 288h8v8H128V288M136 288h8v8H136V288M144 288h8v8H144V288M160 288h8v8H160V288M168 288h8v8H168V288M208 288h8v8H208V288M224 288h8v8H224V288M232 288h8v8H232V288M240 288h8v8H240V288M248 288h8v8H248V288M264 288h8v8H264V288M280 288h8v8H280V288"></path></svg>

::::
:::

## References {#refs}
