Starting at a fixed time, we observe the gender of each
newborn child at a certain hospital until a boy $\left( B\right)$ is
born. Let $p = P\left( B\right)$ , assume that successive births are
independent, and define the rv $X$ by $x =$ number of births observed.
Then

$$p\left( 1\right) = P\left( {X = 1}\right) = P\left( B\right) = p$$

$$p\left( 2\right) = P\left( {X = 2}\right) = P\left( {GB}\right) = P\left( G\right) \cdot P\left( B\right) = \left( {1 - p}\right) p$$

and

$$p\left( 3\right) = P\left( {X = 3}\right) = P\left( {GGB}\right) = P\left( G\right) \cdot P\left( G\right) \cdot P\left( B\right) = {\left( 1 - p\right) }^{2}p$$

Continuing in this way, a general formula emerges:

$$p\left( x\right) = \left\{ \begin{matrix} {\left( 1 - p\right) }^{x - 1}p & x = 1,2,3,\ldots \\ 0 & \text{ otherwise } \end{matrix}\right. \tag{3.2}$$

The parameter $p$ can assume any value between 0 and 1 . Expression
(3.2) describes the family of geometric distributions. In the gender
scenario, $p = {.51}$ might be appropriate, but if we were looking for
the first child with Rh-positive blood, then it might be the case that
$p = {.85}$ .