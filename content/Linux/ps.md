---
title: "ps"
date: 2014-07-07 12:45
---

##查看进程##

	ps aux|grep http
	a 显示所有用户的所有进程（包括其它用户）
	u 按用户名和启动时间的顺序来显示进程
	x 显示无控制终端的进程


##删除进程##
	ps -ax|grep http | axrgs kill -9


	