---
title: "Intro to R"
output: html_document
---

R is a programing language that is geared towards statistics. From summary stats to machine learning to data visualizations, R most likely has a package that does all those things. 

R has a number of advantages over other langauges/statstical packages 

- It's open source and most of the packages are open source 
- Syntax will make a lot of sense if you have used other stats packages
- Eats all data! From SPSS to CSV to Excel it reads everything 


Here is a sample of R resources that I've found most useful. 


## Installation  

R from CRAN: https://cloud.r-project.org/bin/windows/ 

Intergrated Development Environment Rstudio: https://www.rstudio.com/products/rstudio/download/#download 

## You have just started programing and are a bit lost and you really like a Graphical User Interface(GUI)

Radiant is for you! 

https://github.com/radiant-rstats/radiant.design  

```{r}
if (!require('radiant')) install.packages('radiant'); library('radiant')

library(radiant)

radiant::launcher() 

radiant()

```

## Learning Resources 

### R for Data Science by Garrett Grolemund and Hadley Wickham

This book will teach you how to do data science with R: You’ll learn how to get your data into R, get it into the most useful structure, transform it, visualise it and model it. I highly recomend this book. Specifically the data cleaning portions of it. 

http://r4ds.had.co.nz/ 

### Swirl 

Swirl is a package in R that teaches you R in the R console. It's a great introduction to programing as well. 

```{r}

if (!require('swirl')) install.packages('swirl'); library('swirl')

```


## Packages that are highly recomended

Packages are collections of R functions, data, and compiled code in a well-defined format. The directory where packages are stored is called the library. R comes with a standard set of packages. Here are some more packages that really help make writing R easier 

### Here 

This one is easy, it stores in a string what is your working

```{r}
if (!require('here')) install.packages('here'); library('here')

#run here()

here() 

``` 

### Tidyverse 

Tidyverse is a compilation of a number of packages. THEY ARE ALL USEFUL. (I <3 ggplot)

```{r}
if (!require('tidyverse')) install.packages('tidyverse'); library('tidyverse')
```

### Caret 

caret (Classification And Regression Training) R package that contains misc functions for training and plotting classification and regression models

```{r}
if (!require('caret')) install.packages('caret'); library('caret')
```

### Shiny 

Shiny is an R package that makes it easy to build interactive web apps straight from R. You can host standalone apps on a webpage or embed them in R Markdown documents or build dashboards. You can also extend your Shiny apps with CSS themes, htmlwidgets, and JavaScript actions

```{r}
if (!require('shiny')) install.packages('shiny'); library('shiny')
if (!require('flexdashboard')) install.packages('flexdashboard'); library('flexdashboard')

```

### Plotly

Plotly is a plotting library that generates interactive plots. (Their also a Canadian company)

```{r}
if (!require('plotly')) install.packages('plotly'); library('plotly')

```


## Packages worth experimenting with

### GIS Funtionality 

#### Leaflet 

For all your web maping needs. Use Leaflet 

```{r}
if (!require('Leaflet')) install.packages('Leaflet'); library('Leaflet')

```

#### rgdal 

Need to change a spatial projection? rgdal is for you!

```{r}
if (!require('rgdal')) install.packages('rgdal'); library('rgdal')

```



### Web Scraping 

#### rvest 

Scrape websites of their precious precious information using rvest

```{r}
if (!require('rvest')) install.packages('rvest'); library('rvest')

```
