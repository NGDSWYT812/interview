#Android基础面试（一面）和技术面试（二面）知识要点
author：王宇滔

date  ：2018


##基本功
* **面向对象的特征**
	* 封装 继承 多态 抽象 

* final, finally, finalize 关键字

* int 和 integer 区别，对自动装箱&自动拆箱的考察

* 重载和重写的区别

* 抽象类的作用，接口的作用

* 抽象类和接口区别

* 注解的本质，枚举的本质

* Object 内的方法考察：equals wait notify notifyAll finalize hashCode

反射的用途及实现

##集合
* List 和 Set 区别

* List 和 Map 区别

* **Arraylist 与 LinkedList 区别 （提示：for 循环 和 foreach 循环的区别）**

* ArrayList 与 Vector 区别 

* HashMap 和 Hashtable 的区别

* HashSet 和 HashMap 区别

* HashMap 和 ConcurrentHashMap 的区别

* **HashMap 的工作原理及代码实现**

* ConcurrentHashMap 的工作原理及代码实现

##计算机网络
* **TCP 握手过程（为什么要三次握手）**

* **TCP 挥手过程（为什么要四次挥手）**

* SSL 协议握手过程

* **网络层 TCP UDP 协议的区别**

* HTTP 请求的 GET 与 POST 方式的区别

* POST 请求 POST 提交 大&小 文件时的区别

##jvm/dvm虚拟机
* vm的线程模型

* vm内存模型

* **垃圾回收机制**

* 堆栈知识点的考察 ：堆栈的区别 堆溢出 栈溢出 

* **类加载机制： 加载步骤 双亲委派机制考察**

##线程
* 创建线程的方式及实现

* sleep() 、join（）、yield（）等方法

* **ThreadLocal 原理分析**

* 讲讲线程池的实现原理

* 线程池的几种默认实现（ThreadPoolExecutor）

* 线程的生命周期

##锁机制
* 说说线程安全问题

* volatile 含义&实现原理

* **synchronize 使用场景&实现原理**

* synchronized 与 lock 的区别

* CAS 乐观锁

* ABA 问题

##Android零碎相关
* **view的绘制流程：**
	* Measure Layout Draw方法的考察
	* 不同 ViewGroup 性能上的区别（比如相对布局会多次measure）
	* MeasureSpec的考察

* **setContentView 之后直到 view展示 发生了哪些事情**

* **事件分发流程：**
	* dispatchTouchEvent
	* onInterceptTouchEvent 
	* onTouch

* **Android中ipc的方式：**</br>
	通常binder重点考察，考察 binder.stub  binder.proxy 的区别和使用者；
	有些面试官会深入考察 bnbinder 和 bpbinder ；通过对binder的考察，面试官会知道你的知识深度大概在什么水平；
	* **binder**
	* intent
	* provider
	* brocast
	* socket
	* messager
	* file
	
* **ActivityThread** </br>
	这个知识点有大量的知识可以展开，面试关于这个知识点的展开如下：
	* 说一说 app 是怎么启动的
	
	* 为什么只有ui线程可以更新ui
		* view的实现是线程不安全的
		
	* Handler Looper msgqueue机制 
		* ThreadLocal 实现
			* arrayMap实现的
			* arrayMap和hashmap的区别
		* memoryleak 的考察；leakcanry 原理

	* **为什么ui线程的Looper.loop开始后，在queue中没有msg死循环的情况下，cpu不会100%**（epoll+pip）
		
* ApplicationThread
	* 与 ActivityThread 的关系
	* ApplicationThread的实质

* Fragment缓存机制

* 图片加载框架fresco glide picaso 区别

* rgb几种图片格式的区别
	* rgb8888 rgb565 之类的
	* 这些不同的图片格式占的内存分别是多少
	
* retrofit okhttp等框架的考察，主要是设计思维和设计模式
	* retrofit 动态代理等
	* okhttp 责任链等	 

	







