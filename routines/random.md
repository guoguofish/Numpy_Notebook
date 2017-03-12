## Simple random data

rand\(d0, d1, ..., dn\)    根据shape参数产生随机值。下图是一个2000个2D随机点的例子，随机值分布在0-1之间.

![](/assets/np_random_rand.png)  
randn\(d0, d1, ..., dn\)    根据shape参数产生随机值.下图是一个2000个2D随机点的例子，可见随机值的分布符合正态分布。

![](/assets/np_random_randn.png)  
randint\(low\[, high, size, dtype\]\)    从low到high生成随机整数，size相当于shape参数  
random\_integers\(low\[, high, size\]\)   废弃。使用上者。  
random\_sample\(\[size\]\)    产生 \[0.0, 1.0\).之间随机小数，分布像rand，size相当于shape元组参数  
random\(\[size\]\)    同random\_sample  
ranf\(\[size\]\)      同random\_sample  
sample\(\[size\]\)    同random\_sample  
choice\(a\[, size, replace, p\]\)    输入a可以是 1-D的数据串，或者是一个整数n，代表arange\(n\)  
       size代表在a里选择了几次数据.   p.shape=a.shape, p里的元素对应a里相应元素的选中概率.  
       返回的数据也是1-D  
bytes\(length\)    返回length个字节.内容是随机的，也可以认为是乱码。

## Permutations随机排列

np.random.shuffle\(x\)     \[in-place\] 随机打乱数据的排列顺序，对于多维数组，只打乱第一个维度。  
permutation\(x\)    随即打乱一个序列数据, 或返回一个打乱的范围数据, 有点像arange\(x\)。对于多维数组，只打乱第一个维度。

## Distributions 分布

beta\(a, b\[, size\]\)    Draw samples from a Beta distribution.  
binomial\(n, p\[, size\]\)    Draw samples from a binomial distribution.  
chisquare\(df\[, size\]\)    Draw samples from a chi-square distribution.  
dirichlet\(alpha\[, size\]\)    Draw samples from the Dirichlet distribution.  
exponential\(\[scale, size\]\)    Draw samples from an exponential distribution.  
f\(dfnum, dfden\[, size\]\)    Draw samples from an F distribution.  
gamma\(shape\[, scale, size\]\)    Draw samples from a Gamma distribution.  
geometric\(p\[, size\]\)    Draw samples from the geometric distribution.  
gumbel\(\[loc, scale, size\]\)    Draw samples from a Gumbel distribution.  
hypergeometric\(ngood, nbad, nsample\[, size\]\)    Draw samples from a Hypergeometric distribution.  
laplace\(\[loc, scale, size\]\)    Draw samples from the Laplace or double exponential distribution with specified location \(or mean\) and scale \(decay\).  
logistic\(\[loc, scale, size\]\)    Draw samples from a logistic distribution.  
lognormal\(\[mean, sigma, size\]\)    Draw samples from a log-normal distribution.  
logseries\(p\[, size\]\)    Draw samples from a logarithmic series distribution.  
multinomial\(n, pvals\[, size\]\)    Draw samples from a multinomial distribution.  
multivariate\_normal\(mean, cov\[, size\]\)    Draw random samples from a multivariate normal distribution.  
negative\_binomial\(n, p\[, size\]\)    Draw samples from a negative binomial distribution.  
noncentral\_chisquare\(df, nonc\[, size\]\)    Draw samples from a noncentral chi-square distribution.  
noncentral\_f\(dfnum, dfden, nonc\[, size\]\)    Draw samples from the noncentral F distribution.  
normal\(\[loc, scale, size\]\)    Draw random samples from a normal \(Gaussian\) distribution.  
pareto\(a\[, size\]\)    Draw samples from a Pareto II or Lomax distribution with specified shape.  
poisson\(\[lam, size\]\)    Draw samples from a Poisson distribution.  
power\(a\[, size\]\)    Draws samples in \[0, 1\] from a power distribution with positive exponent a - 1.  
rayleigh\(\[scale, size\]\)    Draw samples from a Rayleigh distribution.  
standard\_cauchy\(\[size\]\)    Draw samples from a standard Cauchy distribution with mode = 0.  
standard\_exponential\(\[size\]\)    Draw samples from the standard exponential distribution.  
standard\_gamma\(shape\[, size\]\)    Draw samples from a standard Gamma distribution.  
standard\_normal\(\[size\]\)    Draw samples from a standard Normal distribution \(mean=0, stdev=1\).  
standard\_t\(df\[, size\]\)    Draw samples from a standard Student’s t distribution with df degrees of freedom.  
triangular\(left, mode, right\[, size\]\)    Draw samples from the triangular distribution over the interval \[left, right\].  
uniform\(\[low, high, size\]\)    Draw samples from a uniform distribution.  
vonmises\(mu, kappa\[, size\]\)    Draw samples from a von Mises distribution.  
wald\(mean, scale\[, size\]\)    Draw samples from a Wald, or inverse Gaussian, distribution.  
weibull\(a\[, size\]\)    Draw samples from a Weibull distribution.  
zipf\(a\[, size\]\)    Draw samples from a Zipf distribution.

## 随机生成器

RandomState    Container for the Mersenne Twister pseudo-random number generator.  
seed\(\[seed\]\)    Seed the generator.  
get\_state\(\)    Return a tuple representing the internal state of the generator.  
set\_state\(state\)    Set the internal state of the generator from a tuple.

