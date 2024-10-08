引理D.1 (Hoeffding引理)
$X$ 是一个随机变量，具有 $E\left\lbrack X\right\rbrack = 0$ 和 $a \leq X \leq b$ ，并且 $b > a$ 。那么，对于任何 $t > 0$ ，以下不等式成立:
$$
\mathbb{E}\left\lbrack {e}^{tX}\right\rbrack \leq {e}^{\frac{{t}^{2}{\left( b - a\right) }^{2}}{8}}. \tag{D. 2}
$$

证明:由于 $x \mapsto {e}^{x}$ 的凸性，对于所有 $x \in \left\lbrack {a, b}\right\rbrack$ ，以下成立:

$$
{e}^{tx} \leq \frac{b - x}{b - a}{e}^{ta} + \frac{x - a}{b - a}{e}^{tb}.
$$

因此，使用 $\mathbb{E}\left\lbrack X\right\rbrack = 0$ ，

$$
\mathbb{E}\left\lbrack {e}^{tX}\right\rbrack \leq \mathbb{E}\left\lbrack {\frac{b - X}{b - a}{e}^{ta} + \frac{X - a}{b - a}{e}^{tb}}\right\rbrack = \frac{b}{b - a}{e}^{ta} + \frac{-a}{b - a}{e}^{tb} = {e}^{\phi \left( t\right) },
$$

其中，

$$
\phi \left( t\right) = \log \left( {\frac{b}{b - a}{e}^{ta} + \frac{-a}{b - a}{e}^{tb}}\right) = {ta} + \log \left( {\frac{b}{b - a} + \frac{-a}{b - a}{e}^{t\left( {b - a}\right) }}\right) .
$$

对于任何 $t > 0$ ，$\phi$ 的一阶和二阶导数如下:

$$
{\phi }^{\prime }\left( t\right) = a - \frac{a{e}^{t\left( {b - a}\right) }}{\frac{b}{b - a} - \frac{a}{b - a}{e}^{t\left( {b - a}\right) }} = a - \frac{a}{\frac{b}{b - a}{e}^{-t\left( {b - a}\right) } - \frac{a}{b - a}},
$$
$$
\begin{align}
{\phi }^{\prime \prime }\left( t\right) &= \frac{-{ab}{e}^{-t\left( {b - a}\right) }}{{\left\lbrack \frac{b}{b - a}{e}^{-t\left( {b - a}\right) } - \frac{a}{b - a}\right\rbrack }^{2}} \\
&= \frac{\alpha \left( {1 - \alpha }\right) {e}^{-t\left( {b - a}\right) }{\left( b - a\right) }^{2}}{{\left\lbrack \left( 1 - \alpha \right) {e}^{-t\left( {b - a}\right) } + \alpha \right\rbrack }^{2}} \\
&= \frac{\alpha }{{\left( \left( 1 - \alpha \right) {e}^{-t\left( {b - a}\right) } + \alpha \right)}^2} \cdot \frac{\left( 1 - \alpha \right) {e}^{-t\left( {b - a}\right)}}{{\left( \left( 1 - \alpha \right) {e}^{-t\left( {b - a}\right)} + \alpha \right)}^2}{\left( b - a \right)}^{2}.
\end{align}
$$
其中 $\alpha$ 表示 $\frac{-a}{b - a}$ 。注意 $\phi \left( 0\right) = {\phi }^{\prime }\left( 0\right) = 0$ 并且 ${\phi }^{\prime \prime }\left( t\right) = u\left( {1 - u}\right) {\left( b - a\right) }^{2}$ ，其中 $u = \frac{\alpha }{\left\lbrack \left( 1 - \alpha \right) {e}^{-t\left( {b - a}\right) } + \alpha \right\rbrack }$ 。由于 $u$ 在 $\left\lbrack {0,1}\right\rbrack , u\left( {1 - u}\right)$ 中，$\left\lbrack {0,1}\right\rbrack , u\left( {1 - u}\right)$ 被 $1/4$ 和 ${\phi }^{\prime \prime }\left( t\right) \leq \frac{{\left( b - a\right) }^{2}}{4}$ 界定。因此，通过函数 $\phi$ 的二阶展开，存在 $\theta \in \left\lbrack {0, t}\right\rbrack$ 使得:

$$
\phi \left( t\right) = \phi \left( 0\right) + t{\phi }^{\prime }\left( 0\right) + \frac{{t}^{2}}{2}{\phi }^{\prime \prime }\left( \theta \right) \leq {t}^{2}\frac{{\left( b - a\right) }^{2}}{8}, \tag{D.3}
$$

这完成了证明。
