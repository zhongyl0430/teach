## The Cumulative Distribution Function 

For some fixed value $x$ , we often wish to compute the probability that the observed value of $X$ will be at most $x$ . For example, let $X$ be
the number of number of beds occupied in a hospital's emergency room at
a certain time of day; suppose the pmf of $X$ is given by

| x   | 0    | 1    | 2    | 3    | 4    |
|-----|------|------|------|------|------|
| p(x)| .20  | .25  | .30  | .15  | .10  |

Then the probability that at most two beds are occupied is

$$P\left( {X \leq 2}\right) = p\left( 0\right) + p\left( 1\right) + p\left( 2\right) = {.75}$$

Furthermore, since $X \leq {2.7}$ if and only if $X \leq 2$ , we also
have $P\left( {X \leq {2.7}}\right) = {.75}$ , and similarly
$P\left( {X \leq {2.999}}\right) = {.75}$ . Since 0 is the smallest
possible $X$ value, $P\left( {X \leq - {1.5}}\right) = 0$ ,
$P\left( {X \leq - {10}}\right) = 0$ , and in fact for any negative
number $x,P\left( {X \leq x}\right) = 0$ . And because 4 is the largest
possible value of
$X,P\left( {X \leq 4}\right) = 1,P\left( {X \leq {9.8}}\right) = 1$ ,
and so on.

Very importantly,

$$P\left( {X < 2}\right) = p\left( 0\right) + p\left( 1\right) = {.45} < {.75} = P\left( {X \leq 2}\right)$$

because the latter probability includes the probability mass at the $x$
value 2 whereas the former probability does not. More generally,
$P\left( {X < x}\right) < P\left( {X \leq x}\right)$ whenever $x$ is a
possible value of $X$ . Furthermore, $P\left( {X \leq x}\right)$ is a
well-defined and computable probability for any number $x$ .

> [!definition] 
> The cumulative distribution function (cdf) $F\left( x\right)$ of a discrete rv variable $X$ with $\operatorname{pmf}p\left( x\right)$ is defined for every number $x$ by
> $$F\left( x\right) = P\left( {X \leq x}\right) = \mathop{\sum }\limits_{{y : y \leq x}}p\left( y\right) \tag{3.3}$$
> For any number $x,F\left( x\right)$ is the probability that the observed value of $X$ will be at most $x$ .

[[EX 3.13]]

For $X$ a discrete rv, the graph of $F\left( x\right)$ will have a jump
at every possible value of $X$ and will be flat between possible values.
Such a graph is called a step function.

[[EX 3.12 EX 3.14 continued]]

In examples thus far, the cdf has been derived from the pmf. This
process can be reversed to obtain the pmf from the cdf whenever the
latter function is available. For example, consider again the rv of
Example 3.7 (the number of computers being used in a lab); possible $X$
values are $0,1,\ldots ,6$ . Then

$$p\left( 3\right) = P\left( {X = 3}\right)$$

$$= \left\lbrack {p\left( 0\right) + p\left( 1\right) + p\left( 2\right) + p\left( 3\right) }\right\rbrack - \left\lbrack {p\left( 0\right) + p\left( 1\right) + p\left( 2\right) }\right\rbrack$$

$$= P\left( {X \leq 3}\right) - P\left( {X \leq 2}\right)$$

$$= F\left( 3\right) - F\left( 2\right)$$

More generally, the probability that $X$ falls in a specified interval
is easily obtained from the cdf. For example,

$$P\left( {2 \leq X \leq 4}\right) = p\left( 2\right) + p\left( 3\right) + p\left( 4\right)$$

$$= \left\lbrack {p\left( 0\right) + \cdots + p\left( 4\right) }\right\rbrack - \left\lbrack {p\left( 0\right) + p\left( 1\right) }\right\rbrack$$

$$= P\left( {X \leq 4}\right) - P\left( {X \leq 1}\right)$$

$$= F\left( 4\right) - F\left( 1\right)$$

Notice that
$P\left( {2 \leq X \leq 4}\right) \neq F\left( 4\right) - F\left( 2\right)$
. This is because the $X$ value 2 is included in $2 \leq X \leq 4$ , so
we do not want to subtract out its probability. However,
$P\left( {2 < X \leq 4}\right) = F\left( 4\right) - F\left( 2\right)$
because $X = 2$ is not in the interval $2 < X \leq 4$ .

> [!proposition]
> For any two numbers $a$ and $b$ with $a \leq b$ ,
> $$P\left( {a \leq X \leq b}\right) = F\left( b\right) - F\left( {a - }\right)$$
> where "$a -$" represents the largest possible $X$ value that is strictly less than $a$ . 
> In particular, if the only possible values are integers and if $a$ and $b$ are integers, then
> $$
> \begin{aligned}
> P\left( {a \leq X \leq b}\right) 
> &= P\left( X = a\text{ or } a + 1 \text{ or ... or } b \right) \\
> &= F\left( b\right) - F\left( {a - 1}\right)
> \end{aligned}
> $$
> Taking $a = b$ yields
> $$P\left( {X = a}\right) = F\left( a\right) - F\left( {a - 1}\right)$$
>  in this case.

The reason for subtracting $F\left( {a - }\right)$ rather than
$F\left( a\right)$ is that we want to include
$P\left( {X = a}\right) ;F\left( b\right) - F\left( a\right)$ gives
$P\left( {a < X \leq b}\right)$ . This proposition will be used
extensively when computing binomial and Poisson probabilities in
Sections 3.4 and 3.6.

[[EX 3.15]]