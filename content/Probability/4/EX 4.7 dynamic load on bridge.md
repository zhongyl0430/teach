Suppose the pdf of the magnitude $X$ of a dynamic load on a bridge (in newtons) is given by

$$
f\left( x\right) = \left\{ \begin{matrix} \frac{1}{8} + \frac{3}{8}x & 0 \leq x \leq 2 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

For any number $x$ between 0 and 2,

$$
F\left( x\right) = {\int }_{-\infty }^{x}f\left( y\right) {dy} = {\int }_{0}^{x}\left( {\frac{1}{8} + \frac{3}{8}y}\right) {dy} = \frac{x}{8} + \frac{3}{16}{x}^{2}
$$

Thus

$$
F\left( x\right) = \left\{ \begin{matrix} 0 & x < 0 \\ \frac{x}{8} + \frac{3}{16}{x}^{2} & 0 \leq x \leq 2 \\ 1 & 2 < x \end{matrix}\right.
$$

The graphs of $f\left( x\right)$ and $F\left( x\right)$ are shown in Figure 4.9. The probability that the load is between 1 and 1.5 is

$$
P\left( {1 \leq X \leq {1.5}}\right) = F\left( {1.5}\right) - F\left( 1\right)
$$

$$
= \left\lbrack {\frac{1}{8}\left( {1.5}\right) + \frac{3}{16}{\left( {1.5}\right) }^{2}}\right\rbrack - \left\lbrack {\frac{1}{8}\left( 1\right) + \frac{3}{16}{\left( 1\right) }^{2}}\right\rbrack
$$

$$
= \frac{19}{64} = {.297}
$$

The probability that the load exceeds 1 is

$$
P\left( {X > 1}\right) = 1 - P\left( {X \leq 1}\right) = 1 - F\left( 1\right) = 1 - \left\lbrack {\frac{1}{8}\left( 1\right) + \frac{3}{16}{\left( 1\right) }^{2}}\right\rbrack
$$

$$
= \frac{11}{16} = {.688}
$$

![01925166-48c0-7eca-9860-67f13d0848b1_9_475_808_1159_313_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_9_475_808_1159_313_0.jpg)

Figure 4.9 The pdf and cdf for Example 4.7