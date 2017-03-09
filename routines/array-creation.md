### 全0和全1的数据块

empty\( `shape`,      dtype,  order \)           创建一块空数据，没有初始化工作，节省时间

empty\_like\(** **`a`,      dtype, order, subok \)  创建一块空数据，它的shape和a.shape一样。

eye\(** **`N`,     M, k, dtype_ _\) 2D单位矩阵，对角线全1，其余为0

identity\( `n`,    dtype\) 单位矩阵

ones\( `shape`,  dtype, order \)            全1数据块

ones\_like\( `a`,  dtype, order, subok \) 全1数据块

zeros\( `shape`,  dtype, order \) 全0数据块

zeros\_like\( `a`,  dtype, order, subok \) 全0数据块

full\( `shape, fill_value`, dtype, order \) 全 fill-value 的数据块

fulllike\( `a, fill_value`,  dtype, order, subok \) 全 fill-value 的数据块

### 由外部数据转换而来

array\( `object`, dtype, copy, order, subok, ndmin \)  把python的一个object（通常是列表），转变成一个ndarray数据块。

asarray\( `a`,  dtype, order \)

asanyarray\( `a`, dtype, order \) 把ndarray的派生类数据块，转换成ndarray数据块。

ascontiguousarray\( `a`, dtype \) 让一块ndarray的数据在内存中紧凑起来。

asmatrix\( `data`,  dtype\) 将data转换成 matrix 矩阵类型

frombuffer\( `buffer`, dtype, count, offset \)

##### fromfile\( `file`, dtype, count, sep\)  和 ndarray.tofile\(file\) 配合使用

fromfunction\( `function`, shape, \*\*kwargs \) 用函数根据index坐标来生成数据块，函数的参数有几个，由shape决定。

fromiter\(`iterable, dtype`,    count\)   把python的可迭代对象转换成1D的数据

fromstring\( `string`, dtype, count, sep \)   把python的字符串转换成1D的数据

#### loadtxt 函数 和 savetxt 函数配合，支持gzip

loadtxt\( `fname`, dtype, comments,  delimiter, ... \)   从硬盘的 txt 文件载入数据，可自动识别gzip文件

savetxt\(`fname, X`, fmt='%.18e', delimiter='', newline='\n', header='', footer='', comments='\#'\) 将数据X保存到外部文件中去，如果fname以“.gz”结尾，文件将自动保存为压缩的gzip文件。

#### load 函数 和 save, savez, savez\_compressed函数配合，支持pickle

load\( `file`, mmap=None, allow\_pickle=True, fix\_imports=True, encoding='ASCII' \) 从npy或npz文件里载入数据,和下面的 save,  savez,  savez\_compressed函数配合使用。

save\( `file, arr`,   allowpickle=True, fix\_imports=True\) 将一块数据 arr 保存到硬盘二进制文件 xxx.npy

savez\( `file, *args`, \*\*kwds\)  将多个数据块保存到硬盘单一文件 xxx.npz里，不压缩。

savez\_compressed\( `file, *args`, \*\*kwds \)  压缩版 savez\( \)

## 创建 record arrays \(numpy.rec是numpy.core.records的别名\)

大多数情况下，一块ndarray里的每个元素都是一个标量数，但是它也可以是一个组和后的数据，我们把这样的ndarray数据叫作 结构化的ndarray数据。

下面这段代码的a数组里两个元素，每个元素由两个数据构成，我们称它为field，分别是x和y，对应的数据类型分别是int和float。

```
>>> import numpy as np
>>> a = np.array([(1,2.0), (1,2.0)], dtype=[('x',int),('y', float)])
>>> type(a)     # 返回 <class 'numpy.ndarray'>
>>> type(a[0])  # 这里竟然返回的是 <class 'numpy.void'>
>>> a['x']      # 返回全  int数的ndarray: [1, 1]
>>> a['y']      # 返回全float数的ndarray: [ 2., 2.]
```

但是像 a\['x'\] 这样写代码太麻烦了, 于是就引入了record 数组，它的数据类型是 recarray .

```
>>> ar = np.rec.array(a)
>>> type(ar)   # 返回 <class 'numpy.recarray'>
>>> ar.x   # 返回全  int数的ndarray: [1, 1]
>>> ar.y   # 返回全float数的ndarray: [ 2., 2.]
```

我们可以看到 ar.x 其实就是 a\['x'\] 的简写版。

np.rec.array\( `obj`,  dtype, shape, ... \) 把各种obj转换成一个 record 数据块。

np.rec.fromarrays\( `arrayList`,  dtype, ... \) 把python列表里的每个 array 合并成一个 record 数据块。

np.rec.fromrecords\( recList, dtype, ...\) 把python列表里的每个 reccord 合并成一个大 record 数据块。

