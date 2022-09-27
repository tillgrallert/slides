---
title: "Looking at the iceberg from below the waterline"
subtitle: "Stylometric authorship attribution for anonymous periodical articles"
panel: "Computational contributions to the Social and Cultural History of the Islamicate World"
event: "#DOT2022"
author: Till Grallert
institute: Humboldt-Universität zu Berlin
email: till.grallert@hu-berlin.de
date: 2022-09-12 
ORCID: orcid.org/0000-0002-5739-8094
lang: en-GB
bibliography: 
    - /Users/Shared/BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /Users/Shared/BachUni/research-projects/Sihafa/assets/bibliography/sihafa.csl.json
    - /Users/Shared/BachUni/applications/applications.csl.json
nocite: |
	@Grallert2022DHQ; @Grallert+2020
---

## outline

1. Background
2. Method and corpus
3. Results

# Background {data-background-image="../../assets/OpenArabicPE/front-pages_strip.png" data-background-size="90%"}
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

::: columns
:::: column

![Title page of *al-Quds* #331, 10 Jan. 1913](../../assets/OpenArabicPE/front-pages/al-quds-v_5-i_331_annotated.jpg){#fig:al-quds}

::::
:::: column

- Green: Ottoman crescent with 3 stars and slogan of the Young Turk Revolution of 1908: "Liberty, Equality, Fraternity"
- Blue: French title
- Red: Date line according to 3 calendars
    + reformed Julian: 28 Dec. 1912
    + Gregorian: 10 Jan. 1913
    + Islamic: 2 Ṣafar 1331

::::
:::

## Research interest: intellectual networks

There will be a [paper](https://tillgrallert.github.io/slides/dh/2022-dot-periodicals/index.html) on Wednesday

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
- plotting results with `ggpragh()` and `ggplot2()`


::::
:::

::: notes

- Maxim designed and ran parameter test on a corpus of 300 nineteenth-century books
- I confirmed the viability of these settings in my work on periodicals

:::

## Corpus

| Periodical                      | Place             | Dates[^tb1]   | Vol.s   | No.s    | Words       | Articles | with author | 2500+ words | words/articles | Authors | DOI                                                              |
| ------------------------------- | ----------------- | ------------- | ------: | ------: | ------:     | ------:  | ------:     | -----:      | ------:        | ------: | ------------------------                                         |
| [al-Ḥaqāʾiq][haqaiq_git]        | Damascus          | 1910--13      | 3       | 35      | 298090      | 389      | **41.90**   | 22          | 832.66         | 104     | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) |
| [al-Muqtabas][muqtabas_git]     | Cairo, Damascus   | 1906--18      | **9**   | **96**  | **1981081** | **2964** | 12.72       | **241**     | 873.34         | 140     | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   |
| [al-Ustādh][ustadh_git]         | Cairo             | 1892--93      | 1       | 42      | 221447      | 435      | 5.52        | 13          | 582.21         | 8       | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) |
| [al-Zuhūr][zuhur_git]           | Cairo             | 1910--13      | 4       | 39      | 292333      | 436      | **41.51**   | 6           | 695.09         | 112     | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) |
| [Lughat al-ʿArab][lughat_git]   | Baghdad           | 1911--14      | 3       | 34      | 373832      | 939      | 16.19       | 21          | 485.21         | 53      | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) |
| **total**                       |                   |               | 20      | 246     | 3166783     | 5163     |             | 303         | 613.36         |         |                                                                  |

Table: Our corpus from "[Open Arabic Periodical Editions](https://openarabicpe.github.io/)" {#tbl:openarabicpe-corpus}

[^tb1]: The current cut-off date is 1918.

[muqtabas_git]: https://github.com/OpenArabicPE/journal_al-muqtabas
[haqaiq_git]: https://github.com/OpenArabicPE/journal_al-haqaiq
[lughat_git]: https://github.com/OpenArabicPE/journal_lughat-al-arab
[ustadh_git]: https://github.com/OpenArabicPE/journal_al-ustadh
[zuhur_git]: https://www.github.com/openarabicpe/journal_al-zuhur

## Corpus

Plain text files of >2500 words

::: columns
:::: column

- corpus 1: 303 individual articles
    + 76 unique authors
    + 190 anonymous articles

-> **very different from Maxim Romanov's test corpus**

::::
:::: column

- corpus 2: 88 sections of anonymous articles from 2 journals
- corpus 3: 246 full issues from 5 journals
- corpus 4: 6 books by Muḥammad Kurd ʿAlī

::::
:::

# Results
## articles

We found the spaghetti monster!

![Bootstrap consensus network, coloured by author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-w_2500-size_degree-colour_author-2022-09-09.png){#fig:network-author}

::: notes

- centrality measure
	+ degree: 
		* number of connections
		* local measure
- authorship
	+ 116 attributed texts
	+ 112 unattributed
	+ 75 authors
:::

## Zooming in: Kāẓim al-Dujaylī

Anonymous travellogue in *Lughat al-ʿArab* most likely written by the magazine's editor Kāẓim al-Dujaylī

::: columns
:::: column

![Detail from @fig:network-author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-oape_396.png){#fig:network-detail-dujayli}

::::
:::: column

![Radar plot for the unattributed article (20) in @fig:network-detail-dujayli, ["Riḥla ilá Shufāthā", *Lughat al-ʿArab* 3(1), Aug. 1913](https://openarabicpe.github.io/journal_lughat-al-arab/tei/oclc_472450345-i_25.TEIP5.xml#div_7.d2e1438)](../../assets/OpenArabicPE/stylometry/stylo_NN_oclc.472450345_v.3_i.1_div_7.d2e1438_lollipop.png){#fig:radar-dujayli}

::::
:::


## Zooming in: Ibn al-Muqaffaʿ?

A cluster of texts potentially written by Ibn al-Muqaffaʿ (d. 759) and edited by Ṭāhir al-Jazāʾirī

::: columns
:::: column

![Detail from @fig:network-author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-oape_185.png){#fig:network-detail-muqaffa}

::::
:::: column

![Radar plot for the unattributed article (34) in @fig:network-detail-muqaffa, ["al-Adab al-ṣaghīr", *al-Muqtabas* 3(1), Sep. 1911](https://OpenArabicPE.github.io/journal_al-muqtabas/teioclc_4770057679-i_25.TEIP5.xml#div_3.d1e733)](../../assets/OpenArabicPE/stylometry/stylo_NN_oclc.4770057679_v.3_i.1_div_3.d1e733_lollipop.png){#fig:radar-muqaffa}

::::
:::

::: notes

- this is a case where the algorithm for extracting bibliographic information did not work as expected
	+ the title clearly mentions Ibn al-Muqaffaʿ as the author

:::

## Zooming in: William Shakespeare

Unmarked translations of Shakespeare's "Julius Caesar" in *al-Zuhūr*

::: columns
:::: column

![Detail from @fig:network-author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-oape_760.png){#fig:network-detail-shakespeare}

::::
:::: column

![Radar plot for the attributed article in @fig:network-detail-shakespeare, [Shakespear, "Yūliyūs Qayṣar", *al-Zuhūr* 3(4), Oct. 1912](https://openarabicpe.github.io/journal_al-zuhur/tei/oclc_1034545644-i_27.TEIP5.xml#div_1.d2e1819)](../../assets/OpenArabicPE/stylometry/stylo_oape.760_oclc.1034545644_v.3_i.6_div_1.d2e1819_lollipop.png){#fig:radar-shakespeare}

::::
:::

::: notes

- one case of faulty transcription by al-Maktaba al-Shamela: *būlūs qayṣar*
- the fourth installment of the play was too short to make it into the corpus
- #3 is also a play featuring Antonius, Casius, Brutus -> https://openarabicpe.github.io/journal_al-zuhur/tei/oclc_1034545644-i_30.TEIP5.xml#div_1.d2e2328
	+ but kept under the title of "Fukaha ilá madāris al-banāt" and a brief introductory scene

:::

## Zooming in: Charles Seignobos

Historical texts by Charles Seignobos translated by Muḥammad Kurd ʿAlī. 

When does the distance measure become unrealiable?

::: columns
:::: column 

![Detail from @fig:network-author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-oape_741.png){#fig:network-detail-seignobos}

::::
:::: column

![Radar plot for the attributed article (201) in @fig:network-detail-seignobos, [Seignobos, "al-Yūnān", *al-Muqtabas* 2(5), June 1907](https://OpenArabicPE.github.io/journal_al-muqtabas/tei/oclc_4770057679-i_17.TEIP5.xml#div_9.d1e1431)](../../assets/OpenArabicPE/stylometry/stylo_oape.741_oclc.4770057679_v.2_i.5_div_9.d1e1431_lollipop.png){#fig:radar-seignobos}

::::
:::

::: notes

- Which values of the distance measure are close enough to be considered?
- The text of Jibrāʾīl Madīnā is closer than other texts by Seignobos

:::

## owners-cum-editors as authors?
### *al-Muqtabas*

:::{.c_width-30 .c_right}

Muḥammad Kurd ʿAlī most likely not the author

:::
:::{.c_width-60 .c_left}

![Anonmyous sections and editors, coloured by author](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_muqtabas-size_degree-colour_author.png)

:::

## owners-cum-editors as authors?
### *al-Muqtabas*

:::{.c_width-30 .c_right}

Multiple anonymous candidates?

:::
:::{.c_width-60 .c_left}

![Anonmyous sections and editors, coloured by community](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_muqtabas-size_degree-colour_louvain.png)

:::

## owners-cum-editors as authors?
### *Lughat al-ʿArab*

:::{.c_width-30 .c_right}

Authorship of Anastās Mārī al-Karmalī and Kāẓim al-Duyalī more likely

:::
:::{.c_width-60 .c_left}

![Anonmyous sections and editors, coloured by author](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_lughat-size_degree-colour_author.png)

:::

## owners-cum-editors as authors?
### *Lughat al-ʿArab*

:::{.c_width-30 .c_right}

Authorship of Anastās Mārī al-Karmalī and Kāẓim al-Duyalī more likely

:::
:::{.c_width-60 .c_left}

![Anonmyous sections and editors, coloured by community](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_lughat-size_degree-colour_louvain.png)

:::

## stylistic differences between journals
### Auctorial voices?

:::{.c_width-60 .c_left}

![Issues of 5 periodicals from Cairo, Damascus, and Baghad](../../assets/OpenArabicPE/stylometry/stylo_network-issues-size_degree-colour_publication.png)

:::
:::{.c_width-30 .c_right}

- periodicals show distinct stylistic features
- some similarity between *al-Muqtabas* and *al-Zuhūr*

:::

## stylistic differences between journals
### *al-Ḥaqāʾiq*, *Lughat al-ʿArab*, and *al-Muqtabas*

:::{.c_width-30}

![PCA covariance matrix for the 100 MFWs in a corpus of *al-Ḥaqāʾiq*, *Lughat al-ʿArab*, and *al-Muqtabas* ](../../assets/OpenArabicPE/stylometry/comb_muqtabas-haqaiq-lughat_PCA_100_MFWs_Culled_0__PCA__001.png){#fig:pca-halumu-100}

:::
:::{.c_width-30}

- *Lughat al-ʿArab* and *al-Muqtabas* are indistinguishable
- *al-Ḥaqāʾiq* is different
- some issues of *al-Muqtabas* are very different

:::
:::{.c_width-30}

![PCA covariance matrix for the 900 MFWs in a corpus of *al-Ḥaqāʾiq*, *Lughat al-ʿArab*, and *al-Muqtabas* ](../../assets/OpenArabicPE/stylometry/comb_muqtabas-haqaiq-lughat_PCA_900_MFWs_Culled_0__PCA__001.png){#fig:pca-halumu-900}

:::

## stylistic differences between journals
### *Lughat al-ʿArab*, *al-Muqtabas*, and *al-Zuhūr*

:::{.c_width-30}

![PCA covariance matrix for the 100 MFWs in a corpus of *Lughat al-ʿArab*, *al-Muqtabas*, and *al-Zuhūr*](../../assets/OpenArabicPE/stylometry/comb_muqtabas-lughat-zuhur_PCA_100_MFWs_Culled_0__PCA__001.png){#fig:pca-lumuzu-100}

:::
:::{.c_width-30}

- Strong stylistic similarities between all three periodicals
- some issues of *al-Muqtabas* are very different

:::
:::{.c_width-30}

![PCA covariance matrix for the 900 MFWs in a corpus of *Lughat al-ʿArab*, *al-Muqtabas*, and *al-Zuhūr*](../../assets/OpenArabicPE/stylometry/comb_muqtabas-lughat-zuhur_PCA_900_MFWs_Culled_0__PCA__001.png){#fig:pca-lumuzu-900}

:::

## stylistic differences between journals
### Importance of genre

:::{.c_width-60 .c_left}

![The same 5 periodicals + 6 works by one of the editors](../../assets/OpenArabicPE/stylometry/stylo_network-issues-authors-size_degree-colour_publication.png)

:::
:::{.c_width-30 .c_right}

- very limited similarity between *al-Muqtabas* and its editor Muḥammad Kurd ʿAlī

:::

# Thank you!
## Thank you!

- Maxim Romanov for his work on parameter testing
- Contributors to OpenArabicPE: Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Links:
    + Slides: [https://tinyurl.com/dot2022-grallert-dh](https://tillgrallert.github.io/slides/dh/2022-dot-dh/index.html)
    + Project blog: [https://openarabicpe.github.io](https://openarabicpe.github.io)
    + Papers: <http://digitalhumanities.org/dhq/vol/16/2/000593/000593.html>, <https://doi.org/10/gkhrjr>
    + Twitter: \@[tillgrallert](https://twitter.com/tillgrallert)
    + Email: <till.grallert@fu-berlin.de>, <till.grallert@hu-berlin.de>
- Licence: slides and images are licenced as [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

## References {#refs}