> [!theorem] The Law of Total Probability
> Let ${A}_{1},\ldots ,{A}_{k}$ be mutually exclusive and exhaustive events. 
> Then for any other event $B$ ,
> $$
> \begin{align}
> P\left( B\right) 
> &= P\left( {B \mid {A}_{1}}\right) P\left( {A}_{1}\right) + \cdots + P\left( {B \mid {A}_{k}}\right) P\left( {A}_{k}\right) \\
> &= \mathop{\sum }\limits_{{i = 1}}^{k}P\left( {B \mid {A}_{i}}\right) P\left( {A}_{i}\right) \tag{2.5}
> \end{align}
> $$

`\begin{proof}`
- Because the ${\mathrm{A}}_{i}$'s are mutually exclusive and exhaustive, 
	- then if $B$ occurs, it must be in conjunction with *exactly one* of the ${\mathrm{A}}_{i}$'s. 
- That is, $B = \left( {{A}_{1} \cap B}\right) \cup \ldots \cup \left( {{A}_{k} \cap B}\right)$ , 
	- where the events $\left( {{A}_{i} \cap B}\right)$ are mutually exclusive. 
- This "partitioning of $B$ " is illustrated in Figure 2.11. 

Figure 2.11 Partition of $B$ by mutually exclusive and exhaustive ${A}_{i}$'s
![](01913607-292d-7d0a-a250-4b01870485a1_29_505370.jpg)

Thus
$$
P\left( B\right) = \mathop{\sum }\limits_{{i = 1}}^{k}P\left( {{A}_{i} \cap B}\right) = \mathop{\sum }\limits_{{i = 1}}^{k}P\left( {B \mid {A}_{i}}\right) P\left( {A}_{i}\right)
$$
as desired.
`\end{proof}`