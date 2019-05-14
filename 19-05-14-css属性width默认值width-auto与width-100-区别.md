---
title: 'css属性width默认值width: auto与width: 100%区别'
date: 'Tue, 14 May 2019 16:57:34 +0800'
stacks: []
---

#  width: auto  
- 子元素（包括content+padding+border+margin）撑满整个父元素的content区域。  
- 子元素有margin、border、padding时，会减去子元素content区域相对应的width值  
- 父元素的content = 子元素（content + padding + border + margin )  
# width: 100%  
- 强制将子元素的content区域 撑满 父元素的content区域  
- 子元素有margin、border、padding时，不改变子元素content区域的width，而是溢出父盒子，保持原有值  
- 父元素的content = 子元素的content  
---------------------  
作者：dreamer_zhou 
来源：CSDN 
原文：https://blog.csdn.net/wq_zhou/article/details/78220634 
版权声明：本文为博主原创文章，转载请附上博文链接！Write some content...


