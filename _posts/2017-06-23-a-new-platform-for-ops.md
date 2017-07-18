---
layout: post
title: 一个服务器监控产品 - Cloud Insight
category: tech
tags: devops linux
---
![](/assets/img/devops.jpg)

在知乎这个答案里看到一个宣传答案，答案蛮专业的，试用了下。感觉还可以，不过心里多少有点担心，毕竟不是开源的，东西都在别人手上。

[《开源监控系统中 Zabbix 和 Nagios 哪个更好？》](https://www.zhihu.com/question/19973178)

官网是这个：<https://cloud.oneapm.com>

作为一个手上有一堆服务器的开发者来说，如何管理这些服务器确实比较头疼。我之前用过监控宝，然而感觉还是不能满足需求，免费用户只能监控2台服务器，
其他功能也弱，界面也蛮丑的。

于是也有想过用 zabbix，接下来有时间可以考虑一下。目前精力不济，还是得寻求现成的产品解决一下先。

接下来说说这个国产的监控产品 cloud insight。界面是这个样子：

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201706/2017-06-24-11.18.01.png)

产品似乎只支持3台服务器。在我添加第四台之时就把第一台顶没了。然而报警还是继续会发过来。

仪表盘应该算是他们的小优势。 简单易懂，可以选择单独的一台机器，也可以选择特定的端口监控，蛮方便的。

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201706/2017-06-24-11.28.26.png)

更复杂的功能就没有用了。进入控制台，发现这个团队还有其他的产品，看来野心蛮大的，^_^希望能做好：

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201706/2017-06-24-11.32.17.png)
