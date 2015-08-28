---
layout: post
title: rapidjson
category: 游戏技术
tags: Game　Engine
keywords: 
description: 
---

```
filenameValue.SetString(temp.c_str(), static_cast<int>(temp.size()));
```
Value::SetString need to allocate memory, so you have to pass allocator.

```
filenameValue.SetString(temp.c_str(), static_cast<int>(temp.size()), document.GetAllocator());
```

##Reference
