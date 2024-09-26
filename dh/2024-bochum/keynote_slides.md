---
title: "Do it yourself (but not alone) and KISS!"
subtitle: ""
panel: ""
event: "Bochum"
author: Till Grallert
institute: 
    - "Humboldt-Universität zu Berlin, Institut für Geschichtswissenschaften"
    - "Methods Innovation Lab, NFDI4Memory"
email: till.grallert@hu-berlin.de
date: 2024-09-30
ORCID: orcid.org/0000-0002-5739-8094
lang: de
url: https://tillgrallert.github.io/slides/dh/2024-bochum/
bibliography: 
    - references.bib #csl.json
background-image: ""
nocite:
---

# Raison d'etre <br/>Wir leben in einem postdigitalen Moment
## *Digital* als ein historischer Begriff 

::: columns
:::: wide

<!-- **Datafication** emphasises the epistemic shift from a world where data were a closely defined part of the output of research processes towards the new status quo in which all research processes are always already computationally mediated through information and communication technologies. -->

**Datafizierung** unterstreicht den fundamentalen  epistemischen und konzeptionellen Wandel von einer Welt, in der Daten ein eng definierter Teil der Ergebnisse von Forschungsprozessen waren, hin zu einem neuen Status Quo, in dem alle  Forschungsprozesse immer bereits durch Informations- und Kommunikationstechnologien (ICT) computationell mediiert sind. 

::::
:::: narrow

[wir leben in *datafizierten* Gesellschaften]{.keyphrase}

::::
:::

::: columns
:::: narrow

["*digital*" hat seine Bedeutung verloren]{.keyphrase}

::::
:::: wide

>We think of the 'digital' as a previous historic movement when computation as digitality was understood in opposition to the analogue, rather than complementary [...]

<cite>@Berry+2017, 2</cite>

::::
:::

::: columns
:::: narrow

[*Algorithmen* sind Teil des sozialen Gewebes]{.keyphrase}

::::
:::: wide

>Today, algorithms are such an intrinsic and fundamental part of how daily life is experienced that some scholars even argue that we live in "algorithmic  cultures" [...]. This evocative notion points to the increasing difficulty of separating  algorithms from the activities that make up culture. It also evinces the complex ways in which human agency and algorithmic actions are intertwined [...] 

<cite>@Siles2023Living, 1</cite>

>It is our position that the "digital" cannot be understood as a separate domain of culture. If we actually examine the digital [...] we see that today digital information processing is present in every aspect of our lives.

<cite>[@CPCAbout]</cite>

::::
:::

::: notes

- Digital history, then, accepts that the human cultural record is being *datafied* and we need computational methods in order to make historical arguments [cf. @DigitalHistoryArgument2017, 2; @Laessig2021DigitalHistory, 6]
- Digital history also addresses the age of abundance, as postulated by Roy Rosenzweig, and epitomised by the recent advances in generative AI and LLMs, which will create an infinite amount of absolutely plausible and convincing yet utterly false sources 
- Daraus folgt aber auch, dass **digital** history oder **digital** humanities hilfreiche Begriffe einer Übergangsphase sind. Sie sind Label mit einem hohen symbolischen und ökonomischen Kapital. 


:::

## Daten aller Ecken



::: columns
:::: narrow

[Jegliche digitale Informationen sind Daten]{.keyphrase} ...

::::
:::: wide

>Data are forms of information, a larger concept that is even more difficult to define. Epistemological and ontological problems abound, resulting in many books devoted to explicating information and knowledge 

<cite>@Borgman2015BigData, 18</cite>

::::
:::

::: columns
:::: wide

>[Datafication/modeling] is the work of abstracting discrete values from a phenomenon or artifact. These values may be expressed in numbers or texts and are necessarily a reduction of complex materials into a form for computation. <!--With data we can automate processes -->

<cite>@Drucker2021DHCoursebook, 3</cite>

>Data need to be imagined *as* data to exist and function as such, and the imagination of data entails an interpretive base.

<cite>@Gitelman2013Introduction, 3</cite>

::::
:::: narrow

... und [alle Daten sind modelliert]{.keyphrase}

<!-- - Mapping
- Reduction
- Purpose -->

::::
:::



::: notes 

- Data literacy as part of data culture
- data are always a concrete embodyment and a socio-technological stack: serialisation
- If we subscribe to social constructivism then all models are historically situated
    - Data and models are situated in historical processes of knowledge production
- Models have three characteristics [@Stachowiak1973AllgemeineModelltheorie]
    - Mapping/ replacing: model for something
    - Reduction: abstracts aspects of interest
    - Purpose: models have a purpose for something
- drucker: capta

:::

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

## Die Humanities in der Epoche der Berechenbarkeit

[Für einen aufgeklärten Umgang mit *Datafizierung* brauchen wir einen fundamentalen **Kulturwandel**]{.keyphrase}

::: columns
:::: column

[Kennen Sie die?]{.keyphrase}

!["Werkzeuge" in Digital Humanities Quarterly](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/wordcloud-rel-100-repel_tools-dhq-w_100.png){#fig:wordcloud-dhq}

<!-- !["Werkzeuge" in Abstracts für DH Konferenzen, 2014--22](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/wordcloud-rel-100-repel_tools-dh-conferences_abstracts-2014-2022-w_100.png){#fig:wordcloud-dh-conferences} -->

::::
:::: column

Es herrscht in der Breite ein Mangel an 

- **Diskurs**: Austausch über unser (disziplinäres) Selbstverständnis 
+ **Theorie**: Verständnis des epistemischen Wandels und der ontologischen Dimensionen der *Datafizierung*
+ **Praktiken**: Beherrschung der notwendigen Methoden und Werkzeuge
+ positivem **Wissen**: Überblick über die Möglichkeiten in einem sich rapide wandelnden Umfeld 

<!-- - Es gibt ein starkes Ressentiment gegenüber allem "digitalen"
- *"Digital" Humanities* als Indikator -->

::::
:::

::: notes

- David Berry "epoch of computationability" 

:::

## Von *digital consumers* zu *digital citizens*, oder warum wir eine Datenkultur brauchen

<!-- requires some work -->

[*digital natives* sind nicht automatisch *digital citizens*]{.keyphrase}

::: columns
:::: column

### im weiteren Sinn

- eine **Fachkultur**, bei der (Forschungs-)daten und datengetriebener Methoden ein integraler Bestandteil sind, die Arbeit mit und an Daten also nicht mehr als ein netter Appendix zum "eigentlichen" Forschungsprozess verstanden wird.
    - braucht Verständnis der theoretischen und epistemologischen Grundlagen und Implikationen der Datafizierung und Diskussion über deren Folgen

::::
:::: column

### im engeren Sinn

- **alltägliche Praktiken** und Verantwortlichkeiten (auch rechtlich und ethisch) im Umgang mit Forschungsdaten, bei deren Erzeugung, Bereitstellung und Nutzung mit Hilfe von computationellen Methoden und Werkzeugen.
    - braucht Orientierung, Guidelines und Unterstützung

::::
:::

::: notes

- *digital citizenry* ist von [@Rankin2018PeoplesHistory, 11] geprägt
    - >Kurtz, the director of the Computation Center, used the language of “citizenship” to describe the relationship between a user and the user’s computing network. A good computing citizen respected the college’s ongoing computer memory limitations. [@Rankin2018PeoplesHistory, 43-44]
- Ziel ist *digital* or *computing citizens*, die über ihre Teilnahme  und -habe an einer Gemeinschaft definiert sind. 
    + Unterschied zu Produzenten und *Makers*
    + **ABER** Digital natives sind nicht automatisch digital citizens
        + >despite what the term “digital natives” invokes, it does not mean that those who are digital natives (born after 1980) understand digital technology. In fact, digital natives may not remember life before the internet, but that does not mean they understand the complex systems that supports it or the nuances of communication and knowledge creation in the digital age [@Levy2017DigitalZombies, §16].
- kann **nur kollaborativ** adäquat bewältigt werden. 
+ ich fokussiere heute eher auf die Datenkultur im engeren Sinn, und schlage alltägliche Praktiken vor, die uns erlauben auch eine Datenkultur im weiteren Sinn zu etablieren.

:::

# DIY <br/>Do it yourself
## Making

::: columns
:::: narrow

>Do artefacts have politics? 

<cite>[@Winner+1980]</cite>

>Do politics have artefacts? 

<cite>[@DunbarHester2014LowPower]</cite>

::::
:::: wide

>To use [...] tools well, we must, in some real sense, understand them better than the tool makers. [...] The best kind of tools are therefore the ones that we make ourselves. 

<cite>[@Tenen2016BluntInstrumentalism, 85]</cite>

>Without access to the code, whether because it is proprietary or generated on the fly, as in the case of some machine-learning algorithms, analysts can only comment on the apparent operations of the code based on its effects. The operations of the code are left in the hands of those who can access it, usually those who have made or maintain it, and those who can read it. 

<cite>[@Marino2020CriticalCodeStudies, 4]</cite>

::::
:::

::: columns
:::: column

### Making

- Experimentieren, Tüfteln, Ausprobieren, Werkeln 
- Selbstermächtigung mit dem Ziel der (Wieder)Aneignung der Produktionsmittel

::::
:::: column

### Maker turn

Kreativität von Design, Herstellung und Erfahrung von (digitalen) Objekten als From von Wissenschaft

::::
:::


::: notes

- Grundsatz: Werkzeuge und Methoden sind mit Machtverhältnissen verwoben
    - >The Cloud *is* a factory. Your AI *is* a human. Sexism *is* a feature, not a bug. [@Mullaney2021Intro, 7, Hervorhebung im Original]
- Geschichte
    + 1970er Kalifornien: kooperative Werkstätten
    + Recht auf Reparatur
    + DIY: do it yourself culture
    + "Maker Movement Manifesto" von Hatch (2013)
        * make, share, give, learn, tool up, play, participate, support, change
- bezieht sich auf [@Wythoff2022MinimalComputing], der die beiden Fragen verknüpft hat
    + Do artefacts have politics? [@Winner+1980]
    + Do politics have artefacts? [@DunbarHester2014LowPower]
- Kritik an Maker culture als omnipotenter maskuliner Raum:
    - >knowledge of circuitry is often conflated with (superheroic) command over people, situations, and things. In present-day “maker” cultures, consider the ubiquity of remarks such as “getting under the hood” or “knowing the nuts and bolts,” which tend to fuse logic with mastery, control with masculinity, engineering with rationality, and programming with revealing. [@Sayers2017Introduction, 3]

:::

## Datenkultur und Werkzeugkompetenz

::: notes

- maker culture als ein Teil der Datenkultur
    - als praktische Kritik der Digitalität
- Das Ziel des *Scholarly Makerspaces* ist die Erarbeitung von *tool literacy*, die in zwei Dimensionen gedacht wird: 
    1. Zum einen geht es um das ganz konkrete Erlernen von Werkzeugen und computergestützten Verfahren: Wie kann ich Korpus von Digitalisaten mit Methoden des *distant reading* analysieren? Was ist eine Netzwerkanalyse? Was sind die Möglichkeiten der Datenvisualisierung? Wie kann ich die Disinformationskampagnien rechter Trollfarmen in Social Media sinnvoll analysieren?
    2. Zum anderen wird *tool literacy* aber mit dem Fokus auf Werkzeuge und Methoden als Gegenstand der Untersuchung weiter gedacht und mit  [*Critical Code Studies*](https://criticalcodestudies.com/) [@Marino2020CriticalCodeStudies] und den *Science and Technology Studies* in Beziehung gesetzt: von der Reflexion über die hermeneutischen und epistemologischen Folgen bestimmter Werkzeuge und Zugänge zu digitalen Daten bis zu den ethischen und ökologischen Folgen im Bereich der künstlichen Intelligenz bzw. des maschinellen Lernens, wie z.B. dem massiven [Einsatz endlicher natürlicher Resourcen](https://dhc-barnard.github.io/dhclimate/) und die verschiedenen Biases ihrer Schöpfer\*innen perpetuierende Algorithmen und Modelle.

:::

# Do it yourself, but not alone!
## Gemeinschaftlich und kollaborativ

>I also remind DH is an imposter syndrome house of mirrors. You look around and see experts in GIS, TEI, dataviz, etc.; it's hard to remember that people tend to be good at *one* of those things when the collective appears to be good at *all* of them. **We all suck at most of DH**.

<cite>[@Weingart2021AlsoRemindDH]</cite>

>Unfortunately, I'm not particularly handy. On every new project, the tools require blood.

<cite>[@Graham2023FindMyselfCharge]</cite>

::: notes

- daraus folgt, dass es neue Rollen und neue Anforderungen gibt

:::

## Generous thinking: zuhören und lernen

>Generous Thinking [begins] by proposing that rooting the humanities in generosity, and in particular in the practices of thinking *with* rather than reflexively *against* both the people and the materials with which we work, might invite more productive relationships and conversations not just among scholars but between scholars and the surrounding community.

<cite>[@Fitzpatrick2016GenerousThinking]</cite>

::: notes

- frage:
    - Wie kann Kollaboration zum Nutzen aller gestaltet werden?
- sie entwirft eine Kritik der neoliberalen Universität, in der, vor allem in den Humanities, eine destruktive Kritik geübt wird

:::

## trading zones, contact languages, and project management

>to coordinate and develop [...] ‘contact languages’ [..] is the necessary underpinning of a stable, respectful and hybrid form of interdisciplinary collaboration. Done correctly they can create something new: Galison’s ‘full-fledged creoles’  supporting ‘activities as complex as poetry and metalinguistic reflection’.  They can create new disciplinary spaces and practices in their own right. 

<cite>[@AhnertEtAl2023CollaborativeHistoricalResearch]</cite>


::: columns
:::: column

![](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/cover_Kemman2021.jpeg){#fig:book-kemman2021}

::::
:::: column

![](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/cover_Cremer2024.png){#fig:book-cremer2024}

::::
:::

::: notes

- Max Kemman und andere auf der Basis von Peter Galison
- contact zones müssen in "trading zones" verwandelt werden
    - Aber allein der Aufenthalt in einer Kontaktzone erfordert ein Mindestmaß an Toleranz
- Zonen der lokalen Verständigung, in den sich erst ein 
    - Pidgin und dann 
        - Pidgnization als die Periode, in der Labels, wie Digital History, sinnvoll sein können
    - Kreolisch entwickeln kann

- Peter Galison:
            >employed the metaphor of a ‘trading zone’ to explain  how engineers and physicists from a number of different sub-fields went about  collaborating with each other to develop particle detectors and radar.


:::

## Leistungen anerkennen

::: columns
:::: column

![](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/website_CRediT.png){#fig:credit}

::::
:::: column

Anteile an jeglichem Output transparent klassifizieren

- Seit 2012: [Contributor Role Taxonomy (CRediT)](https://credit.niso.org)
    - ANSI/NISO Standard (seit 2022)
    - 14 Rollen im gesamten Forschungsprozess
    - einige Zeitschriften erlauben weitere Unterscheidung als _lead_ ,_equal_ oder _supporting_
- Die [relators](http://id.loc.gov/vocabulary/relators) Taxonomie der LoC
- Und natürlich gibt es Zeitschriften zum Thema, z.B. [Accountability in Research](https://www.tandfonline.com/journals/gacr20)

Unsere Stakeholder und ihre Bedürfnisse kennen

- z.B. über die Entwicklung von Personae

::::
:::

::: notes

- CRediT
    - Rollen
        1. Conceptualization  
        2. Data curation  
        3. Formal analysis  
        4. Funding acquisition  
        5. Investigation  
        6. Methodology  
        7. Project administration  
        8. Resources  
        9. Software  
        10. Supervision  
        11. Validation  
        12. Visualization  
        13. Writing – original draft  
        14. Writing – review & editing
    - Außerhalb der Geisteswissenschaften weithin umgesetzt
    - >CRediT grew from a practical realization that bibliographic conventions for describing and listing authors on scholarly outputs are increasingly outdated and fail to represent the range of contributions that researchers make to published output. Furthermore, there is growing interest among researchers, funding agencies, academic institutions, editors, and publishers in increasing both the transparency and accessibility of research contributions.

:::

# KISS <br/>keep it simple, stupid
## minimal computing
### Was **wir brauchen** müssen **wir** schaffen mit dem was **wir zuhanden haben**

::: columns
:::: narrow

![Webseite der [GO::DH working group zu minimal computing](https://go-dh.github.io/mincomp)](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/website_mincomp.png){#fig:mincomp-website}

::::
:::: wide

>Das Haus ist gebaut aus den Steinen, die vorhanden waren 

<cite>[@Brecht1967SchlechteZeiten]</cite>

>minimal computing connotes digital humanities work undertaken in the context of some set of constraints. This could include lack of access to hardware or software, network capacity, technical education, or even a reliable power grid

<cite>[@RisamGil2022Introduction, §3]</cite>

>this implies learning how to produce, disseminate, and preserve digital scholarship ourselves, **without the help we can’t get**, even as we fight to build the infrastructures we need at the intersection of, with, and beyond institutional libraries and schools.

<cite>[@Gil+2016, 29]</cite>

::::
:::


::: notes

- minimal computing ist ein Ergebnis von GO::DH und Ereignissen und Bedingungen der Digitalität in Cuba
- Alex Gil's ideas resonated with me, upon meeting in Beirut in April 2015

:::

## Centering the *we* in "what do we need?"

::: columns
:::: column

### *wir* ist bestimmt durch geteilte

- Interessen
- Werte
    + Zugänglichkeit
    + Teilhabe
    + Nachhaltigkeit: sozial, ökologisch, technologisch
    + Verantwortlichkeit
    + Gerechtigkeit
    + [FAIR](https://www.go-fair.org/fair-principles/) principles
    + [CARE](https://www.gida-global.org/care) principles
    + -> digital commons

::::
:::: column

### *wir* bestimmt

- den spezifischen Kontext und die Arbeitsbedingungen
- unseren Zugang zu Fähigkeiten, Methoden, Arbeitszeit, Werkzeug, Material ...

::::
:::

::: notes

- FAIR: **F**indability, **A**ccessability, **I**nteroperability, **R**euse
- [CARE](https://www.gida-global.org/care): **C**ollective benefit, **A**uthority to control, **R**esponsibility, **E**thics 
    + developped in the context of indigenous communities

:::

## Was bedeutet *minimal*?

<!-- add images -->

::: columns
:::: column

### Aus einer privilegierten Position

- Minimalismus als Selbstzweck
    - Vorhandene Resourcen zerstörend
    - Mode
    - Prinzipieller Purismus

![[Webseite](https://bulthaup.com/en/b3/) für Luxus-Küchen](../../assets/dh/bulthaupt.png){#fig:bulthaupt}

::::
:::: column

### Aus einer marginalisierten Position

- Minimalismus als ein *Mittel* zum Zweck
    - Abwägung unserer Bedürfnisse und unserer Ressourcen
    - Anerkennung der unausweichlichen Folgen unserer Handlungen
    - minimal computing als *meaningful* computing

![Frankfurter Küche, Quelle: [WikiCommons, CCO](https://commons.wikimedia.org/wiki/File:SchutteLihotzky_FrankfurtKitchen_MIA_2004195_001.jpg)](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/SchutteLihotzky_FrankfurtKitchen_MIA_2004195_001.jpg/450px-SchutteLihotzky_FrankfurtKitchen_MIA_2004195_001.jpg){#fig:bauhaus}

::::
:::


::: notes

1. minimalism as an end
    - resource-intensive
    - example: Mary Condo
    - example: purist computing infrastructures
        + you got to run your own server and never use evil platforms
2. minimalism as a means to an end 
    + meaningful connectivity
    + original Bauhaus / modernist design:
        * form follows function to 
            - decrease the cost of industrial production
            - increase the material benefits of the expended resources

:::

## Und schließlich was ist mit *computing*<!-- in minimal computing-->?

::: columns
:::: column

- Nutze was wir bereits kennen
- Nutze was wir uns langfristig leisten könne
- Lege den Nutzer_innen keine unnötigen Kosten auf
- Verschwende keine Resourcen zum Schaden unsers Planeten

::::
:::: column

- Lerne *für uns* neue Techniken
- Entwickle Fähigkeiten
- Fördere und nähre Communities of Practice

::::
:::


::: notes

- first column
    + Etablierte Standards und bewährte Technologien
    + nicht das neuest Framework
        + es muss nicht glitzern und funkeln, es soll mit minimalem Aufwand lange laufen
        + Hier sollten wir uns an der Raumfahrtindustrie (nicht SpaceX) ein Beispiel nehmen: Voyager I and II are still functioning with rudimentary computing powers
    - Flache technology stacks

:::

## *Project Endings*


::: columns
:::: narrow

!["[Endings Principles for Digital Longevity](https://endings.uvic.ca/principles.html)"](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/website_project-endings-principles.png){#fig:endings-principles}


::::
:::: wide

- kollaboratives Projekt von Faculty, Bibliothekar_innen, Entwickler_innen an der University of Victoria, Kanada, zur Untersuchung 
- Hauptziele
    - Belange von Forscher_innen und Archivar_innen bei der langfristigen Kuratierung und Erhaltung von DH-Projekten in Einklang zu bringen
    - Entwicklung praktischer Werkzeuge.

::::
:::


::: notes

- bei den gezeigten Prinzipien wird ganz klar ein *minimal computing* Ansatz deutlich
- tools to assist with the archiving of both data and interactive elements of digital projects.

:::


## Digital Humanities Climate Coalition

it all started with a manifesto <!-- "Digital Humanities and the Climate Crisis" (2021)-->

::: columns
:::: column

![Webseite des [DHCC Toolkit](https://sas-dhrh.github.io/dhcc-toolkit/)](/Users/Shared/BachUni/BachBibliothek/GitHub/slides/assets/dh/website_dhcc.png){#fig:website-dhcc}

::::
:::: column

>The digital is material. As digital humanists, every project we create, every software application we use, every piece of hardware we purchase impacts our environment. [...] we aim to surface the ecological impacts of our work while learning with and from our DH community about ways to reduce harm to the environment and to the people most impacted by environmental injustices.
>As humanities researchers, it is also our role to probe the values, the power structures, and the future imaginaries that underpin sustainable solutions. Given, especially, the immense and monopolistic power wielded by the global tech sector, and the critiques of this power that are part of DH, our use of their resources should be informed by the ways corporate economic, cultural, and scientific power perpetuates and exacerbates the crisis.

<cite>[@BaillotEtAl2021DHCCManifesto]</cite>

::::
:::

::: notes

- 2021 manifesto
- seit 2022: Entwicklung des Toolkits
- DHd AG Greening DH

:::

# scholarly makerspace
## Makerspace

>Der Grundgedanke von Makerspaces ist das Teilen von **Räumen**, **Ressourcen** und **Wissen** innerhalb einer **Gemeinschaft**, welche Einzelpersonen sonst nicht zur Verfügung stünden 

<cite>[@Spath2019Makerspaces, 41]</cite>

::: notes

- Damit greifen makerspaces dem minimal computing vor
- Es gibt das "Maker Movement Manifesto" von Hatch (2013), der das Wort "Makerspace" geprägt hat
    + >Maker Movement Manifest von HATCH (2013), das die Prinzipien folgendermaßen beschreibt, zitiert werden dabei nur die Überschriften: „make, share, give, learn, tool up, play, participate, support“ und „change“. Betont werden also darin das konkrete Tun, das Teilen, der offene Austausch und das Lernen, der spielerische Zugang, Unterstützung und der Wille, etwas und sich selbst zu ändern als Prinzipien für Maker. [@SchonEbner2017Makerspaces]
- >Die physische und inhaltliche Ausrichtung des Makerspace ist in diesem Kontext entscheidend. Als **wichtige Schnittstelle zwischen formellem und informellem Lernen** verfolgen Makerspaces an Bildungseinrichtungen sehr unterschiedliche Ansätze, die von offenen interdisziplinären Werkstätten über mobile Fab Labs bis hin zu großflächigen 3D-Technologie-Laboren reichen. [@Heinzeletal2020Einleitung, 1]
- >Die Ermöglichung des Zugangs für alle, stellt so einen zentralen Faktor für eine offene und demokratische Gesellschaft dar. [@Heinzeletal2020Einleitung, 2]

:::


## Gegenstand

- digitale und computationelle Aspekte zeitgenössischer Geistes- und Kulturwissenschaften
- durch Forschungsfragen getrieben
- die Auswirkungen auf den Erkenntnisprozess untersuchend
- die gesellschaftlichen Auswirkungen untersuchend

::: notes

- durch Forschungsfragen getrieben:
    + Wie lassen sich genuin digitale, kulturelle Artefakte für die Zeitgeschichte des 21. Jahrhunderts einsetzen
    + Wie lassen sich (sehr) große Corpora mit *distant reading* statistisch valide erschließen?
    + Wie lassen sich Soziale Medien für die Untersuchung gesellschaftlichen Wandels in repressiven Systemen nutzen?
- die Auswirkungen auf den Erkenntnisprozess untersuchend:
    + Welche Auswirkungen haben OCR Algorithmen und Normalisierung auf die Qualität meines Korpus?
    + Was ist die Auswirkung von abstrahierenden Operationalisierungen für die quantitative Auswertung?
- die gesellschaftlichen Auswirkungen untersuchend?
    + Wie hoch ist der Verbrauch natürlicher Ressourcen für das Training einer KI auf die Klassifizierung von Abbildungen in mittelalterlichen Handschriften?
    + Was ist mit dem Einsatz von Sklaverei-ähnlichen Zuständen für die Herstellung und Erhalt der notwendigen technischen Infrastrukturen?
    + Welche Folge hat eine auf Beiträge in den Sozialmedien trainierte KI für die Hausratversicherungen in sozialen Brennpunkten?

:::


# Conclusion
## Summary

- Die minimale Lösung 
    - ist unter den Rahmenbedingungen zeitgenössischen Wissenschaft im Kontext von Polykrisen, **die einzig machbare**.
    - schont natürliche und menschliche Ressourcen.
    - trägt dazu bei, dass Forschung im Einklang mit guter Wissenschaftlicher Praxis steht.
    - **ermächtigt** alle Beteiligten am Forschungsprozess.
    - ermöglicht die Weiternutzung und Archivierung ihrer Ergebnisse.

### minimal computing principles

- build what **we need** with what **we have** at hand
    - *vorhanden* reicht im Sinne Heideggers nicht, Dinge müssen *zuhanden* sein
- as **few** as possible, **open** and **established** formats and tools
- running on **our** hardware
- with **our** skills and knowledge
- **free-to-use** platforms without lock-in of data