---
title: "在Arch Linux上安裝deb格式包"
date: 2023-01-23T13:34:24+08:00
tags:
  - Linux
  - 笔记
---


### **環境：**

#### Arch Linux，提前安裝好yay（包管理器）

### **步驟：**

#### 打開Konsole（終端）

###### **1.首先確保你已經安裝了AUR包管理器**

```bash
yay --version #查看版本
```

###### **2.進入你下載的deb包的位置**

Arch Linux默認的下載位置是 **/home/username/Downloads**

如果接下來的步驟你不希望在**Downloads**目錄進行

請使用mv指令將它移動到別的目錄

```bash
find -name FilesName #通過名稱搜索文件
mv FliesName Route #將文件移動到指定路徑
```

###### **3.我們接下來就使用yay安裝debtap**

在終端輸入以下內容

```bash
yay -S debtap
```

在安裝完成後，我們輸入：

```bash
su #獲取root權限
```

然後我們檢查一遍自己所在的位置和文件

```bash
pwd #輸出當前位置
ls #查看當前目錄所有文件
```

如果沒有問題就可以繼續下一步了

###### **4.使用debtap將deb包轉化**

首先在終端輸入：

```bash
debtap -u #更新debtap數據庫（時間較長，請耐心等待，按 Ctrl + c 可以中止）
```

如果你沒有切換root，請使用sudo

然後將deb包轉化

```bash
debtap FilesName #輸入文件名回車後等待轉化
```

```bash
#提示輸入名稱，可以填寫也可以直接回車
:: Enter Packager name (can be left blank):
#下一步，提示輸入输入软件包许可证，略過
:: Enter package license (can be left blank, you can enter multiple licenses comma separated):
#選擇編輯器，我這裏直接回車
:: If you want to edit .PKGINFO and .INSTALL files (in this order), press (1) For vi (2) For nano (3) For default editor (4) For a custom editor or any other key to continue
#然後靜靜等待他轉換
```

完成後他生成了一個.zst的文件

我們可以直接使用pacman安裝了

```bash
pacman -U FilesName #安裝，如果你沒有root權限，請使用sudo
```

等待...........

安裝完成後你就可以在菜單打開它了
