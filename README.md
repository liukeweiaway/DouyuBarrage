# DouyuBarrage

斗鱼弹幕抓取及实时弹幕数据可视化，分为crawler(弹幕抓取)，server(弹幕统计数据服务器)，web(统计数据可视化前端)三部分。

![预览](https://github.com/Crawler995/DouyuBarrage/blob/master/doc/preview.png)

## 运行

1. 启动server模块（即启动spring boot服务器）
2. 启动web模块（npm start），输入`localhost:3000?roomid=[斗鱼房间号]`即可开始爬取

从用户角度来看，其实只做了“打开web页面”一件事就可以开始抓取弹幕，弹幕抓取进程由服务器负责启动。系统详细结构将在下面详述。

## 相关技术

1. crawler

   Python 3.7

   Mysql

2. server

   Java 8

   Spring Boot

   Mybatis

3. web

   JavaScript

   React

   Ant Design

   Echarts
   
## 架构

   ![系统运行基本流程](https://github.com/Crawler995/DouyuBarrage/blob/master/doc/process.jpg)

先随便画一个，有一说一，要说清楚这个系统有丶难，我得去复习软件工程了，不然我没法画数据流图什么的，讲不清楚这个系统的结构……

## 一些闲聊

1. 自己运行了两天，主要分析了C皇和电棍的直播间，发现棍孝子确实只会刷屏，平均一个人发了5、6条弹幕，有一个头号棍孝子一个人发了400多条弹幕；C皇观众比较均匀，平均一个人发了2条弹幕，最多的一个人也只发了20多条。