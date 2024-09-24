- Each day, Monday through Friday, a batch of components sent by a first supplier arrives at a certain inspection facility. 
- Two days a week, a batch also arrives from a second supplier. 
	- $80 \%$ of all supplier 1's batches pass inspection, 
	- ${90}\%$ of supplier 2's do likewise. 

> [!question]
> What is the probability that, on a randomly selected day, two batches pass inspection? 

We will answer this assuming that on days when two batches are tested, 
- whether the first batch passes is independent of whether the second batch does so. 
Figure 2.13 displays the relevant information.

Figure 2.13 Tree diagram for Example 2.35
![Figure 2.13](01913607-292d-7d0a-a250-4b01870485a1_36_681895.jpg)

$$
\begin{aligned}
P\left( \text{two pass}\right) 
&= P\left( {\text{two received} \cap \text{both pass}}\right)\\
&= P\left( {\text{both pass} \mid \text{two received}}\right) \cdot P\left( \text{two received}\right)\\
&= \left\lbrack {\left( {.8}\right) \left( {.9}\right) }\right\rbrack \left( {.4}\right) = {.288}
\end{aligned}
$$


<a id="org56d0125"></a>