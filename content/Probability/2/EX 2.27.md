- Four individuals have responded to a request by a blood bank for blood donations. 
- None of them has donated before, 
	- so their blood types are unknown. 
- Suppose 
	- only type $\mathrm{O} +$ is desired 
	- only one of the four actually has this type. 
- If the potential donors are selected in random order for typing, 
	- what is the probability that *at least three* individuals must be typed to obtain the desired type?

- Making the identification 
	- $B$ = { first type not $\mathrm{O} +$ } 
	- $A$ = { second type not $\mathrm{O} +$ }, 
	- $P\left( B\right) = 3/4$
- Given that 
	- the first type is not $\mathrm{O} +$ , 
- two of the three individuals left are not $\mathrm{O} +$, 
	- so $P\left( {A \mid B}\right) = 2/3$ . 
- The multiplication rule now gives
$$
\begin{align}
&P\left( \text{at least three individuals are typed}\right) \\
= &P\left( {A \cap B}\right) \\
= &P\left( {A \mid B}\right) \cdot P\left( B\right) \\
= &\frac{2}{3} \cdot \frac{3}{4} = \frac{6}{12} \\
= &{.5}
\end{align}
$$
