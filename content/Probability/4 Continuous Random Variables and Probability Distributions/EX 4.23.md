The article "The Probability Distribution of Maintenance Cost of a System Affected by the Gamma Process of Degradation" (Reliability Engr. and System Safety, 2012: 65-76) notes that the gamma distribution is widely used to model the extent of degradation such as corrosion, creep, or wear. 

Let $X$ represent the amount of degradation of a certain type, and suppose that it has a standard gamma distribution with $\alpha = 2$ . 
Since
$$
P\left( {a \leq X \leq b}\right) = F\left( b\right) - F\left( a\right)
$$

when $X$ is continuous,
$$
\begin{align}
    P\left( 3 \leq X \leq 5 \right) &= F\left( 5; 2 \right) - F\left( 3; 2 \right) \\
    &= 0.960 - 0.801 \\
    &= 0.159
\end{align}
$$

The probability that the amount of degradation exceeds 4 is
$$
\begin{align}
    P\left( X > 4 \right) &= 1 - P\left( X \leq 4 \right) \\
    &= 1 - F\left( 4; 2 \right) \\
    &= 1 - 0.908 \\
    &= 0.092
\end{align}
$$
