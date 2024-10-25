# 59
Let $X =$ the time between two successive arrivals at the drive-up window of a local bank. If $X$ has an exponential distribution with $\lambda = 1$ (which is identical to a standard gamma distribution with $\alpha = 1$ ), compute the following:

a. The expected time between two successive arrivals

b. The standard deviation of the time between successive arrivals

c. $P\left( {X \leq 4}\right)$ d. $P\left( {2 \leq X \leq 5}\right)$
# 60
Let $X$ denote the distance (m) that an animal moves from its birth site to the first territorial vacancy it encounters. Suppose that for banner-tailed kangaroo rats, $X$ has an exponential distribution with parameter $\lambda = {.01386}$ (as suggested in the article "Competition and Dispersal from Multiple Nests," Ecology, 1997: 873-883).

a. What is the probability that the distance is at most ${100}\mathrm{\;m}$ ? At most ${200}\mathrm{\;m}$ ? Between 100 and ${200}\mathrm{\;m}$ ?

b. What is the probability that distance exceeds the mean distance by more than 2 standard deviations?

c. What is the value of the median distance?
# 61
Data collected at Toronto Pearson International Airport suggests that an exponential distribution with mean value 2.725 hours is a good model for rainfall duration (Urban Stormwater Management Planning with Analytical Probabilistic Models, 2000, p. 69).

a. What is the probability that the duration of a particular rainfall event at this location is at least 2 hours? At most 3 hours? Between 2 and 3 hours?

b. What is the probability that rainfall duration exceeds the mean value by more than 2 standard deviations? What is the probability that it is less than the mean value by more than one standard deviation?
# 62
The article "Microwave Observations of Daily Antarctic Sea-Ice Edge Expansion and Contribution Rates" (IEEE Geosci. and Remote Sensing Letters, 2006: 54-58) states that "The distribution of the daily sea-ice advance/retreat from each sensor is similar and is approximately double exponential." The proposed double exponential distribution has density function $f\left( x\right) = {.5\lambda }{e}^{-\lambda \left| x\right| }$ for $- \infty < x < \infty$ . The standard deviation is given as ${40.9}\mathrm{\;{km}}$ .

a. What is the value of the parameter $\lambda$ ?

b. What is the probability that the extent of daily sea-ice change is within 1 standard deviation of the mean value?
# 63
A consumer is trying to decide between two long-distance calling plans. The first one charges a flat rate of ${10}¢$ per minute, whereas the second charges a flat rate of ${99}¢$ for calls up to 20 minutes in duration and then ${10}¢$ for each additional minute exceeding 20 (assume that calls lasting a noninteger number of minutes are charged proportionately to a whole-minute's charge). Suppose the consumer's distribution of call duration is exponential with parameter $\lambda$ .

a. Explain intuitively how the choice of calling plan should depend on what the expected call duration is.

b. Which plan is better if expected call duration is 10 minutes? 15 minutes? 
- Hint: Let ${h}_{1}\left( x\right)$ denote the cost for the first plan when call duration is $x$ minutes and let ${h}_{2}\left( x\right)$ be the cost function for the second plan. Give expressions for these two cost functions, and then determine the expected cost for each plan.
# 64
Evaluate the following:

a. $\Gamma \left( 6\right) \;$ b. $\Gamma \left( {5/2}\right)$

c. $F\left( {4;5}\right)$ (the incomplete gamma function) and $F\left( {5;4}\right)$

d. $P\left( {X \leq 5}\right)$ when $X$ has a standard gamma distribution with $\alpha = 7$ .

e. $P\left( {3 < X < 8}\right)$ when $X$ has the distribution specified in (d).
# 65
Let $X$ denote the data transfer time (ms) in a grid computing system (the time required for data transfer between a "worker" computer and a "master" computer. Suppose that $X$ has a gamma distribution with mean value ${37.5}\mathrm{\;{ms}}$ and standard deviation 21.6 (suggested by the article "Computation Time of Grid Computing with Data Transfer Times that Follow a Gamma Distribution," Proceedings of the First International Conference on Semantics, Knowledge, and Grid, 2005).

a. What are the values of $\alpha$ and $\beta$ ?

b. What is the probability that data transfer time exceeds ${50}\mathrm{\;{ms}}$ ?

c. What is the probability that data transfer time is between 50 and ${75}\mathrm{\;{ms}}$ ?
# 66
The two-parameter gamma distribution can be generalized by introducing a third parameter $\gamma$ , called a threshold or location parameter: replace $x$ in (4.8) by $x - \gamma$ and $x \geq 0$ by $x \geq \gamma$ . This amounts to shifting the density curves in Figure 4.27 so that they begin their ascent or descent at $\gamma$ rather than 0 . The article "Bivariate Flood Frequency Analysis with Historical Information Based on Copulas" (J. of Hydrologic Engr., 2013: 1018-1030) employs this distribution to model $X =$ 3-day flood volume $\left( {{10}^{8}{\mathrm{\;m}}^{3}}\right)$ . Suppose that values of the parameters are $\alpha = {12},\beta = 7,\gamma = {40}$ (very close to estimates in the cited article based on past data).

a. What are the mean value and standard deviation of $X$ ?

b. What is the probability that flood volume is between 100 and 150 ?

c. What is the probability that flood volume exceeds its mean value by more than one standard deviation?

d. What is the 95th percentile of the flood volume distribution?
# 67
Suppose that when a transistor of a certain type is subjected to an accelerated life test, the lifetime $X$ (in weeks) has a gamma distribution with mean 24 weeks and standard deviation 12 weeks.

a. What is the probability that a transistor will last between 12 and 24 weeks?

b. What is the probability that a transistor will last at most 24 weeks? Is the median of the lifetime distribution less than 24 ? Why or why not?

c. What is the 99th percentile of the lifetime distribution?

d. Suppose the test will actually be terminated after $t$ weeks. What value of $t$ is such that only ${.5}\%$ of all transistors would still be operating at termination?
# 68
The special case of the gamma distribution in which $\alpha$ is a positive integer $n$ is called an Erlang distribution. If we replace $\beta$ by $1/\lambda$ in Expression (4.8), the Erlang pdf is

$$
f\left( {x;\lambda , n}\right) = \left\{ \begin{matrix} \frac{\lambda {\left( \lambda x\right) }^{n - 1}{e}^{-{\lambda x}}}{\left( {n - 1}\right) !} & x \geq 0 \\ 0 & x < 0 \end{matrix}\right.
$$

It can be shown that if the times between successive events are independent, each with an exponential distribution with parameter $\lambda$ , then the total time $X$ that elapses before all of the next $n$ events occur has pdf $f\left( {x;\lambda , n}\right)$ .

a. What is the expected value of $X$ ? If the time (in minutes) between arrivals of successive customers is exponentially distributed with $\lambda = {.5}$ , how much time can be expected to elapse before the tenth customer arrives?

b. If customer interarrival time is exponentially distributed with $\lambda = {.5}$ , what is the probability that the tenth customer (after the one who has just arrived) will arrive within the next ${30}\mathrm{\;{min}}$ ?

c. The event $\{ X \leq t\}$ occurs iff at least $n$ events occur in the next $t$ units of time. Use the fact that the number of events occurring in an interval of length $t$ has a Poisson distribution with parameter ${\lambda t}$ to write an expression (involving Poisson probabilities) for the Erlang $\operatorname{cdf}F\left( {t;\lambda , n}\right) = P\left( {X \leq t}\right)$ .
# 69
A system consists of five identical components connected in series as shown:

![01925166-48c0-7eca-9860-67f13d0848b1_35_955_922_665_53_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_35_955_922_665_53_0.jpg)

As soon as one component fails, the entire system will fail. Suppose each component has a lifetime that is exponentially distributed with $\lambda = {.01}$ and that components fail independently of one another. Define events ${A}_{i} =$ \{ $i$ th component lasts at least $t$ hours\}, $i = 1,\ldots ,5$ , so that the ${A}_{i}\mathrm{\;s}$ are independent events. Let $X =$ the time at which the system fails-that is, the shortest (minimum) lifetime among the five components.

a. The event $\{ X \geq t\}$ is equivalent to what event involving ${A}_{1},\ldots ,{A}_{5}$ ?

b. Using the independence of the ${A}_{i}{}^{\prime }\mathrm{s}$ , compute $P\left( {X \geq t}\right)$ . Then obtain $F\left( t\right) = P\left( {X \leq t}\right)$ and the pdf of $X$ . What type of distribution does $X$ have?

c. Suppose there are $n$ components, each having exponential lifetime with parameter $\lambda$ . What type of distribution does $X$ have?
# 70
If $X$ has an exponential distribution with parameter $\lambda$ , derive a general expression for the $\left( {100p}\right)$ th percentile of the distribution. Then specialize to obtain the median.
# 71
a. The event $\left\{ {{X}^{2} \leq y}\right\}$ is equivalent to what event involving $X$ itself?

b. If $X$ has a standard normal distribution, use part (a) to write the integral that equals $P\left( {{X}^{2} \leq y}\right)$ . Then differentiate this with respect to $y$ to obtain the pdf of ${X}^{2}$ [the square of a $N\left( {0,1}\right)$ variable]. Finally, show that ${X}^{2}$ has a chi-squared distribution with $\nu = 1\mathrm{{df}}$ [see (4.10)]. [Hint: Use the following identity.]

$$
\frac{d}{dy}\left\{ {{\int }_{a\left( y\right) }^{b\left( y\right) }f\left( x\right) {dx}}\right\} = f\left\lbrack {b\left( y\right) }\right\rbrack \cdot {b}^{\prime }\left( y\right) - f\left\lbrack {a\left( y\right) }\right\rbrack \cdot {a}^{\prime }\left( y\right)
$$