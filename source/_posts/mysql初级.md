---
title: mysql初级
date: 2024-09-06 23:33:06
tags:
    -教程
    -MySQL
    -初级
---
<!-- ## 目录：

MySQL概述

sql

函数

约束

多表查询

事务

*** -->

## MySQL概述

什么是数据库？

数据库就是用在组织、管理和存储数据的仓库。我们如今生活的世界是由数据所充满的互联网世界，音频、图片、文字这些都是数据。这些数据种类繁多，来源也多种多样，因此**数据库管理系统**孕育而生。数据库管理系统也被我们常称为数据库，虽然两者并不是一个东西。SQL语句就是当今数据管理系统的标准语句。

## MySQL下载链接

链接:https://caiyun.139.com/m/i?145CGGExR9vGM
提取码:mS4h

## 安装步骤

1. 安装界面连续两次Next
2. 出现三个选择Typical（推荐）Custom（自定义）Complete（完整安装）。这里我们选择第一个Typical
3. 选择数据存放位置，需要到资源管理器中自建，之后复制地址。**注意要是全英文地址，以防出现问题**。
4. 之后一直默认next，直到出现设置密码界面，密码要牢记（学习建议用admin或123456）
5. 接下来一直next即可，直到遇到next变灰色，选择执行按钮，等全部变绿即可，继续next。
6. 大功告成！

## ~~修改数据库data存放位置（可选）~~

~~这一步的主要目的就是在我们安装的时候是没有办法更改数据库data的存放位置的，且默认位置为C盘。这样就会用久了之后C盘会出现爆红的情况，所以如果需要的话建议修改。~~

1. ~~进入windows服务界面~~
   
   ~~`win+r `~~
   
   ~~` services.msc`~~
2. ~~找到MySQL90，右键选择停止~~
3. ~~选择非C盘，创建存放data文件夹~~

## 环境配置

1. 打开资源管理器，找到左边此电脑右击选择**属性**
2. 找到界面右侧**高级系统设置**选择**环境变量**
3. 上方为用户变量，下方为系统变量，我们需要修改系统变量
4. 我们需要提前准备MySQL安装位置并复制，默认应为C:\Program Files\MySQL\MySQL Server 9.0\bin
5. 双击系统变量中的Path，点击新建，将上一步复制的地址粘贴即可
6. 完成之后三次确定即完成环境配置。
7. 结果检验
   
   进入cmd
   
   输入`mysql --version`查看当前版本
   
   或输入`mysql -uroot -p`，使用root密码登陆数据库
   
   两种方法均可

## 缺少环境 Visual Studio 20 19 x64Redistributable

Microsoft Visual C++ Redistributable 2019
x86: [https://aka.ms/vs/16/release/VC_redist.x86.exe](https://aka.ms/vs/16/release/VC_redist.x86.exe)
x64: [https://aka.ms/vs/16/release/VC_redist.x64.exe](https://aka.ms/vs/16/release/VC_redist.x64.exe)

> 引用此处[https://blog.csdn.net/kpacnB_Z/article/details/110122336](https://blog.csdn.net/kpacnB_Z/article/details/110122336)
