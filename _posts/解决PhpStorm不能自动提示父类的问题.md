---
title: 解决PhpStorm不能自动提示父类的问题
date: 2017-11-3 7:40:15
tags:
- PhpStorm
- IDE使用
categories:
- php
---

> 在phpstorm中发现项目打开之后找不到引入的第三方库，尝试过重新打开并引入项目仍然不能解决，最后采用下面方法解决了问题。

由于phpstorm编辑器在初次引入项目时会缓存项目文件，并为这些文件建立索引，以满足全文查询和方法间的跳转要求。如果这些索引出现损坏那势必影响前述的要求，我遇到的问题就在这里，只要让它清理这些缓存文件并重新加载就好。
<!-- more -->
* `File` =>  `nvalidate Caches/Restart` 清除项目缓存并重新加载。

* [Cleaning System Cache](https://www.jetbrains.com/help/phpstorm/cleaning-system-cache.html)

