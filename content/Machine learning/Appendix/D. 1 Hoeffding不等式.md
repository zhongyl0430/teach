我们首先介绍Hoeffding不等式，其证明使用了通用Chernoff界技术。给定一个随机变量 $X$ 和 $\epsilon > 0$ ，这种技术包括以下步骤来界定 $\mathbb{P}\left\lbrack {X \geq \epsilon }\right\rbrack$ 。对于任何 $t > 0$ ，首先使用Markov不等式来界定 $\mathbb{P}\left\lbrack {X \geq \epsilon }\right\rbrack$ :
$$
\mathbb{P}\left\lbrack {X \geq \epsilon }\right\rbrack = \mathbb{P}\left\lbrack {{e}^{tX} \geq {e}^{t\epsilon }}\right\rbrack \leq {e}^{-{t\epsilon }}\mathbb{E}\left\lbrack {e}^{tX}\right\rbrack . \tag{D.1}
$$

然后，为 $\mathbb{E}\left\lbrack {e}^{tX}\right\rbrack$ 找到一个上界 $g\left( t\right)$ ，并选择 $t$ 以最小化 ${e}^{-{t\epsilon }}g\left( t\right)$ 。
对于Hoeffding不等式，以下引理为 $\mathbb{E}\left\lbrack {e}^{tX}\right\rbrack$ 提供了一个上界。

[[引理D.1 Hoeffding引理]]

该引理可用于证明以下结果，即Hoeffding不等式。

[[定理 D.2 Hoeffding 不等式]]

当每个随机变量 ${\sigma }_{{X}_{i}}^{2}$ 的方差 ${X}_{i}$ 已知且 ${\sigma }_{{X}_{i}}^{2}$ 相对较小时，可以推导出更好的集中界(见练习 D.6 中证明的 Bennett 和 Bernstein 不等式)。