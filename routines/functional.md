np.apply\_along\_axis\( func1d, axis, arr,  \*args, \*\*kwargs\)   
在arr数据块的axis轴向，用func1d\(a, \*args\)来处理. a是arr在axis轴的1-D slice.

apply\_over\_axes\(func, a,  axes\)  用func\(a,axis\)来处理a的多个axis

类 vectorize\(pyfunc, otypes=, doc=, excluded=, ...\)  将python函数“vectorize”化，实例可调用。

frompyfunc\( func, nin, nout\)     将python函数转换成ufunc

piecewise\(x, condlist, funclist, \*args, \*\*kw\) 给定一组条件，在条件为真时，执行每一个函数

