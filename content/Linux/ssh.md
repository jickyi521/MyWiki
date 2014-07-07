---
title: "ssh"
date: 2014-07-07 12:34
---

##远程ssh登录##

	ssh -p 2222 eason@104.131.224.95
	

##新建隧道端口转发反向代理##

	sudo ssh -D 1000 eason@104.131.224.95 -p 2222
	//然后在switchsharp 里新建个 本地 local 的 socket v5监听 1000端口 
	

