- Scenario: 
	- Five individuals from an animal population near extinction have been:
    - Caught, tagged, and released.
	- Purpose: To mix into the population.
- After mixing:
	- A random sample of 10 animals is selected.
- Define:
	- $X$: the number of tagged animals in the second sample.
- Given:
	- Total number of animals in the region: 25.
	- Number of tagged animals: 5.

- Parameter values:
	- $n = 10$: number of animals in the sample.
	- $M = 5$: number of tagged animals in the population.
	- $N = 25$: total number of animals in the population.
- The probability mass function (pmf) of $X$ (the number of tagged animals in the sample) is defined based on these parameters.
	- The pmf can be calculated using the hypergeometric distribution:
    - $$ P(X = k) = \frac{\binom{M}{k} \binom{N-M}{n-k}}{\binom{N}{n}} $$
      - Where:
        - $k$: number of tagged animals in the sample (possible values range from 0 to $\min(n, M)$).

$$h\left( {x;{10},5,{25}}\right) = \frac{\left( \begin{array}{l} 5 \\ x \end{array}\right) \left( \begin{matrix} {20} \\ {10} - x \end{matrix}\right) }{\left( \begin{array}{l} {25} \\ {10} \end{array}\right) }$$
where $x = 0,1,2,3,4,5$

The probability that 
- exactly two of the animals in the second sample are tagged is
$$P\left( {X = 2}\right) = h\left( {2;{10},5,{25}}\right) = \frac{\left( \begin{array}{l} 5 \\ 2 \end{array}\right) \left( \begin{matrix} {20} \\ 8 \end{matrix}\right) }{\left( \begin{array}{l} {25} \\ {10} \end{array}\right) } = {.385}$$

The probability that at most two of the animals in the recapture sample are tagged is
$$
\begin{align}
P(X \leq 2) &= P(X = 0, 1, \text{ or } 2) \\
            &= \sum_{x=0}^{2} h(x; 10, 5, 25) \\
            &= 0.057 + 0.257 + 0.385 \\
            &= 0.699
\end{align}
$$