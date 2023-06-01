---
title: 安装nodejs和npm以后出现问题
date: 2018-03-30 16:23:25
tags:
---
安装nodejs和npm以后出现 /usr/bin/env: node: No such file or directory
安装完成以后需要执行此命令：
sudo ln -s /usr/bin/nodejs /usr/bin/node
将2个文件夹链接。