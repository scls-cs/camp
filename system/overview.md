---
jupytext:
	formats: md:myst
	text_representation:
		extension: .md
		format_name: myst
rise:
	start_slideshow_at: beginning

kernelspec:
	display_name: Python 3
	language: python
	name: python3
---


# 计算机网络概论 #

* 互联网的所有设备都有一个IP地址。


* IP地址的格式：x.x.x.x，每个x都是一个8位二进制数。所以IP地址由32位二进制数组成。


* 域名是IP地址的别称，为了方便人类记忆。比如Google主页的IP地址之一172.217.25.14，域名是google.com。


* DNS服务器里存储域名和IP地址的对应关系。


* 可以通过nslookup命令来查找域名对应的IP地址。如果你用Mac，在Launchpad里面搜索"Terminal"。如果你用的是Windows，在开始菜单中搜索"cmd"进入终端。输入"nslookup google.com"，显示类似如下结果：（返回的IP地址可能不同，与电脑配置的DNS服务器有关）

```
  nslookup google.com
  
  Server:     10.10.0.215
  Address:    10.10.0.215#53

  Non-authoritative answer:
  Name:       google.com
  Address:    172.217.25.14
```

* 路由器的作用是对数据进行转发，类似物流公司根据目的地对包裹进行中转。

* 可以通过traceroute命令来观察数据的路径。如果你用Mac，在终端里面输入"traceroute google.com"; 如果你用Windows，在终端里面输入"tracert google.com"。

##  作业 ##

完成作业：

1. 请查找自己计算机的IP地址，在本题下方放上屏幕截图。

2. 打开终端（Windows是cmd），用nslookup命令查找下列域名对应的IP地址，并在下方放上屏幕截图。

* www.baidu.com
* www.google.com
* www.scls.org.cn

3. 请用traceroute(Mac)或者tracert(Windows)命令来追踪从你的电脑到任意一个国外大学的服务器的网络路径，放上屏幕截图并回答下列问题：

    a.	请描述路径经过的地理位置，以及传输所需要的时间

    b.	第一个路由器的ip地址是多少？你认为第一个路由器在哪里？

对于traceroute命令，你可以查看：https://www.fortinet.com/cn/resources/cyberglossary/traceroutes

4. HTTP 响应状态码用来表明特定 HTTP 请求是否成功完成。 响应被归为以下五大类：

* 信息响应 (100–199)
* 成功响应 (200–299)
* 重定向消息 (300–399)
* 客户端错误响应 (400–499)
* 服务端错误响应 (500–599)

访问以下网站，通过浏览器中的开发者工具来查看网络请求和相应。其中最主要的状态码是什么？状态码在这里的作用是什么？

* 世界三流大学.com
* https://www.bilibili.com/fake
* https://docs.google.com/document/d/1Ejqwtz9M5OIxkvXcUUx3Ijk5OkbSfonGseUg9JBmJlw/edit?usp=sharing

提交方式：每位同学提交一份Word文档，截止本周日晚10点。


