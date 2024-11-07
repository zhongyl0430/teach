In [[EXAMPLE 5.5]], the joint pdf of the amount $X$ of almonds and amount $Y$ of cashews in a 1-lb can of nuts was
$$
f\left( {x, y}\right) = \left\{ \begin{matrix} {24xy} & 0 \leq x \leq 1,0 \leq y \leq 1, x + y \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

If 1 lb of almonds costs the company $\$ {1.50}$, $1\mathrm{{lb}}$ of cashews costs $\$ {2.25}$ , and $1\mathrm{{lb}}$ of peanuts costs $\$ {.75}$, then the total cost of the contents of a can is
$$
h\left( {X, Y}\right) = \left( {1.5}\right) X + \left( {2.25}\right) Y + \left( {.75}\right) \left( {1 - X - Y}\right) = {.75} + {.75X} + {1.5Y}
$$
(since $1 - X - Y$ of the weight consists of peanuts). 
The expected total cost is
$$
\begin{align}
E[h(X,Y)] &= \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} h(x,y) \cdot f(x,y) \, dxdy \\
&= \int_{0}^{1} \int_{0}^{1-x} \left( 0.75 + 0.75x + 1.5y \right) \cdot 24xy \, dydx = \$ {1.65}
\end{align}
$$