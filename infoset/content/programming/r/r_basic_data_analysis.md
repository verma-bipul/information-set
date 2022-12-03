---
title: "R_basic_data_analysis"
date: 2022-09-04T17:47:22-05:00
draft: false 
---

## Loading Dataset 

```R
dataset_name <- read_dta("./family_data.dta")
df<-read.csv("path")
```


## Data Exploration

```R
names(family_data) # gives the list of column names present in the dataset 
head(family_data)  # gives a few starting values of the all column in the dataset
dim(family_data)   # gives the dimension fo the dataset i.e rows and columns
str(family_data)   # give the structure of columns in the dataset
```


## Subsetting in R

```R
subset(df, df$colname = c(a, c)) 
```
