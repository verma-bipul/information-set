---
title: "R_basics"
date: 2022-09-04T12:16:42-05:00
draft: false 
---
## Intro

To begin with we first set the working directory of a project. The code to do so is:

```R
getwd()  # This will give the current working directory
setwd("./../dir_path")  # This will set the new working directory.
```

The next important thing is to learn to install and load packages. This can be done as seen in the following demostration.
```R
install.packages("tidyverse") # to install a package
library(tidyverse)  # to call a package
```


## Standard Packages in R

- tidyverse: This is a package specifically designed for data science.
- haven: This package allows R to read data from other statistical softwares like SAS, SPSS, Stata. Haven comes as a part of tidyverse
- stringr: used for string manipulations
- random: to draw random numbers


##  Some useful commands

### Remove objects in R
```R
remove(obj_name)
```




