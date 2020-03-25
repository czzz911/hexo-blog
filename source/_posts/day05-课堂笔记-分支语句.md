---
title: day05_课堂笔记(分支语句)
date: 2020-03-21 23:48:42
tags: JavaSE
declare: true
essayending: true
---

生活又不是热血动漫，你也没有主角光环。

<!--more-->

## day05——分支语句

##### 2.1、程序的流程结构

```
程序的流程结构：
A：顺序结构：默认的，从上向下，逐行的执行。
B：选择结构：条件满足，某些代码才会执行。
C：循环结构：条件满足，某些代码会反复多次的执行。直到条件不满足。
```



##### 2.2、if语句

**最基本的if语句**

```java
if(条件：boolean){
	//条件成立，执行此处的代码
}
```

执行流程：

![4if的流程图](if的流程图.png)

**2、if...else语句**

```java
if(条件：boolean){
	//条件成立，执行此处的代码
}else{
	//条件不成立，执行此处的代码
}
```

实现二者必选其一。

```java
//课堂练习2：给定一个性别，如果是男，就去男厕所，否则去女厕所。。
		/*
		思路：
		step1：有个性别这个变量
			boolean true false
			int 1 0 
			char 男 女
			String 男生 女生
		step2：if else语句来实现
			判断条件：



		在比较数值上：
			基本类型：使用==这个运算符进行比较数值，是否相等
				byte，short，int，long，float，double，char，boolean

			引用类型：使用equals()来比较
				String
		*/
```





![6ifelse的流程](ifelse的流程.png)

多个条件：

```java
if(条件1){
	条件1满足，执行此处的代码
}else if(条件2){
	条件1不满足，条件2满足，执行此处的代码
}else if(条件3){
	条件1、2都不满足，条件3满足，执行此处的代码。
}。。。
else{

}
```



![多分支流程图](多分支流程图.png)

if语句的嵌套

```java
if(外层条件){
	if(内层条件){
	
	}else{
	
	}
}else{

}
```



>说明：如果说if语句里只有一行代码，那么{}可以省略不写。但是不建议。



##### 2.3、switch语句

switch也是实现分支语句

```java
switch(变量/表达式){
case 数值1：分支1；break；
case 数值2：分支2；break；
case 数值3：分支3；break；

default：最后一个分支；
}
```



注意点：

1、case后的数值，不能重复。

2、case是无序的，先写后写都可以，关键是是否能够匹配上switch作用的变量。

3、switch作用的变量类型：short，byte，char，int，String。

4、default语句是可选的。

5、某个case匹配上后，如果该分支中没有break，那么后续的case都不再匹配，直接执行。一直到遇到break位置。

##### 2.4 If 和 Switch的比较

**if：**

判断条件：boolean

判断分支少

**switch：**

判断条件：byte，short，int，char，String

​	不支持 float， double，boolean

判断分支多    ：case

