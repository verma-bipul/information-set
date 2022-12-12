---
title: "R_plots"
date: 2022-12-03T10:40:09-06:00
draft: false 
---

### R Plots

We'll start by describing the functioning of the inbuilt R plot function, though there are better packages like ggplot.    

```R
plot(x_axis_data, y_axis_data, type="l", col="b",
     xlab="label_x", ylab="label_y", 
     xlim=c(0, 10), ylim=c(-10, 20))
title(main="TITLE", sub="subtile")
```


### GG Plots

