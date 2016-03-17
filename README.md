# set-up-mac
一个 JAVA 开发者的 OS X 工作环境

## 目录
1. [OS X](#1-os-x)
   - [F1-F12 改成标准功能键](#F1-F12 改成标准功能键)
2. [常用工具](#2-常用工具)
3. [开发工具](#3-开发工具)
 - 3.1 [Homebrew](#31-homebrew)

## 1. OS X

### F1-F12 改成标准功能键

默认情况下，F1-F12 都是特殊功能，比如调节屏幕亮度。而当你需要键入 F1-F12 时（比如在使用 IntelliJ IDEA 的快捷键时），需要同时按住 Fn。这对于开发人员来说是非常不方便的。

把 F1-F12 改成标准功能键：选择`System Preferences` > `Keyboard`，在`Keyboard`标签页中选中`Use all F1, F2, etc. keys as standard function keys`。


## 2. 常用工具

- [enpass](https://itunes.apple.com/cn/app/enpass-password-manager-mi/id732710998?mt=12)，配套 iOS 版使用，管理常用密码  「土豪可以用[1Password](https://itunes.apple.com/cn/app/1password/id443987910?mt=12)」
- [Alfred](https://itunes.apple.com/cn/app/alfred/id405843582?mt=12) 「Mac 神软」 「快速启动工具」，输入关键字后能够快速得定位出你想要的文件或程序 [了解更多](http://www.wellsnake.com/jekyll/update/2014/06/15/001/)

## 3. 开发工具

### 3.1 Homebrew
安装包管理工具 [Homebrew](http://brew.sh/)
在安装 Homebrew 之前，需要将 Xcode Command Line Tools 安装完成，这样你就可以使用基于 Xcode Command Line Tools 编译的 Homebrew。

在 terminal 中复制以下命令（不包括 $），跟随指引，将完成 Hombrew 安装。
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

安装完后，运行以下命令，确保 brew 运行正常。
```
$ brew doctor
```
安装完成后，Homwbrew 会将本地 /usr/local 初始化为 git 的工作树，并将目录所有者变更为当前所操作的用户，将来 brew 的相关操作不需要 sudo 。
