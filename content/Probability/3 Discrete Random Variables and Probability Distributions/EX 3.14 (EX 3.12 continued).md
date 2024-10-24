([[EX 3.12 gender of newborn child]] continued)
The pmf of $X =$ the number of births up to and including that of the first boy had
$$p\left( x\right) = \left\{ \begin{matrix} {\left( 1 - p\right) }^{x - 1}p & x = 1,2,3,\ldots \\ 0 & \text{ otherwise } \end{matrix}\right.$$

For any positive integer $x$ ,
$$
\begin{align}
F(x) &= \mathop{\sum}\limits_{y \leq x} p(y) \\
     &= \mathop{\sum}\limits_{y = 1}^{x} (1 - p)^{y - 1} p \\
     &= p \mathop{\sum}\limits_{y = 0}^{x - 1} (1 - p)^{y} \tag{3.4}
\end{align}
$$

To evaluate this sum, recall that the partial sum of a geometric series is
$$\mathop{\sum }\limits_{{y = 0}}^{k}{a}^{y} = \frac{1 - {a}^{k + 1}}{1 - a}$$

Using this in Equation (3.4), with $a = 1 - p$ and $k = x - 1$ , gives
$$F\left( x\right) = p \cdot \frac{1 - {\left( 1 - p\right) }^{x}}{1 - \left( {1 - p}\right) } = 1 - {\left( 1 - p\right) }^{x}$$
where $x$ a positive integer. 

Since $F$ is constant in between positive integers,
$$F\left( x\right) = \left\{ \begin{matrix} 0 & x < 1 \\ 1 - {\left( 1 - p\right) }^{\left\lbrack x\right\rbrack } & x \geq 1 \end{matrix}\right. \tag{3.5}$$

where $\left\lbrack x\right\rbrack$ is the largest integer $\leq x$ 
- e.g., $\left\lbrack {2.7}\right\rbrack = 2$ 

Thus if $p = {.51}$ as in the birth example, then the probability of having to examine at most five births to see the first boy is 
$$F\left( 5\right) = 1 - {\left( {.49}\right) }^{5} = 1 - {.0282} = {.9718}$$
whereas $F\left( {10}\right) \approx {1.0000}$. 
This cdf is graphed in Figure 3.6.

Figure 3.6 
A graph of $F\left( x\right)$ for Example 3.14
![image](images/019165cb-e657-75f5-b964-f15ddb80567f_12_594421.jpg)
