---
title: github push 出现broken pipe 
date: 2018-03-30 16:17:09
tags:
---
github push 出现broken pipe 
fatal: The remote end hung up unexpectedly的问题

重新将ssh添加进github得以解决，
其他办法
~./etc/ssh/ssh_config
Host *  
ServerAliveInterval 120

With this kind of error, I usually start by raising the postBuffer size by:

git config --global http.postBuffer 524288000

(some comments below report having to double the value):

git config --global http.postBuffer 1048576000
