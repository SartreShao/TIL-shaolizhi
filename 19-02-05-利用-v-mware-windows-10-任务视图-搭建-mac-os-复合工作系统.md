---
title: 利用 VMware + Windows10 任务视图 搭建 MAC-OS 复合工作系统
date: 'Tue, 5 Feb 2019 23:10:40 +0800'
stacks:
    - VMware
    - 环境配置
    - 黑苹果
---

## 利用 VMware + Windows10 任务视图 搭建 MAC-OS 复合工作系统
> 参考资料：安装 MAC-OS 于 VMware 中 - https://jingyan.baidu.com/article/59a015e374a45bf795886542.html
### 第一步：下载并安装 VMWare Pro 15
- 官网下载
- 激活序列号建议用正版，也可以利用搜索引擎搜一个

### 第二步：阅读上述参考资料，在 VMware Pro 15 中安装 MAC-OS
值得一提的是，我们需要在 VMware 中配置虚拟化引擎：
- 勾选“虚拟化 Intel VT-x/EPT 或 AMD-V/RVI(V)”
- 勾选“虚拟化 IOMMU (IO 内存管理单元)(I)”

如图：

![](http://lc-7085gfy8.cn-n1.lcfile.com/477f38952e90e25ea4e1.png)

这可以帮助我们提高 MAC-OS 虚拟机的性能，虚拟机将和宿主机共享一个CPU，而不是互相竞争。

### 第三步：使用 Windows10 任务视图，搭建 MAC-OS 复合工作系统
Windows10 的一个非常出色的功能，大家可能平时使用的比较少，这就是它的 “任务视图” 功能。  
下面，我们将利用 “任务视图” 帮助我们搭建一个非常方便的“复合工作系统”。  

任务流程：
- 打开任务视图，创建新的桌面
- 在新的桌面上打开 VMware，打开之前安装好的 MAC-OS 虚拟机
- VMware 进入全屏模式

此时，我们已经有了一个 MAC-OS 的工作系统了，再配合两个快捷键，就可以流畅使用了。

快捷键：
- Windows + Ctrl + 方向键 ----- 切换任务视图
- Ctrl + Alt ----- 从 VMware 返回到宿主计算机

熟练运用这两个快捷键后，我们就算搭建完成了 MAC-OS 复合工作系统了。

演示：

![](http://lc-7085gfy8.cn-n1.lcfile.com/83a40405ebf386fd58fa.gif)




