copyto\(`dst, src`, casting, where\) 数据块间拷贝。

### 改变数据块的形状

reshape\( `a, newshape`, order\) 改变数据块的形状  
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

concatenate\(\(a1, a2, ...\), axis\)  
stack\(arrays, axis\)  
column\_stack\(tup\)  
hstack\(tup\)  
vstack\(tup\)

### 拆分数据块 Splitting Arrays

split\(ary, indices\_or\_sections, axis\)  
array\_split\(ary, indices\_or\_sections, axis\)  
dsplit\(ary,indices\_or\_sections, axis\)  
hsplit\(ary, indices\_or\_sections, axis\)  
vsplit\(ary, indices\_or\_sections, axis\)

### 把小块数据铺成大块数据，像铺砖瓦一样 Tiling Arrays

tile\(A, reps\)  
repeat\(a, repeats, axis\)

### 添加和删除元素

delete\(arr, obj, axis\)  
insert\(arr, obj, values, axis\)  
append\(arr, values, axis\)  
resize\(a, new\_shape\)  
trim\_zeros\( filt, trim\)  
unique\(ar, return\_index, return\_inverse, ...\)

### 重新排列元素

flip\(m, axis\)  
fliplr\(m\)  
flipud\(m\)  
reshape\(a, newshape, order\)  
roll\(a, shift, axis\)  
rot90\(m, k, axes\)

