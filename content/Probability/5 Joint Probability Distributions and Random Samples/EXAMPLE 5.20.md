Suppose that material strength for a randomly selected specimen of a particular type has a Weibull distribution with parameter values $\alpha = 2$ (shape) and $\beta = 5$ (scale). The corresponding density curve is shown in Figure 5.7. Formulas from Section 4.5 give

$$
\mu = E\left( X\right) = {4.4311}\;\widetilde{\mu } = {4.1628}\;{\sigma }^{2} = V\left( X\right) = {5.365}\;\sigma = {2.316}
$$

The mean exceeds the median because of the distribution's positive skew.

![0192609f-6f5c-74c9-8588-c1ef28b2184d_22_778_1761_643_406_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_22_778_1761_643_406_0.jpg)

Figure 5.7 The Weibull density curve for Example 5.20

We used statistical software to generate six different samples, each with $n = {10}$ , from this distribution (material strengths for six different groups of ten specimens each). The results appear in Table 5.1, followed by the values of the sample mean, sample median, and sample standard deviation for each sample. Notice first that the ten observations in any particular sample are all different from those in any other sample. Second, the six values of the sample mean are all different from one another, as are the six values of the sample median and the six values of the sample standard deviation. The same is true of the sample ${10}\%$ trimmed means, sample fourth spreads, and so on. Furthermore, the value of the sample mean from any particular sample can be regarded as a point estimate ("point" because it is a single number, corresponding to a single point on the number line) of the population mean $\mu$ , whose value is known to be 4.4311 . None of the estimates from these six samples is identical to what is being estimated. The estimates from the second and sixth samples are much too large, whereas the fifth sample gives a substantial underestimate. Similarly, the sample standard deviation gives a point estimate of the population standard deviation. All six of the resulting estimates are in error by at least a small amount.

Table 5.1 Samples from the Weibull Distribution of Example 5.20

| Sample         | 1       | 2       | 3       | 4       | 5       | 6       |
|----------------|---------|---------|---------|---------|---------|---------|
| 1             | 6.1171  | 5.07611 | 3.46710 | 1.55601 | 3.12372 | 8.93795 |
| 2             | 4.1600  | 6.79279 | 2.71938 | 4.56941 | 6.09685 | 3.92487 |
| 3             | 3.1950  | 4.43259 | 5.88129 | 4.79870 | 3.41181 | 8.76202 |
| 4             | 0.6694  | 8.55752 | 5.14915 | 2.49759 | 1.65409 | 7.05569 |
| 5             | 1.8552  | 6.82487 | 4.99635 | 2.33267 | 2.29512 | 2.30932 |
| 6             | 5.2316  | 7.39958 | 5.86887 | 4.01295 | 2.12583 | 5.94195 |
| 7             | 2.7609  | 2.14755 | 6.05918 | 9.08845 | 3.20938 | 6.74166 |
| 8             | 10.2185 | 8.50628 | 1.80119 | 3.25728 | 3.23209 | 1.75468 |
| 9             | 5.2438  | 5.49510 | 4.21994 | 3.70132 | 6.84426 | 4.91827 |
| 10            | 4.5590  | 4.04525 | 2.12934 | 5.50134 | 4.20694 | 7.26081 |
| $\bar{x}$     | 4.401   | 5.928   | 4.229   | 4.132   | 3.620   | 5.761   |
| $\widetilde{x}$ | 4.360 | 6.144   | 4.608   | 3.857   | 3.221   | 6.342   |
| $S$           | 2.642   | 2.062   | 1.611   | 2.124   | 1.678   | 2.496   |

In summary, the values of the individual sample observations vary from sample to sample, so will in general the value of any quantity computed from sample data, and the value of a sample characteristic used as an estimate of the corresponding population characteristic will virtually never coincide with what is being estimated.