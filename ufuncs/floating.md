isfinite\( x  \[, out\] \) 判断是不是NaN 和无穷大数据

isinf\( x  \[, out\] \)     判断是不是无穷大数据

isnan\( x  \[, out\] \)   判断是不是NaN

signbit\( x  \[, out\] \) 判断是否为负数

copysign\( x, y \[,out\] \) 将 x 的符号复制给 y

nextafter\( x, y \[,out\] \)

spacing\( x  \[, out\] \)

modf\( x  \[, out1, out2\] \) 返回一个元组\( x的小数部分， x的整数部分\)

ldexp\( x, y \[,out\] \) 计算 $${x_i} * 2^{y_i}$$

frexp\( x \[, out1, out2\] \) 将x的元素分解为尾数和二进制指数。返回 \(尾数out1，二进制指数out2\) 。符合 $$x = out1*2^{out2}$$

可见 ldexp 函数和 frexp 函数互为逆运算。

floot\( x  \[, out\] \) 返回左整数

ceil\( x  \[, out\] \)   返回右整数

trunc\( x  \[, out\] \) 四舍五入取整

