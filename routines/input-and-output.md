### NumPy 二进制文件 \(NPY, NPZ\)，支持pickle化

load\(file\[, mmap\_mode, allow\_pickle, ...\]\)   从npy或npz文件里载入数据或者 pickled 的对象  
save\(file, arr\[, allow\_pickle, fix\_imports\]\)   将一块数据 arr 保存到硬盘二进制文件 file.npy.  
savez\(file, \_args, \*\*kwds\)    把几个数组保存到一个没压缩的 file.npz文件  
savez\_compressed\(file, \_args, \*\*kwds\)    把几个数组保存到一个压缩了的 file.npz文件  
这些二进制文件的格式说明位于  [http://docs.scipy.org/doc/numpy/neps/npy-format.html](http://docs.scipy.org/doc/numpy/neps/npy-format.html)

### Text files

loadtxt\(fname\[, dtype, comments, delimiter, ...\]\)    从text文件读取数据  
savetxt\(fname, X\[, fmt, delimiter, newline, ...\]\)    将数据X保存到 .txt 文件里  
genfromtxt\(fname, ...\)    分析外部text文件生成数据, 可特殊处理缺失的值. 许多可选参数是用来分析文件的.  
fromregex\(file, regexp, dtype\)    从一个text文件构建一块结构化数据，使用正则表达式分析，正则表达式的分组会转化为结构化数据里的field字段  
fromstring\(string\[, dtype, count, sep\]\)    将字符串转换成1-D的数据串。  
ndarray.tofile\(fid\[, sep, format\]\)    将数据写入文件.   
ndarray.tolist\(\)    将数据块转换成 python list列表.

### Raw binary files

fromfile\(file\[, dtype, count, sep\]\)   读取（txt 或 binary）文件，返回数据块.  
ndarray.tofile\(fid\[, sep, format\]\)    将数据块保存到文件fid.

### String formatting

array2string\(a\[, max\_line\_width, precision, ...\]\)    将数据转换成可以格式化的字符串.  
array\_repr\(arr\[, max\_line\_width, precision, ...\]\)     返回数据字符串和其他信息. 内部使用 array2string函数  
array\_str\(a\[, max\_line\_width, precision, ...\]\)          返回数据字符串. 内部使用 array2string函数

### Memory mapping files

memmap    Create a memory-map to an array stored in a binary file on disk.

### Text formatting options

set\_printoptions\(\[precision, threshold, ...\]\)    Set printing options.  
get\_printoptions\(\)    Return the current print options.  
set\_string\_function\(f\[, repr\]\)    Set a Python function to be used when pretty printing arrays.

### Base-n representations

binary\_repr\(num\[, width\]\)    Return the binary representation of the input number as a string.  
base\_repr\(number\[, base, padding\]\)    Return a string representation of a number in the given base system.  
Data sources  
DataSource\(\[destpath\]\)    A generic data source file \(file, http, ftp, ...\).

