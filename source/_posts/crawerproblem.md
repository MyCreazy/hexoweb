---
title: JAVA爬虫遇到的一些小问题
date: 2019-03-29 22:12:23
tags:
---

目前从事做数据分析仍需要爬取相关数据，这次用JAVA做爬虫，期间使用URLConnection遇到很多问题，目前略记的一二，大概有以下几点：
1.最开始以为数据传输回来都是html，结果返回的是压缩格式，所以需要增加一个解压功能，查看是否是压缩格式，可以通过Fiddler查看，如下截图
![tree](crawerproblem/htmlformat.png)
2.关于HTTPS的请求，需要使用X509TrustManager进行证书管理。