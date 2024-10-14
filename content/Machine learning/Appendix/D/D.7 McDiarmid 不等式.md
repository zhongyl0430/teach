## D.7 McDiarmid 不等式

下面是本节的主要结果。其证明利用了 Azuma 不等式。

定理 D.8(McDiarmid 不等式)${Let}\;{X}_{1},\ldots ,{X}_{m} \in {\mathfrak{X}}^{m}\;{be}\;a\;{set}\;{of}\;m \geq 1\;{independent}$ 随机变量，并假设存在 ${c}_{1},\ldots ,{c}_{m} > 0$ 使得 $f : {\mathcal{X}}^{m} \rightarrow \mathbb{R}$ 满足以下条件:

$$
\left| {f\left( {{x}_{1},\ldots ,{x}_{i},\ldots ,{x}_{m}}\right) - f\left( {{x}_{1},\ldots ,{x}_{i}^{\prime },\ldots {x}_{m}}\right) }\right| \leq {c}_{i}, \tag{D.15}
$$

对于所有 $i \in \left\lbrack m\right\rbrack$ 和任意点 ${x}_{1},\ldots ,{x}_{m},{x}_{i}^{\prime } \in \mathfrak{X}$ 。设 $f\left( S\right)$ 表示 $f\left( {{X}_{1},\ldots ,{X}_{m}}\right)$ ，那么，对于所有 $\epsilon > 0$ ，以下不等式成立:

$$
\mathbb{P}\left\lbrack {f\left( S\right) - \mathbb{E}\left\lbrack {f\left( S\right) }\right\rbrack \geq \epsilon }\right\rbrack \leq \exp \left( \frac{-2{\epsilon }^{2}}{\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}^{2}}\right) \tag{D.16}
$$

$$
\mathbb{P}\left\lbrack {f\left( S\right) - \mathbb{E}\left\lbrack {f\left( S\right) }\right\rbrack \leq - \epsilon }\right\rbrack \leq \exp \left( \frac{-2{\epsilon }^{2}}{\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}^{2}}\right) . \tag{D.17}
$$

证明:定义一个随机变量序列 ${V}_{k}, k \in \left\lbrack m\right\rbrack$ ，如下:$V = f\left( S\right) - \mathbb{E}\left\lbrack {f\left( S\right) }\right\rbrack$ ，${V}_{1} = \mathbb{E}\left\lbrack {V \mid {X}_{1}}\right\rbrack - \mathbb{E}\left\lbrack V\right\rbrack$ ，对于 $k > 1$ ，

$$
{V}_{k} = \mathbb{E}\left\lbrack {V \mid {X}_{1},\ldots ,{X}_{k}}\right\rbrack - \mathbb{E}\left\lbrack {V \mid {X}_{1},\ldots ,{X}_{k - 1}}\right\rbrack .
$$

注意到 $V = \mathop{\sum }\limits_{{k = 1}}^{m}{V}_{k}$。此外，随机变量 $\mathbb{E}\left\lbrack {V \mid {X}_{1},\ldots ,{X}_{k}}\right\rbrack$ 是 ${X}_{1},\ldots ,{X}_{k}$ 的一个函数。因此，给定 ${X}_{1},\ldots ,{X}_{k - 1}$ 并取其期望为：
$$
\mathbb{E}\left\lbrack {\mathbb{E}\left\lbrack {V \mid {X}_{1},\ldots ,{X}_{k}}\right\rbrack \mid {X}_{1},\ldots ,{X}_{k - 1}}\right\rbrack = \mathbb{E}\left\lbrack {V \mid {X}_{1},\ldots ,{X}_{k - 1}}\right\rbrack
$$
这意味着 $\mathbb{E}\left\lbrack {{V}_{k} \mid {X}_{1},\ldots ,{X}_{k - 1}}\right\rbrack = 0$。因此，序列 ${\left( {V}_{k}\right) }_{k \in \left\lbrack m\right\rbrack }$ 是一个马尔可夫差分序列。接下来，观察到，由于 $\mathbb{E}\left\lbrack {f\left( S\right) }\right\rbrack$ 是一个标量，${V}_{k}$ 可以表示如下：
$$
{V}_{k} = \mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k}}\right\rbrack - \mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k - 1}}\right\rbrack .
$$

因此，我们可以通过以下方式为 ${V}_{k}$ 定义上界 ${W}_{k}$ 和下界 ${U}_{k}$：
$$
{W}_{k} = \mathop{\sup }\limits_{x}\mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k - 1}, x}\right\rbrack - \mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k - 1}}\right\rbrack
$$

$$
{U}_{k} = \mathop{\inf }\limits_{x}\mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k - 1}, x}\right\rbrack - \mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k - 1}}\right\rbrack .
$$

现在，根据 (D.15)，对于任何 $k \in \left\lbrack m\right\rbrack$，以下关系成立：
$$
{W}_{k} - {U}_{k} = \mathop{\sup }\limits_{{x,{x}^{\prime }}}\mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k - 1}, x}\right\rbrack - \mathbb{E}\left\lbrack {f\left( S\right) \mid {X}_{1},\ldots ,{X}_{k - 1},{x}^{\prime }}\right\rbrack \leq {c}_{k}, \tag{D.18}
$$
因此，${U}_{k} \leq {V}_{k} \leq {U}_{k} + {c}_{k}$。考虑到这些不等式，我们可以将阿祖玛不等式应用于 $V = \mathop{\sum }\limits_{{k = 1}}^{m}{V}_{k}$，这正好得出 (D.16) 和 (D.17)。

McDiarmid 不等式在本书中的多个证明中都有使用。它可以从稳定性的角度理解：如果改变其任何一个参数仅在有限的范围内影响 $f$，那么 $f$ 相对于其均值的偏差可以被指数界定。还要注意，Hoeffding 不等式（定理 D.2）是 McDiarmid 不等式的一个特例，其中 $f$ 定义为
$$f : \left( {{x}_{1},\ldots ,{x}_{m}}\right) \mapsto \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{x}_{i} .$$