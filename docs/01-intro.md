



# Introduction

## Learning Objectives

In this chapter we will:

- Describe the audience for this guide
- Discuss what you can expect in this guide
- Introduce the [Open Case Studies](https://www.opencasestudies.org/) project
- Introduce the case studies that make up this project

## Motivation

The [Open Case Studies project](https://www.opencasestudies.org), developed at the [Johns Hopkins Data Science Lab](https://jhudatascience.org/), is an education platform that provides self-contained, multimodal, peer-reviewed, and open-source guides for real-world examples for active experiences of complete data analyses. The intention of this guide is to provide instructors more information about how to make the most of our case studies.


## Target Audience  

This guide is intended for educators who are interested in using Open Case Studies for instruction.

Elements of the case studies can be helpful for instructors who teach:

- High school students
- Undergraduate students
- Graduate students

Elements of the case studies can assist with teaching courses about the following topics:

- Data science
- Statistics
- Public health
- Programming
- Technical writing  

... and more

## Curriculum  

This guide documents:

- The Open Case Studies philosophy 
- The general structure of case studies
- Various entry points to using the case studies (including an R package to enable modular use of the case studies)
- Examples of how to use the case studies
- Instructions on how to modify and adapt components of the case studies for the classroom
- Guidelines for contributing new case studies


## Open Case Studies Philosophy

The Open Case Studies project is an educational resource that educators can use in the classroom to teach students how to effectively derive knowledge from data in real-world challenges.

Case studies of the Open Case Studies project provide independent learners and educators with resources for data science education. The case studies use realistic data from sources that are used for actual research or public health initiatives. Each case study addresses a timely and interesting topic, in an effort to make the material more engaging and relevant.

Case studies of the project are not intended to show all aspects of the research process, and we do not claim that the analyses show the most appropriate way to analyze a given data set, however case studies are intended to demonstrate the decision making process of real data analyses, the basic challenges of analyses, to show examples of applications of data methods, and to provide context for when such methods could be applied to glean information from data. We hope to demonstrate best practices for mindful data cleaning, reproducibility, and effective data science communication. 

All case study materials are open source and free. We provide transparency about where the data came from and where possible how it was produced. We cover data and data method limitations. We try to be as complete as possible to provide users with all necessary steps to understand the analysis and to provide context, while also maintaining a reasonable length. 

Our case studies can be used for small additional assignments in a classroom setting or as the main content that educators can slowly work through with students.

We hope you find our case studies useful!

![](resources/images/ocs_graphic.png){width=100%}



### What problem are we addressing?

Despite unprecedented and growing interest in data science on campuses, there are few courses and course materials that provide meaningful opportunity for students to learn about real-world challenges. Most courses frequently fail to frame the lectures around a real-world application and provide unrealistically clean datasets that fit the assumptions of the methods in an unrealistic way. The result is that students are left unable to effectively analyze data and solve real-world challenges outside of the classroom.

### Problems with previously suggested solutions

In 1999, [Nolan and Speed](https://www.stat.berkeley.edu/users/statlabs/) argued the solution was to teach courses through in-depth case studies derived from interesting problems, with nontrivial solutions that leave room for different analyses. This innovative framework teaches the student to make important connections between the scientific question, data and statistical concepts that only come from hands-on experience analyzing data. However, these case studies based on realistic challenges, not toy examples, are scarce. Furthermore they are often open-ended without a single complete full example. This can make it challenging for instructors who are new to these topics or have limited time.

### What are we proposing as a solution?

To address this, we are developing the Open Case Studies educational resource of case studies, which demonstrate illustrative **complete** data analyses that can be used in and outside the classroom to teach learners how to effectively derive knowledge from data. Our case studies have successfully been used to teach data science and statistics courses to graduate and undergraduate students at:

 - [Johns Hopkins Bloomberg School of Public Health](https://jhu-advdatasci.github.io/2018/)
 - [Johns Hopkins University](https://www.jhu.edu/)
 - [University of California Santa Barbara](https://www.ucsb.edu/)
 
If you'd like to learn more about the Open Case Studies you can read this [thesis](https://jscholarship.library.jhu.edu/handle/1774.2/66820) by former graduate student [Michael Breshock](https://mbreshock.github.io/) @breshock_expanding_2021.
 
## Open Case Studies Anatomy



![](resources/images/ocs_anatomy.png){width=100%}

Case studies are designed to be self-contained examples of complete data analyses. They start with a subject area of interest and a problem definition. 

Each case study is composed of three main stages:

  
  
### Stage 1: Getting Started

In the first stage, students learn about the subject area they will be investigating in their data analysis. This can include historical perspectives, previous literature, and current overarching questions in the field. Ideally, this will provide motivation as to why the data analysis they will be performing is interesting and useful. Students will then further refine questions of interest and define a specific question to be investigated by the data at hand. This question will define the statistical and data science learning objectives for the case study. Finally, students will explore the limitations of their investigation and discuss why their data analysis may or may not be able to fully answer the main question of interest. 

- Case study context
- Study motivation
- Main question
- Learning objectives 
- Study limitations 

### Stage 2: Analyzing the Data 

This stage includes the bulk of the data analysis. It begins with a detailed description of the data used in the case study, how it was generated, and where is was obtained. This sets the stage for a walk-through of the data import procedure and exploration of the available data. From there, the specific subsets of the data relevant to answering the main question of interest can be identified and the data can be cleaned and wrangled to give the data in the format needed for analysis. The cleaned data can then be visualized and analyzed to answer the study question. 

- Data description
- Import and exploration 
- Wrangling 
- Visualization 
- Analysis 

### Stage 3: Wrapping-Up

In the final stage of the case study, students synthesize conclusions to the main study question based on the results of their data analysis. They summarize the data exploration and analysis steps they took and discuss potential next steps they could take based on their results. Finally, additional analyses are suggested as homework and additional information relevant to the case study is provided. 

- Analysis conclusions 
- Case study summary
- Next steps 
- Homework 

### Table of Contents
	
This anatomy is reflected in the table of contents of case study sections:

![](resources/images/OCS_TOC_anatomy.png){width=100%}
  
 <br> 
    
| **Case Study Section** | **Description** |
| ------- | ---------------- |
| Motivation | Motivating figure and text at the start of the case study |
| Main questions | Scientific question(s) |
| Learning objectives  | Both data science and statistics learning objectives |
| Context | Context of question(s) or data |
| Limitations | Any limitations in case study or with data used |
| What are the data? | Summary of where the data came from and what the data contain |
| Data import | Analyses for importing data |
| Data wrangling | Analyses for wrangling data |
| Data exploration | Analyses for data exploration | 
| Data visualization | Analyses for data visualization | 
| Data analysis | Analyses containing statistical concepts and methods to answer question(s) | 
| Summary | Summary of results and conclusion |
| Suggested homework | Question(s) to explore further |
| Additional information | Helpful links and packages used |

 <br>

The table of contents can be used to navigate to specific sections in a case study:


```
## `google-chrome`, `chromium-browser` and `chrome` were not found. Try setting the `CHROMOTE_CHROME` environment variable to the executable of a Chromium-based browser, such as Google Chrome, Chromium or Brave or adding one of these executables to your PATH.
```

<iframe src="https://www.youtube.com/embed/j-I0Zgicjsk" width="100%" height="400px" data-external="1"></iframe>

## Starter Kit

Open Case Studies are designed to be beginner friendly. Users can work through an entire case study with no prerequisite knowledge in programming, public health, or statistics. However, the appropriate technology, software, and a basic familiarity with R Studio is required. This section will detail what students will need to be able to jump into a case study. 

### Technical Requirements 

All case studies use the R statistical programming language for data analysis. R is available for Windows, Mac, and Linux and can be downloaded from the [The Comprehensive R Archive Network (CRAN)](https://cran.r-project.org/). While there is no specific R version requirement for the case studies, the [`OCSdata`](https://github.com/opencasestudies/OCSdata) package, which can be used to download the data, requires R version 3.5 or higher. Furthermore, R packages used to run specific analyses in each case study may have their own R version requirements. R version requirements may be checked in the Session Info section in each case study.

Cheat sheets detailing how to use common packages and functions are available at the [RStudio website](https://www.rstudio.com/resources/cheatsheets/).  

Please note that to install R version 3.5 and higher you will need to have a [web browser](https://en.wikipedia.org/wiki/Web_browser) and a compatible [operating system](https://en.wikipedia.org/wiki/Operating_system). See this [link](https://cran.r-project.org/) for more information.

**Case Study Compilation Times**

The following table lists the time it took for RMarkdown to compile each case study using the "Knit" button in RStudio. 

| **Case Study** | **Compilation Time** (seconds) |
| -------------------- | -------------- |
| [School Shootings in the United States](https://www.opencasestudies.org/ocs-bp-school-shootings-dashboard) | 29 - 39 |
| [Disparities in Youth Disconnection](https://www.opencasestudies.org/ocs-bp-youth-disconnection) | 36 - 46 |
| [Opioids in United States](https://www.opencasestudies.org/ocs-bp-opioid-rural-urban) | 103 - 113 |
| [Vaping Behaviors in American Youth](https://www.opencasestudies.org/ocs-bp-vaping-case-study) | 107 - 117 |
| [Mental Health of American Youth](https://www.opencasestudies.org/ocs-bp-youth-mental-health) | 35 - 45 |
| [Exploring global patterns of obesity across rural and urban regions](https://www.opencasestudies.org/ocs-bp-rural-and-urban-obesity) | 31 - 41 |
| [Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 1](https://www.opencasestudies.org/ocs-bp-RTC-wrangling) | ??? |
| [Influence of Multicollinearity on Measured Impact of Right-to-Carry Gun Laws Part 2](https://www.opencasestudies.org/ocs-bp-RTC-analysis) | 39 - 49 |
| [Exploring CO2 emissions across time](https://www.opencasestudies.org/ocs-bp-co2-emissions) | 36 - 46 |
| [Exploring global patterns of dietary behaviors associated with health risk](https://www.opencasestudies.org/ocs-bp-diet) | 79 - 89 |
| [Predicting Annual Air Pollution](https://www.opencasestudies.org/ocs-bp-air-pollution) | 148 - 158 |

These compilation times were measured on a PC machine operating on Windows 10. The ranges listed should only be used as estimates as compilation time will vary with different machines and operating systems.

### RStudio

To work with R, we recommend the RStudio Integrated Development Environment. RStudio includes a console, syntax-highlighting editor that supports direct code execution, as well as tools for plotting, history, debugging and workspace management. RStudio is available in open source and commercial editions and runs on the desktop (Windows, Mac, and Linux) or in a browser connected to RStudio Server. More information and program installation instruction are available at the [RStudio website](https://www.rstudio.com/products/rstudio/).

For reproducible data analyses and easy publishing of reports and presentations, we recommend using RMarkdown. More information about RMarkdown is also available at the [RStudio website](https://rmarkdown.rstudio.com/index.html).  

### GitHub  

Open Case Studies is hosted on GitHub. GitHub is a website and cloud service that enables developers to store, manage, and track changes to their code. OCS uses GitHub for both development and distribution purposes. Users have complete access to all case study material through our [OCS GitHub page](https://github.com/opencasestudies) where each case study is hosted in an individual repository. The repository contains all the materials needed for the case study. This includes the case study text to be distributed to students, the data used in the case study (discussed below), additional documents and references, and brief guidelines on case study use. While GitHub is not needed for users to access the case studies, users can use GitHub to streamline download and modification of case studies. Check out the GitHub Organization and OCSdata sections in [Chapter 2](https://www.opencasestudies.org/OCS_Guide/open-case-study-infrastructure.html) for more details on how to use GitHub to access case studies and modify content for personalized use. An introduction on how to get started with GitHub is available at [Happy Git](https://happygitwithr.com/index.html). 

## Feedback

We are continually working to improve the Open Case Studies project to address learner and educator needs. Feedback is essential for this goal. If you use Open Case Studies material, we would love to hear from you!

### Survey

Please consider participating in our [user experience survey](https://www.opencasestudies.org/#survey).

We appreciate feedback about all aspects of the OCS user experience including but not limited to technical challenges, potential improvements, or new ideas on how to use the case studies in the classroom. 

<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfpN4FN3KELqBNEgf2Atpi7Wy7Nqy2beSkFQINL7Y5sAMV5_w/viewform?embedded=true" width="100%" height="400px" data-external="1"></iframe>

### Feedback for this Guide

If you have feedback for this guide about how we can improve the content, please see [here](https://github.com/opencasestudies/OCS_Guide/issues/new/choose).


## Contact Us 

If you have any questions, suggestions for improvement for individual case studies, ideas, or thoughts, you can contact us through email using this form:

<iframe src="https://www.opencasestudies.org/#contact" width="100%" height="400px" data-external="1"></iframe>



Also, see the [final chapter](https://www.opencasestudies.org/OCS_Guide/new-case-studies---building-and-contributing.html) for information on submitting case studies to our collection.

You can also find us on Twitter with the following handle: [`@OpenCaseStudies`](https://twitter.com/opencasestudies)
