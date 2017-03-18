## Sorting

sort\(a\[, axis, kind, order\]\)        Return a sorted copy of an array.  
lexsort\(keys\[, axis\]\)                Perform an indirect sort using a sequence of keys.  
argsort\(a\[, axis, kind, order\]\)        Returns the indices that would sort an array.  
ndarray.sort\(\[axis, kind, order\]\)    Sort an array, in-place.  
msort\(a\)                            Return a copy of an array sorted along the first axis.  
sort\_complex\(a\)                                Sort a complex array using the real part first, then the imaginary part.  
partition\(a, kth\[, axis, kind, order\]\)        Return a partitioned copy of an array.  
argpartition\(a, kth\[, axis, kind, order\]\)    Perform an indirect partition along the given axis using the algorithm specified by the kind keyword.

## Searching

argmax\(a\[, axis, out\]\)    返回的是数据块里的最大值的index.如果没有给出axis轴向参数，那么a就被扁平化成1D,然后再返回最大值index.如果给出axis值，那么返回的就是在那个轴向上的最大值的index.

```
np.argmax(np.array([0,0,0,0,0, 1,0,0,0,0])) # 返回 5
a = np.array([0,1,2, 2,2,8]).reshape(2,3)
np.argmax(a, axis=0) # 返回 [1,1,1]
np.argmax(a, axis=1) # 返回 [2,2]
np.argmax(np.array([0,5,1,2,3,4,5]))  #有两个最大值， 只返回 1
```

nanargmax\(a\[, axis\]\)    Return the indices of the maximum values in the specified axis ignoring NaNs.  
argmin\(a\[, axis, out\]\)    返回的是数据块里的最小值的index。  
nanargmin\(a\[, axis\]\)    Return the indices of the minimum values in the specified axis ignoring NaNs.  
argwhere\(a\)    Find the indices of array elements that are non-zero, grouped by element.  
nonzero\(a\)    Return the indices of the elements that are non-zero.  
flatnonzero\(a\)    Return indices that are non-zero in the flattened version of a.  
where\(condition, \[x, y\]\)    Return elements, either from x or y, depending on condition.  
searchsorted\(a, v\[, side, sorter\]\)    Find indices where elements should be inserted to maintain order.  
extract\(condition, arr\)    Return the elements of an array that satisfy some condition.

## Counting

count\_nonzero\(a\[, axis\]\)    Counts the number of non-zero values in the array a.

