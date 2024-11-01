A binomial experiment consists of $n$ dichotomous (success-failure), homogenous (constant success probability) independent trials. Now consider a trinomial experiment in which each of the $n$ trials can result in one of three possible outcomes. For example, each successive customer at a store might pay with cash, a credit card, or a debit card. The trials are assumed independent. Let ${p}_{1} = P$ (trial results in a type 1 outcome) and define ${p}_{2}$ and ${p}_{3}$ analogously for type 2 and type 3 outcomes. The random variables of interest here are ${X}_{i} =$ the number of trials that result in a type $i$ outcome for $i = 1,2,3$.

In $n = {10}$ trials, the probability that the first five are type 1 outcomes, the next three are type 2, and the last two are type 3-that is, the probability of the experimental outcome 1111122233-is ${p}_{1}^{5} \cdot {p}_{2}^{3} \cdot {p}_{3}^{2}$. This is also the probability of the outcome 1122311123, and in fact the probability of any outcome that has exactly five 1 ’s, three 2’s, and two 3’s. Now to determine the probability $P\left( {{X}_{1} = 5,{X}_{2} = 3}\right.$, and ${X}_{3} = 2$ ), we have to count the number of outcomes that have exactly five 1 ’s, three 2 ’s, and two 3’s. First, there are $\left( \begin{matrix} {10} \\ 5 \end{matrix}\right)$ ways to choose five of the trials to be the type 1 outcomes. Now from the remaining five trials, we choose three to be the type 2 outcomes, which can be done in $\left( \begin{array}{l} 5 \\ 3 \end{array}\right)$ ways. This determines the remaining two trials, which consist of type 3 outcomes. So the total number of ways of choosing five 1 's, three 2's, and two 3's is
$$
\left( \begin{matrix} {10} \\ 5 \end{matrix}\right) \cdot \left( \begin{array}{l} 5 \\ 3 \end{array}\right) = \frac{{10}!}{5!5!} \cdot \frac{5!}{3!2!} = \frac{{10}!}{5!3!2!} = {2520}
$$

Thus we see that $P\left( {{X}_{1} = 5,{X}_{2} = 3,{X}_{3} = 2}\right) = {2520}{p}_{1}^{5} \cdot {p}_{2}^{3} \cdot {p}_{3}^{2}$. Generalizing this to $n$ trials gives
$$
p\left( {{x}_{1},{x}_{2},{x}_{3}}\right) = P\left( {{X}_{1} = {x}_{1},{X}_{2} = {x}_{2},{X}_{3} = {x}_{3}}\right) = \frac{n!}{{x}_{1}!{x}_{2}!{x}_{3}!}{p}_{1}^{{x}_{1}}{p}_{2}^{{x}_{2}}{p}_{3}^{{x}_{3}}
$$
for ${x}_{1} = 0,1,2,\ldots ;{x}_{2} = 0,1,2,\ldots ;{x}_{3} = 0,1,2,\ldots$ such that ${x}_{1} + {x}_{2} + {x}_{3} = n$. Notice that whereas there are three random variables here, the third variable ${X}_{3}$ is actually redundant. For example, in the case $n = {10}$, having ${X}_{1} = 5$ and ${X}_{2} = 3$ implies that ${X}_{3} = 2$ (just as in a binomial experiment there are actually two rv’s-the number of successes and number of failures - but the latter is redundant).

As a specific example, the genetic allele of a pea section can be either AA, Aa, or aa. A simple genetic model specifies $P\left( \mathrm{{AA}}\right) = {.25}, P\left( \mathrm{{Aa}}\right) = {.50}$, and $P\left( \mathrm{{aa}}\right) = {.25}$. If the alleles of 10 independently obtained sections are determined, the probability that exactly five of these are $\mathrm{{Aa}}$ and two are $\mathrm{{AA}}$ is
$$
p\left( {2,5,3}\right) = \frac{{10}!}{2!5!3!}{\left( {.25}\right) }^{2}{\left( {.50}\right) }^{5}{\left( {.25}\right) }^{3} = {0.769}
$$

A natural extension of the trinomial scenario is an experiment consisting of $n$ independent and identical trials, in which each trial can result in any one of $r$ possible outcomes. Let ${p}_{i} = P$ (outcome $i$ on any particular trial), and define random variables by ${X}_{i} =$ the number of trials resulting in outcome $i\left( {i = 1,\ldots, r}\right)$. This is called a multinomial experiment, and the joint pmf of ${X}_{1},\ldots,{X}_{r}$ is called the multinomial distribution. An argument analogous to the one used to derive the trinomial pmf gives the multinomial pmf as
$$
\begin{align}
p\left( x_{1}, \ldots, x_{r} \right) 
&= \begin{cases} 
\frac{n!}{\left( x_{1}! \right) \left( x_{2}! \right) \cdots \left( x_{r}! \right)} \cdot p_{1}^{x_{1}} \cdots p_{r}^{x_{r}} & \text{ if } x_{i} = 0, 1, 2, \ldots; \; x_{1} + \cdots + x_{r} = n \\ 
0 & \text{ otherwise } 
\end{cases}
\end{align}
$$
