Each of six randomly selected cola drinkers is given a glass containing cola $S$ and one containing cola $F$. 
The glasses are identical in appearance except for a code on the bottom to identify the cola. 
Suppose there is actually no tendency among cola drinkers to prefer one cola to the other. 
Then $$p = P ( \text{a selected individual prefers $S$} ) = {.5}$$so with $$X = \text{the number among the six who prefer $S$}$$
and $$X \sim \operatorname{Bin}\left( {6,{.5}}\right) .$$

Thus
$$P\left( {X = 3}\right) = b\left( {3;6,{.5}}\right) = \left( \begin{array}{l} 6 \\ 3 \end{array}\right) {\left( {.5}\right) }^{3}{\left( {.5}\right) }^{3} = {20}{\left( {.5}\right) }^{6} = {.313}$$

The probability that at least three prefer $S$ is
$$
\begin{align}
P\left( {3 \leq X}\right) 
&= \mathop{\sum }\limits_{{x = 3}}^{6}b\left( {x;6,{.5}}\right) \\ 
&= \mathop{\sum }\limits_{{x = 3}}^{6}\left( \begin{array}{l} 6 \\ x \end{array}\right) {\left( {.5}\right) }^{x}{\left( {.5}\right) }^{6 - x} \\
&= {.656}
\end{align}
$$
and the probability that at most one prefers $S$ is
$$P\left( {X \leq 1}\right) = \mathop{\sum }\limits_{{x = 0}}^{1}b\left( {x;6,{.5}}\right) = {.109}$$