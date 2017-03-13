## Simple random data

rand\(d0, d1, ..., dn\)    根据shape参数产生随机值。下图是一个2000个2D随机点的例子，随机值分布在0-1之间.

![rand\(shape参数\)](/assets/np_random_rand.png)  
randn\(d0, d1, ..., dn\)    根据shape参数产生随机值.下图是一个2000个2D随机点的例子，可见随机值的分布符合正态分布。

![randn\(shape参数\)](/assets/np_random_randn.png)  
randint\(low\[, high, size, dtype\]\)    从low到high生成随机整数，size相当于shape参数  
random\_integers\(low\[, high, size\]\)   废弃。使用上者。  
random\_sample\(\[size\]\)    产生 \[0.0, 1.0\).之间随机小数，分布像rand，size相当于shape元组参数  
random\(\[size\]\)     同random\_sample  
ranf\(\[size\]\)           同random\_sample  
sample\(\[size\]\)     同random\_sample  
choice\(a\[, size, replace, p\]\)    输入a可以是 1-D的数据串，或者是一个整数n，代表arange\(n\)  
       size代表在a里选择了几次数据.   p.shape=a.shape, p里的元素对应a里相应元素的选中概率.  
       返回的数据也是1-D  
bytes\(length\)    返回length个字节.内容是随机的，也可以认为是乱码。

## Permutations随机排列

np.random.shuffle\(x\)     \[in-place\] 随机打乱数据的排列顺序，对于多维数组，只打乱第一个维度。  
permutation\(x\)    随即打乱一个序列数据, 或返回一个打乱的范围数据, 有点像arange\(x\)。对于多维数组，只打乱第一个维度。

## Distributions 分布

beta\(a, b\[, size\]\)    Beta 分布样本，在 \[0, 1\]内.  
binomial\(n, p\[, size\]\)    二项分布.  
chisquare\(df\[, size\]\)    卡方分布 .  
dirichlet\(alpha\[, size\]\)    狄利克雷分布.  
exponential\(\[scale, size\]\)    指数分布.  
f\(dfnum, dfden\[, size\]\)    F分布.  
gamma\(shape\[, scale, size\]\)    伽马分布.  
geometric\(p\[, size\]\)    几何分布.  
gumbel\(\[loc, scale, size\]\)    耿贝尔分布  
hypergeometric\(ngood, nbad, nsample\[, size\]\)   超几何分布.  
laplace\(\[loc, scale, size\]\)    拉普拉斯或双指数分布 with specified location \(or mean\) and scale \(decay\).  
logistic\(\[loc, scale, size\]\)    Logistic分布 .  
lognormal\(\[mean, sigma, size\]\)    对数正态分布.  
logseries\(p\[, size\]\)    对数级数分布.  
multinomial\(n, pvals\[, size\]\)   多项正态分布.  
multivariate\_normal\(mean, cov\[, size\]\)    多元正态分布  
negative\_binomial\(n, p\[, size\]\)    负二项分布.  
noncentral\_chisquare\(df, nonc\[, size\]\)    非中心卡方分布.  
noncentral\_f\(dfnum, dfden, nonc\[, size\]\)    非中心F分布.  
normal\(\[loc, scale, size\]\)   正态\(高斯\)分布   
pareto\(a\[, size\]\)    帕累托（Lomax）分布.  
poisson\(\[lam, size\]\)    泊松分布.  
power\(a\[, size\]\)    Draws samples in \[0, 1\] from a power distribution with positive exponent a - 1.  
rayleigh\(\[scale, size\]\)    Draw samples from a Rayleigh distribution.  
standard\_cauchy\(\[size\]\)    标准柯西分布 with mode = 0.  
standard\_exponential\(\[size\]\)    标准的指数分布.  
standard\_gamma\(shape\[, size\]\)    标准伽马分布.  
standard\_normal\(\[size\]\)   标准正态分布 \(mean=0, stdev=1\).  
standard\_t\(df\[, size\]\)    Draw samples from a standard Student’s t distribution with df degrees of freedom.  
triangular\(left, mode, right\[, size\]\)    三角分布 over the interval \[left, right\].  
uniform\(\[low, high, size\]\)    均匀分布.  
vonmises\(mu, kappa\[, size\]\)    von Mises分布  
wald\(mean, scale\[, size\]\)    瓦尔德（逆高斯）分布.  
weibull\(a\[, size\]\)    Weibull 分布.  
zipf\(a\[, size\]\)    齐普夫分布.

## 随机生成器

RandomState    Container for the Mersenne Twister pseudo-random number generator.  
seed\(\[seed\]\)    Seed the generator.  
get\_state\(\)    Return a tuple representing the internal state of the generator.  
set\_state\(state\)    Set the internal state of the generator from a tuple.

