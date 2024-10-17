- Scenario:
	- Each newborn child is rated on the Apgar scale immediately after birth.
	- Possible ratings range from $0$ to $10$.
- The Apgar scale is a quick assessment tool used to evaluate the health of newborns. 
	- It consists of five criteria, each scored from 0 to 2:
	1. **Appearance**: Skin color
		- 0: Blue or pale all over
		- 1: Pink body with blue extremities
		- 2: Completely pink
	2. **Pulse**: Heart rate
		- 0: No pulse
		- 1: Less than 100 beats per minute
		- 2: Over 100 beats per minute
	3. **Grimace**: Reflex response
		- 0: No response
		- 1: Grimace or weak cry when stimulated
		- 2: Crying and active response to stimulation
	4. **Activity**: Muscle tone
		- 0: Limp
		- 1: Some flexion of arms and legs
		- 2: Active movement
	5. **Respiration**: Breathing effort
		- 0: Not breathing
		- 1: Weak, irregular breathing
		- 2: Good, strong cry
	- **Total Score**: 
		- The scores from each category are summed, with a maximum possible score of 10. 
		- Higher scores indicate better health.
- Random variable definition:
	- Let $X$ denote the Apgar score of a randomly selected child born at a certain hospital during the next year.
- Probability mass function (pmf) of $X$:
	- The pmf provides the probabilities associated with each possible value of $X$.
	- Possible values of $X$ are:
	    - $X = 0, 1, 2, \ldots, 10$

| x | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| p(x) | .002 | .001 | .002 | .005 | .02 | .04 | .18 | .37 | .25 | .12 | .01 |

Then the mean value of $X$ is
$$
\begin{align}
E(X) &= \mu \\
&= 0(0.002) + 1(0.001) + 2(0.002) + \cdots \\ 
&+ 8(0.25) + 9(0.12) + 10(0.01) \\
           &= 7.15
\end{align}
$$
- Context of the Apgar score:
	- The Apgar score $X$ can take values from $0$ to $10$.
	- While the score $\mu$ (the mean) is a calculated value, it is not a possible score for an individual child.
- Conceptual population:
	- The pmf serves as a model for a conceptual population that includes all possible values of $X$:
    $$
    \{0, 1, 2, \ldots, 10\}
    $$
	- This conceptual population does not refer to an existing set of newborns but is based on the distribution of scores across many hypothetical future children.
- Mean of the conceptual population:
	- The mean value of this conceptual population is given by:
    $$
    \mu = 7.15
    $$
	- This value reflects the average Apgar score one would expect if many children were rated, providing insight into overall health assessments.
- Interpretation:
	- While the mean $\mu$ is not an achievable score for an individual, it helps summarize the expected outcome for a large group based on the distribution modeled by the pmf.