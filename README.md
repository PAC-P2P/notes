## P2P

P2P is a PAC team from GDUT.

## 环境配置

### 下载及配置 Git

官网：[https://git-scm.com/downloads](https://git-scm.com/downloads)

配置及其他命令请参考：[http://huihut.com/2017/01/24/GitNotes/](http://huihut.com/2017/01/24/GitNotes/)

### 下载 Node.js

[https://nodejs.org/zh-cn/](https://nodejs.org/zh-cn/)

### 克隆项目及环境

克隆 notes：以下两句任意执行一句（貌似 https 的更快）

	git clone https://github.com/PAC-P2P/notes.git

	git clone git@github.com:PAC-P2P/notes.git

进入 notes 目录

	cd notes


### 初始化及配置依赖

初始化 git


	git init

安装依赖
 
	npm install --unsafe-perm --verbose -g hexo	

### 创建分支

	# huihut 改为你的用户名
	git branch huihut
	
### 转换分支

	# huihut 改为你的分支名
	git checkout huihut

### 写博文


修改 source/_posts 的文件

	# 新建 .md 博文，名字为"FileName"（自己改）
	hexo new "FileName"	

### 构建静态文件

	hexo g
	
### 添加全部文件到本地仓库

	git add .

### 将文件提交到仓库
	
	# "FileName" 写你做的修改
	git commit -m "Add FileName"

### 本地预览（可跳过）

	npm start

### 将本地仓库的内容推送到远程仓库

	# huihut 改为自己的分支
	git push -u origin huihut
	
### 分支合并

	# 把master分支合并到huihut分支
	git merge master huihut
	
### 为日常更博做准备

在 `notes` 同级目录下创建 `temp` 文件夹，用来存放`git`下来的最新博文


## 日常更博

1. 写好博文，并放到 `notes/source/_posts` 下，使用 `Markdown` 写，可参考 [Markdown 简易入门教程](http://huihut.com/2017/01/25/)
		
3. 到与 `notes` 同级的 `temp` 下，删除之前`git`下来的旧`notes`，并克隆下最新工程：

		git clone https://github.com/PAC-P2P/notes.git

4. 拷贝 `temp/notes/source/_posts` 下的最新博文（.md文件）到 `notes/source/_posts` 下，覆盖除了你刚写的博文外的其他博文

6. 转换到 `notes` 目录下
		
8. 转换到你的分支

		git checkout huihut

9. 构建静态文件

		hexo g
	
10. 添加全部文件到本地仓库缓冲区

		git add .

11. 将文件提交到本地仓库
	
		# "FileName" 写你做的修改
		git commit -m "Add FileName"
		
12. 将本地仓库的内容推送到远程仓库

		# huihut 改为自己的分支
		git push origin huihut
	
13. 分支合并

		# 把master分支合并到huihut分支
		git merge master huihut
	
14. 在 Github 上提交合并请求

	* 转换到自己的分支，Pull request
	
		![Pull request1](http://ojlsgreog.bkt.clouddn.com/P2PPullRequest1.jpg)

	* 写合并信息，Pull request

		![Pull request2](http://ojlsgreog.bkt.clouddn.com/P2PPullRequest2.jpg)