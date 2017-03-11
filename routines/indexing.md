### 生成index数组

c\_  沿着第二个轴连接数据块，np.c\[arr1, arr2, ...\]  
r\_  沿着第一个轴连接数据块。  
s\_  为数据构造更好的 index 元组。
例如 >>> np.array([0, 1, 2, 3, 4])[np.s_[2::2]]  # array([2, 4])
nonzero\( a \)  
where\( condition \[, x, y\] \)  
indices\(dimensions\[, dtype\]\)  
ix\_\(\*args\)  
ogrid  
ravel\_multi\_index\(multi\_index, dims\[, mode, ...\]\)  
unravel\_index\(indices, dims\[, order\]\)  
diag\_indices\(n\[, ndim\]\)  
diag\_indices\_from\(arr\)  
mask\_indices\(n, mask\_func\[, k\]\)  
tril\_indices\(n\[, k, m\]\)  
tril\_indices\_from\(arr\[, k\]\)  
triu\_indices\(n\[, k, m\]\)  
triu\_indices\_from\( arr\[, k\] \)

### 类似index的操作

take\(a, indices \[,axis, out, mode\]\)  
choose\(a, choices \[,out, mode\]\)  
compress\(condition, a \[, axis, out\]\)  
diag\(v,  \[ k \]\)  
diagonal\(a \[,offset, axis1, axis2\]\)  
select\( condlist, choicelist  \[, default\] \)

### 插入数据

place\(arr, mask, vals\)  
put\(a, ind, v  \[, mode\]\)  
putmask\(a, mask, values\)  
fill\_diagonal\(a, val   \[, wrap\]\)

### 迭代遍历数据

nditer  
ndenumerate\( arr \)  
ndindex\(\*shape\)  
flatiter  
lib.Arrayterator\( var \[, buf\_size\]\)

