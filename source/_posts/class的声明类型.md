---
title: class的声明类型
date: 2020-03-23 20:39:55
tags: JavaSE
declare: true
essayending: true
---

7岁到17岁全是期待，而17岁到27岁满是心酸皆是遗憾。

<!--more-->

# java中的类如果不标明是public或private类，默认是什么？

默认的是default 不需要书写

public： [Java语言](https://www.baidu.com/s?wd=Java语言&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)中访问限制最宽的修饰符，一般称之为“公共的”。被其修饰的类、属性以及方法不
　　　　　仅可以跨类访问，而且允许跨包（package）访问。
private: [Java语言](https://www.baidu.com/s?wd=Java语言&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)中对[访问权限](https://www.baidu.com/s?wd=访问权限&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)限制的最窄的修饰符，一般称之为“私有的”。被其修饰的类、属性以
　　　　　及方法只能被该类的对象访问，其子类不能访问，更不能允许跨包访问。
protect: 介于public 和 private 之间的一种访问修饰符，一般称之为“保护形”。被其修饰的类、
　　　　　属性以及方法只能被类本身的方法及子类访问，即使子类在不同的包中也可以访问。
default：即不加任何访问修饰符，通常称为“默认访问模式“。该模式下，只允许在同一个包中进行访问。