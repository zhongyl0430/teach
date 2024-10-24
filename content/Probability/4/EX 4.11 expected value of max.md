Two species are competing in a region for control of a limited amount of a certain resource. 
Let $X =$ the proportion of the resource controlled by species 1 and suppose $X$ has pdf
$$
f\left( x\right) = \left\{ \begin{array}{ll} 1 & 0 \leq x \leq 1 \\ 0 & \text{ otherwise } \end{array}\right.
$$
which is a uniform distribution on $\left\lbrack {0,1}\right\rbrack$. 
- In her book Ecological Diversity, E. C. Pielou calls this the "broken-stick" model for resource allocation, since it is analogous to breaking a stick at a randomly chosen point. 

Then the species that controls the majority of this resource controls the amount$$
\begin{align}
    h\left( X \right) &= \max \left( X, 1 - X \right) \\
    &= 
    \begin{cases} 
        1 - X & \text{if } 0 \leq X < \frac{1}{2} \\ 
        X & \text{if } \frac{1}{2} \leq X \leq 1 
    \end{cases}
\end{align}
$$

The expected amount controlled by the species having majority control is then
$$
\begin{align}
    E\left[ h\left( X \right) \right] &= \int_{-\infty}^{\infty} \max \left( x, 1 - x \right) \cdot f\left( x \right) \, dx \\
    &= \int_{0}^{1} \max \left( x, 1 - x \right) \cdot 1 \, dx \\
    &= \int_{0}^{1/2} \left( 1 - x \right) \cdot 1 \, dx + \int_{1/2}^{1} x \cdot 1 \, dx \\
    &= \frac{3}{4}
\end{align}
$$