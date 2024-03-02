---
title: "记一次Kotlin 报错:No such file or directory"
date: 2024-01-12T19:37:52+08:00
tags: 
  - Android开发
  - Kotlin
---


今天在学习 Kotlin 的时候,想要实现解析JSON文件,在读取文件时一直提示没有文件或者目录(No such file or directory),当时目录结构是:

```
Kotlin/:
├── Main.kt
└── List.json
```

`Main.kt`文件中设定的路径是`List.json`,但是在运行时一直提示找不到文件.

解决方法:设置运行配置的工作目录至 `Main.kt的上级目录`

点击运行按钮旁的运行配置,因为默认是当前文件,所以需要自己添加.

设置主要类为`Main.kt`文件,以及工作目录.保存后应用即可.

> 被这个小问题折腾半天,晕了
