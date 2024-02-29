---
title: "JetpackCompose组件介绍-Buttom app bar"
date: 2023-08-28T13:51:34+08:00
tags:
  - Jetpack-Compose
  - Android开发
  - Kotlin
---


![Demo](https://lh3.googleusercontent.com/l12xRZWyitFw6eD6eohMi1rSKb2Un_7zX-lT1wqBNJ2AOA1NCT8bv8iKCgH9k2oHP7cEYQYI0xM3eeDpDmQ88xXeHw3nHf1cOolr_-aBD-t7=s0)

此图片来自Material You 官网

## Buttom app bar 只是一个载体，里面的内容是可以自定义的。

本文章按照Material You官网给出的要求来

> 底部应用栏在移动屏幕底部显示导航和关键操作。

我们先观察Buttom app bar里面的组成，从左至右依次是四个IconButton，最右边则是一个FloatingActionButton

首先添加一个Buttom app bar组件

```kotlin
@Composable
fun ButtomAppBar(

)
```

在里面添加四个IconButton，你也可以添加其他的东西。

```Kotlin
@Composable
fun ButtomAppBar(
	actions = {
                IconButton(onClick = { /* doSomething() */ }) {
                    Icon(
                        Icons.Filled.Search,
                        contentDescription = "Description"
                    )
                }
                IconButton(onClick = { /* doSomething() */ }) {
                    Icon(
                        Icons.Filled.DeleteOutline,
                        contentDescription = "Description",
                    )
                }
                IconButton(onClick = { /* doSomething() */ }) {
                    Icon(
                        Icons.Outlined.Archive,
                        contentDescription = "Description",
                    )
                }
                IconButton(onClick = { /* doSomething() */ }) {
                    Icon(
                        Icons.Filled.TurnRight,
                        contentDescription = "Description",
                    )
                }
            },
)
```

再添加一个FloatingActionButton

```Kotlin
	floatingActionButton = {
                FloatingActionButton(
                    onClick = { /* do something */ },
                    containerColor = BottomAppBarDefaults.bottomAppBarFabColor,
                    elevation = FloatingActionButtonDefaults.bottomAppBarFabElevation()
                ) {
                    Icon(Icons.Filled.Add, "Description")
                }
            }
```


