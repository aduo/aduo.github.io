---
layout: post
title: MacOS升级ruby版本
date: 2017-04-11 12:27:50
tag: 工具
---

MacOS自带的ruby版本比较低, 使用`ruby -v`查看版本信息为`ruby 2.0.0p648 (2015-12-16 revision 53162) [universal.x86_64-darwin16]`

现在很多工具都需要把ruby版本升级到2.2以上才可以使用.

使用homebrew就可以非常快速的升级ruby版本.

`brew install ruby`

等待安装完成后, 关闭当前终端, 打开一个新终端, 再次执行`ruby -v`就可以看到ruby版本已经更新了.

`ruby 2.4.0p0 (2016-12-24 revision 57164) [x86_64-darwin16]`

需要说明一下的是, 系统自带的ruby地址为`/usr/local/ruby`, brew新安装的ruby地址为`/usr/local/bin/ruby`. 可以使用`which ruby`命令查看.
