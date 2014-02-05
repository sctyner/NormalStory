What would happen if we never knew about the normal distribution?
========================================================

In a parellel dimension, the normal distribution was never discovered.  Therefore there was no sampling theory.  If you were studying sizes of oranges, you had to measure the sizes of ALL of the oranges. You had no idea if the next sample would also be normally distributed.  

hmm restart. 

1) Normal Distribution exists but is not discovered.
- the normal distribution is using samples to summarize the entire population.  Most of the population is near an average.
- therefore without a normal or any "distribution," researchers would have to measure the entire population. They could not assume that the next sample would match the current sample.

2) Normal Distribution does not exist.
- the world revolves around a uniform, gamma, exponential distribution, other
- maybe it doesn't even have a distribution
- non normal distributions: uniform, gamma, exponential, cycling (sin/cos, tangent etc)
- music

World 2:
- 


Non-Normal Distributions:
Uniform

```r
library(ggplot2)
x = c(rep(c(1:5), 5))
qplot(x)
```

```
## stat_bin: binwidth defaulted to range/30. Use 'binwidth = x' to adjust this.
```

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-1.png) 


Bimodal

```r
library(ggplot2)
x = rnorm(1000)
x1 = x + 5
x = c(x, x1)
qplot(x, )
```

```
## stat_bin: binwidth defaulted to range/30. Use 'binwidth = x' to adjust this.
```

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 



You can also embed plots, for example:


```r
plot(cars)
```

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-3.png) 


