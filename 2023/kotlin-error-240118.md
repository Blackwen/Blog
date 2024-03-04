---
title: "Kotlin Multiplatform 构建报错:Failed to find Build Tools"
date: 2024-01-18T13:31:31+08:00
tags:
    - Android开发
    - Kotlin
---

在尝试运行 KMP项目时 提示Failed to find Build Tools但已经在 SDK Manger 中安装了

## 解决方法

打开 `local.properties` 文件,检查 sdk.dir 是否正常(我就因为没写空着的)

