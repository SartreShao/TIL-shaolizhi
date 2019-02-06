---
title: 【使用 cnpm 安装 vue-cli】
date: 'Tue, 5 Feb 2019 23:29:49 +0800'
stacks:
    - nodejs
    - vue
    - 环境配置
---

> 参考资料：https://npm.taobao.org/

cnpm 属于淘宝出品，是一个完整的 npm 镜像源，它每 10 分钟就会和 npm 的官方镜像同步一次。  
我之前由于使用 npm 安装 vue cli 失败，因此认为有可能是网络环境问题，故做此尝试。  
（但是我明明也挂 VPN 了，真是奇怪啊）

### 安装 CNPM
#### 第一步：打开 CMD，输入如下代码：
``` 
npm install -g cnpm --registry=https://registry.npm.taobao.org
```
#### 第二步：检测是否安装成功
```
cnpm --version
```
如果可以执行，则说明安装成功

### 使用 CNPM 安装 Vue Cli
#### 第一步：打开 CMD，输入如下代码：
```
cnpm install -g @vue/cli
```
#### 第二步：检测是否安装成功
```
vue -V
```
如果出现了版本号，则说明安装成功


