Expected value in [[EX 4.9 amount of gravel]]. 

The pdf of weekly gravel sales $X$ was
$$
f\left( x\right) = \left\{ \begin{matrix} \frac{3}{2}\left( {1 - {x}^{2}}\right) & 0 \leq x \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

$$
\begin{align}
    E\left( X \right) &= \int_{-\infty}^{\infty} x \cdot f\left( x \right) \, dx \\
    &= \int_{0}^{1} x \cdot \frac{3}{2} \left( 1 - x^{2} \right) \, dx \\
    &= \left. \frac{3}{2} \int_{0}^{1} \left( x - x^{3} \right) \, dx \right. \\
    &= \frac{3}{2} \left( \frac{x^{2}}{2} - \frac{x^{4}}{4} \right) \bigg|_{x = 0}^{x = 1} \\
    &= \frac{3}{8}
\end{align}
$$
