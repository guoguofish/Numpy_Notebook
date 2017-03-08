之前介绍了ufun函数，看到它就应该立刻想到数据的**并行**处理。

并行我们理解它的含义，接下来就要看看这类函数到底都能干些什么事。根据其官方的文档，从以下几个方面介绍这些个并行的函数们。

1. math 一些基本的数学计算
2. Trigonometric 三角函数
3. Bit-twidding 位变换操作
4. Comparison 比较操作
5. Floating 浮点数处理

函数中有个可有可无的参数out, 他的意思是说你可以把计算结果放在out里面，不给出这个参数就返回结果。

out的shape要和计算结果匹配。加入out参数的好处是可以减少大数据长计算所产生的临时内存需求。

例如可以把G=A\*B+C改写成

```
 G=A*B
 add(G, C, G)
```


