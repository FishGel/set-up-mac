# set-up-mac
My OS X 工作环境 「一个 JAVA 开发者的 OS X 工作环境」

## 目录
1. [OS X](#1-os-x)
   - [F1-F12 改成标准功能键](#F1-F12 改成标准功能键)
2. [常用工具](#2-常用工具)
3. [开发工具](#3-开发工具)
 - 3.1 [Homebrew](#31-homebrew)
 - 3.2 [IntelliJ IDEA](#user-content-32-intellij-idea)
 - 3.3 [Mysql 客户端](#user-content-33-mysql-客户端)
 - 3.4 [SSH 客户端](#user-content-34-SSH-客户端)
 

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

### 3.2 IntelliJ IDEA
Java 开发必备工具 IntelliJ IDEA。可以安装 Ultimate Edition：

```sh
brew cask install intellij-idea
```

也可以安装开源免费的 Community Edition：

```sh
brew cask install intellij-idea-ce
```

IntelliJ IDEA 有几套内建的快捷键方案（Keymap）。其中适用于 OS X 的有`Mac OS X`和`Mac OS X 10.5+`两种。区别是:

- `Mac OS X`方案和其他平台上的快捷键类似，
- 而`Mac OS X 10.5+`更加符合 OS X 常用的快捷键。

一个团队使用不同的快捷键会严重影响效率。可以用`View | Quick Switch Scheme`（`⌃ Back Quote`）快速切换 Keymap。

可以从 IDEA 的`Help > Default Keymap Reference`打开快捷键的参考手册。不过从这里打开的是`Mac OS X 10.5+`方案的，而`Mac OS X`方案的可以从这里找到：<http://www.basrikahveci.com/static/ij_keymap_mac.pdf>。

### 3.3 Mysql 客户端
 这里推荐两个，看个人喜好。
 一个是官方的「[mysql-workbench](https://dev.mysql.com/downloads/file/?id=460634)」功能强大
 另外一个是「[sequelpro](http://sequelpro.com/)」，比较简洁。
 
### 3.4 SSH 客户端 
 这里也推荐两个。
 「[zoc6](http://www.emtec.com/zoc/)」界面优美
 「[shuttle](https://github.com/fitztrev/shuttle)」，比较简洁。
