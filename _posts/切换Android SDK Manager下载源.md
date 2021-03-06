---
title: 切换Android SDK Manager下载源
date: 2016-10-14 16:13:57
tags: 
- android
- sdk
categories: 
- 安卓开发
---

在Android开发时需要新下载或升级相应的工具包，通常大家都会使用sdk管理工具下载，但是由于默认采用的是google下载源，在实际下载过程中并不会太顺利，主要表现一是下载速度慢，二是如果不采用些技术手段，连google网站都上不去。

此时我们可以换个下载源来解决这个问题，比如选择国内的某个源来提高下载速度。

<!-- more -->

![Android-SDK-Manager.png](/images/Android-SDK-Manager.png)

1. 打开  `SDK Manager.exe` 工具，你可以在ide中启动，也可以在sdk安装目录中找到它。
1. 在启动  `Android SDK Manager` 的主界面，依次选择「Tools」、「Options…」，弹出『Android SDK Manager - Settings』窗口。
1. 在 `Android SDK Manager - Settings` 窗口中，在 `HTTP Proxy Server` 和  `HTTP Proxy Port` 输入框内填入 `mirrors.neusoft.edu.cn` 和 `80`，并且选中 `Force https://… sources to be fetched using http://…` 复选框。
1. 设置完成后单击  `Close` 按钮关闭『Android SDK Manager - Settings』窗口返回到主界面依次选择「Packages」、「Reload」。

由于某些网络接入商进行了劫持，会弹出用户认证界面无法使用，这个和镜像服务器配置无关。
