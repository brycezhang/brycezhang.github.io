---
layout: post
title: "在Mac OS中使用Homebrew"
date: 2014-04-21 21:40:30 +0800
comments: true
categories: iOS
---

**`Homebrew`**可以很方便的进行软件包管理，用[官网](http://brew.sh/index.html)的一句话来形容就是

> Homebrew 使 OS X 更完整。用 `gem` 来安装您的 gems、用 brew 来搞定它们的依赖包。

#### 安装Homebrew

只需要一条命令，so easy

> ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)" 

如果你的Mac OS跟我一样，之前没有安装过**Command Line Tools**，期间会自动提示，安装即可。

![install](http://images.cnitblog.com/blog/187312/201404/212108354669672.png)

#### Homebrew的用法

其实**`Homebrew`**像其他包管理器一样，使用非常简单

~~~
$ brew
Example usage:
  brew [info | home | options ] [FORMULA...]
  brew install FORMULA...   // 安装包
  brew uninstall FORMULA... // 卸载包
  brew search [foo]         // 搜索包
  brew list [FORMULA...]    // 显示已经安装的软件列表
  brew update               // 更新brew
  brew upgrade [FORMULA...] // 更新包，不跟包名就是更新所有包
  brew pin/unpin [FORMULA...]
Troubleshooting:
  brew doctor
  brew install -vd FORMULA
  brew [--env | --config]
Brewing:
  brew create [URL [--no-fetch]]
  brew edit [FORMULA...]
  open https://github.com/Homebrew/homebrew/wiki/Formula-Cookbook
Further help:
  man brew
  brew home
~~~

####参考
- [1] [http://brew.sh/index_zh-cn.html](http://brew.sh/index_zh-cn.html)
- [2] [https://github.com/Homebrew/homebrew/wiki/Installation](https://github.com/Homebrew/homebrew/wiki/Installation)