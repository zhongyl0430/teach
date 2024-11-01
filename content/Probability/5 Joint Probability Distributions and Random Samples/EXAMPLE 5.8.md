Suppose that the lifetimes of two components are independent of one another and that the first lifetime, ${X}_{1}$, has an exponential distribution with parameter ${\lambda }_{1}$, whereas the second, ${X}_{2}$, has an exponential distribution with parameter ${\lambda }_{2}$. Then the joint pdf is
$$
\begin{align}
&f\left( x_{1}, x_{2} \right) \\
&= f_{X_{1}}\left( x_{1} \right) \cdot f_{X_{2}}\left( x_{2} \right) \\
&= \begin{cases} 
\lambda_{1} e^{-\lambda_{1} x_{1}} \cdot \lambda_{2} e^{-\lambda_{2} x_{2}} = \lambda_{1} \lambda_{2} e^{-\lambda_{1} x_{1} - \lambda_{2} x_{2}} & \text{ if } x_{1} > 0, x_{2} > 0 \\ 
0 & \text{ otherwise } 
\end{cases}
\end{align}
$$

Let ${\lambda }_{1} = 1/{1000}$ and ${\lambda }_{2} = 1/{1200}$, so that the expected lifetimes are 1000 hours and 1200 hours, respectively. The probability that both component lifetimes are at least 1500 hours is
$$
\begin{align}
&P\left( 1500 \leq X_{1}, \; 1500 \leq X_{2} \right) \\
&= P\left( 1500 \leq X_{1} \right) \cdot P\left( 1500 \leq X_{2} \right) \\
&= e^{-\lambda_{1} \left( 1500 \right)} \cdot e^{-\lambda_{2} \left( 1500 \right)} \\
&= \left( 0.2231 \right) \left( 0.2865 \right) = 0.0639.
\end{align}
$$
