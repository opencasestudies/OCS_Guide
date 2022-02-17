


# New Case Studies - Building and Contributing 

In this chapter we will discuss the guidelines for creating new case studies as well as how to publish your own new case study as part of our project. To preserve the integrity of the core ideas of our resource we provide the following guidelines for case studies to be included in the Open Case Studies collection:

### Guidelines:

- **Programming language:** Case studies should be written in open source programming languages (preferably R). 
- **Data:**
  - Case studies should use data that is publicly available or can be made publicly available. Please ensure that you are allowed to make the data public if it is not already. 
  - Transparent descriptions of data sources and how data was generated should be included when possible. 
- **Core sections**: all case studies should include the following sections consistent with the published case studies. See Chapter 1, Case Study Anatomy for a detailed description on what each section should include:
  - Case study context 
  - Study motivation 
  - Main question 
  - Learning objectives 
  - Study limitations
  - Data description 
  - Import and exploration 
  - Wrangling 
  - Visualization 
  - Analysis
  - Analysis conclusions 
  - Case study summary 
  - Next steps 
  - Homework 
  - Additional information
- **Content:** Despite often being motivated by articles, case studies are not intended to demonstrate the methods of a paper - they are intended as an educational resource where users are guided through the data science process. 
  - Links to literature or other sources to motivate the scientific topic of the case study should be included where possible.
  - Case studies should aim to describe the decision making process involved in performing data science related tasks.
- **Attribution:** all outside resources used in the case study should be referenced appropriately. 
  - Case studies should include disclaimers and appropriate license agreements.
  - All included images (that are not original to the case study) should include relevant sources.

### Submission: 

- **Data:**
  - All data files should be saved in a folder named "data" within the project directory. All files should be contained in a sub-folder using the design scheme outlined in this diagram:
  <img src="resources/images/OCS_GitHub_Data_Directory_Diagram_Final.png" title="Diagram explaining the case study data folder structure and how data is categorized into different sub-folders" alt="Diagram explaining the case study data folder structure and how data is categorized into different sub-folders" style="display: block; margin: auto;" />
  - The data folder is required to have at least raw, imported, and wrangled data files. This allows users to skip sections when convenient. 
  - The raw data folder consists of data files as they came from the source. These are used at the beginning of the case study analysis at the Data Import section. 
  - Imported data is the version of the data after it has already been imported into R. These should be in the form of R Data files (extensions include .RData, .Rda, and .Rds). To create these files, use the `save()` function in R after importing the raw data. 
  - Wrangled data is the version of the data after it has been cleaned and is ready for analysis. Use the `save()` function in R after wrangling the data to create these files. This data should be provided in both RDA and CSV format. 
  - The next two data sub-folders are optional and used as needed: 
    - If the raw data files for your case study come in a format that requires a complicated data import process (such as web scraping) you may consider providing the raw data in an import friendly format such as CSV or XLS(X). Place these files in the "simpler_import" sub-folder.
    - If there are any raw data files from your source that are not used in the case study analysis, but could be analyzed in a similar fashion, please include these in the "extra" sub-folder. 



```r
sessionInfo()
```

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
##  [1] bookdown_0.24   digest_0.6.25   crayon_1.3.4    R6_2.4.1       
##  [5] lifecycle_1.0.0 magrittr_2.0.2  evaluate_0.14   highr_0.8      
##  [9] pillar_1.4.6    stringi_1.5.3   rlang_0.4.10    fs_1.5.0       
## [13] jquerylib_0.1.4 vctrs_0.3.4     ellipsis_0.3.1  rmarkdown_2.10 
## [17] tools_4.0.2     stringr_1.4.0   readr_1.4.0     hms_0.5.3      
## [21] yaml_2.2.1      xfun_0.26       compiler_4.0.2  pkgconfig_2.0.3
## [25] htmltools_0.5.0 ottrpal_0.1.2   knitr_1.33      tibble_3.0.3
```
