---
title: "解决Surface keyboard日版键盘与输入不对应问题"
date: 2024-10-26T22:08:42+08:00
Description: ""
draft: false
tags:
  - 技术
categories:
  - post
---
*如题，想着在外更轻便地进行翻译工作入手Surface Pro5，随后入手Surface Keyboard日版，就键位问题折腾了一番。*

#### 设备

* Surface Pro5
* Surface Keyboard

最先搜索的帖子里教程大部分为以下两大步骤；
> &nbsp;
> ##### 更新驱动
> 1. 打开<kbd>设备管理器</kbd>
> 2. 选择<kbd>键盘</kbd>
> 3. 找到<kbd>Surface Type Cover Filter Device</kbd>
> 4. 右键找到<kbd>更新驱动程序</kbd>
> 5. 选择<kbd>浏览我的电脑以查找驱动程序</kbd>
> 6. 选择<kbd>让我从计算机上的可用驱动</kbd>
> 7. 取消勾选<kbd>显示兼容硬件</kbd>
> 8. 找到<kbd>(标准硬盘)</kbd>
> 9. 找到<kbd>Japanese PS/2 Keyboard (106/109 Key Ctrl+Eisuu)</kbd>并按提示更新驱动并重启
> ----
> ##### 修改注册表
> 1. 打开regedit
> 2. 进入<kbd>[HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Control\Keyboard Layouts]</kbd>其中每个编号代表一个输入法，找到以<kbd>0804</kbd>结尾的是简体输入法
> 3. 将其中的LayoutFile改为<kbd>kbdjpn.dll</kbd>重启即可

&emsp;&emsp;<mark>\*咱改为**<u>kbd106.dll</u>**才生效</mark>

#### 外部链接
* https://www.cnblogs.com/xpvincent/p/13785793.html
* https://oshukezu-work.blogspot.com/2009/12/blog-post.html
* https://www.mobile01.com/topicdetail.php?f=242&t=310095