---
title: '【VUE的component中，height:100%不管用】'
date: 'Sun, 5 May 2019 15:49:30 +0800'
stacks:
    - vue
    - html
    - stylus
---

解决方案：
在 APP.vue 的 style 块下面添加如下代码即可：
```
html, body, #app
  height 100%
```
原因：
这是因为 VUE 是一个大型单页应用，也就是说它只有一个 HTML 文件。
所有的 Component 都是 App.vue 的子节点，而 App.vue 的中所有的 height 默认都是 auto。

又因为子节点的 height:100% 是根据父节点的 height 来定的，父节点 auto 基本又是根据子节点的 height 定的。

于是不论是父节点的 height 还是子节点的 height 最后都变成了 0px。


