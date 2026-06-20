## Java笔记

---

1.==概述==

定义：java是一种高级语言

特点：简单易学、面向对象编程、平台无关性、安全性、高性能、多线程支持、开源免费

三大版本：javaSE标准版、javaME微型版、javaEE企业版

JVM（Java Virtual Machine），Java虚拟机

JRE（Java Runtime Environment），Java运行环境，包含了JVM和Java的核心类库（Java API）

JDK（Java Development Kit）称为Java开发工具，包含了JRE和开发工具

==命名==

- 必须由数字、字母、下划线_、**美元符号$**组成。
- 数字不能开头
- 不能是关键字
- 区分大小写的。
- 驼峰命名

2.==基本数据类型==

整形类型：byte、short、int、long

浮点数类型：float（定义的适合要加f）、double

字符类型：char

布尔型：boolean

3.==关键词==

==访问修饰符：==public、default、private、protected

==修饰符关键字：==public、protected、private、static（静态）、final（常量）、abstract（抽象）

==类、接口、包、枚举、泛型：==class、interface（接口可以多继承，接口可在主程序创建对象时转化成匿名内部类书写）、enum（枚举）、package、import、extends（继承，只能单继承）、implements（实现接口）、Arraylist<类型>名 = new Arraylist<>();

==方法关键字：==void、return、this(当前)、super（父类）

4.==算数运算符==++，--（重点）

5.==赋值运算符==+=，-=，*=，/=，%=

6.==判断，选择、循环：==if、else if、else、switch-case、for（有确定循环次数）、while（不确定循环次数）、do-while（只循环一次）、break（循环里退出for的小循环）、continue（跳过本次循环，继续执行下次循环）、return（退出整个方法）

7.==静态数组：==数据类型 [] 数组名 = ==new 数据类型（可加可不加）== {元素1，元素2......}

8.==动态数组：==数据类型 [] 数组名 = new 数据类型 [数组长度（数组名.length）]

9.==输入，随机：==scanner、random（0到输入数减一），比如：import  java.util.scanner(导包)

10.==强转：==小到大（自动转）、大到小（手动转）

11.==方法：==继承、封装（私有变量用set、get访问，set设定，get获得）、多态(父类 对象名 = new 子类（）)

==注意==：

abstract创造的子类要写父类所有的方法，而不是abstract的子类就直接继承了父类的方法
abstract只能继承，abstract写的方法在别的方法里必须重写，static是共享，类名方法名调用

---

### API

12.==Object==

- toString（）返回对象的字符串表示形式；
- equals（Object o）比较是否相等；
- clone（）克隆；

13.==Objects==

- equals（）先做非空判断，再比较两个对象
- isNull（）判断对象是否为null、为null返回true，反之
- nonNull（）判断对象是否为null，不为null返回true，反之

14.==StringBulider（线程不安全）和StringBuffer（线程安全）(字符串)==

- append（）添加数据
- reverse（）反转
- toString（）转换成string类型
- length（）返回长度

15.==StringJoiner==

- add（）添加数据
- toString（）返回字符串
- length（）返回长度

16.==Math==

- abs（）绝对值
- ceil（）向上取整
- floor（）向下取整
- round（）四舍五入
- max（）比较两个int值的较大值
- pow（a，b）返回a的b次幂的值
- random（）返回值为double的随机值，范围 [0.0，1.0）

17.==System==

- exit（）终止
- currentTimeMillis（）返回当前系统的时间毫秒值

18.==Runtime==

- Runtime.getRuntime（）返回与当前java应用程序关联的运行对象
- exit（）终止
- availavleProcessors（）返回java虚拟机可用的处理器数
- totalMemory（）返回java虚拟机中的内存总量
- freeMemory（）返回java虚拟机中的可用内存
- exec（String command）启动某个程序，并返回代表该程序的对象

19.==BigDecimal==

- valueof（double val）转换一个double成BigDecimal
- add（BigDeciaml b）加法
- subtract（）减法
- multiply（）乘法
- divide（）除法
- divide（BigDecimal对象，精确几位，舍入模式）
- doubleValue（）将BigDecimal转化为double

20.==Arraylist==

![1](./img/1.png)

![2](./img/2.png)

21.==Date==

![3](./img/3.png)

22.==SimpleDateFormat==![4](./img/4.png)

常见时间格式：![5](./img/5.png)

![6](./img/6.png)

23.==Calendar==

![7](./img/7.png)

24.==LocalDate、LacalTime、LocalDateTime==

![8](./img/8.png)

![9](./img/9.png)

![10](./img/10.png)

![124](./img/124.png)

25.==ZoneId常见方法==

![12](./img/12.png)

![13](./img/13.png)

26.==Instant==

![14](./img/14.png)

27.==Period==

![15](./img/15.png)

28.==Duration(持续时间)==

![16](./img/16.png)

![17](./img/17.png)

29.==compareTo==

![18](./img/18.png)

![19](./img/19.png)

---

### Lambda(正则表达式)

![20](./img/20.png)

![21](./img/21.png)

![22](./img/22.png)

![23](./img/23.png)

![24](./img/24.png)

==正则表达式爬虫==

![25](./img/25.png)

![26](./img/26.png)

---

### 异常

![27](./img/27.png)

![28](./img/28.png)

![29](./img/29.png)

---

### 集合

1.==Collection==

![30](./img/30.png)

![31](./img/31.png)

![32](./img/32.png)

2.==增强for循环==

![33](./img/33.png)

3.==set集合==

![34](./img/34.png)

![35](./img/35.png)

![36](./img/36.png)

![37](./img/37.png)

![38](./img/38.png)

4.==Collections==

![39](./img/39.png)

5.==Map集合==

![40](./img/40.png)

![41](./img/41.png)

![42](./img/42.png)

![43](./img/43.png)

![44](./img/44.png)

6.==Element==

![45](./img/45.png)

![46](./img/46.png)

---

### Stream流

![47](./img/47.png)

![48](./img/48.png)

![49](./img/49.png)

![50](./img/50.png)

![51](./img/51.png)

---

### IO流

![52](./img/52.png)

1.==File==

![53](./img/53.png)

![54](./img/54.png)

![55](./img/55.png)

![56](./img/56.png)

![57](./img/57.png)

![58](./img/58.png)

==输入流==

![59](./img/59.png)

![60](./img/60.png)

![61](./img/61.png)

![62](./img/62.png)

![63](./img/63.png)

![64](./img/64.png)

![65](./img/65.png)

eg：private transient String passWord；//transient这个成员变量不参与序列化

==输出流==

![66](./img/66.png)

![67](./img/67.png)![68](./img/68.png)

![69](./img/69.png)![70](./img/70.png)

![71](./img/71.png)

![72](./img/72.png)

![73](./img/73.png)

2.==Commons-io开源jar==

![74](./img/74.png)

![75](./img/75.png)

---

### 特殊文件

1.==Properties==

![76](./img/76.png)

![77](./img/77.png)

2.==XML的语法规则==

![78](./img/78.png)

3.==Dom4j（jar）==

![79](./img/79.png)

---

### 多线程

==Thread==

==多线程创建方法==

![80](./img/80.png)

![81](./img/81.png)

![82](./img/82.png)

![83](./img/83.png)

==相关方法==

![84](./img/84.png)

==锁（相关）==

![85](./img/85.png)

![86](./img/86.png)

![87](./img/87.png)

![88](./img/88.png)

![89](./img/89.png)![90](./img/90.png)

==ThreadPoolExecutor构造器==

![91](./img/91.png)

![92](./img/92.png)

==ExecutorService常见方法==

![93](./img/93.png)![94](./img/94.png)

![95](./img/95.png)

==线程6种状态==

![96](./img/96.png)

---

### 网络通信

==CS架构==

![97](./img/97.png)

==BS架构==

![98](./img/98.png)

![99](./img/99.png)

![100](./img/100.png)

==网络通信知识点==

![101](./img/101.png)

![102](./img/102.png)

![103](./img/103.png)

![104](./img/104.png)

![105](./img/105.png)

![106](./img/106.png)

==TCP三次握手==

![107](./img/107.png)

==UDP和TCP==

![108](./img/108.png)

![109](./img/109.png)

![110](./img/110.png)

==DatagramSocket==

![111](./img/111.png)

---

### Java高级

==Junit（自带jar）==

![112](./img/12.png)

![113](./img/113.png)

==class==

![114](./img/114.png)

![115](./img/115.png)

![116](./img/116.png)

![117](./img/117.png)

==自定义注释==

![118](./img/118.png)

==元注释==

![119](./img/119.png)

==解析注解==

![120](./img/120.png)

==创建代理人==

![121](./img/121.png)

![122](./img/122.png)

![123](./img/123.png)