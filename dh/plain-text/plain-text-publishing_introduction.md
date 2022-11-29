---
title: "Plain-text Workflows für das akademische Schreiben"
subtitle: "Digital Humanities und die (Wieder-)Aneignung der Produktionsmittel"
author: 
    - Till Grallert
Institution: Future e-Research Support in the Humanities, Humboldt-Universität zu Berlin
date: 2022-12-02
status: published
url: https://tillgrallert.github.io/slides/plain-text/
lang: de
bibliography: 
    - https://furesh.github.io/slides/assets/bibliography/FuReSH.csl.json
suppress-bibliography: false
licence: https://creativecommons.org/licenses/by/4.0/
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


## Unser Wunsch

![Mal wieder eine Blackbox](https://furesh.github.io/slides/assets/images/operationalisierung/plain-text_blackbox.jpg)

## Pandox to the rescue

![Pandoc](https://furesh.github.io/slides/assets/images/operationalisierung/plain-text_pandoc.jpg)

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

## [Yaml (Yaml ain't markup language)](http://yaml.org/)


::: columns
:::: wide

- Was: "human friendly" [data serialization](https://en.wikipedia.org/wiki/Serialization); superset von [JSON]()
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