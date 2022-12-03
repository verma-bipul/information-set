---
title: "Data_manupulation_stata"
date: 2022-08-30T20:12:28-05:00
draft: false 
---

## Data Manipulation in Stata    

Any data manipulation essentially consists of Row Operations, Column Operations. Data in stata is usually stored in two dimensions - rows and columns. If there are more dimensions to the data then they will simply be stacked together. Data manipulation will most of the times involve construction of new columns based on existing columns.

**TIPS**
- The first thing to do is to identify at which level is the data unique. 
-Whenever generating new columns again remind at what level will the new column have unique data.
- Reduce the level of data at which the manupulation is req



## The collapse command

The collapse command is used to reduce the micro level at which data is presented. For instance if the smallest level at which the data is presented is monthly level, then it can be collapsed to be presented at yearly level. 

The following example is taken from stata tutorials ucla.  
Suppose we have a dataset that looks like the following:
```stata

          famid        sex   sexdum1   sexdum2 
  1.         1          f         1         0  
  2.         1          m         0         1  
  3.         1          f         1         0  
  4.         2          m         0         1  
  5.         2          m         0         1  
  6.         2          f         1         0  
  7.         3          m         0         1  
  8.         3          f         1         0  
  9.         3          m         0         1  
```
 Then the collapse command as used below produces the following result. 
```stata
collapse (count) numkids=famid (sum) girls=sexdum1 boys=sexdum2, by(famid) 

list famid boys girls numkids 

         famid      boys     girls    numkids 
  1.         1         1         2          3  
  2.         2         2         1          3  
  3.         3         2         1          3   
```

Here the collapse function tells to count the total number of observation in the familyid variable and store it in numkids, sum the values in sexdum1 and store it in girls, sum values in sexdum2 and store it in boys --- all this will be done at the level of family as specified by the by command.


