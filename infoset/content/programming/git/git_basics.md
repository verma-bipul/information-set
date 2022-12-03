---
title: "Git_basics"
date: 2022-08-31T17:17:36-05:00
draft: false 
---
## Basics of Version Control using Git

Git is a platform for version control. If there are a large number of people working on a single project then keeping track of who made what changes when and where becomes very important.   

In my experience the best way to learn git it by demostration.

## Getting a copy of repository on local device

We don't want to make changes in the original repository which is there in the cloud (or at remote-location), hence we make a clone (or copy) of the repository and save it locally. This is accomplished using git clone as demostrated below.

```Git
git clone <ssh or https url of repo>
```
If nothing further is specified then a copy will be created in the current directory.


## Check what changes have been made locally

```git
git status
git add .
git commit -m "comments"
git push origin main
```
