The general form for the pmf of $X =$ the number of children born up to and including the first boy is
$$p\left( x\right) = \left\{ \begin{matrix} p{\left( 1 - p\right) }^{x - 1} & x = 1,2,3,\ldots \\ 0 & \text{ otherwise } \end{matrix}\right.$$

From the definition,
$$
\begin{align}
E(X) &= \sum_{D} x \cdot p(x) \\
     &= \sum_{x=1}^{\infty} x p (1 - p)^{x - 1} \\
     &= p \sum_{x=1}^{\infty} \left[ -\frac{d}{dp} (1 - p)^{x} \right] \tag{3.9}
\end{align}
$$
Interchanging the order of taking the derivative and the summation, the
sum is that of a geometric series. 

After the sum is computed, the derivative is taken, resulting in $E\left( X\right) = 1/p$ . 
- If $p$ is near 1, we expect to see a boy very soon, 
- whereas if $p$ is near 0, we expect many births before the first boy. 

For $p = {.5}$, $E\left( X\right) = 2$.