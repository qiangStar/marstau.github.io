---
layout: post
title: Sublime Text
category: 书籍与软件工具
tags: software／tool
keywords: Sublime
description: 
---

####快捷键

搜索函数 : ⌘ + R

批量缩进和反缩进:(shift +) tab

跳转到某一行=> ctrl + G

####正则

替换数字

```
\d
```


####删除逗号后面所有字符

```
155973091,chycmaxefgk
```

```
,([a-zA-Z0-9]*)
,(.*)
```

####|字符前的所有字符

```
{云代理}YmEHBgUANzY0Kj8y|.59.102:80{云代理}MzllbmdoVV1TQlVb|7.243.56:8082{云代理}ZTcRQhNEIXEhbiJz|.10.8:80{云代理}NGI9BD8CDjcNKA01|8.60.24:80
([^\n^|]*)[|]
```

##Reference

* [正则使用](http://blog.sina.com.cn/s/blog_df71a16c0101k0q0.html)