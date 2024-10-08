- **Vehicle Diagnostic Test Cost**
	- **Cost Function**:
		- The cost $h(X)$ of the diagnostic test is given by:
		- $h(X) = 20 + 3X + 0.5X^2$
	- **Variables**:
		- $X$: The number of cylinders in the vehicle's engine (random variable)
		- $Y = h(X)$: The cost of the diagnostic test (random variable)
- **Probability Distributions**:
	- **pmf of $X$**:
		  - The probability mass function (pmf) for $X$
	- **Derived pmf of $Y$**:
		  - The pmf of $Y$ derived from the cost function $h(X)$

| x   | 4   | 6   | 8   |
|-----|-----|-----|-----|
| p(x)| .5  | .3  | .2  |

implies

| y   | 40  | 56  | 76  |
|-----|-----|-----|-----|
| p(y)| .5  | .3  | .2  |

With ${D}^{ * }$ denoting possible values of $Y$ ,
$$
\begin{align}
E(Y) &= E\left[ h(X) \right] = \sum_{D^*} y \cdot p(y) \\
     &= (40)(0.5) + (56)(0.3) + (76)(0.2) \tag{3.11} \\
     &= h(4) \cdot (0.5) + h(6) \cdot (0.3) + h(8) \cdot (0.2) \\
     &= \sum_{D} h(x) \cdot p(x)
\end{align}
$$
- **Expected Value of $Y$ Without Determining pmf**
- **According to Equation (3.11)**:
	- It is unnecessary to determine the pmf of $Y$ to calculate $E(Y)$
- **Reasoning**:
    - The desired expected value $E(Y)$ is a weighted average of the possible $h(x)$ values (instead of the $x$ values)
    - This approach simplifies the calculation by focusing on $h(x)$, the cost function, rather than $Y$'s distribution
