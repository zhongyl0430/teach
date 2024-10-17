
Consider testing batteries coming off an assembly line one by one until one having a voltage within prescribed limits is found.
The simple events are
-   ${E}_{1} = \{ S \}$,
-   ${E}_{2} = \{ FS \}$,
-   ${E}_{3} = \{ FFS \}$,
-   ${E}_{4} = \{ FFFS \}$, ...
---
Suppose the probability of any particular battery being satisfactory is .99.
Then it can be shown that
-   $P\left( {E}_{1} \right) = .99$
-   $P\left( {E}_{2} \right) = \left( .01 \right) \left( {.99}\right)$
-   $P\left( {E}_{3}\right) = {\left( {.01}\right) }^{2}\left( {.99}\right) ,\ldots$
is an assignment of probabilities to the simple events that satisfies the axioms.
In particular, because the ${E}_{i}$'s are disjoint and $\mathcal{S} = {E}_{1} \cup {E}_{2} \cup {E}_{3} \cup \ldots$ , it must be the case that
$$

\begin{aligned}
1
&= P\left( \mathcal{S}\right) \\
&= P\left( {E}_{1}\right) + P\left( {E}_{2}\right) + P\left( {E}_{3}\right) + \cdots \\
&= {.99}\left\lbrack {1 + {.01} + {\left( {.01}\right) }^{2} + {\left( {.01}\right) }^{3} + \cdots }\right\rbrack
\end{aligned}

$$
---
Here we have used the formula for the sum of a geometric series:
$$
a + {ar} + a{r}^{2} + a{r}^{3} + \cdots = \frac{a}{1 - r}
$$

However, another legitimate (according to the axioms) probability assignment of the same "geometric" type is obtained by replacing. 99 by any other number $p$ between 0 and 1 (and .01 by $1 - p$ ).

---