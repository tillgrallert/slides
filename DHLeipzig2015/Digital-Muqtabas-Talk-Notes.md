# The journal *al-Muqtabas* between Shamela.ws, HathiTrust, and GitHub: producing open, collaborative, and fully-referencable digital editions of early Arabic periodicals—with almost no funds.

[https://www.github.com/tillgrallert/digital-muqtabas](https://www.github.com/tillgrallert/digital-muqtabas)

@tillgrallert

<grallert@orient-institut.org>

# The problem

- Preservation: 
    + Active destruction of cultural artifacts: iconoclasm, neolibralism
    + fragile materiality
- Access:
    + Absence / destruction of infrastructure / channels of knowledge transmission: lack of access to institutions, hardware, software, internet connections
    + widely-dispersed collections
    + technologies: absence of reliable OCR
    + technical skills: lack of basic scripting skills
- Consequences: focus on "high" culture and canonical texts

# Importance of mundane texts / periodicals

- at the core of various discourses
    + Modernity / -ism at the end of empire
    + Arabic renaissance
    + Arab nationalism
    + Islamic reform movement
- large corpora with an equal distribution along a temporal axis
    + liguistic analysis
    + historical semantics
    + data sets for social history

# State of digitisation

1. gray online libraries / "crowd"-sourced transcriptions
    + lack of metadata
    + unknown editing principles
    + unkown quality
    + cannot be reliably cited 
2. Digital imagery
    + lack of metadata
    + licences
    + no text layer

# Suggested solution: unite the two

- improve and validate the transcription with the facsimiles
- make it cite-able for scholars, referencable for machines
- re-purpose available tools, technologies, and material
    - preference for open and simple formats and tools
- provide the new edition with the broadest possible licence to facilitate access and re-use 


# Test case: digital *Muqtabas*

[https://www.github.com/tillgrallert/digital-muqtabas](https://www.github.com/tillgrallert/digital-muqtabas)

1. Basis: Generate and share the TEI edition of all 96 issues (c. 7000 pages)
2. Core feature: gradually improve the digital edition 
3. Sugar on top: Static webview (doesn't require a permanent internet connection)


# 1. Basis: Generate the TEI edition

- crawl the [digital text from *shamela.ws*](http://shamela.ws/index.php/book/26523)
- automatically transform it into [TEI XML](http://www.tei-c.org)
    + documented URI design to reference all elements
- link to digital facsimiles from the [British Library's "Endangered Archives Programme" (EAP)](http://eap.bl.uk/database/overview_project.a4d?projID=EAP119;r=63) and [HathiTrust](http://catalog.hathitrust.org/Record/100658549) or produce your own imagery
- host everything but images on [GitHub](https://www.github.com)
    + distributed version control
    + attribution of authorship
    + provide a [CC BY-SA 4.0 licence](http://creativecommons.org/licenses/by-sa/4.0/) for all files: edition, tools, webview

# 2. Core feature: Continuously improvement

- correct the transcription
- provide reliable bibliographic metadata based on the facsimile
- add structural mark-up
- add semantic mark-up

# 3. Sugar on top: webview

[https://rawgit.com/tillgrallert/digital-muqtabas/master/xml/oclc_4770057679-i_60.TEIP5.xml](https://rawgit.com/tillgrallert/digital-muqtabas/master/xml/oclc_4770057679-i_60.TEIP5.xml)

- Adaptation of [TEI Boilerplate XSLT stylesheets](http://dcl.slis.indiana.edu/teibp/)
- human-readable and static webview (either rawgit or gh-pages)
    + can be run without a continuous internet connection and with local facsimiles
- parallel display of text and facsimile
    + simple changes to display different facsimiles
- link to metadata on the article level (BibTeX)

# To do, ongoing work

- Schema design
- mark-up of page breaks
- Webview needs some polishing

# Experiences

- Simple technologies and relatively little coding needed: Initial set-up took less than four weeks of after-hour labour
- Hosting with GitHub is free
- Core (but simple) features cannot be automated: page breaks must be manually tagged
- Code that can be repurposed
    + TEI schema for Arabic periodicals
    + customisation of TEI boilerplate for parallel display of Arabic texts and facsimiles
    + conversion from EPub to TEI 
    + automatic extraction of metadata for every level of the text
