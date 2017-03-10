[fv](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fv.html#numpy.fv)\(rate, nper, pmt, pv, when= \) 计算未来值

[pv](https://docs.scipy.org/doc/numpy/reference/generated/numpy.pv.html#numpy.pv)\(rate, nper, pmt, fv=, when=\) 计算当前值

[npv](https://docs.scipy.org/doc/numpy/reference/generated/numpy.npv.html#numpy.npv)\(rate, values\) 返回现金流系列的NPV\(净现值\)

[pmt](https://docs.scipy.org/doc/numpy/reference/generated/numpy.pmt.html#numpy.pmt)\(rate, nper, pv, fv=, when=\) 为偿还贷款\(本金+利息\)，计算还款额

[ppmt](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ppmt.html#numpy.ppmt)\(rate, per, nper, pv, fv=, when=\) 为偿还贷款，计算还款额的本金部分

[ipmt](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ipmt.html#numpy.ipmt)\(rate, per, nper, pv\[, fv, when\]\) 为偿还贷款,计算还款额的利息部分

[irr](https://docs.scipy.org/doc/numpy/reference/generated/numpy.irr.html#numpy.irr)\(values\)  当NPV=0时，返回复合收益率，类似平均后最终的收益率。

[mirr](https://docs.scipy.org/doc/numpy/reference/generated/numpy.mirr.html#numpy.mirr)\(values, finance\_rate, reinvest\_rate\) 修改版的irr

[nper](https://docs.scipy.org/doc/numpy/reference/generated/numpy.nper.html#numpy.nper)\(rate, pmt, pv, fv=, when=\) 计算还款时间。

[rate](https://docs.scipy.org/doc/numpy/reference/generated/numpy.rate.html#numpy.rate)\(nper, pmt, pv, fv, when=, guess=, tol=, maxiter=\) 计算周期利率

