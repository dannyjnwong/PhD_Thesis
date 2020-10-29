# PhD_Thesis

This repository contains the code to reproduce my PhD thesis in its entirety. To reference my thesis use the following citation: **Wong DJN**. *Postoperative Critical Care: Resource Availability, Patient Risk and Other Factors Influencing Referral and Admission*. Doctoral thesis. UCL (University College London); 2020. Available from: https://discovery.ucl.ac.uk/id/eprint/10108589/

The thesis was written entirely in [R Markdown](https://rmarkdown.rstudio.com/), and therefore contains both programming code in R used for the statistical computing and data cleaning that was needed for all analyses performed wihin the thesis, as well as the literary text of the thesis itself. For a primer on writing multi-chapter R Markdown documents, click [here](https://dannyjnwong.github.io/Writing-a-multi-chapter-document-with-R-Markdown/. 

# Structure

- `source/` contains the source code needed to compile the entire thesis. Within that are 12 `.Rmd` files, each which can be knitted into their own chapter. `00-CompiledReport.Rmd` is the parent document that when knitted will stitch each chapter together into a complete document.

- `references/` contains the bibliographic information needed for all the references and citations within the thesis. The references are stored in `SNAP2.bib`, a [BibTeX file](https://en.wikipedia.org/wiki/BibTeX), which can be found in the `references/bib/` subfolder. There is a `vancouver.csl` citation style sheet which is used when knitting the document for formatting the references according to the UCL thesis requirements.

- `output/` contains the following files:

>`00-CompiledReport.docx`, which is the knitted document produced from `00-CompiledReport.Rmd` in the `source/` folder.

>`PhDThesis_Revised_DannyWong_20200808_OnlineVersion.docx` is a document that I made using `00-CompiledReport.docx`, performing formatting tweaks within Microsoft Word, e.g. adding a Table of Figures and Table of Tables, and fixing up some other final aesthetics.

>`PhDThesis_Revised_DannyWong_20200808_OnlineVersion.pdf` is the final saved thesis in `.pdf` format, ready for printing and submission.

# Caveats

This repository does not contain the **data** needed to recompile the entire thesis. While I have shared some of that data before, [here](https://dannyjnwong.github.io/Sharing-data-alongside-code/) and [here](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1003253), There are some remaining bits of SNAP-2: EPICCS data that I still cannot share for [various reasons](https://dannyjnwong.github.io/Sharing-code-whats-the-point/). However, it is my hope that by sharing this code, someone might find it useful for conducting their own research in the future, as well as have some idea about how they might make a multi-chapter document using R Markdown.
