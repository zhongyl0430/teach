"Time headway" in traffic flow is the elapsed time between the time that one car finishes passing a fixed point and the instant that the next car begins to pass that point. 
Let $X =$ the time headway for two randomly chosen consecutive cars on a freeway during a period of heavy flow. 
The following pdf of $X$ is essentially the one suggested in "The Statistical Properties of Freeway Traffic" (Transp. Res., vol. 11: 221-228):
$$
f\left( x\right) = \left\{ \begin{matrix} {.15}{e}^{-{.15}\left( {x - {.5}}\right) } & x \geq {.5} \\ 0 & \text{ otherwise } \end{matrix}\right.
$$

The graph of $f\left( x\right)$ is given in Figure 4.4; 

Figure 4.4 
The density curve for time headway in Example 4.5
![01925166-48c0-7eca-9860-67f13d0848b1_4_744_1776_913_389_0.jpg](images/01925166-48c0-7eca-9860-67f13d0848b1_4_744_1776_913_389_0.jpg)

There is no density associated with headway times less than ${.5}$ , and headway density decreases rapidly (exponentially fast) as $x$ increases from .5. 
Clearly, $f\left( x\right) \geq 0$ ; to show that ${\int }_{-\infty }^{\infty }f\left( x\right) {dx} = 1$ , we use the calculus result $${\int }_{a}^{\infty }{e}^{-{kx}}{dx} = \left( {1/k}\right) {e}^{-k \cdot a} .$$
Then
$$
\begin{align}
{\int }_{-\infty }^{\infty }f\left( x\right) {dx} 
&= {\int }_{.5}^{\infty }{.15}{e}^{-{.15}\left( {x - {.5}}\right) }{dx} \\
&= {.15}{e}^{.075}{\int }_{.5}^{\infty }{e}^{-{.15x}}{dx} \\
&= {.15}{e}^{.075} \cdot \frac{1}{.15}{e}^{-\left( {.15}\right) \left( {.5}\right) } = 1 
\end{align}
$$

The probability that headway time is at most 5 sec is
$$
\begin{align}
P\left( {X \leq 5}\right) 
&= {\int }_{-\infty }^{5}f\left( x\right) {dx} \\
&= {\int }_{.5}^{5}{.15}{e}^{-{.15}\left( {x - {.5}}\right) }{dx} \\
&= {.15}{e}^{.075}{\int }_{.5}^{5}{e}^{-{.15x}}{dx} \\
&= {.15}{e}^{.075} \cdot \left( {-{\left. \frac{1}{.15}{e}^{-{.15x}}\right| }_{x = {.5}}^{x = 5}}\right) \\
&= {e}^{.075}\left( {-{e}^{-{.75}} + {e}^{-{.075}}}\right) \\
&= {1.078}\left( {-{.472} + {.928}}\right) \\
&= {.491} \\
&= P\left( {\text{less than }5\mathrm{{sec}}}\right) \\
&= P\left( {X < 5}\right)
\end{align}
$$
