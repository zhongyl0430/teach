> [!theorem] Bayes' Theorem
> - Let ${A}_{1},{A}_{2},\ldots ,{A}_{k}$ be a collection of
> 	- $k$ *mutually exclusive* and *exhaustive* events 
> 	- with *prior probabilities* $P\left( {A}_{i}\right) \left( {i = 1,\ldots ,k}\right)$ . 
> - Then for any other event $B$ for which $P\left( B\right) > 0$ , 
> 	- the *posterior probability* of ${A}_{j}$ given that $B$ has occurred is
> $$
> \begin{align}
> P\left( {{A}_{j} \mid B}\right) 
> &= \frac{P\left( {{A}_{j} \cap B}\right) }{P\left( B\right) } \\
> &= \frac{P\left( {B \mid {A}_{j}}\right) P\left( {A}_{j}\right) }{\mathop{\sum }\limits_{{i = 1}}^{k}P\left( {B \mid {A}_{i}}\right) \cdot P\left( {A}_{i}\right) }\;\quad \forall j = 1,\ldots ,k \tag{2.6}
> \end{align}
> $$

- The transition from the second to the third expression in (2.6) rests on using 
	- the multiplication rule in the numerator 
	- and the law of total probability in the denominator. 
- The proliferation of events and subscripts in (2.6) can be a bit intimidating to probability newcomers. 