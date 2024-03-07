---
title: "Compose Sonner: Compose Multiplatform 的一个toast 组件"
date: 2024-02-08T11:35:59+08:00
tags:
    - Android开发
    - Kotlin
---


[Github 仓库](https://github.com/dokar3/compose-sonner)

[实例网站](https://dokar3.github.io/compose-sonner/)

![](https://github.com/dokar3/compose-sonner/raw/main/images/banner.png)

[查看视频](https://github.com/dokar3/compose-sonner/assets/68095777/ff97c6cc-012e-4152-8c40-0d2ba382c757)

该库支持堆叠提示,不同类型,多种色彩,任意修改提示的位置,向下滑动关闭,显示关闭按钮和操作按钮自定义图标,设置最多堆叠数量

## 开始

新建一个项目打开`build.gradle(.kts)`,添加依赖

```kotlin
implementation("io.github.dokar3:sonner:<VERSION>")
```

打开`libs.versions.toml`,添加:

```kotlin
sonner = { module = "io.github.dokar3:sonner", version = "<VERSION>" }
```

如果没有这个文件请在`gradle`目录下手动新建一个名为`libs.versions.toml`的文件,具体参考[Google开发者文档](https://developer.android.com/build/migrate-to-catalogs?hl=zh-cn#create-version)

## 实例

```kotlin
@Composable
fun ToastDemo() {
    val toaster = rememberToasterState()

    Button(onClick = {
        toaster.show(
            message = "Hello world!",
            type = ToastType.Normal,
        )
    }) {
        Text("Show a toast")
    }
    Toaster(state = toaster)
}
```

以上是一个简单的实例,在点击按钮后会在屏幕下方显示一个普通类型的Toast,或者修改`type`来修改不同的类型

```
Normal | Success | Info | Warning | Error
```

