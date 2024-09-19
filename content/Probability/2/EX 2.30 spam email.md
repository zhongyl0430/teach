- An individual has 3 different email accounts. 
	- Most of her messages, in fact 70%, come into account #1, 
	- whereas ${20}\%$ come into account #2 
	- and the remaining ${10}\%$ into account #3. 
- Of the messages into account #1, only 1% are spam, 
	- whereas the corresponding percentages for accounts #2
	- and #3 are $2\%$ and $5\%$ , respectively. 

- What is the probability that a randomly selected message is spam?

- To answer this question, let's first establish some notation:
- ${A}_{i} = \{$ message is from account $\# i\}$ for $i = 1,2,3,$
- $B = \{$ message is spam $\}$

- Then the given percentages imply that
	- $P\left( {A}_{1}\right) = {.70}$
	- $P\left( {A}_{2}\right) = {.20}$
	- $P\left( {A}_{3}\right) = {.10}$
- We have
	- $P\left( {B \mid {A}_{1}}\right) = {.01}$
	- $P\left( {B \mid {A}_{2}}\right) = {.02}$
	- $P\left( {B \mid {A}_{3}}\right) = {.05}$

- Now it is simply a matter of substituting into the equation for the law of total probability:
$$
P\left( B\right) = \left( {.01}\right) \left( {.70}\right) + \left( {.02}\right) \left( {.20}\right) + \left( {.05}\right) \left( {.10}\right) = {.016}
$$
- In the long run, ${1.6}\%$ of this individual's messages will be spam.