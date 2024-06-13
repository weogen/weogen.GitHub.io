---
layout: post
title: "Linux磁盘存满报started user manageer for UID 121"
date:   2024-06-13
tags: [linux]
comments: true
author: weogen
---

linux error:started user manageer for UID 121...

<!-- more -->
# 进入恢复模式  
在显示主板品牌后，按住shift,选择ubuntu高级选项-recovery模式，选择root,输入密码进入命令行操作
# 挂载磁盘  
查看磁盘使用情况
''' shell
df -h
mount-rw -o remount /   #挂在磁盘
'''
# 删除相关文件  
``` shell
rm -rf ***
```
