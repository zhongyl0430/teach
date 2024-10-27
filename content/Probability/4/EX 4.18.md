The authors of "Assessment of Lifetime of Railway Axle" (Intl. J. of Fatigue, 2013: 40-46) used data collected from an experiment with a specified initial crack length and number of loading cycles to propose a normal distribution with mean value ${5.496}\mathrm{\;{mm}}$ and standard deviation ${.067}\mathrm{\;{mm}}$ for the rv $X =$ final crack depth. 

> [!question] 
> For this model, what value of final crack depth would be exceeded by only ${.5}\%$ of all cracks under these circumstances? 

Let $c$ denote the requested value. 
Then the desired condition is that $$P\left( {X > c}\right) = {.005}$$or, equivalently, that $$P\left( {X \leq c}\right) = {.995} .$$
Thus $c$ is the 99.5th percentile of the normal distribution with $\mu = {5.496}$ and $\sigma = {.067}$. 
The 99.5th percentile of the standard normal distribution is 2.58, so
$$
\begin{align}
    c &= \eta\left( 0.995 \right) \\
    &= 5.496 + \left( 2.58 \right)\left( 0.067 \right) \\
    &= 5.496 + 0.173 \\
    &= 5.669 \, \text{mm}
\end{align}
$$
This is illustrated in Figure 4.23.

Figure 4.23 
Distribution of final crack depth for Example 4.18
![01925166-48c0-7eca-9860-67f13d0848b1_23_819_905_520_288_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_23_819_905_520_288_0.jpg)