Let’s determine the following standard normal probabilities: 
a. $P\left( {Z \leq {1.25}}\right)$, 
b. $P\left( {Z > {1.25}}\right)$, 
c. $P\left( {Z \leq - {1.25}}\right)$, 
d. $P\left( {-{.38} \leq Z \leq {1.25}}\right)$,
e. $P\left( {Z \leq 5}\right)$.

Figure 4.15 Normal curve areas (probabilities) for Example 4.13
![01925166-48c0-7eca-9860-67f13d0848b1_18_759_182_881_252_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_18_759_182_881_252_0.jpg)

a. $$P\left( {Z \leq {1.25}}\right) = \Phi \left( {1.25}\right) ,$$
a probability that is tabulated in Appendix Table A. 3 at the intersection of the row marked 1.2 and the column marked .05 . 
The number there is .8944, so $P\left( {Z \leq {1.25}}\right) = {.8944}$ . 
Figure 4.15(a) illustrates this probability.

b. $$
\begin{align}
    P\left( Z > 1.25 \right) &= 1 - P\left( Z \leq 1.25 \right) \\
    &= 1 - \Phi\left( 1.25 \right)
\end{align}
$$
the area under the $z$ curve to the right of 1.25 (an upper-tail area). 
Then $\Phi \left( {1.25}\right) = {.8944}$ implies that $P\left( {Z > {1.25}}\right) = {.1056}$ . 
Since $Z$ is a continuous rv, $P\left( {Z \geq {1.25}}\right) = {.1056}$ . 
See Figure 4.15(b).

c. $$P\left( {Z \leq - {1.25}}\right) = \Phi \left( {-{1.25}}\right) ,$$a lower-tail area. Directly from Appendix Table A. $3,\Phi \left( {-{1.25}}\right) = {.1056}$ . 
By symmetry of the $z$ curve, this is the same answer as in part (b).

d. $P\left( {-{.38} \leq Z \leq {1.25}}\right)$ is the area under the standard normal curve above the interval whose left endpoint is -.38 and whose right endpoint is 1.25. 
From Section 4.2, if $X$ is a continuous rv with $\operatorname{cdf}F\left( x\right)$, then $$P\left( {a \leq X \leq b}\right) = F\left( b\right) - F\left( a\right) .$$
Thus 
$$
\begin{align}
    &P\left( -0.38 \leq Z \leq 1.25 \right) \\
    &= \Phi\left( 1.25 \right) - \Phi\left( -0.38 \right) \\
    &= 0.8944 - 0.3520 \\
    &= 0.5424 .
\end{align}
$$
(See Figure 4.16.)

Figure 4.16 
$P\left( {-{.38} \leq Z \leq {1.25}}\right)$ as the difference between two cumulative areas
![01925166-48c0-7eca-9860-67f13d0848b1_18_657_997_1084_233_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_18_657_997_1084_233_0.jpg)

e. $P\left( {Z \leq 5}\right) = \Phi \left( 5\right)$ , the cumulative area under the $z$ curve to the left of 5 . 
This probability does not appear in the table because the last row is labeled 3.4. 
However, the last entry in that row is $\Phi \left( {3.49}\right) = {.9998}$ . 
That is, essentially all of the area under the curve lies to the left of 3.49 (at most 3.49 standard deviations to the right of the mean). 
Therefore we conclude that $P\left( {Z \leq 5}\right) \approx 1$ .