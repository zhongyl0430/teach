If a publisher of nontechnical books takes great pains to ensure that its books are free of typographical errors, so that 
- the probability of any given page containing at least one such error is .005
- errors are independent from page to page,

> [!question] 
> What is the probability that one of its 600-page novels will contain exactly one page with errors? 
> At most three pages with errors?

With $S$ denoting a page containing at least one error and $F$ an error-free page, the number $X$ of pages containing at least one error is a binomial rv with $n = {600}$ and $p = {.005}$, so ${np} = 3$. 
We wish
$$
\begin{aligned}
    P(X = 1) &= b(1; 600, 0.005) \\
    &\approx p(1; 3) = \frac{e^{-3} \cdot 3^{1}}{1!} \\
    &= 0.14936
\end{aligned}
$$

The binomial value is $b\left( {1;{600},{.005}}\right) = {.14899}$ , so the approximation is very good.

Similarly,
$$P\left( {X \leq 3}\right) \approx \mathop{\sum }\limits_{{x = 0}}^{3}p\left( {x;3}\right) = F\left( {3;3}\right) = {.647}$$
which to three-decimal-place accuracy is identical to $B\left( {3;{600},{.005}}\right)$ .