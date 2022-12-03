---
title: "Predef_fns"
date: 2022-11-12T18:44:32-06:00
draft: true
---

## List of predefined function in R

**lapply(x, f)**   
The function lapply applies a function to all the elements of a list and returns another list of the same order.   
Example:    
```R
x = list(a = 1:10, b = exp(-3:3), c=c(TRUE, FALSE) )
lappy(x, mean)
```    

**paste(x, "str", sep = "?")**   
The paste function is used to add strings to a vector of strings by horizontal concatenation. The defualt spacing is a space but can be altered using sep command.     
Example:  
```R
paste(1:12, c("st", "nd", "rd", rep("th", 9)), sep="")
```

**typeof(x)**   
Displays the object type of x.

**rep(x, 10)**   
Repeats x 10 times.

**gsub("a", "b", x)**   
replace a with b at all places in x.

**iflese(istrue, then x, else y)**

**table(df$column_name)**   
builds a frequency table to entries in the column like in stata

**is.na(dat$colname)**   
returns a column with True/False values of if the observation is missing or not.

**nchar(x)**   
returns the number of charaters in each element of the vector 

----
- Character vectors are vectors of strings in R.