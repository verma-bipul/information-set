---
title: "Gen_vs_egen"
date: 2022-08-30T17:32:59-05:00
draft: false 
---
I never understand the difference between the behaviour of gen and egen in stata. I this post I will try to collect resources that clarifies the difference between the two.


## gen vs egen sum 
The first thing to note is that gen is the simple guy which does what is asked for, however, egen likes to be a ninja - it does different things according to what function is it supplied with. egen literally stands for extended generate. 


```stata
set obs 10 
gen a = _n  // generates nos 1:10

egen b = sum(a) //gives the total sum
gen b = sum(a)  // give the running sum
```
