Project managers often use a method labeled PERT-for program evaluation and review technique-to coordinate the various activities making up a large project. (One successful application was in the construction of the Apollo spacecraft.) A standard assumption in PERT analysis is that the time necessary to complete any particular activity once it has been started has a beta distribution with $A =$ the optimistic time (if everything goes well) and $B =$ the pessimistic time (if everything goes badly). Suppose that in constructing a single-family house, the time $X$ (in days) necessary for laying the foundation has a beta distribution with $A = 2, B = 5,\alpha = 2$ , and $\beta = 3$ . Then $\alpha /\left( {\alpha + \beta }\right) = {.4}$ , so $E\left( X\right) = 2 + \left( 3\right) \left( {.4}\right) = {3.2}$ . For these values of $\alpha$ and $\beta$ , the pdf of $X$ is a simple polynomial function. The probability that it takes at most 3 days to lay the foundation is

$$
P\left( {X \leq 3}\right) = {\int }_{2}^{3}\frac{1}{3} \cdot \frac{4!}{1!2!}\left( \frac{x - 2}{3}\right) {\left( \frac{5 - x}{3}\right) }^{2}{dx}
$$

$$
= \frac{4}{27}{\int }_{2}^{3}\left( {x - 2}\right) {\left( 5 - x\right) }^{2}{dx} = \frac{4}{27} \cdot \frac{11}{4} = \frac{11}{27} = {.407}
$$