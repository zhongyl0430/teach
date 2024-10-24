The distribution of the amount of gravel (in tons) sold by a particular construction supply company in a given week is a continuous rv $X$ with pdf
$$
f\left( x\right) = \left\{ \begin{matrix} \frac{3}{2}\left( {1 - {x}^{2}}\right) & 0 \leq x \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

The cdf of sales for any $x$ between 0 and 1 is
$$
\begin{align}
    F\left( x \right) &= \int_{0}^{x} \frac{3}{2} \left( 1 - y^{2} \right) \, dy \\
    &= \left. \frac{3}{2} \left( y - \frac{y^{3}}{3} \right) \right|_{y = 0}^{y = x} \\
    &= \frac{3}{2} \left( x - \frac{x^{3}}{3} \right)
\end{align}
$$

The graphs of both $f\left( x\right)$ and $F\left( x\right)$ appear in Figure 4.11. 

Figure 4.11 
The pdf and cdf for Example 4.9
![01925166-48c0-7eca-9860-67f13d0848b1_11_632_182_904_297_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_11_632_182_904_297_0.jpg)

The $\left( {100p}\right)$ th percentile of this distribution satisfies the equation
$$
p = F\left( {\eta \left( p\right) }\right) = \frac{3}{2}\left\lbrack {\eta \left( p\right) - \frac{{\left( \eta \left( p\right) \right) }^{3}}{3}}\right\rbrack
$$
that is,
$$
{\left( \eta \left( p\right) \right) }^{3} - {3\eta }\left( p\right) + {2p} = 0
$$

For the 50th percentile, $p = {.5}$ , and the equation to be solved is ${\eta }^{3} - {3\eta } + 1 = 0$; the solution is $\eta = \eta \left( {.5}\right) = {.347}$. 
If the distribution remains the same from week to week, then in the long run
- ${50}\%$ of all weeks will result in sales of less than .347 ton
- ${50}\%$ in more than .347 ton.
