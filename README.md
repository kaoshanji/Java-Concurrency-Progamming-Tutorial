# 0 Java 高并发理论 基础知识点全覆盖
## 无论跳槽面试 / 开发，技能都将高人一等


# 1 多线程并发与线程安全，让程序更可靠

## 大量代码实例来讲解，深度掌握高并发编程

![](https://uploadfiles.nowcoder.com/files/20190815/5088755_1565799768157_4685968-6fc1465c0b063ef8.png)

# 2 高并发处理思路与手段，让跳槽面试从容不迫

## 2.1 接轨企业需求的并发技能

从真实应用场景出发,从0解构线程与并发

## 2.2 并发面试综合案例

并发面试必问考点,理清思路总结要点

## 2.3 设计巧妙易于理解

巧妙实例便于理解

![](https://uploadfiles.nowcoder.com/files/20190815/5088755_1565799768174_4685968-7fd306f9bc9b4bec.png)

## 2.4 深入理解底层原理 解决企业级并发业务问题 翻越并发技术的大山

### 线程的核心

#### 工作/面试的利器

- 线程N种实现方式
网络众口不一，真伪难辨，本教程直击本质

- 线程启动你真的会么？
启动线程，从错误到正确，带你从错误中总结真理

- 线程停止、中断的最佳实践
把我线程停止原则

- 图解线程生命周期
面试 show 出此图，优秀候选人非你莫属

- 趣解Thread和Object类中线程相关方法
wait、notify、join、yield…各有千秋

- 一网打尽线程属性线程属性
三大经典面试问题，你晓得么？

- 线程异常处理
无处不在的异常，只需一招自定义异常

- 线程安全与程序性能，取舍之道
线程安全导致性能降低，看似无解，实则只是学艺不精

# 3 精讲Java面试中的高频并发问题
为什么wait必须在同步代码块中使用？

线程是如何在6种状态之间切换的？

哪些场景需要额外注意线程安全问题？

讲一讲什么是Java内存模型？

happens-before、volatile和可见性的关系?

实际开发中如何避免死锁？

# 4 领悟Java大佬的学习方法与体系思想
如何从宏观和微观两个方面来提高技术？

提高技术的途径有哪些？

如何了解技术领域的前沿动态？

工作中业务缠身，如何在业务开发中得到更多成长?

如何分析native的c/cpp代码，如何使用openJDK？

“自顶向下”的学习方法以及好处？

# 5 环境参数

## 基本工具 

- Maven 3.3.9+

- JDK 8+

- Tomcat 8+

- MySQL 8.0.16+

- Redis 5+

## IDE
Intellij IDEA 2019.2+

## 测试工具 
Postman

JMeter

## 框架 
SpringBoot

Mybatis 

## 组件 
Kafka

RabbitMQ

elastic-job...

# 6 知识点概要

## 线程安全性
线程安全性，主要从原子性、可见性、有序性三个方面

原子性部分，   atomic包下相关类、CAS原理、Unsafe类、synchronized关键字等的使用及注意事项
可见性部分，主要介绍的是volatile关键字的规则和使用，及synchronized关键字的可见性
有序性部分，则重点讲解了happens-before原则

## 安全发布对象
安全发布对象的一些核心方法，主要通过单例类的多种实现方式，让大家在实现过程中去体会这些方法的具体含义
这也是对线程安全性的巩固，也是把线程安全性涉及的一些关键字和类再一次放到实际场景中使用，加深大家对他们的印象和认识

## 线程安全策略
线程安全策略，包括定义不可变对象、线程封闭、同步容器、并发容器等，引出并发里的关键知识J.U.C。

同时还额外介绍了开发中常见的一些线程不安全类和写法，并给出他们各自对应的替代方案。这一章涉及的内容在日常开发和面试中都会涉及很多。...

## J.U.C之AQS讲解
AQS是J.U.C的重要组件，也是面试的重要考点。

AQS模型设计及相关同步组件的原理和使用，都非常实用，具体包括：CountDownLatch、Semaphore、CyclicBarrier、ReentrantLock与锁、Condition等。

这些组件需要大家能熟练明白他们的用途及差异，不但会使用，而且还要明确知道不同方法调用后的不同效果。...

##  J.U.C组件拓展
J.U.C相关组件，主要包括FutureTask、Fork/Join框架、BlockingQueue，其中FutureTask讲解时会对比着Callable、Runnable、Future来讲。

这些组件使用场景相对AQS会少一些，但也是J.U.C的重要组成部分，也是需要掌握的

## 线程调度-线程池
J.U.C里最后一部分：线程池。面试大概率会问到线程池相关的知识点。

这一章将主要从new Thread弊端、线程池的好处、ThreadPoolExecutor详细介绍（参数、状态、方法）、线程池类图、Executor框架接口等进行讲解，需要大家能了解线程池的许多细节及配置，并能在实际项目中正确使用


## 多线程并发拓展讲解
对并发编程做些补充，但都贴近当前的面试，主要讲解死锁产生的条件及预防、多线程并发编程的最佳实践、Spring与线程安全、以及面试都特别喜欢问的HashMap和ConcurrentMap源码细节。当然，面试喜欢问的问题，对实际项目开发也是特别重要的


## 高并发之扩容
高并发部分：思路，侧重面试，扩容思路，首先介绍垂直扩容和水平扩容的区别，之后介绍数据库读操作扩展和写操作扩展思路。

## 高并发之缓存
思路，本章讲解高并发中缓存方案。

包含对缓存特征（命中率、最大元素、清空策略）、影响缓存命中率因素、缓存分类和应用场景（本地缓存、分布式缓存）、高并发场景下缓存常见问题（缓存一致性、缓存并发、缓存穿透、雪崩）等的具体介绍。此外，针对大家常用的缓存组件Guava Cache、Memcache、Redis

## 高并发之消息队列
思路，本章介绍了消息队列的特性（业务无关、FIFO、容灾、性能）、为什么需要消息队列以及消息队列的好处（业务解耦、最终一致性、广播、错峰与流控），最后对当前比较流行的消息队列组件kafka和rabbitmq做了架构分析和特性介绍

## 高并发之应用拆分
从实际项目拆分步骤讲起，让大家可以实际感受到应用拆分的好处和解决的问题，之后引出对应用拆分原则（业务优先、循序渐进、兼顾技术、可靠测试）和应用拆分时思考的内容（应用之间通信、应用之间数据库设计、避免事务跨应用），并引出对服务化Dubbo和微服务Spring Cloud的框架介绍

## 高并发之应用限流
思路，本章从实际项目保存百万数据的限流场景开始讲起，让大家感受一下某些高并发场景下使用限流和不使用限流的区别，明确限流的重要作用

之后详细介绍了限流常用的四种算法：计数法、滑动窗口、漏桶算法和令牌桶算法，并对他们做了简单的对比

## 服务降级与服务熔断
通过举例让大家明白什么是服务降级和服务熔断

之后介绍了服务降级的分类：自动降级（超时、失败次数、故障、限流）和人工降级（开关），总结了服务降级和服务熔断的共性（目的、最终表现、粒度、自治）和区别（出发原因、管理目标层次、实现方式）以及服务降级要考虑的问题

最后介绍了Hystrix

## 数据库分库分表与高可用手段
高并发部分：主讲思路，从数据库瓶颈开始讲起，引出对数据库切库分库分表的介绍。数据库切库里重点介绍了读写分离的设计，对比支持多数据源和分库的区别；

最后介绍了什么时候该考虑分表、横向分表与纵向分表，以及通过mybatis的分页插件shardbatis2.0实现数据库分表

之后介绍了高可用的三个常用手段：任务调度系统分布

## 知识体系总结
对知识进行总结回顾,希望大家都能有所收获，并期待与大家共同探讨并发与高并发的话题


![](https://uploadfiles.nowcoder.com/files/20190815/5088755_1565799768221_4685968-76a236d781f7dee7.png)
