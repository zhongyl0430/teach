[[EXAMPLE 5.5]] were continued

The joint and marginal pdf’s of $X =$ amount of almonds and $Y =$ amount of cashews
$$
f\left( {x, y}\right) = \left\{ \begin{matrix} {24xy} & 0 \leq x \leq 1,0 \leq y \leq 1, x + y \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$
$$
{f}_{X}\left( x\right) = \left\{ \begin{matrix} {12x}{\left( 1 - x\right) }^{2} & 0 \leq x \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$
with ${f}_{Y}\left( y\right)$ obtained by replacing $x$ by $y$ in ${f}_{X}\left( x\right)$. 
It is easily verified that ${\mu }_{X} = {\mu }_{Y} = \frac{2}{5}$, and
$$
\begin{align}
E\left( XY \right) 
&= \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} xy f\left( x, y \right) \, dx \, dy \\
&= \int_{0}^{1} \int_{0}^{1 - x} xy \cdot 24xy \, dy \, dx \\
&= 8 \int_{0}^{1} x^{2} \left( 1 - x \right)^{3} \, dx \\
&= \frac{2}{15}.
\end{align}
$$

Thus 
$$
\begin{align}
\operatorname{Cov}(X, Y) &= \frac{2}{15} - \left( \frac{2}{5} \right) \left( \frac{2}{5} \right) \\[10pt]
&= \frac{2}{15} - \frac{4}{25} \\[10pt]
&= - \frac{2}{75}.
\end{align}
$$

A negative covariance is reasonable here because more almonds in the can implies fewer cashews.