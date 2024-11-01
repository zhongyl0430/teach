Reconsider the situation of Examples 5.3 and 5.4 involving $X =$ the proportion of time that a bank’s drive-up facility is busy and $Y =$ the analogous proportion for the walk-up window. The conditional pdf of $Y$ given that $X = {.8}$ is
$$
{f}_{Y \mid X}\left( {y \mid {.8}}\right) = \frac{f\left( {{.8}, y}\right) }{{f}_{X}\left( {.8}\right) } = \frac{{1.2}\left( {{.8} + {y}^{2}}\right) }{{1.2}\left( {.8}\right) + {.4}} = \frac{1}{34}\left( {{24} + {30}{y}^{2}}\right) \;0 < y < 1
$$

The probability that the walk-up facility is busy at most half the time given that $X = {.8}$ is then
$$
P\left( {Y \leq {.5} \mid X = {.8}}\right) = {\int }_{-\infty }^{.5}{f}_{Y \mid X}\left( {y \mid {.8}}\right) {dy} = {\int }_{0}^{.5}\frac{1}{34}\left( {{24} + {30}{y}^{2}}\right) {dy} = {.390}
$$

Using the marginal pdf of $Y$ gives $P\left( {Y \leq {.5}}\right) = {.350}$. Also $E\left( Y\right) = {.6}$, whereas the expected proportion of time that the walk-up facility is busy given that $X = {.8}$ (a conditional expectation) is
$$
E\left( {Y \mid X = {.8}}\right) = {\int }_{-\infty }^{\infty }y \cdot {f}_{Y \mid X}\left( {y \mid {.8}}\right) {dy} = \frac{1}{34}{\int }_{0}^{1}y\left( {{24} + {30}{y}^{2}}\right) {dy} = {.574}
$$
