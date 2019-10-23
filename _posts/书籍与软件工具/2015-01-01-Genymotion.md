---
layout: post
title: Genymotion
category: 书籍与软件工具
tags: software／tool
keywords: 
description: 
---

## `安装`

官网安装without VirtualBox的包,手动下载低版本的virtual box，否则连不上网，如Genymotion V2.6.0,VirtualBox V4.3.4

VirtualBox设置:
Adapter:

	IPv4 Address:192.168.56.1
	Ipv4 Network Mask:255.255.255.0
DHCP Server:

	Server Address:192.168.56.100
	Server Mask:255.255.255.0
	Lower Address Bound:192.168.56.101
	Upeer Address Bound:192.168.56.254

我的本机内网地址是192.168.1.2。

然后模拟器设置上的WiredSSID要连接一下才能正常联网。

## Reference

* [官网](https://www.genymotion.com/download/)

