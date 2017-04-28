---
layout: post
title: bundle 安装nokogiri报错
date: 2017-04-11 12:50:59
tag: 工具
---
使用`bundle install`安装`jekyll`时遇到了安装`nokogiri`报错信息.

```
An error occurred while installing nokogiri (1.6.8.1), and Bundler cannot continue.
Make sure that `gem install nokogiri -v '1.6.8.1'` succeeds before bundling.
```

而直接执行`gem install nokogiri -v '1.6.8.1'`确可以执行成功.

后在stackoverflow上找到的解决方法.

首先执行 `bundle config build.nokogiri --use-system-libraries`, 再执行`bundle install`.

参考地址 [Nokogiri error when running bundle install

Ask](Nokogiri error when running bundle install

Ask)