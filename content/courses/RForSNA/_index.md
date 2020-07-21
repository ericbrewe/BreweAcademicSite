---
title: "R For SNA"
draft: false
date: "2020-07-20T00:00:00Z"
lastmod: "2020-07-20T00:00:00Z"
linktitle: R For SNA
menu:
  RForSNA:
    name: R For SNA
    weight: 1
summary: A workshop on R for doing Social Network Analysis
toc: yes
type: docs
weight: 2
---

Welcome to this workshop designed to help get you started on using R to analyze social network data. First, thanks to Dali Ma and the Social Science Research Committee for supporting these workshops!

## The Plan
These three workshops are intended to get you thinking about Social Network Analysis, which has a number of theoretical and methodological committments that are different than doing standard inferential statistics. The workshops were reverse enginneered, the goal is to do SNA, and we will focus on analyzing networks, and analyzing individuals within networks. In order to do this we will learn some R, the schedule is below.

|Topics| Date|
|------|------|
|R for SNA | 4 August 2020|
|Individuals within networks - centrality and hypothesis testing |11 August 2020|
|Properties of whole networks and network comparison | 18 August 2020|


### What might you learn?
There are lots of things that I hope you would learn: to look at the complexity of Social Networks, to use R tools to look at networks, to read code, to write code, to find that you are not afraid (and actually like) to analyze data with R. By the end of all three sessions here are things I think you should be able to do after participating in each of the workshops:

**Workshop One**

* Import Data into R
* Clean data and prepare data for SNA
* Organize data for SNA
* Vizualize data

**Workshop Two**

* Understand different centrality metrics 
* Plotting networks and incorporating centrality
* Test hypothesis using centrality metrics

**Workshop Three**

* Understand different metrics about whole networks
* Compare networks on the basis of different networks

### What is beyond the scope?
While I would love to say you'd be able to master R in the short span of 3 weeks, you will not. I've spent a decade learning it and am proficient, but am constantly learning. 

Similarly, R is a tool. You are the expert in your research, R can help *you* to uncover elements of your data. I don't know how to analyze your data - learning R will empower you to analyze your data. 


## Why R?
I began learning R because I wanted to have something that worked across different platforms. But then I realized that the Open Source movement was something that was particularly interesting to me.  But those aren't the reason. I have come to see R as crucial for reproducibility. If I write a set of code to analyze a dataset, I can re-run this code, and get the same results. I can share the code with my publications, so someone else can check my work. This is critical to doing science. R allows me to do this in a way that Excel doesn't. 

Certainly other languages (Python, Julia, etc...) will also allow for this, but why I have stuck with R is that there is a rich community that are supportive of learning and growing. 

### Why Tidyverse?
Open source things tend to be a bit tribal - within R one debate is Base R vs. Tidyverse. This is a debate about how to teach R, and I have decided to use the Tidyverse. It might not ever matter to you, but I want you to know that I have thought about this, and my answer is to use Tidyverse for the following reasons:

- Readability - Code should be readable by humans
- Coherence with my practice - I generally try to use the Tidyverse approach in my work, so I feel like I can best help by using these tools
- Coherence with themselves - These tools are organized in a way that helps them to be internally coherent
- Support - There are loads of books and websites that are published open-source, and so you can typically find the help you need. 


## Resources
Leraning R is not easy, as I have learned things, I have tried to maintain a list of the different resources that I have drawn on. 

**The Basics**

1. Install R and RStudio
2. Introduction to R (using Base R) - [R Programming for Data Science](<https://bookdown.org/rdpeng/rprogdatascience/>)
3. My all time favorite book for learning statistics and R is [Learning Statistics with R](<http://tidylsr.djnavarro.net/>)
4. Danielle Navarro also has a course [Robust Tools](<http://robust-tools.djnavarro.net/>) that gives a sense about the breadth of the tools that R provides.
5. These two guides, [The R Guide](<https://drive.google.com/file/d/1G9rqsXdesobxbWivbrD1MN0K97jMNEST/view>) and [R for Beginners](<https://drive.google.com/file/d/1jUivTK7z3Ig_51upZ4mD5l2v-PCXOoGp/view>)

**A bit more advanced**

1. Hadley Wickham's book, [R For Data Science](<https://r4ds.had.co.nz/>)
2. [Project Oriented Workflows](<https://www.tidyverse.org/blog/2017/12/workflow-vs-script/>)
3. [WTF R](<https://rstats.wtf/index.html>) Jenny Bryan is great at explaining things about R and so frequently, I find myself looking at her books.
4. [Cheat Sheets](<https://rstudio.com/resources/cheatsheets/>) I can never remember all the commands. 
  a. [Data Transformation](<file:///Users/ericbrewelaptop/Downloads/data-transformation.pdf>)
  b. [ggplot2](<https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf>)
  c. [Regular Expressions](<https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf>)
5. [Happy Git With R](<https://happygitwithr.com/>) Eventually you'll need to use Git, and this is essential reading for making that transition.
6. [RMarkdown](<https://bookdown.org/yihui/rmarkdown/software-info.html>) Markdown allows you to use reproducible code and integrate R into reporting and writing. This is how I do all my work. 
