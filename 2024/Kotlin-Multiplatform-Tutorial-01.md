---
title: "Kotlin Multiplatform (KMP) Kotlin 多平台开发入门"
date: 2024-01-17T20:46:26+08:00
tags: 
    - Kotlin
    - KMP
    - 笔记
---

借助 JetBrains 开发的基于 Kotlin 的声明式 UI 框架 [Compose Multiplatform](https://www.jetbrains.com/zh-cn/lp/compose-multiplatform/) ,可以在移动端(Android 和 IOS), 桌面端(Windows,macOS和Linux)以及网页端上使用相同的 Kotlin 代码来构建用户界面.使得开发者可以更轻松地共享 UI 逻辑和界面元素，从而实现跨平台的一致性.

## 设置跨平台开发环境

>  如果想要开发 IOS 或是 macOS 下运行的程序,需确保拥有一台MacBook

Windows或Linux下可以使用 [Android Studio](https://developer.android.com/studio?hl=zh-cn) 作为编辑器

macOS则推荐使用 [Xcode](https://developer.apple.com/xcode/)

## 创建多平台项目

推荐使用 [Kotlin Multiplatform Wizard](https://kmp.jetbrains.com/) 去获取一个多平台项目的模板

![screen_shot_2024-01-17-19-24-50.png](https://img.xwyue.com/i/2024/01/17/65a7b95f0249f.png)

设置好Project Name, Project ID和平台后点击`Download` 会开始下载一个`.zip`文件,然后就可以在电脑上使用 `Android Studio` 或是 `Xcode` 打开这个项目

