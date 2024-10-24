The direction of an imperfection with respect to a reference line on a circular object such as a tire, brake rotor, or flywheel is, in general, subject to uncertainty. 
Consider the reference line connecting the valve stem on a tire to the center point, and let $X$ be the angle measured clockwise to the location of an imperfection. 
One possible pdf for $X$ is
$$
f\left( x\right) = \left\{ \begin{matrix} \frac{1}{360} & 0 \leq x < {360} \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

The pdf is graphed in Figure 4.3. 

Figure 4.3 
The pdf and probability from Example 4.4
![01925166-48c0-7eca-9860-67f13d0848b1_3_451_922_1184_286_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_3_451_922_1184_286_0.jpg)

^fig-4-3

Clearly $f\left( x\right) \geq 0$ . 
The area under the density curve is just the area of a rectangle: 
$$(\text{height})(\text{base}) = \left( {1/{360}}\right) \left( {360}\right) = 1 .$$
The probability that the angle is between ${90}^{ \circ }$ and ${180}^{ \circ }$ is
$$
\begin{align}
P\left( {{90} \leq X \leq {180}}\right) &= {\int }_{90}^{180}\frac{1}{360}{dx} \\
&= {\left. \frac{x}{360}\right| }_{x = {90}}^{x = {180}} \\
&= \frac{1}{4} = {.25}
\end{align}
$$

The probability that the angle of occurrence is within ${90}^{ \circ }$ of the reference line is
$$
\begin{align}
&
P\left( {0 \leq X \leq {90}}\right) + P\left( {{270} \leq X < {360}}\right) \\
&= {.25} + {.25} = {.50}
\end{align}
$$