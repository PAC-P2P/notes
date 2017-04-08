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


```
git clone https://github.com/PAC-P2P/notes.git

git clone git@github.com:PAC-P2P/notes.git

```

进入 notes 目录


```
cd notes
```

### 初始化及配置依赖

初始化 git

```
git init
```
安装依赖

``` 
npm install --unsafe-perm --verbose -g hexo	
```

### 写博文


修改 source/_posts 的文件


### 预览及部署

本地预览

```
npm start
```

强制push到远程仓库(不推荐)

```
npm run deploy
```

## 更博到自己的分支（推荐）

1. 写好博文，使用 `Markdown` 写，可参考 [Markdown 简易入门教程](http://huihut.com/2017/01/25/)

		# 转到你的 notes 文件夹， ~/code/git 改为自己的路径
		cd ~/code/git/notes
		
		# 新建 .md 博文，名字为"FileName"（自己改）
		hexo new "FileName"

2. 在 `notes` 同级目录下创建 `temp` 文件夹，进入 `temp`  

		# 到 notes 同级目录
		cd ../
		
		# 新建 temp 文件夹
		mkdir temp
		
		# 进入temp
		cd temp
		
3. 克隆下最新工程：

		git clone https://github.com/PAC-P2P/notes.git

4. 拷贝 `temp/notes/source/_posts` 下的最新博文（.md文件）到 `notes/source/_posts` 下，覆盖你的原来的博文

		cp ./notes/source/_posts/*.md ../notes/source/_posts

5. 把你写好的博文放到 `notes/source/_posts` 下

6. 转换到 `notes` 目录下

		# 转到你的 notes 文件夹， ~/code/git 改为自己的路径
		cd ~/code/git/notes

7. 新建分支

		# huihut 改为你的用户名
		git branch huihut
		
8. 转换分支

		git checkout huihut



## 强制push到远程仓库(不推荐)

	npm run deploy
	
	