- Anyone purchasing an insurance policy for a home or automobile:
- Must specify a deductible amount.
	- Deductible: the amount of loss the policyholder absorbs before the insurance company begins paying out.
- Suppose a particular company offers:
	- Auto deductibles: $\$100$, $\$500$, $\$1000$.
	- Homeowner deductibles: $\$500$, $\$1000$, $\$2000$.
- Consider randomly selecting someone with both auto and homeowner insurance from this company.
- Let:
	- $X$: the auto policy deductible amount.
	- $Y$: the homeowner policy deductible amount.
- The joint pmf of $X$ and $Y$ is represented in a joint probability table.

| y \ p(x, y) | 500  | 1000 | 5000 |
|-------------|------|------|------|
| 100         | .30  | .05  | 0    |
| 500         | .15  | .20  | .05  |
| 1000        | .10  | .10  | .05  |

- According to the joint pmf:
	- There are nine possible $\left(X, Y\right)$ pairs:
    - Examples: $\left(100, 500\right)$, $\left(100, 1000\right)$, ..., $\left(1000, 5000\right)$.
- The probability of $\left(100, 500\right)$ is:
    - $p\left(100, 500\right) = P\left(X = 100, Y = 500\right) = 0.30$.
- General properties of the pmf:
	- $p\left(x, y\right) \geq 0$ for all $\left(x, y\right)$ pairs.
	- The sum of the nine displayed probabilities equals 1.
- To compute the probability $P\left(X = Y\right)$:
	- Sum $p\left(x, y\right)$ over the pairs where the deductible amounts are identical:
    - This includes two $\left(x, y\right)$ pairs.
    
$$
\begin{align}
P(X = Y) &= p(500, 500) + p(1000, 1000) \\
         &= 0.15 + 0.10 \\
         &= 0.25
\end{align}

$$
- To find the probability that the auto deductible amount is at least \$500:
- Calculate the sum of all probabilities for $\left(x, y\right)$ pairs where:
    - $x \geq 500$.
- This corresponds to:
	- The sum of probabilities in the bottom two rows of the joint probability table.

$$
\begin{align}
P(X \geq 500) &= 0.15 + 0.20 + 0.05 + 0.10 + 0.10 + 0.05 \\
              &= 0.65
\end{align}
$$