
> [!property] probability of null set
> $P \left( \varnothing \right) = 0$ where $\varnothing$ is the null event (the event containing no outcomes whatsoever).

This in turn implies that the property contained in Axiom 3 is valid for a finite collection of disjoint events.

`\begin{proof}`
First consider the infinite collection 
$$A_1 = \varnothing, A_2 = \varnothing, A_3 = \varnothing,\ldots .$$
Since $\varnothing \cap \varnothing = \varnothing$, the events in this collection are disjoint and $\cup A_i = \varnothing$.
The third axiom then gives
$$
P \left( \varnothing \right) = \sum P \left( \varnothing \right)
$$
This can happen only if $P \left( \varnothing \right) = 0$.

Now suppose that ${A}_{1},{A}_{2},\ldots ,{A}_{k}$ are disjoint events, and append to these the infinite collection $A_{k+1} = \varnothing$, $A_{k + 2} = \varnothing$, ${A}_{k + 3} = \varnothing$, ... .
Again invoking the third axiom,
$$
\begin{aligned}
P\left( \bigcup_{i = 1}^{k} A_i \right)
&= P \left( \bigcup_{i = 1}^{\infty} A_i \right) \\
&= \sum_{i = 1}^{\infty} P \left( A_i \right) \\
&= \sum_{i = 1}^{k} P \left( A_i \right)
\end{aligned}
$$
as desired.
`\end{proof}`


- [[EX 2.11 toss a thumbtack]]
- [[EX 2.12 test batteries]]
