---
layout: post
title: googleplay支付
category: 游戏技术
tags: googleplay, pay
keywords: 
description: 
---


## FAQ

#### `Error checking for billing v3 support. (response: 3:Billing Unavailable`

要用美国VPN,香港VPN都不行

#### 无法购买您要买的商品？

上传到到alpha版或beta版后，点发布，三个小时候生效，要封闭测试，而不是开放测试。

#### `Can't start async operation (launchPurchaseFlow) because another async operation(launchPurchaseFlow) is in progress`

第一次支付完，要调用handleActivityResult,否则会报错。

```
@Override  
protected void onActivityResult(int requestCode, int resultCode, Intent data) {  
    Log.d(TAG, "onActivityResult(" + requestCode + "," + resultCode + "," + data);  
    if (mHelper == null) return;  

    // Pass on the activity result to the helper for handling  
    if (!mHelper.handleActivityResult(requestCode, resultCode, data)) {  
        // not handled, so handle it ourselves (here's where you'd  
        // perform any handling of activity results not related to in-app  
        // billing...  
        super.onActivityResult(requestCode, resultCode, data);  
    }  
    else {  
        Log.d(TAG, "onActivityResult handled by IABUtil.");  
    }  
} 

``` 

## Reference

* <https://developer.android.com/google/play/billing/billing_integrate.html>