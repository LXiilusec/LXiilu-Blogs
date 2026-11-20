---
title: Web 架构浅知
tags:
  - 计算机基础/Web架构
status: 学习中
---

> [!info] 知识关联
> - 所属主题：[[计算机基础/计算机基础导航|计算机基础导航]]。
> - 通信基础：[[计算机基础/计算机网络/http&https协议|HTTP 与 HTTPS 协议]]，对应前端向后端发送请求、接收响应的过程。
> - 数据存储：[[计算机基础/数据库/MySQL|MySQL 基础]]，对应后端中的数据库部分。
> - 后续应用：[[网安/top10漏洞/upload|文件上传漏洞]]，结合前后端分工理解上传检查发生在哪里。

# 前端后端
## 前端
* html文件：网页的源代码文件.
* CSS：控制页面的展示效果，一般写到html中“style”里面。
* JavaScrip: emmm.....控制页面功能？一般写到“script"里面。
![[Pasted image 20261104232240.png|569]]
## 后端
* 我只能理解到它应该是三个部分: API接口，服务器，数据库。

## API
* 我的理解：前端和后端之间的窗口，我发出请求，它返回数据。

# phpsduty

* phpsduty是一个集成环境管理工具

|        组件         |     角色     |      语言      | 用的协议           |
| :---------------: | :--------: | :----------: | -------------- |
|   Apache/Nginx    |   Web服务器   |    C写的程序     | http https     |
|       Mysql       |    数据库     |     c++      | Mysql协议        |
|    FTP 0.9.60     |   文件传输服务   |     c++      | FTP FTPS       |
| 数据库工具（phpMyAdmin) | 网页版管理Mysql | http mysql协议 | PHP JavaScript |
|                   |            |              |                |

![[Pasted image 20261106123409.png|350]]


