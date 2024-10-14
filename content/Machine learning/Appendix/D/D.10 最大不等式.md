
下面给出了有限集合的随机变量的最大值的期望的一个上界，这在几个上下文中很有用。

定理 D.10(最大不等式)设 ${X}_{1}\ldots {X}_{n}$ 是 $n \geq 1$ 实值随机变量，使得对于所有 $j \in \left\lbrack n\right\rbrack$ 和 $t > 0,\mathbb{E}\left\lbrack {e}^{t{X}_{j}}\right\rbrack \leq {e}^{\frac{{t}^{2}{r}^{2}}{2}}$ 对于某个 $r > 0$ 。那么，以下不等式

成立:

$$
\mathbb{E}\left\lbrack {\mathop{\max }\limits_{{j \in \left\lbrack n\right\rbrack }}{X}_{j}}\right\rbrack \leq r\sqrt{2\log n}
$$

证明:对于任意的 $t > 0$ ，由于指数函数的凸性和Jensen不等式，以下成立:

$$
{e}^{t\mathbb{E}\left\lbrack {\mathop{\max }\limits_{{j \in \left\lbrack n\right\rbrack }}{X}_{j}}\right\rbrack } \leq \mathbb{E}\left\lbrack {e}^{t\mathop{\max }\limits_{{j \in \left\lbrack n\right\rbrack }}{X}_{j}}\right\rbrack = \mathbb{E}\left\lbrack {\mathop{\max }\limits_{{j \in \left\lbrack n\right\rbrack }}{e}^{t{X}_{j}}}\right\rbrack \leq \mathbb{E}\left\lbrack {\mathop{\sum }\limits_{{j \in \left\lbrack n\right\rbrack }}{e}^{t{X}_{j}}}\right\rbrack \leq n{e}^{\frac{{t}^{2}{r}^{2}}{2}}.
$$

对两边取对数得到

$$
\mathbb{E}\left\lbrack {\mathop{\max }\limits_{{j \in \left\lbrack n\right\rbrack }}{X}_{j}}\right\rbrack \leq \frac{\log n}{t} + \frac{t{r}^{2}}{2} \tag{D.25}
$$

选择 $t = \frac{\sqrt{2\log n}}{r}$ ，它最小化了右边，给出了上界 $r\sqrt{2\log n}$ 。注意，考虑到它们的矩生成函数的表达式(方程(C.24))，对于标准高斯随机变量 ${X}_{j}$ ，定理的假设成立且为等式:$\mathbb{E}\left\lbrack {e}^{t{X}_{j}}\right\rbrack = {e}^{\frac{{t}^{2}}{2}}$

推论 D.11(最大不等式)设 ${X}_{1}\ldots {X}_{n}$ 为 $n \geq 1$ 实值随机变量，满足对于所有 $j \in \left\lbrack n\right\rbrack ,{X}_{j} = \mathop{\sum }\limits_{{i = 1}}^{m}{Y}_{ij}$ ，其中，对于每个固定的 $j \in \left\lbrack n\right\rbrack ,{Y}_{ij}$ 是独立的均值为零的随机变量，取值在 $\left\lbrack {-{r}_{i}, + {r}_{i}}\right\rbrack$ 中，对于某个 ${r}_{i} > 0$ 。那么，以下不等式成立:
$$
\mathbb{E}\left\lbrack {\mathop{\max }\limits_{{j \in \left\lbrack n\right\rbrack }}{X}_{j}}\right\rbrack \leq r\sqrt{2\log n}
$$

其中 $r = \sqrt{\mathop{\sum }\limits_{{i = 1}}^{m}{r}_{i}^{2}}$ 。

证明:由于 ${Y}_{ij}$ 对于固定的 $j$ 是独立的，以及根据Hoeffding引理(引理D.1)，以下不等式对于所有 $j \in \left\lbrack n\right\rbrack$ 成立:

$$
\mathbb{E}\left\lbrack {e}^{t{X}_{j}}\right\rbrack = \mathbb{E}\left\lbrack {\mathop{\prod }\limits_{{i = 1}}^{m}{e}^{t{Y}_{ij}}}\right\rbrack = \mathop{\prod }\limits_{{i = 1}}^{m}\mathbb{E}\left\lbrack {e}^{t{Y}_{ij}}\right\rbrack \leq \mathop{\prod }\limits_{{i = 1}}^{m}{e}^{\frac{{t}^{2}{r}_{j}^{2}}{2}} = {e}^{\frac{{t}^{2}{r}^{2}}{2}}, \tag{D.26}
$$

其中 ${r}^{2} = \mathop{\sum }\limits_{{i = 1}}^{m}{r}_{i}^{2}$ 。然后，结果立即由定理D.10得出。