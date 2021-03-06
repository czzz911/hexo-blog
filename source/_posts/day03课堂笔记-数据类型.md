---
title: day03课堂笔记(数据类型)
date: 2020-03-18 21:40:57
tags: JavaSE
declare: true
essayending: true
---

业余生活要有意义，不要越轨。——华盛顿<!--more-->

## day03——数据类型

### 一、本节课内容

##### 1.1、变量

概念：内存中的一小块空间，用于数据的存储。该变量的数值，在程序的执行过程中，可以改变。

三要素：数据类型	变量名  数值

A：定义变量的语法形式：

```
//1.先声明，再赋值
数据类型 变量名;
变量名 = 数值;
//2.声明和赋值写一起
数据类型 变量名 = 数值;
//3.多个变量统一声明，就是写在一起声明：同种类型
数据类型 变量名1，变量名2，变量名;
```

B：变量的注意点：

```
1、变量必须先定义，才能使用
2、变量名不能冲突，同一个作用域内。
3、目前所学的变量：先初始化，再使用。
```



##### 1.2、数据类型

Java中的数据类型：基本数据类型和引用数据类型。

Java语言是强类型语言：对数据类型的要求很严格。**声明是什么类型的变量，就要存储什么类型的数值。**

基本数据类型：4类8种

###### 整数型

- byte，字节，1个字节，8bit，-128~127
- short，短整形，2个字节，16bit，-32768~32767
- int，**默认类型**，4个字节，32bit，-2147483648~2147483647
- long，长整形，8个字节，64bit，9223372036854775807L
  - 在声明long类型的时候，数值后加L或l。建议L。

###### 浮点型

就是生活中的小数

- float类型：4个字节，32bit，定义变量的时候，数值后加f，或F

  float f = 3.14f;

- double类型：8个字节，64bit，**默认类型**



科学计数法：3.4E38

3.4

E1,10的1次方-->10

E2,10的平方-->100

E3,10的立方-->1000

E38,10的38次方-->10000000000...





二进制：0,1,逢二进一。

0

1

10--->2

11--->3

100-->4

...

十进制：0,1,2....9，逢十进一

9

10



A：

###### 布尔类型

boolean类型：取值只有两个，true(对，真)，false(错，假)，



###### 字符型

char，表示单个的字符，使用单引号引起来的，但本质上是个数值，因为对应的字符编码值。

Java语言采用的字符集：Unicode编码。

赋值方式一：通过''引起来的字符：'A'-->65

赋值方式二：通过编码值进行赋值：10进制的编码值，16进制的unicode编码。



##### 1.3、引用数据类型

引用类型：String，用于表示一个字符序列。使用双引号引起来的都是字符串的内容

```
双引号引起来的字符序列：
"abc","helloworld","   王二狗"
```



4类8种：

```
整数型：4种
byte，short，int(默认)，long，加L
浮点型：2种
float加F，double(默认)
字符型：
char：单引号引起来的单个字符，对应的是编码表中的编码值：0-65535。
	转义字符：\，将字符进行转义
		A：有特殊作用的字符，转为普通的字符
				\;,\",\\
		B：普通的字符，转为有特殊作用的字符
				\t,\n
65：A，97：a

boolean，布尔类型，true，false
引用数据类型：
	String：字符串，使用双引号引起来的0-多个字符
		"","a","abc","helloworld","   haha"
	其他
```



##### 1.4、转义字符：

```
转义字符：将字符进行转义-->语法上使用\
			1、将有特殊作用的字符，转为普通的字符，不再起作用
				\',\",\\
			2、还可以将一些普通的字符，转为有特殊含义的作用
				\n,\t
```



##### 1.5、数据类型的转换

Java这门语言，虽然是强类型语言：要求数据类型一致。
		但是实际上允许我们在一定程度上可以转换：

		自动转换：
			A：两种类型兼容
			B：目标类型的取值范围  大于 源类型取值范围
		强制转换：
			A：两种类型兼容
			B：目标类型的取值范围	小于 源类型的取值范围
	
			需要加强制转换符的语法：说明要强制转为哪种类型
					(要转换的类型)数值
	
		取值范围：
			byte-->short-->int-->long-->float-->double
			char：2个字节。单个字符，使用单引号引起来的。对应了Unicode编码。
				A：65，B：66，C：67.。。Z：90
				a：97，b：98，c：99.。。z：122
				0-65535
							转义字符：\
					A：普通字符-->有特殊的作用
						\t,\n
					B：有特殊的作用-->普通字符
						\',\",\\
		布尔型：
			boolean：true，false
			引用数据类型：
		String：字符串，使用双引号引起来的0-多个字符
			"","a","abc","helloworld","   haha"
		其他

类型转换：

- 自动转换：类型兼容，取值范围小-->取值范围大。

- 强制转换：类型兼容，取值范围大-->取值范围小。数据可能不安全，就需要强制转换
  - (要转的类型)数值

boolean 类型不参加这些数值方面的转换



```
自动类型转换：
	A：类型兼容
	B：目标的取值范围大于源数据的取值范围：short-->int
	
强制类型转换：
	A：类型兼容
	B：目标的取值范围 小于 源数据的取值范围：int --> short
		int i = 100;
		short s = (short)i;
```

