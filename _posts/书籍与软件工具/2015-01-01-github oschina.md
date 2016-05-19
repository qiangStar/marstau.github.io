---
layout: post
title: github oschina
category: 书籍与软件工具
tags: software／tool
keywords: markdown
description: 
---

#[github](https://github.com/)
####difference among *master*, *HEAD* and *origin* 
* *master*: The name of the default branch that git creates for you when first creating a repo. In most cases, "master" means "the main branch". Most shops have everyone pushing to master, and master is considered the definitive view of the repo. But it's also common for release branches to be made off of master for releasing. Your local repo has its own master branch, that almost always follows the master of a remote repo.
* *HEAD*: The current commit your repo is on. Most of the time HEAD points to the latest commit in your branch, but that doesn't have to be the case. HEAD really just means "what is my repo currently pointing at". means not the lastest version, but the current version.
* *origin*: A name commonly given to the main remote. remote is another repository that you can pull from and push to. Usually it's on some server, like github.

####reset
* git reset --hard b61ed27
  
  reset head to b61ed27 version.
* jekyll serve

####gihub.io

* jekyll doesn't support `{ {` joining together.
* not support table

First Header | Second Header | Third Header
:----------- | :-----------: | -----------:
Left         | Center        | Right
Left         | Center        | Right
* jekyll not support 

```
  [^1] [^1]: desc
```

####clone specific branch

```
git clone -b [branch_name] --single-branch [url]
```
eg:

```
git clone -b 2 --single-branch https://git.oschina.net/marstau/testing.git
```
####set username and email

```
git config --global user.name [username]
git config --global user.mail [email]
```

####add

```
git add conf
```

####push

```
git diff
git commit -am 'commit message'
git push
```

```
git push origin master
```


#[oschina](http://git.oschina.net/)

####不支持的命令

```
git submodule update --init --recursive
```
####windows下gitignore失效[More](http://blog.lixiphp.com/gitignore-not-flush/#axzz3HvTN3dbF)

用命令行强制执行此命令,
eg:


```
git add ./filename
```

####查看ignore的文件(包括全局ignore文件)

```
git config core.excludesfile
```

####查看远程url[More](http://www.liuyixi.com/2011/09/29/gitchakanyuanchengcangkudizhi/)

```
git remote -v
```  

#####若提交不了

在`.git/config`文件下加入如下内容

```
[user]
	name = marstau
	email = taumars@hotmail.com
```

####.md目录设置方法


```
##顶级目录1
###目录
####子目录1

文本1

文本2

####子目录2
##顶级目录2
```

![](/Resources/github_oschina_1.png)

从两个`##`开始都会处理为目录

##Reference
* <http://stackoverflow.com/questions/4386959/difference-between-head-and-master>
* <http://stackoverflow.com/questions/8196544/what-are-the-git-concepts-of-head-master-origin>
