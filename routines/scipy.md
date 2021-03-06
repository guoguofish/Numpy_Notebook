Numpy实现了一些加速版的Scipy的API，即使你没有安装Scipy也可以使用这些函数。

### Linear algebra 线性代数

np.linalg.cholesky\( a \) 柯勒斯基分解

np.linalg.det\( a \) 计算行列式

np.linalg.eig\( a \)  计算一个方阵的特征值及特征向量

np.linalg.eigh\( a, UPLO='L' \)  返回 Hermitian 或 symmetric 矩阵的特征值和特征向量

np.linalg.eigvals\( a \) 计算矩阵的特征值

np.linalg.eigvalsh\( a \) 计算Hermitian 或 symmetric矩阵的特征值

np.linalg.inv\(a\) 计算逆矩阵

numpy.linalg.lstsq\( a, b, rcond=-1\) 线性矩阵方程的最小二乘解

np.linalg.norm\(x, ord, axis, keepdims\)

np.linalg.pinv\(a, rcond\)  计算 Moore-Penrose 伪逆矩阵

np.linalg.solve\(a, b\) 解线性方程 ax=b 的x

np.linalg.svd\(a, full\_matrics, compute\_uv\) 奇异值分解

### FFT 快速傅立叶变换

np.fft.fft\(a\) 计算1D离散傅立叶变换

np.fft.fft2\(a\)计算2D离散傅立叶变换

np.fft.fftn\(a\)计算nD离散傅立叶变换

np.fft.ifft\(a\)计算1D离散傅立叶反变换

np.fft.ifft2\(a\)计算2D离散傅立叶反变换

np.fft.ifftn\(a\)计算nD离散傅立叶反变换

### 其它

np.i0\( x \)

