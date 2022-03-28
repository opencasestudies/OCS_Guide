


# Modifying open case studies

## Learning Objectives

This chapter will cover how to modify the case studies to your own needs using the following methods:  

- Modular case study use with the help of the [`OCSdata` package](https://github.com/opencasestudies/OCSdata)
- Modifying a case study with [GitHub](https://github.com/opencasestudies) and [RStudio](https://www.rstudio.com/)
- Creating your own case study with our [template](https://github.com/opencasestudies/ocs-bp-template) and [MakeCaseStudies](https://rsconnect.biostat.jhsph.edu/MakeCaseStudies/)

## Modular use

Some educators may find that only certain sections of a case study are relevant to their specific needs. For example, a statistics teacher may want students to practice the skills covered in the data analysis section, but doesn't have time to go through the whole case study. The case studies are designed to allow for such use. This educator and their students may jump right in to any case study section without working through any previous sections. This is made possible because the data files are saved at the end of each section. These data files are made available on the case study's GitHub repository and may also be downloaded with the help of the `OCSdata` package. See Chapter 2 for more details on the structure and organization of a case study data folder. The table below explains which data sub-folder and package function to use for each case study section.

| Data Folder | Case Study Section | `OCSdata` Function |
| ----- | -------- | ------ |
| raw | Data Import | `raw_data` |
| imported | Data Exploration, Data Wrangling | `imported_data` |
| wrangled | Data Visualization, Data Analysis | `wrangled_csv`, `wrangled_rda` |
| simpler_import | Data Import | `simpler_import_data` |
| extra | Suggested Homework (?) | `extra_data` |

If you’d like to learn more about modular use of Open Case Studies you can read this [thesis](https://jscholarship.library.jhu.edu/handle/1774.2/66820) by former graduate student [Michael Breshock](https://mbreshock.github.io/) Breshock (2021).

### Example of Modular Use

The following steps illustrate how one would skip to a specific case study section. The data analysis section from the "Opioids in United States" case study is used for this example, but these directions apply for any section in any case study.

#### Steps for modular use

1) Use the table of contents to navigate to the section of interest. Click on the arrow that reads "If you skipped the previous sections click here."

{height: "400px", width: "100%", align: "middle", type: "video", poster: "http://img.youtube.com/vi/VOCYL-FNbr0/mqdefault.jpg",}
![Click on the lower right corner to expand the screen](https://www.youtube.com/watch?v=Z4WZ7A0OZF8)

2) Follow the instructions provided to download the data files from the previous section either with `OCSdata` or manually through GitHub. We will now demonstrate each option.

#### Downloading data with `OCSdata`:

1) First install and load the `OCSdata` package:
  

```r
install.packages("OCSdata") #only run once to install package
library(OCSdata) #run every new R session to load package
```

2) Now download the wrangled data into your R environment using the following function command:
  

```r
wrangled_rda("ocs-bp-opioid-rural-urban", outpath = getwd())
```
  
*This command will download the wrangled data in .RDA format. You may also be downloaded wrangled data in .CSV format by replacing 'wrangled_rda' with 'wrangled_csv'*

3) Load the RDA files with the following commands:


```r
load(file = here::here("OCS_data", "data", "wrangled", "Annual_opioid_data.rda"))
load(file = here::here("OCS_data", "data", "wrangled", "county_info.rda"))
```

#### Manually Download Data from GitHub:

 1) Download the .RDA files available on the case study GitHub repository from [here](https://github.com/opencasestudies/ocs-bp-opioid-rural-urban/tree/master/data/wrangled).

  *The CSV versions of the files may also be downloaded here, if preferred*

  2) Move the data files from your 'Downloads' folder to your R session's current working directory (you can see what this is with ```getwd()```).

 3) Load the RDA files with the following commands:
  

```r
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

{alt: "Screenshot of RStudio window with Knit button highlighted in red and drop down menu showing. Window also shows the Opioids case study repository with the index.Rmd file opened.", width: "100%", align: "middle",}
![](resources/images/rstudio_modify_knit_red.png)

5. Distribute your modified case study as you please! 

You can share HTML, PDF and Word files directly with your students or you can host your case study for free on GitHub using [GitHub pages](https://pages.github.com/) (“GitHub Pages Documentation” n.d.).

To do so, you will need to set up your version of the case study on GitHub. If you are new to GitHub, also be sure to check out Hester (n.d.).


These steps are demonstrated in the following video about modifying case studies:

{height: "400px", width: "100%", align: "middle", type: "video", poster: "http://img.youtube.com/vi/VOCYL-FNbr0/mqdefault.jpg",}
![Click on the lower right corner to expand the screen](https://www.youtube.com/watch?v=UFs4qvgTuTw)


## Create a case study

Open Case Studies offers two options for creating a case study. The first method is a template repository available on GitHub. The second is a new live web application. The first option offers more customization, while the second is much more fast and simple.

### Template Case Study

A template case study is available in a repository on our GitHub page at [github.com/opencasestudies/ocs-bp-template](https://github.com/opencasestudies/ocs-bp-template). This template contains the basic skeletal structure used for our case studies. Creating a new case study with the template is very similar to modifying an existing case study:

1. Click on the "use this template" button at [opencasestudies/ocs-bp-template](https://github.com/opencasestudies/ocs-bp-template). 

2. Open the index.Rmd file in RStudio.

3. Add the case study content to the index.Rmd file. Use the instructions provided in this file to add different elements such as images and videos.

4. Save your changes and knit the case study to the preferred file format.

5. Distribute the knitted case study as you please!

All of these steps are demonstrated in the following video:


{height: "400px", width: "100%", align: "middle", type: "video", poster: "http://img.youtube.com/vi/VOCYL-FNbr0/mqdefault.jpg",}
![Click on the lower right corner to expand the screen](https://www.youtube.com/watch?v=rP5E7GohTiI)

### MakeCaseStudies App

Open Case Studies now also offers the [MakeCaseStudies](https://rsconnect.biostat.jhsph.edu/MakeCaseStudies/) app as an option for our users to create their own case studies. The app has an easy-to-use interface where users can copy and paste their content into text boxes on the "Create" tab and check the "Preview" tab to see what they’ve made so far. Once satisfied, click the download button to export your finished case study!

Watch the following video to learn more about creating case studies with the MakeCaseStudies app:

{height: "400px", width: "100%", align: "middle", type: "video", poster: "http://img.youtube.com/vi/VOCYL-FNbr0/mqdefault.jpg",}
![Click on the lower right corner to expand the screen](https://www.youtube.com/watch?v=Dd4KASCIsNc)

If you’d like to learn more about MakeCaseStudies, you can read this [thesis](https://jscholarship.library.jhu.edu/handle/1774.2/66820) by former graduate student [Michael Breshock](https://mbreshock.github.io/) Breshock (2021).

## Session info


```
## R version 4.1.2 (2021-11-01)
## Platform: x86_64-apple-darwin17.0 (64-bit)
## Running under: macOS Mojave 10.14.6
## 
## Matrix products: default
## BLAS:   /Library/Frameworks/R.framework/Versions/4.1/Resources/lib/libRblas.0.dylib
## LAPACK: /Library/Frameworks/R.framework/Versions/4.1/Resources/lib/libRlapack.dylib
## 
## locale:
## [1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8
## 
## attached base packages:
## [1] stats     graphics  grDevices utils     datasets  methods   base     
## 
## loaded via a namespace (and not attached):
##  [1] rstudioapi_0.13 knitr_1.37      magrittr_2.0.2  hms_1.1.1      
##  [5] R6_2.5.1        rlang_1.0.2     fastmap_1.1.0   fansi_1.0.2    
##  [9] highr_0.9       stringr_1.4.0   tools_4.1.2     xfun_0.30      
## [13] utf8_1.2.2      cli_3.2.0       jquerylib_0.1.4 htmltools_0.5.2
## [17] ellipsis_0.3.2  ottrpal_1.0     digest_0.6.29   tibble_3.1.6   
## [21] lifecycle_1.0.1 crayon_1.5.0    bookdown_0.24   tzdb_0.2.0     
## [25] readr_2.1.2     sass_0.4.0      vctrs_0.3.8     fs_1.5.2       
## [29] glue_1.6.2      evaluate_0.15   rmarkdown_2.11  stringi_1.7.6  
## [33] bslib_0.3.1     compiler_4.1.2  pillar_1.7.0    jsonlite_1.8.0 
## [37] pkgconfig_2.0.3
```

## References
Breshock, Michael Robert. 2021. “EXPANDING ACCESS AND REMOVING BARRIERS: DATA SCIENCE EDUCATION WITH THE OPEN CASE STUDIES DIGITAL PLATFORM.” Thesis, Johns Hopkins University. <https://jscholarship.library.jhu.edu/handle/1774.2/66820>.


“GitHub Pages Documentation.” n.d. *GitHub Docs*. Accessed March 22, 2022. <https://docs.github.com/en/pages>.


Hester, Jim, the STAT 545 TAs. n.d. *Let’s Git Started Happy Git and GitHub for the <span class="nocase">useR</span>*. Accessed March 22, 2022. <https://happygitwithr.com/>.

