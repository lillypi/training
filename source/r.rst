.. _r:

R
=

This page contains links for learning R at a variety of levels.

.. seealso::

    See :ref:`choosing-r-python` if you're trying to decide whether to learn
    R or Python


Beginner
--------

.. note::

    There are two "flavors" of R: base R, which has been around for many years,
    and the `"tidyverse" <https://www.tidyverse.org/>`_, which is more recent.
    They are both good, and you will see them both used in R code. For example,
    see `this page of comparisons
    <https://tavareshugo.github.io/data_carpentry_extras/base-r_tidyverse_equivalents/base-r_tidyverse_equivalents.html>`_
    between the two dialects.

    Norm Matloff, an R educator, has an excellent writeup called `The Tidyverse
    Skeptic <https://github.com/matloff/TidyverseSkeptic>`_ which talks about
    the challenges of having new R users start with the tidyverse.


- `R Programming 101 <https://www.youtube.com/c/RProgramming101>`_ is an
  extensive series of youtube videos that walk you though a variety of topics.
  These can be a good supplement to the resources below, especially when you
  need a break from the written format.

- `Swirl <http://swirlstats.com/>`_ Learn R, in R. An interactive
  tutorial that walks you through the basics. It runs in R itself.

- `FasteR <https://github.com/matloff/fasteR>`_, which has the tagline
  "Becoming productive in R, as fast as possible". This teaches you base R in
  a way that focuses on getting you working with real data quickly.

- `Hadley Wickham's R for Data Science <http://r4ds.had.co.nz/>`_ A
  book on the basics of R focusing on the new-style method
  (“tidyverse”) of interacting with dataframes. It starts you off quickly with
  plotting, which can be rewarding.

- `Hadley Wickham's Advanced R <https://adv-r.hadley.nz/>`_ If there’s
  one single R resource to read, it’s this one. Lots of details, well-written,
  comprehensive . . . yet still accessible to relative beginners. The later
  chapters do get fairly advanced, but the first section ("Foundations") is
  good for beginners.

- `Ten simple rules for teaching yourself
  R <https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010372>`_
  is part of PLOS Comp Bio's "ten simple rules" series. This one has some
  advice for learning R on your own that could be helpful.

- These `cheatsheets from RStudio
  <https://rstudio.com/resources/cheatsheets/>`_ summarize lots of information
  into compact form.

- `R in 8 pages <https://github.com/saghirb/Getting-Started-in-R>`_
  Practical approach of showing how to do things immediately using
  realistic examples and a real life dataset.

- `Software Carpentry's "R for Reproducible Scientific Analysis"
  <https://swcarpentry.github.io/r-novice-gapminder/>`_ These are workshop
  materials for a course commonly taught on NIH campus.

- `NIH Library R courses <https://www.nihlibrary.nih.gov/training/calendar>`_
  The NIH Library in Bldg 10 offers periodic R workshops, though they fill up
  quickly.


- `Efficient R <https://csgillespie.github.io/efficientR/>`_ Once
  you’re comfortable with R and looking to improve efficiency, have a look through this book. 

- `Data Visualization: A Practical Introduction <http://socviz.co/>`_
  A data visualization-centric approach to learning R. Also has some
  great discussions on what makes a plot good or bad (channeling a fair
  amount of Tufte in the process)

Intermediate
------------

- `Modern Statistics for Modern Biology
  <http://web.stanford.edu/class/bios221/book/introduction.html>`_ assumes you
  know R, and goes deeper into many important and useful statistical methods.
  There are exercises and solutions as well. Very well written.

- `R packages <https://r-pkgs.org/>`_ describes how to packages your R code so
  it can be redistributable.

- `Chapter
  7 <https://dtkaplan.github.io/SM2-bookdown/model-formulas-and-coefficients.html>`_
  of Statistical Modeling by Daniel Kaplan gives a great introduction to model
  formulas in R, especially important for handling things like batch effects in
  RNA-seq data.

Skills
------

Here I've attempted to list the various skills you might be expected to know at
various levels. I've tried to keep it to base R, but ggplot2 and dplyr are so
ubiquitous they are becoming de facto base R, so I've included them here as
well.

Level 1
~~~~~~~
- Working in RStudio
- Data types (logical, numeric, character)
- dealing with NA
- load a TSV or CSV into a dataframe
- select rows or columns from a dataframe
- select items from vector or list
- save output to file
- know the differences between vector and list, or between dataframe and matrix
- rownames, colnames
- usage of ``c()``
- writing functions
- basic statistics (t-test, Fisher's exact test, ANOVA, lm)
- basic plots
- ``?`` for getting help
- installing packages with ``install.packages``
- loading packages
- ``str()``
- combining dataframes with rbind/cbind
- if/else
- for-loops
- Basic ggplot2 (scatter, line, histograms)

Level 2
~~~~~~~
- Working outside of RStudio (text file and command-line R interpreter)
- factors (how they work, how they can be a problem)
- ggplot2 additional layers, faceting
- type coercion
- know mulitple ways of selecting from a dataframe
- apply, lapply, sapply
- dplyr: filter, select
- nested lists
- using RMarkdown for literate programming
- formula specification for linear models
- reverse-engineering an object using ``str()`` and the source code
- dplyr: mutate
- dplyr: joins
- dplyr: group_by and summarize
- tidyr: spread/gather (or pivot_longer, pivot_wider)
- caching code chunks in RMarkdown
- debugging (e.g., ``options(error = recover)``)

Level 3
~~~~~~~
- environments
- batch effects, interaction terms in linear models
- object-oriented programming with S3 and S4 objects
- packaging
- testing
- publishing to CRAN or Bioconductor


Shiny
-----

Shiny is an R package that lets you develop web applications with graphical
user interfaces very quickly. This is fantastic if you have everything
installed on your machine and you want to run a web app to interactively look
at data. However it is difficult to host Shiny apps on your own in such a way
that other people can access it from their computers.

NICHD hosts an RStudio Connect instance, which *does* allow you to post your
own apps so other people can access it from their computers. Contact
ryan.dale@nih.gov for more info on this.

- `Main Shiny tutorial <https://shiny.rstudio.com/tutorial/>`_ from the developers

- `Extensive Shiny tutorial
  <http://zevross.com/blog/2016/04/19/r-powered-web-applications-with-shiny-a-tutorial-and-cheat-sheet-with-40-example-apps/>`_


Bioconductor
------------

R has two main repositories of packages: CRAN and Bioconductor. Bioconductor is
for bioinformatics and biology packages, and CRAN is for everything else.
Bioconductor packages need to satisfy lots of documentation and testing
criteria, so they are typically high-quality packages.

The `main Bioconductor page <https://www.bioconductor.org/>`_ has installation
instructions and links for exploring packages. Bioconductor is a vast resource
though, so rather than try to learn it all in practice you'll typically find
a package that does what you want and then read the vignette (a tutorial that
comes with the package) to learn how to use it.

scRNA-seq
~~~~~~~~~

Recently, many people have been asking about R specifically so that they can
learn how to work with scRNA-seq on their own.

.. note::

    If you jump right in to the Seurat tutorials without knowing R, you won't know
    which commands are standard R and which are Seurat-specific. And if your data
    do not exactly match their example data, it will be unclear how to modify the
    code to suit your data if you don't know R.

    You should be fine with the "Level 1" set of R skills above to start using
    Seurat effectively. See the "Beginner" section above for learning these
    skills.


There are several major packages
for scRNA-seq: `Seurat <https://satijalab.org/seurat/>`_, a `suite of
Bioconductor packages <https://bioconductor.org/books/release/OSCA/>`_, and
`scanpy <https://scanpy.readthedocs.io/en/stable/>`_. Seurat and Bioconductor are
in R, scanpy is Python. They are broadly the same, but are in somewhat of an
arms race so some new features or analyses may not be immediately available in
all of them.

The book `Orchestrating Single-Cell Analysis with Bioconductor
<https://bioconductor.org/books/release/OSCA/>`_ is a fantastic, comprehensive
resource that even goes through worked examples of published data. This uses
the suite of tools in Bioconductor. Highly recommended.

`Seurat <https://satijalab.org/seurat/>`_ is another popular package for
scRNA-seq, and has a series of vignettes on the home page. There have been
recent improvments to the normalization (scTransform v1 and v2), and these use
somewhat different steps. The different vignettes therefore differ in the
steps, and it can be a bit confusing. The `PBMC3k tutorial
<https://satijalab.org/seurat/articles/pbmc3k_tutorial.html>`_ is the classic
starting point, so working through this one will at least give you the context
to work through other vignettes.

Additional resources
--------------------

- Curious about factors? See `this blog post
  <https://notstatschat.tumblr.com/post/124987394001/stringsasfactors-sigh>`_
  describing the details.
