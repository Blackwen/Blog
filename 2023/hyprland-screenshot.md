---
title: "解決Hyprland下的截圖問題"
date: 2023-11-28T13:59:28+08:00
draft: false
tags:
  - Linux
  - 笔记
---
## 安装 Grim

flameshot（火焰截图）在 Wayland 下不可用

可以使用 [Grim](https://sr.ht/~emersion/grim/) 来代替

```shell
sudo pacman -S grim
```

## Grim 使用教程

截图整个屏幕

```shell
grim
```

截图特定区域

```shell
grim -g "10,20 300x400"
```

截图整个屏幕并保存到特定路径

```shell
grim $HOME
```

截图特定区域并保持到特定路径

```shell
grim -g "10,20 300x400" $HOME
```

## 安装 Slurp

slurp是一个选取桌面的程序，使用它便能够在wayland下实现选取区域截图。

```shell
sudo pacman -S slurp
```

## Slurp 使用教程

截图桌面选取部分

```shell
grim -g ${slurp}
```

截图桌面选取部分并保存到指定路径

```shell
grim -g ${slurp} $HOME
```

## 配置Hyprland快捷键

打开 `~/.config/hypr/hyprland.conf` 

设置一个新的Mod键位，避免使用中误触

我默认的Mod键是键盘上的SUPER键，我使用SUPER+SHIFT+S组合键来截图。

### 在 Hyprland 中设置变量

```shell
# SUPER+SHIFT 组合键
$shiftMod = SUPER_SHIFT
# 设置截图保存路径，并且将文件名设置为 screen_shot_截图的时间
$screenFile = ${HOME}/Pictures/ScreenShot/screen_shot_$(date +"%Y-%m-%d-%H-%M-%S").png
```

### 在 Hyprland 中配置键位

dunstify的作用是在截图保存后提示

```shell
# 截圖整個屏幕
bind = $shiftMod, A, exec, grim $screenFile ; dunstify "您的截圖以保存至 $screenFile"
# 截圖選取範圍的屏幕
bind = $shiftMod, S, exec, grim -g "$(slurp)" $screenFile ; dunstify "您所選取区域的截圖以保存至 $screenFile"
```


