以下不等式在多种不同的背景下都很有用，包括在证明线性假设的经验 Rademacher 复杂度下界时（第六章）。

定理 D.9(Khintchine-Kahane 不等式)
设 $\left( {\mathbb{H},\parallel \cdot \parallel }\right)$ 是一个范数向量空间，且 ${\mathbf{x}}_{1},\ldots ,{\mathbf{x}}_{m}$ 是 $\mathbb{H}$ 的 $m \geq 1$ 元素。设 $\mathbf{\sigma } = {\left( {\sigma }_{1},\ldots ,{\sigma }_{m}\right) }^{\top }$ ，其中 ${\sigma }_{i}$ 是在 $\{ - 1, + 1\}$ (Rademacher 变量)中取值的独立均匀随机变量。那么，以下不等式成立:
$$
\frac{1}{2}\underset{\sigma }{\mathbb{E}}\left\lbrack {\begin{Vmatrix}\mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{i}{\mathbf{x}}_{i}\end{Vmatrix}}^{2}\right\rbrack \leq {\left( \underset{\sigma }{\mathbb{E}}\left\lbrack \begin{Vmatrix}\mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{i}{\mathbf{x}}_{i}\end{Vmatrix}\right\rbrack \right) }^{2} \leq \underset{\sigma }{\mathbb{E}}\left\lbrack {\begin{Vmatrix}\mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{i}{\mathbf{x}}_{i}\end{Vmatrix}}^{2}\right\rbrack . \tag{D.20}
$$

证明:第二个不等式是 $x \mapsto {x}^{2}$ 的凸性和Jensen不等式(定理 B.20)的直接结果。

为了证明左侧不等式，首先注意到对于任何 ${\beta }_{1},\ldots ,{\beta }_{m} \in \mathbb{R}$ ，展开乘积 $\mathop{\prod }\limits_{{i = 1}}^{m}\left( {1 + {\beta }_{i}}\right)$ 正好得到所有单项式 ${\beta }_{1}^{{\delta }_{1}}\ldots {\beta }_{m}^{{\delta }_{m}}$ 的和，指数 ${\delta }_{1},\ldots ,{\delta }_{m}$ 在 $\{ 0,1\}$ 中。我们将使用 ${\beta }_{1}^{{\delta }_{1}}\cdots {\beta }_{m}^{{\delta }_{m}} = {\beta }^{\delta }$ 和 $\left| \delta \right| = \mathop{\sum }\limits_{{i = 1}}^{m}{\delta }_{m}$ 来表示任何 $\mathbf{\delta } = \left( {{\delta }_{1},\ldots ,{\delta }_{m}}\right) \in \{ 0,1{\} }^{m}$ 。基于此，对于任何 $\left( {{\alpha }_{1},\ldots ,{\alpha }_{m}}\right) \in {\mathbb{R}}^{m}$ 和 $t > 0$ ，以下等式成立:

$$
{t}^{2}\mathop{\prod }\limits_{{i = 1}}^{m}\left( {1 + {\alpha }_{i}/t}\right) = {t}^{2}\mathop{\sum }\limits_{{\delta \in \{ 0,1{\} }^{m}}}{\alpha }^{\delta }/{t}^{\left| \delta \right| } = \mathop{\sum }\limits_{{\delta \in \{ 0,1{\} }^{m}}}{t}^{2 - \left| \delta \right| }{\alpha }^{\delta }.
$$

对两边关于 $t$ 求导，并令 $t = 1$ ，得到

$$
2\mathop{\prod }\limits_{{i = 1}}^{m}\left( {1 + {\alpha }_{i}}\right) - \mathop{\sum }\limits_{{j = 1}}^{m}{\alpha }_{j}\mathop{\prod }\limits_{{i \neq j}}\left( {1 + {\alpha }_{i}}\right) = \mathop{\sum }\limits_{{\delta \in \{ 0,1{\} }^{m}}}\left( {2 - \left| \delta \right| }\right) {\alpha }^{\delta }. \tag{D.21}
$$

对于任何 $\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}$ ，设 ${S}_{\mathbf{\sigma }}$ 由 ${S}_{\mathbf{\sigma }} = \begin{Vmatrix}{s}_{\mathbf{\sigma }}\end{Vmatrix}$ 定义，其中 ${s}_{\mathbf{\sigma }} = \mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{i}{\mathbf{x}}_{i}$ 。然后，令 ${\alpha }_{i} = {\sigma }_{i}{\sigma }_{i}^{\prime }$ ，将 (D.21) 的两边乘以 ${S}_{\mathbf{\sigma }}{S}_{{\mathbf{\sigma }}^{\prime }}$ ，并对所有 $\mathbf{\sigma },{\mathbf{\sigma }}^{\prime } \in$ $\{ - 1, + 1{\} }^{m}$ 求和，得到

$$
\mathop{\sum }\limits_{{\mathbf{\sigma },{\mathbf{\sigma }}^{\prime } \in \{ - 1, + 1{\} }^{m}}}\left( {2\mathop{\prod }\limits_{{i = 1}}^{m}\left( {1 + {\sigma }_{i}{\sigma }_{i}^{\prime }}\right) - \mathop{\sum }\limits_{{j = 1}}^{m}{\sigma }_{j}{\sigma }_{j}^{\prime }\mathop{\prod }\limits_{{i \neq j}}\left( {1 + {\sigma }_{i}{\sigma }_{i}^{\prime }}\right) }\right) {S}_{\mathbf{\sigma }}{S}_{{\mathbf{\sigma }}^{\prime }}
$$

$$
= \mathop{\sum }\limits_{{\mathbf{\sigma },{\mathbf{\sigma }}^{\prime } \in \{ - 1, + 1{\} }^{m}}}\mathop{\sum }\limits_{{\mathbf{\delta } \in \{ 0,1{\} }^{m}}}\left( {2 - \left| \mathbf{\delta }\right| }\right) {\sigma }^{\mathbf{\delta }}{\sigma }^{\prime \mathbf{\delta }}{S}_{\mathbf{\sigma }}{S}_{{\mathbf{\sigma }}^{\prime }}
$$

$$
= \mathop{\sum }\limits_{{\mathbf{\delta } \in \{ 0,1{\} }^{m}}}\left( {2 - \left| \mathbf{\delta }\right| }\right) \mathop{\sum }\limits_{{\mathbf{\sigma },{\mathbf{\sigma }}^{\prime } \in \{ - 1, + 1{\} }^{m}}}{\sigma }^{\mathbf{\delta }}{\sigma }^{\prime \mathbf{\delta }}{S}_{\mathbf{\sigma }}{S}_{{\mathbf{\sigma }}^{\prime }} \tag{D.22}
$$

$$
= \mathop{\sum }\limits_{{\mathbf{\delta } \in \{ 0,1{\} }^{m}}}\left( {2 - \left| \mathbf{\delta }\right| }\right) {\left\lbrack \mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}{\sigma }^{\mathbf{\delta }}{S}_{\mathbf{\sigma }}\right\rbrack }^{2}.
$$

注意，右侧和中的 $\left| \delta \right| \geq 2$ 项是非正的。带有 $\left| \delta \right| = 1$ 的项为零:因为 ${S}_{\mathbf{\sigma }} = {S}_{-\mathbf{\sigma }}$ ，在这种情况下我们有 $\mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}{\sigma }^{\bar{\delta }}{S}_{\mathbf{\sigma }} = 0$ 。因此，右侧可以被 $\mathbf{\delta } = 0$ 项所界定，即 $2{\left( \mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}{S}_{\mathbf{\sigma }}\right) }^{2}$ 。(D.22) 的左侧可以重写如下:

$$
\mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}\left( {{2}^{m + 1} - m{2}^{m - 1}}\right) {S}_{\mathbf{\sigma }}^{2} + {2}^{m - 1}\mathop{\sum }\limits_{\substack{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}} \\ {{\mathbf{\sigma }}^{\prime } \in B\left( {\mathbf{\sigma },1}\right) } }}{S}_{\mathbf{\sigma }}{S}_{{\mathbf{\sigma }}^{\prime }}
$$

$$
= {2}^{m}\mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}{S}_{\mathbf{\sigma }}^{2} + {2}^{m - 1}\mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}{S}_{\mathbf{\sigma }}\left( {\mathop{\sum }\limits_{{{\mathbf{\sigma }}^{\prime } \in B\left( {\mathbf{\sigma },1}\right) }}{S}_{{\mathbf{\sigma }}^{\prime }} - \left( {m - 2}\right) {S}_{\mathbf{\sigma }}}\right) , \tag{D.23}
$$

其中 $B\left( {\mathbf{\sigma },1}\right)$ 表示与 $\mathbf{\sigma }$ 在恰好一个坐标 $j \in \left\lbrack m\right\rbrack$ 上不同的 ${\mathbf{\sigma }}^{\prime }$ 的集合，即与 $\mathbf{\sigma }$ 的汉明距离为1的 ${\mathbf{\sigma }}^{\prime }$ 的集合。注意，对于任何这样的 ${\mathbf{\sigma }}^{\prime },{s}_{\mathbf{\sigma }} - {s}_{{\mathbf{\sigma }}^{\prime }} = 2{\sigma }_{j}{\mathbf{x}}_{j}$ ，对于其中一个坐标 $j \in \left\lbrack m\right\rbrack$ ，因此 $\mathop{\sum }\limits_{{{\mathbf{\sigma }}^{\prime } \in B\left( {\mathbf{\sigma },1}\right) }}{s}_{\mathbf{\sigma }} - {s}_{{\mathbf{\sigma }}^{\prime }} = 2{s}_{\mathbf{\sigma }}$ 。鉴于这一点，并使用三角不等式，我们可以写出

$$
\left( {m - 2}\right) {S}_{\mathbf{\sigma }} = \begin{Vmatrix}{m{s}_{\mathbf{\sigma }}}\end{Vmatrix} - \begin{Vmatrix}{2{s}_{\mathbf{\sigma }}}\end{Vmatrix} = \begin{Vmatrix}{\mathop{\sum }\limits_{{{\mathbf{\sigma }}^{\prime } \in B\left( {\mathbf{\sigma },1}\right) }}{s}_{\mathbf{\sigma }}}\end{Vmatrix} - \begin{Vmatrix}{\mathop{\sum }\limits_{{{\mathbf{\sigma }}^{\prime } \in B\left( {\mathbf{\sigma },1}\right) }}{s}_{\mathbf{\sigma }} - {s}_{{\mathbf{\sigma }}^{\prime }}}\end{Vmatrix}
$$

$$
\leq \begin{Vmatrix}{\mathop{\sum }\limits_{{{\mathbf{\sigma }}^{\prime } \in B\left( {\mathbf{\sigma },1}\right) }}{s}_{{\mathbf{\sigma }}^{\prime }}}\end{Vmatrix} \leq \mathop{\sum }\limits_{{{\mathbf{\sigma }}^{\prime } \in B\left( {\mathbf{\sigma },1}\right) }}{S}_{{\mathbf{\sigma }}^{\prime }}.
$$

因此，(D.23)的第二项是非负的，且(D.22)的左侧可以由第一项 ${2}^{m}\mathop{\sum }\limits_{{\sigma \in \{ - 1, + 1{\} }^{m}}}{S}_{\sigma }^{2}$ 从下面界定。将此与为(D.22)找到的上界相结合，得到

$$
{2}^{m}\mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}{S}_{\mathbf{\sigma }}^{2} \leq 2{\left\lbrack \mathop{\sum }\limits_{{\mathbf{\sigma } \in \{ - 1, + 1{\} }^{m}}}{S}_{\mathbf{\sigma }}\right\rbrack }^{2}.
$$

双方除以 ${2}^{2m}$ 并使用 $\mathbb{P}\left\lbrack \mathbf{\sigma }\right\rbrack = 1/{2}^{m}$ 得到 ${\mathbb{E}}_{\mathbf{\sigma }}\left\lbrack {S}_{\mathbf{\sigma }}^{2}\right\rbrack \leq 2{\left( {\mathbb{E}}_{\mathbf{\sigma }}\left\lbrack {S}_{\mathbf{\sigma }}\right\rbrack \right) }^{2}$ ，从而完成了证明。

在(D.20)的第一个不等式中出现的常数 $1/2$ 是最优的。为了看到这一点，考虑 $m = 2$ 和 ${\mathbf{x}}_{1} = {\mathbf{x}}_{2} = \mathbf{x}$ 对于某个非零向量 $\mathbf{x} \in \mathbb{H}$ 的情况。那么，第一个不等式左侧是 $\frac{\bar{1}}{2}\mathop{\sum }\limits_{{i = 1}}^{{m}^{ - }}\parallel {\mathbf{x}}_{i}{\parallel }^{2} = \parallel \mathbf{x}{\parallel }^{2}$ ，右侧是 ${\left( {\mathbb{E}}_{\mathbf{\sigma }}\left\lbrack \parallel \left( {\sigma }_{1} + {\sigma }_{2}\right) \mathbf{x}\parallel \right\rbrack \right) }^{2} =$ $\parallel \mathbf{x}{\parallel }^{2}{\left( {\mathbb{E}}_{\mathbf{\sigma }}\left\lbrack \left| {\sigma }_{1} + {\sigma }_{2}\right| \right\rbrack \right) }^{2} = \parallel \overline{\mathbf{x}}{\parallel }^{2}.$

注意，当范数 $\parallel \cdot \parallel$ 对应于内积，如在希尔伯特空间 $\mathbb{H}$ 的情况下，我们可以写出

$$
\underset{\sigma }{\mathbb{E}}\left\lbrack {\begin{Vmatrix}\mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{i}{\mathbf{x}}_{i}\end{Vmatrix}}^{2}\right\rbrack = \mathop{\sum }\limits_{{i, j = 1}}^{m}\underset{\sigma }{\mathbb{E}}\left\lbrack {{\sigma }_{i}{\sigma }_{j}\left( {{\mathbf{x}}_{i} \cdot {\mathbf{x}}_{j}}\right) }\right\rbrack = \mathop{\sum }\limits_{{i, j = 1}}^{m}\underset{\sigma }{\mathbb{E}}\left\lbrack {{\sigma }_{i}{\sigma }_{j}}\right\rbrack \left( {{\mathbf{x}}_{i} \cdot {\mathbf{x}}_{j}}\right) = \mathop{\sum }\limits_{{i = 1}}^{m}{\begin{Vmatrix}{\mathbf{x}}_{i}\end{Vmatrix}}^{2},
$$

因为由随机变量 ${\sigma }_{i}$ 的独立性，对于 $i \neq j,{\mathbb{E}}_{\mathbf{\sigma }}\left\lbrack {{\sigma }_{i}{\sigma }_{j}}\right\rbrack = {\mathbb{E}}_{\mathbf{\sigma }}\left\lbrack {\sigma }_{i}\right\rbrack {\mathbb{E}}_{\mathbf{\sigma }}\left\lbrack {\sigma }_{j}\right\rbrack = 0$ 。因此，(D.20)可以重写如下:

$$
\frac{1}{2}\mathop{\sum }\limits_{{i = 1}}^{m}{\begin{Vmatrix}{\mathbf{x}}_{i}\end{Vmatrix}}^{2} \leq {\left( \mathbb{E}\left\lbrack \begin{Vmatrix}\mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{i}{\mathbf{x}}_{i}\end{Vmatrix}\right\rbrack \right) }^{2} \leq \mathop{\sum }\limits_{{i = 1}}^{m}{\begin{Vmatrix}{\mathbf{x}}_{i}\end{Vmatrix}}^{2} \tag{D.24}
$$