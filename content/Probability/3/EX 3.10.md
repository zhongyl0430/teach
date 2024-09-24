- Group of five potential blood donors:
	- $a, b, c, d, e$
	- Only $a$ and $b$ have type O-positive blood
- Blood typing procedure:
	- Five blood samples, one from each individual, will be typed in random order
	- Process continues until an O-positive ($\mathrm{O}^+$) individual is identified
- Let $Y$ = number of typings necessary to identify an $\mathrm{O}^+$ individual
- The probability mass function (pmf) of $Y$ is:
	- To be determined based on the typing sequence and the likelihood of identifying an $\mathrm{O}^+$ individual
$$
\begin{align}
p(1) &= P(Y = 1) = P(a \text{ or } b \text{ typed first}) = \frac{2}{5} = 0.4 \\
p(2) &= P(Y = 2) = P(c, d, \text{ or } e \text{ first, and then } a \text{ or } b) \\
      &= P(c, d, \text{ or } e \text{ first}) \cdot P(a \text{ or } b \text{ next} \mid c, d, \text{ or } e \text{ first}) \\
      &= \frac{3}{5} \cdot \frac{2}{4} = 0.3 \\
p(3) &= P(Y = 3) = P(c, d, \text{ or } e \text{ first and second, and then } a \text{ or } b) \\
      &= \left( \frac{3}{5} \right) \left( \frac{2}{4} \right) \left( \frac{2}{3} \right) = 0.2 \\
p(4) &= P(Y = 4) = P(c, d, \text{ and } e \text{ all done first}) \\
      &= \left( \frac{3}{5} \right) \left( \frac{2}{4} \right) \left( \frac{1}{3} \right) = 0.1 \\
p(y) &= 0 \quad \text{if} \quad y \neq 1, 2, 3, 4
\end{align}
$$

In tabular form, the pmf is

| $y$     | 1   | 2   | 3   | 4   |
| ------- | --- | --- | --- | --- |
| $p (y)$ | .4  | .3  | .2  | .1  |
where any $y$ value not listed receives zero probability. 

Figure 3.3 shows a line graph of the pmf.

Figure 3.3
![image](images/019165cb-e657-75f5-b964-f15ddb80567f_8_160131.jpg)
The line graph for the pmf in Example 3.10
