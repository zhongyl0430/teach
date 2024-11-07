Consider the distribution shown in Figure 5.17 for the amount purchased (rounded to the nearest dollar) by a randomly selected customer at a particular gas station (a similar distribution for purchases in Britain (in $\pounds$ ) appeared in the article "Data Mining for Fun and Profit," Statistical Science, 2000: 111-131; there were big spikes at the values, ${10},{15},{20},{25}$ , and 30). The distribution is obviously quite non-normal.

We asked Minitab to select 1000 different samples, each consisting of $n = {15}$ observations, and calculate the value of the sample mean $\bar{X}$ for each one. Figure 5.18 is a histogram of the resulting 1000 values; this is the approximate sampling distribution of $\bar{X}$ under the specified circumstances. This distribution is clearly approximately normal even though the sample size is actually much smaller than 30, our rule-of-thumb cutoff for invoking the Central Limit Theorem. As further evidence for normality, Figure 5.19 shows a normal probability plot of the ${1000}\bar{x}$ values; the linear pattern is very prominent. It is typically not nonnormality in the central part of the population distribution that causes the CLT to fail, but instead very substantial skewness.

Figure 5.17 
Probability distribution of X = amount of gasoline purchased ($)
![0192609f-6f5c-74c9-8588-c1ef28b2184d_36_211_1481_1434_752_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_36_211_1481_1434_752_0.jpg)

Figure 5.18 
Approximate sampling distribution of the sample mean amount purchased when $n = {15}$ and the population distribution is as shown in Figure 5.17
![0192609f-6f5c-74c9-8588-c1ef28b2184d_37_690_182_1028_433_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_37_690_182_1028_433_0.jpg)

Figure 5.19 
Normal probability plot from Minitab of the ${1000}\bar{x}$ values based on samples of size $n = {15}$
![0192609f-6f5c-74c9-8588-c1ef28b2184d_37_770_1032_882_599_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_37_770_1032_882_599_0.jpg)
