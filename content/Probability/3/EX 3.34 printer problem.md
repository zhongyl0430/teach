- Problem scenario:
	- University information technology office received 20 service orders for printer problems:
    - 8 laser printers
    - 12 inkjet printers
	- A sample of 5 service orders is to be selected for a customer satisfaction survey.
  
- Selection process:
	- The 5 service orders are selected randomly.
	- Any subset of size 5 has the same chance of being selected as any other subset.

- Objective:
	- Determine the probability of exactly $x$ service orders for inkjet printers in the sample, where $x = 0, 1, 2, 3, 4, \text{ or } 5$.

- Key points:
	- Total service orders: 20
	- Service orders for laser printers: 8
	- Service orders for inkjet printers: 12
	- Sample size: 5
	- Calculate probability for various values of $x$ (number of inkjet printers selected in the sample).

- Population details:
	- Total population size: $N = 20$
	- Sample size: $n = 5$
	- Number of inkjet printers (denoted $S$): $M = 12$
	- Number of laser printers (denoted $F$): $N - M = 8$

- Case where $x = 2$:
	- We are interested in the probability that exactly 2 inkjet printers are selected in the sample.
	- Since all outcomes (each consisting of 5 specific orders) are equally likely, the probability can be calculated based on combinatorics.

- Probability setup:
	- The total number of ways to choose 5 orders from 20: $\binom{20}{5}$
	- The number of ways to choose exactly 2 inkjet printers from 12: $\binom{12}{2}$
	- The number of ways to choose the remaining 3 printers from the 8 laser printers: $\binom{8}{3}$

- Probability expression:
	- The probability for exactly $x = 2$ inkjet printers in the sample:
$$
\begin{align}
P(X = 2) &= h(2; 5, 12, 20) \\
         &= \frac{\text{number of outcomes having } X = 2}{\text{number of possible outcomes}}
\end{align}
$$

- Total number of possible outcomes:
	- The number of ways to select 5 service orders from 20 without regard to order is: $$\binom{20}{5}$$

- Number of outcomes where $X = 2$ (exactly 2 inkjet printers are selected):
	- The number of ways to select 2 inkjet orders from the 12 inkjet printers: $$\binom{12}{2}$$
  - For each of these selections, the number of ways to select the remaining 3 orders from the 8 laser printers: $$ \binom{8}{3}$$

- Applying the product rule:
	- The total number of outcomes with $X = 2$ (2 inkjet printers and 3 laser printers) is given by:
    $$
    \binom{12}{2} \times \binom{8}{3}
    $$

- Probability expression:
	- The probability that exactly 2 inkjet printers are selected is: $$h\left( {2;5,{12},{20}}\right) = \frac{\left( \begin{matrix} {12} \\ 2 \end{matrix}\right) \left( \begin{array}{l} 8 \\ 3 \end{array}\right) }{\left( \begin{matrix} {20} \\ 5 \end{matrix}\right) } = \frac{77}{323} = {.238}$$
