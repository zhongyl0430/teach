A certain brand of MP3 player comes in three configurations: 
- a model with $2\mathrm{{GB}}$ of memory, costing \$ 80, 
- a $4\mathrm{\;{GB}}$ model priced at \$ 100, 
- an $8\mathrm{\;{GB}}$ version with a price tag of \$120. 
If 
- 20% of all purchasers choose the 2 GB model,
- 30% choose the 4 GB model, 
- 50% choose the $8\mathrm{\;{GB}}$ model, 

then the probability distribution of the cost $X$ of a single randomly selected MP3 player purchase is given by

| $x$    | 80  | 100 | 120 |
| ------ | --- | --- | --- |
| $p(x)$ | 0.2 | 0.3 | 0.5 |
with
$$
\mu = {106},{\sigma }^{2} = {244} \tag{5.2}
$$

Suppose on a particular day only two MP3 players are sold. 
Let 
- ${X}_{1} =$ the revenue from the first sale
- ${X}_{2} =$ the revenue from the second. 

Suppose that ${X}_{1}$ and ${X}_{2}$ are independent, each with the probability distribution shown in (5.2) 
- so that ${X}_{1}$ and ${X}_{2}$ constitute a random sample from the distribution (5.2)

Table 5.2 lists possible $\left( {{x}_{1},{x}_{2}}\right)$ pairs, the probability of each computed using (5.2) and also the assumption of independence, and the resulting $\bar{x}$ and ${s}^{2}$ values. 
Note that when $n = 2$, ${s}^{2} =$ ${\left( {x}_{1} - \bar{x}\right) }^{2} + {\left( {x}_{2} - \bar{x}\right) }^{2}$.

Now to obtain the probability distribution of $\bar{X}$, the sample average revenue per sale, we must consider each possible value $\bar{x}$ and compute its probability. 

For example, $\bar{x} = {100}$ occurs three times in the table with probabilities ${.10}$, ${.09}$, and .10, so
$$
{p}_{\bar{X}}\left( {100}\right) = P\left( {\bar{X} = {100}}\right) = {.10} + {.09} + {.10} = {.29}
$$

Similarly,
$$
\begin{align}
{p}_{{S}^{2}}\left( {800}\right) &= P\left( {{S}^{2} = {800}}\right) \\
&= P\left( {{X}_{1} = {80},{X}_{2} = {120}\text{ or }{X}_{1} = {120},{X}_{2} = {80}}\right) \\
&= {.10} + {.10} = {.20}
\end{align}
$$
Table 5.2 Outcomes, Probabilities, and Values of $\bar{x}$ and ${s}^{2}$ for Example 5.21

| $x_1$ | $x_2$ | $p(x_1, x_2)$ | $\bar{x}$ | $s^2$ |
| ----- | ----- | ------------- | --------- | ----- |
| 80    | 80    | 0.04          | 80        | 0     |
| 80    | 100   | 0.06          | 90        | 200   |
| 80    | 120   | 0.10          | 100       | 800   |
| 100   | 80    | 0.06          | 90        | 200   |
| 100   | 100   | 0.09          | 100       | 0     |
| 100   | 120   | 0.15          | 110       | 200   |
| 120   | 80    | 0.10          | 100       | 800   |
| 120   | 100   | 0.15          | 110       | 200   |
| 120   | 120   | 0.25          | 120       | 0     |

The complete sampling distributions of $\bar{X}$ and ${S}^{2}$ appear in (5.3) and (5.4). 

| $\bar{x}$              | 80   | 90   | 100  | 110  | 120  |
| ---------------------- | ---- | ---- | ---- | ---- | ---- |
| $p_{\bar{X}}(\bar{x})$ | 0.04 | 0.12 | 0.29 | 0.30 | 0.25 |

| $s^2$          | 0    | 200  | 800  |
| -------------- | ---- | ---- | ---- |
| $p_{S^2}(s^2)$ | 0.38 | 0.42 | 0.20 |

Figure 5.8 pictures a probability histogram for both the original distribution (5.2) and the $\bar{X}$ distribution (5.3). 
The figure suggests first that the mean (expected value) of the $\bar{X}$ distribution is equal to the mean 106 of the original distribution, since both histograms appear to be centered at the same place.

Figure 5.8 
Probability histograms for the underlying distribution and $\bar{X}$ distribution in Example 5.21
![0192609f-6f5c-74c9-8588-c1ef28b2184d_26_526_183_1071_249_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_26_526_183_1071_249_0.jpg)


From (5.3),
$$
{\mu }_{\bar{X}} = E\left( \bar{X}\right) = \sum \bar{x}{p}_{\bar{X}}\left( \bar{x}\right) = \left( {80}\right) \left( {.04}\right) + \cdots + \left( {120}\right) \left( {.25}\right) = {106} = \mu
$$

Second, it appears that the $\bar{X}$ distribution has smaller spread (variability) than the original distribution, since probability mass has moved in toward the mean. Again from (5.3),
$$
\begin{align}
\sigma_{\bar{X}}^{2} 
&= V\left( \bar{X} \right) = \sum \bar{x}^{2} \cdot p_{\bar{X}}\left( \bar{x} \right) - \mu_{\bar{X}}^{2} \\

&= \left( 80^{2} \right) \left( 0.04 \right) + \cdots + \left( 120^{2} \right) \left( 0.25 \right) - \left( 106 \right)^{2} \\

&= 122 = \frac{244}{2} = \frac{\sigma^{2}}{2}.
\end{align}
$$

The variance of $\bar{X}$ is precisely half that of the original variance (because $n = 2$ ).

Using (5.4), the mean value of ${S}^{2}$ is
$$
\begin{align}
\mu_{{S}^{2}} 
&= E\left( {S}^{2} \right) = \sum s^{2} \cdot p_{{S}^{2}}\left( s^{2} \right) \\

&= \left( 0 \right) \left( 0.38 \right) + \left( 200 \right) \left( 0.42 \right) + \left( 800 \right) \left( 0.20 \right) \\

&= 244 = \sigma^{2}.
\end{align}
$$

That is, the $\bar{X}$ sampling distribution is centered at the population mean $\mu$, and the ${S}^{2}$ sampling distribution is centered at the population variance ${\sigma }^{2}$.

If there had been four purchases on the day of interest, the sample average revenue $\bar{X}$ would be based on a random sample of four ${X}_{i}$’s, each having the distribution (5.2). 
Mildly tedious calculations yield the pmf of $\bar{X}$ for $n = 4$ as

| $\bar{x}$                        | 80     | 85     | 90     | 95     | 100    | 105    | 110    | 115    | 120    |
| -------------------------------- | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| $p_{\overline{X}}(\overline{x})$ | 0.0016 | 0.0096 | 0.0376 | 0.0936 | 0.1761 | 0.2340 | 0.2350 | 0.1500 | 0.0625 |

From this, ${\mu }_{\bar{X}} = {106} = \mu$ and ${\sigma }_{\bar{X}}^{2} = {61} = {\sigma }^{2}/4$. 
Figure 5.9 is a probability histogram of this pmf.

Figure 5.9 
Probability histogram for $\bar{X}$ based on $n = 4$ in Example 5.21
![0192609f-6f5c-74c9-8588-c1ef28b2184d_26_782_1554_599_303_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_26_782_1554_599_303_0.jpg)
