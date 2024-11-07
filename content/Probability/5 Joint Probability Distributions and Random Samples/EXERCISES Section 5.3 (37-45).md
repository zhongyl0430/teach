# 37
A particular brand of dishwasher soap is sold in three sizes: ${25}\mathrm{{oz}},{40}\mathrm{{oz}}$ , and ${65}\mathrm{{oz}}$ . Twenty percent of all purchasers select a 25-oz box, 50% select a 40-oz box, and the remaining ${30}\%$ choose a 65-oz box. Let ${X}_{1}$ and ${X}_{2}$ denote the package sizes selected by two independently selected purchasers.

a. Determine the sampling distribution of $\bar{X}$ , calculate $E\left( \bar{X}\right)$ , and compare to $\mu$ .

b. Determine the sampling distribution of the sample variance ${S}^{2}$ , calculate $E\left( {S}^{2}\right)$ , and compare to ${\sigma }^{2}$ .

# 38
There are two traffic lights on a commuter's route to and from work. Let ${X}_{1}$ be the number of lights at which the commuter must stop on his way to work, and ${X}_{2}$ be the number of lights at which he must stop when returning from work. Suppose these two variables are independent, each with pmf given in the accompanying table (so ${X}_{1},{X}_{2}$ is a random sample of size $n = 2$ ).

| \( x_1 \)                   | 0   | 1   | 2   |
|-----------------------------|-----|-----|-----|
| \( p(x_1) \)                | 0.2 | 0.5 | 0.3 |

$$
\mu = {1.1},{\sigma }^{2} = {.49}
$$

a. Determine the pmf of ${T}_{o} = {X}_{1} + {X}_{2}$ .

b. Calculate ${\mu }_{{T}_{o}}$ . How does it relate to $\mu$ , the population mean?

c. Calculate ${\sigma }_{{T}_{o}}^{2}$ . How does it relate to ${\sigma }^{2}$ , the population variance?

d. Let ${X}_{3}$ and ${X}_{4}$ be the number of lights at which a stop is required when driving to and from work on a second day assumed independent of the first day. With ${T}_{o} =$ the sum of all four ${X}_{i}$ ’s, what now are the values of $E\left( {T}_{o}\right)$ and $V\left( {T}_{o}\right)$ ?

e. Referring back to (d), what are the values of $P\left( {{T}_{o} = 8}\right)$ and $P\left( {{T}_{o} \geq 7}\right)$ [Hint: Don’t even think of listing all possible outcomes!]

# 39
It is known that ${80}\%$ of all brand A external hard drives work in a satisfactory manner throughout the warranty period (are "successes"). Suppose that $n = {15}$ drives are randomly selected. Let $X =$ the number of successes in the sample. The statistic $X/n$ is the sample proportion (fraction) of successes. Obtain the sampling distribution of this statistic. [Hint: One possible value of $X/n$ is .2, corresponding to $X = 3$ . What is the probability of this value (what kind of rv is $X)$ ?]

# 40
A box contains ten sealed envelopes numbered $1,\ldots ,{10}$ . The first five contain no money, the next three each contains $\$ 5$ , and there is a $\$ {10}$ bill in each of the last two. A sample of size 3 is selected with replacement (so we have a random sample), and you get the largest amount in any of the envelopes selected. If ${X}_{1},{X}_{2}$ , and ${X}_{3}$ denote the amounts in the selected envelopes, the statistic of interest is $M =$ the maximum of ${X}_{1},{X}_{2}$ , and ${X}_{3}$ .

a. Obtain the probability distribution of this statistic.

b. Describe how you would carry out a simulation experiment to compare the distributions of $M$ for various sample sizes. How would you guess the distribution would change as $n$ increases?

# 41
Let $X$ be the number of packages being mailed by a randomly selected customer at a certain shipping facility. Suppose the distribution of $X$ is as follows:

| \( x \)                   | 1   | 2   | 3   | 4   |
|---------------------------|-----|-----|-----|-----|
| \( p(x) \)                | 0.4 | 0.3 | 0.2 | 0.1 |

a. Consider a random sample of size $n = 2$ (two customers), and let $\bar{X}$ be the sample mean number of packages shipped. Obtain the probability distribution of $\bar{X}$ .

b. Refer to part (a) and calculate $P\left( {\bar{X} \leq {2.5}}\right)$ .

c. Again consider a random sample of size $n = 2$ , but now focus on the statistic $R =$ the sample range (difference between the largest and smallest values in the sample). Obtain the distribution of $R$ . [Hint: Calculate the value of $R$ for each outcome and use the probabilities from part (a).]

d. If a random sample of size $n = 4$ is selected, what is $P\left( {\bar{X} \leq {1.5}}\right)$ ? [Hint: You should not have to list all possible outcomes, only those for which $\bar{x} \leq {1.5}$ .]

# 42
A company maintains three offices in a certain region, each staffed by two employees. Information concerning yearly salaries (1000s of dollars) is as follows:

| Office   | 1   | 1   | 2   | 2   | 3   | 3   |
|----------|-----|-----|-----|-----|-----|-----|
| Employee | 1   | 2   | 3   | 4   | 5   | 6   |
| Salary   | 29.7 | 33.6 | 30.2 | 33.6 | 25.8 | 29.7 |

a. Suppose two of these employees are randomly selected from among the six (without replacement). Determine the sampling distribution of the sample mean salary $\bar{X}$ .

b. Suppose one of the three offices is randomly selected. Let ${X}_{1}$ and ${X}_{2}$ denote the salaries of the two employees. Determine the sampling distribution of $\bar{X}$ .

c. How does $E\left( \bar{X}\right)$ from parts (a) and (b) compare to the population mean salary $\mu$ ?

# 43
Suppose the amount of liquid dispensed by a certain machine is uniformly distributed with lower limit $A = 8\mathrm{{oz}}$ and upper limit $B = {10}$ oz. Describe how you would carry out simulation experiments to compare the sampling distribution of the (sample) fourth spread for sample sizes $n = 5,{10},{20}$ , and 30 .

# 44
Carry out a simulation experiment using a statistical computer package or other software to study the sampling distribution of $\bar{X}$ when the population distribution is Weibull with $\alpha = 2$ and $\beta = 5$ , as in Example 5.20. Consider the four sample sizes $n = 5,{10},{20}$ , and 30, and in each case use 1000 replications. For which of these sample sizes does the $\bar{X}$ sampling distribution appear to be approximately normal?

# 45
Carry out a simulation experiment using a statistical computer package or other software to study the sampling distribution of $\bar{X}$ when the population distribution is lognormal with $E\left( {\ln \left( X\right) }\right) = 3$ and $V\left( {\ln \left( X\right) }\right) = 1$ . Consider the four sample sizes $n = {10},{20},{30}$ , and 50, and in each case use 1000 replications. For which of these sample sizes does the $\bar{X}$ sampling distribution appear to be approximately normal?