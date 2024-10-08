## D. 3 乘法Chernoff界限

Sanov定理可以用来证明以下乘法Chernoff界限。

定理D.4(乘法Chernoff界限)${Let}\;{X}_{1},\ldots ,{X}_{m}\;{be}\;{independent}\;{random}\;{vari}$ - ables根据某个分布 $\mathcal{D}$ 抽取，该分布的平均值为 $p$ 且支撑集包含在 $\left\lbrack {0,1}\right\rbrack$ 中。那么，对于任何 $\gamma \in \left\lbrack {0,\frac{1}{p} - 1}\right\rbrack$ ，以下不等式对于 $\widehat{p} = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i}$ 成立:

$$
\mathbb{P}\left\lbrack {\widehat{p} \geq \left( {1 + \gamma }\right) p}\right\rbrack \leq {e}^{-\frac{{mp}{\gamma }^{2}}{3}}
$$

$$
\mathbb{P}\left\lbrack {\widehat{p} \leq \left( {1 - \gamma }\right) p}\right\rbrack \leq {e}^{-\frac{{mp}{\gamma }^{2}}{2}}.
$$

证明:证明包括在每个情况下推导出比Pinsker不等式更精细的二进制相对熵的下界。使用不等式 $\log \left( {1 + x}\right) \geq \frac{x}{1 + \frac{x}{2}}$ 和 $\log \left( {1 + x}\right) < x$ ，我们可以写出

$$
- \mathrm{D}\left( {\left( {1 + \gamma }\right) p\parallel p}\right) = \left( {1 + \gamma }\right) p\log \frac{p}{\left( {1 + \gamma }\right) p} + \left( {1 - \left( {1 + \gamma }\right) p}\right) \log \left\lbrack \frac{1 - p}{1 - \left( {1 + \gamma }\right) p}\right\rbrack
$$

$$
= \left( {1 + \gamma }\right) p\log \frac{1}{1 + \gamma } + \left( {1 - p - {\gamma p}}\right) \log \left\lbrack {1 + \frac{\gamma p}{1 - p - {\gamma p}}}\right\rbrack
$$

$$
\leq \left( {1 + \gamma }\right) p\frac{-\gamma }{1 + \frac{\gamma }{2}} + \left( {1 - p - {\gamma p}}\right) \frac{\gamma p}{1 - p - {\gamma p}}
$$

$$
= {\gamma p}\left\lbrack {1 - \frac{1 + \gamma }{1 + \frac{\gamma }{2}}}\right\rbrack = \frac{-\frac{{\gamma }^{2}p}{2}}{1 + \frac{\gamma }{2}} = \frac{-{\gamma }^{2}p}{2 + \gamma }
$$

$$
\leq \frac{-{\gamma }^{2}p}{2 + 1} = \frac{-{\gamma }^{2}p}{3}
$$

类似地，使用对于 $x \in \left( {0,1}\right)$ 和 $\log \left( {1 - x}\right) < - x$ 有效的 $\left( {1 - x}\right) \log \left( {1 - x}\right) \geq - x + \frac{{x}^{2}}{2}$ 不等式，我们可以写出

$$
- \mathrm{D}\left( {\left( {1 - \gamma }\right) p\parallel p}\right) = \left( {1 - \gamma }\right) p\log \frac{p}{\left( {1 - \gamma }\right) p} + \left( {1 - \left( {1 - \gamma }\right) p}\right) \log \left\lbrack \frac{1 - p}{1 - \left( {1 - \gamma }\right) p}\right\rbrack
$$

$$
= \left( {1 - \gamma }\right) p\log \frac{1}{1 - \gamma } + \left( {1 - p + {\gamma p}}\right) \log \left\lbrack {1 - \frac{\gamma p}{1 - p + {\gamma p}}}\right\rbrack
$$

$$
\leq \left( {\gamma - \frac{{\gamma }^{2}}{2}}\right) p + \left( {1 - p + {\gamma p}}\right) \frac{-{\gamma p}}{1 - p + {\gamma p}} = \frac{-{\gamma }^{2}p}{2}.
$$

这完成了证明。