---
output:
  html_document: default
  pdf_document: default
---



# Introduction


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
- How to modify and adapt components of the case studies for the classroom
- How to contribute new case studies. 


## Open Case Studies Philosophy

<img src="resources/images/ocs_graphic.png" title="Open Case Study graphic stating that open case studies provide real-world data analysis examples, that there are over 12 currently, that they are free and open-source, that the github organization is OpenCaseStudies, that the twitter handle is @OpenCaseStudies, and that the website is www.opencasestudies.org. There is a quote that says - it is always so challenging to find datasets that allow students to explore rich and complex questions. The Open Case Studies project provides an absolute gold mine of resources - from a case study reviewer. It also says that case studies are experiential - evaluating real-world problems with realistic data in a hands-on experience, complete - Demonstrating analyses from start to finish emphasizing data prepration, multimodal - including diverse education content including figures, images, videos, gifs and links, interactive - option to use case studies with questions and exercises with real-time feedback, and peer-reviewed - our case studies have been reviewed by subject matter, data science, and statistics experts." alt="Open Case Study graphic stating that open case studies provide real-world data analysis examples, that there are over 12 currently, that they are free and open-source, that the github organization is OpenCaseStudies, that the twitter handle is @OpenCaseStudies, and that the website is www.opencasestudies.org. There is a quote that says - it is always so challenging to find datasets that allow students to explore rich and complex questions. The Open Case Studies project provides an absolute gold mine of resources - from a case study reviewer. It also says that case studies are experiential - evaluating real-world problems with realistic data in a hands-on experience, complete - Demonstrating analyses from start to finish emphasizing data prepration, multimodal - including diverse education content including figures, images, videos, gifs and links, interactive - option to use case studies with questions and exercises with real-time feedback, and peer-reviewed - our case studies have been reviewed by subject matter, data science, and statistics experts." style="display: block; margin: auto;" />

## Open Case Studies Anatomy



<img src="resources/images/ocs_anatomy.png" title="Illustration of Open Case Studies anatomy, where there are three panels showing the components of the three main stages of a case study: Getting Started, 2. Analyzing the Data, 3. Wrapping-Up. Getting started includes case study context, study motivation, main question, learning objectives, and study limitations. Analyzing the data includes data description, import and exploration, wrangling, visualization, and analysis. Wrapping-up includes analysis conclusions, case study summary, next steps, homework, and additional information" alt="Illustration of Open Case Studies anatomy, where there are three panels showing the components of the three main stages of a case study: Getting Started, 2. Analyzing the Data, 3. Wrapping-Up. Getting started includes case study context, study motivation, main question, learning objectives, and study limitations. Analyzing the data includes data description, import and exploration, wrangling, visualization, and analysis. Wrapping-up includes analysis conclusions, case study summary, next steps, homework, and additional information" style="display: block; margin: auto;" />

Case studies are designed to be self-contained examples of complete data analyses. They start with a subject area of interest and a problem definition. 

Each case study is composed of three main stages: \ 

  
  
#### Stage 1: Getting Started \ 

In the first stage, students learn about the subject area they will be investigating in their data analysis. This can include historical perspectives, previous literature, and current overarching questions in the field. Ideally, this will provide motivation as to why the data analysis they will be performing is interesting and useful. Students will then further refine questions of interest and define a specific question to be investigated by the data at hand. This question will define the statistical and data science learning objectives for the case study. Finally, students will explore the limitations of their investigation and discuss why their data analysis may or may not be able to fully answer the main question of interest. 

- Case study context
- Study motivation
- Main question
- Learning objectives 
- Study limitations 

#### Stage 2: Analyzing the Data \ 

This stage includes the bulk of the data analysis. It begins with a detailed description of the data used in the case study, how it was generated, and where is was obtained. This sets the stage for a walk-through of the data import procedure and exploration of the available data. From there, the specific subsets of the data relevant to answering the main question of interest can be identified and the data can be cleaned and wrangled to give the data in the required format. The cleaned data can then be visualized and analyzed to answer the study question. 

- Data description
- Import and exploration 
- Wrangling 
- Visualization 
- Analysis 

#### Stage 3: Wrapping-Up \ 

In the final stage of the case study, students synthesize conclusions to the main study question based on the results of their data analysis. They summarize the data exploration and analysis steps they took and discuss potential next steps they could take based on their results. Finally, additional analyses are suggested as homework and additional information relevant to the case study is provided. 

- Analysis conclusions 
- Case study summary
- Next steps 
- Homework 

	
This anatomy is reflected in the table of contents of case study sections:	
<img src="resources/images/OCS_TOC_anatomy.png" title="Open Case Study Anatomy in the Table of Contents" alt="Open Case Study Anatomy in the Table of Contents" style="display: block; margin: auto;" />
  
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


The table of contents can be used to navigate to specific sections in a case study:
<img src="resources/images/TOC_scroll.gif" title="Moving GIF image illustrating how to navigate a case study with the table of contents" alt="Moving GIF image illustrating how to navigate a case study with the table of contents" style="display: block; margin: auto;" />

## Starter Kit

Open Case Studies are designed to be beginner friendly. Users can work through an entire case study with no prerequisite knowledge in programming, public health, or statistics. However, the appropriate technology, software, and a basic familiarity with R Studio is required. This section will detail what students will need to be able to jump into a case study. 

### Technical Requirements 

(avocado note from slack: what physical resources are needed - software installed - what type of computers - think about interactive case studies)

All case studies use the R statistical programming language for data analysis. R is available for Windows, Mac, and Linux and can be downloaded from the [The Comprehensive R Archive Network (CRAN)](https://cran.r-project.org/). While there is no specific R version requirement for the case studies, the OCSdata package, which can be used to download the data, requires R version 3.5 or higher. Furthermore, R packages used to run specific analyses in each case study may have their own R version requirements. R version requirements may be checked in the Session Info section in each case study.

Cheat sheets detailing how to use common packages and functions are available at the [RStudio website](https://www.rstudio.com/resources/cheatsheets/).  

### RStudio

To work with R, we recommend the RStudio Integrated Development Environment. RStudio includes a console, syntax-highlighting editor that supports direct code execution, as well as tools for plotting, history, debugging and workspace management. RStudio is available in open source and commercial editions and runs on the desktop (Windows, Mac, and Linux) or in a browser connected to RStudio Server. More information and program installation instruction are available at the [RStudio website](https://www.rstudio.com/products/rstudio/).

For reproducible data analyses and easy publishing of reports and presentations, we recommend using RMarkdown. More information about RMarkdown is also available at the [RStudio website](https://rmarkdown.rstudio.com/index.html).  

### GitHub  

Open Case Studies is hosted on GitHub. GitHub is a website and cloud service that enables developers to store, manage, and track changes to their code. OCS uses GitHub for both development and distribution purposes. Users have complete access to all case study material through our [OCS GitHub page](https://github.com/opencasestudies) where each case study is hosted in an individual repository. The repository contains all the materials needed for the case study. This includes the case study text to be distributed to students, the data used in the case study (discussed below), additional documents and references, and brief guidelines on case study use. While GitHub is not needed for users to access the case studies, users can use GitHub to streamline download and modification of case studies. Check out the GitHub Organization and OCSdata sections in Chapter 2 for more details on how to use GitHub to access case studies and modify content for personalized use. An introduction on how to get started with GitHub is available at [Happy Git](https://happygitwithr.com/index.html). 

## Feedback  

We are continually working to improve the Open Case Studies project to address learner and educator needs. Feedback is essential for this goal. If you use Open Case Studies material, we would love to hear from you! Please submit your feedback in the [user experience survey](https://www.opencasestudies.org/). We appreciate feedback about all aspects of the Open Case Studies user experience including but not limited to technical challenges, potential improvements, or new ideas on how to use the case studies in the classroom. 

## Contact Us 

You can contact us through email using this form:

<form
  action="https://formspree.io/f/myybqzpz"
  method="POST"
>
  <label>
    Your email:
    <input type="text" name="_replyto">
  </label>
  <label>
    Your message:
    <textarea rows = "5" cols = "60" name="message"></textarea>
  </label>
  <!-- your other form fields go here -->
  <button type="submit">Send</button>
</form>

<br>

You can also find us on Twitter with the following handle: [`@OpenCaseStudies`](https://twitter.com/opencasestudies)
