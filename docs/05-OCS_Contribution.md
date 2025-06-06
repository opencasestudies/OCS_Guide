


# New Case Studies - Building and Contributing 

## Learning Objectives

In this chapter we will discuss:
- Creating your own case study with our [template](https://github.com/opencasestudies/ocs-bp-template)
<!-- - Creating your own case study with our [app](https://rsconnect.biostat.jhsph.edu/MakeCaseStudies/) -->
- The guidelines for how to publish your own case studies as part of our project

## Create a Case Study

<!-- Open Case Studies offers two options for creating a case study. The first method is a template repository available on GitHub. The second is a new live web application. The first option offers more customization, while the second is much more fast and simple. These methods are free for all to use. If you'd like to create a case study to contribute to the Open Case Studies, using one of these methods is recommended, but not required. -->

### Template Case Study

A template case study is available in a repository on our GitHub page at [github.com/opencasestudies/ocs-bp-template](https://github.com/opencasestudies/ocs-bp-template). This template contains the basic skeletal structure used for our case studies. Creating a new case study with the template is very similar to modifying an existing case study:

1. Click on the "use this template" button at [opencasestudies/ocs-bp-template](https://github.com/opencasestudies/ocs-bp-template). 

2. Open the index.Rmd file in RStudio.

3. Add the case study content to the index.Rmd file. Use the instructions provided in this file to add different elements such as images and videos.

4. Save your changes and knit the case study to the preferred file format.

5. Distribute the knitted case study as you please!

All of these steps are demonstrated in the following video:



```
## `google-chrome`, `chromium-browser` and `chrome` were not found. Try setting the `CHROMOTE_CHROME` environment variable to the executable of a Chromium-based browser, such as Google Chrome, Chromium or Brave or adding one of these executables to your PATH.
```

<iframe src="https://www.youtube.com/embed/rP5E7GohTiI" width="100%" height="400px" data-external="1"></iframe>

<!-- ### MakeCaseStudies App -->

<!-- Open Case Studies now also offers the [MakeCaseStudies](https://rsconnect.biostat.jhsph.edu/MakeCaseStudies/) app as an option for our users to create their own case studies. The app has an easy-to-use interface where users can copy and paste their content into text boxes on the "Create" tab and check the "Preview" tab to see what they’ve made so far. Once satisfied, click the download button to export your finished case study! (This is currently being rehosted so the URL will not work!) -->

<!-- Watch the following video to learn more about creating case studies with the MakeCaseStudies app: -->

<!-- ```{r, fig.align="center", fig.alt = "video", echo=FALSE, out.width="100%"} -->
<!-- knitr::include_url("https://www.youtube.com/embed/Dd4KASCIsNc") -->
<!-- ``` -->

If you'd like to learn more about MakeCaseStudies, you can read this [thesis](https://jscholarship.library.jhu.edu/handle/1774.2/66820) by former graduate student [Michael Breshock](https://mbreshock.github.io/) @breshock_expanding_2021.

## Case Study Libraries

To help curate case studies for educators and learners, we would like to encourage others to help us expand our library of case studies. 


We recognize that other educators may have case studies in various stages of development that could be helpful to others.

We hope to facilitate sharing of these case studies on the Open Case Studies project.


However, we unfortunately do not have the resources or time to help integrate all case studies we receive into the official Open Case Studies library

For this reason, we have outlined the following two modes of submission: 


1) **Submissions for integration into the official library:** 

With this submission type, the Open Case Studies team will work with you starting from a case study idea through development and peer review stages, with the ultimate goal of adding your case study to the Open Case Studies project. Please note that we will only be able to accept one or two case studies a year to the official repository, as we are currently doing this as a passion project and have limited time to review and collaborate on the case studies. Please note that it is not required that case studies explore a public health topic, instead the just need to explore an interesting and timely problem. 

2) **Submissions for a publicly available community repository:** 

We hope to also create a more casual community library that allows others to share their work more easily and quickly. This repository will contain case studies submitted by educators but not included in the official Open Case Studies project library. The submission process is much simpler. 


Please note that case studies submitted to either collection need to be open source and with a license that permits sharing of derivatives to allow other educators to make use of our case studies as needed. 

The original others will retain the rights of their case studies, but need to provide citation information for others to attribute their case studies. For official case studies, the OCS team may help modify the case study and may therefore be included as authors. 

## Submission Process 

The process of submitting community case studies, involves filling out a simple form. The process of submitting to our official library involves ensuring that your case study meets our more lengthy requirements and a review process. Now we will describe the submission process for each library

### Community Library Submissions

These case studies will be shared publicly on the Open Case Studies Community Repository for the benefit of other educators and learners, with minimal review from the Open Case Studies team. To submit a case study to the Community Repository, please fill out the form below: 

**[Open Case Studies Community Repository Submission Form](https://forms.gle/BgkQMbb13wtaYHMo6)**

### Official Library Submissions

If you have not yet created a case study, but want to create one for our official library, please complete the form below to contact the Open Case Studies team regarding a new case study idea. The team will get back to do as soon as we can. 

**[Open Case Studies New Idea Offical Repository Submission Form](https://forms.gle/2EEYfnTJkNB7Nn9dA)**


Ultimately your case study will be submitted using an issue template to the GitHub repository for this guide, located at [this link](https://github.com/opencasestudies/OCS_Guide/issues/new?assignees=carriewright11%2Cstephaniehicks&labels=&template=new-official-case-study-submission.md&title=). The form indicates what is required for case studies to be considered for inclusion in our official collection, including peer review. We will now also describe some of these requirements in more depth in the next section.

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
  
![](resources/images/OCS_GitHub_Data_Directory_Diagram_Final.png){width=100%}
  
This diagram is from former graduate student [Michael Breshock's](https://mbreshock.github.io/) [thesis](https://jscholarship.library.jhu.edu/handle/1774.2/66820) on the Open Case Studies. In this thesis you can find a detailed description on the organization and structure of the case study data files @breshock_expanding_2021.

  - The data folder is required to have at least raw, imported, and wrangled data files. This allows users to skip sections when convenient. 

  - The raw data folder consists of data files as they came from the source. These are used at the beginning of the case study analysis at the Data Import section. 

  - Imported data is the version of the data after it has already been imported into R. These should be in the form of R Data files (extensions include .RData, .Rda, and .Rds). To create these files, use the `save()` function in R after importing the raw data. 

  - Wrangled data is the version of the data after it has been cleaned and is ready for analysis. Use the `save()` function in R after wrangling the data to create these files. This data should be provided in both RDA and CSV format. 
  
  - The next two data sub-folders are optional and used as needed: 
    - If the raw data files for your case study come in a format that requires a complicated data import process (such as web scraping) you may consider providing the raw data in an import friendly format such as CSV or XLS(X). Place these files in the "simpler_import" sub-folder.
    - If there are any raw data files from your source that are not used in the case study analysis, but could be analyzed in a similar fashion, please include these in the "extra" sub-folder. 


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
