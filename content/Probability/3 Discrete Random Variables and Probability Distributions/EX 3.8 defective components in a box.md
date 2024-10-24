Six boxes of components are ready to be shipped by a certain supplier. 
The number of defective components in each box is as follows:

| Box  | 1  | 2  | 3  | 4  | 5  | 6  |
|------|----|----|----|----|----|----|
| Number of defectives | 0  | 2  | 0  | 1  | 2  | 0  |

- Scenario:
	- One of several boxes is randomly selected for shipment to a customer
- Let $X$ = number of defectives in the selected box
	- Possible $X$ values: 
		- 0, 1, 2
- Simple events:
	- Six equally likely simple events
    - Three result in $X = 0$
    - One results in $X = 1$
    - Two result in $X = 2$
- Then
$$
\begin{align}
p(0) &= P(X = 0) = P(\text{box 1, 3, or 6 is sent}) = \frac{3}{6} = 0.500 \\
p(1) &= P(X = 1) = P(\text{box 4 is sent}) = \frac{1}{6} = 0.167 \\
p(2) &= P(X = 2) = P(\text{box 2 or 5 is sent}) = \frac{2}{6} = 0.333
\end{align}
$$
- Probability distribution for $X$:
	- $X = 0$: probability = 0.500
	- $X = 1$: probability = 0.167
	- $X = 2$: probability = 0.333
- These values collectively specify the probability mass function (pmf)
- Long-run behavior if the experiment is repeated:
	- $X = 0$ occurs one-half of the time
	- $X = 1$ occurs one-sixth of the time
	- $X = 2$ occurs one-third of the time
