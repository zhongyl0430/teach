Five friends have purchased tickets to a certain concert. 
If the tickets are for seats 1-5 in a particular row and the tickets are randomly distributed among the five, what is the expected number of seats separating any particular two of the five? 
Let $X$ and $Y$ denote the seat numbers of the first and second individuals, respectively. 
Possible $\left( {X, Y}\right)$ pairs are $\{ \left( {1,2}\right) ,\left( {1,3}\right) ,\ldots ,\left( {5,4}\right) \}$ , and the joint pmf of $\left( {X, Y}\right)$ is
$$
p\left( {x, y}\right) = \left\{ \begin{array}{ll} \frac{1}{20} & x = 1,\ldots ,5;y = 1,\ldots ,5;x \neq y \\ 0 & \text{ otherwise } \end{array}\right.
$$

The number of seats separating the two individuals is $h\left( {X, Y}\right) = \left| {X - Y}\right| - 1$ . The accompanying table gives $h\left( {x, y}\right)$ for each possible $\left( {x, y}\right)$ pair.

| $h(x, y)$ | 1   | 2   | 3   | 4   | 5   |
| --------- | --- | --- | --- | --- | --- |
| 1         | $-$ | 0   | 1   | 2   | 3   |
| 2         | 0   | $-$ | 0   | 1   | 2   |
| 3         | 1   | 0   | $-$ | 0   | 1   |
| 4         | 2   | 1   | 0   | $-$ | 0   |
| 5         | 3   | 2   | 1   | 0   | $-$ |

Thus
$$
E\left\lbrack {h\left( {X, Y}\right) }\right\rbrack = \mathop{\sum }\limits_{\left( x, y\right) }h\left( {x, y}\right) \cdot p\left( {x, y}\right) = \mathop{\sum }\limits_{\substack{{x = 1} \\ {x \neq y} }}^{5}\mathop{\sum }\limits_{\substack{{y = 1} \\ {x \neq y} }}^{5}\left( {\left| {x - y}\right| - 1}\right) \cdot \frac{1}{20} = 1
$$
