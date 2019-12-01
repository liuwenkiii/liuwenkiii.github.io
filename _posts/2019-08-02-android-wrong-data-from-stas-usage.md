---
layout: post
title: Android：使用 UsageStatsManager.queryUsageState() 返回数据有误
categories: android
description: 这个问题很不google
keywords: UsageStatsManager, queryUsageState, 应用使用情况
---

今天遇到一个问题  
  
我想获取本日的应用使用时长的数据，如下：  
~~~java
manager.queryUsageStats(UsageStatsManager.INTERVAL_DAILY, getStartMillis(), System.currentTimeMillis());  
~~~
将返回的数据打印出来觉得有些不对，于是手动算了一下  
  
结果很显然它将昨天的一部分数据也返回了  
  
这很不 Google，我不相信，于是打开浏览器查相关问题  
  
发现有开发者反映了**[同样的问题](https://stackoverflow.com/questions/45929357/getting-wrong-data-from-stats-usage-android)**，他的描述如下：  
  
~~~
I have found the daily usage stats using queryUsageStats to be completely unreliable. 
Even with UTC time adjustment, it seems that depending on the time of day it'll send back
yesterday's stats instead of today's stats.
~~~
翻译：  
~~~
我发现使用queryUsageStats的每日使用情况统计数据是完全不可靠的。
即使使用UTC时间调整，似乎根据一天中的时间它会发回昨天的统计数据而不是今天的统计数据。
~~~  
  
最后只能改用 **[UsageEvent](https://developer.android.com/reference/android/app/usage/UsageStatsManager)** 手动计算了  