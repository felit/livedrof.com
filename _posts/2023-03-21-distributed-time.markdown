---
layout: post
title:  "分布式挑战之无全局时钟-time"
date:   2021-03-19 20:37:20 +0800
categories: distributed foundation
---

# 分布式挑战之无全局时钟-time
时间本身有两个属性：顺序、精度，理想中有一个绝对时钟，即全局时钟，且无限精度
-  顺序：
-  精度：
    - 局域网：数据分析,时间段的长度做为分母；
    - 授时：学校考场时钟同步，医院、机场、区间测速、公共场所显示时间、金融
    - 事后：公安、故障监控、安全、交通、
## 应用场景：
- 消息的顺序性

## 时钟相关的问题
- 时钟漂移
- 

## 时钟同步与产品
- 也可以称之为“对钟”“校钟” 、子母钟、数显钟；
- 时钟同步场景：http://www.t-timing.com/solu/a1/1.html
- [时钟同步系统应用的重要性](https://www.syn029.com/h-nd-2109.html)

有以下几种：

 | 解决方案 |  特点|精度 | 使用场景 | 案例 |
 |---| --- | --- | --- | --- |
 | 本地时间 | 单点 | ns| Mysql/Postgresql|
 | 时钟同步  | |ms| ntp/chrony|
 | 前后关系接口 | ||google spanner||
 | 逻辑时钟/向量时钟 | |||raft/etcd|

[分布式系统中的时间](https://zhuanlan.zhihu.com/p/449977322)
[分布式系统：时间、时钟和事件序列](https://zhuanlan.zhihu.com/p/75143473)
参考：
- http://lamport.azurewebsites.net/pubs/time-clocks.pdf
- [计算机的时钟系统演进 ： 物理时钟 --＞ NTP --＞ LC --＞ VC --＞ TrueTime --＞ HLC](https://vigourtyy-zhg.blog.csdn.net/article/details/122633868)
-[基于一致性算法的分布式时间协同制导律](https://www.bilibili.com/read/cv16812515/)
-[分布式系统原理-时间和全局状态](https://wenku.baidu.com/view/ba846fee0975f46527d3e116.html?_wkts_=1679384067902)
- [分布式系统概念 | 分布式时钟：物理时钟、逻辑时钟、Lamport 时间戳、向量时钟、版本向量](https://oreki.blog.csdn.net/article/details/124099496)
-[Distributed System Clocks分布式系统时钟解决方案](https://blog.csdn.net/No_Game_No_Life_/article/details/110872537)