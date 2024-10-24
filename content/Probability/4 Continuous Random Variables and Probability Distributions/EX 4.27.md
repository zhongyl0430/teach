According to the article "Predictive Model for Pitting Corrosion in Buried Oil and Gas Pipelines" (Corrosion, 2009: 332-342), the lognormal distribution has been reported as the best option for describing the distribution of maximum pit depth data from cast iron pipes in soil. The authors suggest that a lognormal distribution with $\mu = {.353}$ and $\sigma = {.754}$ is appropriate for maximum pit depth $\left( \mathrm{{mm}}\right)$ of buried pipelines. For this distribution, the mean value and variance of pit depth are

$$
E\left( X\right) = {e}^{{.353} + {\left( {.754}\right) }^{2}/2} = {e}^{.6373} = {1.891}
$$

$$
V\left( X\right) = {e}^{2\left( {.353}\right) + {\left( {.754}\right) }^{2}} \cdot \left( {{e}^{{\left( {.754}\right) }^{2}} - 1}\right) = \left( {3.57697}\right) \left( {.765645}\right) = {2.7387}
$$

The probability that maximum pit depth is between 1 and $2\mathrm{\;{mm}}$ is
$$
\begin{align}
    &P\left( 1 \leq X \leq 2 \right) \\
    &= P\left( \ln\left( 1 \right) \leq \ln\left( X \right) \leq \ln\left( 2 \right) \right) \\
    &= P\left( 0 \leq \ln\left( X \right) \leq 0.693 \right) \\
    &= P\left( \frac{0 - 0.353}{0.754} \leq Z \leq \frac{0.693 - 0.353}{0.754} \right) \\
    &= \Phi\left( 0.47 \right) - \Phi\left( -0.45 \right) \\
    &= 0.354
\end{align}
$$

This probability is illustrated in Figure 4.31 (from Minitab).

Figure 4.31 
Lognormal density curve with $\mu = {.353}$ and $\sigma = {.754}$
![01925166-48c0-7eca-9860-67f13d0848b1_39_770_1331_616_420_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_39_770_1331_616_420_0.jpg)

What value $c$ is such that only $1\%$ of all specimens have a maximum pit depth exceeding $c$ ? The desired value satisfies

$$
{.99} = P\left( {X \leq c}\right) = P\left( {Z \leq \frac{\ln \left( c\right) - {.353}}{.754}}\right)
$$

The $z$ critical value 2.33 captures an upper-tail area of ${.01}\left( {{z}_{.01} = {2.33}}\right)$ , and thus a cumulative area of .99 . This implies that

$$
\frac{\ln \left( c\right) - {.353}}{.754} = {2.33}
$$

from which $\ln \left( c\right) = {2.1098}$ and $c = {8.247}$ . Thus 8.247 is the 99th percentile of the maximum pit depth distribution.