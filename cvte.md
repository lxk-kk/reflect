#### 选择题

1. AVL树相关的，比如高度之类的
2. gc方面的，我记得有个选项是说调用System.gc()之后会不会同步gc（gc什么时候回收对象）（x3）
3. 标记清除算法
4. 数据库判断语法错误,我记得是having错了
5. volatile、automic等知识
6. JVM的OutOfMemoryError可能是什么导致的（选项有堆，栈，PermGen space，线程太多）
7. 强引用、弱引用、软引用、虚引用区别（Java引用）（x2）
8. 一道关于计算www.cvte.com字符串中的非空子串构成的二叉树节点有多少层
9. 可能导致数据库幻读的隔离级别有哪些
10. Java8新特性（x2）
11. 泛型
12. 类加载
13. ArrayList 扩容次数（扩容机制）（x2）
14. Java IO（File；数据类型读写采用DataInputStream、DataOutputStream？；BufferReader）
15. 链表的特点
16. synchronized公平？可重入?
17. HashMap（包括线程安全性等）
18. ThreadLocal机制多线程实现线程安全？
19. JVM，内存回收策略（年代阈值；Full GC；MinorGC）
20. 数据库相关判断
21. 索引使用B树/变种B+树实现
22. 完整性约束的例子
23. Socket；UDP
24. 数据库范式（xx范式消除除非主属性对键的部分/传递函数的依赖）
25. 最小堆插入排序
26. 空指针异常的判断
27. TCP/IP参考模型不包括什么层
28. HTTP方法有些什么
29. sleep()，wait()用法，捕获异常（notify()、notifyall()）
30. Java8 Optional类
31. https 安全问题
32. hash表拉链法平均访问次数
33. 给出一张图，求图的深度或者广度遍历有多少种可能
34. 类加载什么时候final static 的成员变量什么时候赋值了
35. Integer 常量池 -128到127
36. 储存过程 预编译sql
37. arrays.asList是否使用了适配器模式
38. java语法（String.length()）：空字符串在那种操作下会报异常、集合数据结构的实现
39. 数据结构：二叉树（遍历顺序）、堆、huffman树。
40. JVM参数
41. java8 新特性
42. 连通图
43. 回溯法
44. CMS垃圾回收
45. 数据库的事务和幻读
46. http请求信息
47. tcp的三次握手与四次挥手
48. volatile与synchronized
49. 集合

#### 编程题：

1. 对5位数加密，加密规则忘了，但是输入的5位数不能够超过3位是连续的。

2. 最小编辑距离的问题。例如：输入abcd abcde 则输出1

3. 找出超过半数的生日月份

4. 解码方式，1—A 2—B…26—Z，给定字符串，问有多少种解码的方式（如：12——2种【1，2】或【12】，56——1种【5，6】） 【 leetcode上的题】

5. 给一个整型数组，求其中出现频率大于总个数的1/3的元素列表【剑指offer是求总数个数大于1/2的元素，变形题】

6. 合并有序数组，找到第k大数

7. 合并以降序排序好的数组，保持降序（x2）

   [答案1](https://blog.csdn.net/qq_38294937/article/details/81165069)

   [答案2](https://blog.csdn.net/zxl_Dragon/article/details/81139828)

8. 模拟200天服药过程（一次半片，盒子里面有100片。拿出半片吃掉，拿出一片分半扔回去)

9. 给定N*N的矩阵M，如果M[i][j]=1，表示已知第i个和j个小伙伴互为合作同事关系，否则不知道，要求输出所有小伙伴中的已知的事业部总数。（x2）
   示例1：
   输入：
   [[1,1,0]
   [1,1,0]
   [0,0,1]]
   输出：2
   说明：已知小伙伴0和小伙伴1护卫合作方同事，他们在一个事业部。
   第二个学生自己在一个事业部，所以返回2
   注意：
   N在[1,200]范围内
   对于所有小伙伴，有M[i][i]=1,如果有M[i][j]=1,则有M[j][i]=1

10. CVTE最近组织了一场趣味知识竞赛，由于场地大小，参赛者被分到两个场地分别进行比赛，活动结束后，组织者小明却犯愁了，两个场地参赛者是分开进行排名的，现在需要把这两组有序的分数排名合并成一个总的排名表，于是小明求助于WEB的同时小张编写一个排名算法实现。假如你是小张，你会如何设计这个算法。

    样例：

    两组的分数排名分别为：[99, 92, 87, 80] [98, 90, 82]

    汇总得到的排名结果：[99, 98, 92, 90, 87, 82, 80]

    [答案](https://blog.csdn.net/m0_37135421/article/details/81318175)

11. CVTE某后台项目组需要设计一个ID生成器，每次生成一个与之前不重复的，长度为4的字符串，该字符串是由字符0—9、a—z、A—Z组成。现给定一个用于返回累计生成过的ID总数的方法getTotal()，试编程实现ID生成方法generate()。（x4）

    [答案1](https://blog.csdn.net/m0_37135421/article/details/81318175)

    [答案2](https://blog.csdn.net/qq_38294937/article/details/81165069)

    [答案3](https://blog.csdn.net/zxl_Dragon/article/details/81139828)

10. CVTE的笔试题目：
    要求在数组 A [ 1 00 ］中按输入的范围表达式求和”表示从 m 到末尾 : m ·函数实现累加功能支梯浓口卞 2 种字符侧覃表示符，
    " n : m " ”表示从n到 m , " :m  ”表示从 o 到 m ,
    "m:"表示从m-99;
    char range1[17] = “3:7,9,45,2,77:78”;
    即 93 + 4 + 5 +6 + 7 + 9 + 45 + 2 + 77 + 78+79)
    char range2[10] = “:3,50,97:”;
    1 + 2 + 3 + 50 + 97 + 98 + 99 )
    写出求和函数：
    int Sum ( char ＊ ange )
    [答案](https://blog.csdn.net/lovexlsforever/article/details/100864913)
11. 题目：给定一个int数组A，实现一个函数判断输入的数组能否被分成2个平均值的非空数组，如果能则返回true，否则返回false。
    样例：
    A = [1, 2, 3, 4]    true
    A = [0, 0, 6, 2]    true
    A = [1, 2]            false
    [答案](https://blog.csdn.net/qazbaby/article/details/88903877)
12. 有100个饼干，每次吃一半，有多少种吃法？
13. 给一个只有数字的字符串，解密，1-27对应a-z比如123有三种方式，abc,或者kc,或者av；对应1，2，3；或者12，3；或者1，23；求给定字符串的明文数量

#### 设计题：

1. 这是一个高并发的问题，题目大概意思是有两台服务器，在晚上11点访问量超级大，其余时间很空闲，不用扩容，设计一个限流交易系统，让多余的请求排队或者直接抛弃

2. 设计一个物资管理系统，开放式问题

3. 背景：一个点餐系统，由一个应用服务器和一个数据库服务器组撑。当收到前端的订单请求，后台要直接将数据保存到一张订单表中，订单的状态包含：待付款（等待顾客付款）、已接单（店家已经接单）、已完成（顾客点的菜品已全部上完）
   问题：经过一年多的发展，目前订单表的数据已经鸡肋了100多万条，当用户下单的时候，数据库经常出现查询慢和死锁的情况。请问除了升级和增加服务器之外， 我们还可以有那些优化的方案？

4. 说他们公司有很多部门，每个部门负责不同的业务，如短信推送业务、验证码业务、人脸识别业务等等。
   现在要求设计一个公共管理平台，将这些业务整合到一起，这样外界可以通过这个平台调用公司的各项业务，要求考虑安全方面等。【我是以dubbo微服务，暴露在zookeeper，然后zookeeper统一入口，把消费者生产者分离这个角度答的，因为最近项目刚好用到，不知道对不对】

5. 最后一个设计题比较外放，题目是：学校有几个信息系统，但现在需要开发一款校园移动信息系统。

   使用webService改造原有的信息系统，开放几个数据接口，新系统调用接口获取数据

#### 面试：

+ 场景设计题:
  + 设计一个学生选课系统。（画了ER图，写出几个表大概的字段，很久没用有些地方有小bug）

+ 数据库索引（包括底层数据结构的讲解，聚集索引，非聚集索引，主键索引，唯一索引），索引使用场景、索引失效（范例）、底层实现（b+树）绘制结构、索引种类（x6）
+ 事务的隔离级别

+ 数据库三大范式的理解（x2）

+ 你所了解的集合框架

+ 讲讲hashmap，结构，扩容（x2）

+ arraylist与linkedlist的区别，以及插入，删除，查询时间复杂度比较（x4）
+ spring框架的特点
+ jvm：构成

+ spring IOC的理解

+ TCP与UDP的理解以及区别

+ UDP为什么不保证可靠连接

+ HTTP状态码五种大类型的区分，以及301、302、304、500等状态码
+ 线程的几种状态和切换：能从阻塞直接到死亡吗？（x2）
+ 线程池
+ 线程安全的几种手段
+ 创建线程的方式
+ Java GC的几种算法（x2）
+ 死锁的几种条件
+ MyISAM与InnoDB引擎的区别（Mysql了解哪些储存引擎）（x4）
+ Spring和SpringBoot的区别
+ SpringAOP如何实现（采用什么设计模式）（x3）
+ aop里提到了代理，为什么需要代理，原类不能自己做么？这里又扯到动态代理，反射
+ 动态代理的应用?博主说了springmvc主要就是aop和拦截器
+ springmvc执行流程?工作原理？详细问了我HandlerMapper为什么能根据DispatcherServlet传来的参数得到需要的相应的HandlerChain执行链返回给他。（x2）
+ 了解哪些设计模式：写一个单例模式（5中实现方法）（x2）
+ 算法题：
  + 找出0-100的质数
  + 层次遍历二叉树（二叉树遍历）（x2）
  + 倒序字符串
  + 给定一个数组，找出出现次数最多的数，出现次数一样的话，把第一个出现的找出来（2，1，3，2，3  => 2而不是3）
+ Mysql调优，如何优化查询（x2）
+ new String("abc")到底创建了几个对象
+ equals、hashCode关系
+ jvm常量池
+ 如何判断对象不可用
+ 多线程的创建方式（多线程如何实现）（x2）
+ 了解线程池吗？有哪些参数？
+ synchorized关键字、锁、violoate
+ reentrantlock
+ CAS如何实现
+ 多个线程、串行并行如何实现（信号量？）
+ 如何实现一个全局的发号器，考虑分布式场景和性能问题
+ 是否使用过dubbo？RPC原理？
+ ssm那么流行，他们好用在哪里
+ 为什么要面向对象
+ 面向对象的特性：多态、继承、封装
+ 重载和重写
+ hashmap底层实现，如何解决冲突
+ 线程安全的HashMap？hashtable、concurrentHashMap、synchorizedMap? 以及各自具体的实现？
+ 熟悉的排序算法：手写排序
+ 二分查找、冒泡查找选哪个？
+ 项目的异步处理如何实现

------- 已摘录 --------

[**2019秋招 | CVTE线上笔试（web后台开发）**](https://blog.csdn.net/qq_38666896/article/details/100175689)【已】

[**CVTE java web后台实习生笔试+技术一面总结**](https://blog.csdn.net/u013453787/article/details/88547490)【已】

------- 没有答案 --------

[**实习-笔试-面试整理汇总（一）CVTE篇**](https://blog.nowcoder.net/n/22b033bb6131435fa6d43eb4faf15bbc)【未】

------- 附带答案 --------

[**CVTE面试总结（全网面经，已收offer）**](https://blog.csdn.net/qq_38056704/article/details/88656655)【未】

[**CVTE在线笔试**](https://blog.csdn.net/weixin_40804971/article/details/82629667)【未】

[**CVTE 2017 内推笔试整理**](https://blog.csdn.net/xiao__jia__jia/article/details/82426117)【未】

[**Web后台开发之CVTE的面试经历**](https://blog.csdn.net/weixin_39453325/article/details/82843232)【未】

[**互联网公司校招Java面试题总结及答案——CVTE**](https://blog.csdn.net/d12345678a/article/details/54376798)【未】

[**2016CVTE校招在线笔试题**](https://blog.csdn.net/wwwdc1012/article/details/77887445)【未】

[**CVTE笔试题**](https://blog.csdn.net/obession/article/details/77620282)【未】