---
layout: post
title: javascript基础知识
category: 编程开发
tags: javascript
keywords: 
description: 
---

## 基础语法


```
JSON.stringify(result); // object转为string
JSON.parse(str); // string转为json
```

#### `=>`

```
(x) => x + 6

相当于

function(x){
    return x + 6;
};
```

#### json使用

```
{
  "networks": {
    "5777": {
      "events": {},
      "links": {},
      "address": "0x49f62f21510b8ec6d812979b723e8f59dfa4b6de",
      "transactionHash": "0xc541427f63e958db2a04d6f64ff8371d7fb8fe13f131b9732b8b66ddce4bea70"
    }
  }
}
```

```
var MyJson = require('./x.json')
var str = JSON.stringify(MyJson["networks"]);
var jsonStr = JSON.parse(str);
console.log("jsonStr=", jsonStr[5777].address);
console.log("jsonStr2=", MyJson["networks"]["5777"]["address"]);
```


#### `...`[More](https://blog.csdn.net/qq_30100043/article/details/53391308)

### 页面加载效果fakeLoader[More](http://www.jq22.com/jquery-info2082)

扩展运算符

将一个数组转为用逗号分隔的参数序列。

## Reference



