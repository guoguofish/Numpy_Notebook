### NumPy 二进制文件 \(NPY, NPZ\)，支持pickle化

load\(file\[, mmap\_mode, allow\_pickle, ...\]\)   从npy或npz文件里载入数据或者 pickled 的对象  
save\(file, arr\[, allow\_pickle, fix\_imports\]\)   将一块数据 arr 保存到硬盘二进制文件 file.npy.  
savez\(file, \_args, \*\*kwds\)    把几个数组保存到一个没压缩的 file.npz文件  
savez\_compressed\(file, \_args, \*\*kwds\)    把几个数组保存到一个压缩了的 file.npz文件  
这些二进制文件的格式说明位于  [http://docs.scipy.org/doc/numpy/neps/npy-format.html](http://docs.scipy.org/doc/numpy/neps/npy-format.html)

### Text files

loadtxt\(fname\[, dtype, comments, delimiter, ...\]\)    Load data from a text file.  
savetxt\(fname, X\[, fmt, delimiter, newline, ...\]\)    Save an array to a text file.  
genfromtxt\(fname\[, dtype, comments, ...\]\)    Load data from a text file, with missing values handled as specified.  
fromregex\(file, regexp, dtype\)    Construct an array from a text file, using regular expression parsing.  
fromstring\(string\[, dtype, count, sep\]\)    A new 1-D array initialized from raw binary or text data in a string.  
ndarray.tofile\(fid\[, sep, format\]\)    Write array to a file as text or binary \(default\).  
ndarray.tolist\(\)    Return the array as a \(possibly nested\) list.

### Raw binary files

fromfile\(file\[, dtype, count, sep\]\)    Construct an array from data in a text or binary file.  
ndarray.tofile\(fid\[, sep, format\]\)    Write array to a file as text or binary \(default\).

### String formatting

array2string\(a\[, max\_line\_width, precision, ...\]\)    Return a string representation of an array.  
array\_repr\(arr\[, max\_line\_width, precision, ...\]\)    Return the string representation of an array.  
array\_str\(a\[, max\_line\_width, precision, ...\]\)    Return a string representation of the data in an array.

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

