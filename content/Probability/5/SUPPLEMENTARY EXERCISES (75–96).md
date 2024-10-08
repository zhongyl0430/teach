## SUPPLEMENTARY EXERCISES (75–96)

75. A restaurant serves three fixed-price dinners costing $\$ {12}$ , $\$ {15}$ , and $\$ {20}$ . For a randomly selected couple dining at this restaurant, let $X =$ the cost of the man’s dinner and $Y =$ the cost of the woman’s dinner. The joint pmf of $X$ and $Y$ is given in the following table:

<table><thead><tr><th rowspan="2">$p\left( {x, y}\right)$</th><th colspan="3">$y$</th></tr><tr><th>12</th><th>15</th><th>20</th></tr></thead><tr><td>12</td><td>.05</td><td>.05</td><td>.10</td></tr><tr><td>$x$15</td><td>.05</td><td>.10</td><td>.35</td></tr><tr><td>20</td><td>0</td><td>.20</td><td>.10</td></tr></table>

a. Compute the marginal pmf’s of $X$ and $Y$ .

b. What is the probability that the man's and the woman's dinner cost at most \$15 each?

c. Are $X$ and $Y$ independent? Justify your answer.

d. What is the expected total cost of the dinner for the two people?

e. Suppose that when a couple opens fortune cookies at the conclusion of the meal, they find the message "You will receive as a refund the difference between the cost of the more expensive and the less expensive meal that you have chosen." How much would the restaurant expect to refund?

76. In cost estimation, the total cost of a project is the sum of component task costs. Each of these costs is a random variable with a probability distribution. It is customary to obtain information about the total cost distribution by adding together characteristics of the individual component cost distributions-this is called the "roll-up" procedure. For example, $E\left( {{X}_{1} + \cdots + }\right.$ $\left. {X}_{n}\right) = E\left( {X}_{1}\right) + \cdots + E\left( {X}_{n}\right)$ , so the roll-up procedure is valid for mean cost. Suppose that there are two component tasks and that ${X}_{1}$ and ${X}_{2}$ are independent, normally distributed random variables. Is the roll-up procedure valid for the 75th percentile? That is, is the 75th percentile of the distribution of ${X}_{1} + {X}_{2}$ the same as the sum of the 75 th percentiles of the two individual distributions? If not, what is the relationship between the percentile of the sum and the sum of percentiles? For what percentiles is the roll-up procedure valid in this case?

77. A health-food store stocks two different brands of a certain type of grain. Let $X =$ the amount (lb) of brand A on hand and $Y =$ the amount of brand $\mathrm{B}$ on hand. Suppose the joint pdf of $X$ and $Y$ is

$$
f\left( {x, y}\right) = \left\{ \begin{array}{ll} {kxy} & x \geq 0, y \geq 0,{20} \leq x + y \leq {30} \\ 0 & \text{ otherwise } \end{array}\right.
$$

a. Draw the region of positive density and determine the value of $k$ .

b. Are $X$ and $Y$ independent? Answer by first deriving the marginal pdf of each variable.

c. Compute $P\left( {X + Y \leq {25}}\right)$ .

d. What is the expected total amount of this grain on hand?

e. Compute $\operatorname{Cov}\left( {X, Y}\right)$ and $\operatorname{Corr}\left( {X, Y}\right)$ .

f. What is the variance of the total amount of grain on hand?

78. According to the article "Reliability Evaluation of Hard Disk Drive Failures Based on Counting Processes" (Reliability Engr. and System Safety, 2013: 110-118), particles accumulating on a disk drive come from two sources, one external and the other internal. The article proposed a model in which the internal source contains a number of loose particles $W$ having a Poisson distribution with mean value $\mu$ ; when a loose particle releases, it immediately enters the drive, and the release times are independent and identically distributed with cumulative distribution function $G\left( t\right)$ . Let $X$ denote the number of loose particles not yet released at a particular time $t$ . Show that $X$ has a Poisson distribution with parameter $\mu \left\lbrack {1 - G\left( t\right) }\right\rbrack$ . [Hint: Let $Y$ denote the number of particles accumulated on the drive from the internal source by time $t$ so that $X + Y = W$ . Obtain an expression for $P\left( {X = x, Y = y}\right)$ and then sum over $y$ .]

79. Suppose that for a certain individual, calorie intake at breakfast is a random variable with expected value 500 and standard deviation 50 , calorie intake at lunch is random with expected value 900 and standard deviation 100 , and calorie intake at dinner is a random variable with expected value 2000 and standard deviation 180. Assuming that intakes at different meals are independent of one another, what is the probability that average calorie intake per day over the next (365- day) year is at most 3500 ? [Hint: Let ${X}_{i},{Y}_{i}$ , and ${Z}_{i}$ denote the three calorie intakes on day $i$ . Then total intake is given by $\sum \left( {{X}_{i} + {Y}_{i} + {Z}_{i}}\right)$ .]

80. The mean weight of luggage checked by a randomly selected tourist-class passenger flying between two cities on a certain airline is ${40}\mathrm{{lb}}$ , and the standard deviation is ${10}\mathrm{{lb}}$ . The mean and standard deviation for a business-class passenger are ${30}\mathrm{{lb}}$ and $6\mathrm{{lb}}$ , respectively.

a. If there are 12 business-class passengers and 50 tourist-class passengers on a particular flight, what are the expected value of total luggage weight and the standard deviation of total luggage weight?

b. If individual luggage weights are independent, normally distributed rv's, what is the probability that total luggage weight is at most ${2500}\mathrm{{lb}}$ ?

81. We have seen that if $E\left( {X}_{1}\right) = E\left( {X}_{2}\right) = \cdots = E\left( {X}_{n}\right) = \mu$ , then $E\left( {{X}_{1} + \cdots + {X}_{n}}\right) = {n\mu }$ . In some applications, the number of ${X}_{i}$ ’s under consideration is not a fixed number $n$ but instead is an rv $N$ . For example, let $N =$ the number of components that are brought into a repair shop on a particular day, and let ${X}_{i}$ denote the repair shop time for the $i$ th component. Then the total repair time is ${X}_{1} + {X}_{2} + \cdots + {X}_{N}$ , the sum of a random number of random variables. When $N$ is independent of the ${X}_{i}$ ’s, it can be shown that

$$
E\left( {{X}_{1} + \cdots + {X}_{N}}\right) = E\left( N\right) \cdot \mu
$$

a. If the expected number of components brought in on a particularly day is 10 and expected repair time for a randomly submitted component is ${40}\mathrm{\;{min}}$ , what is the expected total repair time for components submitted on any particular day?

b. Suppose components of a certain type come in for repair according to a Poisson process with a rate of 5 per hour. The expected number of defects per component is 3.5. What is the expected value of the total number of defects on components submitted for repair during a 4-hour period? Be sure to indicate how your answer follows from the general result just given.

82. Suppose the proportion of rural voters in a certain state who favor a particular gubernatorial candidate is .45 and the proportion of suburban and urban voters favoring the candidate is .60 . If a sample of 200 rural voters and 300 urban and suburban voters is obtained, what is the approximate probability that at least 250 of these voters favor this candidate?

83. Let $\mu$ denote the true $\mathrm{{pH}}$ of a chemical compound. A sequence of $n$ independent sample $\mathrm{{pH}}$ determinations will be made. Suppose each sample $\mathrm{{pH}}$ is a random variable with expected value $\mu$ and standard deviation .1 . How many determinations are required if we wish the probability that the sample average is within .02 of the true $\mathrm{{pH}}$ to be at least .95 ? What theorem justifies your probability calculation?

84. If the amount of soft drink that I consume on any given day is independent of consumption on any other day and is normally distributed with $\mu = {13}$ oz and $\sigma = 2$ and if I currently have two six-packs of 16-oz bottles, what is the probability that I still have some soft drink left at the end of 2 weeks (14 days)?

85. Refer to Exercise 58, and suppose that the ${X}_{i}$ ’s are independent with each one having a normal distribution. What is the probability that the total volume shipped is at most ${100},{000}{\mathrm{{ft}}}^{3}$ ?

86. A student has a class that is supposed to end at 9:00 A.M. and another that is supposed to begin at $9 : {10}$ A.M.

Suppose the actual ending time of the 9 A.M. class is a normally distributed rv ${X}_{1}$ with mean 9:02 and standard deviation ${1.5}\mathrm{\;{min}}$ and that the starting time of the next class is also a normally distributed rv ${X}_{2}$ with mean 9:10 and standard deviation $1\mathrm{\;{min}}$ . Suppose also that the time necessary to get from one classroom to the other is a normally distributed rv ${X}_{3}$ with mean $6\mathrm{\;{min}}$ and standard deviation $1\mathrm{\;{min}}$ . What is the probability that the student makes it to the second class before the lecture starts? (Assume independence of ${X}_{1},{X}_{2}$ , and ${X}_{3}$ , which is reasonable if the student pays no attention to the finishing time of the first class.)

87. Garbage trucks entering a particular waste-management facility are weighed prior to offloading their contents. Let $X =$ the total processing time for a randomly selected truck at this facility (waiting, weighing, and offloading). The article "Estimating Waste Transfer Station Delays Using GPS" (Waste Mgmt., 2008: 1742-1750) suggests the plausibility of a normal distribution with mean ${13}\mathrm{\;{min}}$ and standard deviation $4\mathrm{\;{min}}$ for $X$ . Assume that this is in fact the correct distribution.

a. What is the probability that a single truck's processing time is between 12 and 15 min?

b. Consider a random sample of 16 trucks. What is the probability that the sample mean processing time is between 12 and 15 min?

c. Why is the probability in (b) much larger than the probability in (a)?

d. What is the probability that the sample mean processing time for a random sample of 16 trucks will be at least 20 min?

88. Each customer making a particular Internet purchase must pay with one of three types of credit cards (think Visa, MasterCard, AmEx). Let ${A}_{i}\left( {i = 1,2,3}\right)$ be the event that a type $i$ credit card is used, with $P\left( {A}_{1}\right) = {.5}$ , $P\left( {A}_{2}\right) = {.3}$ , and $P\left( {A}_{3}\right) = {.2}$ . Suppose that the number of customers who make such a purchase on a given day is a Poisson rv with parameter $\lambda$ . Define rv’s ${X}_{1},{X}_{2},{X}_{3}$ by ${X}_{i} =$ the number among the $N$ customers who use a type $i$ card $\left( {i = 1,2,3}\right)$ . Show that these three rv’s are independent with Poisson distributions having parameters ${.5\lambda },{.3\lambda }$ , and ${.2\lambda }$ , respectively. [Hint: For non-negative integers ${x}_{1},{x}_{2},{x}_{3}$ , let $n = {x}_{1} + {x}_{2} + {x}_{3}$ . Then $P\left( {{X}_{1} = {x}_{1}}\right.$ , $\left. {{X}_{2} = {x}_{2},{X}_{3} = {x}_{3}}\right) = P\left( {{X}_{1} = {x}_{1},{X}_{2} = {x}_{2},{X}_{3} = {x}_{3}, N = n}\right)$ [why is this?]. Now condition on $N = n$ , in which case the three ${Xi}$ ’s have a trinomial distribution (multinomial with three categories) with category probabilities .5, .3, and .2.]

89. a. Use the general formula for the variance of a linear combination to write an expression for $V\left( {{aX} + Y}\right)$ . Then let $a = {\sigma }_{Y}/{\sigma }_{X}$ , and show that $\rho \geq - 1$ . [Hint: Variance is always $\geq 0$ , and $\operatorname{Cov}\left( {X, Y}\right) = {\sigma }_{X} \cdot {\sigma }_{Y} \cdot \rho$ .]

b. By considering $V\left( {{aX} - Y}\right)$ , conclude that $\rho \leq 1$ .

c. Use the fact that $V\left( W\right) = 0$ only if $W$ is a constant to show that $\rho = 1$ only if $Y = {aX} + b$ .

90. Suppose a randomly chosen individual’s verbal score $X$ and quantitative score $Y$ on a nationally administered aptitude examination have a joint pdf

$$
f\left( {x, y}\right) = \left\{ \begin{matrix} \frac{2}{5}\left( {{2x} + {3y}}\right) & 0 \leq x \leq 1,0 \leq y \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

You are asked to provide a prediction $t$ of the individual’s total score $X + Y$ . The error of prediction is the mean squared error $E\left\lbrack {\left( X + Y - t\right) }^{2}\right\rbrack$ . What value of $t$ minimizes the error of prediction?

91. a. Let ${X}_{1}$ have a chi-squared distribution with parameter ${\nu }_{1}$ (see Section 4.4), and let ${X}_{2}$ be independent of ${X}_{1}$ and have a chi-squared distribution with parameter ${\nu }_{2}$ . Use the technique of Example 5.22 to show that ${X}_{1} + {X}_{2}$ has a chi-squared distribution with parameter ${\nu }_{1} + {\nu }_{2}$ .

b. In Exercise 71 of Chapter 4, you were asked to show that if $Z$ is a standard normal rv, then ${Z}^{2}$ has a chi-squared distribution with $\nu = 1$ . Let ${Z}_{1},{Z}_{2},\ldots ,{Z}_{n}$ be $n$ independent standard normal rv’s. What is the distribution of ${Z}_{1}^{2} + \cdots + {Z}_{n}^{2}$ ? Justify your answer.

c. Let ${X}_{1},\ldots ,{X}_{n}$ be a random sample from a normal distribution with mean $\mu$ and variance ${\sigma }^{2}$ . What is the distribution of the sum $Y = \mathop{\sum }\limits_{{i = 1}}^{n}{\left\lbrack \left( {X}_{i} - \mu \right) /\sigma \right\rbrack }^{2}$ ? Justify your answer.

92. a. Show that $\operatorname{Cov}\left( {X, Y + Z}\right) = \operatorname{Cov}\left( {X, Y}\right) + \operatorname{Cov}\left( {X, Z}\right)$ .

b. Let ${X}_{1}$ and ${X}_{2}$ be quantitative and verbal scores on one aptitude exam, and let ${Y}_{1}$ and ${Y}_{2}$ be corresponding scores on another exam. If $\operatorname{Cov}\left( {{X}_{1},{Y}_{1}}\right) = 5$ , $\operatorname{Cov}\left( {{X}_{1},{Y}_{2}}\right) = 1,\operatorname{Cov}\left( {{X}_{2},{Y}_{1}}\right) = 2$ , and $\operatorname{Cov}\left( {{X}_{2},{Y}_{2}}\right) =$ 8 , what is the covariance between the two total scores ${X}_{1} + {X}_{2}$ and ${Y}_{1} + {Y}_{2}$ ?

93. A rock specimen from a particular area is randomly selected and weighed two different times. Let $W$ denote the actual weight and ${X}_{1}$ and ${X}_{2}$ the two measured weights. Then ${X}_{1} = W + {E}_{1}$ and ${X}_{2} = W + {E}_{2}$ , where ${E}_{1}$ and ${E}_{2}$ are the two measurement errors. Suppose that the ${E}_{i}$ ’s are independent of one another and of $W$ and that $V\left( {E}_{1}\right) = V\left( {E}_{2}\right) = {\sigma }_{E}^{2}$ .

a. Express $\rho$ , the correlation coefficient between the two measured weights ${X}_{1}$ and ${X}_{2}$ , in terms of ${\sigma }_{W}^{2}$ , the variance of actual weight, and ${\sigma }_{X}^{2}$ , the variance of measured weight.

b. Compute $\rho$ when ${\sigma }_{W} = 1\mathrm{\;{kg}}$ and ${\sigma }_{E} = {.01}\mathrm{\;{kg}}$ .

94. Let $A$ denote the percentage of one constituent in a randomly selected rock specimen, and let $B$ denote the percentage of a second constituent in that same specimen. Suppose $D$ and $E$ are measurement errors in determining the values of $A$ and $B$ so that measured values are $X = A + D$ and $Y = B + E$ , respectively. Assume that measurement errors are independent of one another and of actual values.

a. Show that

$\operatorname{Corr}\left( {X, Y}\right) = \operatorname{Corr}\left( {A, B}\right) \cdot \sqrt{\operatorname{Corr}\left( {{X}_{1},{X}_{2}}\right) } \cdot \sqrt{\operatorname{Corr}\left( {{Y}_{1},{Y}_{2}}\right) }$ ${\sigma }_{4} = {4.0}\mathrm{\;V}$ . Calculate the approximate expected value and standard deviation of the current (suggested by "Random Samplings," CHEMTECH, 1984: 696-697).

96. A more accurate approximation to $E\left\lbrack {h\left( {{X}_{1},\ldots ,{X}_{n}}\right) }\right\rbrack$ in Exercise 95 is

$$
h\left( {{\mu }_{1},\ldots ,{\mu }_{n}}\right) + \frac{1}{2}{\sigma }_{1}^{2}\left( \frac{{\partial }^{2}h}{\partial {x}_{1}^{2}}\right) + \cdots + \frac{1}{2}{\sigma }_{n}^{2}\left( \frac{{\partial }^{2}h}{\partial {x}_{n}^{2}}\right)
$$

Compute this for $Y = h\left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4}}\right)$ given in Exercise 93, and compare it to the leading term $h\left( {{\mu }_{1},\ldots ,{\mu }_{n}}\right)$ .

97. Let $X$ and $Y$ be independent standard normal random variables, and define a new rv by $U = {.6X} + {.8Y}$ .

a. Determine $\operatorname{Corr}\left( {X, U}\right)$ .

b. How would you alter $U$ to obtain $\operatorname{Corr}\left( {X, U}\right) = \rho$ for a specified value of $\rho$ ?

98. Let ${X}_{1},{X}_{2},\ldots ,{X}_{n}$ be random variables denoting $n$ independent bids for an item that is for sale. Suppose each ${X}_{i}$ is uniformly distributed on the interval $\left\lbrack {{100},{200}}\right\rbrack$ . If the seller sells to the highest bidder, how much can he expect to earn on the sale? [Hint: Let $Y = \max \left( {{X}_{1},{X}_{2},\ldots ,{X}_{n}}\right)$ . First find ${F}_{Y}\left( y\right)$ by noting that $Y \leq y$ iff each ${X}_{i}$ is $\leq y$ . Then obtain the pdf and $E\left( Y\right)$ .] where ${X}_{1}$ and ${X}_{2}$ are replicate measurements on the value of $A$ , and ${Y}_{1}$ and ${Y}_{2}$ are defined analogously with respect to $B$ . What effect does the presence of measurement error have on the correlation?

b. What is the maximum value of $\operatorname{Corr}\left( {X, Y}\right)$ when $\operatorname{Corr}\left( {{X}_{1},{X}_{2}}\right) = {.8100}$ and $\operatorname{Corr}\left( {{Y}_{1},{Y}_{2}}\right) = {.9025}$ ? Is this disturbing?

95. Let ${X}_{1},\ldots ,{X}_{n}$ be independent rv’s with mean values ${\mu }_{1},\ldots ,{\mu }_{n}$ and variances ${\sigma }_{1}^{2},\ldots ,{\sigma }_{n}^{2}$ . Consider a function $h\left( {{x}_{1},\ldots ,{x}_{n}}\right)$ , and use it to define a rv $Y = h\left( {{X}_{1},\ldots ,{X}_{n}}\right)$ . Under rather general conditions on the $h$ function, if the ${\sigma }_{i}$ ’s are all small relative to the corresponding ${\mu }_{i}$ ’s, it can be shown that $E\left( Y\right) \approx h\left( {{\mu }_{1},\ldots ,{\mu }_{n}}\right)$ and

$$
V\left( Y\right) \approx {\left( \frac{\partial h}{\partial {x}_{1}}\right) }^{2} \cdot {\sigma }_{1}^{2} + \cdots + {\left( \frac{\partial h}{\partial {x}_{n}}\right) }^{2} \cdot {\sigma }_{n}^{2}
$$

where each partial derivative is evaluated at $\left( {{x}_{1},\ldots ,{x}_{n}}\right) =$ $\left( {{\mu }_{1},\ldots ,{\mu }_{n}}\right)$ . Suppose three resistors with resistances ${X}_{1},{X}_{2}$ , ${X}_{3}$ are connected in parallel across a battery with voltage ${X}_{4}$ . Then by Ohm's law, the current is

$$
Y = {X}_{4}\left\lbrack {\frac{1}{{X}_{1}} + \frac{1}{{X}_{2}} + \frac{1}{{X}_{3}}}\right\rbrack
$$

Let ${\mu }_{1} = {10}$ ohms, ${\sigma }_{1} = {1.0}\mathrm{{ohm}},\;{\mu }_{2} = {15}$ ohms, ${\sigma }_{2} = {1.0}\mathrm{{ohm}},{\mu }_{3} = {20}\mathrm{{ohms}},{\sigma }_{3} = {1.5}\mathrm{{ohms}},{\mu }_{4} = {120}\mathrm{\;V}$ ,