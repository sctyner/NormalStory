What would happen if we never knew about the normal distribution?
========================================================

<<<<<<< HEAD
This story is a very sad story about a world without a Normal distribution.  As a statistician it is very difficult to imagine a world without the Normal distribution.  She is the queen of the distributions!  She is very elegant with a perfect symmetric shape, and a lot of the other curves aspire to her ideal unimodal and symmetric shape. Some of the other curves, like gamma or exponential, have a lot of asymmetry that is difficult to change. 

Here is our queen…...
=======
<<<<<<< HEAD
This story is a very sad story about a world without a Normal distribution.  As statistician it is very difficult imagine a world without the Normal distribution.  She is the queen of the distributions is very elegant with a perfect symmetric shape and a lot of the other curves want to be  normal at the end. For some of the other curves it is very difficult because they have a lot of asymetry that it is difficult to change... 

=======
This story is a very sad story about a world without a Normal distribution.  As statistician it is very difficult imagine a world without the Normal distribution.  She is the queen of the distributions is very elegant with a perfect symmetric shape that some of the other curves want to reach at the end.
>>>>>>> e287cc64a8f9c9c607315cf81cb758151b6dd142
Here is our queen...
>>>>>>> 4b17ca7256e33f940c2b830df9db2c6563eb84ad


```r
normal <- rnorm(10000)
library(ggplot2)
qplot(normal, geom = "histogram", binwidth = 0.25) + geom_density(colour = "red")
```

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-1.png) 

But what would a world without our queen be?? What would happen in a world that hadn't discovered this magic curve?  Suppose that we live in a world where people are holding our queen hostage.  These people are at terrible kind of evil hippie who are so dedicated to saving a few sheets of tables in the back of statistics textbooks that they have taken our queen hostage so that no one knows about her.  So, there's no need for normal quantile and p-value tables and many trees are rescued. These are our queen's evil captors!
![](http://flowerpower89.files.wordpress.com/2010/10/hippies.jpg){width:20px}

<<<<<<< HEAD
We may have saved some trees, but is this conservation of a few trees worth the cost of living without our queen?? 
=======
<<<<<<< HEAD
=======
If the normal distribution had never been discovered, that would reduce the amount of tables in the back of every statistics books. All this saved paper would make all the Hippies very happy.

![](http://flowerpower89.files.wordpress.com/2010/10/hippies.jpg)
>>>>>>> 4b17ca7256e33f940c2b830df9db2c6563eb84ad

>>>>>>> e287cc64a8f9c9c607315cf81cb758151b6dd142

Could be the distruibution of 


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

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 


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

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-3.png) 



You can also embed plots, for example:


```r
plot(cars)
```

![plot of chunk unnamed-chunk-4](figure/unnamed-chunk-4.png) 



We know that at the end all the problems when we have enough information we get a Normal distribution. But what happened if the Normal distribution does not exists? This means that with a huge sample size for some specific problem we will not get our precious Normal curve? Mmmm  difficult to believe …….
