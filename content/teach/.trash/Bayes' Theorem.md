
The computation of a posterior probability $P\left( {{A}_{i} \mid B}\right)$ from given prior probabilities $P\left( {A}_{i}\right)$ and conditional probabilities $P\left( {B \mid {A}_{i}}\right)$ occupies a central position in elementary probability. 
- The general rule for such computations, which is really just a simple application of the multiplication rule, goes back to Reverend Thomas Bayes, who lived in the eighteenth century. 
To state it we first need another result. 
- Recall that events ${A}_{1},\ldots ,{A}_{k}$ are mutually exclusive if no two have any common outcomes. 
- The events are **exhaustive** if one ${A}_{i}$ must occur, so that ${A}_{1} \cup \ldots \cup {A}_{k} = \mathcal{E}$ .

> [!theorem] The Law of Total Probability
> Let ${A}_{1},\ldots ,{A}_{k}$ be mutually exclusive and exhaustive events. Then for any other event $B$ ,
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



[[EX 2.30 spam email]]

> [!theorem] Bayes' Theorem
> - Let ${A}_{1},{A}_{2},\ldots ,{A}_{k}$ be a collection of
> 	- $k$ mutually exclusive and exhaustive events 
> 	- with *prior probabilities* $P\left( {A}_{i}\right) \left( {i = 1,\ldots ,k}\right)$ . 
> - Then for any other event $B$ for which $P\left( B\right) > 0$ , 
> 	- the *posterior probability* of ${A}_{j}$ given that $B$ has occurred is
> $$
> \begin{align}
> P\left( {{A}_{j} \mid B}\right) 
> &= \frac{P\left( {{A}_{j} \cap B}\right) }{P\left( B\right) } \\
> &= \frac{P\left( {B \mid {A}_{j}}\right) P\left( {A}_{j}\right) }{\mathop{\sum }\limits_{{i = 1}}^{k}P\left( {B \mid {A}_{i}}\right) \cdot P\left( {A}_{i}\right) }\;j = 1,\ldots ,k \tag{2.6}
> \end{align}
> $$

- The transition from the second to the third expression in (2.6) rests on using 
	- the multiplication rule in the numerator 
	- and the law of total probability in the denominator. 
- The proliferation of events and subscripts in (2.6) can be a bit intimidating to probability newcomers. 
- As long as there are relatively few events in the partition, a *tree diagram* (as in Example 2.29) can be used as a basis for calculating posterior probabilities without ever referring explicitly to Bayes' theorem.

从（2.6）中的第二个表达式过渡到第三个表达式，依赖于在分子中使用乘法规则以及在分母中使用全概率定律。对于概率初学者来说，（2.6）中事件和下标的激增可能会有些令人畏惧。只要划分中的事件相对较少，就可以使用树状图（如示例2.29中所示）作为计算后验概率的基础，而无需明确引用贝叶斯定理。

[[EX 2.31 Incidence of a rare disease]]
