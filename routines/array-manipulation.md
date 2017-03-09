## （这里np代表numpy模块，ndarray代表数据块）

np.copyto\(`dst, src`, casting, where\) 数据块间拷贝。

### 改变数据块的形状

np.reshape\( `a, newshape`, order\)

np.ravel\( `a`, order\) 返回内存连续版

ndarray.flat           返回一个1D的迭代器

ndarray.flatten\( \)  返回一个1D的副本

### 类似转置的操作

np.moveaxis\( a, source, destination \)

np.rollaxis\( a, axis, start \)

np.swapaxes\( a, axis1, axis2\)

ndarray.T

transpose\( a, axes \)

### 改变维度

np.atleast\_1d\( \*arys \)

np.atleast\_2d\( \*arys \)

np.atleast\_3d\( \*arys \)

np.broadcast

np.broadcast\_to\( `array, shape`, subok\)

np.broadcast\_arrays\(\*args, \*\*kwargs\)

expand\_dims\(a, axis\)

squeeze\( a, axis\)

