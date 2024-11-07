The amount of a particular impurity in a batch of a certain chemical product is a random variable with mean value ${4.0}\mathrm{\;g}$ and standard deviation ${1.5}\mathrm{\;g}$ . If 50 batches are independently prepared, what is the (approximate) probability that the sample average amount of impurity $\bar{X}$ is between 3.5 and ${3.8}\mathrm{\;g}$ ? According to the rule of thumb to be stated shortly, $n = {50}$ is large enough for the CLT to be applicable. $\bar{X}$ then has approximately a normal distribution with mean value ${\mu }_{\bar{X}} = {4.0}$ and ${\sigma }_{\bar{X}} = {1.5}/\sqrt{50} = {.2121}$ , so
$$
\begin{align}
P\left( {3.5 \leq \bar{X} \leq 3.8} \right) 
&\approx P\left( {\frac{3.5 - 4.0}{0.2121} \leq Z \leq \frac{3.8 - 4.0}{0.2121}} \right) \\
&= \Phi\left( -0.94 \right) - \Phi\left( -2.36 \right) \\
&\approx 0.1645.
\end{align}
$$

Now consider randomly selecting 100 batches, and let ${T}_{o}$ represent the total amount of impurity in these batches. Then the mean value and standard deviation of ${T}_{o}$ are ${100}\left( 4\right) = {400}$ and $\sqrt{100}\left( {1.5}\right) = {15}$ , respectively, and the CLT implies that ${T}_{0}$ has approximately a normal distribution. The probability that this total is at most ${425}\mathrm{\;g}$ is
$$
\begin{align}
P\left( {T_{0} \leq 425} \right) 
&\approx P\left( {Z \leq \frac{425 - 400}{15}} \right) \\
&= P\left( {Z \leq 1.67} \right) \\
&= \Phi\left( 1.67 \right) = 0.9525.
\end{align}
$$
