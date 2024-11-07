A nut company markets cans of deluxe mixed nuts containing almonds, cashews, and peanuts. Suppose the net weight of each can is exactly $1\mathrm{{lb}}$, but the weight contribution of each type of nut is random. 
Because the three weights sum to 1, a joint probability model for any two gives all necessary information about the weight of the third type. 
Let 
- $X =$ the weight of almonds in a selected can
- $Y =$ the weight of cashews. 

Then the region of positive density is 
$$D = \{ \left( {x, y}\right) : 0 \leq x \leq 1,0 \leq y \leq 1, x + y \leq 1\}$$ the shaded region pictured in Figure 5.2.

Figure 5.2 
Region of positive density for Example 5.5
![0192609f-6f5c-74c9-8588-c1ef28b2184d_5_978_895_444_326_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_5_978_895_444_326_0.jpg)

Now let the joint pdf for $\left( {X, Y}\right)$ be
$$
f\left( {x, y}\right) = \left\{ \begin{matrix} {24xy} & 0 \leq x \leq 1,0 \leq y \leq 1, x + y \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

For any fixed $x$, $f\left( {x, y}\right)$ increases with $y$; for fixed $y, f\left( {x, y}\right)$ increases with $x$. 
This is appropriate because the word deluxe implies that most of the can should consist of almonds and cashews rather than peanuts, so that the density function should be large near the upper boundary and small near the origin. 
The surface determined by $f\left( {x, y}\right)$ slopes upward from zero as $\left( {x, y}\right)$ moves away from either axis.

Clearly, $f\left( {x, y}\right) \geq 0$. 
To verify the second condition on a joint pdf, recall that a double integral is computed as an iterated integral by holding one variable fixed (such as $x$ as in Figure 5.2), integrating over values of the other variable lying along the straight line passing through the value of the fixed variable, and finally integrating over all possible values of the fixed variable. 
Thus
$$
\begin{align}
\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f(x, y) \, dy \, dx &= \int_{D} \int f(x, y) \, dy \, dx \\
&= \int_{0}^{1} \left\{ \int_{0}^{1 - x} 24xy \, dy \right\} dx \\
&= \int_{0}^{1} 24x \left\{ \left. \frac{y^2}{2} \right|_{y=0}^{y=1-x} \right\} dx \\
&= \int_{0}^{1} 12x (1 - x)^2 \, dx \\
&= 1.
\end{align}
$$

To compute the probability that the two types of nuts together make up at most ${50}\%$ of the can, let $A = \{ \left( {x, y}\right) : 0 \leq x \leq 1,0 \leq y \leq 1$, and $x + y \leq {.5}\}$, as shown in Figure 5.3. 
Then
$$
\begin{align}
P\left( (X, Y) \in A \right) &= \iint_{A} f(x, y) \, dx \, dy \\
&= \int_{0}^{0.5} \int_{0}^{0.5 - x} 24xy \, dy \, dx \\
&= 0.0625.
\end{align}
$$

Figure 5.3 
Computing $P\left\lbrack {\left( {X, Y}\right) \in A}\right\rbrack$ for Example 5.5
![0192609f-6f5c-74c9-8588-c1ef28b2184d_6_799_469_564_433_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_6_799_469_564_433_0.jpg)

The marginal pdf for almonds is obtained by holding $X$ fixed at $x$ and integrating the joint pdf $f\left( {x, y}\right)$ along the vertical line through $x$ :
$$
\begin{align}
{f}_{X}\left( x\right) 
&= {\int }_{-\infty }^{\infty }f\left( {x, y}\right) {dy} \\
&= \left\{ \begin{matrix} {\int }_{0}^{1 - x}{24xydy} = {12x}{\left( 1 - x\right) }^{2} & 0 \leq x \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
\end{align}
$$
$$
f_X(x) = \int_{-\infty}^{\infty} f(x, y) \, dy = 
\begin{cases} 
    \int_{0}^{1 - x} 24xy \, dy = 12x(1 - x)^2 & 0 \leq x \leq 1 \\ 
    0 & \text{otherwise} 
\end{cases}
$$
By symmetry of $f\left( {x, y}\right)$ and the region $D$, the marginal pdf of $Y$ is obtained by replacing $x$ and $X$ in ${f}_{X}\left( x\right)$ by $y$ and $Y$, respectively.