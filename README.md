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

部署到 github

```
npm run deploy
```

## 日常更博

1. 写好博文，使用 `Markdown` 写，可参考 [Markdown 简易入门教程](http://huihut.com/2017/01/25/MarkdownTutorial/)
2. 在 `notes` 同级目录下创建 `temp` 文件夹，进入 `temp`  
3. 克隆下最新工程：`git clone https://github.com/PAC-P2P/notes.git`
4. 拷贝 `temp/notes/source/_posts` 下的最新博文（`.md`文件）到 `notes/source/_posts` 下，覆盖你的原来的博文
5. 把你写好的博文放到 `notes/source/_posts` 下
6. 转换到 `notes` 目录下
7. 本地预览（可跳过）：`npm start`
8. 部署到 github：`npm run deploy`

