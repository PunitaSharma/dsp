# [Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```python

from __future__ import print_function, division
import first
import math

live, firsts, others = first.MakeFrames()

def CohenEffectSize(group1, group2):
    diff = group1.mean() - group2.mean()
    var1 = group1.var()
    var2 = group2.var()
    n1, n2 = len(group1), len(group2)
    pooled_var = (n1 * var1 + n2 * var2) / (n1 + n2)
    d = diff / math.sqrt(pooled_var)
    return d

CohenEffectSize(firsts.prglngth, others.prglngth)

```
**  RESULTS: ** 
> > 0.028879044654449883
