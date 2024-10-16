本节介绍了凸集和凸函数的概念。凸函数在学习和算法的设计和分析中扮演着重要的角色，部分原因是因为凸函数的局部最小值必然也是全局最小值。
因此，通过找到凸优化的局部最小值来学习假设的性质通常很清楚，而对于一些非凸优化问题，可能存在非常多的局部最小值，对于这些局部最小值，无法给出学习假设的明确特征。

> [!definition] 定义 B.4 凸集
> $A\;{{set}\;X} \subseteq {\mathbb{R}}^{N}\;{is}\;{said}\;{to}\;{be}\;$ 是凸的 $\;{if}\;{for}\;{any}\;{two}\;{points}\;\mathbf{x},\mathbf{y} \in X$ 段 $\left\lbrack {\mathbf{x},\mathbf{y}}\right\rbrack$ 位于 $\mathcal{X}$ 中，即
> $$
> \{ \alpha \mathbf{x} + \left( {1 - \alpha }\right) \mathbf{y} : 0 \leq \alpha \leq 1\} \subseteq X.
> $$

图 B. 1
凸函数(左)和凹函数(右)的示例。
注意，在凸函数上任意两点之间画的线段完全位于函数图形的上方，而在凹函数上任意两点之间画的线段完全位于函数图形的下方。
![01928a40-c638-783b-803a-1bf2444d1c2b_1_464_257_895_343_0.jpg](images/01928a40-c638-783b-803a-1bf2444d1c2b_1_464_257_895_343_0.jpg)

下面的引理说明了几个保持凸性的凸集上的运算。这些运算对于证明本节中的几个后续结果将非常有用。

> [!lemma] 引理B.5 保持集合凸性的运算
> ${The}\;{following}\;{operations}\;{on}\;{convex}$ 集合保持凸性:
> - 设 ${\left\{ {\mathcal{C}}_{i}\right\} }_{i \in I}$ 为任意集合族，其中对于所有 $i \in I$ ，集合 ${\mathcal{C}}_{i}$ 是凸的。那么这些集合的交集 $\mathop{\bigcap }\limits_{{i \in I}}{\mathcal{C}}_{i}$ 也是凸的。
> - 设 ${\mathcal{C}}_{1}$ 和 ${\mathcal{C}}_{2}$ 为凸集，那么它们的和 ${\mathcal{C}}_{1} + {\mathcal{C}}_{2} = \left\{ {{x}_{1} + {x}_{2} : {x}_{1} \in {\mathcal{C}}_{1},{x}_{2} \in {\mathcal{C}}_{2}}\right\}$ (当定义时)是凸的。
> - 设 ${\mathcal{C}}_{1}$ 和 ${\mathcal{C}}_{2}$ 为凸集，那么它们的笛卡尔积 $\left( {{\mathcal{C}}_{1} \times {\mathcal{C}}_{2}}\right)$ 也是凸的。
> - 任意凸集 $\mathcal{C}$ 的投影也是凸的。

证明:

第一个性质成立，因为对于任意的 $x, y \in \mathop{\bigcap }\limits_{{i \in I}}{\mathcal{C}}_{i}$ 和任意的 $\alpha \in \left\lbrack {0,1}\right\rbrack$ ，由于 ${\mathcal{C}}_{i}$ 的凸性，我们有 ${\alpha x} +$ $\left( {1 - \alpha }\right) y \in {\mathcal{C}}_{i}$ 对于任意的 $i \in I$ 成立。

第二个性质成立，因为对于任意的 $\left( {{x}_{1} + {x}_{2}}\right) ,\left( {{y}_{1} + {y}_{2}}\right) \in \left( {{\mathcal{C}}_{1} + {\mathcal{C}}_{2}}\right)$ 我们有 $\alpha \left( {{x}_{1} + }\right.$ $\left. {x}_{2}\right) + \left( {1 - \alpha }\right) \left( {{y}_{1} + {y}_{2}}\right) = \left( {\alpha {x}_{1} + \left( {1 - \alpha }\right) {y}_{1} + \alpha {x}_{2} + \left( {1 - \alpha }\right) {y}_{2}}\right) \in \left( {{\mathrm{C}}_{1} + {\mathrm{C}}_{2}}\right)$ ，这是由于 $\alpha {x}_{1} + \left( {1 - \alpha }\right) {y}_{1} \in {\mathcal{C}}_{1}$ 和 $\alpha {x}_{2} + \left( {1 - \alpha }\right) {y}_{2} \in {\mathcal{C}}_{2}$ 。

第三个性质成立，因为对于 $\left( {{x}_{1},{x}_{2}}\right) ,\left( {{y}_{1},{y}_{2}}\right) \in \left( {{\mathrm{C}}_{1} \times {\mathrm{C}}_{2}}\right)$ 我们有 $\alpha \left( {{x}_{1},{x}_{2}}\right) + (1 -$ $\alpha )\left( {{y}_{1},{y}_{2}}\right) = \left( {\alpha {x}_{1} + \left( {1 - \alpha }\right) {y}_{1},\alpha {x}_{2} + \left( {1 - \alpha }\right) {y}_{2}}\right) \in \left( {{\mathcal{C}}_{1} \times {\mathcal{C}}_{2}}\right)$ ，其中成员资格成立是由于假设 ${\mathcal{C}}_{1}$ 和 ${\mathcal{C}}_{2}$ 是凸的。

最后，第四个性质成立，因为对于任意将凸集 $\mathcal{C}$ 分解为投影 ${\mathcal{C}}_{1}$ 和 ${\mathcal{C}}_{2}$ 的情况，使得 $\mathcal{C} = \left( {{\mathcal{C}}_{1} \times {\mathcal{C}}_{2}}\right)$ ，必然有 ${\mathcal{C}}_{1}$ 是凸的。如果 ${\mathcal{C}}_{2}$ 是空的，那么结果显然成立。否则，固定一个元素 ${x}_{2} \in {\mathcal{C}}_{2}$ ，那么对于任意的 $x, y \in {\mathcal{C}}_{1}$ 和任意的 $\alpha \in \left\lbrack {0,1}\right\rbrack$ ，我们有 $\alpha \left( {x,{x}_{2}}\right) + \left( {1 - \alpha }\right) \left( {y,{x}_{2}}\right) \in \mathcal{C}$ ，这意味着 ${\alpha x} + \left( {1 - \alpha }\right) y \in {\mathcal{C}}_{1}$ 。由于 ${\mathcal{C}}_{1}$ 是任意选择的，这一事实对于 $\mathcal{C}$ 的任何投影都成立。

注意，许多集合运算可能不会保持凸性。考虑 $\mathbb{R} : \left\lbrack {a, b}\right\rbrack \cup \left\lbrack {c, d}\right\rbrack$ 上的不相交区间的并集，其中 $a < b < c < d$ 。显然 $\left\lbrack {a, b}\right\rbrack$ 和 $\left\lbrack {c, d}\right\rbrack$ 是凸的，然而我们有 $\frac{1}{2}b + \left( {1 - \frac{1}{2}}\right) c \notin \left( {\left\lbrack {a, b}\right\rbrack \cup \left\lbrack {c, d}\right\rbrack }\right)$ 。

> [!definition] 定义 B.6 凸包
> 一个点集 $X \subseteq {\mathbb{R}}^{N}$ 的凸包 conv(X) 是包含 $x$ 的最小凸集，也可以等价地定义如下:
> $$
> \operatorname{conv}\left( \mathcal{X}\right) = \left\{ {\mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i}{\mathbf{x}}_{i} : m \geq 1,\forall i \in \left\lbrack m\right\rbrack ,{\mathbf{x}}_{i} \in \mathcal{X},{\alpha }_{i} \geq 0,\mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i} = 1}\right\} . \tag{B.1}
> $$

令 Epi $f$ 表示函数 $f : X \rightarrow \mathbb{R}$ 的上图形，即位于其图形上方的点集:$\{ \left( {x, y}\right) : x \in X, y \geq f\left( x\right) \}$ 。

图 B.2
所有凸函数满足的一阶性质的图示。
![01928a40-c638-783b-803a-1bf2444d1c2b_2_545_255_712_530_0.jpg](images/01928a40-c638-783b-803a-1bf2444d1c2b_2_545_255_712_530_0.jpg)

> [!definition] 定义 B.7 凸函数
> 令 $X$ 为一个凸集。如果函数 $f : X \rightarrow \mathbb{R}$ 的上图形 Epi $f$ 是一个凸集，或者等价地，对于所有的 $\mathbf{x},\mathbf{y} \in X$ 和 $\alpha \in \left\lbrack {0,1}\right\rbrack$ ，
> $$
> f\left( {\alpha \mathbf{x} + \left( {1 - \alpha }\right) \mathbf{y}}\right) \leq {\alpha f}\left( \mathbf{x}\right) + \left( {1 - \alpha }\right) f\left( \mathbf{y}\right) . \tag{B.2}
> $$

$f$ 在不等式 (B.2) 对于所有 $\mathbf{x} \neq \mathbf{y}$ 和 $\alpha \in \left( {0,1}\right)$ 严格成立时，被称为严格凸。当 $- f$ 是(严格)凸时，$f$ 被称为(严格)凹。图 B.1 展示了凸和凹函数的简单示例。凸函数也可以用其一阶或二阶微分来表征。

> [!definition] 定理 B.8 
> 设 $f$ 是一个可微函数，那么 $f$ 是凸的当且仅当 $\operatorname{dom}\left( f\right)$ 是凸的，并且以下不等式成立:
> $$
> \forall \mathbf{x},\mathbf{y} \in \operatorname{dom}\left( f\right) , f\left( \mathbf{y}\right) - f\left( \mathbf{x}\right) \geq \nabla f\left( \mathbf{x}\right) \cdot \left( {\mathbf{y} - \mathbf{x}}\right) . \tag{B.3}
> $$

性质 (B.3) 由图 B.2 说明:对于凸函数，其在 $\mathbf{x}$ 处的切平面总是位于图形下方。

> [!definition] 定理 B.9 
> 设 $f$ 是一个二阶可微函数，那么 $f$ 是凸的当且仅当 $\operatorname{dom}\left( f\right)$ 是凸的且其 Hessian 矩阵是半正定的:
> $$
> \forall \mathbf{x} \in \operatorname{dom}\left( f\right) ,{\nabla }^{2}f\left( \mathbf{x}\right) \succcurlyeq 0.
> $$

请记住，一个对称矩阵是半正定的当且仅当它的所有特征值都是非负的。进一步注意，当 $f$ 是标量时，该定理表明 $f$ 是凸的当且仅当其二阶导数总是非负的，即对于所有 $x \in \operatorname{dom}\left( f\right) ,{f}^{\prime \prime }\left( x\right) \geq 0$。

> [!example] 示例 B.10(线性函数)
> 任何线性函数 $f$ 既凸又凹，因为根据线性定义，方程 (B.2) 对于 $f$ 和 $- f$ 都以等式形式成立。

> [!example] 示例 B.11(二次函数)
> 定义在 $\mathbb{R}$ 上的函数 $f : x \mapsto {x}^{2}$ 是凸的，因为它是二阶可微的且对于所有 $x \in \mathbb{R},{f}^{\prime \prime }\left( x\right) = 2 > 0$。

> [!example] 示例 B.12(范数)
> 任何在凸集 $\parallel \cdot \parallel$ 上定义的范数 $x$ 都是凸的，因为根据三角不等式和范数的齐次性质，对于所有 $\alpha \in \left\lbrack {0,1}\right\rbrack ,\mathbf{x},\mathbf{y} \in \mathcal{X}$ ，我们可以写出
> $$
> \parallel \alpha \mathbf{x} + \left( {1 - \alpha }\right) \mathbf{y}\parallel \leq \parallel \alpha \mathbf{x}\parallel + \parallel \left( {1 - \alpha }\right) \mathbf{y}\parallel = \alpha \parallel \mathbf{x}\parallel + \left( {1 - \alpha }\right) \parallel \mathbf{y}\parallel .
> $$

> [!example] 示例 B.13(最大函数)
> 定义在所有 $\mathbf{x} \in {\mathbb{R}}^{N}$ 上的最大函数 $\mathbf{x} \mapsto \mathop{\max }\limits_{{j \in \left\lbrack N\right\rbrack }}{\mathbf{x}}_{j}$ 是凸的。对于所有 $\alpha \in \left\lbrack {0,1}\right\rbrack ,\mathbf{x},\mathbf{y} \in {\mathbb{R}}^{N}$ ，由于最大值的次可加性，我们可以写出
> $$
> \mathop{\max }\limits_{j}\left( {\alpha {\mathbf{x}}_{j} + \left( {1 - \alpha }\right) {\mathbf{y}}_{j}}\right) \leq \mathop{\max }\limits_{j}\left( {\alpha {\mathbf{x}}_{j}}\right) + \mathop{\max }\limits_{j}\left( {\left( {1 - \alpha }\right) {\mathbf{y}}_{j}}\right) = \alpha \mathop{\max }\limits_{j}\left( {\mathbf{x}}_{j}\right) + \left( {1 - \alpha }\right) \mathop{\max }\limits_{j}\left( {\mathbf{y}}_{j}\right) .
> $$

证明函数的凸性或凹性的一个有用方法是利用复合规则。为了简化表述，我们将假设函数具有二阶可导性，尽管即使没有这个假设，结果也可以被证明。

引理 B.14(凸/凹函数的复合)${Assume}\;h : \mathbb{R} \rightarrow \mathbb{R}\;{and}\;g : {\mathbb{R}}^{N} \rightarrow$ $\mathbb{R}$ 是二阶可导的函数，对于所有 $\mathbf{x} \in {\mathbb{R}}^{N}$ ，定义 $f\left( \mathbf{x}\right) = h\left( {g\left( \mathbf{x}\right) }\right)$ 。那么以下蕴含关系是有效的:

- $h$ 是凸的且非递减，并且 $g$ 是凸的 $\Rightarrow f$ 是凸的。

- $h$ 是凸的且非递增，并且 $g$ 是凹的 $\Rightarrow f$ 是凸的。

- $h$ 是凹的且非递减，并且 $g$ 是凹的 $\Rightarrow f$ 是凹的。

- $h$ 是凹的且非递增，并且 $g$ 是凸的 $\Rightarrow f$ 是凹的。

证明:我们限制在 $N = 1$ 上，因为这足以证明沿着穿过定义域的所有任意直线的凸性(凹性)。现在，考虑 $f$ 的二阶导数:

$$
{f}^{\prime \prime }\left( x\right) = {h}^{\prime \prime }\left( {g\left( x\right) }\right) {g}^{\prime }{\left( x\right) }^{2} + {h}^{\prime }\left( {g\left( x\right) }\right) {g}^{\prime \prime }\left( x\right) . \tag{B.4}
$$

注意，如果 $h$ 是凸的且单调不减，那么我们有 ${h}^{\prime \prime } \geq 0$ 和 ${h}^{\prime } \geq 0$ 。此外，如果 $g$ 是凸的，我们也有 ${g}^{\prime \prime } \geq 0$ ，并且可以得出 ${f}^{\prime \prime }\left( x\right) \geq 0$ ，这证明了第一个陈述。其余的陈述以类似的方式证明。

示例 B.15(函数的复合)之前的引理显示了以下复合函数的凸性或凹性:

- 如果 $f : {\mathbb{R}}^{N} \rightarrow \mathbb{R}$ 是凸的，那么 $\exp \left( f\right)$ 是凸的。

- 任何平方范数 $\parallel \cdot {\parallel }^{2}$ 都是凸的。

- 对于所有 $\mathbf{x} \in {\mathbb{R}}^{N}$ ，函数 $\mathbf{x} \mapsto \log \left( {\mathop{\sum }\limits_{{j = 1}}^{N}{x}_{j}}\right)$ 是凹的。

下面的两个引理给出了另外两种保持凸性的操作的例子。

引理 B.16(凸函数的点态上确界或最大值)${Let}{\left( {f}_{i}\right) }_{i \in \mathfrak{I}}$ ${be}$ $a$ ${fam}$ - ily 的凸函数，定义在凸集 $\mathcal{C}$ 上。那么，它们的点态上确界 $f$ 对于所有 $x \in \mathcal{C}$ 通过 $f\left( x\right) = \mathop{\sup }\limits_{{i \in \mathcal{I}}}{f}_{i}\left( x\right)$ 定义(如果 $\left| \mathcal{I}\right| < + \infty$ ，则是它们的点态最大值)是凸函数。

证明:观察到 $\operatorname{Epi}f = { \cap }_{i \in \mathcal{I}}\operatorname{Epi}{f}_{i}$ ，因此作为一个凸集的交集，它是凸的。

示例 B.17(凸函数的点态上确界)$\mathrm{{The}}$ 引理特别显示了以下函数的凸性:

- 一个分段线性函数 $f$ 对于所有 $x \in {\mathbb{R}}^{N}$ 通过 $f\left( x\right) = \mathop{\max }\limits_{{i \in \lceil m\rceil }}{\mathbf{w}}_{i}^{\top }\mathbf{x} + {b}_{i}$ 定义，作为仿射(因此是凸的)函数的点态最大值是凸的。

- 最大特征值 ${\lambda }_{\max }\left( \mathbf{M}\right)$ 是对称矩阵集合 $\mathbf{M}$ 上的凸函数，因为对称矩阵的集合是凸的，并且因为 ${\lambda }_{\max }\left( \mathbf{M}\right) = \mathop{\sup }\limits_{{\parallel \mathbf{x}{\parallel }_{2} \leq 1}}{\mathbf{x}}^{\top }\mathbf{M}\mathbf{x}$ 被定义为线性(因此是凸的)函数 $\mathbf{M} \mapsto {\mathbf{x}}^{\top }\mathbf{M}\mathbf{x}$ 的上确界。

- 更一般地，令 ${\lambda }_{1}\left( \mathbf{M}\right) ,\ldots ,{\lambda }_{k}\left( \mathbf{M}\right)$ 表示对称 $n \times$ $n$ 矩阵 $\mathbf{M}$ 的顶部 $k \leq n$ 特征值。那么，通过类似的论证，$\mathbf{M} \mapsto \mathop{\sum }\limits_{{i = 1}}^{k}{\lambda }_{i}\left( \mathbf{M}\right)$ 是一个凸函数，因为 $\mathop{\sum }\limits_{{i = 1}}^{k}{\lambda }_{i}\left( \mathbf{M}\right) = \mathop{\sup }\limits_{{\dim \left( \mathbf{V}\right) = k}}\mathop{\sum }\limits_{{i = 1}}^{k}{\mathbf{u}}_{i}^{\top }\mathbf{M}{\mathbf{u}}_{i}$ ，其中 ${\mathbf{u}}_{1},\ldots ,{\mathbf{u}}_{k}$ 是 $\mathbf{V}$ 的正交归一基。

- 利用之前的性质，以及 $\operatorname{Tr}\left( \mathbf{M}\right)$ 在 $\mathbf{M}$ 中是线性的这一事实，也表明 $\mathbf{M} \mapsto \mathop{\sum }\limits_{{i = k + 1}}^{n}{\lambda }_{i}\left( \mathbf{M}\right) = \operatorname{Tr}\left( \mathbf{M}\right) - \mathop{\sum }\limits_{{i = 1}}^{k}{\lambda }_{i}\left( \mathbf{M}\right)$ 或 $\mathbf{M} \mapsto \mathop{\sum }\limits_{{i = n - k + 1}}^{n}{\lambda }_{i}\left( \mathbf{M}\right) = - \mathop{\sum }\limits_{{i = 1}}^{k}{\lambda }_{i}\left( {-\mathbf{M}}\right)$ 是凹函数。

引理 B.18(部分下确界)令 $f$ 为定义在凸集 $\mathcal{C} \subseteq X \times \mathcal{Y}$ 上的凸函数，并且令 $\mathcal{B} \subseteq \mathcal{Y}$ 为一个凸集，使得 $\mathcal{A} = \{ x \in \mathcal{X} : \exists y \in \mathcal{B} \mid \left( {x, y}\right) \in \mathcal{C}\}$ 非空。那么，$\mathcal{A}$ 是一个凸集，并且对于所有 $x \in \mathcal{A}$ 由 $g\left( x\right) = \mathop{\inf }\limits_{{y \in \mathcal{B}}}f\left( {x, y}\right)$ 定义的函数 $g$ 是凸的。

证明:首先注意到凸集 $\mathcal{C}$ 和 $\left( {\mathcal{X} \times \mathcal{B}}\right)$ 的交集是凸的。因此，$\mathcal{A}$ 是凸的，因为它是凸集 $\mathcal{C} \cap \left( {\mathcal{X} \times \mathcal{B}}\right)$ 在 $\mathcal{X}$ 上的投影。

令 ${x}_{1}$ 和 ${x}_{2}$ 属于 $\mathcal{A}$ 。根据 $g$ 的定义，对于任意 $\epsilon > 0$ ，存在 ${y}_{1},{y}_{2} \in \mathcal{B}$ 使得 $\left( {{x}_{1},{y}_{1}}\right) ,\left( {{x}_{2},{y}_{2}}\right) \in \mathcal{C}$ ，使得 $f\left( {{x}_{1},{y}_{1}}\right) \leq g\left( {x}_{1}\right) + \epsilon$ 和 $f\left( {{x}_{2},{y}_{2}}\right) \leq g\left( {x}_{2}\right) + \epsilon$ 成立。那么，对于任意 $\alpha \in \left\lbrack {0,1}\right\rbrack$ ，

$$
g\left( {\alpha {x}_{1} + \left( {1 - \alpha }\right) {x}_{2}}\right) = \mathop{\inf }\limits_{{y \in \mathcal{B}}}f\left( {\alpha {x}_{1} + \left( {1 - \alpha }\right) {x}_{2}, y}\right)
$$

$$
\leq f\left( {\alpha {x}_{1} + \left( {1 - \alpha }\right) {x}_{2},\alpha {y}_{1} + \left( {1 - \alpha }\right) {y}_{2}}\right)
$$

$$
\leq {\alpha f}\left( {{x}_{1},{y}_{1}}\right) + \left( {1 - \alpha }\right) f\left( {{x}_{2},{y}_{2}}\right)
$$

$$
\leq {\alpha g}\left( {x}_{1}\right) + \left( {1 - \alpha }\right) g\left( {x}_{2}\right) + \epsilon
$$

由于不等式对所有 $\epsilon > 0$ 都成立，它暗示了

$$
g\left( {\alpha {x}_{1} + \left( {1 - \alpha }\right) {x}_{2}}\right) \leq {\alpha g}\left( {x}_{1}\right) + \left( {1 - \alpha }\right) g\left( {x}_{2}\right)
$$

这完成了证明。

示例 B.19 引理特别表明，在任意范数向量空间中，到凸集 $\mathcal{B}, d\left( {x,\mathcal{B}}\right) =$ $\mathop{\inf }\limits_{{y \in \mathcal{B}}}\parallel x - y\parallel$ 的距离是 $x$ 的凸函数，因为对于任意范数 $\parallel \cdot \parallel$ ，$\left( {x, y}\right) \mapsto \parallel x - y\parallel$ 在 $x$ 和 $y$ 上是联合凸的。

以下是在各种情境中应用的一个有用的不等式。它实际上是凸性定义的直接推论。

定理B.20(Jensen不等式)${Let}X$ 是一个随机变量，其在非空凸集 $\mathcal{C} \subseteq {\mathbb{R}}^{N}$ 中取值，并且具有有限的期望 $\mathbb{E}\left\lbrack X\right\rbrack$，以及 $f$ 是定义在 $\mathcal{C}$ 上的可测凸函数。那么，$\mathbb{E}\left\lbrack X\right\rbrack$ 在 $\mathcal{C},\mathbb{E}\left\lbrack {f\left( X\right) }\right\rbrack$ 中是有限的，并且以下不等式成立:

$$
f\left( {\mathbb{E}\left\lbrack X\right\rbrack }\right) \leq \mathbb{E}\left\lbrack {f\left( X\right) }\right\rbrack
$$

证明:我们给出证明的概要，该证明基本上遵循凸性的定义。注意，对于 $\mathcal{C}$ 中任意有限个元素 ${x}_{1},\ldots ,{x}_{n}$ 和任意正实数 ${\alpha }_{1},\ldots ,{\alpha }_{n}$ 使得 $\mathop{\sum }\limits_{{i = 1}}^{n}{\alpha }_{i} = 1$ ，我们有

$$
f\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{\alpha }_{i}{x}_{i}}\right) \leq \mathop{\sum }\limits_{{i = 1}}^{n}{\alpha }_{i}f\left( {x}_{i}\right)
$$

这直接从凸性的定义通过归纳法得出。由于 ${\alpha }_{i}\mathrm{\;s}$ 可以解释为概率，这立即证明了对于由 $\mathbf{\alpha } = \left( {{\alpha }_{1},\ldots ,{\alpha }_{n}}\right)$ 定义的有限支撑的任意分布的不等式:

$$
f\left( {\underset{\mathbf{\alpha }}{\mathbb{E}}\left\lbrack X\right\rbrack }\right) \leq \underset{\mathbf{\alpha }}{\mathbb{E}}\left\lbrack {f\left( X\right) }\right\rbrack
$$

将此扩展到任意分布可以通过 $f$ 在任意开集上的连续性来证明，这种连续性由 $f$ 的凸性保证，并且具有有限支撑的分布在所有概率测度族中是弱密集的。