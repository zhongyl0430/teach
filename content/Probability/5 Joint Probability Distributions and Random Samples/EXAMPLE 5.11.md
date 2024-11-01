If ${X}_{1},\ldots,{X}_{n}$ represent the lifetimes of $n$ components, the components operate independently of one another, and each lifetime is exponentially distributed with parameter $\lambda$, then for ${x}_{1} \geq 0,{x}_{2} \geq 0,\ldots,{x}_{n} \geq 0$,

$$
f\left( {{x}_{1},{x}_{2},\ldots,{x}_{n}}\right) = \left( {\lambda {e}^{-\lambda {x}_{1}}}\right) \cdot \left( {\lambda {e}^{-\lambda {x}_{2}}}\right) \cdot \cdots \cdot \left( {\lambda {e}^{-\lambda {x}_{n}}}\right) = {\lambda }^{n}{e}^{-{\lambda \sum }{x}_{i}}
$$

Suppose a system consisting of these components will fail as soon as a single component fails. 
Let $T$ represent system lifetime. Then the probability that the system lasts past time $t$ is
$$
\begin{align}
P\left( T > t \right) 
&= P\left( X_{1} > t, \ldots, X_{n} > t \right) \\
&= \int_{t}^{\infty} \ldots \int_{t}^{\infty} f\left( x_{1}, \ldots, x_{n} \right) \, d{x}_{1} \ldots d{x}_{n} \\
&= \left( \int_{t}^{\infty} \lambda e^{-\lambda x_{1}} \, d{x}_{1} \right) \ldots \left( \int_{t}^{\infty} \lambda e^{-\lambda x_{n}} \, d{x}_{n} \right) \\
&= \left( e^{-\lambda t} \right)^{n} = e^{-n \lambda t}.
\end{align}
$$

Therefore,
$$
P\left( {\text{ system lifetime } \leq t}\right) = 1 - {e}^{-{n\lambda t}}\;\text{  for }t \geq 0
$$
which shows that system lifetime has an exponential distribution with parameter ${n\lambda }$ ; the expected value of system lifetime is $1/{n\lambda }$.

A variation on the foregoing scenario appeared in the article "A Method for Correlating Field Life Degradation with Reliability Prediction for Electronic Modules" (Quality and Reliability Engr. Intl., 2005: 715-726). The investigators considered a circuit card with $n$ soldered chip resistors. The failure time of a card is the minimum of the individual solder connection failure times (mileages here). It was assumed that the solder connection failure mileages were independent, that failure mileage would exceed $t$ if and only if the shear strength of a connection exceeded a threshold $d$, and that each shear strength was normally distributed with a mean value and standard deviation that depended on the value of mileage $t : \mu \left( t\right) = {a}_{1} - {a}_{2}t$ and $\sigma \left( t\right) = {a}_{3} + {a}_{4}t$ (a weld’s shear strength typically deteriorates and becomes more variable as mileage increases). Then the probability that the failure mileage of a card exceeds $t$ is

$$
P\left( {T > t}\right) = {\left( 1 - \Phi \left( \frac{d - \left( {{a}_{1} - {a}_{2}t}\right. }{{a}_{3} + {a}_{4}t}\right) \right) }^{n}
$$

The cited article suggested values for $d$ and the ${a}_{i}$ ’s based on data. In contrast to the exponential scenario, normality of individual lifetimes does not imply normality of system lifetime.
