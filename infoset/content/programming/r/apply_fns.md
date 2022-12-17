---
title: "Apply_fns"
date: 2022-12-11T21:18:37-06:00
draft: false
---

https://www.datasciencemadesimple.com/apply-function-r/


There are different kinds of apply functions:
- apply 
- mapply
- sapply


### apply

```R
apply(df, 1, fun) # Row-wise operation
apply(df, 2, fun) # Column-wise operation
```