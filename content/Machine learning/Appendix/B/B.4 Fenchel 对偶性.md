## B.4 Fenchel 对偶性

在本节中，我们提出了一个关于凸优化或凸分析的替代理论，其中考虑的函数 $f$ 可能是不可微的并取无穷大值。

在本节中，集合 $x$ 表示一个内积为 $\langle \cdot , \cdot \rangle$ 的希尔伯特空间。然而，所呈现的结果可以直接推广到巴拿赫空间的情况。我们考虑取值在 $\left\lbrack {-\infty , + \infty }\right\rbrack$ 中的函数。函数 $f : x \rightarrow$ $\left\lbrack {-\infty , + \infty }\right\rbrack$ 的定义域定义为集合

$$
\operatorname{dom}\left( f\right) = \{ x \in X : f\left( x\right) < + \infty \} . \tag{B. 15}
$$

我们扩展了凸性的定义，并说 $f : x \rightarrow \left\lbrack {-\infty , + \infty }\right\rbrack$ 是凸的，如果它在 $\operatorname{dom}\left( f\right)$ 上是凸的，即对于所有 $x,{x}^{\prime } \in \operatorname{dom}\left( f\right)$ 和所有 $t \in \left\lbrack {0,1}\right\rbrack$ ，

$$
f\left( {{tx} + \left( {1 - t}\right) {x}^{\prime }}\right) \leq {tu} + \left( {1 - t}\right) v \tag{B.16}
$$

对于所有 $\left( {u, v}\right) \in {\mathbb{R}}^{2}$ ，其中 $u \geq f\left( x\right)$ 和 $v \geq f\left( {x}^{\prime }\right)$ 。如果一个凸函数取值在 $( - \infty , + \infty \rbrack$ 中，并且不均匀等于 $+ \infty$ ，则称其为正则的。当其上确界闭合时，称其为闭函数。

### B.4.1 次梯度

定义 B. 31 设 $f : X \rightarrow ( - \infty , + \infty \rbrack$ 为一个凸函数。那么，向量 $g \in X$ 是 $f$ 在点 $x \in \operatorname{dom}\left( f\right)$ 处的次梯度，如果对于所有 $z \in X$ ，以下不等式成立:

$$
f\left( z\right) \geq f\left( x\right) + \langle z - x, g\rangle . \tag{B.17}
$$

所有在 $x$ 处的次梯度集合称为 $f$ 在 $x$ 处的次微分，并表示为 $\partial f\left( x\right)$ ，其中 $\partial f\left( x\right) = \varnothing$ 对于 $x \notin \operatorname{dom}\left( f\right)$ 。

因此，$g$ 是 $x$ 处的次梯度，当且仅当通过点 $\left( {x, f\left( x\right) }\right)$ 的法向量为 $g$ 的超平面位于 $f$ 的图形下方，即当它支撑 $f$ 的图形时。图 14.1 描述了这些定义。

以下引理表明，如果 $f$ 在 $x \in \operatorname{dom}\left( f\right)$ 处可微，那么它的子微分在 $x$ 处简化为其梯度。

引理 B.32 如果 $f$ 在 $x \in \operatorname{dom}\left( f\right)$ 处可微，那么 $\partial f\left( x\right) = \{ \nabla f\left( x\right) \}$ 。

证明:显然，梯度 $\nabla f\left( x\right)$ 在 $x$ 处总是一个子梯度。现在，设 $g$ 在 $\partial f\left( x\right)$ 中。那么，根据子梯度的定义，对于任何 $\epsilon \in \mathbb{R}$ ，

$$
f\left( {x + \epsilon \left( {\nabla f\left( x\right) - g}\right) }\right) \geq f\left( x\right) + \epsilon \langle \nabla f\left( x\right) - g, g\rangle .
$$

一阶泰勒级数展开给出

$$
f\left( {x + \epsilon \left( {\nabla f\left( x\right) - g}\right) }\right) - f\left( x\right) = \epsilon \langle \nabla f\left( x\right) ,\nabla f\left( x\right) - g\rangle + o\left( {\epsilon \parallel \nabla f\left( x\right) - g\parallel }\right) .
$$

考虑到这一点，第一个不等式可以重写为

$$
\epsilon \parallel \nabla f\left( x\right) - g{\parallel }^{2} \leq o\left( {\epsilon \parallel \nabla f\left( x\right) - g\parallel }\right) ,
$$

这意味着 $\parallel \nabla f\left( x\right) - g\parallel = o\left( 1\right)$ 和 $\nabla f\left( x\right) = g$ 。

命题 B.33 设 $f : X \rightarrow ( - \infty , + \infty \rbrack$ 是一个适当的函数。那么，${x}^{ * }$ 是 $f$ 的全局最小化子当且仅当 $\partial f\left( {x}^{ * }\right)$ 包含 0。

证明:由于 $f$ 是适当的，如果 ${x}^{ * }$ 是最小化子，那么 $f\left( {x}^{ * }\right)$ 不能是 $+ \infty$ 。因此 ${x}^{ * }$ 必须在 $\operatorname{dom}\left( f\right)$ 中(因此 $\partial f\left( x\right)$ 不定义为空)。现在，${x}^{ * }$ 是全局最小化子当且仅当对于所有 $z \in X$ ，$f\left( z\right) \geq f\left( {x}^{ * }\right)$ ，即当且仅当 0 是 $f$ 在 ${x}^{ * }$ 处的子梯度。

### B.4.2 核心

集合 $\mathcal{C} \subseteq \mathcal{X}$ 的核心用 core( $\mathcal{C}$ ) 表示，并定义如下:

$$
\operatorname{core}\left( \mathcal{C}\right) = \{ x \in \mathcal{C} : \forall u \in X,\exists \epsilon > 0 \mid \forall t \in \left\lbrack {0,\epsilon }\right\rbrack ,\left( {x + {tu}}\right) \in \mathcal{C}\} . \tag{B.18}
$$

因此，对于 $x \in \operatorname{core}\left( \mathcal{C}\right)$ ，对于任何方向 $u,\left( {x + {tu}}\right)$ 在 $\mathcal{C}$ 中，$t$ 足够小。基于这个定义，核心 $\left( \mathcal{C}\right)$ 显然包含 $\mathcal{C}$ 的内部，即 int $\left( \mathcal{C}\right)$。

命题B.34 设 $h : X \rightarrow \left\lbrack {-\infty , + \infty }\right\rbrack$ 是一个凸函数。如果存在 ${x}_{0} \in \operatorname{core}\left( {\operatorname{dom}\left( h\right) }\right)$ 使得 $h\left( {x}_{0}\right) > - \infty$ ，那么 $h\left( x\right) > - \infty$ 对于所有 $x \in X$ 。

证明:设 $x$ 在 $x$ 中。由于 ${x}_{0}$ 在核心 $\left( {\operatorname{dom}\left( h\right) }\right)$ 中，存在 $t > 0$ 使得 ${x}_{0}^{\prime } = {x}_{0} + t\left( {{x}_{0} - x}\right)$ 在 $\operatorname{dom}\left( h\right)$ 中，即满足 $h\left( {x}_{0}^{\prime }\right) < + \infty$ 。由于 ${x}_{0} = \frac{1}{1 + t}{x}_{0}^{\prime } + \frac{t}{1 + t}x$ ，根据凸性，以下成立

对于所有 。

$$
h\left( {x}_{0}\right) \leq \frac{1}{1 + t}h\left( {x}_{0}^{\prime }\right) + \frac{t}{1 + t}v \Leftrightarrow v \geq \frac{1 + t}{t}\left\lbrack {h\left( {x}_{0}\right) - \frac{1}{1 + t}h\left( {x}_{0}^{\prime }\right) }\right\rbrack \tag{B.19}
$$

这意味着 $h\left( x\right) \geq \frac{1 + t}{t}\left\lbrack {h\left( {x}_{0}\right) - \frac{1}{1 + t}h\left( {x}_{0}^{\prime }\right) }\right\rbrack > - \infty$ ，这完成了证明。 $\square$

下一个结果的证明留给作为练习(练习B.3)。

命题B.35 设 $h : X \rightarrow ( - \infty , + \infty \rbrack$ 是一个凸函数。那么， $h$ 在任何 $x \in \operatorname{core}\left( {\operatorname{dom}\left( h\right) }\right)$ 处都存在次微分。

### B.4.3 伴随函数

定义B.36(伴随函数)设 $X$ 是一个 ${Hilbert}{space}.\;{The}\;\mathrm{{conjugate}\;{function}}\;{or}$ ，函数 $f : X \mapsto \left\lbrack {-\infty , + \infty }\right\rbrack$ 的Fenchel伴随是一个定义为 ${f}^{ * } : X \mapsto \left\lbrack {-\infty , + \infty }\right\rbrack$ 的函数

$$
{f}^{ * }\left( u\right) = \mathop{\sup }\limits_{{x \in \mathcal{X}}}\{ \langle u, x\rangle - f\left( x\right) \} . \tag{B.20}
$$

注意到 ${f}^{ * }$ 是凸函数 $u \mapsto \langle x, u\rangle - f\left( x\right)$ 的点态上确界，因此是凸的。另外，如果存在 $x$ 使得 $f\left( x\right) < + \infty$ ，那么 $f > - \infty$ 。伴随关系是逆序的:对于任何 $f$ 和 $g$ ，如果 $f \leq g$ ，那么 ${g}^{ * } \leq {f}^{ * }$ 。同样，如果 $f$ 是闭的适当凸集，那么 ${f}^{* * } = f$ 。

图B.3说明了伴随函数的定义。如图所示，伴随函数对应于函数的图在支撑超平面及其交点方面的对偶描述。

![01928a40-c638-783b-803a-1bf2444d1c2b_9_513_254_788_584_0.jpg](images/01928a40-c638-783b-803a-1bf2444d1c2b_9_513_254_788_584_0.jpg)

图B.3

Illustration of the conjugate ${f}^{ * }$ of a function $f$ . Given $y,{x}^{ * }$ is the point at which the distance between the hyperplane of equation $z = \langle x, y\rangle$ with normal $y$ (slope $y$ in dimension one) and the plot of $f\left( x\right)$ is the largest. This largest distance is equal to ${f}^{ * }\left( y\right)$ . The parallel hyperplane $z = \left\langle {x - {x}^{ * }, y}\right\rangle + f\left( {x}^{ * }\right)$ with normal $y$ and passing through the point $\left( {{x}^{ * }, f\left( {x}^{ * }\right) }\right.$ is shown. This is a supporting hyperplane of the plot of $f\left( x\right)$ . The point at which it intercepts the $y$ -axis (crossing point) has $y$ -coordinate $- {f}^{ * }\left( y\right)$ .

Lemma B.37 (Conjugate of extended relative entropy) ${Let}\;{p}_{0}\; \in \;\Delta \;{be}\;a\;{distribution}\;{over}\;X$ such that ${p}_{0}\left( x\right) > 0$ for all $x \in X$ . Define $f : {\mathbb{R}}^{x} \rightarrow \mathbb{R}$ by

$$
f\left( p\right) = \left\{ \begin{array}{ll} \mathrm{D}\left( {p\parallel {p}_{0}}\right) & \text{ if }p \in \Delta \\ + \infty & \text{ otherwise. } \end{array}\right.
$$

Then, the conjugate function ${f}^{ * } : {\mathbb{R}}^{x} \rightarrow \mathbb{R}$ of $f$ is defined by

$$
\forall q \in {\mathbb{R}}^{X},{f}^{ * }\left( q\right) = \log \left( {\mathop{\sum }\limits_{{x \in X}}{p}_{0}\left( x\right) {e}^{q\left( x\right) }}\right) .
$$

Proof: By definition of $f$ , for any $q \in {\mathbb{R}}^{x}$ , we can write

$$
\mathop{\sup }\limits_{{p \in {\mathbb{R}}^{X}}}\left( {\langle p, q\rangle - \mathrm{D}\left( {p\parallel {p}_{0}}\right) }\right) = \mathop{\sup }\limits_{{p \in \Delta }}\left( {\langle p, q\rangle - \mathrm{D}\left( {p\parallel {p}_{0}}\right) }\right) . \tag{B.21}
$$

Fix $q \in {\mathbb{R}}^{\mathcal{X}}$ and let $\bar{q} \in \Delta$ be defined for all $x \in \mathcal{X}$ by

$$
\bar{q}\left( x\right) = \frac{{p}_{0}\left( x\right) {e}^{q\left( x\right) }}{\mathop{\sum }\limits_{{x \in X}}{p}_{0}\left( x\right) {e}^{q\left( x\right) }} = \frac{{p}_{0}\left( x\right) {e}^{q\left( x\right) }}{{\mathbb{E}}_{{p}_{0}}\left\lbrack {e}^{q}\right\rbrack }. \tag{B.22}
$$

Then, the following holds for all $p \in \Delta$ :

$$
\langle p, q\rangle - \mathrm{D}\left( {p\parallel {p}_{0}}\right) = \underset{p}{\mathbb{E}}\left\lbrack {\log \left( {e}^{q}\right) }\right\rbrack - \underset{p}{\mathbb{E}}\left\lbrack {\log \frac{p}{{p}_{0}}}\right\rbrack = \underset{p}{\mathbb{E}}\left\lbrack {\log \frac{{p}_{0}{e}^{q}}{p}}\right\rbrack = - \mathrm{D}\left( {p\parallel \bar{q}}\right) + \log \underset{{p}_{0}}{\mathbb{E}}\left\lbrack {e}^{q}\right\rbrack .
$$

Since $\mathrm{D}\left( {p\parallel \bar{q}}\right) \geq 0$ and $\mathrm{D}\left( {p\parallel \bar{q}}\right) = 0$ for $p = \bar{q}$ , this shows that $\mathop{\sup }\limits_{{p \in \Delta }}\left( {p \cdot q - \mathrm{D}\left( {p\parallel {p}_{0}}\right) }\right) = \log \left( {{\mathbb{E}}_{{p}_{0}}\left\lbrack {e}^{q}\right\rbrack }\right)$ and concludes the proof.

Table B. 1 gives a series of other examples of functions and their conjugates. The following is an immediate consequence of the definition of the conjugate functions.

Table B. 1

Examples of functions $g$ and their conjugates ${g}^{ * }$ .

<table><thead><tr><th>$g\left( x\right)$</th><th>$\operatorname{dom}\left( g\right)$</th><th>${g}^{ * }\left( y\right)$</th><th>$\operatorname{dom}\left( {g}^{ * }\right)$</th></tr></thead><tr><td>$f\left( {ax}\right) \left( {a \neq 0}\right)$</td><td>$x$</td><td>${f}^{ * }\left( \frac{y}{a}\right)$</td><td>${x}^{ * }$</td></tr><tr><td>$f\left( {x + b}\right)$</td><td>$x$</td><td>${f}^{ * }\left( y\right) - \langle b, y\rangle$</td><td>${x}^{ * }$</td></tr><tr><td>${af}\left( x\right) \left( {a > 0}\right)$</td><td>$x$</td><td>$a{f}^{ * }\left( \frac{y}{a}\right)$</td><td>${x}^{ * }$</td></tr><tr><td>${\alpha x} + \beta$</td><td>$\mathbb{R}$</td><td>$\left\{ \begin{array}{ll} - \beta & \text{if }y = \alpha \\ + \infty & \text{otherwise} \end{array}\right.$</td><td>$\mathbb{R}$</td></tr><tr><td>$\frac{{\left| x\right| }^{p}}{p}\left( {p > 1}\right)$</td><td>$\mathbb{R}$</td><td>$\frac{{\left| y\right| }^{q}}{q}\left( {\frac{1}{p} + \frac{1}{q} = 1}\right)$</td><td>$\mathbb{R}$</td></tr><tr><td>$\frac{-{x}^{p}}{p}\left( {0 < p < 1}\right)$</td><td>${\mathbb{R}}_{ + }$</td><td>$\frac{-{\left( -y\right) }^{q}}{q}\left( {\frac{1}{p} + \frac{1}{q} = 1}\right)$</td><td>$\mathbb{R}$ _</td></tr><tr><td>$\sqrt{1 + {x}^{2}}$</td><td>$\mathbb{R}$</td><td>$- \sqrt{1 - {\left( y\right) }^{2}}$</td><td>$\left\lbrack {-1,1}\right\rbrack$</td></tr><tr><td>$- \log \left( x\right)$</td><td>${\mathbb{R}}_{ + } \smallsetminus \{ 0\}$</td><td>$- \left( {1 + \log \left( {-y}\right) }\right)$</td><td>${\mathbb{R}}_{ - } \smallsetminus \{ 0\}$</td></tr><tr><td>${e}^{x}$</td><td>$\mathbb{R}$</td><td>$\left\{ \begin{array}{ll} y\log \left( y\right) - y, & \text{if }y > 0 \\ 0, & \text{if }y = 0 \end{array}\right.$</td><td>${\mathbb{R}}_{ + }$</td></tr><tr><td>$\log \left( {1 + {e}^{x}}\right)$</td><td>$\mathbb{R}$</td><td>$y\log \left( y\right) + \left( {1 - y}\right) \log \left( {1 - y}\right) ,\;$ if $\;0 < y < 1$ 0 , if $y = 0,1$</td><td>$\left\lbrack {0,1}\right\rbrack$</td></tr><tr><td>$- \log \left( {1 - {e}^{x}}\right)$</td><td>$\mathbb{R}$</td><td>$y\log \left( y\right) - \left( {1 + y}\right) \log \left( {1 + y}\right) ,\;$ if $\;y > 0$ if $y = 0$</td><td>${\mathbb{R}}_{ + }$</td></tr></table>

Proposition B.38 (Fenchel’s inequality) Let $X$ be a ${Hilbert}{space}.{For}{any}{function}f : X \mapsto$ $\left\lbrack {-\infty , + \infty }\right\rbrack$ and any $x \in \operatorname{dom}\left( f\right)$ and $u \in x$ , the following inequality holds:

$$
f\left( x\right) + {f}^{ * }\left( u\right) \geq \langle u, x\rangle \tag{B.23}
$$

等式成立当且仅当 $u$ 是 $f$ 在 $x$ 处的子梯度。

我们将用 ${A}^{ * }$ 表示一个有界(或连续)线性映射 $A : x \rightarrow y$ 的伴随算子。此外，我们用 $\operatorname{cont}\left( f\right)$ 表示那些 $x \in X$ 点的集合，在这些点上 $f : X \rightarrow \left\lbrack {-\infty , + \infty }\right\rbrack$ 是有限且连续的。

定理 B.39(Fenchel 对偶定理)${Let}\;X\;{and}\;y\;{be}\;{two}\;{Hilbert}\;{spaces}$、$f:X \rightarrow ( - \infty , + \infty \rbrack$ 和 $g : y \rightarrow ( - \infty , + \infty \rbrack$ 是两个凸函数，$A : x \rightarrow y$ 是一个有界线性映射。那么，以下两个优化问题(Fenchel 问题)

$$
{p}^{ * } = \mathop{\inf }\limits_{{x \in \mathcal{X}}}\{ f\left( x\right) + g\left( {Ax}\right) \}
$$

$$
{d}^{ * } = \mathop{\sup }\limits_{{y \in \mathcal{Y}}}\left\{ {-{f}^{ * }\left( {{A}^{ * }y}\right) - {g}^{ * }\left( {-y}\right) }\right\}
$$

满足弱对偶性 ${p}^{ * } \geq {d}^{ * }$。如果进一步 $f$ 和 $g$ 满足条件

$$
0 \in \operatorname{core}\left( {\operatorname{dom}\left( g\right) - A\left( {\operatorname{dom}\left( f\right) }\right) }\right)
$$

或者更强的条件

$$
A\left( {\operatorname{dom}\left( f\right) }\right) \cap \operatorname{cont}\left( g\right) \neq \varnothing ,
$$

那么强对偶性成立，即 ${p}^{ * } = {d}^{ * }$ 并且对偶问题中的上确界在 ${d}^{ * } \in \mathbb{R}$ 时达到。

证明:通过将 Fenchel 不等式(命题 B.38)应用于 $f$ 和 $g$，对于任意的 $x \in x$ 和 $y \in \mathcal{Y}$，以下不等式成立:

$$
f\left( x\right) + {f}^{ * }\left( {{A}^{ * }y}\right) \geq \left\langle {{A}^{ * }y, x}\right\rangle = \langle y,{Ax}\rangle = - \langle - y,{Ax}\rangle \geq - g\left( {Ax}\right) - {g}^{ * }\left( {-y}\right) .
$$

比较最左边的项和最右边的项得到

$$
f\left( x\right) + {f}^{ * }\left( {{A}^{ * }y}\right) \geq - g\left( {Ax}\right) - {g}^{ * }\left( {-y}\right) \Leftrightarrow f\left( x\right) + g\left( {Ax}\right) \geq - {f}^{ * }\left( {{A}^{ * }y}\right) - {g}^{ * }\left( {-y}\right) .
$$

对最后一个不等式的左边关于 $x \in X$ 取下确界，对右边关于 $y \in y$ 取上确界得到 ${p}^{ * } \geq {d}^{ * }$。

现在考虑函数 $h : y \rightarrow \left\lbrack {-\infty , + \infty }\right\rbrack$，它对于所有 $u \in y$ 定义为

$$
h\left( u\right) = \mathop{\inf }\limits_{{x \in \mathcal{X}}}\{ f\left( x\right) + g\left( {{Ax} + u}\right) \} . \tag{B.24}
$$

由于 $\left( {x, u}\right) \mapsto f\left( x\right) + g\left( {{Ax} + u}\right)$ 是凸函数，$h$ 作为该函数一个变量的下确界也是凸的。$u$ 在 $\operatorname{dom}\left( h\right)$ 中当且仅当存在 $x \in \mathcal{X}$ 使得 $f\left( x\right) + g\left( {{Ax} + u}\right) < + \infty$，即存在 $x \in \mathfrak{X}$ 使得 $f\left( x\right) < + \infty$ 且 $g\left( {{Ax} + u}\right) < + \infty$，即存在 $x \in \operatorname{dom}\left( f\right)$ 使得 $\left( {{Ax} + u}\right) \in \operatorname{dom}\left( g\right)$。因此，我们有 $\operatorname{dom}\left( h\right) = \operatorname{dom}\left( g\right) - A\operatorname{dom}\left( f\right)$。

如果 ${p}^{ * } = - \infty$ ，那么显然强对偶性成立。否则，${p}^{ * } > - \infty$ 。如果 $0 \in \operatorname{core}(\operatorname{dom}\left( g\right) -$ $A\left( {\operatorname{dom}\left( f\right) }\right) ) = \operatorname{core}\left( {\operatorname{dom}\left( h\right) }\right)$ ，那么 0 在 $\operatorname{dom}\left( h\right)$ 中且 ${p}^{ * } < + \infty$ 。因此，${p}^{ * } = h\left( 0\right)$ 在 $\mathbb{R}$ 中。根据命题 B.34，由于 $h\left( 0\right) > - \infty$ 且 $0 \in \operatorname{core}\left( {\operatorname{dom}\left( h\right) }\right) , h$ 取值在 $( - \infty , + \infty \rbrack$ 中。因此，根据命题 B.35，$h$ 在 0 处允许有一个子梯度 $- y$ 。根据 $y$ 的定义，对于所有 $x \in x$ 和 $u \in y$ ，

$$
h\left( 0\right) \leq h\left( u\right) + \langle y, u\rangle
$$

$$
\leq f\left( x\right) + g\left( {{Ax} + u}\right) + \langle y, u\rangle
$$

$$
= \left\{ {f\left( x\right) - \left\langle {{A}^{ * }y, x}\right\rangle }\right\} + \left\{ {g\left( {{Ax} + u}\right) +\langle y, u\rangle + \left\langle {{A}^{ * }y, x}\right\rangle }\right\}
$$

$$
= \left\{ {f\left( x\right) - \left\langle {{A}^{ * }y, x}\right\rangle }\right\} + \{ g\left( {{Ax} + u}\right) + \langle y,{Ax} + u\rangle \} .
$$

对 $u$ 取下确界，对 $x$ 取上确界，可以得到

$$
h\left( 0\right) \leq - {f}^{ * }\left( {{A}^{ * }y}\right) - {g}^{ * }\left( {-y}\right) \leq {d}^{ * } \leq {p}^{ * } = h\left( 0\right) ,
$$

这证明了 ${d}^{ * } = {p}^{ * }$ 以及定义 ${d}^{ * }$ 的上确界在 $y$ 处达到。

最后，假设 $A\left( {\operatorname{dom}\left( f\right) }\right) \cap \operatorname{cont}\left( g\right) \neq \varnothing$ 并且令 $u \in A\left( {\operatorname{dom}\left( f\right) }\right) \cap \operatorname{cont}\left( g\right)$ 。那么，$u = {Ax}$ ，其中 $x \in \operatorname{dom}\left( f\right)$ 和 $u \in \operatorname{cont}\left( g\right) \subseteq \operatorname{dom}\left( g\right)$ 。因此，我们有 $0 = u - {Ax} \in \operatorname{dom}\left( g\right) - A\operatorname{dom}\left( f\right)$ 。由于 $g$ 在 $u$ 处连续且 $g\left( u\right)$ 有限，对于任何 $v \in X$ ，存在 $\epsilon > 0$ 使得对于所有 $t \in \left\lbrack {0,\epsilon }\right\rbrack$ ，$g\left( {u + {tv}}\right)$ 是有限的，因此 ${w}_{t} = \left( {u + {tv}}\right) \in \operatorname{dom}\left( g\right)$ 。因此，对于任何 $t \in \left\lbrack {0,\epsilon }\right\rbrack ,{tv} = {w}_{t} - u =$ ${w}_{t} - {Ax} \in \operatorname{dom}\left( g\right) - A\operatorname{dom}\left( f\right)$ ，这表明 $0 \in \operatorname{core}\left( {\operatorname{dom}\left( g\right) - A\left( {\operatorname{dom}\left( f\right) }\right) }\right)$ 。

为了说明这个定理，考虑 $A$ 是恒等算子的情况。那么原优化问题就是 $\mathop{\min }\limits_{x}\{ f\left( x\right) + g\left( x\right) \}$ 。图 B.4 在那种情况下说明了 Fenchel 对偶定理。原问题包括找到点 ${x}^{ * }$，在该点上 $f\left( x\right)$ 和 $- g\left( x\right)$ 的图像之间的距离最小，因为 $f\left( x\right) + g\left( x\right) = f\left( x\right) - \left( {-g\left( x\right) }\right)$ 。如图所示，在定理的条件下，这等同于寻找 ${y}^{ * }$，在该点上 $f\left( x\right)$ 和 $- g\left( x\right)$ 的共轭值之差，即差值 $- {f}^{ * }\left( y\right) - {g}^{ * }\left( {-y}\right)$ 最大。