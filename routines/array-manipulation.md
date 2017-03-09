copyto\(`dst, src`, casting, where\) 数据块间拷贝。

### 改变数据块的形状

reshape\( `a, newshape`, order\)

ravel\( `a`, order\) 返回内存连续版

ndarray.flat           返回一个1D的迭代器

ndarray.flatten\( \)  返回一个1D的副本

### 类似转置的操作

moveaxis\( a, source, destination \)

rollaxis\( a, axis, start \)

swapaxes\( a, axis1, axis2\)

ndarray.T

transpose\( a, axes \)

### 改变维度

atleast\_1d\( \*arys \)

atleast\_2d\( \*arys \)

atleast\_3d\( \*arys \)

broadcast

broadcast\_to\( `array, shape`, subok\)

broadcast\_arrays\(\*args, \*\*kwargs\)

expand\_dims\(a, axis\)

squeeze\( a, axis\)

### 改变数据块的种类

asarray\(a, dtype, order\)

asanyarray\(a, dtype, order\)

asmatrix\(data, dtype\)

asfarray\(a, dtype\)

asfortranarray\( a, dtype\)

ascontiguousarray\(a, dtype\)

asarray\_chkfinite\(a, dtype, order\)

asscalar\(a\)

require\( a, dtype, requirements \)

### 结合数据块 Joining Arrays

### 拆分数据块 Splitting Arrays

### 把小块数据铺成大块数据，像铺砖瓦一样 Tiling Arrays 

### 添加和删除元素

### 重新排列元素



