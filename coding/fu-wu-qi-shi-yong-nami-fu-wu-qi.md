---
description: 等待相关维护人员完成编写。
---

# 【服务器】使用NaMI服务器

{% hint style="info" %}
**为什么要使用服务器？**

众所周知，AI项目首先应当具备算力保证。
{% endhint %}

首先你需要一个能进行SSH连接的工具，这里windows下推荐使用WinSCP+Putty的方式。

提供某个版本的下载地址：

[https://zyfan.lanzouj.com/b04q45onc\
密码:nami](https://zyfan.lanzouj.com/b04q45onc%E5%AF%86%E7%A0%81:nami)

安装好WINSCP后，配置Putty路径：

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

使用同济大学VPN系统进入同济内网。

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

新建服务器SSH链接，输入主机IP和用户名、密码，点击登录

**主机IP：**10.60.45.111

**用户名：**姓名首字母缩写（如fzy/hpc/czx...）

**默认密码：**openit

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

请使用conda新建环境进行作业，_<mark style="color:red;">**请勿直接在系统环境中进行pip install操作！**</mark>_





**其他conda使用请自行搜索相关教程。**

{% hint style="info" %}
**使用过程中任何问题请咨询网络管理员。**
{% endhint %}



***

前任网管曾留下过一份服务器维护指南文档（用户一般用不到）：

{% embed url="https://serverdocs.readthedocs.io/en/latest/index.html" %}
