

* 1.JAVA程序基础
  *  1.1 GC(垃圾回收机制)的实现方式
  *  1.2 新建进程的三种方法
  *  1.3 抽象类与接口的区别
  *  1.4 单例模式有哪几种？写出其中的一种
* 2.操作系统
 * 1.进程间通信的几种方式
 * 2.将程序后台运行的方法
* 3.计算机网络基础
 * 3.1 三次握手协议
 * 3.2 [HTTP协议请求的几种方式](#HTTP协议请求的几种方式) 
 * 3.3 网络下一跳地址的配置
 *  4.数据库及数据分析
* 5.软件测试与测试开发
 * 5.1 如何对微信红包流程进行测试？(没有标准答案，自由发挥)
 * 5.2 安卓手机上，手势开锁的测试方法与流程 (没有标准答案，自由发挥)
 * [5.3 A/B Test的含义，A/B Test的几种实现策略.](#3.a/btest的含义,a/btest的几种实现策略)
 
 
 
 
 
 (注：在此md中，只是列出一些知识点，以作后续复习参考，时间精力有限，并没有对知识点进行仔细归纳，考参考书籍或网址进行知识点归纳)
 
***
#1.JAVA程序基础
###1.1 GC(垃圾回收机制)的实现方式
垃圾回收机制有两种实现方法 System.gc()方法和 finalize()方法。算法有几种。可参考《深入理解Java虚拟机》这本书

详情参考：http://jayfeng.com/2016/03/11/%E7%90%86%E8%A7%A3Java%E5%9E%83%E5%9C%BE%E5%9B%9E%E6%94%B6%E6%9C%BA%E5%88%B6/
###1.2 新建进程的三种方法
掌握新建进程的三种方法后，还要研究一下进程同步：

详情参考：http://wiki.jikexueyuan.com/project/java-enhancement/java-five.html
###1.3 抽象类与接口的区别

详情参考：http://wiki.jikexueyuan.com/project/java-enhancement/java-five.html

###1.4 单例模式有哪几种？写出其中的一种
单例模式（Singleton）是几个创建模式中最对立的一个，它的主要特点不是根据用户程序调用生成一个新的实例，而是控制某个类型的实例唯一性，通过上图我们知道它包含的角色只有一个，就是Singleton，它拥有一个私有构造函数，这确保用户无法通过new直接实例它。除此之外，该模式中包含一个静态私有成员变量instance与静态公有方法Instance()。Instance()方法负责检验并实例化自己，然后存储在静态成员变量中，以确保只有一个实例被创建。

详情参考：http://www.cnblogs.com/rush/archive/2011/10/30/2229565.html





###HTTP协议请求的几种方式
HTTP协议中共定义了八种方法或者叫“动作”来表明对Request-URI指定的资源的不同操作方式.

详情可参考：http://blog.csdn.net/zhu_xun/article/details/16939691 


###<span name="3.a/btest的含义,a/btest的几种实现策略">3.A/BTest的含义,A/B Test的几种实现策略</span>
ABtest就是通过特定的标记对流量进行切分（多数是通过hash），根据切分的结果和实验流量的配比来决定打上那个流量标签。 
然后根据流量标签来确定走哪个逻辑分支，这样子就可以在同一套系统上，进行不同的策略实验。
 * http://www.liuxingshe.com/qt/1199906.html
 * http://www.aliued.cn/2010/09/27/ab-testing-realization-method.html

 
