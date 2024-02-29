---
title: "JetpackCompose组件介绍-Button"
date: 2023-08-24T23:13:08+08:00
tags:
  - Android开发
  - Jetpack-Compose
  - Kotlin
---

![AllButton](https://lh3.googleusercontent.com/-ZA5rZmbZHsg01D2xWH3U8_oLvviEPddXPs32hueCDeD6Q-xU8OUNbg3hRE8xTl6Z8kQYM0qPCZ3PAM152e1c6Q-8rck8N6sdJmtI6Hcux4=s0)

此图片来自Material You官网

## ElevatedButton 阴影按钮(带图标)

```kotlin
	ElevatedButton(onClick = {

        }) {
            Icon(
                imageVector = Icons.Default.Add,
                contentDescription = "Test",
                modifier = Modifier.size(16.dp)
            )
            Spacer(modifier = Modifier.width(8.dp))
            Text(text = "New a Word")
        }
```

![image-20230825185739067](https://img.lilkon.cn/Blog/JepackCompose/image-20230825185739067.png)

## Button 按钮(默认)

```Kotlin
	Button(onClick = {

        }) {
            Text(text = "Show All")
        }
```

![image-20230825185709434](https://img.lilkon.cn/Blog/JepackCompose/image-20230825185709434.png)

## FilledTonalButton 填充色调按钮

```kotlin
	FilledTonalButton(onClick = {

        }) {
            Text(text = "Visit site")
        }
```

![image-20230825185609817](https://img.lilkon.cn/Blog/JepackCompose/image-20230825185609817.png)

## OutlinedButton 边框按钮

```Kotlin
	OutlinedButton(onClick = {

	    }) {
    		Text(text = "Enable")
	}
```

![image-20230825185820952](https://img.lilkon.cn/Blog/JepackCompose/image-20230825185820952.png)

## TextButton 文本按钮

```Kotlin
	TextButton(onClick = {

        }) {
            Text(text = "Text")
        }
```

![image-20230825185905972](https://img.lilkon.cn/Blog/JepackCompose/image-20230825185905972.png)

## IconButton 图标按钮

```Kotlin
	IconButton(onClick = {

        }) {
            Icon(imageVector = Icons.Default.StarBorder,
                contentDescription = "Test")
        }
```

![image-20230825190042082](https://img.lilkon.cn/Blog/JepackCompose/image-20230825190059436.png)

## FloatingActionButton 浮动操作按钮

```Kotlin
	FloatingActionButton(onClick = {

        }) {
            Icon(imageVector = Icons.Default.Add,
                contentDescription = "Test",
                modifier = Modifier.size(24.dp))
            Spacer(modifier = Modifier.width(8.dp))
        }
```

![image-20230825190121282](https://img.lilkon.cn/Blog/JepackCompose/image-20230825190121282.png)

## ExtendedFloatingActionButton 扩展浮动操作按钮

```Kotlin
	ExtendedFloatingActionButton(onClick = {

        }) {
            Icon(imageVector = Icons.Default.Add,
                contentDescription = "Test",
                modifier = Modifier.size(24.dp))
            Spacer(modifier = Modifier.width(8.dp))
            Text(text = "Test")
        }
```

![image-20230825190222144](https://img.lilkon.cn/Blog/JepackCompose/image-20230825190222144.png)

