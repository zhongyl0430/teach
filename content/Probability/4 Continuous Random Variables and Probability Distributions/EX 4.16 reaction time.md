The time that it takes a driver to react to the brake lights on a decelerating vehicle is critical in helping to avoid rear-end collisions. The article "Fast-Rise Brake Lamp as a Collision-Prevention Device" (Ergonomics, 1993: 391-395) suggests that reaction time for an in-traffic response to a brake signal from standard brake lights can be modeled with a normal distribution having mean value 1.25 sec and standard deviation of .46 sec. 

> [!question] 
> What is the probability that reaction time is between 1.00 sec and 1.75 sec? 

If we let $X$ denote reaction time, then standardizing gives
$$
{1.00} \leq X \leq {1.75}
$$
if and only if
$$
\frac{{1.00} - {1.25}}{.46} \leq \frac{X - {1.25}}{.46} \leq \frac{{1.75} - {1.25}}{.46}
$$

Thus
$$
\begin{align}
    &P\left( 1.00 \leq X \leq 1.75 \right) \\
    &= P\left( \frac{1.00 - 1.25}{0.46} \leq Z \leq \frac{1.75 - 1.25}{0.46} \right) \\
    &= P\left( -0.54 \leq Z \leq 1.09 \right) \\
    &= \Phi\left( 1.09 \right) - \Phi\left( -0.54 \right) \\
    &= 0.8621 - 0.2946 \\
    &= 0.5675
\end{align}
$$

This is illustrated in Figure 4.22. 

Figure 4.22 
Normal curves for Example 4.16
![01925166-48c0-7eca-9860-67f13d0848b1_21_603_1784_953_384_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_21_603_1784_953_384_0.jpg)

Similarly, if we view 2 sec as a critically long reaction time, the probability that actual reaction time will exceed this value is
$$
\begin{align}
    &P\left( X > 2 \right) \\
    &= P\left( Z > \frac{2 - 1.25}{0.46} \right) \\
    &= P\left( Z > 1.63 \right) \\
    &= 1 - \Phi\left( 1.63 \right) \\
    &= 0.0516
\end{align}
$$
