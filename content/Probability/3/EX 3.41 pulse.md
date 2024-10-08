- Pulses arrive at a counter:
	- Average rate: 6 pulses per minute
    - Parameter: $\alpha = 6$
- Calculation of probability:
	- Time interval: 0.5 minutes
	- Number of pulses in this interval:
	    - Follows a Poisson distribution
	    - Parameter: $\alpha t = 6 \cdot 0.5 = 3$
	- (0.5 minutes used because $\alpha$ is expressed as a rate per minute)
- Notation:
	- Let $X$ denote number of pulses received in the 30-second interval
- We have
$$
\begin{align}
P(1 \leq X) &= 1 - P(X = 0) \\
            &= 1 - \frac{e^{-3} (3)^0}{0!} \\
            &= 0.950
\end{align}
$$