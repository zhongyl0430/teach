
- Only 1 in 1000 adults is afflicted with a rare disease for which a diagnostic test has been developed. 
- The test is such that when an individual actually has the disease, 
	- a positive result will occur ${99}\%$ of the time, 
	- whereas an individual without the disease will show a positive test result only $2\%$ of the time 
		- the sensitivity of this test is ${99}\%$ 
		- and the specificity is ${98}\%$ ; 
		- in contrast, the Sept. 22, 2012 issue of The Lancet reports that the first at-home HIV test has a sensitivity of only ${92}\%$ and a specificity of ${99.98}\%$

- If a randomly selected individual is tested and the result is positive, 
	- what is the probability that the individual has the disease?


- To use Bayes' theorem, let 
	- ${A}_{1} =$ individual has the disease, 
	- ${A}_{2} =$ individual does not have the disease, 
	- $B =$ positive test result. 
- Then 
	- $P\left( {A}_{1}\right) = {.001}$ , 
	- $P\left( {A}_{2}\right) = {.999}$, 
	- $P\left( {B \mid {A}_{1}}\right) = {.99}$ , 
	- $P\left( {B \mid {A}_{2}}\right) = {.02}$ . 
- The tree diagram for this problem is in Figure 2.12.

Figure 2.12 Tree diagram for the rare-disease problem
![](01913607-292d-7d0a-a250-4b01870485a1_31_864460.jpg)

- Next to each branch corresponding to a positive test result, 
	- the multiplication rule yields the recorded probabilities. 
- Therefore, $P\left( B\right) = {.00099} + {.01998} = {.02097}$ , 
	- from which we have
$$
P\left( {{A}_{1} \mid B}\right) = \frac{P\left( {{A}_{1} \cap B}\right) }{P\left( B\right) } = \frac{.00099}{.02097} = {.047}
$$

- This result seems counterintuitive; 
	- the diagnostic test appears so accurate that we expect someone with a positive test result to be highly likely to have the disease, 
	- whereas the computed conditional probability is only .047 . 
- However, the rarity of the disease implies that most positive test results arise from errors rather than from diseased individuals. 
- The probability of having the disease has increased by a multiplicative factor of 47 (from prior .001 to posterior .047); 
	- but to get a further increase in the posterior probability, a diagnostic test with much smaller error rates is needed.

