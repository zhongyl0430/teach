- Definition of the random variable:
	- Let $X$ be defined as:
	    - $X = 1$ if a randomly selected vehicle passes the emissions test.
	    - $X = 0$ if it does not pass.
  
- Nature of $X$:
	- $X$ is a Bernoulli random variable with the following probability mass function (pmf):
	    - $P(X = 1) = p$
	    - $P(X = 0) = 1 - p$

- Expected value calculation:
	- The expected value of $X$ is computed as follows:
    $$
    \begin{align}
E(X) &= 0 \cdot P(X = 0) + 1 \cdot P(X = 1) \\
     &= 0 \cdot (1 - p) + 1 \cdot p \\
     &= p
\end{align}

    $$
	- Thus, the expected value $E(X)$ is simply the probability that $X$ takes the value 1 
		- i.e., the probability of passing the test.

- Conceptual population:
	- If we think of a population consisting of:
	    - $0$s in proportion $1 - p$ (vehicles that fail).
	    - $1$s in proportion $p$ (vehicles that pass).
	- The average of this conceptual population is:
    $$
    \mu = p
    $$
  
- Interpretation:
	- The mean $\mu$ represents the overall probability of a vehicle passing the emissions test when considering a large population.
