If a publisher of nontechnical books takes great pains to
ensure that its books are free of typographical errors, so that the
probability of any given page containing at least one such error is .005
and errors are independent from page to page, what is the probability
that one of its 600-page novels will contain exactly one page with
errors? At most three pages with errors?

With $S$ denoting a page containing at least one error and $F$ an
error-free page, the number $X$ of pages containing at least one error
is a binomial rv with $n = {600}$ and $p = {.005}$ , so ${np} = 3$ . We
wish

$$P\left( {X = 1}\right) = b\left( {1;{600},{.005}}\right) \approx p\left( {1;3}\right) = \frac{{e}^{-3}{\left( 3\right) }^{1}}{1!} = {.14936}$$

The binomial value is $b\left( {1;{600},{.005}}\right) = {.14899}$ , so
the approximation is very good.

Similarly,

$$P\left( {X \leq 3}\right) \approx \mathop{\sum }\limits_{{x = 0}}^{3}p\left( {x;3}\right) = F\left( {3;3}\right) = {.647}$$

which to three-decimal-place accuracy is identical to
$B\left( {3;{600},{.005}}\right)$ .