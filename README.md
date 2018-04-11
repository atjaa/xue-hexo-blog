一个以hexo为模版的轻量级博客模版
-----------------------
[官方网站](https://hexo.io/docs/setup.html)
#####环境准备：
hexo基于nodejs，因此需要首先具备nodejs环境
install nodejs
cURL:
``` bash
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.2/install.sh | bash
```
> Wget:
``` bash
$ wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.2/install.sh | bash
```
nvm安装好之后，使用nvm安装nodejs，注意，可能需要刷新系统环境变量$source .bashrc
``` bash
$ nvm install stable
```
>安装Hexo
``` bash
$ npm install -g hexo-cli
```
>初始化一个博客工程
``` bash
$ hexo init [folder]
```
创建一篇文章,
文章内容格式
``` bash
layout: photo
title: mytitle
date: 2018-04-10 17:45:50
tags: 标签
categories:
- 一级分类
- 二级分类
---
content
```
``` bash
$ hexo new [layout] <title>
```
启动本地服务，服务地址为http://localhost:4000/，如果要指定端口，使用-p参数
``` bash
$ hexo server
```
