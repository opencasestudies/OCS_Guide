


# Use of Open Case Studies

## Learning Objectives

This chapter will provide guidance on how to use Open Case Studies in classroom settings for beginner, intermediate, and advanced students. Example uses will be discussed as well as suggestions for crafting homework assignments based on the case studies. 

### Experience Level Descriptions

In this chapter we will discuss how we envisioned case studies to be used in the classroom. We will give a coarse guide on which case studies include material appropriate for beginner, intermediate, or advanced learners. We will present some examples of assignments that can accompany the case studies and the rubrics that they can be evaluated with. Furthermore, we provide examples of extensions to case studies that can serve as a template for homework assignments or independent student exploration. 

The examples presented in this chapter are merely suggestions - modifications to the case studies to fit student needs are expected and encouraged! If you come up with a different way to use the case studies, please let us know what you come up with so that other educators may be inspired by your creativity. 

| Experience Level | Description |
| ---------------- | ----------- |
| Beginner         | Little to no previous experience with coding and/or statistical analysis. |
| Intermediate     | Familiar with at least one programming language and has experience working with data and statistics. |
| Advanced         | Fluent in at least one programming language and likely familiar with more. Has a depth of experience working with data science projects. |

Typically, most middle/high school and first year undergraduate students will fit in the beginner category. Upperclassmen undergraduates and some graduate students are often at the intermediate level. Most advanced level students will be at the graduate level. However, this is a generalization, and a student may be considered beginner, intermediate, or advanced at any academic level depending on their independent studies and experiences. 

## Open Case Studies in the Classroom

The case studies are structured to support both partial and full use of a case study. Educators are also free to use case study data by itself.  

### Teaching a Full Case Study

The case studies are written to provide a cohesive story that simulates data science in the real world. Reading through an entire case study is an excellent exercise for students to experience a standard data science workflow and learn the best practices of today from start to finish. The following list provides a few examples of how educators have used a full case study in the past: 

- Converted the case study into a slide deck (add link, source and example image of slide)
- Assigned students to read the case study and write a report as homework
- Suggested reading and supplemental material 
- more? 

### Teaching Part of a Case Study

Some educators may find that only certain sections of a case study are relevant to their course learning objectives. For these educators the case studies are structured to allow for modular use. The case study ![GitHub repositories](https://github.com/opencasestudies) provide the appropriate data files to be used at the start of each section. These data files can be downloaded directly from GitHub or with the ![OCSdata](https://github.com/opencasestudies/OCSdata) package (see chapter 2.5). The following table describes which data folder contains the corresponding data for each case study section. An example use for each data type is provided as well. 

| Data Folder | Case Study Section | Example Use |
| ----------- | ------------------ | ----------- |
| raw | Data Import | Assigning public health students to read through a case study starting from the beginning |
| imported | Data Exploration, Data Wrangling | Data science students practicing wrangling methods with in class exercises |
| wrangled | Data Visualization, Data Analysis | Statistics course practicing analysis methods with real data as a live lesson |
| simpler_import | Data Import | Introductory data science instructor wants students to practice data import without over-complication |
| extra | Not Used in Case Study | Public health course assigns homework to practice case study methods with similar but new data | 

*MB: Should we highlight the interactive case studies here as well?*

### Teaching With Case Study Data Only

- Data available on GitHub
- Can use OCSdata package for streamlined data retrieval process
- Suggestions on how to use data?
- Look at case studies for exercise ideas
- more?

## Case Study Recommendations

The following table lists a few example case studies that would be suitable for each experience level. 

| Experience Level | Case Studies |
| ---------------- | ------------ |
| Beginner         | ![Exploring CO2 emissions across time](https://www.opencasestudies.org/ocs-bp-co2-emissions/), ![Vaping Behaviors in American Youth](https://www.opencasestudies.org/ocs-bp-vaping-case-study/) |
| Intermediate     | ![Mental Health of American Youth](https://www.opencasestudies.org/ocs-bp-youth-mental-health/), ![Opioids in United States](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban/) |
| Advanced         | ![Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 1](https://www.opencasestudies.org/ocs-bp-RTC-wrangling/), ![Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 2](https://www.opencasestudies.org/ocs-bp-RTC-analysis/) |


## Examples


## Homework Assignments



=======
## Examples of assignments 

In addition to helping students develop data analysis skills, we hope that the case studies can also help students develop their technical writing and communication skills. This includes but is not limited to data visualization and presentation, written reports, and oral presentations. 

### Data visualization

The data visualizations included in the case studies are not the only way to present the results of the analyses. Below is an example of an assignment to guide students in exploring different ways of visualizing the same results.

(avocado data visualization assignment guide, example, rubric)

### Written report 

Below is an example of a scientific-style paper written based on the [Opioid Use Case Study](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban/#Main_Question). We also include an example rubric by which this paper can be evaluated adapted from [here](https://ocw.mit.edu/courses/biological-engineering/20-109-laboratory-fundamentals-in-biological-engineering-spring-2010/assignments/guidelines-for-writing-up-your-research/#Evaluation). 

(avocado report assignment guide)
[OCS Opioid Use in the US Example Report](https://raw.githubusercontent.com/opencasestudies/OCS_Guide/main/assets/OCS_Opioids_Example_Report.pdf)
[OCS Opioid Use in the US Example Report Rubric](https://raw.githubusercontent.com/opencasestudies/OCS_Guide/main/assets/OCS_Opioids_Example_Report_Rubric.pdf)


### Oral presentation 

Below is an example of a presentation based on the [Vaping Behaviors in American Youth Case Study](https://www.opencasestudies.org/ocs-bp-vaping-case-study/). This presentation focuses on the context of the study and the methods used in the analysis. Assignments for presentations can be modified to emphasize presenting results and conclusions or to emphasize communication to different audiences (e.g. policy makers, other researchers, the public, etc. ).  

(avocado insert presentation assignment guide, example, and grading rubric)





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
##  [5] lifecycle_1.0.0 magrittr_1.5    evaluate_0.14   pillar_1.4.6   
##  [9] leanbuild_0.1.2 stringi_1.5.3   rlang_0.4.10    fs_1.5.0       
## [13] jquerylib_0.1.1 vctrs_0.3.4     ellipsis_0.3.1  rmarkdown_2.10 
## [17] tools_4.0.2     stringr_1.4.0   readr_1.4.0     hms_0.5.3      
## [21] yaml_2.2.1      xfun_0.26       compiler_4.0.2  pkgconfig_2.0.3
## [25] htmltools_0.5.0 knitr_1.33      tibble_3.0.3
```

