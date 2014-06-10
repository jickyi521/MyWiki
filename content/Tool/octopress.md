---
title: "Octopress"
date: 2014-06-09 23:23
---
## Commands##

* `rake setup_github_pages` 设置github_pages
* `rake new post['article name']` 生成博文框架，编辑md文件即可
* `rake watch` 检测文件变化，实时生成新内容
* `rake generate` 生成静态文件 
* `rake preview` 在本机4000端口生成访问内容 
* `rake deploy` 发布文件，同步到github master  



##Zsh下octopress命令问题##

	rake new_post["test"]
	->zsh: no matches found: new_post[test]

	*1、 由于zsh的通配符造成的 *, (, |, <, [, ?, 可以用引号括起来 
    rake "new_post[test]"

    *2、要根治的话需要改zsh配置文件 加 alias rake="noglob rake" 取消通配    
	vim ~/.zshrc 


##中文标题问题##
	

	rake new_post["测试"]
	rake generate 
    Creating new post: source/_posts/2014-06-10-ce-shi-zhong-wen.markdown

    octopress自动将中文转到了拼音，如果强制将 md 改成中文标题，博客可以显示标题但点进详情后找不着对应的index.html文件，需要手工补全才能显示详情页

    推荐做法
    rake new_post["Test"]
    编辑新生成的md文件中将 title:Test 改成 title:测试


	




