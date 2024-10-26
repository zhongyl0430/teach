The breakdown voltage of a randomly chosen diode of a particular type is known to be normally distributed. 

> [!question] 
> What is the probability that a diode's breakdown voltage is within 1 standard deviation of its mean value? 

This question can be answered without knowing either $\mu$ or $\sigma$ , as long as the distribution is known to be normal; the answer is the same for any normal distribution:
$$
\begin{align}
    &P\left( X \text{ is within 1 standard deviation of its mean} \right) \\
    &= P\left( \mu - \sigma \leq X \leq \mu + \sigma \right) \\
    &= P\left( \frac{\mu - \sigma - \mu}{\sigma} \leq Z \leq \frac{\mu + \sigma - \mu}{\sigma} \right) \\
    &= P\left( -1.00 \leq Z \leq 1.00 \right) \\
    &= \Phi\left( 1.00 \right) - \Phi\left( -1.00 \right) \\
    &= 0.6826
\end{align}
$$

The probability that $X$ is 
- within 2 standard deviations of its mean is $$P\left( {-{2.00} \leq Z \leq {2.00}}\right) = {.9544}$$
- within 3 standard deviations of the mean is $$P\left( {-{3.00} \leq Z \leq {3.00}}\right) = {.9974}$$