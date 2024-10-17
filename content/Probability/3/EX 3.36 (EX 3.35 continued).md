([[EX 3.35 animal population]] continued)
- In the animal-tagging example:
- Parameters are defined as:
    - $n = 10$: number of animals tagged.
    - $M = 5$: number of tagged animals.
    - $N = 25$: total number of animals.
- Calculate probability:
    - $p = \frac{M}{N} = \frac{5}{25} = 0.2$.
- Expected value of $X$:
	- $$E(X) = n \cdot p = 10 \cdot 0.2 = 2$$.
- Variance of $X$ (without replacement):
	- $$V(X) = \frac{M}{N-1} \cdot n \cdot p \cdot (1 - p)$$.
- Substituting values:
	- $$V(X) = \frac{15}{24} \cdot 10 \cdot 0.2 \cdot 0.8 = (0.625)(1.6) = 1$$.
- If the sampling had been carried out with replacement:
  - Variance becomes:
    - $$V(X) = 1.6$$
- Given:
    - Population size $N$ is unknown
    - Observed value $x$ is provided
  - Objective:
    - Estimate the population size $N$
  - Reasoning:
    - Equate observed sample proportion $\frac{x}{n}$ with population proportion $\frac{M}{N}$
  - Conclusion:
    - Provides an estimate for $N$

$$\widehat{N} = \frac{M \cdot n}{x}$$

If $M = {100}$ , $n = {40}$, and $x = {16}$, then  $\widehat{N} = {250}$. 