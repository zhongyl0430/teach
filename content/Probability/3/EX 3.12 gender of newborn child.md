- **Observation Setup**
	- Start at a fixed time
	- Observe gender of each newborn child at a certain hospital
	- Continue until a boy (B) is born

- **Definitions**
	- Let $p = P(B)$
	- Assume that successive births are independent
	- Define the random variable (rv) $X$
		- $X$ = number of births observed

$$
\begin{align}
p(1) &= P(X = 1) \\&= P(B) = p \\

p(2) &= P(X = 2) \\&= P(GB) = P(G) \cdot P(B) = (1 - p)p \\

p(3) &= P(X = 3) \\&= P(GGB) = P(G) \cdot P(G) \cdot P(B) \\&= (1 - p)^{2} p.
\end{align}
$$
- Continuing in this way, a general formula emerges:
$$p\left( x\right) = \left\{ \begin{matrix} {\left( 1 - p\right) }^{x - 1}p & x = 1,2,3,\ldots \\ 0 & \text{ otherwise } \end{matrix}\right. \tag{3.2}$$
- **Parameter $p$**
	- Can assume any value between 0 and 1

- **Geometric Distributions**
	- Expression (3.2) describes the family of geometric distributions

- **Specific Scenarios**
	- Gender Scenario
	    - Appropriate $p = 0.51$
	- Rh-Positive Blood Scenario
	    - Appropriate $p = 0.85$
