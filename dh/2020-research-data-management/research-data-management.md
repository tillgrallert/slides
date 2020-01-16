---
title: "Research data management"
author: Till Grallert
date: 2020-01-15 22:35:25 +0200
ORCID: orcid.org/0000-0002-5739-8094
duration: 30
---

## Research data management
### Till Grallert, Orient-Institut Beirut
### 16 January 2020, DH brown bag meetings

Slides: [tillgrallert.github.io/slides/dh/2020-research-data-management/](https://tillgrallert.github.io/slides/dh/2020-research-data-management/index.html)

Twitter: @[tillgrallert](https://twitter.com/tillgrallert)

Email: <grallert@orient-institut.org>

## Outline

... today's topic: research data management ...

- what is it?
- why should we care?
- when should we think about it?
- how to do it?

## Outline

1. (research) data
2. (research) data management

# Research data management
## what is it?

... let's postpone this for a moment ...

## why should we care?

1. extrinsic incentive:
    - funding agencies (ERC, DFG) require it
    - our research is subject to legal frameworks (e.g. copy right, data protection)
2. intrinsic incentive:
    - we got data (lots of them)
    - some of them is valuable
    - some of them is sensitive
    - the research project will come to an end
    - we will need (and get) external help

## when should think about it?

... always! ...

+ start right now!
+ throughout a research project

# research data
## always already digital data

>The question of whether something is or is not 'digital' will be increasingly secondary as many forms of culture become mediated, produced, accessed, distributed or consumed through digital devices and technologies. Thus, [...] the digital humanities must be able to offer theoretical interventions and digital methods for a historical moment when the computational has become both hegemonic and post-screenic. [...] We think of the 'digital' as a previous historic movement when computation as digitality was understood in opposition to the analogue, rather than complementary, as we argue in this book.

<cite>Berry and  Fagerjord, *Digital Humanities: Knowledge and Critique in a Digital Age*, 2017, p.2[^2]</cite>

[^2]: Berry, David M and Anders Fagerjord. *Digital Humanities: Knowledge and Critique in a Digital Age.* Cambridge; Malden: Polity, 2017.

## so what are research data?

>Unter digitalen geistes- und kulturwissenschaftlichen Forschungsdaten werden [...] all jene Quellen/Materialien und Ergebnisse verstanden, die im Kontext einer geistes-und kulturwissenschaftlichen Forschungsfrage gesammelt, erzeugt, beschrieben und/oder ausgewertet werden und in maschinenlesbarer Form zum Zwecke der Archivierung, Zitierbarkeit  und zur weiteren Verarbeitung aufbewahrt werden können.

<cite>Puhl, Andorfer, et al., *Forschungsdaten*, 2015, p.14[^1]</cite>

[^1]: Puhl, Johanna, Peter Andorfer, et al. "Diskussion und Definition eines Research Data LifeCycle Für die Digitalen Geisteswissenschaften." *DARIAH-DE Working Papers 11.* Göttingen: DARIAH-DE, 2015. [urn:nbn:de:gbv:7-dariah-2015-4-4](http://nbn-resolving.de/urn:nbn:de:gbv:7-dariah-2015-4-4).


>In the context of the humanities and social sciences, digital research data shall be understood as all those sources/ materials and results that were collected, generated, annotated and/or analysed and that can be stored in machine-readable form for the purpose of archiving, referencing and further reuse.

<cite>My translation</cite>

## data are always mediated

+ we access (generate, read) data through different levels
    1. hardware
    2. software
    3. human-readable representation
+ we need tools to do so
+ all tools are subject to external decisions

## data are always mediated

... we (are made to) think of <!-- and interact --> with data in metaphors ...

>Readers know how paragraphs, pages, files, and folders relate to paper and would like for their digital images to behave in a similar way. The principles of metaphor-driven design contain an implicit model of human-computer interaction, which suggests that humans prefer to manipulate digital information stored on computational media by the means of familiar mediating structures (paragraphs, pages, files, and folders) associated figuratively with the affordances of print media.

>We do not literally drag or drop bits, but we use metaphors of paper and trash cans to help us manipulate bits and bytes as though they were common household objects. The metaphor opens figurative possibilities. It also obscures actual physical contingencies of interacting with bits and bytes, logic gates and electromagnetic traces.

<cite>Tenen, *Plain Text: The Poetics of Computation*, 2017, p.36[^3]</cite>

[^3]: Tenen, Dennis. *Plain Text: The Poetics of Computation.* Stanford: Stanford University Press, 2017.

## data are created different

- raw data
- processed data:
    + we filter,
    + normalise, correct or *clean*,
    + annotate, and
    + aggregate raw data to make it *useful* for answering our research question
- results

<!-- ## data are created different {>>cut<<}

-  Metadaten, bibliographische Daten, Kataloge
-  Digitale und/oder digitalisierte Daten und/oder digitale Repräsentationen von analogen Daten
-  Digitale Objekte
-  Volltexte und Transkriptionen
-  Angereicherte Volltexte
-  Bilder, Filme, Musik, Noten
-  Normdaten, kontrollierte Vokabularien, Ontologien -->

## data are created different <!-- and for a purpose -->

+ some are important or valuable to you (and other stakeholders)
    * you want to protect them from loss
    * *recreating* will be costly or nigh impossible
    * *loss* might create legal liabilities (we promised results)
+ some are sensitive
    * you want to protect them from preying eyes
    * *disclosure* will
        + endanger you or others
        + create legal liabilities for you and others
    * *recording* / *preservation* might be illegal
+ few are both
+ many are neither

## data are alive?!

- remember? data are always mediated
- we mostly think of data in metaphors, such as a "file" <!-- that we can store -->
    + hardware level: various bits distributed across local and remote physical locations
    + software level
        * OS: assembling the various bits into a "file" that lives in volatile memory
        * application software: creating a readable representation
- all data is in constant flux


## data are alive?!

![Eliane Blumer, Pierre-Yves Burgi: [Data Life-Cycle](http://doi.org/10.16911/ethz-ib-1992-en), CC BY-SA 4.0](../../assets/dh/2015-09-08_data-life-cicle.jpg)

## data are alive?!

![Helen Morgan, Nadine Davdson-Wall: [Research Data Life Cycle](http://s3.amazonaws.com/libapps/customers/137/images/Research_Life_Cycle.png), CC BY-NC](../../assets/dh/Research_Life_Cycle.png)

## data will (have to) die

- at the end of a research project, data is either
    + archived
    + published or
    + **deleted**

# research data management
## what is research data management?

- data management is done at all stages of the data life cycle
- each step in the process has its own best practices and standards

![Eliane Blumer, Pierre-Yves Burgi: [Data Life-Cycle](http://doi.org/10.16911/ethz-ib-1992-en), CC BY-SA 4.0](../../assets/dh/2015-09-08_data-life-cicle.jpg)

<!-- - all activities concerning the
    + saving
    + processing
    + sharing
    + archiving
    + publishing and
    + deleting of research data
- a process during the entire life cycle of a research project -->

<!-- ## purpose:

+ protect data from loss and involuntary disclosure
+ ensure replicability of results
+ during and after a research project -->

## why research data management?

- efficient use of limited resources (i.e. our time)
- compliance with funding guidelines
- good research practice ([DFG guidelines](https://www.dfg.de/en/research_funding/principles_dfg_funding/good_scientific_practice/index.html))
- reusability
- open data
- guarantee data quality
- prevent data loss
- visibility and reputation
- transparency and verifiability

## aim:

- strategies,
- protocols,
- responsibilities for each kind of data

## decisions (questions)

+ what data to we expect?
    * which tools are needed?
+ do we need to keep it?
    * for how long?
    * where?
    * in which format?
+ do we need to protect it from others?
    * from whom?
    * for how long?

## strategies

1. documentation: data management plan (DMP)
2. FAIR principles for data: findable, accessible, interoperable, reusable to both human- and machine-driven activities
    - endorsed for research data by the G20 in 2016
    - meta data
    - standard-compliant formats
    - explicit licences
3. Open Source tools

## data management plan

- no standard *per se*
- should cover:
    + administrative tasks
    + responsibilities
    + data protection, legal aspects
    + data formats, metadata schemes, file-naming conventions, data structure and organisation
    + documentation

# material
## tools and infrastructures

- too many to cover
- data management plan
    + [RDMO](https://rdmorganiser.github.io/en/project/)
- publicly funded infrastructures
    + CLARIAH (EU, merger of DARIAH and CLARIN)
    + NFDI (Germany): early planning phase
- publicly funded repositories
    + Zenodo (EU, CERN)

# Open end
## Thank you!

- Links:
    + Slides: [tillgrallert.github.io/slides/dh/2020-research-data-management/](https://tillgrallert.github.io/slides/dh/2020-research-data-management/index.html)
    + Twitter: @[tillgrallert](https://twitter.com/tillgrallert)
    + Email: <grallert@orient-institut.org>

- Licence: The slides are licenced as [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

## links, bibliography

- DFG Leitlinien zu [guter wissenschaftlicher Praxis](https://www.dfg.de/download/pdf/foerderung/rechtliche_rahmenbedingungen/gute_wissenschaftliche_praxis/kodex_gwp.pdf)
- NYU libraries [Data Management Planning](https://guides.nyu.edu/data_management)
- [Forschungsdaten im Kontext von DARIAH-DE](https://de.dariah.eu/forschungsdaten)
- Puhl, Johanna, Peter Andorfer, et al. "Diskussion und Definition eines Research Data LifeCycle Für die Digitalen Geisteswissenschaften." *DARIAH-DE Working Papers 11.* Göttingen: DARIAH-DE, 2015. [urn:nbn:de:gbv:7-dariah-2015-4-4](http://nbn-resolving.de/urn:nbn:de:gbv:7-dariah-2015-4-4).
- Lisa Klaffki. "Forschungsdatenmanagement mit DARIAH-DE", 11. Oktober 2018, <http://vad-ev.de/wp-content/uploads/2019/04/Forschungsdatenmanagement-mit-DARIAH-DE.pdf>, CC
- [Forschungsinfrastrukturen für die Geisteswissenschaften](http://www.forschungsinfrastrukturen.de/doku.php) im Rahmen der NFDI (National Forschungsdaten Initiative)
- [forschungsdaten.info](https://www.forschungsdaten.info/): operated by various German universities, Leibniz and Helmholtz Centres
- [forschungsdaten.org](https://www.forschungsdaten.org/): independent Wiki
- Berry, David M and Anders Fagerjord. *Digital Humanities: Knowledge and Critique in a Digital Age.* Cambridge; Malden: Polity, 2017.
- Tenen, Dennis. *Plain Text: The Poetics of Computation.* Stanford: Stanford University Press, 2017.

<!-- # notes
## images

![SangyaPundir: FAIR principles, CC BY-SA 4.0](../../assets/dh/FAIR_data_principles.jpg)
![Eliane Blumer, Pierre-Yves Burgi: [Data Life-Cycle](http://doi.org/10.16911/ethz-ib-1992-en), CC BY-SA 4.0](../../assets/dh/2015-09-08_data-life-cicle.jpg)
![Helen Morgan, Nadine Davdson-Wall: [Research Data Life Cycle](http://s3.amazonaws.com/libapps/customers/137/images/Research_Life_Cycle.png), CC BY-NC](../../assets/dh/Research_Life_Cycle.png) -->