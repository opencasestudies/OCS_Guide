

# New Case Studies - Building and Contributing 

In this chapter we will discuss the guidelines for creating new case studies as well as how to publish your own new case study as part of our project. We recognize that educators may have case studies in various stages of development. We hope to facilitate sharing of these case studies on the Open Case Studies project to fullest extent possible. However, we may not be able to integrate all case studies we receive into the Open Case Studies. For this reason, we have outlined the following two modes of submission: 

1) **Submitting case studies for integration into the Open Case Studies project:** Here, the Open Case Studies team will work with you starting from a case study idea through development, testing, and peer review stages, with the ultimate goal of adding your case study to the Open Case Studies project. See details in the Submission section below on how to initiate this process.    
2) **Submitting case studies and/or case study materials for sharing on our publicly available community repository:** Here, you can submit your case study materials (data, code, content explanations) to the Open Case Studies community repository. This repository will contain case studies submitted by educators but not included in the Open Case Studies project. See details in the Submission section below on how to submit. 

## Submission: 

### Submitting case study materials to the Open Case Studies community repository

These case studies will be shared publicly on the Open Case Studies Community Repository for the benefit of other educators and learners, with minimal review from the Open Case Studies team. To submit a case study to the Community Repository, please fill out the form below. 

(avocado google form)

### Submitting case study idea for integration into the Open Case Studies project

Please complete the form below to contact the Open Case Studies team regarding a new case study idea. The team will get back to do as soon as possible. 

<form
  action="https://formspree.io/f/myybqzpz"
  method="POST"
>
  <label>
    Name: <br>
    <input type="text" name="_replyto"><br>
  </label>
  <label>
    Email:  <br>
    <input type="text" name="_replyto"><br>
  </label>
  <label>
    Case study title (tentative): <br>
    <textarea rows = "5" cols = "60" name="message"></textarea><br>
  </label>
  <label>
    Case study description: <br>
    <textarea rows = "5" cols = "60" name="message"></textarea><br>
  </label>
  <label>
    Dataset description: <br>
    <textarea rows = "5" cols = "60" name="message"></textarea><br>
  </label>
  <label>
    Statistics learning goals for the case study: <br>
    <textarea rows = "5" cols = "60" name="message"></textarea><br>
  </label>
  <label>
    Data science learning goals for the case study: <br>
    <textarea rows = "5" cols = "60" name="message"></textarea><br>
  </label>
  <!-- your other form fields go here -->
  <button type="submit">Send</button>
</form>



## Guidelines:

To ensure that the submitted case studies provide the most benefit to the community, we hope that they adhere as much as possible to the core structure and ideas of the Open Case Studies project. We provide the guidelines detailed below for submission to the Community Repository. Furthermore, because the Open Case Studies team does not have the infrastructure to perform a full content review of submitted case studies, we ask that you provide brief comments from at least two independent reviewers supporting the validity of the content and conclusions presented in your case study. 


**Programming language:** Case studies should be written in open source programming languages (such as R or python). 


**Data:**
  - Case studies should use data that is publicly available or can be made publicly available. Please ensure that you are allowed to make the data public if it is not already. 
  - Transparent descriptions of data sources and how data was generated should be included when possible. 


**Core sections**: all case studies should include the following sections consistent with the published case studies. See [Chapter 1, Case Study Anatomy](https://www.opencasestudies.org/OCS_Guide/introduction.html#open-case-studies-anatomy) for a detailed description on what each section should include:

  - **Getting Started:** *Case study context, Study motivation, Main question, Learning objectives, Study limitations.* This section will outline previous literature and overarching questions in the field that make this case study question important, providing motivation for conducting the analysis in the case study. It will specify the exact question that the case study endeavors to address as well as the definining the statistical and data analysis learning objectives for the case study. It will also discuss the limitations of the investigation that may prevent the analysis from answering the main question of interest. 


  - **Analyzing the Data:** *Data description, Import and exploration, Wrangling, Visualization, Analysis.* This section includes the bulk of the data analysis, beginning with a detailed description of the data used in the case study, how it was generated, and where it was obtained. Then it walks through, step-by-step, the data import, exploration, wrangling, procedures. Finally, it demonstrates the visualization and statistical analysis steps used to address the case study question. 


  - **Wrapping-up:** *Analysis conclusions, Case study summary, Next steps, Homework, Additional information.* This section synthesized conclusions to the main study question based on the data analysis results demonstrated in the previous sections. It summarizes the analysis steps and potential next steps for further exploration, which can be suggseted as homework. If applicable, additional information relevant to further study can be provided here. 


**Content:** Despite often being motivated by articles, case studies are not intended to demonstrate the methods of a paper - they are intended as an educational resource where users are guided through the data science process. 
  - Links to literature or other sources to motivate the scientific topic of the case study should be included where possible.
  - Case studies should aim to describe the decision making process involved in performing data science related tasks.


**Attribution:** all outside resources used in the case study should be referenced appropriately. 
  - Case studies should include disclaimers and appropriate license agreements.
  - All included images (that are not original to the case study) should include relevant sources.

**Data:**
  - All data files should be saved in a folder named "data" within the project directory. All files should be contained in a sub-folder using the design scheme outlined in this diagram:
  ![](resources/images/OCS_GitHub_Data_Directory_Diagram_Final.png)
  - The data folder is required to have at least raw, imported, and wrangled data files. This allows users to skip sections when convenient. 
  - The raw data folder consists of data files as they came from the source. These are used at the beginning of the case study analysis at the Data Import section. 
  - Imported data is the version of the data after it has already been imported into R. These should be in the form of R Data files (extensions include .RData, .Rda, and .Rds). To create these files, use the `save()` function in R after importing the raw data. 
  - Wrangled data is the version of the data after it has been cleaned and is ready for analysis. Use the `save()` function in R after wrangling the data to create these files. This data should be provided in both RDA and CSV format. 
  - The next two data sub-folders are optional and used as needed: 
    - If the raw data files for your case study come in a format that requires a complicated data import process (such as web scraping) you may consider providing the raw data in an import friendly format such as CSV or XLS(X). Place these files in the "simpler_import" sub-folder.
    - If there are any raw data files from your source that are not used in the case study analysis, but could be analyzed in a similar fashion, please include these in the "extra" sub-folder. 


## Session info


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
##  [1] bookdown_0.24   crayon_1.3.4    digest_0.6.25   R6_2.4.1       
##  [5] lifecycle_1.0.0 magrittr_2.0.2  evaluate_0.14   pillar_1.4.6   
##  [9] rlang_0.4.10    stringi_1.5.3   fs_1.5.0        ellipsis_0.3.1 
## [13] vctrs_0.3.4     rmarkdown_2.10  tools_4.0.2     stringr_1.4.0  
## [17] readr_1.4.0     hms_0.5.3       xfun_0.26       yaml_2.2.1     
## [21] compiler_4.0.2  pkgconfig_2.0.3 htmltools_0.5.0 ottrpal_0.1.2  
## [25] knitr_1.33      tibble_3.0.3
```
