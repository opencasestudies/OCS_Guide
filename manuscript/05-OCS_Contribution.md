


# New Case Studies - Building and Contributing 

## Learning Objectives

In this chapter we will discuss:
- Our two case study submission options
- The guidelines for  how to publish your own case studies as part of our project

## Case Study Libraries

To help curate case studies for educators and learners, we would like to encourage others to help us expand our library of case studies. 



We recognize that other educators may have case studies in various stages of development that could be helpful to others.

We hope to facilitate sharing of these case studies on the Open Case Studies project.


However, we unfortunately do not have the resources or time to help integrate all case studies we receive into the official Open Case Studies library

For this reason, we have outlined the following two modes of submission: 


1) **Submissions for integration into the official library:** 

With this submission type, the Open Case Studies team will work with you starting from a case study idea through development and peer review stages, with the ultimate goal of adding your case study to the Open Case Studies project. 

2) **Submissions for a publicly available community repository:** 

We hope to also create a more casual community library that allows others to share their work more easily and quickly. This repository will contain case studies submitted by educators but not included in the official Open Case Studies project library. The submission process is much simpler. 

## Submission Process 

The process of submitting community case studies, involves filling out a simple form. The process of submitting to our official library involves ensuring that your case study meets our more lengthy requirements and a review process. Now we will describe the submission process for each library

### Community Library Submissions

These case studies will be shared publicly on the Open Case Studies Community Repository for the benefit of other educators and learners, with minimal review from the Open Case Studies team. To submit a case study to the Community Repository, please fill out the form below: 

**[OpenCaseStudies Community Repository Submission Form](https://forms.gle/BgkQMbb13wtaYHMo6)**

### Official Library Submissions

If you have not yet created a case study, but want to create one for our official library, please complete the form below to contact the Open Case Studies team regarding a new case study idea. The team will get back to do as soon as we can. 

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

Ultimately your case study will be submitted using an issue template to the GitHub repository for this guide, located at [this link](https://github.com/opencasestudies/OCS_Guide/issues/new?assignees=carriewright11%2Cstephaniehicks&labels=&template=new-official-case-study-submission.md&title=).

## Offical Case Study Guidelines

To ensure that the submitted case studies provide the most benefit to the community, we hope that they adhere as much as possible to the core structure and ideas of the Open Case Studies project. We provide the guidelines detailed below for submission to the official library. Furthermore, because the Open Case Studies team does not have the infrastructure to perform a full content review of submitted case studies, we ask that you find at least two independent reviewers to comment about the validity of the content and conclusions presented in your case study. 


**Programming language:** Case studies should be written in open source programming languages (such as R or python). 


**Data:**

  - Case studies should use data that is publicly available or can be made publicly available. Please ensure that you are allowed to make the data public if it is not already. 


  - Transparent descriptions of data sources and how data was generated should be included when possible. 


**Core sections**: all case studies should include the following sections consistent with the published case studies. See [Chapter 1, Case Study Anatomy](https://www.opencasestudies.org/OCS_Guide/introduction.html#open-case-studies-anatomy) for a detailed description on what each section should include:

  - **Getting Started:** *Case study context, Study motivation, Main question, Learning objectives, Study limitations.* This section will outline previous literature and overarching questions in the field that make this case study question important, providing motivation for conducting the analysis in the case study. It will specify the exact question that the case study endeavors to address as well as the defining the statistical and data analysis learning objectives for the case study. It will also discuss the limitations of the investigation that may prevent the analysis from answering the main question of interest. 


  - **Analyzing the Data:** *Data description, Import and exploration, Wrangling, Visualization, Analysis.* This section includes the bulk of the data analysis, beginning with a detailed description of the data used in the case study, how it was generated, and where it was obtained. Then it walks through, step-by-step, the data import, exploration, wrangling, procedures. Finally, it demonstrates the visualization and statistical analysis steps used to address the case study question. 


  - **Wrapping-up:** *Analysis conclusions, Case study summary, Next steps, Homework, Additional information.* This section synthesized conclusions to the main study question based on the data analysis results demonstrated in the previous sections. It summarizes the analysis steps and potential next steps for further exploration, which can be suggested as homework. If applicable, additional information relevant to further study can be provided here. 


**Content:** Despite often being motivated by articles, case studies are not intended to demonstrate the methods of a paper - they are intended as an educational resource where users are guided through the data science process. 

  - Links to literature or other sources to motivate the scientific topic of the case study should be included where possible.

  - Case studies should aim to describe the decision making process involved in performing data science related tasks.


**Attribution:** all outside resources used in the case study should be referenced appropriately. 

  - Case studies should include disclaimers and appropriate license agreements.

  - All included images (that are not original to the case study) should include relevant sources.

**Data:**

  - All data files should be saved in a folder named "data" within the project directory. All files should be contained in a sub-folder using the design scheme outlined in this diagram:
  
{alt: "Diagram explaining the case study data folder structure and how data is categorized into different sub-folders", width: "100%", align: "middle",}
![](resources/images/OCS_GitHub_Data_Directory_Diagram_Final.png)
  
This diagram is from former graduate student [Michael Breshock’s](https://mbreshock.github.io/) [thesis](https://jscholarship.library.jhu.edu/handle/1774.2/66820) on the Open Case Studies. In this thesis you can find a detailed description on the organization and structure of the case study data files Breshock (2021).

  - The data folder is required to have at least raw, imported, and wrangled data files. This allows users to skip sections when convenient. 

  - The raw data folder consists of data files as they came from the source. These are used at the beginning of the case study analysis at the Data Import section. 

  - Imported data is the version of the data after it has already been imported into R. These should be in the form of R Data files (extensions include .RData, .Rda, and .Rds). To create these files, use the `save()` function in R after importing the raw data. 

  - Wrangled data is the version of the data after it has been cleaned and is ready for analysis. Use the `save()` function in R after wrangling the data to create these files. This data should be provided in both RDA and CSV format. 
  
  - The next two data sub-folders are optional and used as needed: 
    - If the raw data files for your case study come in a format that requires a complicated data import process (such as web scraping) you may consider providing the raw data in an import friendly format such as CSV or XLS(X). Place these files in the "simpler_import" sub-folder.
    - If there are any raw data files from your source that are not used in the case study analysis, but could be analyzed in a similar fashion, please include these in the "extra" sub-folder. 


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

