# TextMate Bundle for knitr noweb files

## Installation

Put this bundle in your TextMate bundle directory:

```bash
# For Textmate 2:
mkdir -p ~/Library/Application\ Support/Avian/Bundles/
cd ~/Library/Application\ Support/Avian/Bundles/
git clone https://github.com/fonnesbeck/knitr.tmbundle.git
```

## Commands

* __Knit, Typeset & View__ 
	* This is the main command. It will knit the R noweb file (Rnw, rnw), produce the tex file, then the pdf file and finally open it in the viewer you specified (edit the command to choose your favorite viewer).
* __Knit in R__
	* This command knits the file in R creating the tex file.
* __View (PDF)__
	* This command opens the PDF in the specified viewer. It is useful if you are using the _Knit in R_ command.
* __Insert R Code Chunk__
	* Inserts an R code chunk into the file. The chunk will have no options defined.
* __Change Block Parameters__
	* Changes the parameters of the R code chunk among a few options provided.
* __Fix Code Block Indent__
	* As the name suggests, it fixes the indentation of an R code chunk.
* __Select Previous Code Block__
	* Selects the previous code block in case that you then want to evaluate it in R using the [R TextMate bundle](https://github.com/textmate/r.tmbundle).
* __setwd in R__
	* Sets the current working directory in R using the `setwd()` R function.
	
For R markdown files (Rmd, rmd) you might be interested in the [Redcarpet Markdown TextMate bundle](https://github.com/streeter/markdown-redcarpet.tmbundle) which bridges GitHub flavored markdown and R code using [knitrBootstrap](http://cran.at.r-project.org/web/packages/knitrBootstrap/index.html) or [knitr](http://cran.r-project.org/web/packages/knitr/index.html).
