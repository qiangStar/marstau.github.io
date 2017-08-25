---
layout: post
title: Sublime Text
category: 书籍与软件工具
tags: software／tool
keywords: Sublime
description: 
---

#### 快捷键[More](http://www.ithome.com/html/soft/31560.htm)

搜索函数 : ⌘ + R

批量缩进和反缩进:(shift +) tab

跳转到某一行=> ctrl + G

搜索打开项目中的文件: ctrl + P

粘贴并格式化: ctrl + shift + V

打开文件所在目录: ctrl + O

同文件内设置标签 : cmd + F2

前一视图: ctrl + tab

#### 正则

替换数字

```
\d
```

任意非数字

```
(.[^0-9]*)
```

#### 删除逗号后面所有字符

```
155973091,chycmaxefgk
```

```
,([a-zA-Z0-9]*)
,(.*)
```
#### 匹配中文

```
[\x{4e00}-\x{9fa5}]
```

#### |字符前的所有字符

```
{云代理}YmEHBgUANzY0Kj8y|.59.102:80
{云代理}MzllbmdoVV1TQlVb|7.243.56:8082
{云代理}ZTcRQhNEIXEhbiJz|.10.8:80
{云代理}NGI9BD8CDjcNKA01|8.60.24:80

([^\n^|]*)[|]
```

#### 定位文件到左边工程所在位置[More](http://julianhigman.com/blog/2013/07/23/sublime-text-3-keyboard-shortcut-to-reveal-file-in-sidebar/)

首选项->按键绑定 - 用户，下添加如下:

```
[
    { "keys": ["ctrl+shift+r"], "command": "reveal_in_side_bar"}
]
```

然后在当前文件中输入设置的快捷键即可跟踪工程文件位置。

#### sublime text 2 对js进行重新排版[More](http://www.iplaysoft.com/sublimetext.html)

JsFormat 的功能就是可以将一些凌乱的 JavaScript 代码重新排版，
以方便更好地阅读与编辑。
使用 Ctrl+Shift+P 调用命令面板，
输入“Package Control: Install Package”(安装扩展包)，
在插件列表中选择安装“JsFormat”(可以输入字符过滤)，待提示成功之后即已完成安装。
随便打开一个js文件（最好是换行、对齐特别凌乱的那种），
按下 Ctrl+Shift+P 调用命令面板，你会发现已经多了一项命令叫做
“Format: Javascript”，快捷键是“CTRL+ALT+F”

## Reference

* [正则使用](http://blog.sina.com.cn/s/blog_df71a16c0101k0q0.html)