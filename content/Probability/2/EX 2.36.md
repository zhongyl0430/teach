The article "Reliability Evaluation of Solar Photovoltaic Arrays" (Solar Energy, 2002: 129-141) presents various configurations of solar photovoltaic arrays consisting of crystalline silicon solar cells. 

Figure 2.14 
![](01913607-292d-7d0a-a250-4b01870485a1_37_425535.jpg)

^fig-2-14

System configurations for Example 2.36: 
a. series-parallel; 
b. total-cross-tied

Consider first the system illustrated in [[#^fig-2-14|Figure 2.14]] (a).
- There are two subsystems connected in parallel, 
	- each one containing three cells. 
- In order for the system to function, 
	- at least one of the two parallel subsystems must work. 
- Within each subsystem, 
	- the three cells are connected in series, 
	- so a subsystem will work only if all cells in the subsystem work. 

> [!question]
> - Consider a particular lifetime value ${t}_{0}$
> - Suppose we want to determine the probability that the system lifetime exceeds ${t}_{0}$. 

- Let ${A}_{i}$ denote the event that the lifetime of cell $i$ exceeds ${t}_{0}\left( {i = 1,2,\ldots ,6}\right)$ . 
- We assume that the ${A}_{i}^{\prime }s$ are independent events
	- whether any particular cell lasts more than ${t}_{0}$ hours has no bearing on whether or not any other cell does
	- and that $P\left( {A}_{i}\right) = {.9}$ for every $i$ since the cells are identical. 
- Then
$$
\begin{aligned}
&P\left( {\text{system lifetime exceeds }{t}_{0}}\right) \\
= &P\left\lbrack {\left( {{A}_{1} \cap {A}_{2} \cap {A}_{3}}\right) \cup \left( {{A}_{4} \cap {A}_{5} \cap {A}_{6}}\right) }\right\rbrack \\
= &P\left( {{A}_{1} \cap {A}_{2} \cap {A}_{3}}\right) + P\left( {{A}_{4} \cap {A}_{5} \cap {A}_{6}}\right) \\
&- P\left\lbrack {\left( {{A}_1 \cap {A}_2 \cap {A}_3}\right) \cap \left( {{A}_4 \cap {A}_5 \cap {A}_6}\right) }\right\rbrack \\
= &\left( {.9}\right) \left( {.9}\right) \left( {.9}\right) + \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) - \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) \\
= &{.927}
\end{aligned}
$$

- Alternatively,
$$
\begin{aligned}
&P\left( {\text{system lifetime exceeds } {t}_{0}}\right) \\
= &1 - P\left( {\text{both subsystem lives are} \leq {t}_{0}}\right) \\
= &1 - {\left\lbrack P\left( \text{ subsystem life is } \leq {t}_{0}\right) \right\rbrack }^{2} \\
= &1 - {\left\lbrack 1 - P\left( \text{ subsystem life is } > {t}_{0}\right) \right\rbrack }^{2} \\
= &1 - {\left\lbrack 1 - {\left( {.9}\right) }^{3}\right\rbrack }^{2} 
= &{.927}
\end{aligned}
$$

Next consider the total-cross-tied system shown in  [[#^fig-2-14|Figure 2.14]] (b), 
- obtained from the series-parallel array by connecting ties across each column of junctions. 
- Now the system fails as soon as an entire column fails, 
- and system lifetime exceeds ${t}_{0}$ 
	- only if the life of every column does so. 
- For this configuration,
$$
\begin{aligned}
&P\left( {\text{system lifetime is at least }{t}_{0}}\right) \\
= &{\left\lbrack P\left( \text{column lifetime exceeds }{t}_{0}\right) \right\rbrack }^{3} \\
= &{\left\lbrack 1 - P\left( \text{ column lifetime is } \leq {t}_{0}\right) \right\rbrack }^{3} \\
= &{\left\lbrack 1 - P\left( \text{ both cells in a column have lifetime } \leq {t}_{0}\right) \right\rbrack }^{3} \\
= &{\left\lbrack 1 - {\left( 1 - {.9}\right) }^{2}\right\rbrack }^{3} \\
= &{.970}
\end{aligned}
$$
