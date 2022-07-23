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

# Arabic as an under-resourced language
## Linguistic imperialism

>'Linguistic imperialism' is shorthand for a multitude of activities, ideologies, and structural relationships. Linguistic imperialism takes place within an overarching structure of asymmetrical North/ South relations, where language interlocks with other dimensions, cultural (particularly in education, science, and the media), economic and political

<cite>[@Phillipson1997RealitiesAndMyths, 239]</cite>

>The basis for the codes, languages, methodologies, and technical instruments of the digital humanities is English; the written and spoken language of all the main conferences, the most prestigious journals, the institutions that control the discipline, the organizations and international consortia, and the central authorities of knowledge is, with few exceptions, some dialect of British or American English.

<cite>[@Fiormonte+2021+TaxationagainstOverrepresentation, 334-335]</cite>

## Arabic

::: columns
:::: column

### Script

- Second most common script
    + 14 languages, among them Arabic, Persian, Urdu, Pashtu

::::
:::: column

### Language

+ Fifth most common language
    * 1 of 6 official languages at the UN
    * official language in 26 countries
    * \>420M speakers
- Liturgic language of 1.6B Muslims

::::
:::

![Example: [@oclc_4770057679-i_13-div_8.d1e1249]](../../assets/dh/arabic-script_sample-annotated.png){#fig:arabic-sample-1}

## Arabic
### Script

+ Writing direction: from right to left
+ Letters (graphemes) are mostly connected in the writing direction and change their shape (allographs):  [ج جـ ـجـ ـج]{.c_rtl lang="ar"}
+ Graphemes combine basic shapes (archigrapheme, *rasm*) and diacritic marks (*iʿjām*)
    * usage subject to change and regional preferences
* Vocalisation (*tashkīl*) fixes meaning and **can** be added

::: columns
:::: column

### أميركا وعلماء العرب

[كانت أميركا مجهولة عند ابنآء القرن الخامس عشر بدليل ان المؤرخين في ذلك العهد لم يذكروا عنها سوى اخبار اكتشافها في أواخر ذلك القرن]{.c_rtl lang="ar"}

<cite>[@oclc_4770057679-i_13-div_8.d1e1249]</cite>

::::
:::: column

### امىرکا وعلماء العرٮ

[کاںٮ امىرکا محهوله عںد اٮںا الٯرں الحامس عسر ٮدلىل اں المورحىں ڡى دلک العهد لم ىدکروا عںها سوى احٮار اکٮساڡها ڡى اواحر دلک الٯرں]{.c_rtl lang="ar"}

*rasm*

::::
:::

# Method
## Corpus

| Periodical                      | Place             | Dates[^tb1]   | Vol.s   | No.s    | Words       | Articles | with author | 2500+ words | words/articles | Authors | DOI                                                              |
| ------------------------------- | ----------------- | ------------- | ------: | ------: | ------:     | ------:  | ------:     | -----:      | ------:        | ------: | ------------------------                                         |
| [al-Ḥaqāʾiq][haqaiq_git]        | Damascus          | 1910--13      | 3       | 35      | 298090      | 389      | **41.90**   | 22          | 832.66         | 104     | [10.5281/zenodo.1232016](https://doi.org/10.5281/zenodo.1232016) |
| [al-Muqtabas][muqtabas_git]     | Cairo, Damascus   | 1906--18      | **9**   | **96**  | **1981081** | **2964** | 12.72       | **241**     | 873.34         | 140     | [10.5281/zenodo.597319](https://doi.org/10.5281/zenodo.597319)   |
| [al-Ustādh][ustadh_git]         | Cairo             | 1892--93      | 1       | 42      | 221447      | 435      | 5.52        | 13          | 582.21         | 8       | [10.5281/zenodo.3581028](https://doi.org/10.5281/zenodo.3581028) |
| [al-Zuhūr][zuhur_git]           | Cairo             | 1910--13      | 4       | 39      | 292333      | 436      | **41.51**   | 6           | 695.09         | 112     | [10.5281/zenodo.3580606](https://doi.org/10.5281/zenodo.3580606) |
| [Lughat al-ʿArab][lughat_git]   | Baghdad           | 1911--14      | 3       | 34      | 373832      | 939      | 16.19       | 21          | 485.21         | 53      | [10.5281/zenodo.3514384](https://doi.org/10.5281/zenodo.3514384) |
| **total**                       |                   |               | 20      | 246     | c.3000000   |          |             | 303         |                |         |                                                                  |

Table: Our corpus from "Open Arabic Periodical Editions" {#tbl:openarabicpe-corpus}

[^tb1]: The current cut-off date is 1918.

[muqtabas_git]: https://github.com/OpenArabicPE/journal_al-muqtabas
[haqaiq_git]: https://github.com/OpenArabicPE/journal_al-haqaiq
[lughat_git]: https://github.com/OpenArabicPE/journal_lughat-al-arab
[ustadh_git]: https://github.com/OpenArabicPE/journal_al-ustadh
[zuhur_git]: https://www.github.com/openarabicpe/journal_al-zuhur

## Stylometry
# Thank you!
## References