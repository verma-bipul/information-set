---
title: "R_basic_data_analysis"
date: 2022-09-04T17:47:22-05:00
draft: false 
---

## Loading Dataset 

```R
dataset_name <- read_dta("./family_data.dta")
df<-read.csv("path", header = T, sep = ",")
```

## Saving Dataset 

## Data Exploration

```R
names(data) # gives the list of column names present in the dataset 
colnames(data)
head(data)  # gives a few starting values of the all column in the dataset
dim(data)   # gives the dimension fo the dataset i.e rows and columns
str(data)   # give the structure of columns in the dataset
```


## Select Columns in R

```R
subset(df, df$colname = c(a, c)) 
```
This will select columns a and c from the dataset 


## Sort Datasets based on Columns
```R
df_new <- df[order(df$col1,df$col2), ]
```
This will sort the dataset in ascending order based on col1 and col2. For inverse sorting we just need to use the negative sign.


## Counting the number of unique values in R

```R
length(unique(df))
```


## Count NAs

```R
sum(is.na(vec))
```


## Merging in R

The first thing to note is that there are four standard SQL joins: Inner, Outer, Right, and Left.

```
merge(df1, df2)  #this will merge based on common columns in the two datasets
# this is a inner join which keeps only the common elements in the two datasets
```

## Fuzzy Matching in R

Sometime we would like merge two datasets based on imperfect matching of strings. This is called fuzzy matching.

