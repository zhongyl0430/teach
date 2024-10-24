IQ in a particular population (as measured by a standard test) is known to be approximately normally distributed with $\mu = {100}$ and $\sigma = {15}$. 

> [!question] 
> What is the probability that a randomly selected individual has an IQ of at least 125?

Letting $X =$ the IQ of a randomly chosen person, we wish $P\left( {X \geq {125}}\right)$. 
The temptation here is to standardize $X \geq {125}$ as in previous examples. 
However, the IQ population distribution is actually discrete, since IQs are integer-valued. 
So the normal curve is an approximation to a discrete probability histogram, as pictured in Figure 4.24.

Figure 4.24 
A normal approximation to a discrete distribution
![01925166-48c0-7eca-9860-67f13d0848b1_24_994_184_409_237_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_24_994_184_409_237_0.jpg)

The rectangles of the histogram are centered at integers. 
IQs of at least 125 correspond to rectangles beginning at 124.5, as shaded in Figure 4.24. 
Thus we really want the area under the approximating normal curve to the right of 124.5. 
Standardizing this value gives $P\left( {Z \geq {1.63}}\right) = {.0516}$, whereas standardizing 125 results in $P\left( {Z \geq {1.67}}\right) = {.0475}$. 
The difference is not great, but the answer .0516 is more accurate. 
Similarly, $P\left( {X = {125}}\right)$ would be approximated by the area between 124.5 and 125.5, since the area under the normal curve above the single value 125 is zero.