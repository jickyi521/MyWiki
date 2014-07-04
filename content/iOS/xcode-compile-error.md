---
title: "xcode compile error"
date: 2014-07-04 14:43
---

## xx duplicate symbols for architecture x86_64##

一个工程里面有多个 main 入口，只能保留一个

##Undefined symbols for architecture i386##

说明缺少某种框架，或者类。根据提示进行添加某些框架或者类。
点进相应的框架入口 .m， 看import 哪些包，如果没有引入，试着在 build phases -> link binary with libraries 里引入