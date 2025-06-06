


# Modifying open case studies

## Learning Objectives

This chapter will cover how to modify the case studies to your own needs using the following methods:  

- Modular case study use with the help of the [`OCSdata` package](https://github.com/opencasestudies/OCSdata)
- Modifying a case study with [GitHub](https://github.com/opencasestudies) and [RStudio](https://www.rstudio.com/)

## Modular use

Some educators may find that only certain sections of a case study are relevant to their specific needs. For example, a statistics teacher may want students to practice the skills covered in the data analysis section, but doesn't have time to go through the whole case study. The case studies are designed to allow for such use. This educator and their students may jump right in to any case study section without working through any previous sections. This is made possible because the data files are saved at the end of each section. These data files are made available on the case study's GitHub repository and may also be downloaded with the help of the `OCSdata` package. See Chapter 2 for more details on the structure and organization of a case study data folder. The table below explains which data sub-folder and package function to use for each case study section.

| Data Folder | Case Study Section | `OCSdata` Function |
| ----- | -------- | ------ |
| raw | Data Import | `raw_data` |
| imported | Data Exploration, Data Wrangling | `imported_data` |
| wrangled | Data Visualization, Data Analysis | `wrangled_csv`, `wrangled_rda` |
| simpler_import | Data Import | `simpler_import_data` |
| extra | Suggested Homework (?) | `extra_data` |

If you'd like to learn more about modular use of Open Case Studies you can read this [thesis](https://jscholarship.library.jhu.edu/handle/1774.2/66820) by former graduate student [Michael Breshock](https://mbreshock.github.io/) @breshock_expanding_2021.

### Example of Modular Use

The following steps illustrate how one would skip to a specific case study section. The data analysis section from the "Opioids in United States" case study is used for this example, but these directions apply for any section in any case study.

#### Steps for modular use

1) Use the table of contents to navigate to the section of interest. Click on the arrow that reads "If you skipped the previous sections click here."


```
## `google-chrome`, `chromium-browser` and `chrome` were not found. Try setting the `CHROMOTE_CHROME` environment variable to the executable of a Chromium-based browser, such as Google Chrome, Chromium or Brave or adding one of these executables to your PATH.
```

<iframe src="https://www.youtube.com/embed/Z4WZ7A0OZF8" width="100%" height="400px" data-external="1"></iframe>

2) Follow the instructions provided to download the data files from the previous section either with `OCSdata` or manually through GitHub. We will now demonstrate each option.

#### Downloading data with `OCSdata`:

1) First install and load the `OCSdata` package:
  

``` r
install.packages("OCSdata") #only run once to install package
library(OCSdata) #run every new R session to load package
```

2) Now download the wrangled data into your R environment using the following function command:
  

``` r
wrangled_rda("ocs-bp-opioid-rural-urban", outpath = getwd())
```
  
*This command will download the wrangled data in .RDA format. You may also be downloaded wrangled data in .CSV format by replacing 'wrangled_rda' with 'wrangled_csv'*

3) Load the RDA files with the following commands:


``` r
load(file = here::here("OCS_data", "data", "wrangled", "Annual_opioid_data.rda"))
load(file = here::here("OCS_data", "data", "wrangled", "county_info.rda"))
```

#### Manually Download Data from GitHub:

 1) Download the .RDA files available on the case study GitHub repository from [here](https://github.com/opencasestudies/ocs-bp-opioid-rural-urban/tree/master/data/wrangled).

  *The CSV versions of the files may also be downloaded here, if preferred*

  2) Move the data files from your 'Downloads' folder to your R session's current working directory (you can see what this is with ```getwd()```).

 3) Load the RDA files with the following commands:
  

``` r
load(file = here::here("Annual_opioid_data.rda"))
load(file = here::here("county_info.rda"))
```

3) All the data you need to work through the current section is now loaded into your environment. You are ready to work through the section of interest, without needing to work through any of the previous sections.

## Modify a case study

The case studies are written in [R Markdown](https://rmarkdown.rstudio.com/) documents and developed within an RStudio project. R Markdown documents are denoted with the file extension ".Rmd" and allow for the inclusion of code chunks and outputs in a written report. They are written using [Markdown syntax](https://raw.githubusercontent.com/rstudio/cheatsheets/main/rmarkdown.pdf). RStudio projects are used to organize the case studies. The [knitr](https://yihui.org/knitr/) package "knits" the case study written in R Markdown and outputs the document as an HTML file. Open Case Studies uses these HTML files to post the case studies online. The entire case study project is contained in a GitHub repository which allows for easy distribution and version control. [GitHub Pages](https://pages.github.com/) is used to host the case study webpage from the case study repository.

Modifying a case study requires the following simple steps:

1. Use the `OCSdata` package `zip_ocs()` function to download the case study files without our git history. Alternatively, if you are familiar with GitHub and wish to you can clone or fork the case study repository from GitHub. See [this section](https://www.opencasestudies.org/OCS_Guide/open-case-study-infrastructure.html#fork-or-clone-the-case-study-repository) of chapter 2 for more information.

2. In the repository folder, open the case study .Rproj file to open the project up in RStudio.

3. Edit the sections to be modified in the index.Rmd file.

4. Save your changes, then click on the "Knit" drop down menu in the top left corner of RStudio. Choose which file format you'd like to knit to.

![](resources/images/rstudio_modify_knit_red.png){width=100%}

5. Distribute your modified case study as you please! 

You can share HTML, PDF and Word files directly with your students or you can host your case study for free on GitHub using [GitHub pages](https://pages.github.com/) [@pages_github]. 

To do so, you will need to set up your version of the case study on GitHub. If you  are new to GitHub, also be sure to check out @happygitwithr.


These steps are demonstrated in the following video about modifying case studies:

<iframe src="https://www.youtube.com/embed/UFs4qvgTuTw" width="100%" height="400px" data-external="1"></iframe>

## Session info


```
## R version 4.3.2 (2023-10-31)
## Platform: x86_64-pc-linux-gnu (64-bit)
## Running under: Ubuntu 22.04.4 LTS
## 
## Matrix products: default
## BLAS:   /usr/lib/x86_64-linux-gnu/openblas-pthread/libblas.so.3 
## LAPACK: /usr/lib/x86_64-linux-gnu/openblas-pthread/libopenblasp-r0.3.20.so;  LAPACK version 3.10.0
## 
## locale:
##  [1] LC_CTYPE=en_US.UTF-8       LC_NUMERIC=C              
##  [3] LC_TIME=en_US.UTF-8        LC_COLLATE=en_US.UTF-8    
##  [5] LC_MONETARY=en_US.UTF-8    LC_MESSAGES=en_US.UTF-8   
##  [7] LC_PAPER=en_US.UTF-8       LC_NAME=C                 
##  [9] LC_ADDRESS=C               LC_TELEPHONE=C            
## [11] LC_MEASUREMENT=en_US.UTF-8 LC_IDENTIFICATION=C       
## 
## time zone: Etc/UTC
## tzcode source: system (glibc)
## 
## attached base packages:
## [1] stats     graphics  grDevices utils     datasets  methods   base     
## 
## loaded via a namespace (and not attached):
##  [1] digest_0.6.34   R6_2.5.1        later_1.3.2     bookdown_0.41  
##  [5] fastmap_1.1.1   xfun_0.48       websocket_1.4.2 magrittr_2.0.3 
##  [9] knitr_1.48      htmltools_0.5.7 rmarkdown_2.25  ps_1.7.6       
## [13] promises_1.2.1  cli_3.6.2       processx_3.8.3  webshot2_0.1.1 
## [17] chromote_0.3.1  compiler_4.3.2  highr_0.11      tools_4.3.2    
## [21] evaluate_0.23   Rcpp_1.0.12     yaml_2.3.8      jsonlite_1.8.8 
## [25] rlang_1.1.4
```
