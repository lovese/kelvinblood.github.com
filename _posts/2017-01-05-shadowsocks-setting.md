---
layout: post
title: shadowsocks的设置
category: tech
tags: proxy shadowsocks
---

* 购买请戳这里 >>>[购买链接](http://wechat.kelu.org/charge)<<<
  
* L2TP协议请戳这里  >>>[L2TP](/tech/2017/03/15/L2TP-VPN-setting.html)<<<

* PPTP协议请戳这里  >>>[PPTP](/tech/2015/02/14/PPTP-VPN-setting.html)<<<

Shadowsocks 是当下一个蛮重要的科学上网工具，查询科研论文和开发程序必不可少。学会正确的上网姿势，是成为现代人的很重要的一步哦。

* 在[Windows](#windows)下的设置
* 在[Mac](#mac)下的设置
* 在[Android](#android)下的设置
* 在[iOS](#iOS)下的设置


<span id="windows"></span>

# Windows 基本使用

新手在使用前请关闭本机/浏览器的本地代理插件，例如,Chrome插件Proxy SwitchySharp。

* 下载程序： [链接一][ss_w]，[链接二][ss_w_baidu] 密码 f53i。 解压到你希望运行程序的路径，例如：`C:\Program Files (x86)\ss`

* 在任务栏找到 Shadowsocks 图标，在 服务器 菜单添加服务器(首次双击运行程序自动打开)

![1](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201701/20170108223605.png)

* 选择 启用系统代理 来启用系统代理。

![2](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201701/20170108223622.png)
![3](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201701/20170108223615.png)

* 完成。

	海外党的代理模式要设置成全局模式噢。

* PAC 模式和全局模式的区别：

    全局模式就是所有请求都通过 Shadowsocks 设置的服务器进行访问.
PAC 模式是智能判断该网站是否需要通过设置的服务器进行访问。

<span id="mac"></span>

# Mac 基本使用

新手在使用前请关闭本机/浏览器的本地代理插件，例如,Chrome插件Proxy SwitchySharp。

*  高于 10.10 的系统，请使用这个： [链接一][ss_x]，[链接二][ss_x_baidu] 密码 26p4。

    低于 10.10 的系统，请使用这个： [链接一][ss_x2]，[链接二][ss_x2_baidu] 密码 yvcr。
    
    双击 dmg 文件安装。

* 在任务栏找到 Shadowsocks 图标，在 服务器 菜单添加服务器

![5](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201701/D28973C0-7E48-46BC-997F-6470261382C1.png)

* 选择 启用系统代理 来启用系统代理。

![4](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201701/4BFA4DCB-563A-453B-A4C7-942B25E85858.png)

* 完成。

	海外党的代理模式要设置成全局模式噢。

* PAC 模式和全局模式的区别：

    全局模式就是所有请求都通过 Shadowsocks 设置的服务器进行访问.
PAC 模式是智能判断该网站是否需要通过设置的服务器进行访问。

<span id="android"></span>

# android 基本使用

* 下载安装程序： [链接一][ss_a]，[链接二][ss_a_baidu] 密码 imsn。

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502195710.jpg)

* 手动输入配置，或选择二维码扫描。

[![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/QQ20170503001203.png)](http://wechat.kelu.org/dashboard)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502195748.jpg)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502195832.jpg)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502200022.jpg)

* 完成。

	海外党的代理模式要设置成全局模式噢。

<span id="iOS"></span>

# iOS 基本使用

* 前往 App Store 中国区搜索、下载：[Wingy][ss_i]

    有一个是免费的一个是收费的，没什么区别，下免费的吧233333

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502173508.jpg)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502194435.jpg)

* 手动输入配置，或选择二维码扫描。

[![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/QQ20170503001203.png)](http://wechat.kelu.org/dashboard)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502194509.jpg)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502194723.jpg)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201705/20170502194757.jpg)

* 完成。

	海外党的代理模式要设置成全局模式噢。

# 高级使用

## PAC
* 可以编辑 PAC 文件来修改 PAC 设置。Shadowsocks 会监听文件变化，修改后会自动生效。
* 也可以从 GFWList（由第三方维护）更新 PAC 文件或使用在线 PAC URL.

## 服务器自动切换

* 负载均衡：随机选择服务器
* 高可用：根据延迟和丢包率自动选择服务器
* 累计丢包率：通过定时 ping 来测速和选择。如果要使用本功能，请打开菜单里的统计可用性。
* 也可以实现 IStrategy 接口来自定义切换规则，然后给我们发一个 pull request。

[ss_w]: http://wechat.kelu.org/download/kelussW.zip
[ss_x]: http://wechat.kelu.org/download/kelussX.zip
[ss_x2]: http://wechat.kelu.org/download/kelussX2.zip
[ss_a]: http://wechat.kelu.org/download/kelussA.zip
[ss_i]: https://appsto.re/cn/19xBeb.i
[ss_w_baidu]: http://pan.baidu.com/s/1bFnQWm 
[ss_x_baidu]: http://pan.baidu.com/s/1dENVlAT
[ss_x2_baidu]: http://pan.baidu.com/s/1geFMUpP
[ss_a_baidu]: https://pan.baidu.com/s/1i5qXrc5
