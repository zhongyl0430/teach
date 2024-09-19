- Complex components are assembled in a plant that uses two different assembly lines, $A$ and ${A}^{\prime }$. 
- Line $A$ uses older equipment than ${A}^{\prime }$, so it is somewhat slower and less reliable. 
- Suppose 
	- on a given day line $A$ has assembled 8 components, 
		- of which 2 have been identified as defective $\left( B\right)$ 
		- 6 as nondefective $\left( {B}^{\prime }\right)$, 
	- whereas ${A}^{\prime }$ has produced 
		- 1 defective 
		- 9 nondefective components. 
- This information is summarized in the accompanying table.

|   | \(B\) | \(B'\) |
|---|------|-------|
| \(A\)  | 2    | 6     |
| \(A'\) | 1    | 9     |

- Unaware of this information, the sales manager randomly selects
	- 1 of these 18 components for a demonstration. 
- Prior to the demonstration
$$
\begin{align}
&P\left( {\text{line A component selected}}\right) \\
= &P\left( A\right) \\
= &\frac{N\left( A\right) }{N} \\
= &\frac{8}{18} = {.44}
\end{align}
$$

- However, if the chosen component turns out to be defective, 
	- then the event $B$ has occurred, 
	- so the component must have been 1 of the 3 in the $B$ column of the table. 
- Since these 3 components are equally likely among themselves after $B$ has occurred,
$$
P\left( {A \mid B}\right) = \frac{2}{3} = \frac{2/{18}}{3/{18}} = \frac{P\left( {A \cap B}\right) }{P\left( B\right) } \tag{2.2}
$$
