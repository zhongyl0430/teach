Suppose that ${25}\%$ of all students at a large public university receive financial aid. Let $X$ be the number of students in a random sample of size 50 who receive financial aid, so that $p = {.25}$ . Then $\mu = {12.5}$ and $\sigma = {3.06}$ . Since ${np} = {50}\left( {.25}\right) = {12.5} \geq {10}$ and ${nq} = {37.5} \geq {10}$ , the approximation can safely be applied. The probability that at most 10 students receive aid is

$$
P\left( {X \leq {10}}\right) = B\left( {{10};{50},{.25}}\right) \approx \Phi \left( \frac{{10} + {.5} - {12.5}}{3.06}\right)
$$

$$
= \Phi \left( {-{.65}}\right) = {.2578}
$$

Similarly, the probability that between 5 and 15 (inclusive) of the selected students receive aid is

$$
P\left( {5 \leq X \leq {15}}\right) = B\left( {{15};{50},{.25}}\right) - B\left( {4;{50},{.25}}\right)
$$

$$
\approx \Phi \left( \frac{{15.5} - {12.5}}{3.06}\right) - \Phi \left( \frac{{4.5} - {12.5}}{3.06}\right) = {.8320}
$$

The exact probabilities are .2622 and .8348 , respectively, so the approximations are quite good. In the last calculation, $P\left( {5 \leq X \leq {15}}\right)$ is being approximated by the area under the normal curve between 4.5 and 15.5 - the continuity correction is used for both the upper and lower limits.