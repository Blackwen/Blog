---
title: "Kotlin 编码规范"
date: 2024-02-14T19:41:28+08:00
tags:
    - Kotlin
    - 笔记
    - 文档
---

## 编码规范

### 源文件名称

如果 Kotlin 文件中包含单个函数,类或是接口,那么文件名应该保持一致. (这适用于所有类型的函数,类和接口)

如果包含多个函数,类或接口.那么文件名应该能概括他们, 例如 `ProcessDeclarations.kt`

### 多平台项目

在多项目平台中,不同平台的文件名称后需要加上后缀,比如:

- jvmMain/kotlin/Platform.jvm.kt
    
- androidMain/kotlin/Platform.android.kt
    
- iosMain/kotlin/Platform.ios.kt

对于共同源码(commonMain/kotlin/Platform.kt), 则不需要后缀

## 命名规则

### 包,类,对象和接口

包的名称总是小写且不使用下划线,例如 `org.example.project`, 尽量不要使用多个词作为包的名称.

如果需要使用多个词，请将它们连接在一起并使用驼峰风格, 例如 `org.example.myProject`.

类,对象与接口的名称以大写字母开头并使用驼峰风格, 例如:

```Kotlin
class FileManager() {

}
```

### 函数名

函数,属性与局部变量的名称以小写字母开头、使用驼峰风格而不使用下划线

### 属性名

常量或标记为`const`的属性. 使用大写,下划线风格的格式. 例如 `MAX_SIZE`

## 格式化

### 缩进

使用 4 个空格缩进而不是使用 Tab


