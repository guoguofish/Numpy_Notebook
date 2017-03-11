### 元素级位操作

bitwise\_and\(x1, x2\[, out\]\)    元素之间 AND 运算.  
bitwise\_or\(x1, x2\[, out\]\)      元素之间 OR 运算.  
bitwise\_xor\(x1, x2\[, out\]\)    元素之间 XOR 运算.  
invert\(x\[, out\]\)                      元素 取反 运算.  
left\_shift\(x, y \[, out\]\)            位向左移，右测补0.  相当于$$x_i * 2^{y_i}$$.  
right\_shift\(x1, x2\[, out\]\)       位向右移.  相当于$$x_i \div 2^{y_i}$$.

### Bit packing

packbits\(myarray, axis=-1\)        将myarray数据块打包成字节数据块，打包后的数组元素类型是uint8.  
myarray的数据元素是二值数据，要么是 0 或 1，要么是Ture 或 False. 

axis=-1可保持输入和输出的数据形状基本不变。

unpackbits\(myarray\[, axis\]\)    将一个 uint8 数据块里的每个字节转换成二值输出的数组

### 输出格式

binary\_repr\(num\[, width\]\)    将输入的整数转换成二进制字符串，width控制二进制字符串的宽度

