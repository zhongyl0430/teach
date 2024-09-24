## A Parameter of a Probability Distribution
The pmf of the Bernoulli rv $X$ in Example 3.9 was
$p\left( 0\right) = {.8}$ and $p\left( 1\right) = {.2}$ because ${20}\%$ of all purchasers selected a desktop computer. At another store, it may
be the case that $p\left( 0\right) = {.9}$ and $p\left( 1\right) = {.1}$. More generally, the pmf of any Bernoulli rv can be expressed in the
form $p\left( 1\right) = \alpha$ and $p\left( 0\right) = 1 - \alpha$, where $0 < \alpha < 1$ . Because the pmf depends on the particular value
of $\alpha$ , we often write $p\left( {x;\alpha }\right)$ rather than
just $p\left( x\right)$ :

$$p\left( {x;\alpha }\right) = \left\{ \begin{matrix} 1 - \alpha & \text{ if }x = 0 \\ \alpha & \text{ if }x = 1 \\ 0 & \text{ otherwise } \end{matrix}\right. \tag{3.1}$$

Then each choice of $\alpha$ in Expression (3.1) yields a different pmf.

> [!definition]
> Suppose $p\left( x\right)$ depends on a quantity that can be assigned any one of a number of possible values, with each different value determining a different probability distribution. Such a quantity is called a parameter of the distribution. The collection of all probability distributions for different values of the parameter is called a family of probability distributions.

The quantity $\alpha$ in Expression (3.1) is a parameter. Each different
number $\alpha$ between 0 and 1 determines a different member of the
Bernoulli family of distributions.

[[EX 3.12]]