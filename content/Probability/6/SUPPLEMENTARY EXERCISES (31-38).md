## SUPPLEMENTARY EXERCISES (31-38)

31. An estimator $\widehat{\theta }$ is said to be consistent if for any $\epsilon > 0$ , $P\left( {\left| {\widehat{\theta } - \theta }\right| \geq \epsilon }\right) \rightarrow 0$ as $n \rightarrow \infty$ . That is, $\widehat{\theta }$ is consistent if, as the sample size gets larger, it is less and less likely that $\widehat{\theta }$ will be further than $\epsilon$ from the true value of $\theta$ . Show that $\bar{X}$ is a consistent estimator of $\mu$ when ${\sigma }^{2} < \infty$ by using Chebyshev's inequality from Exercise 44 of Chapter 3. [Hint: The inequality can be rewritten in the form

$$
P\left( {\left| {Y - {\mu }_{Y}}\right| \geq \epsilon }\right) \leq {\sigma }_{Y}^{2}/\epsilon
$$

Now identify $Y$ with $\bar{X}$ .]

32. a. Let ${X}_{1},\ldots ,{X}_{n}$ be a random sample from a uniform distribution on $\left\lbrack {0,\theta }\right\rbrack$ . Then the mle of $\theta$ is $\widehat{\theta } = Y = \max \left( {X}_{i}\right)$ . Use the fact that $Y \leq y$ iff each ${X}_{i} \leq y$ to derive the cdf of $Y$ . Then show that the pdf of $Y = \max \left( {X}_{i}\right)$ is

$$
{f}_{Y}\left( y\right) = \left\{ \begin{matrix} \frac{n{y}^{n - 1}}{{\theta }^{n}} & 0 \leq y \leq \theta \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

b. Use the result of part (a) to show that the mle is biased but that $\left( {n + 1}\right) \max \left( {X}_{i}\right) /n$ is unbiased.

33. At time $t = 0$ , there is one individual alive in a certain population. A pure birth process then unfolds as follows. The time until the first birth is exponentially distributed with parameter $\lambda$ . After the first birth, there are two individuals alive. The time until the first gives birth again is exponential with parameter $\lambda$ , and similarly for the second individual. Therefore, the time until the next birth is the minimum of two exponential $\left( \lambda \right)$ variables, which is exponential with parameter ${2\lambda }$ . Similarly, once the second birth has occurred, there are three individuals alive, so the time until the next birth is an exponential rv with parameter ${3\lambda }$ , and so on (the memoryless property of the exponential distribution is being used here). Suppose the process is observed until the sixth birth has occurred and the successive birth times are ${25.2},{41.7},{51.2},{55.5},{59.5}$ , 61.8 (from which you should calculate the times between successive births). Derive the mle of $\lambda$ . [Hint: The likelihood is a product of exponential terms.]

34. The mean squared error of an estimator $\widehat{\theta }$ is MSE $\left( \widehat{\theta }\right) = E{\left( \widehat{\theta } - \widehat{\widehat{\theta }}\right) }^{2}$ . If $\widehat{\theta }$ is unbiased, then $\operatorname{MSE}\left( \widehat{\theta }\right) = V\left( \widehat{\theta }\right)$ , but in general $\operatorname{MSE}\left( \widehat{\theta }\right) = V\left( \widehat{\theta }\right) + {\left( \text{bias}\right) }^{2}$ . Consider the estimator ${\widehat{\sigma }}^{2} = K{S}^{2}$ , where ${S}^{2} =$ sample variance. What value of $K$ minimizes the mean squared error of this estimator when the population distribution is normal? [Hint: It can be shown that

$$
E\left\lbrack {\left( {S}^{2}\right) }^{2}\right\rbrack = \left( {n + 1}\right) {\sigma }^{4}/\left( {n - 1}\right)
$$

In general, it is difficult to find $\widehat{\theta }$ to minimize $\operatorname{MSE}\left( \widehat{\theta }\right)$ , which is why we look only at unbiased estimators and minimize $V\left( \widehat{\theta }\right)$ .]

35. Let ${X}_{1},\ldots ,{X}_{n}$ be a random sample from a pdf that is symmetric about $\mu$ . An estimator for $\mu$ that has been found to perform well for a variety of underlying distributions is the Hodges-Lehmann estimator. To define it, first compute for each $i \leq j$ and each $j = 1,2,\ldots , n$ the pairwise average ${\bar{X}}_{i, j} = \left( {{X}_{i} + {X}_{j}}\right) /2$ . Then the estimator is $\widehat{\mu } =$ the median of the ${\bar{X}}_{i, j}$ ’s. Compute the value of this estimate using the data of Exercise 44 of Chapter 1. [Hint: Construct a square Use this to obtain an unbiased estimator for $\sigma$ of the form ${cS}$ . What is $c$ when $n = {20}$ ?

38. Each of $n$ specimens is to be weighed twice on the same scale. Let ${X}_{i}$ and ${Y}_{i}$ denote the two observed weights for the $i$ th specimen. Suppose ${X}_{i}$ and ${Y}_{i}$ are independent of one another, each normally distributed with mean value ${\mu }_{i}$ (the true weight of specimen $i$ ) and variance ${\sigma }^{2}$ .

a. Show that the maximum likelihood estimator of ${\sigma }^{2}$ is ${\widehat{\sigma }}^{2} = \sum {\left( {X}_{i} - {Y}_{i}\right) }^{2}/\left( {4n}\right)$ . [Hint: If $\bar{z} = \left( {{z}_{1} + {z}_{2}}\right) /2$ , then $\sum {\left( {z}_{i} - \bar{z}\right) }^{2} = {\left( {z}_{1} - {z}_{2}\right) }^{2}/2$ .]

b. Is the mle ${\widehat{\sigma }}^{2}$ an unbiased estimator of ${\sigma }^{2}$ ? Find an unbiased estimator of ${\sigma }^{2}$ . [Hint: For any rv $Z$ , $E\left( {Z}^{2}\right) = V\left( Z\right) + {\left\lbrack E\left( Z\right) \right\rbrack }^{2}$ . Apply this to $Z = {X}_{i} - {Y}_{i}$ .] table with the ${x}_{i}$ ’s listed on the left margin and on top. Then compute averages on and above the diagonal.]

36. When the population distribution is normal, the statistic median $\left\{ {\left| {{X}_{1} - \widetilde{X}}\right| ,\ldots ,\left| {{X}_{n} - \widetilde{X}}\right| }\right\} /{.6745}$ can be used to estimate $\sigma$ . This estimator is more resistant to the effects of outliers (observations far from the bulk of the data) than is the sample standard deviation. Compute both the corresponding point estimate and $s$ for the data of Example 6.2.

37. When the sample standard deviation $S$ is based on a random sample from a normal population distribution, it can be shown that

$$
E\left( S\right) = \sqrt{2/\left( {n - 1}\right) }\Gamma \left( {n/2}\right) \sigma /\Gamma \left( {\left( {n - 1}\right) /2}\right)
$$