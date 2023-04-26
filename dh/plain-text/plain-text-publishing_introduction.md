---
title: "Plain-text Workflows für das akademische Schreiben"
subtitle: "Digital Humanities und die (Wieder-)Aneignung der Produktionsmittel"
author: 
    - Till Grallert
Institution: Future e-Research Support in the Humanities, Humboldt-Universität zu Berlin
date: 2022-12-02
status: published
url: https://tillgrallert.github.io/slides/dh/plain-text/
lang: de
bibliography: 
    - https://furesh.github.io/slides/assets/bibliography/FuReSH.csl.json
suppress-bibliography: false
licence: https://creativecommons.org/licenses/by-sa/4.0/
markdown: pandoc
tags:
    - FuReSH
---

# Hintergrund
## Das Problem

::: columns
:::: column

### Die akademische Produktionsweise

- Inhalt und Produktionsmittel gehören einigen wenigen Unternehmen
- Arbeitskraft / -zeit der Wissenschaftler_innen wird kostenlos zur Verfügung gestellt

::::
:::: column

### Konsequenzen

- Produzenten und Öffentlichkeit müssen mehrfach bezahlen
- massiv eingeschränkter Zugang
- Unvereinbarkeit und nicht mehr unterstützte Software und Formate

::::
:::

## Das Problem
+-----------------------+-----------------------------+-------------------------+
|        Prozess        |           "Früher"          |          Heute          |
+=======================+=============================+=========================+
| 1. Schreiben          | - Wissenschaftler_innen     | - Wissenschaftler_innen |
|                       |                             | - Öffentlichkeit        |
+-----------------------+-----------------------------+-------------------------+
| 2. Veröffentlichen    | - Verlage                   | - Verlagskonglomerate   |
|                       | - akademische Vereinigungen | - Werbewirtschaft       |
+-----------------------+-----------------------------+-------------------------+
| 3. Entdecken          | - Bibliotheken              | - Verlagskonglomerate   |
|                       | - Verlagskataloge           | - Werbewirtschaft       |
|                       | - Fachindezes               |                         |
+-----------------------+-----------------------------+-------------------------+
| 4. Lesen              | - Wissenschaftler_innen     | - Wissenschaftler_innen |
|                       | - Öffentlichkeit            | - Öffentlichkeit        |
+-----------------------+-----------------------------+-------------------------+
| 5. Wissensmanagement/ | - Wissenschaftler_innen     | - Verlagskonglomerate   |
| Annotation            |                             | - Werbewirtschaft       |
+-----------------------+-----------------------------+-------------------------+

# Eine Lösung?!
## Unser Wunsch

![Mal wieder eine Blackbox](https://furesh.github.io/slides/assets/images/operationalisierung/plain-text_blackbox.jpg)

## Pandox to the rescue

![Pandoc](https://furesh.github.io/slides/assets/images/operationalisierung/plain-text_pandoc.jpg)

## Pandox to the rescue

::: columns
:::: column

```md
---
title: "Ankündigung Scholarly Makerspace"
subtitle: "Status: Draft"
author: Till Grallert
date: 2022-03-25
lang: de
ORCID: orcid.org/0000-0002-5739-8094
bibliography: ../assets/bibliography/FuReSH.csl.json
---

Die Universitätsbibliothek der Humboldt-Universität richtet in den kommenden drei Jahren im Rahmen des DFG-geförderten Projekts "Future e-Research Support in the Humanities II" in Zusammenarbeit mit den Lehrstühlen für [Digital History](https://www.geschichte.hu-berlin.de/de/bereiche-und-lehrstuehle/digital-history) am Institut für Geschichte und für [Information Processing and Analytics](https://www.ibi.hu-berlin.de/de/forschung/info_processing_analytics/ipa) am Institut für Bibliotheks- und Informationswissenschaften einen **prototypischen *Scholarly Makerspace*** ein. Inspiriert von der *maker culture* und der  Idee der Makerspaces, die in einigen Bibliotheken bereits  etabliert sind [@Spath2019Makerspaces], stellen wir das experimentierende "Machen" mit Computern und digitalen Artefakten in das Zentrum hermeneutischer und epistemologischer Zugänge [@Sayers2018MakingThings]. Der *Scholarly Makerspace* wir dafür die Infrastruktur aus Raum, computergestützten Werkzeugen und Erfahrungen in den Digital Humanities zur Verfügung stellen, um gemeinsam mit Forschenden in allen Phasen ihrer Karrieren die **Herausforderungen der Digitalität für die Geistes- und Kulturwissenschaften experimentell anzugehen**.

![Eine geschlossene "Blackbox"](https://furesh.github.io/slides/assets/images/blackbox/blackbox_makerspace-closed.png){#fig:box-closed}
```

::::
:::: column

![als `DOCX`](https://furesh.github.io/slides/assets/images/pandoc_result-docx.png)

![als `PDF`](https://furesh.github.io/slides/assets/images/pandoc_result-pdf.png)

::::
:::

## Pandox to the rescue

Diese Folien sind selber mit Pandoc aus Markdown generiert worden. Die Quelle der letzten Folie sieht so aus:

~~~md
::: columns
:::: column

```md
---
title: "Ankündigung Scholarly Makerspace"
subtitle: "Status: Draft"
author: Till Grallert
date: 2022-03-25
lang: de
ORCID: orcid.org/0000-0002-5739-8094
bibliography: ../assets/bibliography/FuReSH.csl.json
---

Die Universitätsbibliothek der Humboldt-Universität richtet in den kommenden drei Jahren im Rahmen des DFG-geförderten Projekts "Future e-Research Support in the Humanities II" in Zusammenarbeit mit den Lehrstühlen für [Digital History](https://www.geschichte.hu-berlin.de/de/bereiche-und-lehrstuehle/digital-history) am Institut für Geschichte und für [Information Processing and Analytics](https://www.ibi.hu-berlin.de/de/forschung/info_processing_analytics/ipa) am Institut für Bibliotheks- und Informationswissenschaften einen **prototypischen *Scholarly Makerspace*** ein. Inspiriert von der *maker culture* und der  Idee der Makerspaces, die in einigen Bibliotheken bereits  etabliert sind [@Spath2019Makerspaces], stellen wir das experimentierende "Machen" mit Computern und digitalen Artefakten in das Zentrum hermeneutischer und epistemologischer Zugänge [@Sayers2018MakingThings]. Der *Scholarly Makerspace* wir dafür die Infrastruktur aus Raum, computergestützten Werkzeugen und Erfahrungen in den Digital Humanities zur Verfügung stellen, um gemeinsam mit Forschenden in allen Phasen ihrer Karrieren die **Herausforderungen der Digitalität für die Geistes- und Kulturwissenschaften experimentell anzugehen**.

![Eine geschlossene "Blackbox"](https://furesh.github.io/slides/assets/images/blackbox/blackbox_makerspace-closed.png){#fig:box-closed}
```

::::
:::: column

![als `DOCX`](https://furesh.github.io/slides/assets/images/pandoc_result-docx.png)

![als `PDF`](https://furesh.github.io/slides/assets/images/pandoc_result-pdf.png)

::::
:::
~~~

# Voraussetzungen
## Software

- Plain-text editor
    + [Sublime Text](https://www.sublimetext.com)
    + [VS Code](https://code.visualstudio.com)
- Command line terminal
    + Windows >= 10: Windows Terminal
    + Unix (macOS, Linux): Terminal
- Konverter für verschiedenste Eingabe und Ausgabeformate: [Pandoc](https://pandoc.org)
- Literaturverwaltungsprogramm
    + [Zotero](https://zotero.org)

## Mark-up oder Auszeichnungsprachen

- Plain text bringt massive Einschränkungen mit sich
- Ein Text ist mehr als eine Sequenz von Zeichen
    + Text hat **Form** und **Inhalt** (mit potentiellen Metainformationen)
    + Text hat eine **Struktur** und **kommunikative Funktion**
    + Text hat mehrere mögliche **Lesarten**
- **Markup** ist die Möglichkeit das alles explizit zu machen

::: alert

Nur explizites Wissen kann verlässlich wiedergefunden und angezeigt werden

:::

# Glossar
## [Markdown (md)](http://daringfireball.net/projects/markdown)

::: columns
:::: wide

- Was: eine *leichtgewichtige Auszeichnungssprache* (plain-text **Syntax**) und text-to-`HTML` Konvertierungs-**Werkzeug**. 
    + Die Syntax ist durch plain-text Email inspiriert
- Wann: **2004**
- Wer: John Gruber (und Adam Swartz)
- Aktuelle Version: Markdown 1.0.1 (2004)

::::
:::: narrow

```md
# [Markdown (md)](http://daringfireball.net/projects/markdown)

- Was: eine *leichtgewichtige Auszeichnungssprache* (plain-text **Syntax**) und text-to-`HTML` Konvertierungs-**Werkzeug**. 
    + Die Syntax ist durch plain-text Email inspiriert
- Wann: **2004**
```

::::
:::

::: columns
:::: column

### Pros

+ extrem flexibel
+ sehr breit unterstützt
    * HU: Element (Matrix), HU Box, Open Project
    * Slack, Discord
    * GitHub, R Markdown, Jupyter Notebooks

::::
:::: column

### Cons:

+ `md` ist eine **Konvention** mit vielen Uneindeutigkeiten
    * keine strikte Syntax oder Standard jenseits der originalen Implementation
+ fehlende Features: Fußnoten, Tabellen ...
+ nicht weiter entwickelt

::::
:::


## [Pandoc](https://pandoc.org/)

- Was: Konvertierungs-**Werkzeug** und auf Markdown basierende plain-text **Syntax**
- Wann: aktive Entwicklung seit **2006**
- Wer: John MacFarlane (UC Berkeley)
- Aktuelle Version: 2.19.2 (2022)

::: columns
:::: column

### Pros

+ aktive Entwicklung
+ sehr große Anzahl von unterstützten Ein- und Ausgabeformaten
+ extrem flexibles, modulares Design
+ Fußnoten
+ Tabellen
+ Zitationen

::::
:::: column

### Cons:

+ weiterhin kein strikter Standard
+ teilweise Inkompatibilität mit anderen Markdown Flavours

::::
:::

## Pandoc Spickzettel

- Basis: 
    - specify input file (can be an URL): `FILENAME`
    - specify input format (optional): `-f FORMAT`, `-r FORMAT`  / `--from=FORMAT`, `--read=FORMAT`
    - specify output format (optional: `-t FORMAT`, `-w FORMAT` /  `--to=FORMAT`, `--write=FORMAT`
    - specify output file: `-o FILENAME` / `--output=FILENAME`  
    - available formats: 
        + markdown, markdown_strict, markdown_mmd, commonmark, textile
        + html, html5, docbook, epub, epub3, asciidoc, tei
        + mediawiki
        + docx, odt
        + pdf, latex
- styling
    + typographic quotation marks etc.:  `-S` / `--smart`
    + use a template file: `--template=FILE|URL`
- additional options:
    + generate table of content: `--toc`, `--table-of-contents`
    + standalone (include a proper header and footer): `-s`, `--standalone` 

## [Yaml (Yaml ain't markup language)](http://yaml.org/)


::: columns
:::: wide

- Was: "menschenfreundliche" [Datenserialisierung](https://en.wikipedia.org/wiki/Serialization); superset von [JSON]()
    + provides a very simple means of adding metadata to the beginning of plain text files
- Wann: seit **2001** <!--; first working draft of YAML 1.1 in 2004-->
- Wer: Clark Evans, Ingy döt Net and Oren Ben-Kiki
- Aktuelle Version: YAML 1.2 ([spec](http://yaml.org/spec/1.2/spec.html))



::::
:::: narrow

```yml
---
- title: "Alles nur Spielerei?"
- author: 
    - Till Grallert
    - Samantha Tirtohusodo
- date: 2022-11-29
---
```

::::
:::

## [BibTeX](http://www.bibtex.org/Format/)


::: columns
:::: wide

- Was: ein strukturiertes **Format** für bibliographische Daten (und ein Programm zur Erstellung von Literaturverzeichnissen in TeX/ LaTeX)
- Wann: seit **1985** 
- Wer: Oren Patashnik, Leslie Lamport
- Aktuelle Version: 0.99c (1988), 0.99d (2010)

::::
:::: narrow

```bibtex
@book{JannidisEtAl2017DigitalHumanities,
  title = {{Digital Humanities}},
  editor = {Jannidis, Fotis and Kohle, Hubertus and Rehbein, Malte},
  year = {2017},
  publisher = {{J.B. Metzler}},
  address = {{Stuttgart}},
  doi = {10.1007/978-3-476-05446-3},
  isbn = {978-3-476-02622-4 978-3-476-05446-3},
  langid = {ngerman}
}
```

::::
:::

::: columns
:::: column

### Pros

+ von allen relevanten Anwendungen unterstüzt

::::
:::: column

### Cons:

+ praktisch keine Entwicklung seit 1988
+ kein strikter Standard

::::
:::