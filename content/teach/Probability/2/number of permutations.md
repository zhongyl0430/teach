
The number of permutations can be determined by using our earlier *counting rule* for $k$ -tuples. 

> [!example]
> Suppose, for example, that 
> - a college of engineering has seven departments, which we denote by 
> $$a,b,c,d,e,f, g$$
> - Each department has one representative on the college's student council. 
> - From these seven representatives, 
> 	- one is to be chosen chair, 
> 	- another is to be selected vice-chair, 
> 	- a third will be secretary. 
> 
> - How many ways are there to select the three officers?
> 	- That is, how many permutations of size 3 can be formed from the 7 representatives? 
> 
> - To answer this question, think of forming a triple (3-tuple) in which 
> 	- the first element is the chair, 
> 	- the second is the vice-chair, 
> 	- the third is the secretary. 
> - e.g. $\left( {a,g,b}\right)$, $\left( {b,g,a}\right)$, $\left( {d,f,b}\right)$ . 
> 
> - The chair can be selected in any of ${n}_{1} = 7$ ways. 
> - For each way of selecting the chair, 
> 	- there are ${n}_{2} = 6$ ways to select the vice-chair, 
> 	- hence $7 \times 6 = {42}$ (chair, vice-chair) pairs. 
> - Finally, for each way of selecting a chair and vice-chair, 
> 	- there are ${n}_{3} = 5$ ways of choosing the secretary. 
> - This gives 
>   $${P}_{3,7} = \left( 7\right) \left( 6\right) \left( 5\right) = {210}$$
>   as the number of permutations of size 3 that can be formed from 7 distinct individuals. 
>   A tree diagram representation would show three generations of branches.

- The expression for ${P}_{3,7}$ can be rewritten with the aid of factorial notation. 
	- Recall that 7! (read "7 factorial") is compact notation for the descending product of integers (7)(6)(5)(4)(3)(2)(1).
	- More generally, for any positive integer $m$, 
	  $$m! = m\left( {m - 1}\right) \left( {m - 2}\right) \cdots \cdot \left( 2\right) \left( 1\right) .$$
	- This gives $1! = 1$ , 
	- we also define $0! = 1$ . 
- Then $$
{P}_{3,7} = \left( 7\right) \left( 6\right) \left( 5\right) = \frac{\left( 7\right) \left( 6\right) \left( 5\right) \left( {4!}\right) }{\left( 4!\right) } = \frac{7!}{4!}
$$
- Generalizing to arbitrary group size $n$ and subset size $k$ yields 
$$
{P}_{k,n} = n\left( {n - 1}\right) \left( {n - 2}\right) \cdots \cdot \left( {n - \left( {k - 2}\right) }\right) \left( {n - \left( {k - 1}\right) }\right)
$$
- Multiplying and dividing this by $\left( {n - k}\right) !$ gives a compact expression for the number of permutations.

> [!proposition]
> $${P}_{k,n} = \frac{n!}{\left( {n - k}\right) !}$$

[[Ex 2.21 grading questions]]