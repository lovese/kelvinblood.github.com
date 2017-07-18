---
layout: post
title:  Mac 下 MySQL 安装以及 phpmyadmin 配置
category: tech
tags: mysql mac homebrew
---
![](/assets/img/php.jpg)

# MySQL 安装

安装 MySQL 有很多种方式，包括 源代码安装、homebrew安装、还有直接下载dmg安装包安装。

一切从简把，直接在官网上下载 dmg 文件，双击安装。<https://dev.mysql.com/downloads/mysql/>

一路无脑安装即可。在系统偏好里开启。 一般还是不要开机自启动，因为 mysql 比较耗内存，像我这的 air 就比较吃力了。

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201707/QQ20170703-215209.png)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201707/QQ20170703-215337.png)

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201707/QQ20170703-215359.png)

# phpmyadmin 配置

phpMyAdmin. 由php开发的一个 MySQL 管理工具。在官网上下载源代码：<https://www.phpmyadmin.net/downloads/>

下载到本地后把文件 「config.sample.inc.php」 拷贝一份，重命名为 「config.inc.php」

找到这一行：
 
    $cfg['Servers'][$i]['host'] = 'localhost';

改为：

    $cfg['Servers'][$i]['host'] = '127.0.0.1';
    
配置好 nginx/apache，就能够跑起来了。 我用的是 IDEA 自带的配置，就不那么费神了。下面是IDEA中的配置方法，可以做个参考。

![](http://7vigrt.com1.z0.glb.clouddn.com/blog/pic/201707/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202017-07-03%2022.04.28.png)
