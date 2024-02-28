---
title: "Oh-my-zsh 插件推荐"
date: 2023-08-12T21:04:14+08:00
draft: false
tags:
  - oh-my-zsh
  - 插件推荐
---

## 辅助向

### [archlinux](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/archlinux) 

该插件简化了使用 ArchLinux 的包管理器时的组合命令，如

| Alias   | Command                   | Description                                         |
| ------- | ------------------------- | --------------------------------------------------- |
| pacin   | `sudo pacman -S`          | Install packages from the repositories              |
| pacins  | `sudo pacman -U`          | Install a package from a local file                 |
| pacinsd | `sudo pacman -S --asdeps` | Install packages as dependencies of another package |
| paclean | `sudo pacman -Sc`         | Clean out old and unused caches and packages        |

更多可前往README查看

### [wd]([wd](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/wd)) 

该插件约等于一个终端上的目录书签，使用中，我们可以将自己常用的目录使用

```shell

wd add Name 

```

命令来添加当前目录，下次在需要跳转该目录时直接使用

```shell

wd Name

```

命令即可成功跳转

### [web-search](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/web-search) 

可以快速调用搜索引擎搜索，如

```shell

google oh-my-zsh # 使用Google搜索 oh-mu-zsh

bing oh-my-zsh # 使用 Bing 搜索 oh-my-zsh

```

### [sudo](https://github.com/ohmyzsh/ohmyzsh/blob/master/plugins/sudo/README.md)

双击 Esc 键快速在命令前添加 sudo 

### [z](https://github.com/ohmyzsh/ohmyzsh/blob/master/plugins/z/README.md)

快速跳转到之前使用过的目录

```shell

# 例如，我使用 cd 访问过 ～/Desktop 和 ~/.config/Chrome
# 下次访问可以直接使用 z 加正则表达式匹配来快速访问
z De `or` z Desk
z Chro `or` z Ch

```

## 美化向

### [hitokoto](https://github.com/ohmyzsh/ohmyzsh/blob/master/plugins/hitokoto/README.md)

随机一言
