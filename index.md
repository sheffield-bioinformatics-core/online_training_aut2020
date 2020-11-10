---
title: "Bioinformatics Training Nov/Dec 2020"
author: "Sheffield Bioinformatics Core"
output: 
  html_document: 
    toc: yes
    toc_float: yes
    css: stylesheets/styles.css
editor_options: 
  chunk_output_type: inline
---

<img src="images/logo-sm.png" style="position:absolute;top:40px;right:10px;" width="200" />


## Contact

web : [sbc.shef.ac.uk](https://sbc.shef.ac.uk)  
twitter: [SheffBioinfCore](https://twitter.com/SheffBioinfCore)  
email: [bioinformatics-core@sheffield.ac.uk](bioinformatics-core@sheffield.ac.uk)

# November 2nd/6th - Introduction to Data Manipulation and Visualisation using R

## Overview

As the data generated from high-throughput biological experiments increase in volume and become more complex, the ability to manipulate and visualise data is a highly-desirable skill in academia and industry. Whilst familiar tools such as Excel allow basic manipulations, they are often not scalable to larger datasets and are not ameanable to reproducible analysis. 

R is a highly-regarded, free, software environment for statistical analysis, with many useful features that promote and facilitate reproducible research.

In this course, we give an introduction to the R environment and explain how it can be used to import, manipulate and visualise tabular data. 

After the course you should feel confident to start exploring your own dataset using the materials and references provided. 

## Setup

These instructions are also described in a video:- [https://youtu.be/QIubJ8W8R4g](https://youtu.be/QIubJ8W8R4g)

1) First, install both R **and** RStudio for your operating system. 

### Windows

Install R by downloading and running [this .exe file](http://cran.r-project.org/bin/windows/base/release.htm) from CRAN. Also, please install the [RStudio IDE](http://www.rstudio.com/ide/download/desktop). Note that if you have separate user and admin accounts, you should run the installers as administrator (right-click on .exe file and select "Run as administrator" instead of double-clicking). Otherwise problems may occur later, for example when installing R packages.

### Mac

Install R by downloading and running [this .pkg file](http://cran.r-project.org/bin/macosx/R-latest.pkg) from CRAN. Also, please install the free [RStudio IDE](https://www.rstudio.com/products/rstudio/download/#download) 

### Linux

You can download the binary files for your distribution from CRAN. Or you can use your package manager (e.g. for Debian/Ubuntu run `sudo apt-get install r-base` and for Fedora run `sudo yum install R`). Also, please install free [the RStudio IDE](https://www.rstudio.com/products/rstudio/download/#download). 


  
2) Please download and extract (un-zip) [this zip file](CourseData.zip) into the directory on the computer that you wish to work in

3) Create an RStudio project using the menu **File -> New Project -> Existing Directory** and browse to the directory that you extraced the zip file to. Rstudio will refresh so that the working directory corresponds to the course data folder.

4) Type the following into the R console to install some extra R packages required for the workshop

```
install.packages("dplyr")
install.packages("ggplot2")
install.packages("readr")
```



**Mac Users may get the following error message when trying to install these packages**

```
xcrun error: inactive developer path (/Library/Developer/CommandLineTools), missing xcrun at:.....

```

If this is the case, you will need to follow the instructions from this link to install "Xcode"

[https://apple.stackexchange.com/questions/254380/why-am-i-getting-an-invalid-active-developer-path-when-attempting-to-use-git-a](https://apple.stackexchange.com/questions/254380/why-am-i-getting-an-invalid-active-developer-path-when-attempting-to-use-git-a)

**Window users might get a message that Rtools is required. This shouldn't be neccesary, but you might need it for other packages. It can be installed here:-**

[https://cran.r-project.org/bin/windows/Rtools/](https://cran.r-project.org/bin/windows/Rtools/)


5) Check your installation. You can check everything is installed by copying and pasting this into the R console

```
source("https://raw.githubusercontent.com/sheffield-bioinformatics-core/r-online/master/check_packages.R")

```

Please watch this short presentation (<10 minutes) before attending the workshop

- [Course Introduction](https://www.youtube.com/watch?v=bb-qyh3c9vE)

## Course Notes

+ [Introduction Slides](http://sbc.shef.ac.uk/r-online/intro_slides.html)
+ [Part 1](part1.nb.html)
+ [Part 2](part2.nb.html)



# November 10th - Statistical Analysis

## Overview

This course provides a refresher on the foundations of statistical analysis. The course is aimed at scientists at all levels – especially those whose formal education likely included statistics, but who have not perhaps put this into practice since. The focus of the course is on understanding the principles behind statistical testing, how to choose and execute the most appropriate test for your data, and how to interpret the result.

## Setup

Please download and unzip [this file](http://sbc.shef.ac.uk/stats-in-r/stats_course.zip)

Please watch these lectures before the workshop on November 10th

- [Introduction](https://youtu.be/towMwBtg0KA)
- [Part 1](https://youtu.be/UXdsOBcsBjA)
- [Part 2](https://youtu.be/oDjOSV5yas4)
- [Part 3](https://youtu.be/uL6N07w3L18)

## Course Notes

- [Notes and exercise solutions](https://sbc.shef.ac.uk/stats-in-r/practical.nb.html)


# Dec 8th/11th - Introduction to RNA-seq analysis


## Overview

High-throughput RNA-sequencing is now the standard technique for quantifying transcript abundance in a biological sample of interest. In this course we will describe the processes that take place once you submit a library for RNA sequencing, and what data you should expect to receive from the Bioinformatics Core.

We will describe the steps involved to go from sequencing library to a list of genes that show statistically significant differences between your biological conditions of interest. Practical sessions will use the user-friendly Galaxy interface (https://usegalaxy.org/) to demonstrate tasks such as *alignment*, *quality control* and *assessing differential expression*. We will also showcase some web sites you can use for enrichment and pathways analysis.

*Please note that the course will not cover the analysis of RNA-seq data using the  R programming langugage*

## Setup

- Please register for an account at [usegalaxy.eu](https://usegalaxy.eu).**Make sure to check your email to activate your account**
- Please download the GSEA app from 
[http://software.broadinstitute.org/gsea/downloads.jsp](http://software.broadinstitute.org/gsea/downloads.jsp) for your operating system (GSEA_Win_4.1.0-installer.exe or GSEA_4.1.0.app.zip)
- Please watch these pre-recorded lectures

  + [Introduction and Experimental Design](https://youtu.be/YtOG-77FfIg)
  + [RNA-seq workflow overview](https://youtu.be/m1x4CaLg90A)
  + [Functional Gene Analysis](https://youtu.be/clb0bh3zFSM)


## Course Notes

+ RNA-seq Pre-processing
+ Differential Expression
+ Gene Set Enrichment

