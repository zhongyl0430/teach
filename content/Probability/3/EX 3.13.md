EXAMPLE 3.13 A store carries flash drives with either
$1\mathrm{\;{GB}},2\mathrm{\;{GB}},4\mathrm{\;{GB}},8\mathrm{\;{GB}}$ ,
or ${16}\mathrm{\;{GB}}$ of memory. The accompanying table gives the
distribution of $Y =$ the amount of memory in a purchased drive:

| $y$    | 1   | 2   | 4   | 8   | 16  |
| ------ | --- | --- | --- | --- | --- |
| $p(y)$ | .05 | .10 | .35 | .40 | .10 |

Let's first determine $F\left( y\right)$ for each of the five possible
values of $Y$ :

$$F\left( 1\right) = P\left( {Y \leq 1}\right) = P\left( {Y = 1}\right) = p\left( 1\right) = {.05}$$

$$F\left( 2\right) = P\left( {Y \leq 2}\right) = P\left( {Y = 1\text{ or }2}\right) = p\left( 1\right) + p\left( 2\right) = {.15}$$

$$F\left( 4\right) = P\left( {Y \leq 4}\right) = P\left( {Y = 1\text{or }2\text{ or }4}\right) = p\left( 1\right) + p\left( 2\right) + p\left( 4\right) = {.50}$$

$$F\left( 8\right) = P\left( {Y \leq 8}\right) = p\left( 1\right) + p\left( 2\right) + p\left( 4\right) + p\left( 8\right) = {.90}$$

$$F\left( {16}\right) = P\left( {Y \leq {16}}\right) = 1$$

Now for any other number $y,F\left( y\right)$ will equal the value of
$F$ at the closest possible value of $Y$ to the left of $y$ . For
example,

$$F\left( {2.7}\right) = P\left( {Y \leq {2.7}}\right) = P\left( {Y \leq 2}\right) = F\left( 2\right) = {.15}$$

$$F\left( {7.999}\right) = P\left( {Y \leq {7.999}}\right) = P\left( {Y \leq 4}\right) = F\left( 4\right) = {.50}$$

If $y$ is less than $1,F\left( y\right) = 0$ \[e.g.
$F\left( {.58}\right) = 0$ \], and if $y$ is at least
${16},F\left( y\right) = 1$ \[e.g., $F\left( {25}\right) = 1\rbrack$ .
The cdf is thus

$$F\left( y\right) = \left\{ \begin{matrix} 0 & y < 1 \\ {.05} & 1 \leq y < 2 \\ {.15} & 2 \leq y < 4 \\ {.50} & 4 \leq y < 8 \\ {.90} & 8 \leq y < {16} \\ 1 & {16} \leq y \end{matrix}\right.$$

A graph of this cdf is shown in Figure 3.5.

Figure 3.5 A graph of the cdf of Example 3.13
![image](images/019165cb-e657-75f5-b964-f15ddb80567f_11_550958.jpg)
