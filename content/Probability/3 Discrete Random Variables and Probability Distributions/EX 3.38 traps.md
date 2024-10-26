- Definition:
	- Let $X$ denote number of traps (defects of a certain kind)
- Distribution:
	- Follows a Poisson distribution
	    - Parameter $\mu = 2$
- The probability that there are exactly three traps is
$$P\left( {X = 3}\right) = p\left( {3;2}\right) = \frac{{e}^{-2}{2}^{3}}{3!} = {.180},$$
- the probability that there are at most three traps is
$$
\begin{align}
P(X \leq 3) &= F(3; 2) \\
&= \sum_{x=0}^{3} \frac{e^{-2} 2^x}{x!} \\
&= 0.135 + 0.271 + 0.271 + 0.180 \\
&= 0.857
\end{align}
$$
- This latter cumulative probability is found at the intersection of the $\mu = 2$ column and the $x = 3$ row of Appendix Table A.2,
- whereas $$p\left( {3;2}\right) = F\left( {3;2}\right) - F\left( {2;2}\right) = {.857} - {.677} = {.180}$$
- the difference between two consecutive entries in the $\mu = 2$ column of the cumulative Poisson table.