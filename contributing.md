# Contributor's Guide

## Version Control

### Making a New Branch

1. Go to the main branch and pull

```
git checkout main
git pull
```

2. Create new branch from main. Replace 'new_branch' with your desired branch name.

```
git checkout -b new_branch
```

Note: See list of current branches with ```git branch```

3. Add your changes to the content.

4. Commit changes to GitHub. 

```
git add name_of.file
git commit -m "commit message here"
git push
```

5. You will likely receive this message when you attempt to push the first commit for a new branch:

```
fatal: The current branch new_branch has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin new_branch
```

Use the suggested push command set the origin upstream from your new branch. Your new branch is all set up! For all future commits you may just use ```git push``` to push your changes. 

**Tip:** If you added a file that you do not want to commit to GitHub, use ```git reset name_of.file```. This works before or after commit, but must be before push. If the file has already been pushed, use ```git revert```.

**Tip:** If you want pull changes from main into your local branch, you may stash your changes first with ```git stash```. Then move to the main branch with ```git checkout main``` and ```git pull``` to make sure your local main branch is up to date. Go back to the branch you are working on with ```git checkout your_branch``` and use ```git merge main```. Use ```git stash pop``` to bring back your local changes from the stash. This may require you to resolve conflicts if there are any. 

### Resolving Conflicts

1. Move to the main branch and pull to make sure your local main branch is up to date.

```
git checkout main
git pull
``` 

2. Go back to the branch you are working on and merge with the main branch. 

```
git checkout your_branch
git merge main
```

3. Look in the files that git lists conflicts for. The conflicting lines will be highlighed as such:

```
<<<<<<< HEAD:file.txt
My local changes
=======
...
=======
Remote main branch version
>>>>>>>
```

Keep the parts you want to save and delete the parts that need to be removed. Once you are finished resolving conflicts, make sure to remove all the lines with "<<<<<<<", "=======", ">>>>>>>".

4. Add, commit and push changes.

```
git add your_file.name
git commit -m "commit message here"
git push
```

*Note:* If you need to remove a file both locally and remotely, use ```git rm your_file.name```. If the file needs to stay on your local system but be removed from the remote, use ```git rm --cached your_file.name```.

## Writing a Chapter

### Learning Objectives

*Every chapter also needs Learning objectives that will look like this:  

This chapter will cover:  

- {You can use https://tips.uark.edu/using-blooms-taxonomy/ to define some learning objectives here}
- {Another learning objective}

### Libraries

For this chapter, we'll need the following packages attached:

*Remember to add [any additional packages you need to your course's own docker image](https://github.com/jhudsl/OTTR_Template/wiki/Using-Docker#starting-a-new-docker-image).

```{r}
library(magrittr)
```

# Topic of Section

You can write all your text in sections like this!

## Subtopic

Here's a subheading and some text in this subsection!

### Code examples

You can demonstrate code like this:

```{r}
output_dir <- file.path("resources", "code_output")
if (!dir.exists(output_dir)) {
  dir.create(output_dir)
}
```

And make plots too:

```{r}
hist_plot <- hist(iris$Sepal.Length)
```

You can also save these plots to file:

```{r}
png(file.path(output_dir, "test_plot.png"))
hist_plot
dev.off()
```

### Image example


How to include a Google slide. It's simplest to use the `ottr` package:

```{r, fig.align='center', echo = FALSE, fig.alt= "Major point!! example image"}
ottrpal::include_slide("https://docs.google.com/presentation/d/1YmwKdIy9BeQ3EShgZhvtb3MgR8P6iDX4DfFD65W_gdQ/edit#slide=id.gcc4fbee202_0_141")
```

But if you have the slide or some other image locally downloaded you can also use html like this:

<img src="resources/images/02-chapter_of_course_files/figure-html//1YmwKdIy9BeQ3EShgZhvtb3MgR8P6iDX4DfFD65W_gdQ_gcc4fbee202_0_141.png" title="Major point!! example image" alt="Major point!! example image" style="display: block; margin: auto;" />


### Video examples

You can use `knitr::include_url()` like this:

```{r}
knitr::include_url("https://www.youtube.com/embed/VOCYL-FNbr0")
```

OR this works:

<iframe src="https://www.youtube.com/embed/VOCYL-FNbr0" width="672" height="400px"></iframe>

### Links to files

This works:

```{r, fig.align="center", echo=FALSE}
knitr::include_url("https://drive.google.com/file/d/1mm72K4V7fqpgAfWkr6b7HTZrc3f-T6AV/preview", height = "800px")
```

Or this:

[This works](https://drive.google.com/file/d/1mm72K4V7fqpgAfWkr6b7HTZrc3f-T6AV/preview).

Or this:

<iframe src="https://drive.google.com/file/d/1mm72K4V7fqpgAfWkr6b7HTZrc3f-T6AV/preview" width="672" height="800px"></iframe>

### Links to websites

Examples of including a website link.

This works:

```{r, fig.align="center"}
knitr::include_url("https://yihui.org")
```

OR this:

![Another link](https://yihui.org)

OR this:

<iframe src="https://yihui.org" width="672" height="400px"></iframe>

### Citation examples

We can put citations at the end of a sentence like this [@rmarkdown2021].
Or multiple citations [@rmarkdown2021, @Xie2018].

but they need a ; separator [@rmarkdown2021; @Xie2018].

In text, we can put citations like this @rmarkdown2021.

### Print out session info

```{r}
sessionInfo()
```

