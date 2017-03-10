##### 这里的函数都位于 np.fft 模块

### 离散傅立叶变换

np.fft.fft\(a\) 计算1D离散傅立叶变换

np.fft.fft2\(a\)计算2D离散傅立叶变换

np.fft.fftn\(a\)计算nD离散傅立叶变换

np.fft.ifft\(a\)计算1D离散傅立叶反变换

np.fft.ifft2\(a\)计算2D离散傅立叶反变换

np.fft.ifftn\(a\)计算nD离散傅立叶反变换

## Real FFTs

rfft\( a , n=, axis=, norm= \) 计算1D离散傅立叶变换，输入的是 real-valued array

irfft\( a, n=, axis=, norm= \) 1D反变换

tfft2\( a, s=, axes=, norm= \) 计算2D离散傅立叶变换

irfft2\( a, s=, axes=, norm= \) 2D反变换

rfftn\( a, s=, axes=, norm= \) 计算nD离散傅立叶变换

irfftn\( a, s=, axes=, norm= \) nD反变换

## Hermitian FFTs

hfft\( a, n=, axis=, norm= \) 计算具有Hermitian对称性的信号的real频谱

ihfft\( a, n=, axis=, norm= \) 逆变换

## 帮助程序

fftfreq\(n, d=1.0\)  返回离散傅立叶变换的一组频率

rfftfreq\(n, d\)

fftshift\(x, axes\) 把0频移到频谱的中间

ifftshift\(x, axes\)   是fftshift的逆运算

