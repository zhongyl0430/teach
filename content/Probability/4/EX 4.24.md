Suppose the survival time $X$ in weeks of a randomly selected male mouse exposed to 240 rads of gamma radiation has (what else!) a gamma distribution with $\alpha = 8$ and $\beta = {15}$ . (Data in Survival Distributions: Reliability Applications in the Biomedical Services, by A. J. Gross and V. Clark, suggests $\alpha \approx {8.5}$ and $\beta \approx {13.3}$ .) The expected survival time is $E\left( X\right) = \left( 8\right) \left( {15}\right) = {120}$ weeks, whereas $V\left( X\right) = \left( 8\right) {\left( {15}\right) }^{2} = {1800}$ and ${\sigma }_{X} = \sqrt{1800} = {42.43}$ weeks. The probability that a mouse survives between 60 and 120 weeks is

$$
P\left( {{60} \leq X \leq {120}}\right) = P\left( {X \leq {120}}\right) - P\left( {X \leq {60}}\right)
$$

$$
= F\left( {{120}/{15};8}\right) - F\left( {{60}/{15};8}\right)
$$

$$
= F\left( {8;8}\right) - F\left( {4;8}\right) = {.547} - {.051} = {.496}
$$

The probability that a mouse survives at least 30 weeks is

$$
P\left( {X \geq {30}}\right) = 1 - P\left( {X < {30}}\right) = 1 - P\left( {X \leq {30}}\right)
$$

$$
= 1 - F\left( {{30}/{15};8}\right) = {.999}
$$