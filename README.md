# ScientificWriting
This is the repo for scientific writing.

It shall give you an idea on how to write reports on Case Studies on the LFC Cham for topics that are handed out by Prof. Weber.

There are many way on how to do Case Study reports as well as Thesis on a technical basis. 
One rule of thumb does apply: The content matters more than the means of how you arrive at the final report.

By adhering to those guidelines you make it easier for everyone to read, and finally grade, your papers.

# Structure

In general, you **MUST** comply to the following structure:

1) Introduction
2) Materials and Methods
3) Results
4) Discussion

Those four chapters are the last structure you will need in your life in order to do technical writing.
There is no technical/engineering/scientific writing topic on the face of this earth, that does not use this structure in one way or another.

The chapters can be appended by two (not so) optional chapters:

5) References
6) Appendix
7) Acknowledgements

Not all engineering/technical/scientific writing scenarios include an appendix. 
Usually, they do include references.

> [!IMPORTANT]
> In general: Always show if something (algorithm, code, figures) are **NOT** your own work. Below are guidelines on how to do that in various scenarios. Everything else is **PLAGIARISM** and will be treated as such.

> [!TIP]
> Aim for a high information density! No elaborate paragraphs that "look good". Think of every sentence: if new information is added - it is needed. if no information is added - it is not needed.

## Introduction

- describes the state of the art
- includes a literature research 
- identifies the research question based on the literature research
- the last paragraph/the last sentence *always* contains the actual research question at which you arrive

> [!Tip]
> Write the introduction *after* you finished (except for the literature review). This way it is easier to formulate the research question.

## Materials and Methods

- describes what you did
- describes what you used
- do not include results in this section
- show how and where the method was verified (if needed)
- you do not need to explain all methods in detail, you can cite the respective paper - but show where your approach may differ

>[!Tip]
> The materials and methods section can always be written during the actual work on the project.

## Results

- describes only the results
- no interpretations in the results section
- will be boring, but is necessary
- if you have figures of the same type it is enough to describe the results in the figure once and put repeated figures in the appendix
- do not repeat parts of the introduction or the M&M section

>[!Tip]
> The results are *just* reported, do **NOT** interprate the results in the results section.

## Discussion

- is the heart of your actual paper
- is where you can get creative
- consists of the following sub-structure
  1) short repetition of the research question in the introduction
  2) discussion of the results, connecting the dots
  3) strengths and limitations: there are **ALWAYS** strengths and limitations in **EVERY** study. If none are reported and discussed, it actually decreases the quality of your paper. Discuss how the limitations impact or may impact the results and report either counter actions you took or report some that are possible.
  4) future research: good research is always the basis for new studies, discuss new ideas/method/approaches, but keep this paragraph concise. Do add literature if applicable.
  5) conclude by summarizing the whole discussion in a concise paragraph and end with how the research question has been answered
  
>[!Tip]
> The discussion is *your* section. This is where you can get creative and show how the results fit together in the bigger picture. 
  
## References and Bibliography

Every engineering/scientific writing project is standing on the shoulders of giants[^1].
Therefore you will need to first read literature and also add literature to you final paper/final report.
There are numerous ways of how to do this, which also depend on your choice of writing style (WYSIWYG[^2] vs. WYSIWYM[^3]).

The lab uses it's own citation style which is fully specified in [`csl/SensorLab.csl`](csl/SensorLab.csl).
This folder contains a [`*.csl`-file ](csl/SensorLab.csl) which can be uses by many document processing systems, therefore ensuring a consistent citation style throughout the works.
The style is in essence the [Elsevier - Harvard (with titles)](https://editor.citationstyles.org/styleInfo/?styleId=http%3A%2F%2Fwww.zotero.org%2Fstyles%2Felsevier-harvard) style if you need to search differently for it and can not use it out-of-the-box.

[^1]: Newton, Isaac. "Letter from Sir Isaac Newton to Robert Hooke". Historical Society of Pennsylvania.
[^2]: (W)hat (Y)ou (S)ee (I)s (W)hat (Y)ou (G)et 
[^3]: (W)hat (Y)ou (S)ee (I)s (W)hat (Y)out (M)eam

### Literature management

There are many ways on how to manage literature.
It is recommended to use such a method together with an automated bibliography creation.
Creating a literature section once is not a problem, but with changes in your document also the literature section may change, as may the order of citations.
There are solutions on DIT on how to work with literature, follow this [link](https://www.th-deg.de/bib) to get involved with the DIT library.
Updating literature sections quickly becomes cumbersome and eats up a lot of your precious time - use software support.

1) CiteDrive: [CiteDrive](https://www.citedrive.com/en/) is a browser based application for the management of bibliographies. You have to sign up for it. You can add you identifiers (`doi`, `ISBN`, ...) and the reference should be imported correctly. You can also import a `bibtex` based citation, which will then be processed. It allows for more users to work on one bibliography. It connects to your document via an `API` key - if your are using `LaTeX` or `quarto` to write. You can get the citation key (which are automatically generated from the browser). I am using it - after many years of fiddling with bibliographies it is a warmly welcomed method to organize literature. 

2) JabRef: [JabRef](https://www.jabref.org/) is a Desktop application to manage literature. It is very powerful, but in some cases a little over the top (for my taste). It really is a good piece of software and build upon `bibtex` files (`*.bib`). You can also connect to a `PostgreSQL` database, which should make collaborative work easier. Open source - so if you want you can fiddle with the source code

3) bibtex: [bibtex](https://www.bibtex.org/) is the "language" on which both the technologies mentioned (CiteDrive and JabRef) are build upon. But you do not need a management software, you can organize your literature in a simple `*.bib` file in a text editor. This is a perfect valid method and especially useful if things go wrong.

4) zotero: [zotero](https://www.zotero.org/) is another management software for references. Its main advantage is probably the (supposedly) seamless integration with WYSIWYG software (like MS Word or its cousins). I never worked with it, but many colleagues do and it seems to be a good solution. It is also open source and free. 

5) citavi: [citavi](https://www.citavi.com/de) is also a desktop literature management software. As with `zotero` one of its main features is the seamless integration in WYSIWYG software.  I know many students who have worked with `citavi`, all of them were satisfied. You can get a license from [DIT bib](https://www.th-deg.de/bib), see the [Homepage](https://www.th-deg.de/bib) for more info on this.

6) Mendeley: [Mendeley](https://www.mendeley.com/) is again a desktop literature management software. It also integrates with popular WYSIWYG software, there are many citation styles online to look for. It used to have a great pdf importer a few years back.

## Appendix

Everything that belongs to your study/paper/project that does not "fit" into the upper sections goes in the appendix.
Stuff in the appendix should also be *referenced* throughout the paper/report.

Examples are:
- Code
- repeated figures (reporting the results in a similar)
- additional table

> [!Note]
> The appendix does **NOT** count for the word count or the length of your paper.

## Acknowledgments

Acknowledge people here.
You can put the author contributions for Case Studies here.

# Figures

It is very likely that you will have images in your paper/report. 
In general figure 

- need to have a caption *below* the figure
- need to have a number
- must be cited if not your own work, check the [license](https://commons.wikimedia.org/wiki/Commons:Licensing/en) 
- must be referenced in the text; if not referenced it will be deemed unnecessary and treated as such

> [!CAUTION]
> Figure that are not referenced in the text are not necessary and **MUST** be removed. This influences grading!

## raster images

- at least `300dpi` in resolution
- preferred file format: `*.png`, also possible: `*.tiff`, avoid: `*.jpg`, `*.bmp`
- only images that are referenced in the text (as in: needed) shall be used
- if the images are not your own work, cite the source
- ask for permission, check the [license](https://commons.wikimedia.org/wiki/Commons:Licensing/en) 
- no stock images

## vector graphics

- can be very useful for workflows, diagrams
- can be scaled indefinitely, very good for printed output
- use `*.svg` files (also web standard)
- use software to create: [inkscape](https://inkscape.org/de/) - open source and free, [Adobe Illustrator](https://www.adobe.com/de/products/illustrator.html) - closed source not free
- check the [svgrepo](https://www.svgrepo.com/)

## plots

- always label all axis
- add a title
- add a legend (if necessary), avoid legends (where possible)
- fontsize at least the fontsize of the text
- resolution at least `300dpi`, or use as vector graphic
- use colorblind friendly color palettes (e.g. `viridis`)
- gridlines only if information is added 
- in general: consider the [data-ink ratio](https://www.matthewdeverna.com/docs/notes/Tufte_dataInk.html) proposed by Edward Tufte[^4].

[^4]: Edward Tufte: https://de.wikipedia.org/wiki/Edward_Tufte

# tables

- need to have a caption *above* the figure
- need to have a number
- must be referenced in the text; if not referenced it will be deemed unnecessary and treated as such
- must have the same fontsize as the text

## Online table generator (static tables)

If you are using a WYSIWYM System you can use [online table generators](https://www.tablesgenerator.com/) that make it easier to compile tables.
All advantages of those systems aside, creating tables is a pain.

## table generator packages (copmutation tables)

R:
- [gt](https://CRAN.R-project.org/package=gt)
- [formattable](https://CRAN.R-project.org/package=formattable)
- [kableExtra](https://CRAN.R-project.org/package=kableExtra)
- [flextable](https://CRAN.R-project.org/package=flextable)
- ... and more online

python:
- [gt](https://posit-dev.github.io/great-tables/articles/intro.html)
- ... probably more that I do not know of

other languages:
- your are on your own

# pseudocode

If algorithms are included in your project that you want to describe thoroughly you can do this using `pseudocode`.
This is an effective and language agnostic way to describe the your algorithms.
For WYSIWYM systems there are packages and methods on how to include pseudocode.
There are many tips online on how to write [pseudecode](https://gist.github.com/camilstaps/59c4574ab8131fb83612a446606cbcba), check it out.

- Use mathematical notation when applicable.
- Don't rely on programming language conventions.
- You shouldn't have to explain your pseudocode.
- Pseudocode works better when strongly typed.
- Indent code blocks
- Use 'syntax' highlighting

> [!IMPORTANT]
> There should be no "real" code in the body of your text. The body of your text shall include pseudocode, the actual code goes in the appendix.

# Technial means of writing

There are two main ways of writing: (W)hat (Y)ou (S)ee (I)s (W)hat (Y)ou (G)et vs. (W)hat (Y)ou (S)ee (I)s (W)hat (Y)ou (M)ean.
The choice of writing does **NOT** influence your grade, its the content of your paper that matters.
The general guidelines above are stated in such a way, so that they are applicable for both writing styles.

## (W)hat (Y)ou (S)ee (I)s (W)hat (Y)ou (G)et - WYSISWYG

- arguably the most popular software out there
- software examples are: [MS Word](https://th-deg.de/it-services), Libre Office, Open Office
- rule of thumb: Quick results, but good formatting also takes time in this software
- writing mathematical equations used to be a pain (especially equation numbering)
- start the formatting *before* writing the thesis
- you have to adhere to the standards mentioned above, even if there is no template available out-of-the-box.

## (W)hat (Y)ou (S)ee (I)s (W)hat (Y)ou (M)ean - WYSIWYM

- arguably the most popular software out there
- software example are: LaTex, quarto, markdown
- content and formatting are seperated, which means formatting can (in theory) easily exchanged
- typesetting in LaTex is probably the most advanced on the planet
- steep learning curve
- once you know how to use it, and get to know the advantages, you may enjoy it
- you **DO NOT** have to use it

### LaTex

- Linux Distribution style
- Most popular distribution in WIN is [MiKTex](https://miktex.org/)
- Editors are available: [TexnicCenter](https://www.texniccenter.org/), [TexMaker](https://www.xm1math.net/texmaker/), [Notepadd++](https://notepad-plus-plus.org/)
- Popular Online Editor: [Overleaf](https://de.overleaf.com/)
- Vast number of packages available to do practically everything [CTAN](https://ctan.org/).
- can quickly become cumbersome, output is [beautiful though](https://i.sstatic.net/kv4NS.jpg) 

### quarto

- new kid on the block
- uses `markdown` formatting and is quite versatile because if this
- can be downloaded [here](https://quarto.org/) 
- does not **NEED** an editor, but works beautiful with [RStudio](https://posit.co/download/rstudio-desktop/)
- is cross platform
- can be extended [really easily](https://github.com/quarto-journals/)
- you should be able to download the `quarto_example` folder and use the template out-of-the-box.

# Case Study specific rules

## Abstract

- You **MUST** add an abstract to final paper/report.
- The abstract has no numbering and appears *before* the actual manuscript.
- The abstract must *mirror* all the chapters as introduced in the `Structure` section in proportion and content.

- Length of the abstract: 250-300 words

## Article

- linespacing: 1.5
- font: serif
- fontsize: 12-14pt
- number of pages: see length of the article
- single column

- Length of the article: 3500 - 5000 words (excluding: Appendix, Bibliography, Abstract, Acknowledgements, including: Headings)


## Submission - report

- ... **must** be completed on the communicated date (see [i-learn](https://ilearn.th-deg.de/) for the specific case study).
- ... **must** be **printed on A4 paper** and must be nondetachably connected to each other on the day of submission.
- ... **must be signed by all authors** including the printed name, the signature and the date
- ... **must** include Author contributions (see `Acknowledgments` section)

## Submission - files

- ... **must** be uploaded in i-learn link via Nextcloud (see the respective case study)
- ... **must** be in a `*.zip` (or [`*.7zip`](https://7-zip.de/)) archive
- ... **must** include a `readme.txt` or `readme.md` that clarify the contents of a file (also if the upload itself is only one file)
- ... **must** include all data up to `500MB`
- ... **must** be uploaded **BEFORE** your final presentation
- ... **must** contain all your presentations (start, intermediate, final)
- ... **must** follow the following naming convention: `GroupXX_GroupTitle`. All files that do not follow this convention will be ignored and count as **NOT SUBMITTED**
- ... are a prerequisite to pass the final gate (as in: no data, no gate)