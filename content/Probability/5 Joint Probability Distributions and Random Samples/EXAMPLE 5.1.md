Anyone who purchases an insurance policy for a home or automobile must specify a deductible amount, the amount of loss to be absorbed by the policyholder before the insurance company begins paying out. Suppose that a particular company offers auto deductible amounts of $\$ {100},\$ {500}$, and $\$ {1000}$, and homeowner deductible amounts of $\$ {500},\$ {1000}$, and $\$ {2000}$. 
Consider randomly selecting someone who has both auto and homeowner insurance with this company, and let 
- $X =$ the amount of the auto policy deductible 
- $Y =$ the amount of the homeowner policy deductible. 

The joint pmf of these two variables appears in the accompanying joint probability table:

| $p(x, y)$ | 500 | 1000 | 5000 |
| --------- | --- | ---- | ---- |
| 100       | .30 | .05  | 0    |
| 500       | .15 | .20  | .05  |
| 1000      | .10 | .10  | .05  |

According to this joint pmf, there are nine possible $\left( {X, Y}\right)$ pairs: $\left( {{100},{500}}\right),({100}$, ${1000}),\ldots$, and finally $\left( {{1000},{5000}}\right)$. 
The probability of $\left( {{100},{500}}\right)$ is $$p\left( {{100},{500}}\right) = P\left( {X = {100}, Y = {500}}\right) = {.30} .$$
Clearly $p\left( {x, y}\right) \geq 0$, and it is easily confirmed that the sum of the nine displayed probabilities is 1. 

The probability $P\left( {X = Y}\right)$ is computed by summing $p\left( {x, y}\right)$ over the two $\left( {x, y}\right)$ pairs for which the two deductible amounts are identical:
$$
P\left( {X = Y}\right) = p\left( {{500},{500}}\right) + p\left( {{1000},{1000}}\right) = {.15} + {.10} = {.25}
$$

Similarly, the probability that the auto deductible amount is at least \$500 is the sum of all probabilities corresponding to $\left( {x, y}\right)$ pairs for which $x \geq {500}$; 
this is the sum of the probabilities in the bottom two rows of the joint probability table:
$$
P\left( {X \geq {500}}\right) = {.15} + {.20} + {.05} + {.10} + {.10} + {.05} = {.65}
$$
