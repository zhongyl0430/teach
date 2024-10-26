
A university warehouse has received a shipment of 25 printers, of which 10 are laser printers and 15 are inkjet models. 
If 6 of these 25 are selected at random to be checked by a particular technician, what is the probability that exactly 3 of those selected are laser printers (so that the other 3 are inkjets)?

Let ${D}_{3} = \{$ exactly 3 of the 6 selected are inkjet printers $\}$. 
Assuming that any particular set of 6 printers is as likely to be chosen as is any other set of 6, we have equally likely outcomes, so $P\left( {D}_{3}\right) = N\left( {D}_{3}\right) /N$, where $N$ is the number of ways of choosing 6 printers from the 25 and $N\left( {D}_{3}\right)$ is the number of ways of choosing 3 laser
printers and 3 inkjet models. 
Thus
$N = \left( \begin{matrix} {25} \\ 6 \end{matrix}\right)$ . 
To obtain $N\left( {D}_{3}\right)$, think of first choosing 3 of the 15 inkjet
models and then 3 of the laser printers. 
There are $\left( \begin{matrix} {15} \\ 3 \end{matrix}\right)$ ways of choosing the 3 inkjet models, and there are $\left( \begin{matrix} {10} \\ 3 \end{matrix}\right)$ ways of choosing the 3 laser printers; 
$N\left( {D}_{3}\right)$ is now the product of these two numbers (visualize a tree diagram-we are really using a product rule argument here), so $$
P\left( {D}_{3}\right) = \frac{N\left( {D}_{3}\right) }{N} = \frac{\left( \begin{matrix} {15} \\ 3 \end{matrix}\right) \left( \begin{matrix} {10} \\ 3 \end{matrix}\right) }{\left( \begin{matrix} {25} \\ 6 \end{matrix}\right) } = \frac{\frac{{15}!}{3!{12}!} \cdot \frac{{10}!}{3!7!}}{\frac{{25}!}{6!{19}!}} = {.3083}
$$

Let ${D}_{4} = \{$ exactly 4 of the 6 printers selected are inkjet
models $\}$ and define ${D}_{5}$ and ${D}_{6}$ in an analogous manner. 
Then the probability that at least 3 inkjet printers are selected is 
$$
\begin{align*}
&P\left( {{D}_{3} \cup {D}_{4} \cup {D}_{5} \cup {D}_{6}}\right) \\
&= P\left( {D}_{3}\right) + P\left( {D}_{4}\right) + P\left( {D}_{5}\right) + P\left( {D}_{6}\right) \\
&= \frac{\left( \begin{matrix} {15} \\ 3 \end{matrix}\right) \left( \begin{matrix} {10} \\ 3 \end{matrix}\right) }{\left( \begin{matrix} {25} \\ 6 \end{matrix}\right) } + \frac{\left( \begin{matrix} {15} \\ 4 \end{matrix}\right) \left( \begin{matrix} {10} \\ 2 \end{matrix}\right) }{\left( \begin{matrix} {25} \\ 6 \end{matrix}\right) } + \frac{\left( \begin{matrix} {15} \\ 5 \end{matrix}\right) \left( \begin{matrix} {10} \\ 1 \end{matrix}\right) }{\left( \begin{matrix} {25} \\ 6 \end{matrix}\right) } + \frac{\left( \begin{matrix} {15} \\ 6 \end{matrix}\right) \left( \begin{matrix} {10} \\ 0 \end{matrix}\right) }{\left( \begin{matrix} {25} \\ 6 \end{matrix}\right) } = {.8530}
\end{align*}$$
$$