add\(x, y \[, out\]\)             返回 $$x_i + y_i$$

subtract\(x, y \[, out\]\)     返回 $$x_i - y_i$$

multiply\(x, y \[, out\]\)      返回 $$x_i * y_i$$

divide\(x, y \[, out\]\)         返回 $$x_i \div y_i$$

logaddexp\(x, y \[, out\]\)      求 $$ln(e^{x_i}+e^{y_i})$$

logaddexp2\(x, y \[, out\]\)    求$$log_2{(2^{x_i} + 2^{y_i})}$$

true\_divide\(x1, x2\[, out\]\)     返回 x1 / x2 （真除法）的结果。

floor\_divide\(x1, x2\[, out\]\)    返回 x1 / x2 （地板除）的结果。返回左侧最靠近的整数。

negative\(x\[, out\]\)      求负

power\(x, y \[, out\]\)     求$$x_i^{y_i}$$幂远算

remainder\(x1, x2\[, out\]\)    返回 x1 / x2 的余数

mod\(x1, x2\[, out\]\)             返回 x1 / x2 的余数

fmod\(x1, x2\[, out\]\)           返回 x1 / x2 的余数

absolute\(x\[, out\]\)    求元素值的绝对值; 如果元素是复数，比如a+bj来说,  这个函数就求解模 $$\sqrt{a^2+b^2}$$

fabs\(x\[, out\]\)           求x里元素的绝对值，不能处理复数

rint\(x\[, out\]\)       求最近的整数，即四舍五入取整

sign\(x\[, out\]\)      返回符号，-1, 0, 1

conj\(x\[, out\]\)      求共轭复数

exp\(x\[, out\]\)        计算 $$e^{x_i}$$

exp2\(x\[, out\]\)      计算 $$2^{x_i}$$

log\(x\[, out\]\)         求自然对数 $$\ln(x_i)$$

log2\(x\[, out\]\)       求对数 $$log_2^{x_i}$$

log10\(x\[, out\]\)     求对数 $$\log_{10}^{x_i}$$

expm1\(x\[, out\]\)   计算 $$e^{x_i}-1$$

log1p\(x\[, out\]\)     求自然对数 $$\ln(x_i+1)$$

sqrt\(x\[, out\]\)        平方根$$\sqrt{x_i}$$

square\(x\[, out\]\)   平方$${x_i}^2$$

cbrt\(x\[, out\]\)        立方根 $$\sqrt[3]{x_i}$$

reciprocal\(x\[, out\]\)    倒数$$\dfrac{1}{x_i}$$,  注意，$$x_i$$最好不要使用整数，因为python的除法问题会导致结果为0。

