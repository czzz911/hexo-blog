---
title: day01课堂笔记
date: 2020-03-16 20:21:09
tags: JavaSE
declare: true
essayending: true
---

如果你浪费了自己的年龄，那是挺可悲的。因为你的青春只能持续一点儿时间——很短的一点儿时间。——王尔德<!--more-->

## day01——课堂笔记

### 一、Java的历史

1、Java的由来

Java之父：James Gosling，高司令

![JamesGosling](JamesGosling.jpg)

2、Java的各种版本

​		1995年推出JDK1.0

​		JDK8.0



3、Java的三大体系

​	A：JavaSE，Java Platform Standard Edition(Java平台标准版)

​	B：JavaEE，Java Platform Enterprise Edition(Java平台企业版)，企业级开发

​	C：JavaME，Java Platform Micro Edition(Java平台微小版)

![java的分支](java的分支.png)

### 二、Java的特点

1、纯面向对象

2、简单性

3、跨平台：靠JVM



### 三、Java的运行机制

程序的执行：

1、解释执行：将源文件一行一行解释，一行一行执行。不同的操作系统具备不同的解释器。

​		执行效率低。跨平台。

​	python，JavaScript。。。

2、编译执行：将源文件编译成机器码文件，一次编译。多次执行。

​		执行效率高。不可跨平台。

​	C，C++

![跨平台](跨平台.png)

**Java的执行步骤：**

step1：编写Java源代码：(程序员干的，就是你)，后缀是.java的文件

step2：需要编译器进行编译：产生字节码文件，后缀是.class的文件

step3：解释执行字节码文件。



理念：一次编译，到处执行。



![Java的名词](Java的名词.png)

### 四、Java环境搭建

1、安装JDK-->版本是8.0版本

​	默认安装的位置：C:\Programe Files\Java

​		bin目录：存放java的可执行文件，编译器，街十字等工具

​		db目录：java自带的一个小型数据库

​		include目录：存放用于本地方法的一些文件

​		lib目录：存放的是java的一些类库文件。

​		src.zip：JDK提供的类的源代码。

2、配置环境变量

​	当使用dos窗口执行某个命令的时候，默认在当前目录下查找。找到了就执行。如果没有，那么就找path目录下的路径。

​	A：新建：JAVA_HOME

​			变量名：JAVA_HOME

​			变量值：C:\Program Files\Java\jdk1.8.0_77

​			说明：就是jdk的安装目录

​	B：新建：CLASSPATH

​			变量名：CLASSPATH

​			变量值：.

​			说明：.代表的是当前的目录

​	C：修改：path

​			变量名：path

​			变量值：C:\Program Files\Java\jdk1.8.0_77\bin

​					%JAVA_HOME%\bin

​			注意事项：path下其他的软件的目录不要删，只要添加jdk的bin目录就可以了的

具体的操作：

第一步：我的电脑，右键选择属性

![配置环境变量1](配置环境变量1.png)



step2：左侧栏选择：高级系统变量

![配置环境变量2](配置环境变量2.png)



第三步：选择高级-->环境变量

![配置环境变量3](配置环境变量3.png)



第四步：添加JAVA_HOME

![配置环境变量4](配置环境变量4.png)



第五步：添加CLASSPATH变量

![配置环境变量5](配置环境变量5.png)

第六步：修改path的值，添加javac等命令所在的bin目录。

![配置环境变量](配置环境变量.png)



第七步：重启dos窗口。

最后可以使用：

```
java -version
这个命令来检查当前电脑上安装的jdk的版本。
```



3、安装开发工具





程序的执行：

dos命令：打开dos窗口。

​	方式一：开始|程序|系统|命令提示符

​	方式二：快捷键：win+R，输入cmd(Command命令)



dos命令：

​	1、切换盘符，c:，回车

​	2、显示该文件夹下的所有内容：dir

​	3、退回到上一层：cd ..

​	4、直接退回到根目录：cd \

​	5、进入一个目录：cd 文件夹的名字

​		





图形界面：windows



