
- Now let's move on to combinations 
	- i.e., unordered subsets. 

> [!example]
> - Again refer to the student council scenario, 
> - and suppose that three of the seven representatives are to be selected to attend a statewide convention. 
> - The order of selection is *not important*; 
> 	- all that matters is which three get selected. 
> - So we are looking for $\left( \begin{array}{l} 7 \\ 3 \end{array}\right)$, 
> 	- the number of combinations of size 3 that can be formed from the 7 individuals.
> - Consider for a moment the combination $a,c,g$. 
> - These three individuals can be ordered in $3! = 6$ ways to produce permutations: 
>   $$a,c,g\;a,g,c\;c,a,g\;c,g,a\;g,a,c\;g,c,a$$
> 	  - Similarly, there are $3! = 6$ ways to order the  combination $b,c,e$ to produce permutations, 
> 	  - in fact $3!$ ways to order any particular combination of size 3 to produce permutations. 
>   - This implies the following relationship 
> 	  - between the number of combinations 
> 	  - and the number of permutations: 
> $$
> \begin{align}
> &{P}_{3,7} = \left( {3!}\right) \cdot \left( \begin{array}{l} 7 \\ 3 \end{array}\right) \\\Rightarrow &\left( \begin{array}{l} 7 \\ 3 \end{array}\right) = \frac{{P}_{3,7}}{3!} = \frac{7!}{\left( {3!}\right) \left( {4!}\right) } = \frac{\left( 7\right) \left( 6\right) \left( 5\right) }{\left( 3\right) \left( 2\right) \left( 1\right) } = {35}
> \end{align}
> $$
> - It would not be too difficult to list the 35 combinations, 
> 	- but there is no need to do so if we are interested only in how many there are. 
> - Notice that 
> 	- the number of permutations 210 far exceeds the number of combinations; 
> 	- the former is larger than the latter by a factor of $3!$ 
> 		- since that is how many ways each combination can be ordered.

- Generalizing the foregoing line of reasoning gives a simple relationship 
	- between the number of permutations 
	- and the number of combinations 
- that yields a concise expression for the latter quantity.

> [!proposition]
> $$\left( \begin{array}{l} n \\ k \end{array}\right) = \frac{{P}_{k,n}}{k!} = \frac{n!}{k!\left( {n - k}\right) !}$$

Notice that
- $\left( \begin{array}{l} n \\ n \end{array}\right) = 1$ 
- $\left( \begin{array}{l} n \\ 0 \end{array}\right) = 1$ 
	- since there is only one way to choose a set of (all) $n$ elements or of no elements, 
- $\left( \begin{array}{l} n \\ 1 \end{array}\right) = n$ 
	- since there are $n$ subsets of size 1 .


[[EX 2.22 Beatles' songs]]

[[EX 2.23 laser printer and inkjet printer]]