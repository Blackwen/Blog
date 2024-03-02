---
title: "基于终端的Markdown演示工具-Slides"
date: 2023-12-20T21:08:30+08:00
tags:
  - Linux
  - 工具推荐 
---

> Slides 是一个终端下的Markdown演示工具

[Github 仓库链接](https://github.com/maaslalani/slides)

## 自定义

您可以自定义底部显示的信息

例如作者，显示时间方式，页数显示以及主题

```
--- 
author: VinKon
date: MMMM DD YYYY
paging: 一共有 %d 页，当前在第 %d 页 
theme: ./theme.json
--- 
```

![Show](https://img.lilkon.cn/Design/Slidespng.png)


### 主题 

可以根据官方提供的 [默认主题](https://github.com/charmbracelet/glamour/tree/master/styles) 进行更改



## 语法

Slides中使用分割线来隔开页面

在两段话之间使用`---` 即可分为两个页面
例如
```markdown
# 欢迎使用 Slides
这是第一页
`---`
# 说明
这是第二页
```

使用Slides浏览时就会有两个页面了

## 键位

使用以下组合按键转到第一张幻灯片：
* <kbd>g</kbd> <kbd>g</kbd>

使用以下任意按键转到下一张幻灯片：

* <kbd>space</kbd>
* <kbd>right</kbd>
* <kbd>down</kbd>
* <kbd>enter</kbd>
* <kbd>n</kbd>
* <kbd>j</kbd>
* <kbd>l</kbd>
* <kbd>Page Down</kbd>
* 数字+以上任何一项（前进n张幻灯片）

使用以下任意按键转到上一张幻灯片：
* <kbd>left</kbd>
* <kbd>up</kbd>
* <kbd>p</kbd>
* <kbd>h</kbd>
* <kbd>k</kbd>
* <kbd>N</kbd>
* <kbd>Page Up</kbd>
* 数字 + 以上任意一项（返回 n 张幻灯片）

使用以下按键顺序转到特定幻灯片：

* 数字 + <kbd>G</kbd>

使用G键转到最后一张幻灯片：

* <kbd>G</kbd>

如果展示的页面拥有代码块，您可以通过下面的键位运行它：

* <kbd> Ctrl </kbd> + <kbd> e </kbd>


## 问题

目前该项目对于图片的支持并未完善

具体信息可查看 [Support Images #2](https://github.com/maaslalani/slides/issues/2)

如果你不能忍受对图片显示的不支持，可以尝试以下替代

* [`lookatme`](https://github.com/d0c-s4vage/lookatme)
* [`sli.dev`](https://sli.dev/)
* [`presenterm`](https://github.com/mfontanini/presenterm)

其中lookatme似乎只在特定终端才能够显示图片

具体信息请查看 [Render images directly in terminal (if supported natively) #149](https://github.com/d0c-s4vage/lookatme/issues/149)

