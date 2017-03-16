之前介绍了ufun函数，看到它就应该立刻想到 数据的**并行**处理。

并行我们理解它的含义，接下来就要看看这类函数到底都能干些什么事。根据其官方的文档，从以下几个方面介绍这些个并行的函数们。

1. math 一些基本的数学计算
2. Trigonometric 三角函数
3. Bit-twidding 位变换操作
4. Comparison 比较操作
5. Floating 其它处理

这些函数中有个可有可无的参数out, 他的意思是说你可以把计算结果放在out里面，若没有这个参数就返回结果。

out的shape要和计算结果匹配。加入out参数的好处是可以减少大数据长计算所产生的临时内存需求。

例如可以把 G=A\*B+C 改写成

```
 G=A*B
 add(G, C, G)
```

在Python 里，任何函数都是对象，是对象就可以有属性，ufunc也不例外，它自身都一些数据属性和method。数据属性没什么好说的，但有4个method 比较有用, 

[ufunc.reduce](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ufunc.reduce.html#numpy.ufunc.reduce)\(a\[, axis, dtype, out, keepdims\]\)

|  | Reduces_a_‘s dimension by one, by applying ufunc along one axis. |
| :--- | :--- |
| [ufunc.accumulate](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ufunc.accumulate.html#numpy.ufunc.accumulate)\(array\[, axis, dtype, out, ...\]\) | Accumulate the result of applying the operator to all elements. |
| [ufunc.reduceat](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ufunc.reduceat.html#numpy.ufunc.reduceat)\(a, indices\[, axis, dtype, out\]\) | Performs a \(local\) reduce with specified slices over a single axis. |
| [ufunc.outer](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ufunc.outer.html#numpy.ufunc.outer)\(A, B, \*\*kwargs\) | Apply the ufunc_op_to all pairs \(a, b\) with a in_A_and b in_B_. |



