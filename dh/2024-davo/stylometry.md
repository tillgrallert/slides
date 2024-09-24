---
title: "Looking at the iceberg from below the waterline"
subtitle: "Stylometric authorship attribution for anonymous articles in Arabic periodicals from the early twentieth century"
panel: ""
event: "DAVO 2024"
author: Till Grallert
institute: 
    - "Humboldt-Universität zu Berlin, Institut für Geschichtswissenschaften"
    - "Methods Innovation Lab, NFDI4Memory"
email: till.grallert@hu-berlin.de
date: 2024-09-27
ORCID: orcid.org/0000-0002-5739-8094
lang: en-GB
url: https://tillgrallert.github.io/slides/dh/2024-davo/
bibliography: 
    - /Users/Shared/BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /Users/Shared/BachUni/research-projects/Sihafa/assets/bibliography/sihafa.csl.json
    - /Users/Shared/BachUni/applications/applications.csl.json
background-image: ../../assets/OpenArabicPE/front-pages_strip.png
nocite: |
    @Grallert2022DHQ; @Grallert+2020; @Romanov+2021; @RomanovGrallert2022Stylometry; @Grallert2023LookingIceberg
---

## outline

1. Background
    - Arab periodical studies
    - Research question
2. Method: stylometric authorship attribution
3. Corpus, data sets
4. Results

# Background
## Arabic periodicals

::: columns
:::: column

- Periodical press as agent of change
    + first mass medium
    + central medium of the literary and cultural Arabic renaissance (*nahḍa*)
    + medium of linguistic change
    + central forum for negotiations over modernity, nationalism, Islamism etc.

::::
:::: column

- Periodicals as *source* but not a *subject*
- Research is dominated by
    + national(ist) narratives
    + bias on two places and small no. of titles
    + implicit hypotheses

::::
:::

![Distribution of new Arabic periodical titles, 1799--1929](../../assets/jaraid/map-periodicals_World_1855-1929_temp-dist-status-y_5.gif){#fig:map-jaraid}

## Arabic periodicals

::: columns-3
:::: column

<!-- ![Title page of *al-Quds* #331, 10 Jan. 1913](../../assets/OpenArabicPE/front-pages/al-quds-v_5-i_331_annotated.jpg){#fig:al-quds} -->
![First page of the journal [*al-Muqtabas* 1(1)](https://openarabicpe.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_1.TEIP5.xml), 1906, Cairo](../../assets/OpenArabicPE/front-pages/al-muqtabas-m-v_1-i_1.png){#fig:muqtabas-1}

::::
:::: column

![Front page of the newspaper *al-Iqbāl* #1, 9 April 1902, Beirut](../../assets/OpenArabicPE/front-pages/al-iqbal-v_1-i_1.png){#fig:iqbal-1}

::::
:::: column

![Front page of the newspaper *Kawkab Amīrkā* #1, 15 April 1892, New York](../../assets/OpenArabicPE/front-pages/kawkab-amirka-v_1-i_1.png){#fig:kawkab-1}

::::
:::


<!-- - Green: Ottoman crescent with 3 stars and slogan of the Young Turk Revolution of 1908: "Liberty, Equality, Fraternity"
- Blue: French title
- Red: Date line according to 3 calendars
    + reformed Julian: 28 Dec. 1912
    + Gregorian: 10 Jan. 1913
    + Islamic: 2 Ṣafar 1331 -->

::: notes

- striking similarity in layouts of newspapers
    + despite temporal and geographic distance

:::

## Research interest: intellectual networks

::: columns
:::: column

![Undirected network of authors in *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *Lughat al-ʿArab*, and *al-Muqtabas*. Colour of nodes: betweenness centrality; size of nodes: number of periodicals; width of edges: number of articles.](../../assets/OpenArabicPE/networks/network_oape-p3a6afa20_authors_unimodal-n-size_out-degree-n-colour_betweenness-e-colour_grey.png){#fig:network-authors-2}

::::
:::: column

### Aims

- empirical testing of hypotheses
- evaluate existing literature

### Observations

<!-- * Nur wenige Knoten sind von relativer Bedeutung (14 von 319) -->
- very limited overlap between periodicals from the same place
- core network (14 of 319 nodes):
    - absent from the literature
    - suprising set up: many Iraqis (6), few Syrians (2), few Christians (2)

::::
:::

::: notes
- of the 14, Ayalon mentions only ʿIsā Iskandar al-Maʿlūf 
:::

## Problem: missing bylines

::: columns
:::: column

![](../../assets/clipart/iceberg-2070977_960_720.png)

::::
:::: column

- About 4/5 of all articles or 2/3 of all words carry no byline
* Commonly ignored in scholarship 
* Implicit hypothesis is implausible and untested
* Stylometric authorship attribution is untested for this material

::::
:::

# Method
## Stylometric authorship attribution

Authorship signal is prevalent in most frequent words, i.e. function words

::: columns
:::: column

### comparative method

- steps:
    1. compute frequencies for every text
    2. compare every text with every text
    3. validate through voting (*consensus*) of multiple iterations

::::
:::: column

### challenges

- novel application to Arabic and this genre
- comparison depends on input
- reliability depends on a minimal length of texts

::::
:::

::: notes

- stylometry is old, compution has supercharged it
- Computational Stylometry Group
    + Maciej Eder
    + Mike Kestemont
    + Jan Rybicki

:::

## Stylometry

- In R with the `stylo()` package [@Eder+2016b]
- Based on parameter settings established in our tests [@RomanovGrallert2022Stylometry]

::: columns
:::: column

### `stylo()` settings

- Tokens: words
- Sampling: 2500 tokens
- Most Frequent Features: 200--500 tokens, incremented by 100
- Culling: 0
- distance measure: Eder's simple delta

::::
:::: column

### Analysis

- edges (and nodes) tables from `stylo()`
- computing network measures with `tidygraph()` and `igraph()`
    + centrality
    + community detection
- plotting results with `ggraph()` and `ggplot2()`


::::
:::

::: notes

- Maxim designed and ran parameter test on a corpus of 300 nineteenth-century books
- I confirmed the viability of these settings in my work on periodicals

:::

## Parameter testing

[@RomanovGrallert2022Stylometry]

::: columns
:::: column

- [corpus](https://zenodo.org/record/5772261)
    + 300 books from 28 authors
    + 19th and early 20th century
- parameters
    + MFF: 100--500 tokens and character n-grams in increments of 100
    + culling: 0--50% in increments of 10 
    + distance measure: all 14
    + sample length: 100 to 12000 tokens in increments of 100

::::
:::: column

- testing
    + all possible combinations
    + Ward’s clustering (`ward.D2` in `hclust`) for authors and works
- infrastructure
    + Server from the [KITAB project]()
    + 20--30 cores
    + multiple weeks

::::
:::

## Parameter testing


![Plot of results from the parameter testing. Source: @RomanovGrallert2022Stylometry](../../assets/sihafa/stylometry/parameter-test.png){#fig:param-test}


# Corpus and data sets
## Corpus

| Periodical                      | Place             | Dates[^tb1]   | Vol.s   | No.s    | Words       | Articles | with author     | 2500+ words | words/ article | Authors | DOI                                                              |
| ------------------------------- | ----------------- | ------------- | ------: | ------: | ------:     | ------:  | ------:         | -----:      | ------:        | ------: | ------------------------                                         |
| [*al-Ḥaqāʾiq*][haqaiq_git]      | Damascus          | 1910--13      | 3       | 35      | 298090      | 389      | [41.90]{.green} | 22          | 832.66         | 104     | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) |
| [*al-Muqtabas*][muqtabas_git]   | Cairo, Damascus   | 1906--18      | [9]{.green}   | [96]{.green}  | [1981081]{.green} | [2964]{.green} | [12.72]{.red}   | [241]{.green}     | 873.34         | 140     | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   |
| [*al-Zuhūr*][zuhur_git]         | Cairo             | 1910--13      | 4       | 39      | 292333      | 436      | [41.51]{.green} | [6]{.red}     | 695.09         | 112     | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) |
| [*Lughat al-ʿArab*][lughat_git] | Baghdad           | 1911--14      | 3       | 34      | 373832      | 939      | 16.19           | 21          | 485.21         | 53      | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) |
| total                           |                   |               | 19      | 204     | 2945336     | 4728     |                 | 290         | 622.96         |         |                                                                  |
|                                 |                   |               |         |         |             |          |                 |             |                |         |                                                                  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [*al-Ustādh*][ustadh_git]       | Cairo             | [1892--93]{.red} | 1       | 42      | 221447      | 435      | [5.52]{.red}    | 13          | 582.21         | 8       | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) |

Table: Our corpus from "[Open Arabic Periodical Editions](https://openarabicpe.github.io/)" {#tbl:openarabicpe-corpus}

[^tb1]: The current cut-off date is 1918.

[muqtabas_git]: https://github.com/OpenArabicPE/journal_al-muqtabas
[haqaiq_git]: https://github.com/OpenArabicPE/journal_al-haqaiq
[lughat_git]: https://github.com/OpenArabicPE/journal_lughat-al-arab
[ustadh_git]: https://github.com/OpenArabicPE/journal_al-ustadh
[zuhur_git]: https://www.github.com/openarabicpe/journal_al-zuhur

::: notes

- human-transcribed full text from a major Arabic shadow library
- modelled in TEI/XML
- mark-up of  
    + sections
    + articles
    + heads
    + bylines, as far as they exist

:::

## Why this corpus?
### Collection and digitisation biases

::: columns
:::: wide

![Geographic distribution of Arabic periodical titles published across South West Asia and North Africa (SWANA) between 1789--1929. The size of the pie charts corresponds to the total number of titles published at a location. Slices show the percentage of known holdings and digitized collections](../../assets/jaraid/map-data-set-periodicals_1789-1929-scatterpie-mena-label_en.png){#fig:map-periodicals-status}

::::
:::: narrow

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

## Data sets

All data sets consist of plain text files with minimal normalisation generated from the TEI/XML in our corpus.

::: columns-3
:::: column

### Data set 1

- 215 articles of 2.500+ tokens
- 74 authors with only one or two texts
- 103 unattributed texts

::::
:::: column

### Data set 2

- 88 texts of 2.500+ tokens
- compilations of smaller anonymous texts from rubrics
- most likely written by editors

::::
:::: column

### Data set 3

- 612 full issues
- for basic sanity checks

::::
:::

::: notes

- data set 1 includes texts from some of the periodicals's known editors, it is unclear to which extent included authors could or should be considered potential candidates for authorship of the unattributed texts.
- data set 1: test the method
    - large number of authors with only a small number of text
    - large number of unattributed texts
    - relatively short texts (close to the minimal length)
    + unclear if the actual authors are part of the data set
    + -> **very different from [@RomanovGrallert2022Stylometry]'s test corpus**
- data set 2: test the hypothesis


:::

# Results
## Sanity check: data set 3

Questions:

1. Are individual periodicals stylistically distinguishable?
2. Do they a single auctorial voice?

::: columns
:::: column

![Network plot of stylometric similarity in data set 3. Node colours indicate periodicals: purple = al-Ḥaqāʾiq,  turquoise = al-Muqtabas, green = Lughat al-ʿArab, red = al-Zuhūr](../../assets/OpenArabicPE/stylometry/2023-paper/stylo_network-issues-size_degree-colour_publication.png){#fig:dataset3-publication}

::::
:::: column

![Network plot of stylometric similarity in data set 3. Node colours indicate communities established by the walktrap algorithm](../../assets/OpenArabicPE/stylometry/2023-paper/stylo_network-issues-size_degree-colour_walktrap.png){#fig:dataset3-walktrap}

::::
:::

::: notes

- two issues of al-Zuhūr are stylistically different from the rest of the journal 
    - These are issues no. 88 and 91 in the plot, which refer to vol.3, no.8 and 9.,
    - confirmed by community-detection algorithms 
    - might indicate a shift in editorship. 
- Similar shifts seemingly happened at other periodicals as well.
    - at least at al-Muqtabas as indicated by walktrap and Louvain.
        - There is one issue of al-Muqtbas, vol. 4, no.5-6, which is stylistically part of al-Zuhūr.
        - There are two issues of al-Muqtabas which are pretty close to al-Ḥaqāʾiq
    - using walktrap we get two communities at al-Ḥaqāʾiq as well.

:::

## Test the hypothesis: data set 1

Questions:

1. Do anonymous articles cluster by periodical? 
2. Can the owners-cum-editors present in this data set be considered strong candidates for their authorship?

::: columns
:::: column

![Network plot of stylometric similarity for all articles from data set 1. Node colours indicate periodicals: purple = al-Ḥaqāʾiq,  turquoise = al-Muqtabas, green = Lughat al-ʿArab, red = al-Zuhūr](../../assets/OpenArabicPE/stylometry/2023-paper/stylo_network-articles-w_2500-size_degree-colour_publication.png){#fig:articles-publications}

::::
:::: column

![Network plot of stylometric similarity for all articles from data set 1. Node colours indicate communities established by the Louvain algorithm](../../assets/OpenArabicPE/stylometry/2023-paper/stylo_network-articles-w_2500-size_degree-colour_louvain.png){#fig:articles-louvain}

::::
:::

::: notes

- both hypotheses can be rejected for al-Muqtabas and Lughat al-ʿArab, whose editors, Muḥammad Kurd ʿAlī, Anastās Mārī al-Karmalī, and  Kāẓim al-Duyalī, are present in the data set (labelled with their respective identifiers as oape:878, oape:227, and oape:396). 
- The anonymous articles from al-Muqtabas form two distinct clusters with substantial internal differences and thus force us to reject any notion of single authorship ([@fig:articles-louvain]). 
- neither Muḥammad Kurd ʿAlī nor Anastās Mārī al-Karmalī and Kāẓim al-Duyalī seemingly authored a significant number of articles in their respective journals.
- The small cluster of texts from al-Zuhūr in the top left can all be attributed to Shakespeare through close reading

:::

## Test the hypothesis on stronger candidates: data set 2

::: columns
:::: wide

![Network plot of stylometric similarity for anonymous articles in al-Muqtabas from data set 2 and articles by its publisher Muḥammad Kurd ʿAlī from data set 1. Node colours indicate communities established by the Louvain algorithm.](../../assets/OpenArabicPE/stylometry/2023-paper/stylo_network-sections-editors_muqtabas-size_degree-colour_louvain.png){#fig:muqtabas-editors-louvain}

::::
:::: narrow

Muḥammad Kurd ʿAlī might have authored some texts in his journal *al-Muqtabas* but he was certainly not alone

::::
:::
::: notes

we divided data set 2 by source publication and added texts from data set 1 authored by the owners-cum-editors.

:::

## Test the hypothesis on stronger candidates: data set 2

Adding unlikely contenders to amplify the signal

::: columns
:::: column

![Network plot of stylometric similarity for anonymous articles in al-Muqtabas from data set 2 and all attributed articles from data set 1. Node colours indicate communities established by the Louvain algorithm. Note how the anonymous articles cluster on the left.](../../assets/OpenArabicPE/stylometry/2023-paper/stylo_network-sections-authors_muqtabas-size_degree-colour_louvain.png){#fig:muqtabas-authors-louvain}

::::
:::: column

![Network plot of stylometric similarity for anonymous articles in Lughat al-ʿArab from data set 2 and all attributed articles from data set 1. Node colours indicate communities established by the Louvain algorithm. Note how the anonymous articles cluster in the top right.](../../assets/OpenArabicPE/stylometry/2023-paper/stylo_network-sections-authors_lughat-size_degree-colour_louvain.png){#fig:lughat-authors-louvain}

::::
:::

::: notes

- added all attributed articles from data set 1 as a control group. We argue that if they were less likely to be editors (and thus more stylistically different), they would push the assumed owner-com-editors closer to the anonymous articles.
- not the case for al-Muqtabas nor Lughat al-ʿArab. This indicates that Muḥammad Kurd ʿAlī and Anastās Mārī al-Karmalī should not be considered strong contenders for the authorship of anonymous  reporting in their journals. 
- We can also safely exclude all other 73 authors in data set 1 as potential candidates for the editorship.

:::

## All isn't in vain: individual authors

::: columns
:::: narrow

Let's return to a slightly different version of @fig:articles-publications ...

::::
:::: wide

![Bootstrap consensus network of data set 1, coloured by author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-w_2500-size_degree-colour_author-2022-09-09.png){#fig:network-author}

::::
:::

## All isn't in vain: individual authors
### Kāẓim al-Dujaylī

Anonymous travellogue in *Lughat al-ʿArab* most likely written by the magazine's editor Kāẓim al-Dujaylī

::: columns
:::: column

![Detail from @fig:network-author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-oape_396.png){#fig:network-detail-dujayli}

::::
:::: column

![Radar plot for the unattributed article (20) in @fig:network-detail-dujayli, ["Riḥla ilá Shufāthā", *Lughat al-ʿArab* 3(1), Aug. 1913](https://openarabicpe.github.io/journal_lughat-al-arab/tei/oclc_472450345-i_25.TEIP5.xml#div_7.d2e1438)](../../assets/OpenArabicPE/stylometry/stylo_NN_oclc.472450345_v.3_i.1_div_7.d2e1438_lollipop.png){#fig:radar-dujayli}

::::
:::

## All isn't in vain: individual authors
### Ibn al-Muqaffaʿ?

A cluster of texts potentially written by Ibn al-Muqaffaʿ (d. 759) and edited by Ṭāhir al-Jazāʾirī

::: columns
:::: column

![Detail from @fig:network-author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-oape_185.png){#fig:network-detail-muqaffa}

::::
:::: column

![Radar plot for the unattributed article (34) in @fig:network-detail-muqaffa, ["al-Adab al-ṣaghīr", *al-Muqtabas* 3(1), Sep. 1911](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_25.TEIP5.xml#div_3.d1e733)](../../assets/OpenArabicPE/stylometry/stylo_NN_oclc.4770057679_v.3_i.1_div_3.d1e733_lollipop.png){#fig:radar-muqaffa}

::::
:::

::: notes

- this is a case where the algorithm for extracting bibliographic information did not work as expected
    + the title clearly mentions Ibn al-Muqaffaʿ as the author

:::

## All isn't in vain: individual authors
### Shukrī al-ʿAsalī: resolving acronyms

Texts by Shukrī al-ʿAsalī, later MP for Damascus and co-editor of one of Muḥammad Kurd ʿAlī's newspapers

::: columns
:::: column 

![Detail from @fig:network-author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-oape_460.png){#fig:network-detail-asali}

<!-- this is currently the wrong image -->

::::
:::: column

![Radar plot for the attributed article (164) in @fig:network-detail-asali, [al-ʿAsalī, "al-Jabāya fī al-Islām", *al-Muqtabas* 4(2, 3), Feb., Mar. 1909](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_38.TEIP5.xml#div_4.d1e2328)](../../assets/OpenArabicPE/stylometry/stylo_oape.460_oclc.4770057679_v.4_i.2_div_4.d1e2328_lollipop.png){#fig:radar-asali}

::::
:::

::: notes

- This information could also be gathered from close reading
    + based on the title
    + the text in *al-Muqtabas* 4(2) mentions the one in 2(4) in a footnote, which, however, is not part of the transcription from Shamela
- authors:
    + 482: Jamāl al-Dīn al-Qāsimī

:::

# Conclusion
## Summary

- We tested and falsified a hypothesis: anonymous articles in *al-Muqtabas* from Cairo and, later, Damascus, and *Lughat al-ʿArab* from Baghdad were not authored by their respective owners-cum-editors.
- A small number of anonymous articles could be attributed

### Future work

- identify potential candidates for authorship
- build the necessary data sets for these candidates
- expand the scope by systematically digitising a representative sample of Arabic periodicals


## Thank you!

- Maxim Romanov for his work on parameter testing
- Contributors to OpenArabicPE: Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Daniel Kolland, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Links:
    + Slides: [https://tillgrallert.github.io/slides/dh/2024-davo/](https://tillgrallert.github.io/slides/dh/2024-davo/index.html)
    + Project blog: [https://openarabicpe.github.io](https://openarabicpe.github.io)
    + Papers: <https://doi.org/10.5281/zenodo.10159446>, <http://digitalhumanities.org/dhq/vol/16/2/000593/000593.html>, <https://doi.org/10/gkhrjr>
    + Mastodon: [\@tillgrallert\@digitalcourage.social](https://digitalcourage.social/@tillgrallert)
    + Email: <till.grallert@fu-berlin.de>, <till.grallert@hu-berlin.de>
- Licence: slides and images are licenced as [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

## References {#refs}