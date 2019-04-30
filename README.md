# django-stack-list
Django 开发栈列表

## 资源列表

+ 官方网站：https://www.djangoproject.com/

+ 扩展包聚合：https://djangopackages.org/

+ 开源包、库、框架：https://libraries.io/

+ Awesome-List：./awesome-list.md

## Route

### Python基础

+ 基础语法是否熟悉
+ 有哪些关键字
+ 有哪些内置方法
+ 解释一下什么是动态语言？动态强类型
+ 是否有编码规范的概念？
+ 解释一下什么是深拷贝和浅拷贝
+ lambda的用法以及使用场景
+ 闭包及其作用
+ 实现装饰器，对函数的结果进行缓存
+ Python的几种容器类型的差别及使用场景
+ 列表推导式的使用场景
+ yield
+ 常用内置库
+ magic method
+ 实现常见的设计模式
+ 对python进行序列化
+ 多线程、多进程
+ socket实现http server
+ 协程、进程、线程之间的区别

### Django基础

#### 整体结构

+ 如何理解设计模式中的MVC模式，用途有哪些？
+ 如何理解Django中的MTV模型
+ 介绍一下Django中你熟悉的模块及其作用
+ 如何看待Django自带的admin，并说说你的使用经验
+ 如何理解wsgi的作用
+ 如何自己实现wsgi协议
+ 为什么正式部署时不要开启DEBUG=True

#### Model层

+ 如何理解Django migration的作用
+ 是否有过手动编辑migrations文件的精力？原因是什么？有哪些需要注意的？
+ 介绍一下ORM的概念
+ 如何理解ORM在Django框架中的作用
+ 介绍一下ORM的N+1问题、发生的原因及解决方案
+ 介绍一下Django中Model的作用
+ Model的Meta属性类有哪些可配置项？其作用是什么？日常怎么使用它？
+ 介绍一下QuerySet的作用以及你常用的QuerySet优化措施
+ 介绍一下pagination的用法
+ 介绍一下Model中Field的作用
+ 如何定制Manager？什么场景下需要定制？
+ 原生的SQL的效率是否进行过对比？结果如何？如何理解这种差异？
+ Django内置提供的权限逻辑以及其颗粒度

#### View层

+ Django中function view 和class-based view的差别及其适用场景
+ 如何给class-based view添加login required装饰器
+ middleware 在Django系统中的作用
+ settings中默认配置的MIDDLERWARES有哪些？他们的作用分别是什么?是否可以移除？
+ Django系统如何判断用户是否为登录用户？
+ 对于无cookie的浏览器如何实现用户登录？
+ Django中的request和HttpResponse的作用是什么？
+ 如何处理图片上传的逻辑以及展示逻辑？
+ 介绍一下用过的Django缓存粒度

#### Form层

+ 介绍一下Django中Form的作用
+ Form中Field根Model中的Field有何关联
+ 如何在Form层实现对某个字段的校验？


#### Template层

+ 如何理解Django模板对设计师友好的说法？
+ 日常开发中如何规划Django的模板继承和include？
+ 常用标签（tag）和过滤器（filter）有哪些？
+ 在模板中如何处理静态文件
+ 在模板中如何处理系统内定义的URL？
+ 如何自定义标签和过滤器？

### Django进阶



+ 如何排查Django项目的性能问题？
+ 如何部署Django项目？不同部署方式之间的差别有哪些？
+ 部署时如何处理项目中的静态文件？
+ 如何实现自定义的登录认证逻辑？
+ 如何理解Django中Model、Form、ModelForm和Field、widget之间的关系？
+ paginator的原理是什么？如何自己实现分页逻辑？
+ Model中的Field作用是什么？
+ 什么是SQL注入？ORM又是如何解决这个问题的？
+ CSRF全称是什么？Django是如何解决这个问题的？
+ XSS攻击是指什么？在开发时应该如何避免这种攻击？
+ signal的作用以及实现逻辑是什么？
+ DATABASE 配置中 CONN_MAX_AGE参数的作用以及使用场景
+ CONN_MAX_AGE的实现逻辑是什么？
+ 用Django内置的User模型创建用户时，是否可以直接使用User(username='xxx',password="xxx").save()?
+ 上面的创建方式有什么问题？应该如何处理用户密码？
+ 使用django-rest-framework如何实现用户认证登录逻辑？
+ session模块在Django中的作用是什么？
+ 如何自定义Django中的权限粒度，实现自己的权限逻辑？
+ 如何捕获线上系统的异常？
+ 如何分析某个接口响应时间过长的问题？假设响应时间为2s，一次请求会涉及哪些数据库和缓存查询？


### 部署相关

+ 如何自动化部署项目到生产环境？具体流程是什么？
+ 介绍一下常用的自动化部署工具
+ 用到哪些监控工具？其作用是什么？使用中有什么不足之处？
+ supervisor的作用是什么？如何使用它？
+ Gunicorn的作用是什么？为何使用它？
+ 如何对系统进行压测？如何进行流量预估？
+ Nginx的作用是什么？是否能独立配置？有没有优化经验？
+ 发版逻辑是什么？如何保证新版本发生异常时能快速回滚？

### Mysql数据库

+ 如何确定哪些字段需要设置索引？
+ 什么情况下需要设定字段属性为unique=True?
+ 如何排查某个SQL语句的索引命中情况？
+ 如何排查查询过慢的SQL语句？


### Redis

+ 你了解的Redis的特点是什么？为什么会使用它？
+ Redis支持的数据类型有哪些？
+ 如何规划Redis？
+ 比如我需要把所有文章和分类数据写入Redis，在Django中直接读取Redis拿到分类和文章的数据，怎么规划数据存储？如何处理分页？
+ 是否支持事务？举个例子
+ 有哪些数据淘汰策略？
+ 当你发现有些Redis查询响应时间太长时，如何排查？可能是什么引起的？
+ 你用到的或了解到的Redis的部署结构是怎样的？
+ 是否了解Redis的持久化策略？不同的策略有什么不同？
+ 说说你了解的Redis主从同步的策略

### 常用算法

+ Python中字典类型的实现算法
+ 你了解的高级语言中的垃圾回收机制有哪些？Python中用的是什么？
+ 介绍一下你知道的缓存相关的算法？
+ 介绍一下你知道的负载均衡算法？
+ 介绍一下数据库索引相关的算法















































