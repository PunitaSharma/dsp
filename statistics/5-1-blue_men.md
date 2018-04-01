# [Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

``` python
import scipy.stats

mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)

dist.mean(), dist.std()
low = dist.cdf(177.8)    # 5'10"
high = dist.cdf(185.4)   # 6'1"
print('{:.1%}'.format(high-low))
```
**RESULT: **
> > 34.2%
