---
title: "My Website"
author: Rohitashwa (Rohit) Sinha
date: 1st October 2019
output:
  html_document:
    toc: true
    toc_float:
      collapsed: true
---

Hello, Website!

For more information about simple R Markdown websites, please read the documentation at https://bookdown.org/yihui/rmarkdown/rmarkdown-site.html.

Please also note that simple R Markdown sites are _not_ based on **blogdown**. They are probably good for websites with only a few Rmd documents. For larger-scale and more sophisticated websites (such as blogs), you may want to use **blogdown** instead: https://github.com/rstudio/blogdown.

All things at all times!

Rohit

# The FIRST RULE OF R MARKDOWN -  YOU DON'T TALK ABOUT R MARKDOWN {#head1}


## Header 2 - The second rule of R markdown - you don't talk about R Markdown

You can link back to another section by calling the handle you have assigned it; for example [here] (#head1)



### Header 3 - An actual useful initial rule:

Take the pains to ensure you don't have  **absolute** filepaths. They will have *different* filepaths and hence you codes will fail instantly

^superscript^


Bear in mind that new lines need to be specified by either a double space or a double enter


~subscript is with tildes~


'code' text is within single quotations


Good reference website is rpubs.com


~~strikethrough~~ is within a double tilde


To add a link to another webpage 


#### Header 4 

Now to take a quick look at implanting images


# Images 

![here is the most important focus in all of this](IMG_5490.jpg)
```{r}

t1s <- read.csv("stackedT1s.csv")

summary(t1s)


```

```{r}
#for image plotting
library(tidyverse)
t1s <- read.csv("stackedT1s.csv")
print(t1s)

f<-ggplot(t1s, aes(Lesion, Deficits))
boris<-f + geom_boxplot()
print(boris)
```







