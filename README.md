 

## 目录

- [目录](#目录)
- [Java](#java)
  - [基础](#基础)
  - [容器](#容器)
  - [并发](#并发)
  - [JVM](#jvm)
  - [其他](#其他)
- [网络](#网络)
- [操作系统](#操作系统)
  - [Linux](#linux)
- [数据结构与算法](#数据结构与算法)
  - [数据结构](#数据结构)
  - [算法](#算法)
- [数据库](#数据库)
  - [MySQL](#mysql)
  - [Redis](#redis)
- [系统设计](#系统设计)
  - [必知](#必知)
  - [常用框架](#常用框架)
    - [Spring/SpringBoot](#springspringboot)
    - [MyBatis](#mybatis)
    - [Netty](#netty)
  - [认证授权](#认证授权)
    - [JWT](#jwt)
    - [SSO(单点登录)](#sso单点登录)
  - [分布式](#分布式)
    - [分布式搜索引擎](#分布式搜索引擎)
    - [RPC](#rpc)
    - [消息队列](#消息队列)
    - [API 网关](#api-网关)
    - [分布式 id](#分布式id)
    - [分布式限流](#分布式限流)
    - [分布式接口幂等性](#分布式接口幂等性)
    - [ZooKeeper](#zookeeper)
    - [其他](#其他-1)
    - [数据库扩展](#数据库扩展)
  - [大型网站架构](#大型网站架构)
    - [性能测试](#性能测试)
    - [高并发](#高并发)
    - [高可用](#高可用)
  - [微服务](#微服务)
    - [Spring Cloud](#spring-cloud)
- [必会工具](#必会工具)
  - [Git](#git)
  - [Docker](#docker)
  - [其他](#其他-2)
- [面试指南](#面试指南)
- [Java 学习常见问题汇总](#java学习常见问题汇总)
- [资源](#资源)
  - [Java 程序员必备书单](#java程序员必备书单)
  - [实战项目推荐](#实战项目推荐)
  - [Github](#github)
- [待办](#待办)
- [说明](#说明)

## Java

### 基础

**基础知识系统总结：**

1. **[Java 基础知识](docs/java/Java基础知识.md)**
2. **[Java 基础知识疑难点/易错点](docs/java/Java疑难点.md)**
3. [【选看】J2EE 基础知识](docs/java/J2EE基础知识.md)

**重要知识点详解：**

1. [枚举](docs/java/basic/用好Java中的枚举真的没有那么简单.md) （很重要的一个数据结构，用好枚举真的没有那么简单！）
2. [Java 常见关键字总结：final、static、this、super!](docs/java/basic/final,static,this,super.md)
3. [什么是反射机制?反射机制的应用场景有哪些?](docs/java/basic/reflection.md)
4. [代理模式详解：静态代理+JDK/CGLIB 动态代理实战（动态代理和静态代理的区别？JDK 动态代理 和 CGLIB 动态代理的区别？）](docs/java/basic/java-proxy.md)

**其他：**

1. [JAD 反编译](docs/java/JAD反编译tricks.md)
2. [手把手教你定位常见 Java 性能问题](./docs/java/手把手教你定位常见Java性能问题.md)

### 容器

1. **[Java 容器常见面试题/知识点总结](docs/java/collection/Java集合框架常见面试题.md)**
2. 源码分析：[ArrayList 源码](docs/java/collection/ArrayList.md) 、[LinkedList 源码](docs/java/collection/LinkedList.md) 、[HashMap(JDK1.8)源码](docs/java/collection/HashMap.md) 、[ConcurrentHashMap 源码](docs/java/collection/ConcurrentHashMap.md)

### 并发

**[多线程学习指南](./docs/java/Multithread/多线程学习指南.md)**

**面试题总结：**

1. **[Java 并发基础常见面试题总结](docs/java/Multithread/JavaConcurrencyBasicsCommonInterviewQuestionsSummary.md)**
2. **[Java 并发进阶常见面试题总结](docs/java/Multithread/JavaConcurrencyAdvancedCommonInterviewQuestions.md)**

**面试常问知识点：**

1. [并发容器总结](docs/java/Multithread/并发容器总结.md)
2. **线程池**：[Java 线程池学习总结](./docs/java/Multithread/java线程池学习总结.md)、[拿来即用的线程池最佳实践](./docs/java/Multithread/best-practice-of-threadpool.md)
3. [乐观锁与悲观锁](docs/essential-content-for-interview/面试必备之乐观锁与悲观锁.md)
4. [万字图文深度解析 ThreadLocal](docs/java/Multithread/ThreadLocal.md)
5. [JUC 中的 Atomic 原子类总结](docs/java/Multithread/Atomic.md)
6. [AQS 原理以及 AQS 同步组件总结](docs/java/Multithread/AQS.md)

### JVM

1. **[Java 内存区域](docs/java/jvm/Java内存区域.md)**
2. **[JVM 垃圾回收](docs/java/jvm/JVM垃圾回收.md)**
3. [JDK 监控和故障处理工具](docs/java/jvm/JDK监控和故障处理工具总结.md)
4. [类文件结构](docs/java/jvm/类文件结构.md)
5. **[类加载过程](docs/java/jvm/类加载过程.md)**
6. [类加载器](docs/java/jvm/类加载器.md)
7. **[【待完成】最重要的 JVM 参数指南（翻译完善了一半）](docs/java/jvm/最重要的JVM参数指南.md)**
8. [JVM 配置常用参数和常用 GC 调优策略](docs/java/jvm/GC调优参数.md)
9. **[【加餐】大白话带你认识 JVM](docs/java/jvm/[加餐]大白话带你认识JVM.md)**

### 其他

1.  **Linux IO** ： [Linux IO](docs/java/Linux_IO.md)
2.  **I/O** ：[BIO,NIO,AIO 总结 ](docs/java/BIO-NIO-AIO.md)
3.  **Java 8** ：[Java 8 新特性总结](docs/java/What's%20New%20in%20JDK8/Java8Tutorial.md)、[Java 8 学习资源推荐](docs/java/What's%20New%20in%20JDK8/Java8教程推荐.md)、[Java8 forEach 指南](docs/java/What's%20New%20in%20JDK8/Java8foreach指南.md)
4.  **Java9~Java14** : [一文带你看遍 JDK9~14 的重要新特性！](./docs/java/jdk-new-features/new-features-from-jdk8-to-jdk14.md)
5.  Java 编程规范：**[Java 编程规范以及优雅 Java 代码实践总结](docs/java/Java编程规范.md)** 、[告别编码 5 分钟，命名 2 小时！史上最全的 Java 命名规范参考！](docs/java/java-naming-conventions.md)
6.  设计模式 :[设计模式系列文章](docs/system-design/设计模式.md)

## 网络

1. [计算机网络常见面试题](docs/network/计算机网络.md)
2. [计算机网络基础知识总结](docs/network/干货：计算机网络知识总结.md)

## 操作系统

[最硬核的操作系统常见问题总结！](docs/operating-system/basis.md)

### Linux

- [后端程序员必备的 Linux 基础知识](docs/operating-system/linux.md)
- [Shell 编程入门](docs/operating-system/Shell.md)
- [我为什么从 Windows 转到 Linux？](docs/operating-system/完全使用GNU_Linux学习.md)
- [Linux IO 模型](docs/operating-system/Linux_IO.md)
- [Linux 性能分析工具合集](docs/operating-system/Linux性能分析工具合集.md)

## 数据结构与算法

### 数据结构

- [不了解布隆过滤器？一文给你整的明明白白！](docs/dataStructures-algorithms/data-structure/bloom-filter.md)
- [数据结构知识学习与面试](docs/dataStructures-algorithms/数据结构.md)

### 算法

- [硬核的算法学习书籍+资源推荐](docs/dataStructures-algorithms/算法学习资源推荐.md)
- 常见算法问题总结：
  - [几道常见的字符串算法题总结 ](docs/dataStructures-algorithms/几道常见的子符串算法题.md)
  - [几道常见的链表算法题总结 ](docs/dataStructures-algorithms/几道常见的链表算法题.md)
  - [剑指 offer 部分编程题](docs/dataStructures-algorithms/剑指offer部分编程题.md)
  - [公司真题](docs/dataStructures-algorithms/公司真题.md)
  - [回溯算法经典案例之 N 皇后问题](docs/dataStructures-algorithms/Backtracking-NQueens.md)

## 数据库

### MySQL

**总结：**

1. **[【推荐】MySQL/数据库 知识点总结](docs/database/MySQL.md)**
2. **[阿里巴巴开发手册数据库部分的一些最佳实践](docs/database/阿里巴巴开发手册数据库部分的一些最佳实践.md)**
3. **[一千行 MySQL 学习笔记](docs/database/一千行MySQL命令.md)**
4. [MySQL 高性能优化规范建议](docs/database/MySQL高性能优化规范建议.md)

**重要知识点：**

1. [数据库索引总结 1](docs/database/MySQL%20Index.md)、[数据库索引总结 2](docs/database/数据库索引.md)
2. [事务隔离级别(图文详解)](<docs/database/事务隔离级别(图文详解).md>)
3. [一条 SQL 语句在 MySQL 中如何执行的](docs/database/一条sql语句在mysql中如何执行的.md)
4. **[关于数据库中如何存储时间的一点思考](docs/database/关于数据库存储时间的一点思考.md)**

### Redis

- [关于缓存的一些重要概念(Redis 前置菜)](docs/database/Redis/some-concepts-of-caching.md)
- [Redis 常见问题总结](docs/database/Redis/redis-all.md)

## 系统设计

### 必知

1. **[RestFul API 简明教程](docs/system-design/restful-api.md)**
2. **[因为命名被 diss 无数次。Guide 简单聊聊编程最头疼的事情之一:命名](docs/system-design/naming.md)**

### 常用框架

#### Spring/SpringBoot

1. **[Spring 常见问题总结](docs/system-design/framework/spring/SpringInterviewQuestions.md)**
2. **[SpringBoot 指南/常见面试题总结](https://github.com/Snailclimb/springboot-guide)**
3. **[Spring/Spring 常用注解总结！安排！](./docs/system-design/framework/spring/spring-annotations.md)**
4. **[Spring 事务总结](docs/system-design/framework/spring/spring-transaction.md)**
5. [Spring IoC 和 AOP 详解](https://mp.weixin.qq.com/s?__biz=Mzg2OTA0Njk0OA==&mid=2247486938&idx=1&sn=c99ef0233f39a5ffc1b98c81e02dfcd4&chksm=cea24211f9d5cb07fa901183ba4d96187820713a72387788408040822ffb2ed575d28e953ce7&token=1666190828&lang=zh_CN#rd)
6. [Spring 中 Bean 的作用域与生命周期](docs/system-design/framework/spring/SpringBean.md)
7. [SpringMVC 工作原理详解](docs/system-design/framework/spring/SpringMVC-Principle.md)
8. [Spring 中都用到了那些设计模式?](docs/system-design/framework/spring/Spring-Design-Patterns.md)

#### MyBatis

- [MyBatis 常见面试题总结](docs/system-design/framework/mybatis/mybatis-interview.md)

#### Netty

1. [剖析面试最常见问题之 Netty（上）](https://xiaozhuanlan.com/topic/4028536971)
2. [剖析面试最常见问题之 Netty（下）](https://xiaozhuanlan.com/topic/3985146207)

### 认证授权

**[认证授权基础:搞清 Authentication,Authorization 以及 Cookie、Session、Token、OAuth 2、SSO](docs/system-design/authority-certification/basis-of-authority-certification.md)**

#### JWT

- **[JWT 优缺点分析以及常见问题解决方案](docs/system-design/authority-certification/JWT-advantages-and-disadvantages.md)**
- **[适合初学者入门 Spring Security With JWT 的 Demo](https://github.com/Snailclimb/spring-security-jwt-guide)**

#### SSO(单点登录)

SSO(Single Sign On)即单点登录说的是用户登陆多个子系统的其中一个就有权访问与其相关的其他系统。举个例子我们在登陆了京东金融之后，我们同时也成功登陆京东的京东超市、京东家电等子系统。相关阅读：**[SSO 单点登录看这篇就够了！](docs/system-design/authority-certification/sso.md)**

### 分布式

[分布式相关概念入门](docs/system-design/website-architecture/分布式.md)

#### 分布式搜索引擎

提高搜索效率。常见于电商购物网站的商品搜索于分类。

比较常用的是 Elasticsearch 和 Solr。

代办。

#### RPC

让调用远程服务调用像调用本地方法那样简单。

- [Dubbo 总结：关于 Dubbo 的重要知识点](docs/system-design/data-communication/dubbo.md)
- [服务之间的调用为啥不直接用 HTTP 而用 RPC？](docs/system-design/data-communication/why-use-rpc.md)

#### 消息队列

消息队列在分布式系统中主要是为了解耦和削峰。相关阅读： **[消息队列总结](docs/system-design/data-communication/message-queue.md)** 。

**RabbitMQ:**

1. [RabbitMQ 入门](docs/system-design/data-communication/rabbitmq.md)

**RocketMQ:**

1. [RocketMQ 入门](docs/system-design/data-communication/RocketMQ.md)
2. [RocketMQ 的几个简单问题与答案](docs/system-design/data-communication/RocketMQ-Questions.md)

**Kafka:**

1. **[Kafka 入门+SpringBoot 整合 Kafka 系列](https://github.com/Snailclimb/springboot-kafka)**
2. **[Kafka 常见面试题总结](docs/system-design/data-communication/kafka-inverview.md)**
3. [【加餐】Kafka 入门看这一篇就够了](docs/system-design/data-communication/Kafka入门看这一篇就够了.md)

#### API 网关

网关主要用于请求转发、安全认证、协议转换、容灾。

1. [为什么要网关？你知道有哪些常见的网关系统？](docs/system-design/micro-service/api-gateway-intro.md)
2. [如何设计一个亿级网关(API Gateway)？](docs/system-design/micro-service/API网关.md)

#### 分布式 id

1. [为什么要分布式 id ？分布式 id 生成方案有哪些？](docs/system-design/micro-service/分布式id生成方案总结.md)

#### 分布式限流

1. [限流算法有哪些？](docs/system-design/micro-service/limit-request.md)

#### 分布式接口幂等性

#### ZooKeeper

> 前两篇文章可能有内容重合部分，推荐都看一遍。

1. [【入门】ZooKeeper 相关概念总结 01](docs/system-design/framework/zookeeper/zookeeper-intro.md)
2. [【进阶】ZooKeeper 相关概念总结 02](docs/system-design/framework/zookeeper/zookeeper-plus.md)
3. [【实战】ZooKeeper 实战](docs/system-design/framework/zookeeper/zookeeper-in-action.md)
 

#### 数据库扩展

读写分离、分库分表。

 

## 必会工具

### Git

- [Git 入门](docs/tools/Git.md)

### Docker

1. [Docker 基本概念解读](docs/tools/Docker.md)
2. [一文搞懂 Docker 镜像的常用操作！](docs/tools/Docker-Image.md)
 
