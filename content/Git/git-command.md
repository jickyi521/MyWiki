---
title: "Git Command"
date: 2014-06-04 23:39
---

[TOC]

Git的`help`信息非常好，很多可以直接help来了解

## 远程分支 ##

参考的 [远程分支](http://git-scm.com/book/zh/Git-%E5%88%86%E6%94%AF-%E8%BF%9C%E7%A8%8B%E5%88%86%E6%94%AF)

从远程Git repo克隆，Git会自动将此remote repo命名为`origin`，并下载其中所有的数据，建立一个指向它的`master`分支的指针，在本地命名为`origin/master`

但无法在本地更改其数据。接着，Git建立一个属于自己的本地`master`分支，始于`origin`上`master`分支相同的位置，这样可以就此开始工作

	touch README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin git@github.com:jickyi521/jickyi521.github.io.git
	git push -u origin master


这里origin是remote repo name，branch name 是master

