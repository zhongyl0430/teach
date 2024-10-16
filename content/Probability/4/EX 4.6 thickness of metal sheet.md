Let $X$ , the thickness of a certain metal sheet, have a uniform distribution on $\left\lbrack {A, B}\right\rbrack$ . The density function is shown in Figure 4.6. For $x < A, F\left( x\right) = 0$ , since there is no area under the graph of the density function to the left of such an $x$ . For $x \geq B, F\left( x\right) = 1$ , since all the area is accumulated to the left of such an $x$ . Finally, for $A \leq x \leq B,$

$$
F\left( x\right) = {\int }_{-\infty }^{x}f\left( y\right) {dy} = {\int }_{A}^{x}\frac{1}{B - A}{dy} = {\left. \frac{1}{B - A} \cdot y\right| }_{y = A}^{y = x} = \frac{x - A}{B - A}
$$

Figure 4.6 
The pdf for a uniform distribution
![01925166-48c0-7eca-9860-67f13d0848b1_7_665_1582_800_282_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_7_665_1582_800_282_0.jpg)

The entire cdf is

$$
F\left( x\right) = \left\{ \begin{matrix} 0 & x < A \\ \frac{x - A}{B - A} & A \leq x < B \\ 1 & x \geq B \end{matrix}\right.
$$

The graph of this cdf appears in Figure 4.7.

Figure 4.7 
The cdf for a uniform distribution
![01925166-48c0-7eca-9860-67f13d0848b1_8_944_184_504_243_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_8_944_184_504_243_0.jpg)