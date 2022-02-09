


# Open Case Study Infrastructure

## Learning Objectives

In this chapter we will discuss the overall infrastructure of the Open Case Studies platform, which includes:

- our website
- an Open Case Studies search tool
- our GitHub organization
- an R package called OCSdata


## OCS Website 

### Open Case Studies mission 

The [Open Case Studies website](https://www.opencasestudies.org/) describes the mission of the Open Case Studies project, the history of its inception, and current and previous members of the OCS team, among other information. 

### Open Case Studies feedback 

The website also includes a link to a [user experience survey](https://www.opencasestudies.org/) (takes up to 10 minutes to complete), which helps us learn more about how to improve the data science education experience. Part of this includes getting a better understanding of who is using our case studies and how so that we can better design our case studies. We would greatly appreciate you filling it out  if you have the time! 

### Open Case Studies search tool 

Finally, the website includes the OCS case study search tool to aid instructors in finding appropriate case studies for their learning objectives. The search tool is described in more detail below. 

## OCS Case Study Search Tool 

A brief description of the subject areas of each case study is included at the [Bloomberg American Health Initiative website](https://americanhealth.jhu.edu/open-case-studies).

To aid with case study selection, we created the [OCS case study search tool](https://www.opencasestudies.org/#searchtab). This search tool is designed to aid instructors in identifying appropriate case studies for their learning objectives. The tool consists of a table with searchable columns, where each row is an individual case study. 

The main two columns likely to be helpful in identifying appropriate case studies are the **"Packages"** and **"Objectives"** columns. The **Packages** column details all the R packages used in the case study, and can help identify if a case study teaches a specific data import, wrangling, analysis, or visualization skill. The **Objectives** column details the learning objectives of each case study (e.g. importing data from PDF files, reshaping data, specific statistical analysis, etc.).

The table also includes links to both the static and interactive versions of the case studies and their GitHub repositories. Below is an example of the information included in the search tool results for the case study on [School Shootings in the United States](https://www.opencasestudies.org/ocs-bp-school-shootings-dashboard/).

![](assets/search_tool_example.png)

## GitHub Organization 

The GitHub repository contains all the materials needed for the case study. This includes the case study text to be distributed to students, the data used in the case study (discussed below), additional documents and references, and brief guidelines on case study use. 

Data included in the GitHub repository is available in multiple formats to facilitate modularization of the case studies as described below. To use the case study data, you can download the GitHub repository directly or use the OCSdata R package described below. 

(avocado Add figure 2.4 outlining repo structure)

## OCSdata 
To simplify the process of accessing the data required for each case study, we have created the OCSdata R package. Briefly, the OCSdata package creates a new folder called "OCSdata" where it downloads the data needed for a specific case study. Users can download the data in its original raw format or in various processed formats that correspond to different stages of data wrangling and cleaning. This allows users to perform the data exploration and wrangling or the data visualization and analysis sections of the case study without having to process the data from the raw files. For some of the case studies, the OCSdata package also downloads extra source data that is not used in the case study. 

(Add table 2.1 summarizing data formats available for download via OCSdata)

### Getting Started with OCSdata

The `OCSdata` package is available on the package repository CRAN and can be installed in R as follows: 

[avocado R version requirement?]


```r
install.packages("OCSdata") #only run once to install package
library(OCSdata) #run every new R session to load package
```

### Downloading raw data
The `raw_data` function will download the raw data files that can be imported into R. 

The first argument is the name of the case study. A list of case study names can be found in the package documentation [online](https://cran.r-project.org/web/packages/OCSdata/vignettes/instructions.html#casestudy) or by typing `?raw_data` in R. 

The `outpath` argument is a string specifying the folder where the data should be downloaded. To download the data to a folder named "OCS_data" in the current working directory, you can supply `getwd()` to the `output` argument. If nothing is provided for the argument, you will be prompted to enter 1, 2, or 3 to download the data into the current director, to specify the download path, or to cancel, respectively. 

In the following example, we download the raw data for the "Opioids in the United States" case study to the current directory. 


```r
raw_data("ocs-bp-opioid-rural-urban", outpath = getwd())
```

### Downloading data in other formats
The OCSdata package can be used to download the data in various processed formats that may be helpful in skipping certain case study sections and focusing on data wrangling and/or analysis and visualization. All of the functions take the same arguments described above.

#### Simpler import
The `simpler_import_data` function will download raw data files that have been converted to file formats that are easier to import into R, typically .csv. Some case studies offer this option when the original raw files require a more complicated import step. 


```r
simpler_import_data("ocs-bp-opioid-rural-urban", outpath = getwd())
```

#### Importing data as R objects 
The imported_data function will download raw data files in .rda format. This means the data have already been imported into R objects. This can be used to skip the data import section and start directly with data wrangling. The R objects files can be imported into R by either double clicking on the files in RStudio or using the load() function as follows. 



```r
imported_data("ocs-bp-opioid-rural-urban", outpath = getwd()) #download data in .rda format 
file_path = "~/OCS_data/data/imported/land_area.rda" #specify download directory 
load(file_path) #load R objects 
```

#### Importing wrangled data
The following functions will download the data files that have already been wrangled and are ready to be analyzed. These come in both .csv and .rda formats.

Download as csv files:

```r
wrangled_csv("ocs-bp-opioid-rural-urban", outpath = getwd()) 
```

Downloading as R objects:

```r
wrangled_rda("ocs-bp-opioid-rural-urban", outpath = getwd()) 
```

### Downloading extra data
Some case studies have extra data are not used in the case study but can be used to explore the case study subject from different perspectives. These data  but can This data can be downloaded using the `extra_data` function. 


```r
extra_data("ocs-bp-opioid-rural-urban", outpath = getwd()) 
```

### Downloading all case study data
The `zip_ocs` function will download the all of the repository files in a .zip folder and unzip them into a specified directory. This includes the case study data in all the formats detailed above (raw, simpler_import, imported, wrangled, and extra). It also includes the case study .Rmd file, which can be modified by instructors as needed. 


```r
zip_ocs("ocs-bp-opioid-rural-urban", outpath = getwd()) 
```

### Forking the case study repository



```
## R version 4.0.2 (2020-06-22)
## Platform: x86_64-pc-linux-gnu (64-bit)
## Running under: Ubuntu 20.04.3 LTS
## 
## Matrix products: default
## BLAS/LAPACK: /usr/lib/x86_64-linux-gnu/openblas-pthread/libopenblasp-r0.3.8.so
## 
## locale:
##  [1] LC_CTYPE=en_US.UTF-8       LC_NUMERIC=C              
##  [3] LC_TIME=en_US.UTF-8        LC_COLLATE=en_US.UTF-8    
##  [5] LC_MONETARY=en_US.UTF-8    LC_MESSAGES=C             
##  [7] LC_PAPER=en_US.UTF-8       LC_NAME=C                 
##  [9] LC_ADDRESS=C               LC_TELEPHONE=C            
## [11] LC_MEASUREMENT=en_US.UTF-8 LC_IDENTIFICATION=C       
## 
## attached base packages:
## [1] stats     graphics  grDevices utils     datasets  methods   base     
## 
## loaded via a namespace (and not attached):
##  [1] bookdown_0.24   crayon_1.4.2    digest_0.6.25   R6_2.5.1       
##  [5] lifecycle_1.0.1 magrittr_2.0.2  evaluate_0.14   pillar_1.4.6   
##  [9] rlang_0.4.10    stringi_1.5.3   fs_1.5.2        ellipsis_0.3.1 
## [13] vctrs_0.3.4     rmarkdown_2.10  ottr_0.1.2      tools_4.0.2    
## [17] stringr_1.4.0   readr_1.4.0     hms_0.5.3       xfun_0.26      
## [21] yaml_2.2.2      compiler_4.0.2  pkgconfig_2.0.3 htmltools_0.5.0
## [25] knitr_1.33      tibble_3.0.3
```
