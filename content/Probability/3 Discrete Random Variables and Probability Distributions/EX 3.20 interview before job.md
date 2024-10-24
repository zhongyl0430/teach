- Definition of the random variable:
	- Let $X$ be the number of interviews a student has prior to getting a job.

- Probability mass function (pmf):
	- The pmf of $X$ is given by:
    $$
    p(x) = \begin{cases} 
    k/x^2 & \text{for } x = 1, 2, 3, \ldots \\ 
    0 & \text{otherwise} 
    \end{cases}
    $$
	- Here, $k = \frac{\pi^2}{6}$ is a normalization constant ensuring that the total probability sums to 1:
    $$
    \sum_{x=1}^{\infty} p(x) = 1
    $$

- Expected value of $X$:
	- The expected value $\mu$ is calculated as follows:
    $$
    \mu = E(X) = \sum_{x=1}^{\infty} x \cdot p(x) = \sum_{x=1}^{\infty} x \cdot \frac{k}{x^2}
    $$
	- Simplifying the expression:
    $$
    \mu = k \sum_{x=1}^{\infty} \frac{1}{x}
    $$

- Important note:
	- The series $\sum_{x=1}^{\infty} \frac{1}{x}$ diverges, indicating that the expected value $\mu$ is infinite.

- Conclusion:
	- The interpretation of $\mu$ shows that, on average, a student is expected to have an infinite number of interviews before getting a job, reflecting a potentially very high number of trials in this scenario.

- Harmonic series:
	- The sum in Equation (3.10):
    $$
    \sum_{x=1}^{\infty} \frac{1}{x}
    $$
    is known as the harmonic series.
	- It is a famous series in mathematics that diverges to infinity:
    $$
    \sum_{x=1}^{\infty} \frac{1}{x} = \infty
    $$

- Expected value implications:
	- Since $E(X)$ is based on this divergent series, it follows that:
    $$
    E(X) \text{ is not finite.}
    $$
	- This occurs because the pmf $p(x)$ does not decrease sufficiently fast as $x$ increases.

- Heavy tails:
	- The distribution of $X$ is said to have "a heavy tail."
	- Heavy tails refer to probability distributions that allocate a significant amount of probability to values far from the mean $\mu$.

- Consequences of heavy tails:
	- When a sequence of values of $X$ is drawn from this distribution, the sample average will not converge to a finite number; instead, it will tend to grow without bound.
  
- General implications in statistics:
	- The term "heavy tails" can apply to any distribution where a considerable amount of probability lies far from the mean, not necessarily implying that $\mu = \infty$.
	- Heavy tails complicate statistical inferences about the mean $\mu$, making it challenging to draw conclusions about the expected outcomes.

- Conclusion:
	- Understanding the nature of heavy tails is crucial for interpreting distributions and making reliable statistical inferences.
