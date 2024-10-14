D. 1 双胞胎悖论。 Mamoru教授在一所大学的计算机科学与数学楼授课，该楼有 $F = {30}$ 层。

(1)假设楼层是独立的，并且乘坐电梯的人选择每个楼层的概率相同。需要有多少人乘坐电梯，才能使得两个人去同一楼层的概率超过一半(概率大于一半)？

(提示:使用 ${e}^{-x} = 1 - x + \ldots$ 的泰勒级数展开，并给出解的近似一般表达式。)

(2)Mamoru教授很受欢迎，他的楼层实际上比其他楼层更有可能被选中。假设所有其他楼层被选中的概率相同，推导出两个人去同一楼层的概率的一般表达式，使用之前的相同近似。当Mamoru教授的楼层被选中的概率为.25、.35或.5时，需要有多少人乘坐电梯，才能使得两个人去同一楼层的概率较大？当 $q = {.5}$ ，如果楼层数改为 $F = 1,{000}$ ，答案会改变吗？

(3) 在(1)和(2)中假设的概率模型都是简单模型。如果你能够获取电梯管理员收集的数据，你将如何定义一个更真实可靠的模型？

D. 2 估计标签偏差。设 $\mathcal{D}$ 是 $X$ 上的一个分布，$f : X \times \{ - 1, + 1\}$ 是一个标记函数。假设我们希望找到分布 $\mathcal{D}$ 的标签偏差的一个好的近似，即 ${p}_{ + }$ 的定义如下:

$$
{p}_{ + } = \underset{x \sim \mathcal{D}}{\mathbb{P}}\left\lbrack {f\left( x\right) = + 1}\right\rbrack \tag{D.27}
$$

设 $\mathcal{S}$ 是一个大小为 $m$ 的有限标记样本，独立同分布地根据 $\mathcal{D}$ 抽取。使用 $\mathcal{S}$ 推导出 ${p}_{ + }$ 的估计 ${\widehat{p}}_{ + }$。证明对于任何 $\delta > 0$ ，以至少 $1 - \delta ,\left| {{p}_{ + } - {\widehat{p}}_{ + }}\right| \leq$ 的概率 $\sqrt{\frac{\log \left( {2/\delta }\right) }{2m}}$。

D. 3 偏斜的硬币。Moent教授口袋里有两枚硬币，$\operatorname{coin}{x}_{A}$ 和 $\operatorname{coin}{x}_{B}$。两枚硬币都略有偏斜，即 $\mathbb{P}\left\lbrack {{x}_{A} = 0}\right\rbrack = 1/2 - \epsilon /2$ 和 $\widetilde{\mathbb{P}}\left\lbrack {{x}_{B} = 0}\right\rbrack = 1/2 + \epsilon /2$，其中 $0 < \epsilon < 1$ 是一个小正数，0 表示正面，1 表示反面。他喜欢和学生玩以下游戏。他随机地从口袋里挑选一枚硬币 $x \in \left\{ {{x}_{A},{x}_{B}}\right\}$，抛掷它 $m$ 次，展示出 $0\mathrm{\;s}$ 和 $1\mathrm{\;s}$ 得到的序列，并询问抛掷的是哪枚硬币。确定 $m$ 需要有多大，才能使得学生的硬币预测误差至多 $\delta > 0$。

(a) 设 $S$ 是一个大小为 $m$ 的样本。Moent教授最优秀的学生Oskar，按照决策规则 ${f}_{o} : \{ 0,1{\} }^{m} \rightarrow \left\{ {{x}_{A},{x}_{B}}\right\}$ 进行游戏，该规则定义为当 ${f}_{o}\left( S\right) = {x}_{A}$ 当且仅当 $N\left( S\right) < m/2$，其中 $N\left( S\right)$ 是样本 $S$ 中0的数量。

Suppose $m$ is even, then show that

$$
\operatorname{error}\left( {f}_{o}\right) \geq \frac{1}{2}\mathbb{P}\left\lbrack {N\left( S\right) \geq \frac{m}{2} \mid x = {x}_{A}}\right\rbrack . \tag{D.28}
$$

(b) Assuming $m$ even, show that

$$
\operatorname{error}\left( {f}_{o}\right) > \frac{1}{4}\left\lbrack {1 - {\left\lbrack 1 - {e}^{-\frac{m{\epsilon }^{2}}{1 - {\epsilon }^{2}}}\right\rbrack }^{\frac{1}{2}}}\right\rbrack . \tag{D.29}
$$

(c) Argue that if $m$ is odd, the probability can be lower bounded by using $m + 1$ in the bound in (a) and conclude that for both odd and even $m$ ,

$$
\operatorname{error}\left( {f}_{o}\right) > \frac{1}{4}\left\lbrack {1 - {\left\lbrack 1 - {e}^{-\frac{2\lceil m/2\rceil {\epsilon }^{2}}{1 - {\epsilon }^{2}}}\right\rbrack }^{\frac{1}{2}}}\right\rbrack . \tag{D.30}
$$

(d) Using this bound, how large must $m$ be if Oskar’s error is at most $\delta$ , where $0 < \delta < 1/4$ . What is the asymptotic behavior of this lower bound as a function of $\epsilon$ ?

(e) Show that no decision rule $f : \{ 0,1{\} }^{m} \rightarrow \left\{ {{x}_{A},{x}_{B}}\right\}$ can do better than Oskar’s rule ${f}_{o}$ . Conclude that the lower bound of the previous question applies to all rules.

D. 4 Concentration bounds. Let $X$ be a non-negative random variable satisfying $\mathbb{P}\left\lbrack {X > t}\right\rbrack \leq$ $c{e}^{-{2m}{t}^{2}}$ for all $t > 0$ and some $c > 0$ . Show that $\mathbb{E}\left\lbrack {X}^{2}\right\rbrack \leq \frac{\log \left( {ce}\right) }{2m}$ (Hint: to do that, use the

identity $\mathbb{E}\left\lbrack {X}^{2}\right\rbrack = {\int }_{0}^{+\infty }\mathbb{P}\left\lbrack {{X}^{2} > t}\right\rbrack {dt}$ , write ${\int }_{0}^{+\infty } = {\int }_{0}^{u} + {\int }_{u}^{+\infty }$ , bound the first term by $u$ and find the best $u$ to minimize the upper bound).

D. 5 Comparison of Hoeffding’s and Chebyshev’s inequalities. Let ${X}_{1},\ldots ,{X}_{m}$ be a sequence of random variables taking values in $\left\lbrack {0,1}\right\rbrack$ with the same mean $\mu$ and variance ${\sigma }^{2} < \infty$ and let $\overline{X} = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i}.$

(a) For any $\epsilon > 0$ , give a bound on $\mathbb{P}\left\lbrack {\left| {\bar{X} - \mu }\right| > \epsilon }\right\rbrack$ using Chebyshev’s inequality, then Hoeffd-ing’s inequality. For what values of $\sigma$ is Chebyshev’s inequality tighter?

(b) 假设随机变量 ${X}_{i}$ 取值在 $\{ 0,1\}$ 中。证明 ${\sigma }^{2} \leq \frac{1}{4}$ 。使用这个结果简化切比雪夫不等式。选择 $\epsilon = {.05}$ 并绘制修改后的切比雪夫不等式和作为 $m$ 函数的霍夫丁不等式(你可以使用你偏好的程序来生成图形)。

D. 6 贝内特和伯恩斯坦不等式。这个问题的目标是证明这两个不等式。

(a) 证明对于任意的 $t > 0$ ，以及任意的随机变量 $X$ ，当 $\mathbb{E}\left\lbrack X\right\rbrack = 0,\mathbb{E}\left\lbrack {X}^{2}\right\rbrack = {\sigma }^{2}$ 时，

$X \leq c$

$$
\mathbb{E}\left\lbrack {e}^{tX}\right\rbrack \leq {e}^{f\left( {{\sigma }^{2}/{c}^{2}}\right) } \tag{D.31}
$$

其中

$$
f\left( x\right) = \log \left( {\frac{1}{1 + x}{e}^{-{ctx}} + \frac{x}{1 + x}{e}^{ct}}\right) .
$$

(b) 证明 ${f}^{\prime \prime }\left( x\right) \leq 0$ 对于 $x \geq 0$ 成立。

(c) 使用切尔诺夫界技术，证明

$$
\mathbb{P}\left\lbrack {\frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i} \geq \epsilon }\right\rbrack \leq {e}^{-{tm\epsilon } + \mathop{\sum }\limits_{{i = 1}}^{m}f\left( {{\sigma }_{{X}_{i}}^{2}/{c}^{2}}\right) }
$$

其中 $\left( {\sigma }_{{X}_{i}}^{2}\right.$ 是 ${X}_{i}$ 的方差。

(d) 证明 $f\left( x\right) \leq f\left( 0\right) + x{f}^{\prime }\left( 0\right) = \left( {{e}^{ct} - 1 - {ct}}\right) x$ 。

(e) 使用 (4) 中导出的界，找到 $t$ 的最优值。

(f) 贝内特不等式。设 ${X}_{1},\ldots ,{X}_{m}$ 为独立实值随机变量，均值为零，满足对于 $i = 1,\ldots , m,{X}_{i} \leq c$ 。设 ${\sigma }^{2} = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{{X}_{i}}^{2}$ 。证明

$$
\mathbb{P}\left\lbrack {\frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i} > \epsilon }\right\rbrack \leq \exp \left( {-\frac{m{\sigma }^{2}}{{c}^{2}}\theta \left( \frac{\epsilon c}{{\sigma }^{2}}\right) }\right) \tag{D. 32}
$$

其中 $\theta \left( x\right) = \left( {1 + x}\right) \log \left( {1 + x}\right) - x$ 。

(g) 伯恩斯坦不等式。在贝内特不等式相同的条件下，证明

$$
\mathbb{P}\left\lbrack {\frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i} > \epsilon }\right\rbrack \leq \exp \left( {-\frac{m{\epsilon }^{2}}{2{\sigma }^{2} + {2c\epsilon }/3}}\right) . \tag{D.33}
$$

(提示:证明对于所有 $x \geq 0,\theta \left( x\right) \geq h\left( x\right) = \frac{3}{2}\frac{{x}^{2}}{x + 3}$ 。)

(h) 假设相同条件下写出霍夫丁不等式。对于哪些 $\sigma$ 的值，伯恩斯坦不等式比霍夫丁不等式更好？

D. 7 指数不等式。设 $X$ 为遵循二项分布 $B\left( {m, p}\right)$ 的随机变量。

(a) 使用桑诺夫不等式证明以下指数不等式对于任意

$\epsilon > 0$ 成立:

$$
\mathbb{P}\left\lbrack {\frac{X}{m} - p > \epsilon }\right\rbrack \leq {\left\lbrack {\left( \frac{p}{p + \epsilon }\right) }^{p + \epsilon }{\left( \frac{1 - p}{1 - \left( {p + \epsilon }\right) }\right) }^{1 - \left( {p + \epsilon }\right) }\right\rbrack }^{m}. \tag{D.34}
$$

(b) 使用上述结果证明以下成立:

$$
\mathbb{P}\left\lbrack {\frac{X}{m} - p > \epsilon }\right\rbrack \leq {\left( \frac{p}{p + \epsilon }\right) }^{m\left( {p + \epsilon }\right) }{e}^{m\epsilon } \tag{D. 35}
$$

(c) 证明

$$
\mathbb{P}\left\lbrack {\frac{X}{m} - p > \epsilon }\right\rbrack \leq {e}^{-{mp\theta }\left( \frac{\epsilon }{p}\right) } \tag{D. 36}
$$

其中 $\theta$ 如练习 D.6 中定义。