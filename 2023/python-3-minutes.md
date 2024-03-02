---
title: "Python 3 Minutes"
date: 2023-12-02T12:09:27+08:00
tags:
  - Python
  - 笔记
---

python的学习笔记

## 注释

单行注释

```python
# 单行注释
```

多行注释

```python
"""
多行注释
使用三个 " 或 '
"""
```

## 打印输出

在 Python 中使用`print`关键字进行打印

```python
print("Hello World")
```

## 变量与常量

### 命名

Python中没有变量与常量之分

一般变量名使用小写字母，常量名使用大写字母

注:

只能包含字母、数字和下划线(A-z、0-9和_)。不能使用空格或特殊字符。

不能以数字开头，避免使用关键字作为名称

例如

```python
# 变量
user_name user_age

# 常量
USER_BIRTHDAY
```

### 赋值

在变量名后使用 `=` 进行赋值

注：Python 中的变量不需要声明类型,赋值时会自动推断类型。 

```python
user_name = "Joe"
user_age = 18
```
