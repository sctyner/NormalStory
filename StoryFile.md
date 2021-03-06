What would happen if we never knew about the normal distribution?
========================================================

This story is a very sad story about a world without a Normal distribution.  As a statistician it is very difficult to imagine a world without the Normal distribution.  She is the queen of the distributions!  She is very elegant with a perfect symmetric shape, and a lot of the other curves aspire to her ideal unimodal and symmetric shape. Some of the other curves, like gamma or exponential, have a lot of asymmetry that is difficult to change.  


Here is our queen...


```r
normal <- rnorm(10000)
library(ggplot2)
qplot(normal, geom = "blank", main = "The Queen", xlab = "Value") + geom_histogram(aes(y = ..density..), 
    binwidth = 0.25) + stat_function(fun = dnorm, color = "red")
```

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-1.png) 

But what would a world without our queen be?? What would happen in a world that hadn't discovered this magic curve?  Suppose that we live in a world where people are holding our queen hostage.  These people are a terrible kind of evil hippie who are so dedicated to saving a few sheets of paper in the back of statistics textbooks that they have taken our queen hostage so that no one knows about her.  Without our queen, there's no need for normal quantile and p-value tables and many trees are rescued. They only think in rescue some trees but they don't know all the advantages in statistics that our queen give us.

These are our queen's evil captors!

<img src="http://flowerpower89.files.wordpress.com/2010/10/hippies.jpg" alt="Drawing" style="width: 400px;"/>

<!--  commented out original
![](http://flowerpower89.files.wordpress.com/2010/10/hippies.jpg =50x) 
-->

We may have saved some trees, but is this conservation of a few trees worth the cost of living without our queen?? 

What would happen to the Kindom of distributions?! The beautiful Queen was missing.  Would the distribution kingdom turn into a uniform democracy?

```r
x = c(rep(c(1:10), 5))
qplot(x, binwidth = 0.5)  # uniform distribution
```

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 

Many scientists performed experiments and could not tell if the results were significantly different from the Null Hypothesis, for most of them had only used the normal distribution.  The engineers were unable use the scientist's results to design or improve technology. A vast majority of statisticians became non-parametric statisticians for they were so devoted to their Normal Distribution Queen that none of the other distributions appealed to them.

In those dark times, it was revealed that the Queen had three children: two girls and a boy. Their mother had tried to keep them out of the spotlight, for they were merely students (student's t distributions) and were off at university getting their 30 required degrees.  From youngest to oldest, they had 3, 10 and 25 degrees (of freedom).

```r
c1 = rt(1e+05, 3)
qplot(c1, geom = "blank", main = "The Little Prince", xlab = "Value") + geom_histogram(aes(y = ..density..), 
    binwidth = 0.25) + stat_function(fun = dt, args = c(df = 3), color = "green") + 
    xlim(-10, 10)
```

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-31.png) 

```r
c2 = rt(1e+05, 10)
qplot(c2, geom = "blank", main = "The Younger Princess", xlab = "Value") + geom_histogram(aes(y = ..density..), 
    binwidth = 0.25) + stat_function(fun = dt, args = c(df = 10), color = "blue") + 
    xlim(-10, 10)
```

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-32.png) 

```r
c3 = rt(1e+05, 25)
qplot(c3, geom = "blank", main = "The Eldest Princess", xlab = "Value") + geom_histogram(aes(y = ..density..), 
    binwidth = 0.25) + stat_function(fun = dt, args = c(df = 25), color = "purple") + 
    xlim(-10, 10)
```

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-33.png) 

The scientists, the engineers, and especially the statisticians begged the students to come back and find their Queen mother and return the the world to its beautiful normalness.  So the three children left their studies and set out, crossing the waves of monotony...

```r
x = c(1:(100 * pi))/5
y = sin(x)
qplot(x, y, geom = "line")
```

![plot of chunk unnamed-chunk-4](figure/unnamed-chunk-4.png) 


But after months and months of this monotony, with their mother nowhere to be found, the eldest princess decided to give up the search and return to school.  Being the eldest, she decided that the best thing to do was to earn her last 5 degrees and take the throne, since she'd approximately be her mother after those 5 degrees. 

With their sister back at school, the little prince and the younger princess continued to search the kingdom for their mother. But the evil hippies had planted random forests all throughout the kingdom! The prince and princess got lost in a random forest and were immediately classified. Without the normal distributon to guide the random forest, the prince and princess were deemed to belong to two different groups, and were transported to opposite sides of the kingdom!


With the kingdom divided in two parts the normal princess show all her properties and the advantages in statistics to use the Normal family. For example she mention that the Normal distribution is very useful because of the central limit theorem, that says the mean of many random variables independently drawn from the same distribution is distributed approximately normally. She finish her exposition saying that the Normal distribution is the most important distribution in probability theory and if this kingdom want to be a prosper kingdom needs the normal distribution to survive.


On the opposite side of the kingdom, they were convinced they do not need the Normal distribution to survive and then they say that with a non parametric aproach they will solve all the problems that they have.
At the end these two kingdoms live happy with their different approach and people to each kingdom go on vacation to the other side to know the differences between these two approches.
And each year they make a huge party to celebrate their peaceful convivence.
 
 

"Colorin colorado" is the end of this story...

Here is the huge party...


```r
library(ggplot2)
x = rnorm(1000)
x1 = rgamma(1000, 1, 2)
x2 <- rpois(1000, 1)
x3 <- x1 + 5
x4 <- x2 + 5
x5 <- x + 5
x6 <- rchisq(1000, 4)
x7 <- x6 + 5
x8 <- rnorm(1000, 2, 18)
x9 <- x8 + 5
x10 <- x9 + 5
x11 <- rchisq(1000, 10)
x12 = rgamma(1000, 12, 20)
x13 <- x12 + 5
x14 <- x13 + 5
x15 <- x6 + 10
x16 <- x1 + 10

x = c(x, x1, x2, x3, x4, x5, x6, x7, x8, x9, x10, x11, x12, x13, x14, x15, x16)
qplot(x, binwidth = 0.1) + geom_histogram(aes(y = ..density..), binwidth = 0.25)
```

```
## Warning: position_stack requires constant width: output may be incorrect
```

![plot of chunk unnamed-chunk-5](figure/unnamed-chunk-5.png) 


