# Knitr bundle for TextMate

## Introduction

This bundle produces basic [`knitr`](http://yihui.name/knitr/) funcationality in TextMate. `knitr` is an R package for dynamic report generation with R, and is essentially an enhanced re-implenentation of `knitr`. This bundle was adapted from the `knitr` bundle by Alan Schussman.

The bundle works in conjunction with the R bundle by using the same context for embedded R code: Use the regular couple of R commands to send code to R from TextMate.

**Last modified**: 2014-02-20

## Using the bundle

### Language

The `knitr` bundle uses a simple language configuration, essentially copying a couple of elements from the R and LaTeX bundles and adding code to recognize `knitr` code within a document. `knitr` files get the overall context of text.latex.knitr; this prevents the bundle from hijacking the gear menu for regular LaTeX files while allowing for the use of all the features of the LaTeX bundle within `knitr` files. It also parses \Sexpr{} commands inline and assigns them the context meta.knitr.latex so that they can be given their own color highlighting.


### Usage

Usage is straightforward. There are two main commands: **Knit in R** and **Knit, Typeset & View**. The former sources the current *.rnw* file in R, after which the resulting *.tex* file can be compiled via the LaTeX Bundle's build command (now **cmd-R**). **Knit, Typeset & View* does all of this on one step, and presents the output in your chosen PDF viewer.

Typeset: When using the `knitr` Bundle, you should always set the TM_LATEX_MASTER variable so that you can use the normal LaTeX compile command. Set this either to the master .tex file that includes your `knitr`-built files, or to the name of your working `knitr` file, with .tex substituted for the Snw/Rnw extension. If you haven't set this variable, you can use the LaTeX typeset command built in to the `knitr` bundle. However, the typeset command in the LaTeX bundle is likely to be more recently-updated, so it's preferable to simply set TM_LATEX_MASTER.


### Other elements

The bundle includes a couple of snippets and commands that are as useful in R as they are in `knitr`:

* Insert section/figure: Quick snippets for boilerplate `knitr` section and figure blocks.

The commands are also explained at the [knitr.tmbundle GitHub repository](https://github.com/fonnesbeck/knitr.tmbundle). If you want to propose any changes, please submit a pull request.


#### Contact

* chris.fonnesbeck at vanderbilt.edu

