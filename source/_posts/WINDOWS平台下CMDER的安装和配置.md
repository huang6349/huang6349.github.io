---
title: WINDOWS平台下CMDER的安装和配置
date: 2018-05-25 13:38:37
tags: cmder
categories: 开发工具
updated: 2018-05-25 14:12:45
---

## CMDER的安装

### 下载CMDER

打开[GITHUB](https://github.com)，搜索`cmder`，进入`cmder`的项目主页

![CMDER](WINDOWS平台下CMDER的安装和配置/1.png)

选择GITHUB的版本发布选项，打开版本发布界面

![CMDER](WINDOWS平台下CMDER的安装和配置/2.png)

选择一个发布版，进行下载

![CMDER](WINDOWS平台下CMDER的安装和配置/3.png)

当前最新版下载地址：[v1.3.2下载地址](https://github.com/cmderdev/cmder/releases/download/v1.3.2/cmder_mini.zip)

<!-- more -->

### 安装CMDER

等待下载完成，将下载的压缩包解压，例如我将压缩包解压到“C盘”

![CMDER](WINDOWS平台下CMDER的安装和配置/4.png)

![CMDER](WINDOWS平台下CMDER的安装和配置/5.png)

## 配置环境变量

打开控制面板

![CMDER](WINDOWS平台下CMDER的安装和配置/6.png)

选择系统

![CMDER](WINDOWS平台下CMDER的安装和配置/7.png)

打开高级系统设置

![CMDER](WINDOWS平台下CMDER的安装和配置/8.png)

打开环境变量配置

![CMDER](WINDOWS平台下CMDER的安装和配置/9.png)

新建变量名“CMDER_HOME”，变量值为CMDER解压后的根路径
例如：
变量名：`CMDER_HOME`
变量值：`C:\Users\****\AppData\Local\cmder_mini`

![CMDER](WINDOWS平台下CMDER的安装和配置/10.png)

将CMDER_HOME配置到Path中

例如：`%CMDER_HOME%`（注意，Path变量值如果是在最后，则不用打“`;`”）

![CMDER](WINDOWS平台下CMDER的安装和配置/11.png)

## 验证CMDER是否安装成功

使用`Win+R`键，打开运行界面，输入`cmder`，运行正常则`cmder`安装成功

![CMDER](WINDOWS平台下CMDER的安装和配置/12.png)

## 将CMDER加入Windows的右键菜单中

在管理员权限的终端输入命令行`Cmder.exe /REGISTER ALL`即可将`cmder`加入到Windows的右键菜单中

![CMDER](WINDOWS平台下CMDER的安装和配置/13.png)

输入命令行
```cmd
Cmder.exe /REGISTER ALL
```

效果图如下

![CMDER](WINDOWS平台下CMDER的安装和配置/14.png)

![CMDER](WINDOWS平台下CMDER的安装和配置/15.png)

-EOF-
