---
title: "JetpackCompose组件介绍-Top app bar"
date: 2023-08-28T21:40:00+08:00
tags:
  - Jetpack-Compose
  - Android开发
  - Kotlin
---

![Demo](https://lh3.googleusercontent.com/qpPkklJvKNdaomoh4JjRtmnsoVV3nLuecjkMHWYk0U58Jam0pqqFVkttRbHXE55YvZSuvfXVYTrRy-IKi9Z_yokHOtInhEwjDiX8cjMdK7tg=s0)

此图片来自Material You 官网

## 本着今日事，今日毕的原则，决定把Top app bar也顺带记录下

本文章将会使用Jetpack Compose仿造Material You官网所出示4个Bar的样式

### Center-aligned

使用CenterAlignedTopAppBar组件

```Kotlin
fun mainTopAppBar(){
    Column {
        CenterAlignedTopAppBar (
            // elevation = 4.dp,
            title = {
                Text(
                    "Title Large"
                )
            },
            // backgroundColor =  MaterialTheme.colors.primarySurface,
            navigationIcon = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.Menu, "Menu")
                }
            }, actions = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.PersonPin, "PersonPin")
                }
            })
        // Screen
    }
}
```

### Small

使用TopAppBar组件

```Kotlin
fun mainTopAppBar() {
    Column {
        TopAppBar(
            // elevation = 4.dp,
            title = {
                Text(
                    "Title Large"
                )
            },
            // backgroundColor =  MaterialTheme.colors.primarySurface,
            navigationIcon = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.ArrowBack, null)
                }
            }, actions = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.AttachFile, "AttachFile")
                }
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.Today, "Today")
                }
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.MoreVert, "MoreVert")
                }
            })
        // Screen
    }
}
```

### Medium

使用MediumTopAppBar组件

```Kotlin
fun mainTopAppBar() {
    Column {
        MediumTopAppBar(
            // elevation = 4.dp,
            title = {
                Text(
                    "Headline Small"
                )
            },
            // backgroundColor =  MaterialTheme.colors.primarySurface,
            navigationIcon = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.ArrowBack, null)
                }
            }, actions = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.AttachFile, "AttachFile")
                }
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.Today, "Today")
                }
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.MoreVert, "MoreVert")
                }
            })
        // Screen
    }
}
```

### Large

使用LargeTopAppBar组件

```Kotlin
fun TopAppBarSample() {
    Column {
        LargeTopAppBar(
            // elevation = 4.dp,
            title = {
                Text(
                    "Meadline Large"
                )
            },
            // backgroundColor =  MaterialTheme.colors.primarySurface,
            navigationIcon = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.ArrowBack, null)
                }
            }, actions = {
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.AttachFile, "AttachFile")
                }
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.Today, "Today")
                }
                IconButton(onClick = {/* Do Something*/ }) {
                    Icon(Icons.Filled.MoreVert, "MoreVert")
                }
            })
        // Screen
    }
}
```

几种TopBar的参数都是差不多的，需要更改为其他Bar也很方便，只需要修改名称
