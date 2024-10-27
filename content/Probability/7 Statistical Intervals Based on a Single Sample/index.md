---
title: 7 Statistical Intervals Based on a Single Sample
---
## INTRODUCTION

A point estimate, because it is a single number, by itself provides no information about the precision and reliability of estimation. Consider, for example, using the statistic $\bar{X}$ to calculate a point estimate for the true average breaking strength (g) of paper towels of a certain brand, and suppose that $\bar{x} = {9322.7}$ . Because of sampling variability, it is virtually never the case that $\bar{x} = \mu$ . The point estimate says nothing about how close it might be to $\mu$ . An alternative to reporting a single sensible value for the parameter being estimated is to calculate and report an entire interval of plausible values—an interval estimate or confidence interval (CI). A confidence interval is always calculated by first selecting a confidence level, which is a measure of the degree of reliability of the interval. A confidence interval with a ${95}\%$ confidence level for the true average breaking strength might have a lower limit of 9162.5 and an upper limit of 9482.9. Then at the 95% confidence level, any value of $\mu$ between 9162.5 and 9482.9 is plausible. A confidence level of ${95}\%$ implies that ${95}\%$ of all samples would give an interval that includes $\mu$ , or whatever other parameter is being estimated, and only $5\%$ of all samples would yield an erroneous interval. The most frequently used confidence levels are ${95}\% ,{99}\%$ , and ${90}\%$ . The higher the confidence level, the more strongly we believe that the value of the parameter being estimated lies within the interval (an interpretation of any particular confidence level will be given shortly).

Information about the precision of an interval estimate is conveyed by the width of the interval. If the confidence level is high and the resulting interval is quite narrow, our knowledge of the value of the parameter is reasonably precise. A very wide confidence interval, however, gives the message that there is a great deal of uncertainty concerning the value of what we are estimating. Figure 7.1 shows ${95}\%$ confidence intervals for true average breaking strengths of two different brands of paper towels. One of these intervals suggests precise knowledge about $\mu$ , whereas the other suggests a very wide range of plausible values.

![01927a02-a1da-7086-ba87-2208e017bc0f_1_851_489_698_116_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_1_851_489_698_116_0.jpg)

Figure 7.1 CIs indicating precise (brand 1) and imprecise (brand 2) information about $\mu$

## 7.1 Basic Properties of Confidence Intervals

The basic concepts and properties of confidence intervals (CIs) are most easily introduced by first focusing on a simple, albeit somewhat unrealistic, problem situation. Suppose that the parameter of interest is a population mean $\mu$ and that

1. The population distribution is normal

2. The value of the population standard deviation $\sigma$ is known

Normality of the population distribution is often a reasonable assumption. However, if the value of $\mu$ is unknown, it is typically implausible that the value of $\sigma$ would be available (knowledge of a population's center typically precedes information concerning spread). We'll develop methods based on less restrictive assumptions in Sections 7.2 and 7.3.

EXAMPLE 7.1 Industrial engineers who specialize in ergonomics are concerned with designing workspace and worker-operated devices so as to achieve high productivity and comfort. The article "Studies on Ergonomically Designed Alphanumeric Keyboards" (Human Factors, 1985: 175-187) reports on a study of preferred height for an experimental keyboard with large forearm-wrist support. A sample of $n = {31}$ trained typists was selected, and the preferred keyboard height was determined for each typist. The resulting sample average preferred height was $\bar{x} = {80.0}\mathrm{\;{cm}}$ . Assuming that the preferred height is normally distributed with $\sigma = {2.0}\mathrm{\;{cm}}$ (a value suggested by data in the article), obtain a confidence interval (interval of plausible values) for $\mu$ , the true average preferred height for the population of all experienced typists.

The actual sample observations ${x}_{1},{x}_{2},\ldots ,{x}_{n}$ are assumed to be the result of a random sample ${X}_{1},\ldots ,{X}_{n}$ from a normal distribution with mean value $\mu$ and standard deviation $\sigma$ . The results described in Chapter 5 then imply that, irrespective of the sample size $n$ , the sample mean $\bar{X}$ is normally distributed with expected value $\mu$ and standard deviation $\sigma /\sqrt{n}$ . Standardizing $\bar{X}$ by first subtracting its expected value and then dividing by its standard deviation yields the standard normal variable

$$
Z = \frac{\bar{X} - \mu }{\sigma /\sqrt{n}} \tag{7.1}
$$

Because the area under the standard normal curve between -1.96 and 1.96 is .95 ,

$$
P\left( {-{1.96} < \frac{\bar{X} - \mu }{\sigma /\sqrt{n}} < {1.96}}\right) = {.95} \tag{7.2}
$$

Now let's manipulate the inequalities inside the parentheses in (7.2) so that they appear in the equivalent form $l < \mu < u$ , where the endpoints $l$ and $u$ involve $\bar{X}$ and $\sigma /\sqrt{n}$ . This is achieved through the following sequence of operations, each yielding inequalities equivalent to the original ones.

1. Multiply through by $\sigma /\sqrt{n}$ :

$$
- {1.96} \cdot \frac{\sigma }{\sqrt{n}} < \bar{X} - \mu < {1.96} \cdot \frac{\sigma }{\sqrt{n}}
$$

2. Subtract $\bar{X}$ from each term:

$$
- \bar{X} - {1.96} \cdot \frac{\sigma }{\sqrt{n}} < - \mu < - \bar{X} + {1.96} \cdot \frac{\sigma }{\sqrt{n}}
$$

3. Multiply through by -1 to eliminate the minus sign in front of $\mu$ (which reverses the direction of each inequality):

$$
\bar{X} + {1.96} \cdot \frac{\sigma }{\sqrt{n}} > \mu > \bar{X} - {1.96} \cdot \frac{\sigma }{\sqrt{n}}
$$

that is,

$$
\bar{X} - {1.96} \cdot \frac{\sigma }{\sqrt{n}} < \mu < \bar{X} + {1.96} \cdot \frac{\sigma }{\sqrt{n}}
$$

The equivalence of each set of inequalities to the original set implies that

$$
P\left( {\bar{X} - {1.96}\frac{\sigma }{\sqrt{n}} < \mu < \bar{X} + {1.96}\frac{\sigma }{\sqrt{n}}}\right) = {.95} \tag{7.3}
$$

The event inside the parentheses in (7.3) has a somewhat unfamiliar appearance; previously, the random quantity has appeared in the middle with constants on both ends, as in $a \leq Y \leq b$ . In (7.3) the random quantity appears on the two ends, whereas the unknown constant $\mu$ appears in the middle. To interpret (7.3), think of a random interval having left endpoint $\bar{X} - {1.96} \cdot \sigma /\sqrt{n}$ and right endpoint $\bar{X} + {1.96} \cdot \sigma /\sqrt{n}$ . In interval notation, this becomes

$$
\left( {\bar{X} - {1.96} \cdot \frac{\sigma }{\sqrt{n}},\;\bar{X} + {1.96} \cdot \frac{\sigma }{\sqrt{n}}}\right) \tag{7.4}
$$

The interval (7.4) is random because the two endpoints of the interval involve a random variable. It is centered at the sample mean $\bar{X}$ and extends ${1.96\sigma }/\sqrt{n}$ to each side of $\bar{X}$ . Thus the interval’s width is $2 \cdot \left( {1.96}\right) \cdot \sigma /\sqrt{n}$ , a fixed number; only the location of the interval (its midpoint $\bar{X}$ ) is random (Figure 7.2). Now (7.3) can be paraphrased as "the probability is .95 that the random interval (7.4) includes or covers the true value of $\mu$ ." Before any data is gathered, it is quite likely that $\mu$ will lie inside the interval (7.4).

![01927a02-a1da-7086-ba87-2208e017bc0f_2_855_2018_502_150_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_2_855_2018_502_150_0.jpg)

Figure 7.2 The random interval (7.4) centered at $\bar{X}$

---

DEFINITION

---

If, after observing ${X}_{1} = {x}_{1},{X}_{2} = {x}_{2},\ldots ,{X}_{n} = {x}_{n}$ , we compute the observed sample mean $\bar{x}$ and then substitute $\bar{x}$ into (7.4) in place of $\bar{X}$ , the resulting fixed interval is called a ${95}\%$ confidence interval for $\mathbf{\mu }$ . This CI can be expressed either as

$$
\left( {\bar{x} - {1.96} \cdot \frac{\sigma }{\sqrt{n}},\bar{x} + {1.96} \cdot \frac{\sigma }{\sqrt{n}}}\right) \text{is a}{95}\% \mathrm{{CI}}\text{for}\mu
$$

or as

$$
\bar{x} - {1.96} \cdot \frac{\sigma }{\sqrt{n}} < \mu < \bar{x} + {1.96} \cdot \frac{\sigma }{\sqrt{n}}\text{with}{95}\% \text{confidence}
$$

A concise expression for the interval is $\bar{x} \pm {1.96} \cdot \sigma /\sqrt{n}$ , where - gives the left endpoint (lower limit) and + gives the right endpoint (upper limit).

---

EXAMPLE 7.2 (Example 7.1 continued)

---

2 The quantities needed for computation of the ${95}\% \mathrm{{CI}}$ for true average preferred height are $\sigma = {2.0}, n = {31}$ , and $\bar{x} = {80.0}$ . The resulting interval is

$$
\bar{x} \pm {1.96} \cdot \frac{\sigma }{\sqrt{n}} = {80.0} \pm \left( {1.96}\right) \frac{2.0}{\sqrt{31}} = {80.0} \pm {.7} = \left( {{79.3},{80.7}}\right)
$$

That is, we can be highly confident, at the ${95}\%$ confidence level, that ${79.3} < \mu < {80.7}$ . This interval is relatively narrow, indicating that $\mu$ has been rather precisely estimated.

## Interpreting a Confidence Level

The confidence level ${95}\%$ for the interval just defined was inherited from the probability .95 for the random interval (7.4). Intervals having other levels of confidence will be introduced shortly. For now, though, consider how ${95}\%$ confidence can be interpreted.

We started with an event whose probability was .95 - that the random interval (7.4) would capture the true value of $\mu$ -and then used the data in Example 7.1 to compute the CI $\left( {{79.3},{80.7}}\right)$ . It is therefore tempting to conclude that $\mu$ is within this fixed interval with probability .95 . But by substituting $\bar{x} = {80.0}$ for $\bar{X}$ , all randomness disappears; the interval $\left( {{79.3},{80.7}}\right)$ is not a random interval, and $\mu$ is a constant (unfortunately unknown to us). Thus it is incorrect to write the statement $P\left( {\mu \text{lies in}\left( {{79.3},{80.7}}\right) }\right) = {.95}$ .

A correct interpretation of "95% confidence" relies on the long-run relative frequency interpretation of probability: To say that an event $A$ has probability .95 is to say that if the experiment on which $A$ is defined is performed over and over again, in the long run $A$ will occur ${95}\%$ of the time. Suppose we obtain another sample of typists’ preferred heights and compute another ${95}\%$ interval. Now consider repeating this for a third sample, a fourth sample, a fifth sample, and so on. Let $A$ be the event that $\bar{X} - {1.96} \cdot \sigma /\sqrt{n} < \mu < \bar{X} + {1.96} \cdot \sigma /\sqrt{n}$ . Since $P\left( A\right) = {.95}$ , in the long run ${95}\%$ of our computed CIs will contain $\mu$ . This is illustrated in Figure 7.3, where the vertical line cuts the measurement axis at the true (but unknown) value of $\mu$ . Notice that 7 of the 100 intervals shown fail to contain $\mu$ . In the long run, only $5\%$ of the intervals so constructed would fail to contain $\mu$ .

According to this interpretation, the confidence level ${95}\%$ is not so much a statement about any particular interval such as $\left( {{79.3},{80.7}}\right)$ . Instead it pertains to what would happen if a very large number of like intervals were to be constructed using the same CI formula. Although this may seem unsatisfactory, the root of the difficulty lies with our interpretation of probability-it applies to a long sequence of replications of an experiment rather than just a single replication. There is another approach to the construction and interpretation of CIs that uses the notion of subjective probability and Bayes' theorem, but the technical details are beyond the scope of this text; the book by DeGroot, et al. (see the Chapter 6 bibliography) is a good source. The interval presented here (as well as each interval presented subsequently) is called a "classical" CI because its interpretation rests on the classical notion of probability.

![01927a02-a1da-7086-ba87-2208e017bc0f_4_736_179_685_1073_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_4_736_179_685_1073_0.jpg)

Figure 7.3 One hundred ${95}\%$ CIs (asterisks identify intervals that do not include $\mu$ )

## Other Levels of Confidence

The confidence level of ${95}\%$ was inherited from the probability .95 for the initial inequalities in (7.2). If a confidence level of ${99}\%$ is desired, the initial probability of ${.95}$ must be replaced by .99, which necessitates changing the $z$ critical value from 1.96 to 2.58 . A ${99}\%$ CI then results from using 2.58 in place of 1.96 in the formula for the ${95}\%$ CI.

In fact, any desired level of confidence can be achieved by replacing 1.96 or 2.58 with the appropriate standard normal critical value. Recall from Chapter 4 the notation for a $z$ critical value: ${z}_{\alpha }$ is the number on the horizontal $z$ scale that captures upper tail area $\alpha$ . As Figure 7.4 shows, a probability (i.e., central $z$ curve area) of $1 - \alpha$ is achieved by using ${z}_{\alpha /2}$ in place of 1.96 .

![01927a02-a1da-7086-ba87-2208e017bc0f_5_933_185_530_263_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_5_933_185_530_263_0.jpg)

Figure 7.4 $\;P\left( {-{z}_{\alpha /2} < Z < {z}_{\alpha /2}}\right) = 1 - \alpha$

## DEFINITION

A ${100}\left( {1 - \alpha }\right) \%$ confidence interval for the mean $\mu$ of a normal population when the value of $\sigma$ is known is given by

$$
\left( {\bar{x} - {z}_{\alpha /2} \cdot \frac{\sigma }{\sqrt{n}},\bar{x} + {z}_{\alpha /2} \cdot \frac{\sigma }{\sqrt{n}}}\right) \tag{7.5}
$$

or, equivalently, by $\bar{x} \pm {z}_{\alpha /2} \cdot \sigma /\sqrt{n}$ .

The formula (7.5) for the CI can also be expressed in words as

point estimate of $\mu \pm$ ( $z$ critical value) (standard error of the mean).

EXAMPLE 7.3 The production process for engine control housing units of a particular type has recently been modified. Prior to this modification, historical data had suggested that the distribution of hole diameters for bushings on the housings was normal with a standard deviation of ${.100}\mathrm{\;{mm}}$ . It is believed that the modification has not affected the shape of the distribution or the standard deviation, but that the value of the mean diameter may have changed. A sample of 40 housing units is selected and hole diameter is determined for each one, resulting in a sample mean diameter of ${5.426}\mathrm{\;{mm}}$ . Let’s calculate a confidence interval for true average hole diameter using a confidence level of ${90}\%$ . This requires that ${100}\left( {1 - \alpha }\right) = {90}$ , from which $\alpha = {.10}$ and ${z}_{\alpha /2} = {z}_{.05} = {1.645}$ (corresponding to a cumulative $z$ -curve area of .9500). The desired interval is then

$$
{5.426} \pm \left( {1.645}\right) \frac{.100}{\sqrt{40}} = {5.426} \pm {.026} = \left( {{5.400},{5.452}}\right)
$$

With a reasonably high degree of confidence, we can say that ${5.400} < \mu < {5.452}$ . This interval is rather narrow because of the small amount of variability in hole diameter $\left( {\sigma = {.100}}\right)$ .

## Confidence Level, Precision, and Sample Size

Why settle for a confidence level of ${95}\%$ when a level of ${99}\%$ is achievable? Because the price paid for the higher confidence level is a wider interval. Since the ${95}\%$ interval extends ${1.96} \cdot \sigma /\sqrt{n}$ to each side of $\bar{x}$ , the width of the interval is $2\left( {1.96}\right) \cdot \sigma /\sqrt{n} = {3.92} \cdot \sigma /\sqrt{n}$ . Similarly, the width of the ${99}\%$ interval is $2\left( {2.58}\right) \cdot \sigma /\sqrt{n} = {5.16} \cdot \sigma /\sqrt{n}$ . That is, we have more confidence in the ${99}\%$ interval precisely because it is wider. The higher the desired degree of confidence, the wider the resulting interval will be.

If we think of the width of the interval as specifying its precision or accuracy, then the confidence level (or reliability) of the interval is inversely related to its precision. A highly reliable interval estimate may be imprecise in that the endpoints of the interval may be far apart, whereas a precise interval may entail relatively low reliability. Thus it cannot be said unequivocally that a ${99}\%$ interval is to be preferred to a ${95}\%$ interval; the gain in reliability entails a loss in precision.

An appealing strategy is to specify both the desired confidence level and interval width and then determine the necessary sample size.

EXAMPLE 7.4 Extensive monitoring of a computer time-sharing system has suggested that response time to a particular editing command is normally distributed with standard deviation 25 millisec. A new operating system has been installed, and we wish to estimate the true average response time $\mu$ for the new environment. Assuming that response times are still normally distributed with $\sigma = {25}$ , what sample size is necessary to ensure that the resulting ${95}\% \mathrm{{CI}}$ has a width of (at most) 10 ? The sample size $n$ must satisfy

$$
{10} = 2 \cdot \left( {1.96}\right) \left( {{25}/\sqrt{n}}\right)
$$

Rearranging this equation gives

$$
\sqrt{n} = 2 \cdot \left( {1.96}\right) \left( {25}\right) /{10} = {9.80}
$$

so

$$
n = {\left( {9.80}\right) }^{2} = {96.04}
$$

Since $n$ must be an integer, a sample size of 97 is required.

A general formula for the sample size $n$ necessary to ensure an interval width $w$ is obtained from equating $w$ to $2 \cdot {z}_{\alpha /2} \cdot \sigma /\sqrt{n}$ and solving for $n$ .

The sample size necessary for the CI (7.5) to have a width $w$ is

$$
n = {\left( 2{z}_{\alpha /2} \cdot \frac{\sigma }{w}\right) }^{2}
$$

The smaller the desired width $w$ , the larger $n$ must be. In addition, $n$ is an increasing function of $\sigma$ (more population variability necessitates a larger sample size) and of the confidence level ${100}\left( {1 - \alpha }\right) \%$ (as $\alpha$ decreases, ${z}_{\alpha /2}$ increases).

The half-width ${1.96\sigma }/\sqrt{n}$ of the ${95}\% \mathrm{{CI}}$ is sometimes called the bound on the error of estimation associated with a 95% confidence level. That is, with 95% confidence, the point estimate $\bar{x}$ will be no farther than this from $\mu$ . Before obtaining data, an investigator may wish to determine a sample size for which a particular value of the bound is achieved. For example, with $\mu$ representing the average fuel efficiency (mpg) for all cars of a certain type, the objective of an investigation may be to estimate $\mu$ to within $1\mathrm{{mpg}}$ with ${95}\%$ confidence. More generally, if we wish to estimate $\mu$ to within an amount $B$ (the specified bound on the error of estimation) with ${100}\left( {1 - \alpha }\right) \%$ confidence, the necessary sample size results from replacing $2/w$ by $1/B$ in the formula in the preceding box.

## Deriving a Confidence Interval

Let ${X}_{1},{X}_{2},\ldots ,{X}_{n}$ denote the sample on which the CI for a parameter $\theta$ is to be based.

Suppose a random variable satisfying the following two properties can be found:

1. The variable is a function of both ${X}_{1},\ldots ,{X}_{n}$ and $\theta$ .

2. The probability distribution of the variable does not depend on $\theta$ or on any other unknown parameters.

Let $h\left( {{X}_{1},{X}_{2},\ldots ,{X}_{n};\theta }\right)$ denote this random variable. For example, if the population distribution is normal with known $\sigma$ and $\theta = \mu$ , the variable $h\left( {{X}_{1},\ldots ,{X}_{n};\mu }\right) = \left( {\bar{X} - \mu }\right) /\left( {\sigma /\sqrt{n}}\right)$ satisfies both properties; it clearly depends functionally on $\mu$ , yet has the standard normal probability distribution irrespective of the value of $\mu$ . In general, the form of the $h$ function is usually suggested by examining the distribution of an appropriate estimator $\widehat{\theta }$ .

For any $\alpha$ between 0 and 1, constants $a$ and $b$ can be found to satisfy

$$
P\left( {a < h\left( {{X}_{1},\ldots ,{X}_{n};\theta }\right) < b}\right) = 1 - \alpha \tag{7.6}
$$

Because of the second property, $a$ and $b$ do not depend on $\theta$ . In the normal example, $a = - {z}_{\alpha /2}$ and $b = {z}_{\alpha /2}$ . Now suppose that the inequalities in (7.6) can be manipulated to isolate $\theta$ , giving the equivalent probability statement

$$
P\left( {l\left( {{X}_{1},{X}_{2},\ldots ,{X}_{n}}\right) < \theta < u\left( {{X}_{1},{X}_{2},\ldots ,{X}_{n}}\right) }\right) = 1 - \alpha
$$

Then $l\left( {{x}_{1},{x}_{2},\ldots ,{x}_{n}}\right)$ and $u\left( {{x}_{1},\ldots ,{x}_{n}}\right)$ are the lower and upper confidence limits, respectively, for a ${100}\left( {1 - \alpha }\right) \% \mathrm{{CI}}$ . In the normal example, we saw that $l\left( {{X}_{1},\ldots ,{X}_{n}}\right) = \bar{X} - {z}_{\alpha /2} \cdot \sigma /\sqrt{n}$ and $u\left( {{X}_{1},\ldots ,{X}_{n}}\right) = \bar{X} + {z}_{\alpha /2} \cdot \sigma /\sqrt{n}$ .

EXAMPLE 7.5 A theoretical model suggests that the time to breakdown of an insulating fluid between electrodes at a particular voltage has an exponential distribution with parameter $\lambda$ (see Section 4.4). A random sample of $n = {10}$ breakdown times yields the following sample data (in min): ${x}_{1} = {41.53},{x}_{2} = {18.73},{x}_{3} = {2.99},{x}_{4} = {30.34}$ , ${x}_{5} = {12.33},{x}_{6} = {117.52},{x}_{7} = {73.02},{x}_{8} = {223.63},{x}_{9} = {4.00},{x}_{10} = {26.78}$ . A ${95}\%$ $\mathrm{{CI}}$ for $\lambda$ and for the true average breakdown time are desired.

Let $h\left( {{X}_{1},{X}_{2},\ldots ,{X}_{n};\lambda }\right) = {2\lambda \sum }{X}_{i}$ . It can be shown that this random variable has a probability distribution called a chi-squared distribution with ${2n}$ degrees of freedom (df) $(\nu = {2n}$ , where $\nu$ is the parameter of a chi-squared distribution as mentioned in Section 4.4). Appendix Table A. 7 pictures a typical chi-squared density curve and tabulates critical values that capture specified tail areas. The relevant number of df here is $2\left( {10}\right) = {20}$ . The $\nu = {20}$ row of the table shows that 34.170 captures upper-tail area .025 and 9.591 captures lower-tail area .025 (upper-tail area .975). Thus for $n = {10}$ ,

$$
P\left( {{9.591} < {2\lambda }\sum {X}_{i} < {34.170}}\right) = {.95}
$$

Division by ${2\sum }{X}_{i}$ isolates $\lambda$ , yielding

$$
P\left( {{9.591}/\left( {2\sum {X}_{i}}\right) < \lambda < \left( {{34.170}/\left( {2\sum {X}_{i}}\right) }\right) = {.95}}\right.
$$

The lower limit of the ${95}\%$ CI for $\lambda$ is ${9.591}/\left( {{2\sum }{x}_{i}}\right)$ , and the upper limit is ${34.170}/\left( {{2\sum }{x}_{i}}\right)$ . For the given data, $\sum {x}_{i} = {550.87}$ , giving the interval $({.00871}$ , .03101).

The expected value of an exponential rv is $\mu = 1/\lambda$ . Since

$$
P\left( {2\sum {X}_{i}/{34.170} < 1/\lambda < 2\sum {X}_{i}/{9.591}}\right) = {.95}
$$

the ${95}\% \mathrm{{CI}}$ for true average breakdown time is $\left( {{2\sum }{x}_{i}/{34.170},{2\sum }{x}_{i}/{9.591}}\right) =$ (32.24, 114.87). This interval is obviously quite wide, reflecting substantial variability in breakdown times and a small sample size.

In general, the upper and lower confidence limits result from replacing each $<$ in (7.6) by $=$ and solving for $\theta$ . In the insulating fluid example just considered, ${2\lambda \sum }{x}_{i} = {34.170}$ gives $\lambda = {34.170}/\left( {{2\sum }{x}_{i}}\right)$ as the upper confidence limit, and the lower limit is obtained from the other equation. Notice that the two interval limits are not equidistant from the point estimate, since the interval is not of the form $\widehat{\theta } \pm c$ .

## Bootstrap Confidence Intervals

The bootstrap technique was introduced in Chapter 6 as a way of estimating ${\sigma }_{\widehat{\theta }}$ . It can also be applied to obtain a CI for $\theta$ . Consider again estimating the mean $\mu$ of a normal distribution when $\sigma$ is known. Let’s replace $\mu$ by $\theta$ and use $\bar{\theta } = \bar{X}$ as the point estimator. Notice that ${1.96\sigma }\sqrt{n}$ is the 97.5th percentile of the distribution of $\widehat{\theta } - \theta$ [that is, $P\left( {\bar{X} - \mu < {1.96\sigma }/\sqrt{n}}\right) = P\left( {Z < {1.96}}\right) = {.9750}$ ]. Similarly, $- {1.96\sigma }/\sqrt{n}$ is the 2.5th percentile, so

$$
{.95} = P\left( {{2.5}\text{th percentile} < \widehat{\theta } - \theta < {97.5}\text{th percentile}}\right)
$$

$$
= P\left( {\widehat{\theta } - {2.5}\text{ th percentile } > \theta > \widehat{\theta } - {97.5}\text{ th percentile }}\right)
$$

That is, with

$$
l = \widehat{\theta } - {97.5}\text{th percentile of}\widehat{\theta } - \theta
$$

$$
u = \widehat{\theta } - {2.5}\text{th percentile of}\widehat{\theta } - \theta \tag{7.7}
$$

the CI for $\theta$ is $\left( {l, u}\right)$ . In many cases, the percentiles in (7.7) cannot be calculated, but they can be estimated from bootstrap samples. Suppose we obtain $B = {1000}$ bootstrap samples and calculate ${\widehat{\theta }}_{1}^{ * },\ldots ,{\widehat{\theta }}_{1000}^{ * }$ , and ${\bar{\theta }}^{ * }$ followed by the 1000 differences ${\widehat{\theta }}_{1}^{ * } - {\bar{\theta }}^{ * },\ldots ,{\widehat{\theta }}_{1000}^{ * } - {\bar{\theta }}^{ * }$ . The 25th largest and 25th smallest of these differences are estimates of the unknown percentiles in (7.7). Consult the Devore and Berk or Efron books cited in Chapter 6 for more information.

## EXERCISES Section 7.1 (1-11)

1. Consider a normal population distribution with the value of $\sigma$ known.

a. What is the confidence level for the interval $\bar{x} \pm$ ${2.81\sigma }/\sqrt{n}$ ?

b. What is the confidence level for the interval $\bar{x} \pm$ ${1.44\sigma }/\sqrt{n}$ ?

c. What value of ${z}_{\alpha /2}$ in the CI formula (7.5) results in a confidence level of ${99.7}\%$ ?

d. Answer the question posed in part (c) for a confidence level of ${75}\%$ .

2. Each of the following is a confidence interval for $\mu =$ true average (i.e., population mean) resonance frequency (Hz) for all tennis rackets of a certain type:

$\left( {{114.4},{115.6}}\right) \;\left( {{114.1},{115.9}}\right)$

a. What is the value of the sample mean resonance frequency?

b. Both intervals were calculated from the same sample data. The confidence level for one of these intervals is ${90}\%$ and for the other is ${99}\%$ . Which of the intervals has the ${90}\%$ confidence level, and why?

3. Suppose that a random sample of 50 bottles of a particular brand of cough syrup is selected and the alcohol content of each bottle is determined. Let $\mu$ denote the average alcohol content for the population of all bottles of the brand under study. Suppose that the resulting ${95}\%$ confidence interval is $\left( {{7.8},{9.4}}\right)$ .

a. Would a ${90}\%$ confidence interval calculated from this same sample have been narrower or wider than the given interval? Explain your reasoning.

b. Consider the following statement: There is a ${95}\%$ chance that $\mu$ is between 7.8 and 9.4. Is this statement correct? Why or why not?

c. Consider the following statement: We can be highly confident that ${95}\%$ of all bottles of this type of cough syrup have an alcohol content that is between 7.8 and 9.4. Is this statement correct? Why or why not?

d. Consider the following statement: If the process of selecting a sample of size 50 and then computing the corresponding ${95}\%$ interval is repeated 100 times,95 of the resulting intervals will include $\mu$ . Is this statement correct? Why or why not?

4. A CI is desired for the true average stray-load loss $\mu$ (watts) for a certain type of induction motor when the line current is held at 10 amps for a speed of ${1500}\mathrm{{rpm}}$ . Assume that stray-load loss is normally distributed with $\sigma = {3.0}$ .

a. Compute a ${95}\% \mathrm{{CI}}$ for $\mu$ when $n = {25}$ and $\bar{x} = {58.3}$ .

b. Compute a ${95}\% \mathrm{{CI}}$ for $\mu$ when $n = {100}$ and $\bar{x} =$ 58.3.

c. Compute a ${99}\%$ CI for $\mu$ when $n = {100}$ and $\bar{x} =$ 58.3.

d. Compute an ${82}\%$ CI for $\mu$ when $n = {100}$ and $\bar{x} =$ 58.3.

e. How large must $n$ be if the width of the ${99}\%$ interval for $\mu$ is to be 1.0 ?

5. Assume that the helium porosity (in percentage) of coal samples taken from any particular seam is normally distributed with true standard deviation .75 .

a. Compute a ${95}\% \mathrm{{CI}}$ for the true average porosity of a certain seam if the average porosity for 20 specimens from the seam was 4.85.

b. Compute a ${98}\% \mathrm{{CI}}$ for true average porosity of another seam based on 16 specimens with a sample average porosity of 4.56 .

c. How large a sample size is necessary if the width of the ${95}\%$ interval is to be .40 ?

d. What sample size is necessary to estimate true average porosity to within ${.2}$ with ${99}\%$ confidence?

6. On the basis of extensive tests, the yield point of a particular type of mild steel-reinforcing bar is known to be normally distributed with $\sigma = {100}$ . The composition of bars has been slightly modified, but the modification is not believed to have affected either the normality or the value of $\sigma$ .

a. Assuming this to be the case, if a sample of 25 modified bars resulted in a sample average yield point of ${8439}\mathrm{{lb}}$ , compute a ${90}\% \mathrm{{CI}}$ for the true average yield point of the modified bar.

b. How would you modify the interval in part (a) to obtain a confidence level of ${92}\%$ ?

7. By how much must the sample size $n$ be increased if the width of the CI (7.5) is to be halved? If the sample size is increased by a factor of 25 , what effect will this have on the width of the interval? Justify your assertions.

8. Let ${\alpha }_{1} > 0,{\alpha }_{2} > 0$ , with ${\alpha }_{1} + {\alpha }_{2} = \alpha$ . Then

$$
P\left( {-{z}_{{\alpha }_{1}} < \frac{\bar{X} - \mu }{\sigma /\sqrt{n}} < {z}_{{\alpha }_{2}}}\right) = 1 - \alpha
$$

a. Use this equation to derive a more general expression for a ${100}\left( {1 - \alpha }\right) \%$ CI for $\mu$ of which the interval (7.5) is a special case.

b. Let $\alpha = {.05}$ and ${\alpha }_{1} = \alpha /4,{\alpha }_{2} = {3\alpha }/4$ . Does this result in a narrower or wider interval than the interval (7.5)?

9. a. Under the same conditions as those leading to the interval (7.5), $P\left\lbrack {\left( {\bar{X} - \mu }\right) /\left( {\sigma /\sqrt{n}}\right) < {1.645}}\right\rbrack = {.95}$ . Use this to derive a one-sided interval for $\mu$ that has infinite width and provides a lower confidence bound on $\mu$ . What is this interval for the data in Exercise 5(a)?

b. Generalize the result of part (a) to obtain a lower bound with confidence level ${100}\left( {1 - \alpha }\right) \%$ .

c. What is an analogous interval to that of part (b) that provides an upper bound on $\mu$ ? Compute this ${99}\%$ interval for the data of Exercise 4(a).

10. A random sample of $n = {15}$ heat pumps of a certain type yielded the following observations on lifetime (in years): $\begin{array}{llllllll} {2.0} & {1.3} & {6.0} & {1.9} & {5.1} & {.4} & {1.0} & {5.3} \end{array}$ 15.7 .7 4.8 .9 12.2 5.3 .6

a. Assume that the lifetime distribution is exponential and use an argument parallel to that of Example 7.5 to obtain a ${95}\% \mathrm{{CI}}$ for expected (true average) lifetime.

b. How should the interval of part (a) be altered to achieve a confidence level of ${99}\%$ ?

c. What is a ${95}\% \mathrm{{CI}}$ for the standard deviation of the lifetime distribution? [Hint: What is the standard deviation of an exponential random variable?]

11. Consider the next ${100095}\%$ CIs for $\mu$ that a statistical consultant will obtain for various clients. Suppose the data sets on which the intervals are based are selected independently of one another. How many of these 1000 intervals do you expect to capture the corresponding value of $\mu$ ? What is the probability that between 940 and 960 of these intervals contain the corresponding value of $\mu$ ? [Hint: Let $Y =$ the number among the 1000 intervals that contain $\mu$ . What kind of random variable is $Y$ ?]

## 7.2 Large-Sample Confidence Intervals for a Population Mean and Proportion

The CI for $\mu$ given in the previous section assumed that the population distribution is normal with the value of $\sigma$ known. We now present a large-sample CI whose validity does not require these assumptions. After showing how the argument leading to this interval generalizes to yield other large-sample intervals, we focus on an interval for a population proportion $p$ .

Copyright 2016 Cengage Learning. All Rights Reserved, May not be copied, scanned, or duplicated, in whole or in part. Due to electronic rights, some third party content may be suppressed from the eBook and/or eChapter(s). Editorial review has deemed that any suppressed content does not materially affect the overall learning experience. Congage Learning reserves the right to remove additional content at any time if subsequent rights restrictions require it.

## A Large-Sample Interval for $\mu$

Let ${X}_{1},{X}_{2},\ldots ,{X}_{n}$ be a random sample from a population having a mean $\mu$ and standard deviation $\sigma$ . Provided that $n$ is sufficiently large, the Central Limit Theorem (CLT) implies that $\bar{X}$ has approximately a normal distribution whatever the nature of the population distribution. It then follows that $Z = \left( {\bar{X} - \mu }\right) /\left( {\sigma /\sqrt{n}}\right)$ has approximately a standard normal distribution, so that

$$
P\left( {-{z}_{\alpha /2} < \frac{\bar{X} - \mu }{\sigma /\sqrt{n}} < {z}_{\alpha /2}}\right) \approx 1 - \alpha
$$

An argument parallel to that given in Section 7.1 yields $\bar{x} \pm {z}_{\alpha /2} \cdot \sigma /\sqrt{n}$ as a large-sample CI for $\mu$ with a confidence level of approximately ${100}\left( {1 - \alpha }\right) \%$ . That is, when $n$ is large, the CI for $\mu$ given previously remains valid whatever the population distribution, provided that the qualifier "approximately" is inserted in front of the confidence level.

A practical difficulty with this development is that computation of the CI requires the value of $\sigma$ , which will rarely be known. Consider replacing the population standard deviation $\sigma$ in $Z$ by the sample standard deviation to obtain the standardized variable

$$
\frac{\bar{X} - \mu }{S/\sqrt{n}}
$$

Previously, there was randomness only in the numerator of $Z$ by virtue of $\bar{X}$ . In the new standardized variable, both $\bar{X}$ and $S$ vary in value from one sample to another. So it might seem that the distribution of the new variable should be more spread out than the $z$ curve to reflect the extra variation in the denominator. This is indeed true when $n$ is small. However, for large $n$ the subsititution of $S$ for $\sigma$ adds little extra variability, so this variable also has approximately a standard normal distribution. Manipulation of the variable in a probability statement, as in the case of known $\sigma$ , gives a general large-sample CI for $\mu$ .

---

PROPOSITION

---

If $n$ is sufficiently large, the standardized variable

$$
Z = \frac{\bar{X} - \mu }{S/\sqrt{n}}
$$

has approximately a standard normal distribution. This implies that

$$
\bar{x} \pm {z}_{\alpha /2} \cdot \frac{s}{\sqrt{n}} \tag{7.8}
$$

is a large-sample confidence interval for $\mathbf{\mu }$ with confidence level approximately ${100}\left( {1 - \alpha }\right) \%$ . This formula is valid regardless of the shape of the population distribution.

In words, the CI (7.8) is

point estimate of $\mu \pm$ ( $z$ critical value) (estimated standard error of the mean).

Generally speaking, $n > {40}$ will be sufficient to justify the use of this interval. This is somewhat more conservative than the rule of thumb for the CLT because of the additional variability introduced by using $S$ in place of $\sigma$ .

AMPLE 7.6 Haven't you always wanted to own a Porsche? The author thought maybe he could afford a Boxster, the cheapest model. So he went to www.cars.com on Nov. 18, 2009, and found a total of 1113 such cars listed. Asking prices ranged from \$3499

to $\$ {130},{000}$ (the latter price was one of only two exceeding $\$ {70},{000}$ ). The prices depressed him, so he focused instead on odometer readings (miles). Here are reported readings for a sample of 50 of these Boxsters:

<table><tr><td>2948</td><td>2996</td><td>7197</td><td>8338</td><td>8500</td><td>8759</td><td>12710</td><td>12925</td></tr><tr><td>15767</td><td>20000</td><td>23247</td><td>24863</td><td>26000</td><td>26210</td><td>30552</td><td>30600</td></tr><tr><td>35700</td><td>36466</td><td>40316</td><td>40596</td><td>41021</td><td>41234</td><td>43000</td><td>44607</td></tr><tr><td>45000</td><td>45027</td><td>45442</td><td>46963</td><td>47978</td><td>49518</td><td>52000</td><td>53334</td></tr><tr><td>54208</td><td>56062</td><td>57000</td><td>57365</td><td>60020</td><td>60265</td><td>60803</td><td>62851</td></tr><tr><td>64404</td><td>72140</td><td>74594</td><td>79308</td><td>79500</td><td>80000</td><td>80000</td><td>84000</td></tr><tr><td>113000</td><td>118634</td><td></td><td></td><td></td><td></td><td></td><td></td></tr></table>

A boxplot of the data (Figure 7.5) shows that, except for the two outliers at the upper end, the distribution of values is reasonably symmetric (in fact, a normal probability plot exhibits a reasonably linear pattern, though the points corresponding to the two smallest and two largest observations are somewhat removed from a line fit through the remaining points).

![01927a02-a1da-7086-ba87-2208e017bc0f_11_651_861_1098_291_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_11_651_861_1098_291_0.jpg)

Figure 7.5 A boxplot of the odometer reading data from Example 7.6

Summary quantities include $n = {50},\bar{x} = {45},{679.4},\widetilde{x} = {45},{013.5}, s = {26},{641.675}$ , ${f}_{s} = {34},{265}$ . The mean and median are reasonably close (if the two largest values were each reduced by 30,000 , the mean would fall to 44,479.4 , while the median would be unaffected). The boxplot and the magnitudes of $s$ and ${f}_{s}$ relative to the mean and median both indicate a substantial amount of variability. A confidence level of about ${95}\%$ requires ${z}_{.025} = {1.96}$ , and the interval is

$$
{45},{679.4} \pm \left( {1.96}\right) \left( \frac{{26},{641.675}}{\sqrt{50}}\right) = {45},{679.4} \pm {7384.7}
$$

$$
= \left( {{38},{294.7},{53},{064.1}}\right)
$$

That is, ${38},{294.7} < \mu < {53},{064.1}$ with ${95}\%$ confidence. This interval is rather wide because a sample size of 50 , even though large by our rule of thumb, is not large enough to overcome the substantial variability in the sample. We do not have a very precise estimate of the population mean odometer reading.

Is the interval we’ve calculated one of the ${95}\%$ that in the long run includes the parameter being estimated, or is it one of the "bad" $5\%$ that does not do so? Without knowing the value of $\mu$ , we cannot tell. Remember that the confidence level refers to the long run capture percentage when the formula is used repeatedly on various samples; it cannot be interpreted for a single sample and the resulting interval.

Unfortunately, the choice of sample size to yield a desired interval width is not as straightforward here as it was for the case of known $\sigma$ . This is because the width of (7.8) is $2{z}_{\alpha /2}s/\sqrt{n}$ . Since the value of $s$ is not available before the data has been gathered, the width of the interval cannot be determined solely by the choice of $n$ . The only option for an investigator who wishes to specify a desired width is to make an educated guess as to what the value of $s$ might be. By being conservative and guessing a larger value of $s$ , an $n$ larger than necessary will be chosen. The investigator may be able to specify a reasonably accurate value of the population range (the difference between the largest and smallest values). Then if the population distribution is not too skewed, dividing the range by 4 gives a ballpark value of what $s$ might be.

EXAMPLE 7.7 The charge-to-tap time (min) for carbon steel in one type of open hearth furnace is to be determined for each heat in a sample of size $n$ . If the investigator believes that almost all times in the distribution are between 320 and 440 , what sample size would be appropriate for estimating the true average time to within $5\mathrm{\;{min}}$ . with a confidence level of ${95}\%$ ?

A reasonable value for $s$ is $\left( {{440} - {320}}\right) /4 = {30}$ . Thus

$$
n = {\left\lbrack \frac{\left( {1.96}\right) \left( {30}\right) }{5}\right\rbrack }^{2} = {138.3}
$$

Since the sample size must be an integer, $n = {139}$ should be used. Note that estimating to within $5\mathrm{\;{min}}$ . with the specified confidence level is equivalent to a CI width of 10 min.

## A General Large-Sample Confidence Interval

The large-sample intervals $\bar{x} \pm {z}_{\alpha /2} \cdot \sigma /\sqrt{n}$ and $\bar{x} \pm {z}_{\alpha /2} \cdot s/\sqrt{n}$ are special cases of a general large-sample CI for a parameter $\theta$ . Suppose that $\widehat{\theta }$ is an estimator satisfying the following properties: (1) It has approximately a normal distribution; (2) it is (at least approximately) unbiased; and (3) an expression for ${\sigma }_{\widehat{\theta }}$ , the standard deviation (standard error) of $\widehat{\theta }$ , is available. For example, in the case $\theta = \mu ,\widehat{\mu } = \bar{X}$ is an unbiased estimator whose distribution is approximately normal when $n$ is large and ${\sigma }_{\widehat{\mu }} = {\sigma }_{\bar{X}} = \sigma /\sqrt{n}$ . Standardizing $\widehat{\theta }$ yields the rv $Z = \left( {\widehat{\theta } - \theta }\right) /{\sigma }_{\widehat{\theta }}$ , which has approximately a standard normal distribution. This justifies the probability statement

$$
P\left( {-{z}_{\alpha /2} < \frac{\widehat{\theta } - \theta }{{\sigma }_{\widehat{\theta }}} < {z}_{\alpha /2}}\right) \approx 1 - \alpha \tag{7.9}
$$

Assume first that ${\sigma }_{\widehat{\theta }}$ does not involve any unknown parameters (e.g., known $\sigma$ in the case $\theta = \mu$ ). Then replacing each $<$ in (7.9) by $=$ results in $\theta = \widehat{\theta } \pm {z}_{\alpha /2} \cdot {\sigma }_{\widehat{\theta }}$ , so the lower and upper confidence limits are $\widehat{\theta } - {z}_{\alpha /2} \cdot {\sigma }_{\widehat{\theta }}$ and $\widehat{\theta } + {z}_{\alpha /2} \cdot {\sigma }_{\widehat{\theta }}$ , respectively. Now suppose that ${\sigma }_{\widehat{\theta }}$ does not involve $\theta$ but does involve at least one other unknown parameter. Let ${s}_{\widehat{\theta }}$ be the estimate of ${\sigma }_{\widehat{\theta }}$ obtained by using estimates in place of the unknown parameters (e.g., $s/\sqrt{n}$ estimates $\sigma /\sqrt{n}$ ). Under general conditions (essentially that ${s}_{\widehat{\theta }}$ be close to ${\sigma }_{\widehat{\theta }}$ for most samples), a valid CI is $\widehat{\theta } \pm {z}_{\alpha /2} \cdot {s}_{\widehat{\theta }}$ . The large-sample interval $\bar{x} \pm {z}_{\alpha /2} \cdot s/\sqrt{n}$ is an example.

Finally, suppose that ${\sigma }_{\widehat{\theta }}$ does involve the unknown $\theta$ . For example, we shall see momentarily that this is the case when $\theta = p$ , a population proportion. Then $\left( {\widehat{\theta } - \theta }\right) /{\sigma }_{\widehat{\theta }} = {z}_{\alpha /2}$ can be difficult to solve. An approximate solution can often be obtained by replacing $\theta$ in ${\sigma }_{\widehat{\theta }}$ by its estimate $\widehat{\theta }$ . This results in an estimated standard deviation ${s}_{\widehat{\theta }}$ , and the corresponding interval is again $\widehat{\theta } \pm {z}_{\alpha /2} \cdot {s}_{\widehat{\theta }}$ .

In words, this CI is

point estimate of $\theta \pm$ ( $z$ critical value)(estimated standard error of the estimator)

## A Confidence Interval for a Population Proportion

Let $p$ denote the proportion of "successes" in a population, where success identifies an individual or object that has a specified property (e.g., individuals who graduated from college, computers that do not need warranty service, etc.). A random sample of $n$ individuals or objects is to be selected, and $X$ is the number of successes in the sample. Provided that $n$ is small compared to the population size, $X$ can be regarded as a binomial rv with $E\left( X\right) = {np}$ and ${\sigma }_{X} = \sqrt{{np}\left( {1 - p}\right) }$ . Furthermore, if both ${np} \geq {10}$ and ${nq} \geq {10},\left( {q = 1 - p}\right) , X$ has approximately a normal distribution.

The natural estimator of $p$ is $\widehat{p} = X/n$ , the sample fraction of successes. Since $\widehat{p}$ is just $X$ multiplied by the constant $1/n,\widehat{p}$ also has approximately a normal distribution. As shown in Section 6.1, $E\left( \widehat{p}\right) = p$ (unbiasedness) and ${\sigma }_{\widehat{p}} = \sqrt{p\left( {1 - p}\right) /n}$ . The standard deviation ${\sigma }_{\widehat{p}}$ involves the unknown parameter $p$ . Standardizing $\widehat{p}$ by subtracting $p$ and dividing by ${\sigma }_{\widehat{p}}$ then implies that

$$
P\left( {-{z}_{\alpha /2} < \frac{\widehat{p} - p}{\sqrt{p\left( {1 - p}\right) /n}} < {z}_{\alpha /2}}\right) \approx 1 - \alpha
$$

Proceeding as suggested in the subsection "Deriving a Confidence Interval" (Section 7.1), the confidence limits result from replacing each $<$ by $=$ and solving the resulting equation for $p$ . But whereas the equations $\left( {\bar{x} - \mu }\right) /\left( {s/\sqrt{n}}\right) = \pm {z}_{\alpha /2}$ employed in deriving the large-sample CI for $\mu$ are linear in $\mu$ , the equations here are quadratic $\left( {p}^{2}\right.$ appears in the numerator when both sides of each equation are squared to eliminate the square root). The two roots are

$$
p = \frac{\widehat{p} + {z}_{\alpha /2}^{2}/{2n}}{1 + {z}_{\alpha /2}^{2}/n} \pm {z}_{\alpha /2}\frac{\sqrt{\widehat{p}\left( {1 - \widehat{p}}\right) /n + {z}_{\alpha /2}^{2}/4{n}^{2}}}{1 + {z}_{\alpha /2}^{2}/n}
$$

$$
= \widetilde{p} \pm {z}_{\alpha /2}\frac{\sqrt{\widehat{p}\left( {1 - \widehat{p}}\right) /n + {z}_{\alpha /2}^{2}/4{n}^{2}}}{1 + {z}_{\alpha /2}^{2}/n}
$$

---

PROPOSITION

---

Let $\widetilde{p} = \left\lbrack {\widehat{p} + {z}_{\alpha /2}^{2}/{2n}}\right\rbrack /\left\lbrack {1 + {z}_{\alpha /2}^{2}/n}\right\rbrack$ . Then a confidence interval for a population proportion $p$ with confidence level approximately ${100}\left( {1 - \alpha }\right)$ $\%$ is

$$
\widetilde{p} \pm {z}_{\alpha /2}\frac{\sqrt{\widehat{p}\widehat{q}/n + {z}_{\alpha /2}^{2}/4{n}^{2}}}{1 + {z}_{\alpha /2}^{2}/n} \tag{7.10}
$$

where $\widehat{q} = 1 - \widehat{p}$ and, as before, the - in (7.10) corresponds to the lower confidence limit and the + to the upper confidence limit.

This is often referred to as the score ${CI}$ for $p$ .

If the sample size $n$ is very large, then ${z}^{2}/{2n}$ is generally quite negligible (small) compared to $\widehat{p}$ and ${z}^{2}/n$ is quite negligible compared to 1, from which $\widetilde{p} \approx \widehat{p}$ . In this case ${z}^{2}/4{n}^{2}$ is also negligible compared to ${pq}/n\left( {n}^{2}\right.$ is a much larger divisor than is $n$ ). As a result, the dominant term in the $\pm$ expression is ${z}_{\alpha /2}\sqrt{\widehat{p}\widehat{q}/n}$ and the score interval is approximately

$$
\widehat{p} \pm {z}_{\alpha /2}\sqrt{\widehat{p}\widehat{q}/n} \tag{7.11}
$$

This latter interval has the general form $\widehat{\theta } \pm {z}_{\alpha /2}{\widehat{\sigma }}_{\widehat{\theta }}$ of a large-sample interval suggested in the last subsection. The approximate CI (7.11) is the one that for decades has appeared in introductory statistics textbooks. It clearly has a much simpler and more appealing form than the score CI. So why bother with the latter?

First of all, suppose we use ${z}_{.025} = {1.96}$ in the traditional formula (7.11). Then our nominal confidence level (the one we think we’re buying by using that $z$ critical value) is approximately ${95}\%$ . So before a sample is selected, the probability that the random interval includes the actual value of $p$ (i.e., the coverage probability) should be about .95 . But as Figure 7.6 shows for the case $n = {100}$ , the actual coverage probability for this interval can differ considerably from the nominal probability .95, particularly when $p$ is not close to . 5 (the graph of coverage probability versus $p$ is very jagged because the underlying binomial probability distribution is discrete rather than continuous). This is generally speaking a deficiency of the traditional interval-the actual confidence level can be quite different from the nominal level even for reasonably large sample sizes. Recent research has shown that the score interval rectifies this behavior-for virtually all sample sizes and values of $p$ , its actual confidence level will be quite close to the nominal level specified by the choice of ${z}_{\alpha /2}$ . This is due largely to the fact that the score interval is shifted a bit toward .5 compared to the traditional interval. In particular, the midpoint $\widetilde{p}$ of the score interval is always a bit closer to . 5 than is the midpoint $\widehat{p}$ of the traditional interval. This is especially important when $p$ is close to 0 or 1 .

![01927a02-a1da-7086-ba87-2208e017bc0f_14_540_1047_1070_575_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_14_540_1047_1070_575_0.jpg)

Figure 7.6 Actual coverage probability for the interval (7.11) for varying values of $p$ when $n = {100}$

In addition, the score interval can be used with nearly all sample sizes and parameter values. It is thus not necessary to check the conditions $n\widehat{p} \geq {10}$ and $n\left( {1 - \widehat{p}}\right) \geq {10}$ that would be required were the traditional interval employed. So rather than asking when $n$ is large enough for (7.11) to yield a good approximation to (7.10), our recommendation is that the score CI should always be used. The slight additional tediousness of the computation is outweighed by the desirable properties of the interval.

AMPLE 7.8 The article “Repeatability and Reproducibility for Pass/Fail Data” (J. of Testing and Eval.,1997: 151-153) reported that in $n = {48}$ trials in a particular laboratory, 16 resulted in ignition of a particular type of substrate by a lighted cigarette. Let $p$ denote the long-run proportion of all such trials that would result in ignition. A point estimate for $p$ is $\widehat{p} = {16}/{48} = {.333}$ . A confidence interval for $p$ with a confidence level of approximately ${95}\%$ is

$$
\frac{{.333} + {\left( {1.96}\right) }^{2}/{96}}{1 + {\left( {1.96}\right) }^{2}/{48}} \pm \left( {1.96}\right) \frac{\sqrt{\left( {.333}\right) \left( {.667}\right) /{48} + {\left( {1.96}\right) }^{2}/{9216}}}{1 + {\left( {1.96}\right) }^{2}/{48}}
$$

$$
= {.345} \pm {.129} = \left( {{.216},{.474}}\right)
$$

This interval is quite wide because a sample size of 48 is not at all large when estimating a proportion.

The traditional interval is

$$
{.333} \pm {1.96}\sqrt{\left( {.333}\right) \left( {.667}\right) /{48}} = {.333} \pm {.133} = \left( {{.200},{.466}}\right)
$$

These two intervals would be in much closer agreement were the sample size substantially larger.

Equating the width of the CI for $p$ to a prespecified width $w$ gives a quadratic equation for the sample size $n$ necessary to give an interval with a desired degree of precision. Suppressing the subscript in ${z}_{\alpha /2}$ , the solution is

$$
n = \frac{2{z}^{2}\widehat{p}\widehat{q} - {z}^{2}{w}^{2} \pm \sqrt{4{z}^{4}\widehat{p}\widehat{q}\left( {\widehat{p}\widehat{q} - {w}^{2}}\right) + {w}^{2}{z}^{4}}}{{w}^{2}} \tag{7.12}
$$

Neglecting the terms in the numerator involving ${w}^{2}$ gives

$$
n \approx \frac{4{z}^{2}\widehat{p}\widehat{q}}{{w}^{2}}
$$

This latter expression is what results from equating the width of the traditional interval to $w$ .

These formulas unfortunately involve the unknown $\widehat{p}$ . The most conservative approach is to take advantage of the fact that $\widehat{p}\widehat{q}\left\lbrack { = \widehat{p}\left( {1 - \widehat{p}}\right) }\right\rbrack$ is maximized at $\widehat{p} = {.5}$ . Thus if $\widehat{p} = \widehat{q} = {.5}$ is used in (7.12), the width will be at most $w$ regardless of what value of $\widehat{p}$ results from the sample. Alternatively, if the investigator believes strongly, based on prior information, that $p \leq {p}_{0} \leq {.5}$ , then ${p}_{0}$ can be used in place of $\widehat{p}$ . A similar comment applies when $p \geq {p}_{0} \geq {.5}$ .

9 The width of the ${95}\% \mathrm{{CI}}$ in Example 7.8 is .258 . The value of $n$ necessary to ensure a width of .10 irrespective of the value of $\widehat{p}$ is

$$
n = \frac{2{\left( {1.96}\right) }^{2}\left( {.25}\right) - {\left( {1.96}\right) }^{2}\left( {.01}\right) \pm \sqrt{4{\left( {1.96}\right) }^{4}\left( {.25}\right) \left( {{.25} - {.01}}\right) + \left( {.01}\right) {\left( {1.96}\right) }^{4}}}{.01} = {380.3}
$$

Thus a sample size of 381 should be used. The expression for $n$ based on the traditional CI gives a slightly larger value of 385.

## One-Sided Confidence Intervals (Confidence Bounds)

The confidence intervals discussed thus far give both a lower confidence bound and an upper confidence bound for the parameter being estimated. In some circumstances, an investigator will want only one of these two types of bounds. For example, a psychologist may wish to calculate a ${95}\%$ upper confidence bound for true average reaction time to a particular stimulus, or a reliability engineer may want only a lower confidence bound for true average lifetime of components of a certain

type. Because the cumulative area under the standard normal curve to the left of 1.645 is .95 ,

$$
P\left( {\frac{\bar{X} - \mu }{S/\sqrt{n}} < {1.645}}\right) \approx {.95}
$$

Manipulating the inequality inside the parentheses to isolate $\mu$ on one side and replacing rv’s by calculated values gives the inequality $\mu > \bar{x} - {1.645s}/\sqrt{n}$ ; the expression on the right is the desired lower confidence bound. Starting with $P\left( {-{1.645} < Z}\right) \approx {.95}$ and manipulating the inequality results in the upper confidence bound. A similar argument gives a one-sided bound associated with any other confidence level.

---

PROPOSITION

---

A large-sample upper confidence bound for $\mu$ is

$$
\mu < \bar{x} + {z}_{\alpha } \cdot \frac{s}{\sqrt{n}}
$$

and a large-sample lower confidence bound for $\mathbf{\mu }$ is

$$
\mu > \bar{x} - {z}_{\alpha } \cdot \frac{s}{\sqrt{n}}
$$

A one-sided confidence bound for $p$ results from replacing ${z}_{\alpha /2}$ by ${z}_{\alpha }$ and $\pm$ by either + or - in the CI formula (7.10) for $p$ . In all cases the confidence level is approximately ${100}\left( {1 - \alpha }\right) \%$ .

EXAMPLE 7.10 Titanium and its alloys have found increasing use in aerospace and automotive applications because of durability and high strength-to-weight ratios. However, machining can be difficult because of low thermal conductivity. The article "Modeling and Multi-Objective Optimization of Process Parameters of Wire Electrical Discharge Machining Using Non-Dominated Sorting Genetic Algorithm-II (J. of Engr. Manuf., 2012: 1186-2001) described an investigation into different settings that impact wire electrical discharge machining of titanium 6-2-4-2. One characteristic of interest was surface roughness $\left( {\mu \mathrm{g}}\right)$ of the metal after machining. A sample of 54 surface roughness observations resulted in a sample mean roughness of 1.9042 and a sample standard deviation of .1455 . An upper confidence bound for true average roughness $\mu$ with confidence level ${95}\%$ requires ${z}_{.05} = {1.645}$ (not the value ${z}_{.025} = {1.96}$ needed for a two-sided CI). The bound is

$$
{1.9042} + \left( {1.645}\right) \cdot \frac{\left( {.1455}\right) }{\sqrt{54}} = {1.9042} + {.0326} = {1.9368}
$$

Thus we estimate with a confidence level of roughly ${95}\%$ that $\mu < {1.9368}$ .

## EXERCISES Section 7.2 (12-27)

12. The following observations are lifetimes (days) subse- $\begin{array}{lllllllllll} {115} & {181} & {255} & {418} & {441} & {461} & {516} & {739} & {743} & {789} & {807} \end{array}$ quent to diagnosis for individuals suffering from blood $\begin{array}{lllllllllll} {865} & {924} & {983} & {1025} & {1062} & {1063} & {1165} & {1191} & {1222} & {1222} & {1251} \end{array}$ cancer ("A Goodness of Fit Approach to the Class of $\begin{array}{lllllllllll} {1277} & {1290} & {1357} & {1369} & {1408} & {1455} & {1478} & {1519} & {1578} & {1578} & {1599} \end{array}$ $\begin{array}{llllllllll} {1603} & {1605} & {1696} & {1735} & {1799} & {1815} & {1852} & {1899} & {1925} & {1965} \end{array}$

Life Distributions with Unknown Age," Quality and a. Can a confidence interval for true average lifetime be Reliability Engr. Intl., 2012: 761-766): calculated without assuming anything about the

Copyright 2016 Congage Learning, All Rights Reserved, May not be copied, scanned, or duplicated, in whole or in part. Due to electronic rights, some third party content may be suppressed from the eBook and/or eChapter(s). Editorial review has deemed that any suppressed content does not materially affect the overall learning experience. Congage Learning reserves the right to remove additional content at any time if subsequent rights restrictions require it. nature of the lifetime distribution? Explain your reasoning. [Note: A normal probability plot of the data exhibits a reasonably linear pattern.]

b. Calculate and interpret a confidence interval with a ${99}\%$ confidence level for true average lifetime. [Hint: $\bar{x} = {1191.6}$ and $s = {506.6}$ .]

13. The article "Gas Cooking, Kitchen Ventilation, and Exposure to Combustion Products" (Indoor Air, 2006: 65-73) reported that for a sample of 50 kitchens with gas cooking appliances monitored during a one-week period, the sample mean ${\mathrm{{CO}}}_{2}$ level (ppm) was 654.16, and the sample standard deviation was 164.43.

a. Calculate and interpret a ${95}\%$ (two-sided) confidence interval for true average ${\mathrm{{CO}}}_{2}$ level in the population of all homes from which the sample was selected.

b. Suppose the investigators had made a rough guess of 175 for the value of $s$ before collecting data. What sample size would be necessary to obtain an interval width of ${50}\mathrm{{ppm}}$ for a confidence level of ${95}\%$ ?

14. The negative effects of ambient air pollution on children's lung function has been well established, but less research is available about the impact of indoor air pollution. The authors of "Indoor Air Pollution and Lung Function Growth Among Children in Four Chinese Cities" (Indoor Air, 2012: 3-11) investigated the relationship between indoor air-pollution metrics and lung function growth among children ages 6-13 years living in four Chinese cities. For each subject in the study, the authors measured an important lung-capacity index known as ${\mathrm{{FEV}}}_{1}$ , the forced volume (in $\mathrm{{ml}}$ ) of air that is exhaled in 1 second. Higher ${\mathrm{{FEV}}}_{1}$ values are associated with greater lung capacity. Among the children in the study, 514 came from households that used coal for cooking or heating or both. Their ${\mathrm{{FEV}}}_{1}$ mean was 1427 with a standard deviation of 325. (A complex statistical procedure was used to show that burning coal had a clear negative effect on mean ${\mathrm{{FEV}}}_{1}$ levels.)

a. Calculate and interpret a ${95}\%$ (two-sided) confidence interval for true average ${\mathrm{{FEV}}}_{1}$ level in the population of all children from which the sample was selected. Does it appear that the parameter of interest has been accurately estimated?

b. Suppose the investigators had made a rough guess of 320 for the value of $s$ before collecting data. What sample size would be necessary to obtain an interval width of ${50}\mathrm{{ml}}$ for a confidence level of ${95}\%$ ?

15. Determine the confidence level for each of the following large-sample one-sided confidence bounds:

a. Upper bound: $\bar{x} + {.84s}/\sqrt{n}$

b. Lower bound: $\bar{x} - {2.05s}/\sqrt{n}$

c. Upper bound: $\bar{x} + {.67s}/\sqrt{n}$

16. The alternating current (AC) breakdown voltage of an insulating liquid indicates its dielectric strength. The article "Testing Practices for the AC Breakdown Voltage Testing of Insulation Liquids" (IEEE

Electrical Insulation Magazine, 1995: 21-26) gave the accompanying sample observations on breakdown voltage $\left( \mathrm{{kV}}\right)$ of a particular circuit under certain conditions.

$\begin{array}{llllllllllllllll} {62} & {50} & {53} & {57} & {41} & {53} & {55} & {61} & {59} & {64} & {50} & {53} & {64} & {62} & {50} & {68} \end{array}$

$\begin{array}{llllllllllllllll} {54} & {55} & {57} & {50} & {55} & {50} & {56} & {55} & {46} & {55} & {53} & {54} & {52} & {47} & {47} & {55} \end{array}$

57 48 63 57 57 55 53 59 53 52 50 55 60 50 56 58

a. Construct a boxplot of the data and comment on interesting features.

b. Calculate and interpret a ${95}\% \mathrm{{CI}}$ for true average breakdown voltage $\mu$ . Does it appear that $\mu$ has been precisely estimated? Explain.

c. Suppose the investigator believes that virtually all values of breakdown voltage are between 40 and 70 . What sample size would be appropriate for the ${95}\%$ $\mathrm{{CI}}$ to have a width of $2\mathrm{{kV}}$ (so that $\mu$ is estimated to within $1\mathrm{{kV}}$ with ${95}\%$ confidence)?

17. Exercise 1.13 gave a sample of ultimate tensile strength observations (ksi). Use the accompanying descriptive statistics output from Minitab to calculate a ${99}\%$ lower confidence bound for true average ultimate tensile strength, and interpret the result.

<table><thead><tr><th>$\mathrm{N}$</th><th>Mean</th><th>Median</th><th>TrMean</th><th>StDev</th><th>SE</th><th>Mean</th></tr></thead><tr><td>153</td><td>135.39</td><td>135.40</td><td>135.41</td><td>4.59</td><td></td><td>0.37</td></tr><tr><td>Minimum</td><td></td><td>Maximum</td><td>Q1</td><td>Q3</td><td></td><td></td></tr><tr><td></td><td>122.20</td><td>147.70</td><td>132.95</td><td>138.25</td><td></td><td></td></tr></table>

18. The U.S. Army commissioned a study to assess how deeply a bullet penetrates ceramic body armor (“Testing Body Armor Materials for Use by the U.S. Army-Phase III," 2012). In the standard test, a cylindrical clay model is layered under the armor vest. A projectile is then fired, causing an indentation in the clay. The deepest impression in the clay is measured as an indication of survivability of someone wearing the armor. Here is data from one testing organization under particular experimental conditions; measurements (in $\mathrm{{mm}}$ ) were made using a manually controlled digital caliper:

<table><tr><td>22.4</td><td>23.6</td><td>24.0</td><td>24.9</td><td>25.5</td><td>25.6</td></tr><tr><td>25.8</td><td>26.1</td><td>26.4</td><td>26.7</td><td>27.4</td><td>27.6</td></tr><tr><td>28.3</td><td>29.0</td><td>29.1</td><td>29.6</td><td>29.7</td><td>29.8</td></tr><tr><td>29.9</td><td>30.0</td><td>30.4</td><td>30.5</td><td>30.7</td><td>30.7</td></tr><tr><td>31.0</td><td>31.0</td><td>31.4</td><td>31.6</td><td>31.7</td><td>31.9</td></tr><tr><td>31.9</td><td>32.0</td><td>32.1</td><td>32.4</td><td>32.5</td><td>32.5</td></tr><tr><td>32.6</td><td>32.9</td><td>33.1</td><td>33.3</td><td>33.5</td><td>33.5</td></tr><tr><td>33.5</td><td>33.5</td><td>33.6</td><td>33.6</td><td>33.8</td><td>33.9</td></tr><tr><td>34.1</td><td>34.2</td><td>34.6</td><td>34.6</td><td>35.0</td><td>35.2</td></tr><tr><td>35.2</td><td>35.4</td><td>35.4</td><td>35.4</td><td>35.5</td><td>35.7</td></tr><tr><td>35.8</td><td>36.0</td><td>36.0</td><td>36.0</td><td>36.1</td><td>36.1</td></tr><tr><td>36.2</td><td>36.4</td><td>36.6</td><td>37.0</td><td>37.4</td><td>37.5</td></tr><tr><td>37.5</td><td>38.0</td><td>38.7</td><td>38.8</td><td>39.8</td><td>41.0</td></tr><tr><td>42.0</td><td>42.1</td><td>44.6</td><td>48.3</td><td>55.0</td><td></td></tr></table>

a. Construct a boxplot of the data and comment on interesting features.

b. Construct a normal probability plot. Is it plausible that impression depth is normally distributed? Is a normal distribution assumption needed in order to calculate a confidence interval or bound for the true average depth $\mu$ using the foregoing data? Explain.

c. Use the accompanying Minitab output as a basis for calculating and interpreting an upper confidence bound for $\mu$ with a confidence level of ${99}\%$ . Variable Count Mean SE Mean StDev $\begin{array}{lllll} \text{ Bepth } & {83} & {33.370} & {0.578} & {5.268} \end{array}$ Q1 Median Q3 IQR $\begin{array}{llll} {30.400} & {33.500} & {36.000} & {5.600} \end{array}$

19. The article "Limited Yield Estimation for Visual Defect Sources" (IEEE Trans. on Semiconductor Manuf., 1997: 17-23) reported that, in a study of a particular wafer inspection process, 356 dies were examined by an inspection probe and 201 of these passed the probe. Assuming a stable process, calculate a ${95}\%$ (two-sided) confidence interval for the proportion of all dies that pass the probe.

20. TV advertising agencies face increasing challenges in reaching audience members because viewing TV programs via digital streaming is gaining in popularity. The Harris poll reported on November 13, 2012, that 53% of 2343 American adults surveyed said they have watched digitally streamed TV programming on some type of device.

a. Calculate and interpret a confidence interval at the ${99}\%$ confidence level for the proportion of all adult Americans who watched streamed programming up to that point in time.

b. What sample size would be required for the width of a ${99}\% \mathrm{{CI}}$ to be at most .05 irrespective of the value of $\widehat{p}$ ?

21. In a sample of 1000 randomly selected consumers who had opportunities to send in a rebate claim form after purchasing a product, 250 of these people said they never did so ("Rebates: Get What You Deserve," Consumer Reports, May 2009: 7). Reasons cited for their behavior included too many steps in the process, amount too small, missed deadline, fear of being placed on a mailing list, lost receipt, and doubts about receiving the money. Calculate an upper confidence bound at the ${95}\%$ confidence level for the true proportion of such consumers who never apply for a rebate. Based on this bound, is there compelling evidence that the true proportion of such consumers is smaller than 1/3? Explain your reasoning.

22. The technology underlying hip replacements has changed as these operations have become more popular (over 250,000 in the United States in 2008). Starting in 2003, highly durable ceramic hips were marketed. Unfortunately, for too many patients the increased durability has been counterbalanced by an increased incidence of squeaking. The May 11, 2008, issue of the New York Times reported that in one study of 143 individuals who received ceramic hips between 2003 and 2005, 10 of the hips developed squeaking.

a. Calculate a lower confidence bound at the ${95}\%$ confidence level for the true proportion of such hips that develop squeaking.

b. Interpret the ${95}\%$ confidence level used in (a).

23. The Pew Forum on Religion and Public Life reported on Dec. 9, 2009, that in a survey of 2003 American adults, ${25}\%$ said they believed in astrology.

a. Calculate and interpret a confidence interval at the ${99}\%$ confidence level for the proportion of all adult Americans who believe in astrology.

b. What sample size would be required for the width of a ${99}\% \mathrm{{CI}}$ to be at most .05 irrespective of the value of $\widehat{p}$ ?

24. A sample of 56 research cotton samples resulted in a sample average percentage elongation of 8.17 and a sample standard deviation of 1.42 (“An Apparent Relation Between the Spiral Angle $\phi$ , the Percent Elongation ${E}_{1}$ , and the Dimensions of the Cotton Fiber," Textile Research J., 1978: 407-410). Calculate a ${95}\%$ large-sample CI for the true average percentage elongation $\mu$ . What assumptions are you making about the distribution of percentage elongation?

25. A state legislator wishes to survey residents of her district to see what proportion of the electorate is aware of her position on using state funds to pay for abortions.

a. What sample size is necessary if the ${95}\% \mathrm{{CI}}$ for $p$ is to have a width of at most .10 irrespective of $p$ ?

b. If the legislator has strong reason to believe that at least $2/3$ of the electorate know of her position, how large a sample size would you recommend?

26. The superintendent of a large school district, having once had a course in probability and statistics, believes that the number of teachers absent on any given day has a Poisson distribution with parameter $\mu$ . Use the accompanying data on absences for 50 days to obtain a large-sample CI for $\mu$ . [Hint: The mean and variance of a Poisson variable both equal $\mu$ , so

$$
Z = \frac{\bar{X} - \mu }{\sqrt{\mu /n}}
$$

has approximately a standard normal distribution. Now proceed as in the derivation of the interval for $p$ by making a probability statement (with probability $1 - \alpha$ ) and solving the resulting inequalities for $\mu$ - see the argument just after (7.10).]

Number of

<table><tr><td>absences</td><td>0</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td><td>9</td><td>10</td></tr><tr><td>Frequency</td><td>1</td><td>4</td><td>8</td><td>10</td><td>8</td><td>7</td><td>5</td><td>3</td><td>2</td><td>1</td><td></td></tr></table>

27. Reconsider the CI (7.10) for $p$ , and focus on a confidence level of ${95}\%$ . Show that the confidence limits agree quite well with those of the traditional interval (7.11) once two successes and two failures have been appended to the sample [i.e.,(7.11) based on $x + {2S}$ ’s in $n + 4$ trials]. [Hint: ${1.96} \approx 2$ . Note: Agresti and Coull showed that this adjustment of the traditional interval also has an actual confidence level close to the nominal level.]

## 7.3 Intervals Based on a Normal Population Distribution

The CI for $\mu$ presented in Section 7.2 is valid provided that $n$ is large. The resulting interval can be used whatever the nature of the population distribution. The CLT cannot be invoked, however, when $n$ is small. In this case, one way to proceed is to make a specific assumption about the form of the population distribution and then derive a CI tailored to that assumption. For example, we could develop a CI for $\mu$ when the population is described by a gamma distribution, another interval for the case of a Weibull distribution, and so on. Statisticians have indeed carried out this program for a number of different distributional families. Because the normal distribution is more frequently appropriate as a population model than is any other type of distribution, we will focus here on a CI for this situation.

ASSUMPTION The population of interest is normal, so that ${X}_{1},\ldots ,{X}_{n}$ constitutes a random sample from a normal distribution with both $\mu$ and $\sigma$ unknown.

The key result underlying the interval in Section 7.2 was that for large $n$ , the rv $Z = \left( {\bar{X} - \mu }\right) /\left( {S/\sqrt{n}}\right)$ has approximately a standard normal distribution. When $n$ is small, the additional variability in the denominator implies that the probability distribution of $\left( {\bar{X} - \mu }\right) /\left( {S/\sqrt{n}}\right)$ will be more spread out than the standard normal distribution. The result on which inferences are based introduces a new family of probability distributions called $t$ distributions.

## THEOREM

When $\bar{X}$ is the mean of a random sample of size $n$ from a normal distribution with mean $\mu$ , the rv

$$
T = \frac{\bar{X} - \mu }{S/\sqrt{n}} \tag{7.13}
$$

has a probability distribution called a $t$ distribution with $n - 1$ degrees of freedom (df).

## Properties of $t$ Distributions

Before applying this theorem, a discussion of properties of $t$ distributions is in order. Although the variable of interest is still $\left( {\bar{X} - \mu }\right) /\left( {S/\sqrt{n}}\right)$ , we now denote it by $T$ to emphasize that it does not have a standard normal distribution when $n$ is small. Recall that a normal distribution is governed by two parameters; each different choice of $\mu$ in combination with $\sigma$ gives a particular normal distribution. Any particular $t$ distribution results from specifying the value of a single parameter, called the number of degrees of freedom, abbreviated df. We'll denote this parameter by the Greek letter $\nu$ . Possible values of $\nu$ are the positive integers 1, $2,3,\ldots$ So there is a $t$ distribution with $1\mathrm{{df}}$ , another with $2\mathrm{{df}}$ , yet another with $3\mathrm{{df}}$ , and so on.

For any fixed value of $\nu$ , the density function that specifies the associated $t$ curve is even more complicated than the normal density function. Fortunately, we need concern ourselves only with several of the more important features of these curves.

## Properties of $t$ Distributions

Let ${t}_{\nu }$ denote the $t$ distribution with $\nu$ df.

1. Each ${t}_{\nu }$ curve is bell-shaped and centered at 0 .

2. Each ${t}_{\nu }$ curve is more spread out than the standard normal $\left( z\right)$ curve.

3. As $\nu$ increases, the spread of the corresponding ${t}_{\nu }$ curve decreases.

4. As $\nu \rightarrow \infty$ , the sequence of ${t}_{\nu }$ curves approaches the standard normal curve (so the $z$ curve is often called the $t$ curve with $\mathrm{{df}} = \infty$ ).

Figure 7.7 illustrates several of these properties for selected values of $\nu$ .

![01927a02-a1da-7086-ba87-2208e017bc0f_20_733_898_695_346_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_20_733_898_695_346_0.jpg)

Figure ${7.7}\;{t}_{\nu }$ and $z$ curves

The number of df for $T$ in (7.13) is $n - 1$ because, although $S$ is based on the $n$ deviations ${X}_{1} - \bar{X},\ldots ,{X}_{n} - \bar{X},\sum \left( {{X}_{i} - \bar{X}}\right) = 0$ implies that only $n - 1$ of these are "freely determined." The number of df for a $t$ variable is the number of freely determined deviations on which the estimated standard deviation in the denominator of $T$ is based.

The use of $t$ distribution in making inferences requires notation for capturing $t$ -curve tail areas analogous to ${z}_{\alpha }$ for the $z$ curve. You might think that ${t}_{\alpha }$ would do the trick. However, the desired value depends not only on the tail area captured but also on df.

## NOTATION

Let ${t}_{\alpha ,\nu } =$ the number on the measurement axis for which the area under the

$t$ curve with $\nu$ df to the right of ${t}_{\alpha ,\nu }$ is $\alpha ;{t}_{\alpha ,\nu }$ is called a $t$ critical value.

For example, ${t}_{{.05},6}$ is the $t$ critical value that captures an upper-tail area of .05 under the $t$ curve with 6 df. The general notation is illustrated in Figure 7.8. Because $t$ curves are symmetric about zero, $- {t}_{\alpha ,\nu }$ captures lower-tail area $\alpha$ . Appendix Table A. 5 gives ${t}_{\alpha ,\nu }$ for selected values of $\alpha$ and $\nu$ . This table also appears inside the back cover. The columns of the table correspond to different values of $\alpha$ . To obtain ${t}_{{.05},{15}}$ , go to the $\alpha = {.05}$ column, look down to the $\nu = {15}$ row, and read ${t}_{{.05},{15}} = {1.753}$ . Similarly, ${t}_{{.05},{22}} = {1.717}$ (.05 column, $\nu = {22}$ row), and ${t}_{{.01},{22}} = {2.508}$ .

![01927a02-a1da-7086-ba87-2208e017bc0f_21_967_188_450_220_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_21_967_188_450_220_0.jpg)

Figure 7.8 Illustration of a $t$ critical value

The values of ${t}_{\alpha ,\nu }$ exhibit regular behavior as we move across a row or down a column. For fixed $\nu ,{t}_{\alpha ,\nu }$ increases as $\alpha$ decreases, since we must move farther to the right of zero to capture area $\alpha$ in the tail. For fixed $\alpha$ , as $\nu$ is increased (i.e., as we look down any particular column of the $t$ table) the value of ${t}_{\alpha ,\nu }$ decreases. This is because a larger value of $\nu$ implies a $t$ distribution with smaller spread, so it is not necessary to go so far from zero to capture tail area $\alpha$ . Furthermore, ${t}_{\alpha ,\nu }$ decreases more slowly as $\nu$ increases. Consequently, the table values are shown in increments of 2 between 30 df and 40 df and then jump to $\nu = {50},{60},{120}$ , and finally $\infty$ . Because ${t}_{\infty }$ is the standard normal curve, the familiar ${z}_{\alpha }$ values appear in the last row of the table. The rule of thumb suggested earlier for use of the large-sample CI (if $n > {40}$ ) comes from the approximate equality of the standard normal and $t$ distributions for $\nu \geq {40}$ .

## The One-Sample $t$ Confidence Interval

The standardized variable $T$ has a $t$ distribution with $n - 1\mathrm{{df}}$ , and the area under the corresponding $t$ density curve between $- {t}_{\alpha /2, n - 1}$ and ${t}_{\alpha /2, n - 1}$ is $1 - \alpha$ (area $\alpha /2$ lies in each tail), so

$$
P\left( {-{t}_{\alpha /2, n - 1} < T < {t}_{\alpha /2, n - 1}}\right) = 1 - \alpha \tag{7.14}
$$

Expression (7.14) differs from expressions in previous sections in that $T$ and ${t}_{\alpha /2, n - 1}$ are used in place of $Z$ and ${z}_{\alpha /2}$ , but it can be manipulated in the same manner to obtain a confidence interval for $\mu$ .

---

PROPOSITION

---

Let $\bar{x}$ and $s$ be the sample mean and sample standard deviation computed from the results of a random sample from a normal population with mean $\mu$ . Then a ${100}\left( {1 - \alpha }\right) \%$ confidence interval for $\mu$ is

$$
\left( {\bar{x} - {t}_{\alpha /2, n - 1} \cdot \frac{s}{\sqrt{n}},\bar{x} + {t}_{\alpha /2, n - 1} \cdot \frac{s}{\sqrt{n}}}\right) \tag{7.15}
$$

or, more compactly, $\bar{x} \pm {t}_{\alpha /2, n - 1} \cdot s/\sqrt{n}$ .

An upper confidence bound for $\mu$ is

$$
\bar{x} + {t}_{\alpha , n - 1} \cdot \frac{s}{\sqrt{n}}
$$

and replacing + by - in this latter expression gives a lower confidence bound for $\mathbf{\mu }$ , both with confidence level ${100}\left( {1 - \alpha }\right) \%$ .

EXAMPLE 7.11 Even as traditional markets for sweetgum lumber have declined, large section solid timbers traditionally used for construction bridges and mats have become increasingly scarce. The article "Development of Novel Industrial Laminated Planks from Sweetgum Lumber" (J. of Bridge Engr., 2008: 64-66) described the manufacturing and testing of composite beams designed to add value to low-grade sweetgum lumber.

Here is data on the modulus of rupture (psi; the article contained summary data expressed in $\mathrm{{MPa}}$ ):

<table><tr><td>6807.99</td><td>7637.06</td><td>6663.28</td><td>6165.03</td><td>6991.41</td><td>6992.23</td></tr><tr><td>6981.46</td><td>7569.75</td><td>7437.88</td><td>6872.39</td><td>7663.18</td><td>6032.28</td></tr><tr><td>6906.04</td><td>6617.17</td><td>6984.12</td><td>7093.71</td><td>7659.50</td><td>7378.61</td></tr><tr><td>7295.54</td><td>6702.76</td><td>7440.17</td><td>8053.26</td><td>8284.75</td><td>7347.95</td></tr><tr><td>7422.69</td><td>7886.87</td><td>6316.67</td><td>7713.65</td><td>7503.33</td><td>7674.99</td></tr></table>

Figure 7.9 shows a normal probability plot from the R software. The straightness of the pattern in the plot provides strong support for assuming that the population distribution of MOR is at least approximately normal.

![01927a02-a1da-7086-ba87-2208e017bc0f_22_729_681_712_620_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_22_729_681_712_620_0.jpg)

Figure 7.9 A normal probability plot of the modulus of rupture data

The sample mean and sample standard deviation are 7203.191 and 543.5400, respectively (for anyone bent on doing hand calculation, the computational burden is eased a bit by subtracting 6000 from each $x$ value to obtain ${y}_{i} = {x}_{i} - {6000}$ ; then $\sum {y}_{i} = {36},{095.72}$ and $\sum {y}_{i}^{2} = {51},{997},{668.77}$ , from which $\bar{y} = {1203.191}$ and ${s}_{y} = {s}_{x}$ as given).

Let's now calculate a confidence interval for true average MOR using a confidence level of ${95}\%$ . The CI is based on $n - 1 = {29}$ degrees of freedom, so the necessary $t$ critical value is ${t}_{{.025},{29}} = {2.045}$ . The interval estimate is now

$$
\bar{x} \pm {t}_{{.025},{29}} \cdot \frac{s}{\sqrt{n}} = {7203.191} \pm \left( {2.045}\right) \cdot \frac{543.5400}{\sqrt{30}}
$$

$$
= {7203.191} \pm {202.938} = \left( {{7000.253},{7406.129}}\right)
$$

We estimate that ${7000.253} < \mu < {7406.129}$ with ${95}\%$ confidence. If we use the same formula on sample after sample, in the long run ${95}\%$ of the calculated intervals will contain $\mu$ . Since the value of $\mu$ is not available, we don’t know whether the calculated interval is one of the "good" 95% or the "bad" 5%. Even with the moderately large sample size, our interval is rather wide. This is a consequence of the substantial amount of sample variability in MOR values.

A lower ${95}\%$ confidence bound would result from retaining only the lower confidence limit (the one with -) and replacing 2.045 with ${t}_{{.05},{29}} = {1.699}$ .

Unfortunately, it is not easy to select $n$ to control the width of the $t$ interval. This is because the width involves the unknown (before the data is collected) $s$ and because $n$ enters not only through $1/\sqrt{n}$ but also through ${t}_{\alpha /2, n - 1}$ . As a result, an appropriate $n$ can be obtained only by trial and error.

In Chapter 15, we will discuss a small-sample CI for $\mu$ that is valid provided only that the population distribution is symmetric, a weaker assumption than normality. However, when the population distribution is normal, the $t$ interval tends to be narrower than would be any other interval with the same confidence level.

## A Prediction Interval for a Single Future Value

In many applications, the objective is to predict a single value of a variable to be observed at some future time, rather than to estimate the mean value of that variable.

EXAMPLE 7.12 Consider the following sample of fat content (in percentage) of $n = {10}$ randomly selected hot dogs ("Sensory and Mechanical Assessment of the Quality of Frankfurters," J. of Texture Studies, 1990: 395-409):

$$
\begin{array}{llllllllll} {25.2} & {21.3} & {22.8} & {17.0} & {29.8} & {21.0} & {25.5} & {16.0} & {20.9} & {19.5} \end{array} \tag{19.5}
$$

Assuming that these were selected from a normal population distribution, a ${95}\%$ CI for (interval estimate of) the population mean fat content is

$$
\bar{x} \pm {t}_{{.025},9} \cdot \frac{s}{\sqrt{n}} = {21.90} \pm {2.262} \cdot \frac{4.134}{\sqrt{10}} = {21.90} \pm {2.96}
$$

$$
= \left( {{18.94},{24.86}}\right)
$$

Suppose, however, you are going to eat a single hot dog of this type and want a prediction for the resulting fat content. A point prediction, analogous to a point estimate, is just $\bar{x} = {21.90}$ . This prediction unfortunately gives no information about reliability or precision.

The general setup is as follows: We have available a random sample ${X}_{1},{X}_{2},\ldots ,{X}_{n}$ from a normal population distribution, and wish to predict the value of ${X}_{n + 1}$ , a single future observation (e.g., the lifetime of a single lightbulb to be purchased or the fuel efficiency of a single vehicle to be rented). A point predictor is $\bar{X}$ , and the resulting prediction error is $\bar{X} - {X}_{n + 1}$ . The expected value of the prediction error is

$$
E\left( {\bar{X} - {X}_{n + 1}}\right) = E\left( \bar{X}\right) - E\left( {X}_{n + 1}\right) = \mu - \mu = 0
$$

Since ${X}_{n + 1}$ is independent of ${X}_{1},\ldots ,{X}_{n}$ , it is independent of $\bar{X}$ , so the variance of the prediction error is

$$
V\left( {\bar{X} - {X}_{n + 1}}\right) = V\left( \bar{X}\right) + V\left( {X}_{n + 1}\right) = \frac{{\sigma }^{2}}{n} + {\sigma }^{2} = {\sigma }^{2}\left( {1 + \frac{1}{n}}\right)
$$

The prediction error is normally distributed because it is a linear combination of independent, normally distributed rv's. Thus

$$
Z = \frac{\left( {\bar{X} - {X}_{n + 1}}\right) - 0}{\sqrt{{\sigma }^{2}\left( {1 + \frac{1}{n}}\right) }} = \frac{\bar{X} - {X}_{n + 1}}{\sqrt{{\sigma }^{2}\left( {1 + \frac{1}{n}}\right) }}
$$

has a standard normal distribution. It can be shown that replacing $\sigma$ by the sample standard deviation $S$ (of ${X}_{1},\ldots ,{X}_{n}$ ) results in

$$
T = \frac{\bar{X} - {X}_{n + 1}}{S\sqrt{1 + \frac{1}{n}}} \sim t\text{ distribution with }n - 1\mathrm{{df}}
$$

Manipulating this $T$ variable as $T = \left( {\bar{X} - \mu }\right) /\left( {S/\sqrt{n}}\right)$ was manipulated in the development of a CI gives the following result.

---

PROPOSITION

---

A prediction interval (PI) for a single observation to be selected from a normal population distribution is

$$
\bar{x} \pm {t}_{\alpha /2, n - 1} \cdot s\sqrt{1 + \frac{1}{n}} \tag{7.16}
$$

The prediction level is ${100}\left( {1 - \alpha }\right) \%$ . A lower prediction bound results from replacing ${t}_{\alpha /2}$ by ${t}_{\alpha }$ and discarding the + part of (7.16); a similar modification gives an upper prediction bound.

The interpretation of a ${95}\%$ prediction level is similar to that of a ${95}\%$ confidence level. If the interval (7.16) is calculated for sample after sample and after each calculation ${\mathrm{X}}_{n + 1}$ is observed, in the long run ${95}\%$ of these intervals will include the corresponding future values.

---

EXAMPLE 7.13

(Example 7.12 continued)

---

With $n = {10},\bar{x} = {21.90}, s = {4.134}$ , and ${t}_{{.025},9} = {2.262}$ , a ${95}\%$ PI for the fat content of a single hot dog is

$$
{21.90} \pm \left( {2.262}\right) \left( {4.134}\right) \sqrt{1 + \frac{1}{10}} = {21.90} \pm {9.81}
$$

$$
= \left( {{12.09},{31.71}}\right)
$$

This interval is quite wide, indicating substantial uncertainty about fat content. Notice that the width of the PI is more than three times that of the CI.

The error of prediction is $\bar{X} - {X}_{n + 1}$ , a difference between two random variables, whereas the estimation error is $\bar{X} - \mu$ , the difference between a random variable and a fixed (but unknown) value. The PI is wider than the CI because there is more variability in the prediction error (due to ${X}_{n + 1}$ ) than in the estimation error. In fact, as $n$ gets arbitrarily large, the CI shrinks to the single value $\mu$ , and the PI approaches $\mu \pm {z}_{\alpha /2} \cdot \sigma$ . There is uncertainty about a single $X$ value even when there is no need to estimate.

## Tolerance Intervals

Consider a population of automobiles of a certain type, and suppose that under specified conditions, fuel efficiency (mpg) has a normal distribution with $\mu = {30}$ and $\sigma = 2$ . Then since the interval from -1.645 to 1.645 captures ${90}\%$ of the area under the $z$ curve, ${90}\%$ of all these automobiles will have fuel efficiency values between $\mu - {1.645\sigma } = {26.71}$ and $\mu + {1.645\sigma } = {33.29}$ . But what if the values of $\mu$ and $\sigma$ are not known? We can take a sample of size $n$ , determine the fuel efficiencies, $\bar{x}$ and $s$ , and form the interval whose lower limit is $\bar{x} - {1.645s}$ and whose upper limit is $\bar{x} + {1.645s}$ . However, because of sampling variability in the estimates of $\mu$ and $\sigma$ , there is a good chance that the resulting interval will include less than ${90}\%$ of the population values. Intuitively, to have an a priori ${95}\%$ chance of the resulting interval including at least ${90}\%$ of the population values, when $\bar{x}$ and $s$ are used in place of $\mu$ and $\sigma$ we should also replace 1.645 by some larger number. For example, when $n = {20}$ , the value 2.310 is such that we can be ${95}\%$ confident that the interval $\bar{x} \pm {2.310s}$ will include at least ${90}\%$ of the fuel efficiency values in the population.

Let $k$ be a number between 0 and 100 . A tolerance interval for capturing at least $k\%$ of the values in a normal population distribution with a confidence level ${95}\%$ has the form

$$
\bar{x} \pm \text{(tolerance critical value)} \cdot s
$$

Tolerance critical values for $k = {90},{95}$ , and 99 in combination with various sample sizes are given in Appendix Table A.6. This table also includes critical values for a confidence level of ${99}\%$ (these values are larger than the corresponding ${95}\%$ values). Replacing $\pm$ by + gives an upper tolerance bound, and using - in place of $\pm$ results in a lower tolerance bound. Critical values for obtaining these one-sided bounds also appear in Appendix Table A.6.

EXAMPLE 7.14 As part of a larger project to study the behavior of stressed-skin panels, a structural component being used extensively in North America, the article "Time-Dependent Bending Properties of Lumber" (J. of Testing and Eval., 1996: 187-193) reported on various mechanical properties of Scotch pine lumber specimens. Consider the following observations on modulus of elasticity $\left( \mathrm{{MPa}}\right)$ obtained 1 minute after loading in a certain configuration:

$$
\text{10,490 16,620 17,300 15,480 12,970 17,260 13,400 13,900}
$$

$$
\text{13,630 13,260 14,370 11,700 15,470 17,840 14,070 14,760}
$$

There is a pronounced linear pattern in a normal probability plot of the data. Relevant summary quantities are $n = {16},\bar{x} = {14},{532.5}, s = {2055.67}$ . For a confidence level of ${95}\%$ , a two-sided tolerance interval for capturing at least ${95}\%$ of the modulus of elasticity values for specimens of lumber in the population sampled uses the tolerance critical value of 2.903 . The resulting interval is

$$
{14},{532.5} \pm \left( {2.903}\right) \left( {2055.67}\right) = {14},{532.5} \pm {5967.6} = \left( {8,{564.9},{20},{500.1}}\right)
$$

We can be highly confident that at least ${95}\%$ of all lumber specimens have modulus of elasticity values between 8,564.9 and 20,500.1.

The ${95}\%$ CI for $\mu$ is $\left( {{13},{437.3},{15},{627.7}}\right)$ , and the ${95}\%$ prediction interval for the modulus of elasticity of a single lumber specimen is $\left( {{10},{017.0},{19},{048.0}}\right)$ . Both the prediction interval and the tolerance interval are substantially wider than the confidence interval.

## Intervals Based on Nonnormal Population Distributions

The one-sample $t\mathrm{{CI}}$ for $\mu$ is robust to small or even moderate departures from normality unless $n$ is quite small. By this we mean that if a critical value for ${95}\%$ confidence, for example, is used in calculating the interval, the actual confidence level will be reasonably close to the nominal ${95}\%$ level. If, however, $n$ is small and the population distribution is highly nonnormal, then the actual confidence level may be considerably different from the one you think you are using when you obtain a particular critical value from the $t$ table. It would certainly be distressing to believe that your confidence level is about ${95}\%$ when in fact it was really more like ${88}\%$ ! The bootstrap technique, introduced in Section 7.1, has been found to be quite successful at estimating parameters in a wide variety of nonnormal situations.

In contrast to the confidence interval, the validity of the prediction and tolerance intervals described in this section is closely tied to the normality assumption. These latter intervals should not be used in the absence of compelling evidence for normality. The excellent reference Statistical Intervals, cited in the bibliography at the end of this chapter, discusses alternative procedures of this sort for various other situations. EXERCISES Section 7.3 (28-41)

28. Determine the values of the following quantities:

a. ${t}_{{.1},{15}}\;$ b. ${t}_{{.05},{15}}\;$ c. ${t}_{{.05},{25}}\;$ d. ${t}_{{.05},{40}}\;$ e. ${t}_{{.005},{40}}$

29. Determine the $t$ critical value(s) that will capture the desired $t$ -curve area in each of the following cases:

a. Central area $= {.95},\mathrm{{df}} = {10}$

b. Central area $= {.95},\mathrm{{df}} = {20}$

c. Central area $= {.99},\mathrm{{df}} = {20}$

d. Central area $= {.99},\mathrm{{df}} = {50}$

e. Upper-tail area $= {.01},\mathrm{{df}} = {25}$

f. Lower-tail area $= {.025},\mathrm{{df}} = 5$

30. Determine the $t$ critical value for a two-sided confidence interval in each of the following situations:

a. Confidence level $= {95}\% ,\mathrm{{df}} = {10}$

b. Confidence level $= {95}\% ,\mathrm{{df}} = {15}$

c. Confidence level $= {99}\% ,\mathrm{{df}} = {15}$

d. Confidence level $= {99}\% , n = 5$

e. Confidence level $= {98}\% ,\mathrm{{df}} = {24}$

f. Confidence level $= {99}\% , n = {38}$

31. Determine the $t$ critical value for a lower or an upper confidence bound for each of the situations described in Exercise 30.

32. According to the article "Fatigue Testing of Condoms" (Polymer Testing, 2009: 567-571), "tests currently used for condoms are surrogates for the challenges they face in use," including a test for holes, an inflation test, a package seal test, and tests of dimensions and lubricant quality (all fertile territory for the use of statistical methodology!). The investigators developed a new test that adds cyclic strain to a level well below breakage and determines the number of cycles to break. A sample of 20 condoms of one particular type resulted in a sample mean number of 1584 and a sample standard deviation of 607. Calculate and interpret a confidence interval at the ${99}\%$ confidence level for the true average number of cycles to break. [Note: The article presented the results of hypothesis tests based on the $t$ distribution; the validity of these depends on assuming normal population distributions.]

33. The article "Measuring and Understanding the Aging of Kraft Insulating Paper in Power Transformers" (IEEE Electrical Insul. Mag., 1996: 28-34) contained the following observations on degree of polymerization for paper specimens for which viscosity times concentration fell in a certain middle range: $\begin{array}{lllllll} {418} & {421} & {421} & {422} & {425} & {427} & {431} \end{array}$ $\begin{array}{lllllll} {434} & {437} & {439} & {446} & {447} & {448} & {453} \end{array}$ 454 463 465

a. Construct a boxplot of the data and comment on any interesting features.

b. Is it plausible that the given sample observations were selected from a normal distribution?

c. Calculate a two-sided ${95}\%$ confidence interval for true average degree of polymerization (as did the authors of the article). Does the interval suggest that 440 is a plausible value for true average degree of polymerization? What about 450 ?

34. A sample of 14 joint specimens of a particular type gave a sample mean proportional limit stress of ${8.48}\mathrm{{MPa}}$ and a sample standard deviation of ${.79}\mathrm{{MPa}}$ (“Characterization of Bearing Strength Factors in Pegged Timber Connections," J. of Structural Engr., 1997: 326-332).

a. Calculate and interpret a ${95}\%$ lower confidence bound for the true average proportional limit stress of all such joints. What, if any, assumptions did you make about the distribution of proportional limit stress?

b. Calculate and interpret a ${95}\%$ lower prediction bound for the proportional limit stress of a single joint of this type.

35. Silicone implant augmentation rhinoplasty is used to correct congenital nose deformities. The success of the procedure depends on various biomechanical properties of the human nasal periosteum and fascia. The article “Biomechanics in Augmentation Rhinoplasty” (J. of Med. Engr. and Tech., 2005: 14-17) reported that for a sample of 15 (newly deceased) adults, the mean failure strain (%) was 25.0 , and the standard deviation was 3.5.

a. Assuming a normal distribution for failure strain, estimate true average strain in a way that conveys information about precision and reliability.

b. Predict the strain for a single adult in a way that conveys information about precision and reliability. How does the prediction compare to the estimate calculated in part (a)?

36. A normal probability plot of the $n = {26}$ observations on escape time given in Exercise 36 of Chapter 1 shows a substantial linear pattern; the sample mean and sample standard deviation are 370.69 and 24.36 , respectively.

a. Calculate an upper confidence bound for population mean escape time using a confidence level of ${95}\%$ .

b. Calculate an upper prediction bound for the escape time of a single additional worker using a prediction level of ${95}\%$ . How does this bound compare with the confidence bound of part (a)?

c. Suppose that two additional workers will be chosen to participate in the simulated escape exercise. Denote their escape times by ${X}_{27}$ and ${X}_{28}$ , and let ${\bar{X}}_{\text{new }}$ denote the average of these two values. Modify the formula for a PI for a single $x$ value to obtain a PI for ${\bar{X}}_{\text{new }}$ , and calculate a ${95}\%$ two-sided interval based on the given escape data.

37. A study of the ability of individuals to walk in a straight line ("Can We Really Walk Straight?" Amer. J. of Physical Anthro., 1992: 19-27) reported the accompanying data on cadence (strides per second) for a sample of $n = {20}$ randomly selected healthy men.

$\begin{array}{llllllllll} {.95} & {.85} & {.92} & {.95} & {.93} & {.86} & {1.00} & {.92} & {.85} & {.81} \end{array}$

$\begin{array}{llllllllll} {.78} & {.93} & {.93} & {1.05} & {.93} & {1.06} & {1.06} & {.96} & {.81} & {.96} \end{array}$

A normal probability plot gives substantial support to the assumption that the population distribution of cadence is approximately normal. A descriptive summary of the data from Minitab follows:

<table><tr><td>VariableN</td><td>Mean</td><td>Median</td><td>TrMean</td><td>StDev</td><td>SEMean</td></tr><tr><td>cadence 20</td><td>0.9255</td><td>0.9300</td><td>0.9261</td><td>0.0809</td><td>0.0181</td></tr><tr><td>Variable</td><td>Min</td><td>Max</td><td>Q1</td><td>Q3</td><td></td></tr><tr><td>cadence</td><td>0.7800</td><td>1.0600</td><td>0.8525</td><td>0.9600</td><td></td></tr></table>

a. Calculate and interpret a ${95}\%$ confidence interval for population mean cadence.

b. Calculate and interpret a ${95}\%$ prediction interval for the cadence of a single individual randomly selected from this population.

c. Calculate an interval that includes at least ${99}\%$ of the cadences in the population distribution using a confidence level of ${95}\%$ .

38. Ultra high performance concrete (UHPC) is a relatively new construction material that is characterized by strong adhesive properties with other materials. The article "Adhesive Power of Ultra High Performance Concrete from a Thermodynamic Point of View" (J. of Materials in Civil Engr., 2012: 1050-1058) described an investigation of the intermolecular forces for UHPC connected to various substrates. The following work of adhesion measurements (in $\mathrm{{mJ}}/{\mathrm{m}}^{2}$ ) for UHPC specimens adhered to steel appeared in the article:

107.1 109.5 107.4 106.8 1

a. Is it plausible that the given sample observations were selected from a normal distribution?

b. Calculate a two-sided ${95}\%$ confidence interval for the true average work of adhesion for UHPC adhered to steel. Does the interval suggest that 107 is a plausible value for the true average work of adhesion for UHPC adhered to steel? What about 110 ?

c. Predict the resulting work of adhesion value resulting from a single future replication of the experiment by calculating a ${95}\%$ prediction interval, and compare the width of this interval to the width of the CI from (b).

d. Calculate an interval for which you can have a high degree of confidence that at least ${95}\%$ of all UHPC specimens adhered to steel will have work of adhesion values between the limits of the interval.

39. Exercise 72 of Chapter 1 gave the following observations on a receptor binding measure (adjusted distribution volume) for a sample of 13 healthy individuals: 23, 39, ${40},{41},{43},{47},{51},{58},{63},{66},{67},{69},{72}$ .

a. Is it plausible that the population distribution from which this sample was selected is normal?

b. Calculate an interval for which you can be ${95}\%$ confident that at least ${95}\%$ of all healthy individuals in the population have adjusted distribution volumes lying between the limits of the interval.

c. Predict the adjusted distribution volume of a single healthy individual by calculating a ${95}\%$ prediction interval. How does this interval's width compare to the width of the interval calculated in part (b)?

40. Exercise 13 of Chapter 1 presented a sample of $n = {153}$ observations on ultimate tensile strength, and Exercise 17 of the previous section gave summary quantities and requested a large-sample confidence interval. Because the sample size is large, no assumptions about the population distribution are required for the validity of the CI.

a. Is any assumption about the tensile-strength distribution required prior to calculating a lower prediction bound for the tensile strength of the next specimen selected using the method described in this section? Explain.

b. Use a statistical software package to investigate the plausibility of a normal population distribution.

c. Calculate a lower prediction bound with a prediction level of ${95}\%$ for the ultimate tensile strength of the next specimen selected.

41. A more extensive tabulation of $t$ critical values than what appears in this book shows that for the $t$ distribution with

${20}\mathrm{{df}}$ , the areas to the right of the values ${.687},{.860}$ , and 1.064 are ${.25},{.20}$ , and .15, respectively. What is the confidence level for each of the following three confidence intervals for the mean $\mu$ of a normal population distribution? Which of the three intervals would you recommend be used, and why?

a. $\left( {\bar{x} - {.687s}/\sqrt{21},\bar{x} + {1.725s}/\sqrt{21}}\right)$

b. $\left( {\bar{x} - {.860s}/\sqrt{21},\bar{x} + {1.325s}/\sqrt{21}}\right)$

c. $\left( {\bar{x} - {1.064s}/\sqrt{21},\bar{x} + {1.064s}/\sqrt{21}}\right)$

## 7.4 Confidence Intervals for the Variance and Standard Deviation of a Normal Population

Although inferences concerning a population variance ${\sigma }^{2}$ or standard deviation $\sigma$ are usually of less interest than those about a mean or proportion, there are occasions when such procedures are needed. In the case of a normal population distribution, inferences are based on the following result concerning the sample variance ${S}^{2}$ .

## THEOREM

Let ${X}_{1},{X}_{2},\ldots ,{X}_{n}$ be a random sample from a normal distribution with parameters $\mu$ and ${\sigma }^{2}$ . Then the rv

$$
\frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} = \frac{\sum {\left( {X}_{i} - \bar{X}\right) }^{2}}{{\sigma }^{2}}
$$

has a chi-squared $\left( {\chi }^{2}\right)$ probability distribution with $n - 1\mathrm{{df}}$ .

As discussed in Sections 4.4 and 7.1, the chi-squared distribution is a continuous probability distribution with a single parameter $\nu$ , called the number of degrees of freedom, with possible values $1,2,3,\ldots$ . The graphs of several ${\chi }^{2}$ probability density functions (pdf’s) are illustrated in Figure 7.10. Each pdf $f\left( {x;\nu }\right)$ is positive only for $x > 0$ , and each has a positive skew (stretched out upper tail), though the distribution moves rightward and becomes more symmetric as $\nu$ increases. To specify inferential procedures that use the chi-squared distribution, we need notation analogous to that for a $t$ critical value ${t}_{\alpha ,\nu }$ .

![01927a02-a1da-7086-ba87-2208e017bc0f_28_699_1701_736_237_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_28_699_1701_736_237_0.jpg)

Figure 7.10 Graphs of chi-squared density functions

NOTATION Let ${\chi }_{\alpha ,\nu }^{2}$ , called a chi-squared critical value, denote the number on the horizontal axis such that $\alpha$ of the area under the chi-squared curve with $\nu$ df lies to the right of ${\chi }_{\alpha ,\nu }^{2}$ .

Symmetry of $t$ distributions made it necessary to tabulate only upper-tailed $t$ critical values $\left( {t}_{\alpha ,\nu }\right.$ for small values of $\left. \alpha \right)$ . The chi-squared distribution is not symmetric, so Appendix Table A. 7 contains values of ${\chi }_{\alpha ,\nu }^{2}$ both for $\alpha$ near 0 and near 1, as illustrated in Figure 7.11(b). For example, ${\chi }_{{.025},{14}}^{2} = {26.119}$ , and ${\chi }_{{.95},{20}}^{2}$ (the 5th percentile) $= {10.851}$ .

![01927a02-a1da-7086-ba87-2208e017bc0f_29_754_413_886_418_0.jpg](images/01927a02-a1da-7086-ba87-2208e017bc0f_29_754_413_886_418_0.jpg)

Figure ${7.11}\;{\chi }_{\alpha ,\nu }^{2}$ notation illustrated

The rv $\left( {n - 1}\right) {S}^{2}/{\sigma }^{2}$ satisfies the two properties on which the general method for obtaining a CI is based: It is a function of the parameter of interest ${\sigma }^{2}$ , yet its probability distribution (chi-squared) does not depend on this parameter. The area under a chi-squared curve with $\nu$ df to the right of ${\chi }_{\alpha /2,\nu }^{2}$ is $\alpha /2$ , as is the area to the left of ${\chi }_{1 - \alpha /2,\nu }^{2}$ . Thus the area captured between these two critical values is $1 - \alpha$ . As a consequence of this and the theorem just stated,

$$
P\left( {{\chi }_{1 - \alpha /2, n - 1}^{2} < \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} < {\chi }_{\alpha /2, n - 1}^{2}}\right) = 1 - \alpha \tag{7.17}
$$

The inequalities in (7.17) are equivalent to

$$
\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{\alpha /2, n - 1}^{2}} < {\sigma }^{2} < \frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{1 - \alpha /2, n - 1}^{2}}
$$

Substituting the computed value ${s}^{2}$ into the limits gives a CI for ${\sigma }^{2}$ , and taking square roots gives an interval for $\sigma$ .

A ${100}\left( {1 - \alpha }\right) \%$ confidence interval for the variance ${\sigma }^{2}$ of a normal population has lower limit

$$
\left( {n - 1}\right) {s}^{2}/{\chi }_{\alpha /2, n - 1}^{2}
$$

and upper limit

$$
\left( {n - 1}\right) {s}^{2}/{\chi }_{1 - \alpha /2, n - 1}^{2}
$$

A confidence interval for $\sigma$ has lower and upper limits that are the square roots of the corresponding limits in the interval for ${\sigma }^{2}$ . An upper or a lower confidence bound results from replacing $\alpha /2$ with $\alpha$ in the corresponding limit of the CI.

7.15 The accompanying data on breakdown voltage of electrically stressed circuits was read from a normal probability plot that appeared in the article "Damage of Flexible Printed Wiring Boards Associated with Lightning-Induced Voltage Surges"

(IEEE Transactions on Components, Hybrids, and Manuf. Tech., 1985: 214-220).

The straightness of the plot gave strong support to the assumption that breakdown voltage is approximately normally distributed.

$$
\begin{array}{lllllllll} {1470} & {1510} & {1690} & {1740} & {1900} & {2000} & {2030} & {2100} & {2190} \\ {2200} & {2290} & {2380} & {2390} & {2480} & {2500} & {2580} & {2700} & \end{array} \tag{2190}
$$

Let ${\sigma }^{2}$ denote the variance of the breakdown voltage distribution. The computed value of the sample variance is ${s}^{2} = {137},{324.3}$ , the point estimate of ${\sigma }^{2}$ . With $\mathrm{{df}} = n - 1 = {16}$ , a ${95}\%$ CI requires ${\chi }_{{.975},{16}}^{2} = {6.908}$ and ${\chi }_{{.025},{16}}^{2} = {28.845}$ . The interval is

$$
\left( {\frac{{16}\left( {{137},{324.3}}\right) }{28.845},\;\frac{{16}\left( {{137},{324.3}}\right) }{6.908}}\right) = \left( {{76},{172.3},{318},{064.4}}\right)
$$

Taking the square root of each endpoint yields (276.0,564.0) as the ${95}\% \mathrm{{CI}}$ for $\sigma$ . These intervals are quite wide, reflecting substantial variability in breakdown voltage in combination with a small sample size.

CIs for ${\sigma }^{2}$ and $\sigma$ when the population distribution is not normal can be difficult to obtain. For such cases, consult a knowledgeable statistician.

## EXERCISES Section 7.4 (42-46)

42. Determine the values of the following quantities:

a. ${\chi }_{{.1},{15}}^{2}\;$ b. ${\chi }_{{.1},{25}}^{2}$

c. ${\chi }_{{.01},{25}}^{2}\;$ d. ${\chi }_{{.005},{25}}^{2}$

e. ${\chi }_{{.99},{25}}^{2}\;$ f. ${\chi }_{{.995},{25}}^{2}$

43. Determine the following:

a. The 95th percentile of the chi-squared distribution with $v = {10}$

b. The 5th percentile of the chi-squared distribution with $v = {10}$

c. $P\left( {{10.98} \leq {\chi }^{2} \leq {36.78}}\right)$ , where ${\chi }^{2}$ is a chi-squared rv with $\nu = {22}$

d. $P\left( {{\chi }^{2} < {14.611}}\right.$ or $\left. {{\chi }^{2} > {37.652}}\right)$ , where ${\chi }^{2}$ is a chi-squared rv with $\nu = {25}$

44. The amount of lateral expansion (mils) was determined for a sample of $n = 9$ pulsed-power gas metal arc welds used in LNG ship containment tanks. The resulting sample standard deviation was $s = {2.81}$ mils. Assuming normality, derive a ${95}\% \mathrm{{CI}}$ for ${\sigma }^{2}$ and for $\sigma$ .

45. Wire electrical-discharge machining (WEDM) is a process used to manufacture conductive hard metal components. It uses a continuously moving wire that serves as an electrode. Coating on the wire electrode allows for cooling of the wire electrode core and provides an improved cutting performance. The article "High-Performance Wire Electrodes for Wire Electrical-Discharge Machining-A Review" (J. of Engr. Manuf., 2012: 1757-1773) gave the following sample observations on total coating layer thickness (in $\mu \mathrm{m}$ ) of eight wire electrodes used for WEDM:

$\begin{array}{llllllll} {21} & {16} & {29} & {35} & {42} & {24} & {24} & {25} \end{array}$

Calculate a ${99}\% \mathrm{{CI}}$ for the standard deviation of the coating layer thickness distribution. Is this interval valid whatever the nature of the distribution? Explain.

46. The article "Concrete Pressure on Formwork" (Mag. of Concrete Res., 2009: 407-417) gave the following observations on maximum concrete pressure $\left( {\mathrm{{kN}}/{\mathrm{m}}^{2}}\right)$ : $\begin{array}{llllllll} {33.2} & {41.8} & {37.3} & {40.2} & {36.7} & {39.1} & {36.2} & {41.8} \end{array}$ $\begin{array}{lllllll} {36.0} & {35.2} & {36.7} & {38.9} & {35.8} & {35.2} & {40.1} \end{array}$

a. Is it plausible that this sample was selected from a normal population distribution?

b. Calculate an upper confidence bound with confidence level ${95}\%$ for the population standard deviation of maximum pressure.

47. Example 1.11 introduced the accompanying observations on bond strength.

<table><tr><td>11.5</td><td>12.1</td><td>9.9</td><td>9.3</td><td>7.8</td><td>6.2</td><td>6.6</td><td>7.0</td></tr><tr><td>13.4</td><td>17.1</td><td>9.3</td><td>5.6</td><td>5.7</td><td>5.4</td><td>5.2</td><td>5.1</td></tr><tr><td>4.9</td><td>10.7</td><td>15.2</td><td>8.5</td><td>4.2</td><td>4.0</td><td>3.9</td><td>3.8</td></tr><tr><td>3.6</td><td>3.4</td><td>20.6</td><td>25.5</td><td>13.8</td><td>12.6</td><td>13.1</td><td>8.9</td></tr><tr><td>8.2</td><td>10.7</td><td>14.2</td><td>7.6</td><td>5.2</td><td>5.5</td><td>5.1</td><td>5.0</td></tr><tr><td>5.2</td><td>4.8</td><td>4.1</td><td>3.8</td><td>3.7</td><td>3.6</td><td>3.6</td><td>3.6</td></tr></table>

a. Estimate true average bond strength in a way that conveys information about precision and reliability. [Hint: $\sum {x}_{i} = {387.8}$ and $\sum {x}_{i}^{2} = {4247.08}$ .]

b. Calculate a ${95}\% \mathrm{{CI}}$ for the proportion of all such bonds whose strength values would exceed 10 .

48. The article "Distributions of Compressive Strength Obtained from Various Diameter Cores" (ACI Materials J., 2012: 597-606) described a study in which compressive strengths were determined for concrete specimens of various types, core diameters, and length-to-diameter ratios. For one particular type, diameter, and $l/d$ ratio, the 18 tested specimens resulted in a sample mean compressive strength of ${64.41}\mathrm{{MPa}}$ and a sample standard deviation of ${10.32}\mathrm{{MPa}}$ . Normality of the compressive strength distribution was judged to be quite plausible.

a. Calculate a confidence interval with confidence level ${98}\%$ for the true average compressive strength under these circumstances.

b. Calculate a ${98}\%$ lower prediction bound for the compressive strength of a single future specimen tested under the given circumstances. [Hint: ${t}_{{.02},{17}} =$ 2.224.]

49. For those of you who don't already know, dragon boat racing is a competitive water sport that involves 20 paddlers propelling a boat across various race distances. It has become increasingly popular over the last few years. The article "Physiological and Physical Characteristics of Elite Dragon Boat Paddlers" (J. of Strength and Conditioning, 2013: 137-145) summarized an extensive statistical analysis of data obtained from a sample of 11 paddlers. It reported that a ${95}\%$ confidence interval for true average force $\left( \mathrm{N}\right)$ during a simulated 200-m race was $\left( {{60.2},{70.6}}\right)$ . Obtain a ${95}\%$ prediction interval for the force of a single randomly selected dragon boat paddler undergoing the simulated race.

50. A journal article reports that a sample of size 5 was used as a basis for calculating a ${95}\% \mathrm{{CI}}$ for the true average natural frequency $\left( \mathrm{{Hz}}\right)$ of delaminated beams of a certain type. The resulting interval was (229.764, 233.504). You decide that a confidence level of ${99}\%$ is more appropriate than the ${95}\%$ level used. What are the limits of the ${99}\%$ interval? [Hint: Use the center of the interval and its width to determine $\bar{x}$ and $s$ .]

51. Unexplained respiratory symptoms reported by athletes are often incorrectly considered secondary to exercise-induced asthma. The article “High Prevalence of Exercise-Induced Laryngeal Obstruction in Athletes" (Medicine and Science in Sports and Exercise, 2013: 2030-2035) suggested that many such cases could instead be explained by obstruction of the larynx. In a sample of 88 athletes referred for an asthma workup, 31 were found to have the EILO condition.

a. Calculate and interpret a confidence interval using a ${95}\%$ confidence level for the true proportion of all athletes found to have the EILO condition under these circumstances.

b. What sample size is required if the desired width of the ${95}\% \mathrm{{CI}}$ is to be at most .04, irrespective of the sample results?

c. Does the upper limit of the interval in (a) specify a ${95}\%$ upper confidence bound for the proportion being estimated? Explain.

52. High concentration of the toxic element arsenic is all too common in groundwater. The article "Evaluation of Treatment Systems for the Removal of Arsenic from Groundwater" (Practice Periodical of Hazardous, Toxic, and Radioactive Waste Mgmt., 2005: 152-157) reported that for a sample of $n = 5$ water specimens selected for treatment by coagulation, the sample mean arsenic concentration was ${24.3\mu }\mathrm{g}/\mathrm{L}$ , and the sample standard deviation was 4.1. The authors of the cited article used $t$ -based methods to analyze their data, so hopefully had reason to believe that the distribution of arsenic concentration was normal.

a. Calculate and interpret a ${95}\% \mathrm{{CI}}$ for true average arsenic concentration in all such water specimens.

b. Calculate a ${90}\%$ upper confidence bound for the standard deviation of the arsenic concentration distribution.

c. Predict the arsenic concentration for a single water specimen in a way that conveys information about precision and reliability.

53. Aphid infestation of fruit trees can be controlled either by spraying with pesticide or by inundation with ladybugs. In a particular area, four different groves of fruit trees are selected for experimentation. The first three groves are sprayed with pesticides 1,2 , and 3 , respectively, and the

fourth is treated with ladybugs, with the following results on yield:

<table><thead><tr><th>Treatment</th><th>${n}_{i} =$ Number of Trees</th><th>${\bar{x}}_{i}$ (Bushels/Tree)</th><th>${s}_{i}$</th></tr></thead><tr><td>1</td><td>100</td><td>10.5</td><td>1.5</td></tr><tr><td>2</td><td>90</td><td>10.0</td><td>1.3</td></tr><tr><td>3</td><td>100</td><td>10.1</td><td>1.8</td></tr><tr><td>4</td><td>120</td><td>10.7</td><td>1.6</td></tr></table>

Let ${\mu }_{i} =$ the true average yield (bushels/tree) after receiving the $i$ th treatment. Then

$$
\theta = \frac{1}{3}\left( {{\mu }_{1} + {\mu }_{2} + {\mu }_{3}}\right) - {\mu }_{4}
$$

measures the difference in true average yields between treatment with pesticides and treatment with ladybugs. When ${n}_{1},{n}_{2},{n}_{3}$ , and ${n}_{4}$ are all large, the estimator $\widehat{\theta }$ obtained by replacing each ${\mu }_{i}$ by ${\bar{X}}_{i}$ is approximately normal. Use this to derive a large-sample ${100}\left( {1 - \alpha }\right) \%$ CI for $\theta$ , and compute the ${95}\%$ interval for the given data.

54. It is important that face masks used by firefighters be able to withstand high temperatures because firefighters commonly work in temperatures of ${200} - {500}^{ \circ }\mathrm{F}$ . In a test of one type of mask, 11 of 55 masks had lenses pop out at ${250}^{ \circ }$ . Construct a ${90}\%$ upper confidence bound for the true proportion of masks of this type whose lenses would pop out at ${250}^{ \circ }$ .

55. A manufacturer of college textbooks is interested in estimating the strength of the bindings produced by a particular binding machine. Strength can be measured by recording the force required to pull the pages from the binding. If this force is measured in pounds, how many books should be tested to estimate the average force required to break the binding to within ${.1}\mathrm{{lb}}$ with ${95}\%$ confidence? Assume that $\sigma$ is known to be .8 .

56. The accompanying data on crack initiation depth $\left( {\mu \mathrm{m}}\right)$ was read from a lognormal probability plot that appeared in the article "Incorporating Small Fatigue Crack Growth in Probabilistic Life Prediction: Effect of Stress Ratio in Ti-6Al-2Sn-6Mo" (Intl. J. of Fatigue, 2013: 83-95). Although the pattern in the plot was quite straight, a normal probability plot of the data also shows a reasonably linear pattern. And a boxplot indicates that the distribution is quite symmetric in the middle ${50}\%$ of the data and only mildly skewed overall. It is therefore reasonable to estimate and predict using $t$ intervals. $\begin{array}{llllllll} {4.7} & {5.1} & {5.2} & {5.3} & {5.6} & {5.8} & {6.3} & {6.7} \end{array}$ $\begin{array}{llllllll} {7.2} & {7.4} & {7.7} & {8.5} & {8.9} & {9.3} & {10.1} & {11.2} \end{array}$

a. Estimate the true average crack initiation depth with a ${99}\% \mathrm{{CI}}$ and interpret the resulting interval.

b. Predict the value of a single crack initiation depth by constructing a ${99}\%$ PI.

c. Interpret in context the meaning of ${99}\%$ in (b).

57. In Example 6.8, we introduced the concept of a censored experiment in which $n$ components are put on test and the experiment terminates as soon as $r$ of the components have failed. Suppose component lifetimes are independent, each having an exponential distribution with parameter $\lambda$ . Let ${Y}_{1}$ denote the time at which the first failure occurs, ${Y}_{2}$ the time at which the second failure occurs, and so on, so that ${T}_{r} = {Y}_{1} + \cdots + {Y}_{r} +$ $\left( {n - r}\right) {Y}_{r}$ is the total accumulated lifetime at termination. Then it can be shown that ${2\lambda }{T}_{r}$ has a chi-squared distribution with ${2r}\mathrm{{df}}$ . Use this fact to develop a ${100}\left( {1 - \alpha }\right) \%$ CI formula for true average lifetime $1/\lambda$ . Compute a ${95}\%$ CI from the data in Example 6.8.

58. Let ${X}_{1},{X}_{2},\ldots ,{X}_{n}$ be a random sample from a continuous probability distribution having median $\widetilde{\mu }$ (so that $P\left( {{X}_{i} \leq \widetilde{\mu }}\right) = P\left( {{X}_{i} \geq \widetilde{\mu }}\right) = {.5})$ .

a. Show that

$$
P\left( {\min \left( {X}_{i}\right) < \widetilde{\mu } < \max \left( {X}_{i}\right) }\right) = 1 - {\left( \frac{1}{2}\right) }^{n - 1}
$$

so that $\left( {\min \left( {x}_{\mathrm{i}}\right) ,\max \left( {x}_{i}\right) }\right)$ is a ${100}\left( {1 - \alpha }\right) \%$ confidence interval for $\widetilde{\mu }$ with $\alpha = {\left( \frac{1}{2}\right) }^{n - 1}$ . [Hint: The complement of the event $\left\{ {\min \left( {X}_{i}\right) < \widetilde{\mu } < \max \left( {X}_{i}\right) }\right\}$ is $\left\{ {\max \left( {X}_{i}\right) \leq }\right.$ $\widetilde{\mu }\} \cup \left\{ {\min \left( {X}_{i}\right) \geq \widetilde{\mu }}\right\}$ . But max $\left( {X}_{i}\right) \leq \widetilde{\mu }$ iff ${X}_{i} \leq \widetilde{\mu }$ for all $i$ .]

b. For each of six normal male infants, the amount of the amino acid alanine $\left( {\mathrm{{mg}}/{100}\mathrm{\;{mL}}}\right)$ was determined while the infants were on an isoleucine-free diet, resulting in the following data:2.70

Compute a ${97}\% \mathrm{{CI}}$ for the true median amount of alanine for infants on such a diet ("The Essential Amino Acid Requirements of Infants," Amer. J. of Nutrition, 1964: 322-330).

c. Let ${x}_{\left( 2\right) }$ denote the second smallest of the ${x}_{i}$ ’s and ${x}_{\left( n - 1\right) }$ denote the second largest of the ${x}_{i}$ ’s. What is the confidence level of the interval $\left( {{x}_{\left( 2\right) },{x}_{\left( n - 1\right) }}\right)$ for $\widetilde{\mu }$ ?

59. Let ${X}_{1},{X}_{2},\ldots ,{X}_{n}$ be a random sample from a uniform distribution on the interval $\left\lbrack {0,\theta }\right\rbrack$ , so that

$$
f\left( x\right) = \left\{ \begin{array}{ll} \frac{1}{\theta } & 0 \leq x \leq \theta \\ 0 & \text{ otherwise } \end{array}\right.
$$

Then if $Y = \max \left( {X}_{i}\right)$ , it can be shown that the rv $U = Y/\theta$ has density function

$$
{f}_{U}\left( u\right) = \left\{ \begin{matrix} n{u}^{n - 1} & 0 \leq u \leq 1 \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

a. Use ${f}_{U}\left( u\right)$ to verify that

$$
P\left( {{\left( \alpha /2\right) }^{1/n} < \frac{Y}{\theta } \leq {\left( 1 - \alpha /2\right) }^{1/n}}\right) = 1 - \alpha
$$

and use this to derive a ${100}\left( {1 - \alpha }\right) \%$ CI for $\theta$ .

b. Verify that $P\left( {{\alpha }^{1/n} \leq Y/\theta \leq 1}\right) = 1 - \alpha$ , and derive a ${100}\left( {1 - \alpha }\right) \%$ CI for $\theta$ based on this probability statement.

c. Which of the two intervals derived previously is shorter? If my waiting time for a morning bus is uniformly distributed and observed waiting times are ${x}_{1} = {4.2},{x}_{2} = {3.5},{x}_{3} = {1.7},{x}_{4} = {1.2}$ , and ${x}_{5} = {2.4}$ , derive a ${95}\% \mathrm{{CI}}$ for $\theta$ by using the shorter of the two intervals.

60. Let $0 \leq \gamma \leq \alpha$ . Then a ${100}\left( {1 - \alpha }\right) \%$ CI for $\mu$ when $n$ is large is

$$
\left( {\bar{x} - {z}_{\gamma } \cdot \frac{s}{\sqrt{n}},\bar{x} + {z}_{\alpha - \gamma } \cdot \frac{s}{\sqrt{n}}}\right)
$$

The choice $\gamma = \alpha /2$ yields the usual interval derived in Section 7.2; if $\gamma \neq \alpha /2$ , this interval is not symmetric about $\bar{x}$ . The width of this interval is $w = s\left( {{z}_{\gamma } + {z}_{\alpha - \gamma }}\right) /\sqrt{n}$ . Show that $w$ is minimized for the choice $\gamma = \alpha /2$ , so that the symmetric interval is the shortest. [Hints: (a) By definition of ${z}_{\alpha },\Phi \left( {z}_{\alpha }\right) = 1 - \alpha$ , so that ${z}_{\alpha } = {\Phi }^{-1}\left( {1 - \alpha }\right)$ ; (b) the relationship between the derivative of a function $y = f\left( x\right)$ and the inverse function $x = {f}^{-1}\left( y\right)$ is $\left. {\left( {d/{dy}}\right) {f}^{-1}\left( y\right) = 1/{f}^{\prime }\left( x\right) \text{.}}\right\rbrack$

61. Suppose ${x}_{1},{x}_{2},\ldots ,{x}_{n}$ are observed values resulting from a random sample from a symmetric but possibly heavy-tailed distribution. Let $\widetilde{x}$ and ${f}_{\mathrm{s}}$ denote the sample median and fourth spread, respectively. Chapter 11 of Understanding Robust and Exploratory Data Analysis (see the bibliography in Chapter 6) suggests the following robust ${95}\% \mathrm{{CI}}$ for the population mean (point of symmetry):

$$
\widetilde{x} \pm \left( \frac{\text{ conservative }t\text{ critical value }}{1.075}\right) \cdot \frac{{f}_{s}}{\sqrt{n}}
$$

The value of the quantity in parentheses is 2.10 for $n = {10},{1.94}$ for $n = {20}$ , and 1.91 for $n = {30}$ . Compute this $\mathrm{{CI}}$ for the data of Exercise 45, and compare to the $t\mathrm{{CI}}$ appropriate for a normal population distribution.

62. a. Use the results of Example 7.5 to obtain a ${95}\%$ lower confidence bound for the parameter $\lambda$ of an exponential distribution, and calculate the bound based on the data given in the example.

b. If lifetime $X$ has an exponential distribution, the probability that lifetime exceeds $t$ is $P\left( {X > t}\right) = {e}^{-{\lambda t}}$ . Use the result of part (a) to obtain a ${95}\%$ lower confidence bound for the probability that breakdown time exceeds ${100}\mathrm{\;{min}}$ .

## BIBLIOGRAPHY

DeGroot, Morris, and Mark Schervish, Probability and Statistics (4th ed.), Addison-Wesley, Upper Saddle River, $\mathrm{{NJ}},{2012}$ . A very good exposition of the general principles of statistical inference.

Devore, Jay, and Kenneth Berk, Modern Mathematical Statistics with Applications, Springer, New York, 2012. The exposition is a bit more comprehensive and sophisticated

than that of the current book, and includes more material on bootstrapping.

Hahn, Gerald, and William Meeker, Statistical Intervals, Wiley, New York, 1991. Almost everything you ever wanted to know about statistical intervals (confidence, prediction, tolerance, and others).