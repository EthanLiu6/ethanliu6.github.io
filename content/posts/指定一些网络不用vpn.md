---
title: "指定一些网络不用vpn"
date: 2025-11-12
draft: false
tags: ["网络"]
categories: ["工具"]
---
{{< quote >}}
如何指定一些网址/ip不使用vpn？
{{< /quote >}}
<!--more-->

在公司上班的时候访问公司内网每次都得关掉代理才行，后面直接设置了一下系统网络的代理，然后就可以啦。Mac和Windows的操作都差不多。


比如我现在上班的公司好多内部系统是`xxx.xxx.hxdi.cn`这样子的，我们可以用下面这种方式进行忽略。

## Mac设置
> 进入WI-FI -> 找到详细信息
![20251114221557](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/20251114221557.png)

> 找到代理 -> 添加要忽略的主机和域名
> [!Note]
> `*`是通配符，然后Mac里面添加的每个都要用`英文逗号`隔开，win系统使用`英文分号`
![20251114221914](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/20251114221914.png)
## Windows设置
思路与Mac一样。由于我手头没有win，不方便截图，我记得大概是在：
> 设置 -> 代理 -> 找到类似上面这个忽略掉的填写


> 注意有时候网络重连之后又要重新设置一次。




