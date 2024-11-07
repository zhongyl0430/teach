A bank operates both a drive-up facility and a walk-up window. 
On a randomly selected day, let 
- $X =$ the proportion of time that the drive-up facility is in use (at least one customer is being served or waiting to be served)
- $Y =$ the proportion of time that the walk-up window is in use. 

Then the set of possible values for $\left( {X, Y}\right)$ is the rectangle $D = \{ \left( {x, y}\right) : 0 \leq x \leq 1,0 \leq y \leq 1\}$. 

Suppose the joint pdf of $\left( {X, Y}\right)$ is given by
$$
f\left( {x, y}\right) = \left\{ \begin{matrix} \frac{6}{5}\left( {x + {y}^{2}}\right) & 0 \leq x \leq 1,0 \leq y \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

To verify that this is a legitimate pdf, note that $f\left( {x, y}\right) \geq 0$ and
$$
\begin{align}
&\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f\left( x, y \right) \, dx \, dy \\
&= \int_{0}^{1} \int_{0}^{1} \frac{6}{5} \left( x + y^{2} \right) \, dx \, dy \\
&= \int_{0}^{1} \int_{0}^{1} \frac{6}{5} x \, dx \, dy + \int_{0}^{1} \int_{0}^{1} \frac{6}{5} y^{2} \, dx \, dy \\
&= \int_{0}^{1} \frac{6}{5} x \, dx + \int_{0}^{1} \frac{6}{5} y^{2} \, dy \\
&= \frac{6}{10} + \frac{6}{15} = 1.
\end{align}
$$

The probability that neither facility is busy more than one-quarter of the time is
$$
\begin{align}
&P\left( 0 \leq X \leq \frac{1}{4}, \; 0 \leq Y \leq \frac{1}{4} \right) \\
&= \int_{0}^{1/4} \int_{0}^{1/4} \frac{6}{5} \left( x + y^{2} \right) \, dx \, dy \\
&= \frac{6}{5} \int_{0}^{1/4} \int_{0}^{1/4} x \, dx \, dy + \frac{6}{5} \int_{0}^{1/4} \int_{0}^{1/4} y^{2} \, dx \, dy \\
&= \left. \frac{6}{20} \cdot \frac{x^{2}}{2} \right|_{x = 0}^{x = 1/4} + \left. \frac{6}{20} \cdot \frac{y^{3}}{3} \right|_{y = 0}^{y = 1/4} \\
&= \frac{7}{640} \\
&= 0.0109.
\end{align}
$$
