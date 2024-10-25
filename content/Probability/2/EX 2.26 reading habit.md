- The event whose probability is desired might be a union or intersection of other events, 
	- the same could be true of the conditioning event.

- A news magazine publishes three columns entitled 
	- "Art" $\left( A\right)$ ,
	- "Books" $\left( B\right)$ , 
	- "Cinema" $\left( C\right)$. 
- Reading habits of a randomly selected reader with respect to these columns are

| Read regularly | $A$ | $B$ | $C$ | $A \cap B$ | $A \cap C$ | $A \cap B \cap C$ |
| -------------- | --- | --- | --- | ---------- | ---------- | ----------------- |
| Probability    | .14 | .23 | .37 | .08        | .09        | .05               |

Figure 2.9 illustrates relevant probabilities.

Figure 2.9 Venn diagram for Example 2.26
![Figure 2.9](01913607-292d-7d0a-a250-4b01870485a1_26_654372.jpg)

Consider the following four conditional probabilities:
1. $P\left( {A \mid B}\right) = \frac{P\left( {A \cap B}\right) }{P\left( B\right) } = \frac{.08}{.23} = {.348}$
2. The probability that the selected individual regularly reads the Art column given that he or she regularly reads *at least one of the other two columns* is
$$
\begin{align}
P\left( {A \mid B \cup C}\right) 
&= \frac{P\left( {A \cap \left( {B \cup C}\right) }\right) }{P\left( {B \cup C}\right) } \\
&= \frac{{.04} + {.05} + {.03}}{.47} = \frac{.12}{.47} = {.255}
\end{align}
$$
3. $P\left( {A \mid \text{reads at least one}}\right)$ is equal to 
$$
\begin{align}
P\left( {A \mid A \cup B \cup C}\right) 
&= \frac{P\left( {A \cap \left( {A \cup B \cup C}\right) }\right) }{P\left( {A \cup B \cup C}\right) } \\
&= \frac{P\left( A\right) }{P\left( {A \cup B \cup C}\right) } = \frac{.14}{.49} = {.286}
\end{align}
$$
4. The probability that the selected individual reads *at least one of the first two columns* given that he or she reads the Cinema column is
$$
P\left( {A \cup B \mid C}\right) = \frac{P\left( {\left( {A \cup B}\right) \cap C}\right) }{P\left( C\right) } = \frac{{.04} + {.05} + {.08}}{.37} = {.459}
$$


<a id="orgdef9372"></a>