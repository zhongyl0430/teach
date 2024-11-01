When a certain method is used to collect a fixed volume of rock samples in a region, there are four resulting rock types. Let ${X}_{1},{X}_{2}$, and ${X}_{3}$ denote the proportion by volume of rock types 1, 2, and 3 in a randomly selected sample (the proportion of rock type 4 is $1 - {X}_{1} - {X}_{2} - {X}_{3}$, so a variable ${X}_{4}$ would be redundant). If the joint pdf of ${X}_{1},{X}_{2},{X}_{3}$ is
$$
\begin{align}
f\left( x_{1}, x_{2}, x_{3} \right) 
&= \begin{cases} 
k x_{1} x_{2} \left( 1 - x_{3} \right) & \text{ if } 0 \leq x_{1} \leq 1, \; 0 \leq x_{2} \leq 1, \; 0 \leq x_{3} \leq 1, \; x_{1} + x_{2} + x_{3} \leq 1 \\ 
0 & \text{ otherwise } 
\end{cases}
\end{align}
$$

then $k$ is determined by
$$
\begin{align}
1 &= \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f\left( x_{1}, x_{2}, x_{3} \right) \, d{x}_{3} \, d{x}_{2} \, d{x}_{1} \\
&= \int_{0}^{1} \left\{ \int_{0}^{1 - x_{1}} \left[ \int_{0}^{1 - x_{1} - x_{2}} k x_{1} x_{2} \left( 1 - x_{3} \right) \, d{x}_{3} \right] d{x}_{2} \right\} d{x}_{1}.
\end{align}
$$

This iterated integral has value $k/{144}$, so $k = {144}$. The probability that rocks of types 1 and 2 together account for at most ${50}\%$ of the sample is
$$
\begin{align}
&P\left( X_{1} + X_{2} \leq 0.5 \right) \\
&= \iiint f\left( x_{1}, x_{2}, x_{3} \right) \, d{x}_{3} \, d{x}_{2} \, d{x}_{1} \\
&\text{ subject to } \left\{ 
\begin{matrix} 
0 \leq x_{i} \leq 1 & \text{ for } i = 1, 2, 3 \\ 
x_{1} + x_{2} + x_{3} \leq 1, \; x_{1} + x_{2} \leq 0.5 
\end{matrix}
\right\} \\
&= \int_{0}^{0.5} \left\{ \int_{0}^{0.5 - x_{1}} \left[ \int_{0}^{1 - x_{1} - x_{2}} 144 x_{1} x_{2} \left( 1 - x_{3} \right) \, d{x}_{3} \right] d{x}_{2} \right\} d{x}_{1} \\
&= 0.6066.
\end{align}
$$
