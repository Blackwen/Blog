---
title: "JetpackCompose组件介绍-Card"
date: 2023-08-26T23:06:15+08:00
tags: 
  - Android开发
  - Jetpack-Compose
  - Kotlin  
---

![Card](https://lh3.googleusercontent.com/rmu_B3l4R7wZhKty1HJjOpiJWQ5ieEzS_f5vveAK7Y3GoEqtoZrldzFQocM1NedlTC_lrjgzcQx9iRQEvoHYdsNRd2oKwC2jCTsji297djj1=s0)

此图片来自Material You 官网

## ElevatedCard 阴影卡片

```Kotlin
	ElevatedCard(
            elevation = CardDefaults.cardElevation(
                defaultElevation = 6.dp
            ),
            modifier = Modifier
                .size(width = 240.dp, height = 80.dp)
                .padding(8.dp),

            onClick = {},
        ) {

        }
```

![b](https://developer.android.com/static/images/jetpack/compose/components/card-elevated.png)

## FilledCard 填充卡片

```Kotlin
	Card(
            colors = CardDefaults.cardColors(
                containerColor = MaterialTheme.colorScheme.primary,
            ),
            modifier = Modifier
                .size(width = 240.dp, height = 80.dp)
                .padding(8.dp),
            onClick = {},
        ) {

        }
```
![a](https://developer.android.com/static/images/jetpack/compose/components/card-filled.png)


## Outlined 边框卡片

```kotlin
	OutlinedCard(

            modifier = Modifier
                .size(width = 240.dp, height = 80.dp)
                .padding(8.dp),
            onClick = {},
        ) {

        }
```

![c](https://developer.android.com/static/images/jetpack/compose/components/card-outlined.png)

