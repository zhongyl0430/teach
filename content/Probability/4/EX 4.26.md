An understanding of the volumetric properties of asphalt is important in designing mixtures which will result in high-durability pavement. The article "Is a Normal Distribution the Most Appropriate Statistical Distribution for Volumetric Properties in Asphalt Mixtures?" (J. of Testing and Evaluation, Sept. 2009: 1-11) used the analysis of some sample data to recommend that for a particular mixture, $X =$ air void volume (%) be modeled with a three-parameter Weibull distribution. Suppose the values of the parameters are $\gamma = 4,\alpha = {1.3}$ , and $\beta = {.8}$ (quite close to estimates given in the article).

For $x > 4$ , the cumulative distribution function is

$$
F\left( {x;\alpha ,\beta ,\gamma }\right) = F\left( {x;{1.3},{.8},4}\right) = 1 - {e}^{-{\left\lbrack \left( x - 4\right) /{.8}\right\rbrack }^{1.3}}
$$

The probability that the air void volume of a specimen is between $5\%$ and $6\%$ is

$$
P\left( {5 \leq X \leq 6}\right) = F\left( {6;{1.3},{.8},4}\right) - F\left( {5;{1.3},{.8},4}\right) = {e}^{-{\left\lbrack \left( 5 - 4\right) /{.8}\right\rbrack }^{1.3}} - {e}^{-{\left\lbrack \left( 6 - 4\right) /{.8}\right\rbrack }^{1.3}}
$$

$$
= {.263} - {.037} = {.226}
$$

Figure 4.29 shows a graph from Minitab of the corresponding Weibull density function in which the shaded area corresponds to the probability just calculated.

![01925166-48c0-7eca-9860-67f13d0848b1_38_838_492_719_429_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_38_838_492_719_429_0.jpg)

Figure 4.29 Weibull density curve with threshold $= 4$ , shape $= {1.3}$ , scale $= {.8}$