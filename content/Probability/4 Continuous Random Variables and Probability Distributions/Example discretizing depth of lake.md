Recall [[EX 4.1 depth of lake]]. 

Suppose the variable $X$ of interest is the depth of a lake at a randomly chosen point on the surface. 
Let $M =$ the maximum depth (in meters), so that any number in the interval $\left\lbrack {0, M}\right\rbrack$ is a possible value of $X$ . 
If we "discretize" $X$ by measuring depth to the nearest meter, then possible values are nonnegative integers less than or equal to $M$. 
The resulting discrete distribution of depth can be pictured using a probability histogram. 
If we draw the histogram so that the area of the rectangle above any possible integer $k$ is the proportion of the lake whose depth is (to the nearest meter) $k$ , then the total area of all rectangles is 1. 
A possible histogram appears in [[#^fig-4-1|Figure 4.1(a)]].

If depth is measured much more accurately and the same measurement axis as in Figure 4.1(a) is used, each rectangle in the resulting probability histogram is much narrower, though the total area of all rectangles is still 1. 
A possible histogram is pictured in [[#^fig-4-1|Figure 4.1(b)]]; it has a much smoother appearance than the histogram in Figure 4.1(a). 
If we continue in this way to measure depth more and more finely, the resulting sequence of histograms approaches a smooth curve, such as is pictured in [[#^fig-4-1|Figure 4.1(c)]]. 
Because for each histogram the total area of all rectangles equals 1, the total area under the smooth curve is also 1. 
The probability that the depth at a randomly chosen point is between $a$ and $b$ is just the area under the smooth curve between $a$ and $b$. 
It is exactly a smooth curve of the type pictured in Figure 4.1(c) that specifies a continuous probability distribution.

Figure 4.1 
(a) Probability histogram of depth measured to the nearest meter; 
(b) probability histogram of depth measured to the nearest centimeter; 
(c) a limit of a sequence of discrete histograms
![01925166-48c0-7eca-9860-67f13d0848b1_2_648_575_1100_243_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_2_648_575_1100_243_0.jpg)

^fig-4-1
