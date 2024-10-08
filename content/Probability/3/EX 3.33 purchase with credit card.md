- Scenario:
  - In a certain store, 75% of all purchases are made with a credit card.
  - Let $X$ represent the number of purchases made with a credit card among 10 randomly selected purchases.

- Random variable distribution:
  - $X$ follows a binomial distribution:
    $$
    X \sim \operatorname{Bin}(10, 0.75)
    $$

- Expected value:
  - The expected value (mean) of $X$:
    $$
    E(X) = np = 10 \times 0.75 = 7.5
    $$

- Variance:
  - The variance of $X$:
    $$
    V(X) = npq = 10 \times 0.75 \times 0.25 = 1.875
    $$

- Standard deviation:
  - The standard deviation of $X$:
    $$
    \sigma = \sqrt{1.875} \approx 1.37
    $$

- Interpretation:
  - Although $X$ can only take on integer values (0 to 10), the expected value $E(X)$ need not be an integer.
  - When performing a large number of independent binomial experiments (each with $n = 10$ trials and $p = 0.75$), the average number of purchases made with a credit card per experiment will be close to 7.5.

The probability that $X$ is within 1 standard deviation of its mean value is
$$
\begin{align}
&P(7.5 - 1.37 \leq X \leq 7.5 + 1.37) \\
&= P(6.13 \leq X \leq 8.87) \\
&= P(X = 7 \text{ or } 8) \\
&= 0.532
\end{align}
$$