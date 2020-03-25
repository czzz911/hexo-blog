---
title: hexo搭建自己的博客
date: 2020-03-2 21:52:18
tags: 简易搭建博客...
declare: true
essayending: true
---

生活不是热血动漫，确是独一无二的自传<!--more-->

## node.js

官网下载安装

安装包 打包下载了npm安装下载

node -v	查看node版本

npm -v 	查看npm版本

## 安装hexo-cli

cnpm install  -g hexo-cli

进行全局安装hexo框架

hexo -v	查看hexo版本及各项依赖版本

## 初始化

新建bolg文件夹

在文件下进行hexo初始化

hexo init

## hexo命令

### 1、启动

hexo s				hexo server

默认设置访问端口号为4000

### 2、创建一篇名称为myblog的不可

hexo n "myblog"

## 部署当github上

### 1、创建一个新仓库

名称要与用户名一致

例: czzz911.github.io

### 2、在blog目录下装一个Git的部署插件

cnpm install --save hexo-deployer-git

### 3、设置_config.yml配置文件

在blog文件夹下，找到_config.yml文件，并打开。

在最下面找到 deploy 属性

进行设置

>deploy:
>type: 'git'
>repo: 'https://github.com/czzz911/czzz911.github.io.git'
>branch: 'master'

### 4、hexo clean

Deleled database

Deleted public folder

### 5、 hexo generate

Generate static files

### 6、推送博客到github上

hexo deploy

### 7、打开部署的博客

把仓库名称复制，在地址栏打开，即可。

## 博客文件

在blog.source._post下

## 主题设置

克隆hexo主题，以yilia为例，将其放入theme文件夹中

在_config.yml配置文件中设置theme属性

> theme: yilia









  







