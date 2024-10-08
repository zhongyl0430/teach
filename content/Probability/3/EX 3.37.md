- A pediatrician aims to recruit 5 couples for a childbirth regimen.
	- Each couple is expecting their first child.
- Let:
	- $p = P$: the probability a randomly selected couple agrees to participate.
	- Given: $p = 0.2$.
- We want to find the probability that:
	- 15 couples must be asked before 5 agree to participate.
	- This means we observe 10 failures (F) before the fifth success (S).
- Denote $S = \{\text{agrees to participate}\}$.
- Relevant variables:
	- $r = 5$: number of successes needed.
	- $p = 0.2$: probability of success.
	- $x = 10$: number of failures before the fifth success.
- Substitute these into the negative binomial formula:
	- ${nb}(x; r; p)$ gives the probability of this scenario.
$${nb}\left( {{10};5,{.2}}\right) = \left( \begin{matrix} {14} \\ 4 \end{matrix}\right) {\left( {.2}\right) }^{5}{\left( {.8}\right) }^{10} = {.034}$$

The probability that at most ${10}\mathrm{F}$ 's are observed (at most 15 couples are asked) is

$$
\begin{align}
P(X \leq 10) &= \sum_{x=0}^{10} nb(x; 5, 0.2) \\
             &= (0.2)^5 \sum_{x=0}^{10} \binom{x + 4}{4} (0.8)^x \\
             &= 0.164
\end{align}
$$
