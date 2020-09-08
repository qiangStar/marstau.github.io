---
layout: post
title: Objective-C基本语法
category: 编程开发
tags: Objective　C
keywords: 
description: 
---

#### `@interface` and `@implementation`[More](http://blog.csdn.net/l271640625/article/details/8393531),[<\<Programming in Objective-C 4th>>]

interface和implementation共同代表一个类，两者的组合相当于java中的class，即oc中的类必须包括两部分，interface部分和implementation部分，这才是oc中的一个类的完整声明；然后OC中将成员变量和成员方法的声明部分放置在interface部分中，包括继承关系，protocal实现关系，都在interface里面的头部进行声明，然后将实现部分放置在implementation部分中，相当于是将类拆分成声明和实现两部分，这两部分缺一不可，所以在OC中，不妨不要将interface叫做接口，直接叫做类声明部分来得容易理解多了，简而言之，oc中interface是类的一个部分，和implementation共同组成一个完整的类。

#### `实例方法` and `类方法`

实例方法指成员函数,类方法指静态成员函数

## ERROR

#### `Terminating app due to uncaught exception 'NSInvalidArgumentException'`

```
*** Terminating app due to uncaught exception 'NSInvalidArgumentException', reason: '-[AppController window]: unrecognized selector sent to instance 0x283fddc00'
*** First throw call stack:
(0x19e90c794 0x19e62ebcc 0x19e810f18 0x19e91061c 0x19e9127cc 0x1034dbdb8 0x1034eaf18 0x10355c870 0x103511574 0x10355cc04 0x1a236b750 0x1a23701e0 0x1a23705e8 0x1a2385c64 0x1a237ea54 0x1a2380450 0x1a2382a64 0x1a2e5a1cc 0x1a23829c4 0x1a2382e64 0x1a23828ac 0x1a2382b18 0x103534b58 0x10350c608 0x1035495d4 0x10705a338 0x10705b730 0x107069710 0x19e88a7fc 0x19e8856d0 0x19e884ce8 0x1a89cf38c 0x1a29b3444 0x102536290 0x19e70c8f0)
libc++abi.dylib: terminating with uncaught exception of type NSException
```

Solution:
```
在Appcontroller.mm文件中，在@implementation Appcontroller下增加代码@synthesize window = window；即可，
或者在appcontroller.h文件添加：
@property(nonatomic,retain)UIWindow * window;
```

## Reference





