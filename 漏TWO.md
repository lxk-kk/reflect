##### 项目/开放

+ ​

+ **项目相关，项目细节，遇到的困难，是如何解决的**

  我的项目数据量有多大，假如公司的项目当数据量大的情况下，你觉得瓶颈会在哪里？

  面试官说分库分表过时了，支撑不住大数据量（天哪？我学习的太落后了）

+ **实习经历**

+ ​

+ 你自己的最大优势是什么，举个例子  

+ 编译原理课程做了什么 

+ ​
+ 开放题： 要实现一个像[京东]()商城中的购物车，数据存储应该如何设计 
   追问 1： 对于游客账号，这些数据应该如何存储 
   追问 2： 如果数据量超过数据库承载能力，有什么方案

##### Java

+ **如何在C++中调用汇编代码** 
+ Java基本变量类型 ， java中的基本变量类型，各占多少比特
+ static 关键字的作用 
+ final 关键字的作用，final 能修饰方法吗？（猜了个不能，答错了） 
+ JDK7和8的区别 
+ java反射讲一下  java序列化(这个我真的不会。。。)  
+ ​
+ Java数据结构 
  +  常见的集合类
  +  ArrayList和LinkedList讲一下
  +  ArrayList 和 LinkedList 的原理和实现 
  +  链表和数组的区别 

- HashMap 的实现原理，如何通过Key获得Value 

  - HashMap 和 HashTable 的区别和原理 

  - 哈希冲突解决方法 

  - HashMap原理 

    链表转红黑树阈值，红黑树转链表阈值，为什么 

  - **hashmap讲一下 resize做了啥** 

    + 计算新的桶容量、计算新的阈值、使用新计算的 桶大小 创建一个新的 哈希表（数组）。

    + 将 HashMap 中的哈希表指向新的哈希表。

    + 遍历 旧哈希表 中的桶，分离旧桶中的 链表：原位置 链表，新位置 链表

      将这两条链表存入 新表 中指定的位置。

  - ConcurrentHashMap原理

  - 看过源码吗？我说HashMap  

  - **HashMap当在扩容时候进行put操作时，会怎么办呢？**  

    - put 的时候不会做任何的安全措施，直接
    - *（没问尽量不要说，你没看过 辅助扩容的源码）ConcurrentHashMap 在 putVal 的时候，如果正在 resize 就会辅助扩容。*

- lock 和 synchronized区别  

  + sychronized 静态方法和不同方法的区别 

  + Lock锁，synchronized,volatile

  + 什么时候使用 synchronized，[内部实现](https://www.pianshen.com/article/8275204637/)是怎么样的？

    + synchronized 加锁的目标是 Java 对象，对类加锁也借助 Java 对象实现的，加锁对象为 Class 实例。

    + synchronized 对象锁，在 JVM 层面是通过 对象的 monitor 实现。

      monitorenter：加锁

      monitorexit：释放锁

      每一个对象都有一个 monitor 与之相关联，当线程执行到 monitorenter 时，会尝试获取锁，将 monitor 的 owner 设置尝试获取锁的线程。并且 monitor 中的 锁记数器 count 会执行 +1 操作


  + lock和synchronized区别  

  + Synchronized与ReentrantLock区别 

  + Synchronized锁方法和锁代码段的实现，主要是对象头（markword）与monitor_enter讲一下

  + Synchronized会响应中断么 

- 多线程

  - 进程和线程的区别，为什么不使用多进程而是多线程
  - 线程状态 主线程能拿到子线程的执行结果和异常吗 
  - **线程安全，如何解决多线程下数据不安全的情况 ，线程安全在JVM中的体现 ** 
  - 自旋锁和互斥锁区别 
  - Java中的乐观锁，CAS及其缺点 
  - Java中创建线程的方法 
  - Java中锁的种类 
  - ThreadLocal 
    + ThreadLocal怎么用的？内存泄漏，弱引用问题，垃圾回收（本来想把面试官引过来，没得逞）  
    + 内存泄漏 内存溢出  
  - 线程池参数 
  - 若线程池中2个线程，执行完毕，现有新任务会怎样 

##### JVM

+ jvm了解吗，如果项目上线出现了 异常，怎么排查  
+ 堆栈区别 
+ Jvm 垃圾回收的大致原理 
+ Java 的内存模型 
+ static 什么时候被初始化 
+ Java 的垃圾回收机制 
+ Jvm 分代回收模型    
+ 持久代的作用（不会） 
+ GC 垃圾回收机制
+ JVM内存模型 
+ JVM(记不太清): 
+ JVM构成部分 
+ 垃圾回收机制 
+ GC的种类 
+ JVM分区 
+ 垃圾回收讲一下 
+ 对象是否存活  
+ 垃圾回收俩次标记(忘了。。。)  
+ 讲一下JMM  
+ happens-before，举个例子 
+ CMS原理 
+ CMS 中Stop the word阶段 

##### 操作系统

+ 如何查看系统的启动时间（我答了查看日志，应该是回答 uptime） 

+ CPU Load 和 CPU利用率的区别（不会） 

+ 查看系统当前所有的 Python 进程 

+ top 的作用 

+ 管道的作用 

+ IO 重定向 

+ 死锁线程的方法 互斥资源 

+ 死锁的条件，从破坏死锁必要条件答如何避免死锁 

+ 进程和线程的区别      

  - 介绍协程（不会） 

+ 死锁相关      

  - 死锁的产生 
  - 预防和检测死锁 

+  用户态到内核态 

+ select,poll,epoll 

  epoll数据结构 

+ IO 多路复用，select、poll、epoll 调用

+ 网络编程讲一下 socket 同步通信 异步通信 select poll epoll 

+ 僵尸进程与孤儿进程的区别 

+  进程通信方法 

+  常用的linux命令 

##### 计网/网络编程

+ 拥塞控制原理 

+  AIMD算法中在包丢失情况下，窗口大小

+  不同语言之前通讯方式（跨语言通信方案） C和Java之间 

+  长短连接实现 

+ TCP 和 UDP 的区别 

+ HTTP 状态码 

+ SSL 握手的过程    

  - 有几次RTT 
  - 快速恢复SSL的方法 

  对称加密和非对称加密的对比

+ 浏览器请求的过程 

+  HTTP无状态 

+  1.1和1.0区别 

+  讲一下https 

+  抓包 工具 能否看到ack和状态码 

+ NIO原理 

+ http协议 

+ 从浏览器输入一个url，到客服端得到反馈渲染页面的总过程 

+ 为什么我们输入域名时不用输入端口号，而我们通过IP访问时要输入端口号 

+ TCP协议的概念 

+ TCP的三次握手 

+ TCP和UDP的区别 

+ HTTP状态码 403什么意思

+ cookie知识   

+ Http请求头 

+ Http2.0与1.0的区别 

+ HTTP1.1与1.0的区别 

##### 算法 

+ 算法题：有序整型数组的二分查找

+ 堆排序

+ 快速排序 

+ 单向链表 如何快速得到长度

+ 日志文件很多行 rest接口提供 如何能够快速去对某个字符串进行筛选？？

+ 排序算法 

+ 第K大个数

+ 大量数字中只出现过一次的数字

+ 手撕了个代码：用数组实现循环链表

+ 在10亿数中找到一个数（bitmap） 

+  找数据流的中位数（剑指offer）

+ 思考题

  有100万个IP和对应的地址，你使用什么结构实现他  

  思考问题二，如果让你用二分，你怎么做   


##### Spring 

+ spring boot 了解吗 

+ spring cloud 了解吗

+ SpringMVC 的大致流程是什么？ 

  Spring Aop 的实现原理 

+  Spring核心: IOC AOP 

+  Spring中事务性的体现，还有具体如何实现的 

+  Spring Cloud熟悉么，Spring Cloud有哪些重要的组件

+ spring boot加载bean过程？？？我说了spring bean的生命周期

+ springboot启动类放置目录在哪里？  

+ spring 拦截器知识 

+ 讲一下spring，springmvc，springboot(概述，常用注解)  

+ spring IOC，AOP  

+ AOP原理，静态***和动态***讲一下  

+ Spring AOP实现原理 

+ Mybatis $与#的区别 

+ Mybatis与Hibernate的区别 

##### Redis 

+ redis有哪些高可用方案？我是单机实例，我不会
+ Redis 如何部署 集群 RDB和AOF介绍
+ Redis了解么。Redis除了了解用于缓存,还了解作为消息队列的用法么 
+ 你对redis的了解有多少，我自己会多少说了多少，有哪些类型，持久化，底层数据结构 
+ Redis怎么用的？数据类型有哪些，存验证码的话用的哪个数据类型？数据持久化方式RDB和AOF的优缺点？  
+ Redis缓存怎么解决数据一致性？redis集群用过吗？ 
+ 讲一下Redis 
+ Redis数据结构及其实现
+ Redis跳表  

##### MySQL

+ 手写SQL语句：给出一张表，字段有学号、名字、年龄、性别    

  - 找出最大年龄的人 
  - 找出最大年龄的人有几个 
  - 找出最多年龄人数的年龄

+ MySQL 索引的原理    

  - 对名字、性别、年龄建立组合索引      
    - 哪个字段不适合作索引 
    - 查询名字、年龄会走索引吗？ 

  - 交换链表中的两个节点 
  - 二叉树的层序遍历 

+ 数据库 聚集索引和非聚集索引区别 

+ 一条sql语句是怎么执行的 

+ 隔离级别 一般使用哪种 存在哪些问题 

+ 数据库 单体部署吗？集群有哪些问？主从复制的问题？ 数据不一致怎么解决？？ 

+ MongoDB与MySQL(问的啥不太清楚了) 

+ MySQL的默认隔离等级 

+ MySQL与MongoDB的区别，什么情况适合用mongodb，什么时候适合用MySQL 

+ 数据库用的是什么？MySQL，索引建立过吗？

+ ACID讲一下  

+ 脏读，不可重复读，幻读  

+ MVCC，CAS  

+ ABA问题，解决  

+ 乐观锁，悲观锁，行锁读写锁，表锁    

+ MySQL隔离级别 

+ InnoDB与MyISAM区别 

+ 什么是聚簇索引 

+ MySQL可重复读下如何解决幻读 

+ GAP锁

+ 可重复读与未提交读区别

##### ES 

+ ES原理，倒排索引
+ ES 索引和文档的区别 分片和副本 配置 分片缺失对检索有影响吗 
+ 用过ElasticSearch么 

##### MyBatis 

+ mybatis 分页原理有了解吗？ 不会 。。。
+ mybatis的支持延迟加载吗？ 不了解。。。

##### 设计模式

+ 手写DLC单例模式（突然忘了）      

  - 为什么要DLC？ 
  - 不用 volatile 会怎么样？（不会）

+ 设计模式 命令模式和策略模式。。

+  Java中比较熟悉的设计模式 

  知道的Java设计模式，除了工厂与单例 

##### 框架中间件

+ 还有了解哪些中间件
+ 中间件有用过吗 ZK？kafka？
+ zoo[keep]()er有用过么 
+ RabbitMQ与RocketMQ的区别 
+ 对docker和K8S的了解  
+ 介绍一下 RPC（不会）
+ 分布式消息队列之类的我都没有深入学习，面试官也没问啥 

##### 开放性

感觉面试官层次高了一截，问题也比较发散，而且不太好答，面了一个多小时 

1.  树的遍历 两种方法 计算节点的兄弟节点的差 
2.  大数据 日志 时间最长的10个url mapred 
3.  线程调度 内核态和用户态切换 用户态内的进行线程调度 协程 
4.  了解哪些开发框架 共同点 响应式编程 
5.  BIO NIO Tomcat的作用 
6.  反向代理的作用 静态资源具体怎么处理 
7.  印象深刻的事情 

##### 其他

+ Git中Rebase和Merge区别 
+ Git的内存结构，实现原理 





+ Callable 如何创建线程

  + 将 Callable 对象传递给 FutureTask，创建 FutureTask 对象
  + 将 FutureTask 对象传递给 Thread 类，创建线程实例

+ 线程池的执行原理：新提交一个任务

  + 线程池执行原理

    > 1. 判断运行的线程数量 < corePoolSize，若小于，则创建新线程执行，否则下一步
    > 2. 判断工作队列是否满了，若未满，则将任务加入工作队列，否则下一步
    > 3. 判断运行的线程数量 < maximumPoolSize，若小于，则创建新线程执行，否则下一步
    > 4. 执行拒绝策略

  + 线程池如何复用线程

    > 复用的线程只会从 workQueue 队列中获取任务执行
    >
    > 1. 新任务 submit 时，**无论当前线程池中的线程是否空闲，都会依据 active 的线程的数量判断是否新建新线程。**
    >
    > 2. 若 active 线程的数量达到 corePoolSize，则会尝试将该任务加入 workQueue
    >
    > 3. 此时，**处于 active 的线程，若处于空闲状态，则会从 workQueue 中获取任务执行**
    >
    >    因此，新加入 workQueue 的任务可能被 free 的线程立即执行，让 workQueuue 变空，达到线程复用的目的
    >
    >    若，没有 free 的线程，当工作队列被填满，并且处于 active 的线程的数量达到 maximum 限制，则会执行拒绝策略。

  + 示例：

    ```java
    package test;

    import java.util.concurrent.*;

    public class Main{
        private static class RunnableTest implements Runnable{
            @Override
            public void run() {
                // System.out.println("---- execute work - " + Thread.currentThread().getId());
                // System.out.println(Thread.currentThread().getName());
                try {
                    // 模拟耗时操作：使得新任务加入时，没有 free 的线程可用，也就不会执行加入 workQueue 的任务
                    Thread.sleep(10000);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }

        public static void main(String[] args) {
            ThreadFactory factory = new ThreadFactory() {
                @Override
                public Thread newThread(Runnable r) {
                    Thread thread = new Thread(r);
                    // thread.setName("lxk-test-thread-" + thread.getId());
                    System.out.println("create thread - " + thread.getId());
                    return thread;
                }
            };
            int corePoolSize = 5;
            int maximumPoolSize = 10;
            BlockingQueue workerQueue = new ArrayBlockingQueue<>(1);
            long timeout = 1;
            ExecutorService threadPool = new ThreadPoolExecutor(corePoolSize, maximumPoolSize, timeout, TimeUnit.MINUTES, workerQueue, factory);
            for(int i = 0; i < 3; ++i){
                System.out.println("第 " + (i + 1) + " 阶段");
                for (int j = 0; j < 6; j++) {
                    threadPool.submit(new RunnableTest());
                }
                try {
                    Thread.sleep(10);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
                System.out.println();
            }
        }
    }
    /*
    第 1 阶段
    create thread - 11
    create thread - 12
    create thread - 13
    create thread - 14
    create thread - 15

    第 2 阶段
    create thread - 16
    create thread - 17
    create thread - 18
    create thread - 19
    create thread - 20

    Exception in thread "main" java.util.concurrent.RejectedExecutionException: Task java.util.concurrent.FutureTask@36baf30c rejected from java.util.concurrent.ThreadPoolExecutor@7a81197d[Running, pool size = 10, active threads = 10, queued tasks = 1, completed tasks = 0]

    可见：第二个阶段中，最后一个任务执行了拒绝策略，因为，有 10 个线程处理耗时的任务，另一个任务被加入到 workQueue 中，整个线程池只能够被消化 11 个任务
    */
    ```

    ​

+ Spring 事务传递，如何验证当前使用的哪种传递

+ Spring 和 servlet 的区别，SpringMVC 和 servlet 的区别、tomcat 中如何实现多应用共存

+ jdbc 中使用到了 策略模式吗？

+ 算法：两个栈实现一个队列

+ dubbo 中的监控中心使用的是哪个组件？



+ 多码代码：细心

+ Java 的发展多了解

+ Spring 需要深挖一下，Spring 与 SpringBoot 区别，Spring 的优点

+ ORM 框架，中 MyBatis 如何实现行级锁

  Hibernate 有了解过嘛

  JDBC Template、Hibernate、MyBatis 各自的优缺点

+ 反射，反射慢在哪儿？






##### 加密算法

- [七种常见的加密算法](https://juejin.im/post/6844903638117122056)
- [JWT 签名算法中 HS256 和 RS 256 的区别](https://www.jianshu.com/p/cba0dfe4ad4a)
- [HMAC 加密算法](https://www.jianshu.com/p/35630d32b3e7)
- [抓包工具能够获取 https 数据，所以 https 并不安全](https://learnku.com/articles/19238)
- [HTTPS 能够防止中间人篡改内容吗](https://www.zhihu.com/question/65464646)
- [网络抓包原理](https://www.jianshu.com/p/03b30c8e9117)
- [黑客抓包原理](http://www.jeepxie.net/article/75737.html)
- [网络安全之数据监听](https://www.jianshu.com/p/14c9a4294c31)
- [WEB 安全之 CSRF](https://www.jianshu.com/p/855395f9603b)






































