- An electronics store sells three different brands of DVD players. 
- Of its DVD player sales, 
	- ${50}\%$ are brand 1 (the least expensive), 
	- ${30}\%$ are brand 2, 
	- ${20}\%$ are brand 3 . 
- Each manufacturer offers a 1-year warranty on parts and labor. 
- It is known that ${25}\%$ of brand 1's DVD players require warranty repair work, 
	- whereas the corresponding percentages for brands 2 and 3 are ${20}\%$ and ${10}\%$ , respectively.

1.  What is the probability that a randomly selected purchaser has bought a brand 1 DVD player that will need repair while under warranty?

2.  What is the probability that a randomly selected purchaser has a DVD player that will need repair while under warranty?

5.  If a customer returns to the store with a DVD player that needs warranty repair work, what is the probability that it is a brand 1 DVD player? A brand 2 DVD player? A brand 3 DVD player?

- The first stage of the problem involves a customer selecting one of the three brands of DVD player. 
- Let 
	- ${A}_{i} = \{$ brand $i$ is purchased $\}$ , for $i = 1$, $2$ , and 3 . 
- Then 
	- $P\left( {A}_{1}\right) = {.50}$,
	- $P\left( {A}_{2}\right) = {.30}$ , 
	- $P\left( {A}_{3}\right) = {.20}$ . 

- Once a brand of DVD player is selected, 
	- the second stage involves observing whether the selected DVD player needs warranty repair. 
- With 
	- $B = \{$ needs repair $\}$ 
	- ${B}^{\prime } = \{$ doesn't need repair $\}$ ,
- the given information implies that
	- $P\left( {B \mid {A}_{1}}\right) = {.25}$, 
	- $P\left( {B \mid {A}_{2}}\right) = {.20}$ , 
	- $P\left( {B \mid {A}_{3}}\right) = {.10}$ .

- The tree diagram representing this experimental situation is shown in Figure 2.10. 


Figure 2.10 Tree diagram for Example 2.29
![](01913607-292d-7d0a-a250-4b01870485a1_28_663477.jpg)


- The initial branches correspond to different brands of DVD players; 
- there are two second-generation branches emanating from the tip of each initial branch, 
	- one for "needs repair" and 
	- the other for "doesn't need repair." 
- The probability $P\left( {A}_{i}\right)$ appears on the $i$ th initial branch, 
	- whereas the conditional probabilities $P\left( {B \mid {A}_{i}}\right)$ and $P\left( {{B}^{\prime } \mid {A}_{i}}\right)$ appear on the second-generation branches. 
- To the right of each second-generation branch corresponding to the occurrence of $B$ , 
	- we display the product of probabilities on the branches leading out to that point. 
- This is simply the multiplication rule in action. 
- The answer to the question posed in 1 is thus
$$P\left( {{A}_{1} \cap B}\right) = P\left( {B \mid {A}_{1}}\right) \cdot P\left( {A}_{1}\right) = {.125}$$
- The answer to question 2 is
$$
\begin{aligned}
P\left( B\right) 
&= P\left\lbrack \text{(brand 1 and repair) or (brand 2 and repair) or (brand 3 and repair)}\right\rbrack \\
&= P\left( {{A}_{1} \cap B}\right) + P\left( {{A}_{2} \cap B}\right) + P\left( {{A}_{3} \cap B}\right)\\
&= {.125} + {.060} + {.020} = {.205}
\end{aligned}
$$

Finally,
$$
P\left( {{A}_{1} \mid B}\right) = \frac{P\left( {{A}_{1} \cap B}\right) }{P\left( B\right) } = \frac{.125}{.205} = {.61}
$$
$$
P\left( {{A}_{2} \mid B}\right) = \frac{P\left( {{A}_{2} \cap B}\right) }{P\left( B\right) } = \frac{.060}{.205} = {.29}
$$

and
$$
P\left( {{A}_{3} \mid B}\right) = 1 - P\left( {{A}_{1} \mid B}\right) - P\left( {{A}_{2} \mid B}\right) = {.10}
$$

- The initial or prior probability of brand 1 is .50 . 
- Once it is known that the selected DVD player needed repair, 
	- the posterior probability of brand 1 increases to .61. 
	- This is because brand 1 DVD players are more likely to need warranty repair than are the other brands. 
- The posterior probability of brand 3 is $P\left( {{A}_{3} \mid B}\right) = {.10}$ , 
	- which is much less than the prior probability $P\left( {A}_{3}\right) = {.20}$ .
