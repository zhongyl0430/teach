- Given:
    - $20\%$ of all copies fail the binding strength test
- Definition:
    - Let $X$ denote the number of failures among randomly selected copies
- Distribution:
    - $X$ follows a binomial distribution
	- Parameters:
        - $n = 15$ (number of selected copies)
        - $p = 0.2$ (probability of failure)

1. The probability that at most 8 fail the test is
$$P\left( {X \leq 8}\right) = \mathop{\sum }\limits_{{y = 0}}^{8}b\left( {y;{15},{.2}}\right) = B\left( {8;{15},{.2}}\right)$$
which is the entry in the $x = 8$ row and the $p = {.2}$ column of the $n = {15}$ binomial table. From Appendix Table A.1, the probability is
$B\left( {8;{15},{.2}}\right) = {.999}$ .

2. The probability that exactly 8 fail is
$$P\left( {X = 8}\right) = P\left( {X \leq 8}\right) - P\left( {X \leq 7}\right) = B\left( {8;{15},{.2}}\right) - B\left( {7;{15},{.2}}\right)$$
which is the difference between two consecutive entries in the $p = {.2}$ column. The result is ${.999} - {.996} = {.003}$ .

3. The probability that at least 8 fail is
$$
\begin{align}
P(X \geq 8) &= 1 - P(X \leq 7) \\
            &= 1 - B(7; 15, 0.2) \\
            &= 1 - \left( \begin{array}{l} \text{entry in } x = 7 \\ \text{row of } p = 0.2 \text{ column} \end{array} \right) \\
            &= 1 - 0.996 \\
            &= 0.004
\end{align}
$$

4. Finally, the probability that between 4 and 7, inclusive, fail is
$$
\begin{align}
P(4 \leq X \leq 7) &= P(X = 4, 5, 6, \text{ or } 7) \\
                   &= P(X \leq 7) - P(X \leq 3) \\
                   &= B(7; 15, 0.2) - B(3; 15, 0.2) \\
                   &= 0.996 - 0.648 \\
                   &= 0.348
\end{align}
$$
Notice that this latter probability is the difference between entries in the $x = 7$ and $x = 3$ rows, not the $x = 7$ and $x = 4$ rows.