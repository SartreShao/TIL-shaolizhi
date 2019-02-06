---
title: 【使用 VUE-CLI 构建大型单页 WEB 应用】
date: 'Wed, 6 Feb 2019 12:03:37 +0800'
stacks:
    - vue
---

## VUE 全家桶都有什么？
- vue-router
- vue-cli
- vuex
- vue-resource
- saas

## 构建项目的第一步：Webpack
### Webpack是什么
> 本质上，webpack 是一个现代 JavaScript 应用程序的静态模块打包器(module bundler)。当 webpack 处理应用程序时，它会递归地构建一个依赖关系图(dependency graph)，其中包含应用程序需要的每个模块，然后将所有这些模块打包成一个或多个 bundle。

### 我们为什么要安装 Webpack
VUE-CLI 需要用到 Webpack 作为静态模块打包器。

### 安装 Webpack
#### 安装命令
```
npm install webpack webpack-cli -g
```
#### 检验是否安装成功
```
webpack --version
```
## 构建项目的第二步：VUE-CLI
### VUE-CLI 是什么
VUE-CLI 是一个命令行工具，用官方的说法叫做 “脚手架”，我们可以使用它快速构建出一个完整的 VUE 项目。
### 安装 VUE-CLI
#### 安装
```
npm install -g @vue/cli
```
#### 检验
```
vue -V
```
#### 网络原因导致安装失败的解决办法
由于我国网络部署了防火墙的原因，所以有可能会安装失败，因此我们需要使用 VPN 来进行安装。  
如果没有 VPN 的读者，可以选择使用淘宝提供的 cnpm 镜像仓库进行安装。
##### cnpm 安装 vue-cli 教程如下
> https://github.com/shaolizhi1234/TIL-shaolizhi/blob/master/19-02-05-%E3%80%90vue-cli%E3%80%91%E4%BD%BF%E7%94%A8-cnpm-%E5%AE%89%E8%A3%85-vue-cli.md

### 使用 VUE-CLI 构建项目
```
vue init webpack {{project-name}}
```
> 请用您自己的项目名称代替{{project-name}}

### 运行项目
#### 运行
```
vue run dev
```
#### 浏览
在网页中打开 http://127.0.0.1:8080 即可看到

















