---
layout: post
title:  "分布式挑战之无全局时钟-time"
date:   2021-03-19 20:37:20 +0800
categories: distributed foundation
---
# 分布式挑战之无全局时钟-time
时间本身有两个属性：顺序、计量

有以下几种：

 | 解决方案 |  特点|精度 | 使用场景 | 案例 |
 |---| --- | --- | --- | --- |
 | 本地时间 | 单点 | ns| Mysql/Postgresql|
 | 时钟同步  | |ms| ntp/chrony|
 | 前后关系接口 | ||google spanner||
 | 逻辑时钟/向量时钟 | |||raft/etcd|
