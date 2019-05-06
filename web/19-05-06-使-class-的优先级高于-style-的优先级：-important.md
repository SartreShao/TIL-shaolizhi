---
title: 使 class 的优先级高于 style 的优先级：!important
date: 'Mon, 6 May 2019 10:55:49 +0800'
stacks: []
---

在 WEB 中，外联样式的优先级是要低于内联样式的优先级的。
也就是说当我们的 class 与 style 都对一个属性进行设置之后，
生效的会是 style 的设置。

那么，我们在何时可以使 class 的优先级比 style 高呢？
答案是可以用关键字「!important」

>你只能试试 !important 了. 因为内联样式优先级高于外部引用样式. 而脚本修改样式的语句又高于以上两种.所以,如果脚本里用到了object.style.xxxx='xxx';的话,那你只能再用脚本修改,如果脚本是用document.write输出的话, !important 应该可以优先于内联样式.

```
.jqplot-table-legend {
    xxxx: xxxx!important;
}
```


