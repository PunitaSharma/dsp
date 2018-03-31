# [Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```python

import thinkstats2

d = { 7: 8, 12: 8, 17: 14, 22: 4,
     27: 6, 32: 12, 37: 8, 42: 3, 47: 2 }

pmf = thinkstats2.Pmf(d, label='actual')

def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)

    for x, p in pmf.Items():
        new_pmf.Mult(x, x)

    new_pmf.Normalize()
    return new_pmf

biased_pmf = BiasPmf(pmf, label='observed')

def UnbiasPmf(pmf, label=None):
    new_pmf = pmf.Copy(label=label)

    for x, p in pmf.Items():
        new_pmf[x] *= 1/x

    new_pmf.Normalize()
    return new_pmf

unbiased = UnbiasPmf(biased_pmf, label='unbiased')

print('Actual mean', pmf.Mean())
print('Observed mean', biased_pmf.Mean())
print('Unbiased mean', unbiased.Mean())
 
```
**  RESULTS: ** 
> > Actual mean 23.692307692307693


> > Observed mean 29.123376623376625


> > Unbiased mean 23.69230769230769
