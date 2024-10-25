
When events $A$ and $B$ are mutually exclusive, 
$$P\left( {A \cup B}\right) = P\left( A\right) + P\left( B\right) .$$
For events that are not mutually exclusive, adding $P\left( A\right)$ and $P\left( B\right)$ results in "double-counting" outcomes in the intersection.
The next result, the **addition rule** for a double union probability, shows how to correct for this.

> [!property]
> For any two events $A$ and $B$ ,
> $$
> P\left( {A \cup B}\right) = P\left( A\right) + P\left( B\right) - P\left( {A \cap B}\right)
> $$

`\begin{proof}`
Note first that $A \cup B$ can be decomposed into two disjoint events, $A$ and $B \cap {A}'$; the latter is the part of $B$ that lies outside $A$ (see [[#^fig-2-4|Figure 2.4]]).

Figure 2.4 Representing $A \cup B$ as a union of disjoint events
![[01913607-292d-7d0a-a250-4b01870485a1_11_871099.jpg]]

^fig-2-4

Furthermore, $B$ itself is the union of the two disjoint events $A \cap B$ and ${A}' \cap B$ , so 
$$P\left( B\right) =$ $P\left( {A \cap B}\right) + P\left( {{A}' \cap B}\right) .$$
Thus
$$
\begin{aligned}
P\left( A \cup B \right)
&= P\left( A \right) + P\left( B \cap A' \right) \\
&= P\left( A \right) + \left\lbrack P\left( B \right) - P\left( A \cap B \right)  \right\rbrack \\
&= P\left( A \right) + P\left( B \right) - P\left( A \cap B \right)
\end{aligned}
$$
`\end{proof}`

[[EX 2.14 services of households]]