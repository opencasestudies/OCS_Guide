


# Open Case Study Infastructure

## Learning Objectives


## Libraries

For this chapter, we'll need the following packages attached:

*Remember to add [any additional packages you need to your course's own docker image](https://github.com/jhudsl/OTTR_Template/wiki/Using-Docker#starting-a-new-docker-image).


```r
library(magrittr)
```

# Topic of Section

You can write all your text in sections like this!

## Subtopic

Here's a subheading and some text in this subsection!

### Code examples

You can demonstrate code like this:


```r
output_dir <- file.path("resources", "code_output")
if (!dir.exists(output_dir)) {
  dir.create(output_dir)
}
```



### Image example


How to include a Google slide. It's simplest to use the `leanbuild` package:

<img src="resources/images/02-OCS_Infastructure_files/figure-html//1YmwKdIy9BeQ3EShgZhvtb3MgR8P6iDX4DfFD65W_gdQ_gcc4fbee202_0_141.png" title="Major point!! example image" alt="Major point!! example image" style="display: block; margin: auto;" />





### Video examples

You can use `knitr::include_url()` like this:


```r
knitr::include_url("https://www.youtube.com/embed/VOCYL-FNbr0")
```

<iframe src="https://www.youtube.com/embed/VOCYL-FNbr0" width="672" height="400px"></iframe>

OR this works:

<iframe src="https://www.youtube.com/embed/VOCYL-FNbr0" width="672" height="400px"></iframe>

### Links to files

This works:

<iframe src="https://www.messiah.edu/download/downloads/id/921/Microaggressions_in_the_Classroom.pdf" width="672" height="800px"></iframe>

Or this:

[This works](https://www.messiah.edu/download/downloads/id/921/Microaggressions_in_the_Classroom.pdf).

Or this:

<iframe src="https://www.messiah.edu/download/downloads/id/921/Microaggressions_in_the_Classroom.pdf" width="672" height="800px"></iframe>

### Links to websites

Examples of including a website link.

This works:


```r
knitr::include_url("https://yihui.org")
```

<iframe src="https://yihui.org" width="672" height="400px"></iframe>

OR this:

![Another link](https://yihui.org)

OR this:

<iframe src="https://yihui.org" width="672" height="400px"></iframe>

### Citation examples

We can put citations at the end of a sentence like this [@rmarkdown2021].
Or multiple citations [@rmarkdown2021, @Xie2018].

but they need a ; separator [@rmarkdown2021; @Xie2018].

In text, we can put citations like this @rmarkdown2021.

## Print out session info


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
## other attached packages:
## [1] magrittr_1.5
## 
## loaded via a namespace (and not attached):
##  [1] knitr_1.33      hms_0.5.3       R6_2.4.1        rlang_0.4.10   
##  [5] highr_0.8       stringr_1.4.0   httr_1.4.2      tools_4.0.2    
##  [9] xfun_0.26       jquerylib_0.1.1 htmltools_0.5.0 ellipsis_0.3.1 
## [13] yaml_2.2.1      leanbuild_0.1.2 digest_0.6.25   tibble_3.0.3   
## [17] lifecycle_1.0.0 crayon_1.3.4    bookdown_0.24   readr_1.4.0    
## [21] vctrs_0.3.4     fs_1.5.0        curl_4.3        evaluate_0.14  
## [25] rmarkdown_2.10  stringi_1.5.3   compiler_4.0.2  pillar_1.4.6   
## [29] pkgconfig_2.0.3
```
