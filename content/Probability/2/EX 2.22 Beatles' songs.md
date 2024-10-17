
- A particular iPod playlist contains 100 songs, 
	- 10 of which are by the Beatles. 
- Suppose the shuffle feature is used to play the songs in random order 
	- the randomness of the shuffling process is investigated in "Does Your iPod Really Play Favorites?" (The Amer. Statistician, 2009: 263-268). 
- What is the probability that the first Beatles song heard is the fifth song played?

- In order for this event to occur, it must be the case that 
	- the first four songs played are not Beatles' songs (NBs) 
	- the fifth song is by the Beatles (B). 
- The number of ways to select the first five songs is
  $${100}\left( {99}\right) \left( {98}\right) \left( {97}\right) \left( {96}\right) .$$
- The number of ways to select these five songs so that 
	- the first four are NBs 
	- the next is a B is 90(89)(88)(87)(10). 
- The random shuffle assumption implies that any particular set of 5 songs from amongst the 100 has the same chance of being selected as the first five played as does any other set of five songs; 
	- each outcome is equally likely.
- Therefore the desired probability is the ratio of the number of outcomes for which the event of interest occurs to the number of possible outcomes: 
$$
\begin{align}
&P\left( {{1}^{\text{st }}\mathrm{B}\text{ is the }{5}^{\text{th }}\text{ song played }}\right) \\
= &\frac{{90} \cdot {89} \cdot {88} \cdot {87} \cdot {10}}{{100} \cdot {99} \cdot {98} \cdot {97} \cdot {96}} \\
= &\frac{{P}_{4,{90}} \cdot \left( {10}\right) }{{P}_{5,{100}}} \\
= &{.0679}
\end{align}
$$

Here is an alternative line of reasoning involving combinations. 
- Rather than focusing on selecting just the first five songs, 
	- think of playing all 100 songs in random order. 
- The number of ways of choosing 10 of these songs to be the Bs is $\left( \begin{matrix} {100} \\ {10} \end{matrix}\right)$
	- without regard to the order in which they are then played
- Now if we choose 9 of the last 95 songs to be Bs, 
	- which can be done in $\left( \begin{matrix} {95} \\ 9 \end{matrix}\right)$ ways, 
	- that leaves four NBs and one $\mathrm{B}$ for the first five songs. 
- There is only one further way for these five to 
	- start with four NBs and 
	- then follow with a B 
	- remember that we are considering unordered subsets
- Thus 
  $$P\left( {{1}^{\text{st }}\mathrm{B}\text{ is the }{5}^{\text{th }}\text{ song played }}\right) = \frac{\left( \begin{matrix} {95} \\ 9 \end{matrix}\right) }{\left( \begin{matrix} {100} \\ {10} \end{matrix}\right) }$$
  - It is easily verified that this latter expression is in fact identical to the first expression for the desired probability, 
	  - so the numerical result is again .0679.

- The probability that one of the first five songs played is a Beatles' song is 
$$
\begin{align}
&P \left( {1}^{\text{st}} \mathrm{B} \text{ is the } {1}^{\text{st}} \text{ or } 2^{\text{nd}} \text{ or } 3^{\text{rd}} \text{ or } 4^{\text{th}} \text{ or } 5^{\text{th}} \text{ song played } \right) \\
&= \frac{\left( 
\begin{matrix} {99} \\ 9 \end{matrix}\right)}{\left( \begin{matrix} {100} \\ {10} \end{matrix}\right)} + \frac{\left(\begin{matrix} {98} \\ 9 \end{matrix}\right)}{\left(\begin{matrix} {100} \\ {10} \end{matrix}\right)} + \frac{\left(\begin{matrix} {97} \\ 9 \end{matrix}\right)}{\left(\begin{matrix} {100} \\ {10} \end{matrix}\right)} + \frac{\left(\begin{matrix} {96} \\ 9 \end{matrix}\right)}{\left( \begin{matrix} {100} \\ {10} \end{matrix}\right)} + \frac{\left( \begin{matrix} {95} \\ 9 \end{matrix}\right)}{\left( \begin{matrix} {100} \\ {10} \end{matrix}\right)} \\
&= {.4162}
\end{align}
$$

- It is thus rather likely that a Beatles' song will be one of the first five songs played. 
- Such a "coincidence" is not as surprising as might first appear to be the case.