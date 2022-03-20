# The Legrand Orange Book
This book template can be used for writing anything from fiction, to technical documentation, to advanced mathematics, due to its extensive examples of document elements and many levels of sectioning. A key feature of the template is the orange theme, parts pages and chapter images which give the template its unique aesthetic.


# Authorship
This template was originally created by **[Mathias Legrand](mailto:legrand.mathias@gmail.com)** with inspiration from the material found [here](http://pgoutet.free.fr/latex) and [here](https://cel.archives-ouvertes.fr/cel-00814877/). 

This code is hosted in [LaTeX Templates](https://www.latextemplates.com/template/the-legrand-orange-book), but re-uploaded here (by me) to maintain the code and to see what changes has been made.

It has been extensively modified by [Vel](vel@latextemplates.com).

# License
This template is licensed under a **[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)** license. [Click here](https://www.latextemplates.com/license-explanation) to see what this license means for your use of the template.

# Demo
You can see how the book will look like in the [the-legrand-orange-book.pdf](the-legrand-orange-book.pdf) file.

# Description
This book template is very flexible and can be used for writing anything from fiction, to technical documentation, to advanced mathematics. This is due to its extensive examples of document elements such as a copyright page, lists of figures/tables, theorems, bibliography, index and appendices. The template is strongly sectioned and six levels of sections are available: parts, chapters, sections, subsections, subsubsections and paragraphs. Each gives rise to a distinct style within the template, from the beautiful major part pages, to the bold chapter images, to the smaller levels getting more and more diminutive. Section numbers are displayed in the left margin, making titles aligned neatly with the main text body. Sections and subsections also appear on part pages to provide an outline of the content to come at this major level.

The template is divided into four chapters housed in two parts to show broad categories of document elements that can be included in your book. 

**Chapter 1** shows the way that paragraphs of text look in the book, as well as all levels of sectioning (both numbered and unnumbered). This acts as an example for using this template for writing longform text, such as in a novel, article or report. 

**Chapter 2** shows common in-text elements including: references to publications, links, lists, international characters and ligatures. This shows how the template styles these elements and gives you examples to copy for your own content. 

**Chapter 3** shows advances mathematics examples with multiple styles for theorems, definitions, notations, remarks, corollaries, propositions, examples, exercises, problems and vocabulary. These are useful if you would like to use the template for an advanced technical work requiring these elements. 

**Chapter 4** has examples of including results in figures and tables, both fixed-position and floating. 

The **Bibliography** is split by articles and books but can be easily amalgamated or further split if needed. 

The **Index** shows index entries split nicely by the first letter and then appearing in two levels. 

Finally, **Appendices** chapters are shown as examples for when you have additional content to include that is for reference only.


# Usage Guide
## Compilation
This template should be compiled with standard pdflatex but it features a bibliography and index which need to be compiled separately using biber and makeindex. When you first download the template, run the following commands on the command line to compile it fully:

```
pdflatex main
makeindex main.idx -s indexstyle.ist
biber main
pdflatex main (twice)
```

If you are using a LaTeX editor, you can run the steps above within your editor by selecting the relevant typesetting engine for each step, but be careful that your editor is likely to not use the index style file without manual tweaking of how it runs makeindex.

If your LaTeX distribution is configured correctly and you have run the commands in the right order with the right parameters, you should end up with the same PDF as the preview PDF listed on this page. As you write your book, when you need to update the bibliography or index, use the appropriate command above and make sure to compile with pdflatex several times afterwards to propagate your changes to the document.

## Modifying Chapter Images
A key feature of this template is the large chapter images and colored boxes holding chapter titles. You can choose to use the same chapter image for your entire book, or you can change it for every chapter using 3 commands defined and used in the template. The commands are initially set in the preamble and their values can be changed anywhere in the template, the commands are: ```\chapterimage```, ```\chapterspaceabove``` and ```\chapterspacebelow```.

Use ```\chapterimage{image.jpg}``` to change the image used for all subsequent chapter images. This image should be copied into the Images folder with the template and should be much wider than tall to not take up too much vertical space on chapter pages. ```\chapterspaceabove{length}``` is used to set the vertical whitespace from the top of the page to the chapter title and ```\chapterspacebelow{length}``` sets the amount of vertical whitespace from the top margin to the start of the text on chapter pages. You will need to change these values if your chapter images are different dimensions and it is advisable to keep spacing of the chapter title above the bottom of the chapter image and the start of the chapter text below the bottom of the image roughly equal across chapters.

## Indexing
Add index entries anywhere in your text using the ```\index``` command. Indexes can contain two levels which are created as follows:
```
What's in a name?\index{Names} 
People often have first names\index{Names!First} 
and last names\index{Names!Last}.
```
