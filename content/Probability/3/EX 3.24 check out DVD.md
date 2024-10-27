- A library has an upper limit of 6 on the number of DVDs that can be checked out to an individual at one time. 
- Consider only those who currently have DVDs checked out
- Let $X$ denote the number of DVDs checked out to a randomly selected individual. 
- The pmf of $X$ is as follows:

| $X$    | 1   | 2   | 3   | 4   | 5   | 6   |
| ------ | --- | --- | --- | --- | --- | --- |
| $p(X)$ | .30 | .25 | .15 | .05 | .10 | .15 |

The expected value of $X$ is easily seen to be $$\mu = {2.85} .$$
The variance of $X$ is then
$$
\begin{align}
V(X) &= \sigma^2 = \sum_{x=1}^{6} \left( x - 2.85 \right)^2 \cdot p(x) \\
     &= \left( 1 - 2.85 \right)^2 (0.30) + \left( 2 - 2.85 \right)^2 (0.25) + \cdots + \left( 6 - 2.85 \right)^2 (0.15) \\
     &= 3.2275
\end{align}
$$

The standard deviation of $X$ is 
$$\sigma = \sqrt{3.2275}$$