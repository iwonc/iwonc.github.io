---
title: 使用Hexo搭建GitHub Pages博客
date: 2019-04-24 12:55:53
tags: 
- Hexo
- Next
---

使用Hexo搭建GitHub Pages博客过程中的操作记录

<!-- more -->

## 准备工作

### 下载并安装Node.js

官网：https://nodejs.org/en/

### 下载并安装Git

官网：https://git-scm.com/download/

### 安装Hexo

在`cmd`中输入`npm i -g hexo`

## 搭建本地Hexo博客

 - 新建文件夹：本文使用`blog`
 - 生成Hexo模板：在`blog`文件夹中，右键运行`Git Bash Here`，并输入`hexo init`
 - 启动服务：输入`hexo s`
 - 查看效果：在浏览器中输入`http://localhost:4000/`

## 下载并更换主题

### 下载主题

在`Hexo`官网的`Themes`模块，提供多种主题预览及GitHub链接，本文以Next主题为例。

Next主题GitHub主页：https://github.com/theme-next/hexo-theme-next

克隆主题到`blog/themes/next`
```
git clone https://github.com/theme-next/hexo-theme-next.git themes/next
```


### 启用主题

在Hexo的站点配置文件`_config.yml`中，修改`theme`关键字对应的值为`next`
```
theme: next
```

### 主题配置

参见文档

 - Next主题配置文档：http://theme-next.iissnan.com/theme-settings.html

## 创建GitHub Pages

### 创建项目

在GitHub中创建项目，项目名为`github名.github.io`

### 在Hexo中配置部署信息

在Hexo站点配置文件`_config.yml`中，找到`deploy`关键字

```
deploy:
  type: git
  repo: git@github.com:github名/github名.github.io.git
  branch: master
```

### 部署项目

```
hexo g

hexo d
```

## 推荐Hexo主题

 - Hacker [预览](https://blog.daraw.cn/) / [GitHub](https://github.com/CodeDaraW/Hacker)
 - Icarus [预览](https://blog.zhangruipeng.me/hexo-theme-icarus/) / [GitHub](https://github.com/ppoffice/hexo-theme-icarus)
 - Laughing [预览](http://lalala.lol/) / [GitHub](https://github.com/BoizZ/hexo-theme-laughing)
 - Material-X [预览](https://xaoxuu.com/) / [GitHub](https://github.com/xaoxuu/hexo-theme-material-x)
 - Next [预览](https://theme-next.org/) / [GitHub](https://github.com/theme-next/hexo-theme-next)
 - Ocean [预览](https://zhwangart.github.io/) / [GitHub](https://github.com/zhwangart/hexo-theme-ocean)
 - Replica [预览](https://sabrinaluo.github.io/tech/) / [GitHub](https://github.com/sabrinaluo/hexo-theme-replica)
 - landscape [预览](https://hexojs.github.io/hexo-theme-landscape/) / [GitHub](https://github.com/hexojs/hexo-theme-landscape)

