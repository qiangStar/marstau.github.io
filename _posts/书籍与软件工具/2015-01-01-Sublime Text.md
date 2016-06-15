---
layout: post
title: Sublime Text
category: 书籍与软件工具
tags: software／tool
keywords: Sublime
description: 
---

####快捷键[More](http://www.ithome.com/html/soft/31560.htm)

搜索函数 : ⌘ + R

批量缩进和反缩进:(shift +) tab

跳转到某一行=> ctrl + G

搜索打开项目中的文件: ctrl + P

粘贴并格式化: ctrl + shift + V

打开文件所在目录: ctrl + O

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

####定位文件到左边工程所在位置[More](http://julianhigman.com/blog/2013/07/23/sublime-text-3-keyboard-shortcut-to-reveal-file-in-sidebar/)

首选项->按键绑定 - 用户，下添加如下:

```
[
    { "keys": ["ctrl+shift+r"], "command": "reveal_in_side_bar"}
]
```

然后在当前文件中输入设置的快捷键即可跟踪工程文件位置。

##Reference

* [正则使用](http://blog.sina.com.cn/s/blog_df71a16c0101k0q0.html)