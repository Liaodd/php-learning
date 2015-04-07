# Kohana框架模块介绍

## 官方模块

* auth

基本的认证模块

* cache

缓存模块，默认提供memcache和file cache的方式

* codebench

性能分析模块

* database

mysql访问模块

* image

图片处理模块

* minion

CLI方式执行php模块

* orm

依赖database的orm模块

* unittest

* userguide

文档模块，可以轻松生成文档

## 私有模块

这些模块都是私有模块，代码再公司的git服务器上。

* mkohana

这个模块提供了如下功能：

1. 错误封装
2. 覆盖官方auth模块
3. 覆盖官方Cache模块
4. 提供webpage，api等页面的基类
5. 日志类，自动为日志加上batchID
6. curl调用模块
7. 基于curl调用模块的HPS调用模块
8. 验证码生成类
9. 自动生成配置文件模块

* API

这个模块完成度不高，基本废弃，用于配置文件配置逻辑提供api功能。
