The distribution of egg weights (g) of a certain type is normal with 
- mean value 53
- standard deviation .3 
- (consistent with data in the article "Evaluation of Egg Quality Traits of Chickens Reared under Backyard System in Western Uttar Pradesh" (Indian J. of Poultry Sci., 2009: 261-262)). 
Let ${X}_{1},{X}_{2},\ldots ,{X}_{12}$ denote the weights of a dozen randomly selected eggs; 
- these ${X}_{i}$ ’s constitute a random sample of size 12 from the specified normal distribution.

The total weight of the 12 eggs is ${T}_{o} = {X}_{1} + \ldots + {X}_{12}$; 
it is normally distributed with 
- mean value $E\left( {T}_{o}\right) = {n\mu } = {12}\left( {53}\right) = {636}$
- variance $V\left( {T}_{o}\right) = n{\sigma }^{2} = {12}{\left( {.3}\right) }^{2} =$ 1.08. 

The probability that the total weight is between 635 and 640 is now obtained by standardizing and referring to Appendix Table A.3:
$$
\begin{align}
P\left( {635 < T_{o} < 640} \right) 
&= \left( \frac{635 - 636}{\sqrt{1.08}} < Z < \frac{640 - 636}{\sqrt{1.08}} \right) \\ 
&= P\left( {-0.96 < Z < 3.85} \right) \\ 
&= \Phi\left( 3.85 \right) - \Phi\left( -0.96 \right) \\ 
&\approx 1 - 0.1685 = 0.8315.
\end{align}
$$

If cartons containing a dozen eggs are repeatedly selected, in the long run slightly more than ${83}\%$ of the eggs in a carton will weigh in total between ${635}\mathrm{\;g}$ and ${640}\mathrm{\;g}$ . 
Notice that ${635} < {T}_{o} < {640}$ is equivalent to ${52.9167} < \bar{X} < {53.3333}$ (divide each term in the original system of inequalities by 12). 
Thus $P\left( {{52.9167} < \bar{X} < {53.3333}}\right) \approx$ .8315. 
This latter probability can also be obtained by standardizing $\bar{X}$ directly.

Now consider randomly selecting just four of these eggs. 
The sample mean weight $\bar{X}$ is then normally distributed with mean value ${\mu }_{\bar{X}} = \mu = {53}$ and standard deviation ${\sigma }_{\bar{X}} = \sigma /\sqrt{n} = {.3}/\sqrt{4} = {.15}$ . 
The probability that the sample mean weight exceeds ${53.5}\mathrm{\;g}$ is then
$$
\begin{align}
P\left( \bar{X} > 53.5 \right) 
&= P\left( Z > \frac{53.5 - 53}{0.15} \right) \\ 
&= P\left( Z > 3.33 \right) \\ 
&= 1 - \Phi\left( 3.33 \right) \\ 
&= 1 - 0.9996 = 0.0004.
\end{align}
$$

Because 53.5 is 3.33 standard deviations (of $\bar{X}$ ) larger than the mean value 53, it is exceedingly unlikely that the sample mean will exceed 53.5.