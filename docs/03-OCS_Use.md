


# Use of Open Case Studies

## Learning Objectives


This chapter will provide guidance on how to use Open Case Studies in classroom settings. We will give a coarse guide on which case studies include material appropriate for beginner, intermediate, or advanced learners. We will present some examples of assignments that can accompany the case studies and the rubrics that they can be evaluated with. Furthermore, we provide examples of extensions to case studies that can serve as a template for homework assignments or independent student exploration. 

The examples presented in this chapter are merely suggestions - modifications to the case studies to fit student needs are expected and encouraged! If you come up with a different way to use the case studies, please let us know what you come up with so that other educators may be inspired by your creativity. 

### Prerequisites


**Public Health Subject Matter**  
 
The case studies in Open Case Studies generally deal with topics in public health. We do not require any prior knowledge on the public health subjects examined in the case studies. The Getting Started section in each case study (specifically, the case study context) will present the subject material relevant to understanding the data and the case study implications. 

**Statistics**  

The case studies cover a range of statistical approaches and skillsets. Some case studies will build on more foundational statistical concepts. The Experience Level categorization for each case study (see Section 3.3) will indicate the expected prior skills that the case study will expect. Furthermore, the exact skills that the case study will use are listed in the Case Study Search Tool under the Objectives column. 

**Coding/Data Science**  

All case studies use the R statistical programming language for data analysis. Some familiarity with R basics is expected for effective use of the case studies. However, depending on the data used and the extent to which it needs to be cleaned and processed before analysis, each case study may require experience with additional programming and data wrangling skills. This will be indicated by the Experience Level designation for the case study (see Section 3.3).  

**Software**

All case studies use the R statistical programming language for data analysis. While there is no specific R version requirement for the case studies, the `OCSdata` package, which can be used to get and load the data, does require R 3.5 (avocado). Furthermore, R packages used to run specific analyses in each case study may have their own R version requirements. R version requirements may be checked in the `sessionInfo()` section in each case study.  

### Experience Level Descriptions

### Experience Level Descriptions

The table below explains how we define the beginner, intermediate, and advanced experience levels. 

| Experience Level | Description |
| ------- | ---------------- |
| Beginner | Little to no previous experience with coding and/or statistical analysis. |
| Intermediate | Familiar with at least one programming language and has experience working with data and statistics. |
| Advanced | Fluent in at least one programming language and likely familiar with more. Has a depth of experience working with data science projects. |

Typically, most middle/high school and first year undergraduate students will fit in the beginner category. Upperclassmen undergraduates and some graduate students are often at the intermediate level. Most advanced level students will be at the graduate level. However, this is a generalization, and a student may be considered beginner, intermediate, or advanced at any academic level depending on their independent studies and experiences. 

## Open Case Studies in the Classroom

The case studies are structured to support both partial and full use of a case study. Educators are also free to use case study data by itself.  

### Teaching a Full Case Study

The case studies are written to provide a cohesive story that simulates data science in the real world. Reading through an entire case study is an excellent exercise for students to experience a standard data science workflow and learn the best practices of today from start to finish. The following list provides a few examples of how educators have used a full case study in the past: 

- Converted the case study into a slide deck (add link, source and example image of slide)
- Assigned students to read the case study and write a report as homework
- Suggested reading and supplemental material 
- more? 

(avocado add discussion of interactive case studies)

### Teaching Part of a Case Study

Some educators may find that only certain sections of a case study are relevant to their course learning objectives. For these educators the case studies are structured to allow for modular use. The case study [GitHub repositories](https://github.com/opencasestudies) provide the appropriate data files to be used at the start of each section. These data files can be downloaded directly from GitHub or with the [OCSdata](https://github.com/opencasestudies/OCSdata) package (see chapter 2.5). The following table describes which data folder contains the corresponding data for each case study section. An example use for each data type is provided as well. 

| Data Folder | Case Study Section | Example Use |
| ------- | --------- | ------------------------ |
| raw | Data Import | Assigning public health students to read through a case study starting from the beginning |
| imported | Data Exploration, Data Wrangling | Data science students practicing wrangling methods with in class exercises |
| wrangled | Data Visualization, Data Analysis | Statistics course practicing analysis methods with real data as a live lesson |
| simpler_import | Data Import | Introductory data science instructor wants students to practice data import without over-complication |
| extra | Not Used in Case Study | Public health course assigns homework to practice case study methods with similar but new data | 

(avocado add discussion of interactive case studies)

### Teaching With Case Study Data Only

- Data available on GitHub
- Can use OCSdata package for streamlined data retrieval process
- Suggestions on how to use data?
- Look at case studies for exercise ideas
- more?

## Case Study Recommendations

The following table lists a few example case studies that would be suitable for each experience level. 

| Experience Level | Case Studies |
| ------ | ---------------------- |
| Beginner | Exploring CO2 emissions across time: [Static](https://www.opencasestudies.org/ocs-bp-co2-emissions/), [Interactive](https://rsconnect.biostat.jhsph.edu/ocs-bp-co2-emissions-interactive/). Vaping Behaviors in American Youth: [Static](https://www.opencasestudies.org/ocs-bp-vaping-case-study/). |
| Intermediate | Mental Health of American Youth: [Static](https://www.opencasestudies.org/ocs-bp-youth-mental-health/), [Interactive](https://rsconnect.biostat.jhsph.edu/ocs-bp-youth-mental-health-interactive/). Opioids in United States: [Static](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban/), [Interactive](https://rsconnect.biostat.jhsph.edu/ocs-bp-opioid-rural-urban-interactive). |
| Advanced | Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 1: [Static](https://www.opencasestudies.org/ocs-bp-RTC-wrangling/). Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 2: [Static](https://www.opencasestudies.org/ocs-bp-RTC-analysis/), [Interactive](https://rsconnect.biostat.jhsph.edu/ocs-bp-RTC-analysis-interactive). |


## Example Use Cases

Because the case studies were developed to be modular and stand-alone, they can be used in a variety of ways that cater to the learner's goals, experience, and interests. Below, we provide a few examples of how case studies have been used previously. If you use Open Case Studies in a new way, we would love to hear about it! 

**Beginner Undergraduate Data Science Course** 

[Practical Data Science in R](https://cogs137.github.io/website/) is a 10-week intermediate undergraduate course taught be Dr. Shannon Ellis at University of California Santa Barbara. It includes three Open Case Studies and uses them to illustrate how foundational data science skills and statistical concepts taught throughout the course can be applied to real data. 

The course incorporates labs and homeworks, which have guided coding and analysis exercises related to the concepts discussed in lecture. The course also assigns written reports where students present the analysis they conduct related to the case study in the format of a scientific article (see example assignment below). 

**Advanced Graduate Data Science Course** 

[Advanced Data Science](http://jtleek.com/ads2020/) is a semester-long course taught by Dr. Jeff Leek and Dr. Roger Peng in 2020 at Johns Hopkins Bloomberg School of Public Health, primarily for PhD students. This course is designed for students to gain experience in designing and communicating data analyses effectively and critically analyzing analyses. Assignments included [writing scientific journal sections](https://github.com/advdatasci/homework9) (e.g. Introduction, Methods, Results, Discussion) based on the case studies and [extending analyses](https://github.com/advdatasci/homework11) based on results presented in the case study. 

**Independent Study**  

Case studies can be used for learners to gain experience in statistics and data science independently. We strongly recommend that independent learners aim to actively engage with the case study by running the analyses independently, exploring the data beyond what is presented in the case study, and extending the analyses by to investigate their own hypotheses. Furthermore, creating a finished product, such as a blog post or a presentation, can be an excellent demonstration of the skills learned. 

**Interactive Case Studies** 

Some of the case studies are also included in interactive versions. These versions allow students to write and run code in the browser interactively, with hints and answers available for students to check their progress as they go through the case study. Interactive case studies could be appropriate for independent learning or for in class labs, as they provide real time feedback and can reduce demands on the educator to provide intensive personalized feedback.  

## Examples of assignments 

Educators are not limited to having the students go through the case study in their current format. Case studies can be a spring board for further exploration and additional assignments. For example, in addition to helping students develop data analysis skills, we hope that the case studies can also help students develop their curiosity, technical writing and communication skills. Additional assignments can include but is not limited to data visualization and presentation, written reports, and oral presentations. Below we provide a few examples of potential assignments that educators can use to tailor instruction to the desired learning objectives. 

**Further Exploration**  

Several case studies have additional data that is not discussed. This can be used for further exploration of the subject area that was discussed in the case study. This can be guided by the questions included in the Homework section of the case studies. Case studies that have additional data include the [Opioid Use Case Study](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban/#Main_Question), the [Right to Carry Case Study](https://www.opencasestudies.org/ocs-bp-RTC-analysis/), and the [CO2 Emissions Case Study](https://www.opencasestudies.org/ocs-bp-co2-emissions/).

**Written Report** 

Below is an example of a scientific-style paper written based on the [Opioid Use Case Study](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban/#Main_Question). We also include an example rubric by which this paper can be evaluated adapted from [here](https://ocw.mit.edu/courses/biological-engineering/20-109-laboratory-fundamentals-in-biological-engineering-spring-2010/assignments/guidelines-for-writing-up-your-research/#Evaluation). 

[OCS Example Report Assignment Guide](https://cogs137.github.io/website/project/cs01.html)  

[OCS Opioid Use in the US Example Report](https://raw.githubusercontent.com/opencasestudies/OCS_Guide/main/assets/OCS_Opioids_Example_Report.pdf)

[OCS Opioid Use in the US Example Report Rubric](https://raw.githubusercontent.com/opencasestudies/OCS_Guide/main/assets/OCS_Opioids_Example_Report_Rubric.pdf)

**Oral Presentation** 

Below is an example of a presentation based on the [Vaping Behaviors in American Youth Case Study](https://www.opencasestudies.org/ocs-bp-vaping-case-study/). This presentation focuses on the context of the study and the methods used in the analysis. Assignments for presentations can be modified to emphasize presenting results and conclusions or to emphasize communication to different audiences (e.g. policy makers, other researchers, the public, etc. ).  

(avocado insert presentation assignment guide, example, and grading rubric)

**Data Visualization** 

The data visualizations included in the case studies are not the only way to present the results of the analyses. While the principles of effective data visualization are not a focus of the case studies, the data included as well as the study questions can be used to guide students through the design choices that are commonly considered when determining how to best present data. As examples, we link a [lecture on the principles of data visualization](https://paldhous.github.io/ucb/2019/dataviz/week2.html) from Dr. Peter Aldhous' Introduction to Data Visualization Course and a [data visualization assignment and accompanying grading rubric](http://vis.mit.edu/classes/6.894/A1) from the Interactive Data Visualization course at MIT's Department of Computer Science.

*Acknowledgments*

We would like to thank the following people for generously sharing the ways in which they used Open Case Studies materials in their teaching:  

- Shannon Ellis PhD., *University of California, Santa Barbara




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

