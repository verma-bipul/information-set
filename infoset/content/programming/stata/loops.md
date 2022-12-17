---
title: "Loops"
date: 2022-12-13T10:03:20-06:00
draft: false
---

## For loop in stata


## Looping through parallel lists

```stata
local agrp "cat dog cow pig"

local bgrp "meow woof moo oinkoink"

local n : word count `agrp'

forvalues i = 1/`n' {
    local a : word `i' of `agrp'
  local b : word `i' of `bgrp'
   di "`a' says `b'"
}

/// Output
cat says meow
dog says woof
cow says moo
pig says oinkoink
```







### References

1. https://www.stata.com/support/faqs/programming/looping-over-parallel-lists/