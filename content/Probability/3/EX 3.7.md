1. The Cal Poly Department of Statistics has a lab with six computers reserved for statistics majors.
	- Let $X$ denote the number of these computers that are in use at a particular time of day.
	- Probability distribution of $X$ is as follows:

   | x   | 0   | 1   | 2   | 3   | 4   | 5   | 6   |
   |-----|-----|-----|-----|-----|-----|-----|-----|
   | p(x)| .05 | .10 | .15 | .25 | .20 | .15 | .10 |

2. Elementary probability properties are used to calculate other probabilities of interest.
- Example 1: 
	- The probability that at most 2 computers are in use:
	- 
	$$
     \begin{aligned}
     P(X \leq 2) &= P(X = 0 \text{ or } 1 \text{ or } 2) \\
     &= p(0) + p(1) + p(2) \\
     &= .05 + .10 + .15 = .30
     \end{aligned}
     $$
     
- Example 2: 
	- The probability that at least 3 computers are in use:
		- Since the event "at least 3 computers are in use" is complementary to "at most 2 computers are in use":
		- 
$$
\begin{aligned}
P(X \geq 3) &= 1 - P(X \leq 2) \\
&= 1 - .30 = .70
\end{aligned}
$$
		- Alternatively, this can also be obtained by adding together probabilities for $X = 3, 4, 5, 6$.
   
- Example 3: 
	- The probability that between 2 and 5 computers inclusive are in use:
	- 
$$
\begin{aligned}
P(2 \leq X \leq 5) &= P(X = 2, 3, 4, \text{or } 5) \\
&= .15 + .25 + .20 + .15 = .75
\end{aligned}
$$
   
- Example 4: 
	- The probability that the number of computers in use is strictly between 2 and 5:
     - $$P(2 < X < 5) = P(X = 3 \text{ or } 4) = .25 + .20 = .45$$