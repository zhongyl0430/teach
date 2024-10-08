The pool of prospective jurors for a certain case consists of 50 individuals, of whom 35 are employed. Suppose that 6 of these individuals are randomly selected one by one to sit in the jury box for initial questioning by lawyers for the defense and the prosecution. Label the $i$ th person selected (the ${ith}$ trial) as a success $S$ if he or she is employed and a failure $F$ otherwise. Then
$$P\left( {S\text{ on first trial }}\right) = \frac{35}{50} = {.70}$$
and
$$
\begin{align}
&P(S \text{ on second trial}) \\
&= P(SS) + P(FS) \\
&= P(\text{second } S \mid \text{first } S) P(\text{first } S) \\
&\quad + P(\text{second } S \mid \text{first } F) P(\text{first } F) \\
&= \frac{34}{49} \cdot \frac{35}{50} + \frac{35}{49} \cdot \frac{15}{50} \\
&= \frac{35}{50} \left( \frac{34}{49} + \frac{15}{49} \right) \\
&= \frac{35}{50} \\
&= 0.70
\end{align}
$$

Similarly, it can be shown that $P\left( {S\text{on}i\text{th trial}}\right) = {.70}$ for $i = 3,4,5,6$. However, if the first five individuals selected are all $S$ , then only ${30S}$ s remain for the sixth selection. Thus,
$$P\left( {S\text{ on sixth trial } \mid {SSSSS}}\right) = {30}/{45} = {.667}$$
whereas
$$P\left( {S\text{ on sixth trial } \mid {FFFFF}}\right) = {35}/{45} = {.778}$$

The experiment is not binomial because the trials are not independent.
In general, if sampling is without replacement, the experiment will not yield independent trials.

Now consider a large county that has 500,000 individuals in its jury pool, of whom 400,000 are employed. A sample of 10 individuals from the pool is chosen without replacement. Again the $i$ th trial is regarded as a success $S$ if the $i$ th individual is employed. The important difference between this and the previous scenario is that the size of the population being sampled is very large relative to the sample size.
In this case
$$P\left( {S\text{ on }2 \mid S\text{ on }1}\right) = \frac{{399},{999}}{{499},{999}} = {.8000}$$
and
$$P\left( {S\text{ on }{10} \mid S\text{ on first }9}\right) = \frac{{399},{991}}{{499},{991}} = {.799996} \approx {.8000}$$
$$P\left( {S\text{ on }{10} \mid F\text{ on first }9}\right) = \frac{{400},{000}}{{499},{991}} = {.800014} \approx {.8000}$$

These calculations suggest that although the trials are not exactly independent, the conditional probabilities differ so slightly from one another that for practical purposes the trials can be regarded as independent with constant $P\left( S\right) = {.8}$ . Thus, to a very good approximation, the experiment is binomial with $n = {10}$ and $p = {.8}$ .