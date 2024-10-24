A store carries flash drives with either $1\mathrm{\;{GB}}$, $2\mathrm{\;{GB}}$, $4\mathrm{\;{GB}}$, $8\mathrm{\;{GB}}$, or ${16}\mathrm{\;{GB}}$ of memory. 
The accompanying table gives the distribution of $Y =$ the amount of memory in a purchased drive:

| $y$    | 1   | 2   | 4   | 8   | 16  |
| ------ | --- | --- | --- | --- | --- |
| $p(y)$ | .05 | .10 | .35 | .40 | .10 |

Let's first determine $F\left( y\right)$ for each of the five possible values of $Y$ :
$$
\begin{align}
F(1) &= P(Y \leq 1) = P(Y = 1) = p(1) = 0.05 \\

F(2) &= P(Y \leq 2) = P(Y = 1 \text{ or } 2) = p(1) + p(2) = 0.15 \\

F(4) &= P(Y \leq 4) = P(Y = 1 \text{ or } 2 \text{ or } 4) = p(1) + p(2) + p(4) = 0.50 \\

F(8) &= P(Y \leq 8) = p(1) + p(2) + p(4) + p(8) = 0.90 \\

F(16) &= P(Y \leq 16) = 1
\end{align}
$$

Now for any other number $y,F\left( y\right)$ will equal the value of $F$ at the closest possible value of $Y$ to the left of $y$ . 
For example,
$$F\left( {2.7}\right) = P\left( {Y \leq {2.7}}\right) = P\left( {Y \leq 2}\right) = F\left( 2\right) = {.15}$$
$$F\left( {7.999}\right) = P\left( {Y \leq {7.999}}\right) = P\left( {Y \leq 4}\right) = F\left( 4\right) = {.50}$$

If $y$ is less than $1,F\left( y\right) = 0$ \[e.g. $F\left( {.58}\right) = 0$ \], and if $y$ is at least ${16},F\left( y\right) = 1$ \[e.g., $F\left( {25}\right) = 1\rbrack$.
The cdf is thus
$$F\left( y\right) = \left\{ \begin{matrix} 0 & y < 1 \\ {.05} & 1 \leq y < 2 \\ {.15} & 2 \leq y < 4 \\ {.50} & 4 \leq y < 8 \\ {.90} & 8 \leq y < {16} \\ 1 & {16} \leq y \end{matrix}\right.$$
A graph of this cdf is shown in Figure 3.5.

Figure 3.5 
A graph of the cdf of Example 3.13
![image](images/019165cb-e657-75f5-b964-f15ddb80567f_11_550958.jpg)