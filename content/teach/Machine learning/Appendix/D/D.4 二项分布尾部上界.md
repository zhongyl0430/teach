设 ${X}_{1},\ldots ,{X}_{m}$ 为独立随机变量，取值在 $\{ 0,1\}$ 中，且 $\mathbb{P}\left\lbrack {{X}_{i} = 1}\right\rbrack = p \in$ $\left\lbrack {0,1}\right\rbrack$ 对于 $i = 1,\ldots , m$ 。那么，$\mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i}$ 服从二项分布 $B\left( {m, p}\right)$ 。我们将用 $\bar{X}$ 表示平均值 $\bar{X} = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{\bar{X}}_{i}$ 。然后，以下等式和不等式成立:

$$
\mathbb{P}\left\lbrack {\bar{X} - p > \epsilon }\right\rbrack = \mathop{\sum }\limits_{{k = \lceil \left( {p + \epsilon }\right) m\rceil }}^{m}\left( \begin{matrix} m \\ k \end{matrix}\right) {p}^{k}{\left( 1 - p\right) }^{m - k} \tag{Binomial formula}
$$

$$
\mathbb{P}\left\lbrack {\bar{X} - p > \epsilon }\right\rbrack \leq {e}^{-{2m}{\epsilon }^{2}} \tag{Hoeffding's inequality}
$$

$$
\mathbb{P}\left\lbrack {\bar{X} - p > \epsilon }\right\rbrack \leq {e}^{-\frac{m{\epsilon }^{2}}{2{\sigma }^{2} + \frac{2\epsilon }{3}}} \tag{Bernstein's inequality}
$$

$$
\mathbb{P}\left\lbrack {\overline{X} - p > \epsilon }\right\rbrack \leq {e}^{-m{\sigma }^{2}\theta \left( \frac{\epsilon }{{\sigma }^{2}}\right) } \tag{Bennett's inequality}
$$

$$
\mathbb{P}\left\lbrack {\bar{X} - p > \epsilon }\right\rbrack \leq {e}^{-m\mathrm{D}\left( {p + \epsilon \parallel p}\right) } \tag{Sanov's inequality,}
$$

其中 ${\sigma }^{2} = p\left( {1 - p}\right) = \operatorname{Var}\left\lbrack {X}_{i}\right\rbrack$ 和 $\theta \left( x\right) = \left( {1 + x}\right) \log \left( {1 + x}\right) - x$ 。最后三个不等式在练习 D.6 和 D.7 中有所展示。例如，使用伯恩斯坦不等式，我们可以看到对于 $\epsilon$ 相对较小，即 $\epsilon \ll 2{\sigma }^{2}$ ，上界大致呈 ${e}^{-\frac{m{\epsilon }^{2}}{2{\sigma }^{2}}}$ 的形式，因此表现出高斯行为。对于 $\epsilon \gg 2{\sigma }^{2},{e}^{-\frac{3m\epsilon }{2}}$ ，上界表现出泊松行为。

图 D.1 展示了这些界限对于不同方差 ${\sigma }^{2} = p\left( {1 - p}\right)$ 的值的比较:小方差 $\left( {p = {.05}}\right)$ ，大方差 $\left( {p = {.5}}\right)$ 。