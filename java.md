## Java笔记

---

1.概述

定义：java是一种高级语言

特点：简单易学、面向对象编程、平台无关性、安全性、高性能、多线程支持、开源免费

三大版本：javaSE标准版、javaME微型版、javaEE企业版

JVM（Java Virtual Machine），Java虚拟机

JRE（Java Runtime Environment），Java运行环境，包含了JVM和Java的核心类库（Java API）

JDK（Java Development Kit）称为Java开发工具，包含了JRE和开发工具

==命名：==

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

==类、接口、包、枚举、泛型：==class、interface（接口可以多继承）、enum（枚举）、package、import、extends（继承，只能单继承）、implements（实现接口）、Arraylist<类型>名 = new Arraylist<>();

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

12.==Object：==

- toString（）返回对象的字符串表示形式；
- equals（Object o）比较是否相等；
- clone（）克隆；

13.==Objects：==

- equals（）先做非空判断，再比较两个对象
- isNull（）判断对象是否为null、为null返回true，反之
- nonNull（）判断对象是否为null，不为null返回true，反之

14.==StringBulider（线程不安全）和StringBuffer（线程安全）(字符串):==

- append（）添加数据
- reverse（）反转
- toString（）转换成string类型
- length（）返回长度

15.==StringJoiner：==

- add（）添加数据
- toString（）返回字符串
- length（）返回长度

16.==Math：==

- abs（）绝对值
- ceil（）向上取整
- floor（）向下取整
- round（）四舍五入
- max（）比较两个int值的较大值
- pow（a，b）返回a的b次幂的值
- random（）返回值为double的随机值，范围 [0.0，1.0）

17.==System：==

- exit（）终止
- currentTimeMillis（）返回当前系统的时间毫秒值

18.==Runtime：==

- Runtime.getRuntime（）返回与当前java应用程序关联的运行对象
- exit（）终止
- availavleProcessors（）返回java虚拟机可用的处理器数
- totalMemory（）返回java虚拟机中的内存总量
- freeMemory（）返回java虚拟机中的可用内存
- exec（String command）启动某个程序，并返回代表该程序的对象

19.==BigDecimal:==

- valueof（double val）转换一个double成BigDecimal
- add（BigDeciaml b）加法
- subtract（）减法
- multiply（）乘法
- divide（）除法
- divide（BigDecimal对象，精确几位，舍入模式）
- doubleValue（）将BigDecimal转化为double

20.==Arraylist：==

![屏幕截图 2025-12-07 232136](图片/屏幕截图 2025-12-07 232136.png)

21.