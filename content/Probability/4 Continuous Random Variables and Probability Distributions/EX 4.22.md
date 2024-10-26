Suppose that calls to a rape crisis center in a certain county occur according to a Poisson process with rate $\alpha = {.5}$ call per day. 
Then the number of days $X$ between successive calls has an exponential distribution with parameter value .5, so the probability that more than 2 days elapse between calls is
$$
\begin{align}
    &P\left( X > 2 \right) \\
    &= 1 - P\left( X \leq 2 \right) \\
    &= 1 - F\left( 2; 0.5 \right) \\
    &= e^{-\left( 0.5 \right) \left( 2 \right)} \\
    &= 0.368
\end{align}
$$

The expected time between successive calls is $1/{.5} = 2$ days.