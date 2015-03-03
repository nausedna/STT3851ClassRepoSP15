---
title: "Automagic References using Zotero with R Markdown"
author: "Alan Arnholt"
date: "Spring 2015"
output: html_document
bibliography: ["Items.bib", "Rpkgs.bib"]
---

The only references from your `Items.bib` file that will appear at the end of a document are those that have been cited in the text.  You can use `nocite` to get a full bibliography but we will not discuss that further here.  When you create your `*.Rmd` file, you will need to add the line `bibliography: Items.bib` to the YAML metadata section.  If you have more than one `*.bib` file, place each file indented on a separate line, preceeded with a dash, and make sure to leave a space after the dash.

```bash
bibliography:
    - First.bib
    - Second.bib
    - Third.bib
```


The YAML metadata for this document could be written as

```bash
---
title: "Automagic References using Zotero with R Markdown"
author: "Alan Arnholt"
date: "December 25, 2014"
output: html_document
bibliography: 
    - Items.bib
    - Rpkgs.bib
---
```


To create an `Items.bib`, 

* First, highlight the titles you want to select in Zotero.  
* Second, for Windows users, right click on the highlighted items; for Mac users, Control-click on the highlighted items. 
* Third, select **Export Items**.  Use the drop down menu to select **Bib$\TeX$** not **Bib$\LaTeX$** as the format. 
* Fourth, click OK.  Change the name of the file to `Items.bib` in the **Save As:** box. 
* Fifth, click **Save**.


I will use [@beck2014; @rich2013; @murp2012; @dean2014] for this work which was obtained using `[@beck2014; @rich2013; @murp2012; @dean2014]`.  Plus, @beck2014 says some interesting stuff and that citation was obtained using `@beck2014`.  For more documentation on bibliographies and citations with R Markdown, see [http://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html](http://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html).  For general help with R Markdown, see [http://rmarkdown.rstudio.com/RMarkdownReferenceGuide.pdf](http://rmarkdown.rstudio.com/RMarkdownReferenceGuide.pdf).  The author of `knitr` [@R-knitr] is very generous with his time online! A very useful package for citing work with R Markdown is `knitcitations` [@R-knitcitations].  If you did not watch the [RStudio Reproducible Reporting webinar](http://www.rstudio.com/resources/webinars/) from `week01`, watch it now!

# References
