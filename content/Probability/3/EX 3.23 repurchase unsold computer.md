- Scenario Overview:
	- The computer store purchases 3 computers at $500 each.
	- Selling price per computer: $1000.
	- The manufacturer will repurchase unsold computers at $200 each.
- Definition of Random Variable:
	- Let $X$ represent the number of computers sold.
- Probability Mass Function:
	- The probabilities for the number of computers sold are:
		- $p(0) = 0.1$
	    - $p(1) = 0.2$
	    - $p(2) = 0.3$
	    - $p(3) = 0.4$
- Profit Function:
	- The profit associated with selling $X$ units is defined as:
    $$
    h(X) = \text{Revenue} - \text{Cost}
    $$
	- The profit can be expressed as:
    $$
    h(X) = 1000X + 200(3 - X) - 1500
    $$
	- Simplifying this gives:
    $$
    h(X) = 1000X + 600 - 200X - 1500 = 800X - 900
    $$

- Conclusion:
	- The profit function $h(X) = 800X - 900$ captures the financial outcome based on the number of computers sold.
	- Understanding the distribution of $X$ will allow for calculations of expected profit and decision-making for the store.
	- The expected profit is then
$$
\begin{align}
E[h(X)] &= h(0) \cdot p(0) + h(1) \cdot p(1) + h(2) \cdot p(2) + h(3) \cdot p(3) \\
        &= (-900)(0.1) + (-100)(0.2) + (700)(0.3) + (1500)(0.4) \\
        &= \$700
\end{align}
$$