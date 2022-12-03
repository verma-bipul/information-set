---
title: "Stata Basics"
date: 2022-08-29T16:38:46-05:00
draft: false 
---
## How to set the working directory in stata?   


The first thing to do when you start Stata is to set the working directory correctly.

To set the working directoty use the command:
```stata
cd "<path to file>"
cd "E:\dataset"    ///for example
```

If the directory path name is long, then one can alternatively define a global variable and call it as and when required.
```stata
global <var_name> "<directory_path_string>"
global dataset "E:\dataset"   
cd "$dataset"
```


## How to load dataset in stata?

For this we use the following command.
```stata
use "<path_to_file>"
use "E:\dataset\cars.dta"
```


## Basic data exploration in stata

Once the dataset is laoded in  temperory memory one can use the following commands.
```stata
describe // gives the number of obervations and a list of variables   

codebook // gives summary statistics for each of the variable. The execution if this command may be slow if there are a lot of obervation or variables in the dataset.   

sum <variable_name>  // gives the summary statistics for the selected variable

list <var_name>   // also give brief summary stats for the variables
```

Another useful thing to identify about the dataset is what consititues a unique observation in the dataset.    


## Helpful References

There are a lot of resources out there to learn stata. Below are links to a few of them which themselves contain further links depending on the specifics.

1. https://wlm.userweb.mwn.de/Stata/
2. https://www.stata.com/links/resources-for-learning-stata/



