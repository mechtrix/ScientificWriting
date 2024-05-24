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
7) Acknowldegements

Not all engineering/technical/scientific wirting scenarios include an appendix. 
Usually, they do include references.

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
There are numerous ways of how to do this, which also depend on your choice of writing style (WYSIWYG vs. WYSIWYM).

The lab uses it's own citation style which is fully specified in [`csl/SensorLab.csl`](csl/SensorLab.csl).
This folder contains a [`*.csl`-file ](csl/SensorLab.csl) which can be uses by many document processing systems, therefore ensuring a consistent citation style throughout the works.
The style is in essence the [Elsevier - Harvard (with titles)](https://editor.citationstyles.org/styleInfo/?styleId=http%3A%2F%2Fwww.zotero.org%2Fstyles%2Felsevier-harvard) style if you need to search differently for it and can not use it out-of-the-box.

[^1]: Newton, Isaac. "Letter from Sir Isaac Newton to Robert Hooke". Historical Society of Pennsylvania.

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
> The appendix doe **NOT** count for the word count or the length of your paper.

## Acknowledgments

Acknowledge people here.
You can put the author contributions for Case Studies here.

# Figures

It is very likely that you will have images in your paper/report. 
Please follow the following guidelines/tips.

## raster images

- at least `300dpi` in resolution
- preferred file format: `*.png`, also possible: `*.tiff`, avoid: `*.jpg`, `*.bmp`
- need to have a caption
- need to have a number
- only images that are referenced in the text (as in: needed) shall be used
- if the images are not your own work, cite the source
- ask for permission, check the [license](https://commons.wikimedia.org/wiki/Commons:Licensing/en) 
- no stock images

## vector graphics

- can be very useful for workflows, diagrams
- can be scaled indefinitely, very good for printed output
- use `*.svg` files (also web standard)
- use software to create: [inkscape](https://inkscape.org/de/) - opens source and free, [Adobe Illustrator](https://www.adobe.com/de/products/illustrator.html) - closed source not free

## plots

- always label all axis
- add a title
- add a legend (if necessary), avoid legends (where possible)
- fontsize at least the fontsize of the text
- resolution at least `300dpi`, or use as vector graphic
- use colorblind friendly color palettes (e.g. `viridis`)
- gridlines only if information is added 
- in general: consider the [data-ink ratio](https://www.matthewdeverna.com/docs/notes/Tufte_dataInk.html) proposed by Edward Tufte[^2].

> [!CAUTION]
> Figure that are not referenced in the text are not necessary and **MUST** be removed. This influences grading!

[^2]: Edward Tufte: https://de.wikipedia.org/wiki/Edward_Tufte


