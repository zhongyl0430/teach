Service time for a certain type of bank transaction is a random variable having an exponential distribution with parameter $\lambda$ . Suppose ${X}_{1}$ and ${X}_{2}$ are service times for two different customers, assumed independent of each other. Consider the total service time ${T}_{o} = {X}_{1} + {X}_{2}$ for the two customers, also a statistic. The cdf of ${T}_{o}$ is, for $t \geq 0$ ,
$$
\begin{align}
F_{{T}_{0}}\left( t \right) 
&= P\left( {X}_{1} + {X}_{2} \leq t \right) = \iint_{\left\{ \left( {x}_{1},{x}_{2} \right) : {x}_{1} + {x}_{2} \leq t \right\}} f\left( {x}_{1},{x}_{2} \right) d{x}_{1} d{x}_{2} \\

&= \int_{0}^{t} \int_{0}^{t - {x}_{1}} \lambda e^{-\lambda {x}_{1}} \cdot \lambda e^{-\lambda {x}_{2}} d{x}_{2} d{x}_{1} \\

&= \int_{0}^{t} \left[ \lambda e^{-\lambda {x}_{1}} - \lambda e^{-\lambda t} \right] d{x}_{1} \\

&= 1 - e^{-\lambda t} - \lambda t e^{-\lambda t}.
\end{align}
$$

The region of integration is pictured in Figure 5.10.

Figure 5.10 
Region of integration to obtain cdf of ${T}_{o}$ in Example 5.22
![0192609f-6f5c-74c9-8588-c1ef28b2184d_27_986_720_415_281_0.jpg](images/0192609f-6f5c-74c9-8588-c1ef28b2184d_27_986_720_415_281_0.jpg)

The pdf of ${T}_{o}$ is obtained by differentiating ${F}_{{T}_{o}}\left( t\right)$ :
$$
{f}_{{T}_{o}}\left( t\right) = \left\{ \begin{matrix} {\lambda }^{2}t{e}^{-{\lambda t}} & t \geq 0 \\ 0 & t < 0 \end{matrix}\right. \tag{5.5}
$$

This is a gamma $\operatorname{pdf}\left( {\alpha = 2\text{and}\beta = 1/\lambda }\right)$ . The pdf of $\bar{X} = {T}_{o}/2$ is obtained from the relation $\{ \bar{X} \leq \bar{x}\}$ iff $\left\{ {{T}_{o} \leq 2\bar{x}}\right\}$ as
$$
{f}_{\bar{X}}\left( \bar{x}\right) = \left\{ \begin{matrix} 4{\lambda }^{2}\bar{x}{e}^{-{2\lambda }\bar{x}} & \bar{x} \geq 0 \\ 0 & \bar{x} < 0 \end{matrix}\right. \tag{5.6}
$$

The mean and variance of the underlying exponential distribution are $\mu = 1/\lambda$ and ${\sigma }^{2} = 1/{\lambda }^{2}$ . From Expressions (5.5) and (5.6), it can be verified that $E\left( \bar{X}\right) = 1/\lambda$ , $V\left( \bar{X}\right) = 1/\left( {2{\lambda }^{2}}\right) , E\left( {T}_{o}\right) = 2/\lambda$ , and $V\left( {T}_{o}\right) = 2/{\lambda }^{2}$ . These results again suggest some general relationships between means and variances of $\bar{X},{T}_{o}$ , and the underlying distribution.
