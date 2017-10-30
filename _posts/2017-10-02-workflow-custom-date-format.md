---
title: 在workflow自定义时间格式
layout: post
---

不知道是哪次workflow的更新出了点幺蛾子，我的workflow几个流的时间格式都变成西文格式了。

查看了下workflow中好像没有时区设置。

只能自己动手了。

我一般都使用 2017年10月02日 这样的格式。

workflow中，使用的也是[Unicode Technical Standard #35](http://www.unicode.org/reports/tr35/)

我自定义格式为 yyyy年MM日dd日。

和大部分的编程语言中时间格式设置都差不多。
