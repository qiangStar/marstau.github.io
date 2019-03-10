---
layout: post
title: Android Studio
category: 书籍与软件工具
tags: software／tool
keywords: anroid,game
description: 
---

#### 删除项目[More](http://jingyan.baidu.com/article/c74d6000813b2b0f6b595d48.html)

```
File->Project Structure
```


## Errors


#### Install repository and sync project[More](https://stackoverflow.com/questions/43495549/cannot-install-repository-and-sync-project-in-android-studio)

```
Install repository and sync project
Show in File
Show in Project Structure dialog
```

```
allprojects {
    repositories {
        jcenter()
        maven {
            url "https://maven.google.com"
        }
   }
}
```

#### `Error:Execution failed for task ':app:compileDebugKotlin'. > Compilation error. See log for more details`[More](https://stackoverflow.com/questions/43848845/errorexecution-failed-for-task-appcompiledebugkotlin-compilation-error)

```
Click on Gradle (on the right side bar) then under :app choose assembleDebug (or assembleYourFlavor if you use flavors). Error will show up in Run tab. 
```

#### 编译报错

```
No resource identifier found for attribute
```

试试改成如下

```
compile 'com.android.support:appcompat-v7:26+'
compile 'com.android.support:percent:26.0.0'
compile 'com.android.support.constraint:constraint-layout:1.0.2'
```
## Reference

