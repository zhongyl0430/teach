## EXERCISES Section 4.2 (11-27)

11. Let $X$ denote the amount of time a book on two-hour reserve is actually checked out, and suppose the cdf is

$$
F\left( x\right) = \left\{ \begin{array}{ll} 0 & x < 0 \\ \frac{{x}^{2}}{4} & 0 \leq x < 2 \\ 1 & 2 \leq x \end{array}\right.
$$

a. Calculate $P\left( {X \leq 1}\right)$ .

b. Calculate $P\left( {{.5} \leq X \leq 1}\right)$ .

c. Calculate $P\left( {X > {1.5}}\right)$ .

d. What is the median checkout duration $\widetilde{\mu }$ ? [solve ${.5} = F\left( \widetilde{\mu }\right) \rbrack$ .

e. Obtain the density function $f\left( x\right)$ .

f. Calculate $E\left( X\right)$ .

g. Calculate $V\left( X\right)$ and ${\sigma }_{X}$ .

h. If the borrower is charged an amount $h\left( X\right) = {X}^{2}$ when checkout duration is $X$ , compute the expected charge $E\left\lbrack {h\left( X\right) }\right\rbrack$ .

12. The cdf for $X$ (= measurement error) of Exercise 3 is

$$
F\left( x\right) = \left\{ \begin{matrix} 0 & x < - 2 \\ \frac{1}{2} + \frac{3}{32}\left( {{4x} - \frac{{x}^{3}}{3}}\right) & - 2 \leq x < 2 \\ 1 & 2 \leq x \end{matrix}\right.
$$

a. Compute $P\left( {X < 0}\right)$ .

b. Compute $P\left( {-1 < X < 1}\right)$ .

c. Compute $P\left( {{.5} < X}\right)$ .

d. Verify that $f\left( x\right)$ is as given in Exercise 3 by obtaining ${F}^{\prime }\left( x\right)$ .

e. Verify that $\widetilde{\mu } = 0$ .

13. Example 4.5 introduced the concept of time headway in traffic flow and proposed a particular distribution for $X =$ the headway between two randomly selected consecutive cars (sec). Suppose that in a different traffic environment, the distribution of time headway has the form

$$
f\left( x\right) = \left\{ \begin{array}{ll} \frac{k}{{x}^{4}} & x > 1 \\ 0 & x \leq 1 \end{array}\right.
$$

a. Determine the value of $k$ for which $f\left( x\right)$ is a legitimate pdf.

b. Obtain the cumulative distribution function.

c. Use the cdf from (b) to determine the probability that headway exceeds 2 sec and also the probability that headway is between 2 and 3 sec.

d. Obtain the mean value of headway and the standard deviation of headway.

e. What is the probability that headway is within 1 standard deviation of the mean value?

14. The article "Modeling Sediment and Water Column Interactions for Hydrophobic Pollutants" (Water Research, 1984: 1169-1174) suggests the uniform distribution on the interval $\left( {{7.5},{20}}\right)$ as a model for depth $\left( \mathrm{{cm}}\right)$ of the bioturbation layer in sediment in a certain region.

a. What are the mean and variance of depth?

b. What is the cdf of depth?

c. What is the probability that observed depth is at most 10? Between 10 and 15 ?

d. What is the probability that the observed depth is within 1 standard deviation of the mean value? Within 2 standard deviations?

15. Let $X$ denote the amount of space occupied by an article placed in a $1 - {\mathrm{{ft}}}^{3}$ packing container. The pdf of $X$ is

$$
f\left( x\right) = \left\{ \begin{matrix} {90}{x}^{8}\left( {1 - x}\right) & 0 < x < 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

a. Graph the pdf. Then obtain the cdf of $X$ and graph it.

b. What is $P\left( {X \leq {.5}}\right)$ [i.e., $F\left( {.5}\right)$ ]?

c. Using the cdf from (a), what is $P\left( {{.25} < X \leq {.5}}\right)$ ? What is $P\left( {{.25} \leq X \leq {.5}}\right)$ ?

d. What is the 75th percentile of the distribution?

e. Compute $E\left( X\right)$ and ${\sigma }_{X}$ .

f. What is the probability that $X$ is more than 1 standard deviation from its mean value?

16. The article "A Model of Pedestrians" Waiting Times for Street Crossings at Signalized Intersections" (Transportation Research, 2013: 17-28) suggested that under some circumstances the distribution of waiting time $X$ could be modeled with the following pdf:

$$
f\left( {x;\theta ,\tau }\right) = \left\{ \begin{matrix} \frac{\theta }{\tau }{\left( 1 - x/\tau \right) }^{\theta - 1} & 0 \leq x < \tau \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

a. Graph $f\left( {x;\theta ,{80}}\right)$ for the three cases $\theta = 4,1$ , and .5 (these graphs appear in the cited article) and comment on their shapes.

b. Obtain the cumulative distribution function of $X$ .

c. Obtain an expression for the median of the waiting time distribution.

d. For the case $\theta = 4,\tau = {80}$ , calculate $P\left( {{50} \leq X \leq {70}}\right)$ without at this point doing any additional integration.

17. Let $X$ have a uniform distribution on the interval $\left\lbrack {A, B}\right\rbrack$ .

a. Obtain an expression for the $\left( {100p}\right)$ th percentile.

b. Compute $E\left( X\right) , V\left( X\right)$ , and ${\sigma }_{X}$ .

c. For $n$ , a positive integer, compute $E\left( {X}^{n}\right)$ .

18. Let $X$ denote the voltage at the output of a microphone, and suppose that $X$ has a uniform distribution on the interval from -1 to 1 . The voltage is processed by a "hard limiter" with cutoff values -.5 and .5 , so the limiter output is a random variable $Y$ related to $X$ by $Y = X$ if $\left| X\right| \leq {.5}, Y = {.5}$ if $X > {.5}$ , and $Y = - {.5}$ if $X < - {.5}$ .

a. What is $P\left( {Y = {.5}}\right)$ ?

b. Obtain the cumulative distribution function of $Y$ and graph it.

19. Let $X$ be a continuous rv with cdf

$$
F\left( x\right) = \left\{ \begin{matrix} 0 & x \leq 0 \\ \frac{x}{4}\left\lbrack {1 + \ln \left( \frac{4}{x}\right) }\right\rbrack & 0 < x \leq 4 \\ 1 & x > 4 \end{matrix}\right.
$$

[This type of cdf is suggested in the article "Variability in Measured Bedload-Transport Rates" (Water Resources Bull., 1985: 39-48) as a model for a certain hydrologic variable.] What is

a. $P\left( {X \leq 1}\right)$ ?

b. $P\left( {1 \leq X \leq 3}\right)$ ?

c. The pdf of $X$ ?

20. Consider the pdf for total waiting time $Y$ for two buses

$$
f\left( y\right) = \left\{ \begin{matrix} \frac{1}{25}y & 0 \leq y < 5 \\ \frac{2}{5} - \frac{1}{25}y & 5 \leq y \leq {10} \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

introduced in Exercise 8.

a. Compute and sketch the cdf of $Y$ . [Hint: Consider separately $0 \leq y < 5$ and $5 \leq y \leq {10}$ in computing $F\left( y\right)$ . A graph of the pdf should be helpful.]

b. Obtain an expression for the $\left( {100p}\right)$ th percentile. [Hint: Consider separately $0 < p < {.5}$ and ${.5} < p < 1$ .]

c. Compute $E\left( Y\right)$ and $V\left( Y\right)$ . How do these compare with the expected waiting time and variance for a single bus when the time is uniformly distributed on $\left\lbrack {0,5}\right\rbrack$ ?

21. An ecologist wishes to mark off a circular sampling region having radius ${10}\mathrm{\;m}$ . However, the radius of the resulting region is actually a random variable $R$ with pdf

$$
f\left( r\right) = \left\{ \begin{matrix} \frac{3}{4}\left\lbrack {1 - {\left( {10} - r\right) }^{2}}\right\rbrack & 9 \leq r \leq {11} \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

What is the expected area of the resulting circular region?

22. The weekly demand for propane gas (in 1000s of gallons) from a particular facility is an rv $X$ with pdf

$$
f\left( x\right) = \left\{ \begin{matrix} 2\left( {1 - \frac{1}{{x}^{2}}}\right) & 1 \leq x \leq 2 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

a. Compute the cdf of $X$ .

b. Obtain an expression for the $\left( {100p}\right)$ th percentile. What is the value of $\widetilde{\mu }$ ?

c. Compute $E\left( X\right)$ and $V\left( X\right)$ .

d. If 1.5 thousand gallons are in stock at the beginning of the week and no new supply is due in during the week, how much of the 1.5 thousand gallons is expected to be left at the end of the week? [Hint: Let $h\left( x\right) =$ amount left when demand $= x$ .]

23. If the temperature at which a certain compound melts is a random variable with mean value ${120}^{ \circ }\mathrm{C}$ and standard deviation ${2}^{ \circ }\mathrm{C}$ , what are the mean temperature and standard deviation measured in ${}^{ \circ }\mathrm{F}$ ? [Hint: ${}^{ \circ }\mathrm{F} = {1.8}^{ \circ }\mathrm{C} + {32}$ .]

24. Let $X$ have the Pareto pdf

$$
f\left( {x;k,\theta }\right) = \left\{ \begin{matrix} \frac{k \cdot {\theta }^{k}}{{x}^{k + 1}} & x \geq \theta \\ 0 & x < \theta \end{matrix}\right.
$$

introduced in Exercise 10.

a. If $k > 1$ , compute $E\left( X\right)$ .

b. What can you say about $E\left( X\right)$ if $k = 1$ ?

c. If $k > 2$ , show that $V\left( X\right) = k{\theta }^{2}{\left( k - 1\right) }^{-2}{\left( k - 2\right) }^{-1}$ .

d. If $k = 2$ , what can you say about $V\left( X\right)$ ?

e. What conditions on $k$ are necessary to ensure that $E\left( {X}^{n}\right)$ is finite?


25. Let $X$ be the temperature in ${}^{ \circ }\mathrm{C}$ at which a certain chemical reaction takes place, and let $Y$ be the temperature in

${}^{ \circ }\mathrm{F}$ (so $Y = {1.8X} + {32}$ ).

a. If the median of the $X$ distribution is $\widetilde{\mu }$ , show that ${1.8}\widetilde{\mu } + {32}$ is the median of the $Y$ distribution.

b. How is the 90th percentile of the $Y$ distribution related to the 90th percentile of the $X$ distribution? Verify your conjecture.

c. More generally, if $Y = {aX} + b$ , how is any particular percentile of the $Y$ distribution related to the corresponding percentile of the $X$ distribution?

26. Let $X$ be the total medical expenses (in 1000 s of dollars) incurred by a particular individual during a given year. Although $X$ is a discrete random variable, suppose its distribution is quite well approximated by a continuous distribution with pdf $f\left( x\right) = k{\left( 1 + x/{2.5}\right) }^{-7}$ for $x \geq 0$ .

a. What is the value of $k$ ?

b. Graph the pdf of $X$ .

c. What are the expected value and standard deviation of total medical expenses?

d. This individual is covered by an insurance plan that entails a \$500 deductible provision (so the first \$500 worth of expenses are paid by the individual). Then the plan will pay ${80}\%$ of any additional expenses exceeding $\$ {500}$ , and the maximum payment by the individual (including the deductible amount) is \$2500. Let $Y$ denote the amount of this individual’s medical expenses paid by the insurance company. What is the expected value of $Y$ ?

[Hint: First figure out what value of $X$ corresponds to the maximum out-of-pocket expense of \$2500. Then write an expression for $Y$ as a function of $X$ (which involves several different pieces) and calculate the expected value of this function.]

27. When a dart is thrown at a circular target, consider the location of the landing point relative to the bull’s eye. Let $X$ be the angle in degrees measured from the horizontal, and assume that $X$ is uniformly distributed on $\left\lbrack {0,{360}}\right\rbrack$ . Define $Y$ to be the transformed variable $Y = h\left( X\right) =$ $\left( {{2\pi }/{360}}\right) X - \pi$ , so $Y$ is the angle measured in radians and $Y$ is between $- \pi$ and $\pi$ . Obtain $E\left( Y\right)$ and ${\sigma }_{Y}$ by first obtaining $E\left( X\right)$ and ${\sigma }_{X}$ , and then using the fact that $h\left( X\right)$ is a linear function of $X$ .