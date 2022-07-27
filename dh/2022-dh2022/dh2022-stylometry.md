---
title: "Establishing parameters for stylometric authorship attribution of 19th-century Arabic books and periodicals"
subtitle: ""
author: 
	- Maxim Romanov
	- Till Grallert
date: 2022-07-23 
ORCID: orcid.org/0000-0002-5739-8094
lang: en-GB
bibliography: 
    - /BachUni/research-projects/OpenArabicPE/assets/bibliography/openarabicpe.csl.json
    - /BachUni/applications/applications.csl.json
---

## Establishing parameters for stylometric authorship attribution of 19th-century Arabic books and periodicals

::: columns
:::: column

Maxim Romanov

Universität Hamburg

<maxim.romanov@uni-hamburg.de>

::::
:::: column

Till Grallert

Humboldt-Universität zu Berlin

<till.grallert@hu-berlin.de>

::::
:::

#DH2022, 27 July 2022

# Arabic periodicals
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

![Title pages of *al-Ḥaqāʾiq*, *al-Ḥasnāʾ*, *al-Iqbāl*, *al-Maḥabba*, *al-Ahrām*, *al-Muqtaṭaf*, and *al-ʿAṣr al-Jadīd*](../../assets/OpenArabicPE/front-pages_strip.png){#fig:front-pages .c_height-30}

## Research focus: intellectual networks

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
- core network (14 nodes):
    - absent from the literature
    - suprising set up: many Iraqis (6), few Syrians (2), few Christians (2)

::::
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
## Stylometry

Based on parameter settings established in our tests

::: columns
:::: column

### `stylo()` settings

- Tokens: words
- Sampling: 2500 tokens
- MFF: 200--500 tokens, incremented by 100
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

## Corpus

| Periodical                      | Place             | Dates[^tb1]   | Vol.s   | No.s    | Words       | Articles | with author | 2500+ words | words/articles | Authors | DOI                                                              |
| ------------------------------- | ----------------- | ------------- | ------: | ------: | ------:     | ------:  | ------:     | -----:      | ------:        | ------: | ------------------------                                         |
| [al-Ḥaqāʾiq][haqaiq_git]        | Damascus          | 1910--13      | 3       | 35      | 298090      | 389      | **41.90**   | 22          | 832.66         | 104     | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) |
| [al-Muqtabas][muqtabas_git]     | Cairo, Damascus   | 1906--18      | **9**   | **96**  | **1981081** | **2964** | 12.72       | **241**     | 873.34         | 140     | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   |
| [al-Ustādh][ustadh_git]         | Cairo             | 1892--93      | 1       | 42      | 221447      | 435      | 5.52        | 13          | 582.21         | 8       | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) |
| [al-Zuhūr][zuhur_git]           | Cairo             | 1910--13      | 4       | 39      | 292333      | 436      | **41.51**   | 6           | 695.09         | 112     | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) |
| [Lughat al-ʿArab][lughat_git]   | Baghdad           | 1911--14      | 3       | 34      | 373832      | 939      | 16.19       | 21          | 485.21         | 53      | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) |
| **total**                       |                   |               | 20      | 246     | 3166783     | 5163     |             | 303         | 613.36         |         |                                                                  |

Table: Our corpus from "Open Arabic Periodical Editions" {#tbl:openarabicpe-corpus}

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

-> **very different from the test corpus**

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

![Bootstrap consensus network, coloured by author](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author.png)

## Zooming in: Kāẓim al-Dujaylī

Anonymous travellogue in *Lughat al-ʿArab* most likely written by the magazine's editor Kāẓim al-Dujaylī

::: columns
:::: column

![Detail from the previous network plot](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-details.png)

::::
:::: column

![Radar plot for the unattributed article in the upper right, ["Riḥla ilá Shufāthā", *Lughat al-ʿArab* 3(1), Aug. 1913](https://openarabicpe.github.io/journal_lughat-al-arab/tei/oclc_472450345-i_25.TEIP5.xml#div_7.d2e1438)](../../assets/OpenArabicPE/stylometry/stylo_NN_oclc.472450345_v.3_i.1_div_7.d2e1438_lollipop.png)

::::
:::

## Zooming in: Muḥammad al-Qāsimī?

A cluster of texts <!-- from al-Ḥaqāʾiq and? --> potentially written by Muḥammad al-Qāsimī

::: columns
:::: column

![Detail from the larger network plot](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_louvain-details_1.png)

::::
:::: column

![Radar plot for the unattributed article in the upper left, ["Ajwābat al-ʿulamāʾ ʿan al-tamthīl", *al-Ḥaqāʾiq* 2(3), Sep. 1911](https://OpenArabicPE.github.io/journal_al-haqaiq/tei/oclc_644997575-i_15.TEIP5.xml#div_3.d1e562)](../../assets/OpenArabicPE/stylometry/stylo_NN_oclc.644997575_v.2_i.3_div_3.d1e562_lollipop.png)

::::
:::

## Zooming in: William Shakespeare

Unmarked translations of Shakespeare's Julius Caesar in *al-Zuhūr*

::: columns
:::: column

![Detail from the larger network plot](../../assets/OpenArabicPE/stylometry/stylo_network-articles-size_degree-colour_author-details.png)

::::
:::: column

![Radar plot for the attributed article in the lower right](../../assets/OpenArabicPE/stylometry/stylo_oape.760_oclc.1034545644_v.3_i.6_div_1.d2e1819_lollipop.png)

::::
:::

## owners-cum-editors as authors?
### *al-Muqtabas*

Muḥammad Kurd ʿAlī most likely not the author

![Anonmyous sections and editors, coloured by author](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_muqtabas-size_degree-colour_author.png)

## owners-cum-editors as authors?
### *al-Muqtabas*

Multiple anonymous candidates?

![Anonmyous sections and editors, coloured by community](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_muqtabas-size_degree-colour_louvain.png)

## owners-cum-editors as authors?
### *Lughat al-ʿArab*

Authorship of Anastās Mārī al-Karmalī and Kāẓim al-Duyalī more likely

![Anonmyous sections and editors, coloured by author](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_lughat-size_degree-colour_author.png)

## owners-cum-editors as authors?
### *Lughat al-ʿArab*

Authorship of Anastās Mārī al-Karmalī and Kāẓim al-Duyalī more likely

![Anonmyous sections and editors, coloured by community](../../assets/OpenArabicPE/stylometry/stylo_network-sections-editors_lughat-size_degree-colour_louvain.png)

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

- Maxim Romanov
- Contributors to OpenArabicPE: Jasper Bernhofer, Dimitar Dragnev, Patrick Funk, Talha Güzel, Hans Magne Jaatun, Jakob Koppermann, Xaver Kretzschmar, Daniel Lloyd, Klara Mayer, Tobias Sick, Manzi Tanna-Händel, and Layla Youssef
- Links:
    + Slides: [https://tinyurl.com/lp-7-03-grallert](https://tillgrallert.github.io/slides/dh/2022-dh2022/index.html)
    + Paper: <https://doi.org/10/gkhrjr>
    + Project blog: [https://openarabicpe.github.io](https://openarabicpe.github.io)
    + Twitter: \@[tillgrallert](https://twitter.com/tillgrallert)
    + Email: <till.grallert@fu-berlin.de>
- Licence: slides and images are licenced as [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

## References