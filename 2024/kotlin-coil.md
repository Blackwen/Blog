---
title: "Coil-一个 Kotlin 多平台图片加载库"
date: 2024-01-24T17:53:02+08:00
tags:
    - Kotlin
    - Android开发
---

![](https://coil-kt.github.io/coil/logo.svg)

[中文文档](https://github.com/coil-kt/coil/blob/main/README-zh.md) | [官方仓库](https://github.com/coil-kt/coil)


## 使用 Coil从互联网加载图片

新建一个 kotlin 项目导入依赖

### XML

如果使用 XML 则导入:

```kotlin
implementation("io.coil-kt:coil:2.5.0")
```

具体方法查看 [此处](https://github.com/coil-kt/coil/blob/main/README-zh.md#%E5%BF%AB%E9%80%9F%E4%B8%8A%E6%89%8B)

### Jetpack Compose

此处使用 Compose 作为实例

在 `build.gradle` 文件中导入依赖:

```kotlin
implementation("io.coil-kt:coil-compose:2.5.0")
```

#### 使用

通过使用 `AsyncImage` 组件从网络加载图片

```kotlin
    AsyncImage(
        model = "https://img.xwyue.com/i/2024/01/17/65a7b95f0249f.png",
        contentDescription = null,
    )
```


