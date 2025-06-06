


# Use of Open Case Studies

## Learning Objectives


This chapter will provide guidance on how to use Open Case Studies for instruction. 

- We will give a coarse guide on which case studies include material appropriate for beginner, intermediate, or advanced learners.
- We will describe ways that instructors can use full case studies, part of a case study, or just the data.
- We will present ways in which others have used the case studies.
- We will present some examples of extensions that can accompany the case studies and can serve as a template for homework assignments or independent student exploration. 

The examples presented in this chapter are merely suggestions - modifications to the case studies to fit student needs are expected and encouraged! If you come up with a different way to use the case studies, please [let us know](https://www.opencasestudies.org/#contact) what you come up with so that other educators may be inspired by your creativity. 

### Prerequisites


#### Public Health Subject Matter
 
The case studies in Open Case Studies generally deal with topics in public health. We do not require any prior knowledge on the public health subjects examined in the case studies. The Getting Started section in each case study (specifically, the case study context) will present the subject material relevant to understanding the data and the case study implications. 

#### Statistics

The case studies cover a range of statistical approaches and skillsets. Some case studies will build on more foundational statistical concepts. The Experience Level categorization for each case study (see the [case study recommendation section](https://www.opencasestudies.org/OCS_Guide/use-of-open-case-studies.html#case-study-recommendations)) will indicate the expected prior skills that the case study will expect. Furthermore, the exact skills that the case study will use are listed in the Case Study Search Tool under the Objectives column. 

#### Coding/Data Science

All case studies use the R statistical programming language for data analysis. Some familiarity with R basics is expected for effective use of the case studies. However, depending on the data used and the extent to which it needs to be cleaned and processed before analysis, each case study may require experience with additional programming and data wrangling skills. This will be indicated by the Experience Level designation for the case study ([case study recommendation section](https://www.opencasestudies.org/OCS_Guide/use-of-open-case-studies.html#case-study-recommendations)).  

#### Software 

All case studies use the R statistical programming language for data analysis. While there is no specific R version requirement for the case studies, the `OCSdata` package, which can be used to get and load the data, does require R 3.5. Furthermore, R packages used to run specific analyses in each case study may have their own R version requirements. R version requirements may be checked in the `sessionInfo()` section in each case study.  


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

- Converted the case study into a [slide deck](https://cogs137.github.io/website/lecslides/16-cs2-data.html#1) ([Practical Data Science in R](https://cogs137.github.io/website/) taught by [Dr. Shannon Ellis](https://www.shanellis.com/) at University of California Santa Barbara)
- Assigned students to read the case study and write a report as homework ([Advanced Data Science course at Johns Hopkins ](https://github.com/advdatasci/homework9))
- Assigned students to extend analysis beyond case study ([Advanced Data Science course at Johns Hopkins ](https://github.com/advdatasci/homework11))


**Case Study Reading Time and Readability Index**

The reading time and readability index were calculated for each case study with [koRpus](https://github.com/unDocUMeantIt/koRpus). A readability index estimates the reading difficulty level of a particular text. The following table lists the reading time and the Flesch-Kincaid readability index for each case study. This information may be useful for deciding which case study to use in your curriculum. Based on the course taught by Dr. Ellis, in which the case studies were used for lecture material, it appears that for intermediate level data science students, a 10 week course could cover 2 longer case studies or 3 shorter case studies. How long a case study will take however, will depend on the experience level of the students.

| **Case Study** | **Reading Time** (minutes) | Readability Index (Flesch-Kincaid) |
| -------------------- | --------- | ---------------- |
| [School Shootings in the United States](https://www.opencasestudies.org/ocs-bp-school-shootings-dashboard) | 110 | Grade 9, Age 14 |
| [Disparities in Youth Disconnection](https://www.opencasestudies.org/ocs-bp-youth-disconnection) | 85 | Grade 8, Age 13 |
| [Opioids in United States](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban) | 90 | Grade 9, Age 14 |
| [Vaping Behaviors in American Youth](https://www.opencasestudies.org/ocs-bp-vaping-case-study) | 75 | Grade 10, Age 15 |
| [Mental Health of American Youth](https://www.opencasestudies.org/ocs-bp-youth-mental-health) | 90 | Grade 8, Age 13 |
| [Exploring global patterns of obesity across rural and urban regions](https://www.opencasestudies.org/ocs-bp-rural-and-urban-obesity) | 70 | Grade 9, Age 14 |
| [Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 1](https://www.opencasestudies.org/ocs-bp-RTC-wrangling) | 55 | Grade 9, Age 14 |
| [Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 2](https://www.opencasestudies.org/ocs-bp-RTC-analysis) | 60 | Grade 11, Age 16 |
| [Exploring CO2 emissions across time](https://www.opencasestudies.org/ocs-bp-co2-emissions) | 70 | Grade 9, Age 14 |
| [Exploring global patterns of dietary behaviors associated with health risk](https://www.opencasestudies.org/ocs-bp-diet) | 100 | Grade 10, Age 15 |
| [Predicting Annual Air Pollution](https://www.opencasestudies.org/ocs-bp-air-pollution) | 100 | Grade 10, Age 15 |

### Teaching Part of a Case Study

Some educators may find that only certain sections of a case study are relevant to their course learning objectives. For these educators the case studies are structured to allow for modular use. The case study [GitHub repositories](https://github.com/opencasestudies) provide the appropriate data files to be used at the start of each section. These data files can be downloaded directly from GitHub or with the [OCSdata](https://github.com/opencasestudies/OCSdata) package (see the [OCSdata section](https://www.opencasestudies.org/OCS_Guide/open-case-study-infrastructure.html#ocsdata) in chapter 2). The following table describes which data folder contains the corresponding data for each case study section. An example use for each data type is provided as well. 

<br>


| Data Folder | Case Study Section | Example Use |
| ------- | --------- | ------------------------ |
| raw | Data Import | Assigning public health students to read through a case study starting from the beginning |
| imported | Data Exploration, Data Wrangling | Data science students practicing wrangling methods with in class exercises |
| wrangled | Data Visualization, Data Analysis | Statistics course practicing analysis methods with real data as a live lesson |
| simpler_import | Data Import | Introductory data science instructor wants students to practice data import without over-complication |
| extra | Not Used in Case Study | Public health course assigns homework to practice case study methods with similar but new data | 


### Teaching With Case Study Data Only

Educators can use the data available with the case studies without using the case study as a whole. The data is available on GitHub and can be accessed using the `OCSdata` R package. 


## Case Study Recommendations

Each case study demonstrates an entire data analysis starting from data import and wrangling and continuing to statistical analysis and data visualization. This means that individual case studies can often incorporate different skill levels for different stages of the analyses. For example, a case study can use advanced data wrangling approaches but only need beginner level statistical analysis methods. Below we provide broad categorizations of each of the case studies in terms of the skill levels required (beginner, intermediate, or advanced) for each of the general stages of the case studies (data wrangling, data visualization, and statistics). More details on the specific skills taught in each case study can be found in the [Case Study Search Tool](https://www.opencasestudies.org/#searchtab) or in the Learning Objectives section in each case study. 

Here, we are using the following interpretations of "beginner", "intermediate", and "advanced":  

<br>

| Skill Level | Data Import | Data Wrangling | Data Visualization | Statistics | 
| ------- | --------- | --------- | ------- | --------- |
| Beginner | No experience with importing data into any programming language | No experience wrangling and cleaning raw data in any programming language | No experience visualizing data in any programming language | No experience with statistical concepts |
| Intermediate | Some experience with importing common data formats (e.g. CSVs) into R or significant experience in another programming language | Some experience wrangling or cleaning raw data in common formats (e.g. numerical data) in R or significant experience in another programming language | Some experience with common visualization packages in R (e.g. ggplot) or significant experience in another programming language | Some familiarity with common statistical concepts (e.g. summary statistics, hypothesis testing) and techniques (e.g. t-test) |
| Advanced | Experience with importing uncommon data types (e.g. PDFs or web-scraping) and comfort with troubleshooting import challenges | Experience cleaning and wrangling raw data in uncommon formats (e.g. regular expressions) in R and comfort with troubleshooting wrangling challenges | Experience with creating complex data visualizations in R and comfort with visualization challenges | Good understanding of foundational statistical concepts and comfort with applying foundational statistical techniques |



The following table lists a few example case studies that would be suitable for each experience level. 


| Case Study | Data Import | Data Wrangling | Data Visualization | Statistics | 
| ------- | --------- | --------- | ------- | --------- |
| School Shootings in the United States | Intermediate | Beginner | Advanced | Beginner | 
| Disparities in Youth Disconnection | Intermediate | Beginner | Beginner | Beginner | 
| Opioids in United States | Intermediate | Beginner | Beginner | Intermediate | 
| Vaping Behaviors in American Youth | Beginner | Beginner | Beginner | Intermediate | 
| Mental Health of American Youth | Advanced | Beginner | Beginner | Beginner | 
| Exploring global patterns of obesity across rural and urban regions | Intermediate | Beginner | Beginner | Beginner | 
| Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws - Part 1 | Beginner | Advanced | NA | NA | 
| Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws - Part 2 | NA | NA | Intermediate | Advanced | 
| Exploring CO2 emissions across time | Beginner | Beginner | Beginner | Beginner | 
| Exploring global patterns of dietary behaviors associated with health risk | Intermediate | Intermediate | Intermediate | Intermediate | 
| Predicting Annual Air Pollution | Beginner | Beginner | Intermediate | Advanced | 
| Exploring health expenditure using state-level data in the United States | Beginner | Beginner | Beginner | Beginner | 

## Troubleshooting

You may encounter errors trying to render our case studies. 

In which case, we suggest that you check the "Session Info" section under the "Additional Information "section of the case study to see what versions of packages we used. 

R packages versions can have updates to arguments and function names that can cause code to work differently or can break the code.

If you encounter an error, this is likely the reason. We try to update our case studies when we can, but we can't always update the information in a timely manner as this is currently a passion project. You can either use the error message from trying to knit the case study to determine what function may have been updated or deprecated (we recommend this option to help you or your students learn the most up-to-date information), or you can use the versions of the packages that are shown in our Session Info section and load the versions that we used, following the directions [here](https://search.r-project.org/CRAN/refmans/remotes/html/install_version.html). 

## Example Use Cases

Because the case studies were developed to be modular and stand-alone, they can be used in a variety of ways that cater to the learner's goals, experience, and interests. Below, we provide a few examples of how case studies have been used previously. If you use Open Case Studies in a new way, we would love to [hear](https://www.opencasestudies.org/#contact) about it! 

### Using Case Studies as Lecture Content

[Practical Data Science in R](https://cogs137.github.io/website/) is a 10-week intermediate undergraduate course taught by [Dr. Shannon Ellis](https://www.shanellis.com/) at University of California Santa Barbara. In 2021, Dr. Ellis taught the course using three Open Case Studies and used them to illustrate how foundational data science skills and statistical concepts taught throughout the course can be applied to real data. 

Here you can see how the course used the `OCSdata` package:

![](resources/images/shannon-casestudy.png){width=100%}

[Dr. Ellis](https://www.shanellis.com/) incorporated labs and homework assignments into the course, which had guided coding and analysis exercises related to the concepts discussed in lecture which used content from the case studies in a slide format. She also assigned written reports where students presented the analysis they conducted related to the case study in the format of a scientific article (see example assignment below). 

### Using Case Studies for Assignments

[Advanced Data Science](http://jtleek.com/ads2020/) was a semester-long graduate data science course taught by [Dr. Jeff Leek](https://jtleek.com/) and [Dr. Roger Peng](https://rdpeng.org/) in 2020 at Johns Hopkins Bloomberg School of Public Health, primarily for PhD students. This course is designed for students to gain experience in designing and communicating data analyses effectively and critically analyzing analyses. Assignments included [writing scientific journal sections](https://github.com/advdatasci/homework9) (e.g. Introduction, Methods, Results, Discussion) based on the case studies and [extending analyses](https://github.com/advdatasci/homework11) based on results presented in the case study. 

### Independent Study

Case studies can be used for learners to gain experience in statistics and data science independently. We strongly recommend that independent learners aim to actively engage with the case study by running the analyses independently, exploring the data beyond what is presented in the case study, and extending the analyses by to investigate their own hypotheses. Furthermore, creating a finished product, such as a blog post or a presentation, can be an excellent demonstration of the skills learned. 

### Interactive Case Studies

Some of the case studies also have interactive versions. These versions allow students to write and run code in the browser interactively, with hints and answers available for students to check their progress as they go through the case study. Interactive case studies could be appropriate for independent learning or for in class labs, as they provide real time feedback and can reduce demands on the educator to provide intensive personalized feedback. Please see the following video for a demonstration on how to use the interactive case studies:   


```
## `google-chrome`, `chromium-browser` and `chrome` were not found. Try setting the `CHROMOTE_CHROME` environment variable to the executable of a Chromium-based browser, such as Google Chrome, Chromium or Brave or adding one of these executables to your PATH.
```

<iframe src="https://www.youtube.com/embed/3iFtuDK0o-M" width="100%" height="400px" data-external="1"></iframe>

## Examples of assignments 

Educators are not limited to having the students go through the case study in their current format. Case studies can be a spring board for further exploration and additional assignments. For example, in addition to helping students develop data analysis skills, we hope that the case studies can also help students develop their curiosity, technical writing and communication skills. Additional assignments can include but is not limited to data visualization and presentation, written reports, and oral presentations. Below we provide a few examples of potential assignments that educators can use to tailor instruction to the desired learning objectives. See [here](http://jtleek.com/ads2020/week-5.html) guidelines about considerations for effective and ethical data visualizations from the [Advanced Data Science Course](http://jtleek.com/ads2020/) taught by [Jeff leek](https://jtleek.com/) and [Roger Peng](https://rdpeng.org/) at [Johns Hopkins Bloomberg School of Public Health](https://publichealth.jhu.edu/).

### Written Report 

Below is an example of a scientific-style paper written based on the [Opioid Use Case Study](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban/#Main_Question). We also include an example rubric by which this paper can be evaluated adapted from [here](https://ocw.mit.edu/courses/biological-engineering/20-109-laboratory-fundamentals-in-biological-engineering-spring-2010/assignments/guidelines-for-writing-up-your-research/#Evaluation). 

- [OCS Opioid Use in the US Example Report](https://raw.githubusercontent.com/opencasestudies/OCS_Guide/main/assets/OCS_Opioids_Example_Report.pdf)

- [OCS Opioid Use in the US Example Report Rubric](https://raw.githubusercontent.com/opencasestudies/OCS_Guide/main/assets/OCS_Opioids_Example_Report_Rubric.pdf)

### Oral Presentation 

Below is an example of a presentation based on the [Vaping Behaviors in American Youth Case Study](https://www.opencasestudies.org/ocs-bp-vaping-case-study/). This presentation focuses on the context of the study and the methods used in the analysis. Assignments for presentations can be modified to emphasize presenting results and conclusions or to emphasize communication to different audiences (e.g. policy makers, other researchers, the public, etc. ).  

- [OCS Vaping Case Study Oral Presentation Assignment Example](https://github.com/advdatasci/homework12)
- [OCS Vaping Case Study Oral Presentation Example](https://www.youtube.com/watch?v=noWLCSipKEU)


### Data Visualization

The data visualizations included in the case studies are not the only way to present the data used within the analyses. While the principles of effective data visualization are a focus of the case studies, the data included as well as the study questions can be used to guide students through the design choices that are commonly considered when determining how to best present data. Students can be assigned to create a new visualization beyond what is included in the case studies that emphasizes different aspects in the data.

### Further Exploration

Several case studies have additional data that is not discussed. This can be used for further exploration of the subject area that was discussed in the case study. This can be guided by the questions included in the Homework section of the case studies. Case studies that have additional data include the [Opioid Use Case Study](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban/#Main_Question), the [Right to Carry Case Study](https://www.opencasestudies.org/ocs-bp-RTC-analysis/), and the [CO2 Emissions Case Study](https://www.opencasestudies.org/ocs-bp-co2-emissions/).

Below is an example of an assignment assigned to students in the [Advanced Data Science Course at Johns Hopkins](http://jtleek.com/ads2020/). In this assignment students were asked to create a simpler machine learning analysis based on the case study. They were also asked to share their analysis with another student and write a summary and critique of the other student's analysis. This provides an opportunity for the student to try out analysis skills with their own analysis work, and also work on their comprehension skills of reading other people's work. It also shows how we can get different results with minor changes in our analyses.:

 - [OCS Air Pollution Extension Assignment Example](https://github.com/advdatasci/homework12)


*Acknowledgments*

We would like to thank the following people for generously sharing the ways in which they used Open Case Studies materials in their teaching:  

- [Dr. Shannon Ellis](https://www.shanellis.com/)
- [Dr. Jeff Leek](https://jtleek.com/)
- [Dr. Roger Peng](https://rdpeng.org/)



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

