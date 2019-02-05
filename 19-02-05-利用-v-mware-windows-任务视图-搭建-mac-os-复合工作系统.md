---
title: 利用 VMware + Windows 任务视图 搭建 MAC-OS 复合工作系统
date: 'Tue, 5 Feb 2019 23:10:40 +0800'
stacks:
    - 虚拟机
---

## 利用 VMware 搭建 MAC-OS 复合工作系统
> 参考资料1：安装 MAC-OS 于 VMware 中 - https://jingyan.baidu.com/article/59a015e374a45bf795886542.html \
> 参考资料2：https://www.cnblogs.com/liangning/p/4015662.html
### 第一步：下载并安装 VMWare Pro 15
- 官网下载
- 激活序列号建议用正版，但我用的联合激活版本

### 第二步：阅读上述百度经验，在 VMware Pro 15 中安装 MAC-OS
值得一提的是，我们需要在 VMware 中配置虚拟化引擎：
- 勾选“虚拟化 Intel VT-x/EPT 或 AMD-V/RVI(V)”
- 勾选“虚拟化 IOMMU (IO 内存管理单元)(I)”

如图：

![](http://lc-7085gfy8.cn-n1.lcfile.com/477f38952e90e25ea4e1.png)


