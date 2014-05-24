---
layout: post
title: "CocoaPods版本升级"
date: 2014-04-19 19:44:47 +0800
comments: true
categories: iOS
---
和往常一样使用[CocoaPods](http://cocoapods.org/)管理一个基于[FMDB](https://github.com/ccgus/fmdb)的项目类库

命令行执行

~~~
$ pod install
[!] The 'master' repo requires CocoaPods 0.32.1 - 
~~~
{:lang="ruby"}
失败，提示需要CocoaPods 0.32.1版本

查看CocoaPods版本

~~~
$ pod --version
0.29.0
~~~
{:lang="ruby"}
确实需要更新了

#### 命令行更新步骤 ####
~~~
$ sudo gem update --system // 先更新gem，国内需要切换源
$ gem sources --remove https://rubygems.org/
$ gem sources -a http://ruby.taobao.org/
$ gem sources -l
*** CURRENT SOURCES ***
http://ruby.taobao.org/
$ sudo gem install cocoapods // 安装cocoapods
$ pod setup
~~~
{:lang="ruby"}
和安装过程是一样的，再次查看版本

~~~
$ pod --version
0.32.1
~~~
{:lang="ruby"}
Done!!