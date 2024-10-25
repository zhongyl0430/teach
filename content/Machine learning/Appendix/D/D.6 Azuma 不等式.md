## D.6 Azuma 不等式

本节介绍了一个比霍夫丁不等式更一般的集中不等式。其证明利用了针对随机游走差分的霍夫丁不等式。

定义 D.5 (随机游走差分)
一列随机变量 ${V}_{1},{V}_{2},\ldots$ 是关于 ${X}_{1},{X}_{2},\ldots$ 的随机游走差分序列，如果对于所有 $i > 0$, ${V}_{i}$ 是 ${X}_{1},\ldots ,{X}_{i}$ 的函数且
$$
\mathbb{E}\left\lbrack {{V}_{i + 1} \mid {X}_{1},\ldots ,{X}_{i}}\right\rbrack = 0. \tag{D.9}
$$

下面的结果与霍夫丁引理相似。

引理 D.6 设 $V$ 和 $Z$ 是满足 $\mathbb{E}\left\lbrack {V \mid Z}\right\rbrack = 0$ 的随机变量，对于某个函数 $f$ 和常数 $c \geq 0$ ，不等式:

$$
f\left( Z\right) \leq V \leq f\left( Z\right) + c. \tag{D.10}
$$

然后，对于所有 $t > 0$ ，以下的上界成立:

$$
\mathbb{E}\left\lbrack {{e}^{tV} \mid Z}\right\rbrack \leq {e}^{{t}^{2}{c}^{2}/8}. \tag{D.11}
$$

证明:证明步骤与引理 D.1 相同，只是用条件期望代替期望:在 $Z, V$ 取值在 $\left\lbrack {a, b}\right\rbrack$ 且 $a = f\left( Z\right)$ 和 $b = f\left( Z\right) + c$ 的条件下，其期望消失。

该引理用于证明以下定理，该定理是本节的主要结果之一。

定理 D.7(Azuma 不等式) 
设 ${V}_{1},{V}_{2},\ldots$  是关于随机变量 ${X}_{1},{X}_{2},\ldots$ 的谱，并假设对于所有 $i > 0$ 存在一个常数 ${c}_{i} \geq 0$ 以及随机变量 ${Z}_{i}$ ，它是 ${X}_{1},\ldots ,{X}_{i - 1}$ 的函数，满足
$$
{Z}_{i} \leq {V}_{i} \leq {Z}_{i} + {c}_{i} \tag{D.12}
$$
然后，对于所有 $\epsilon > 0$ 和 $m$ ，以下不等式成立:
$$
\begin{align}
\mathbb{P}\left\lbrack {\mathop{\sum }\limits_{{i = 1}}^{m}{V}_{i} \geq \epsilon }\right\rbrack &\leq \exp \left( \frac{-2{\epsilon }^{2}}{\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}^{2}}\right) \tag{D.13} \\
\mathbb{P}\left\lbrack {\mathop{\sum }\limits_{{i = 1}}^{m}{V}_{i} \leq - \epsilon }\right\rbrack &\leq \exp \left( \frac{-2{\epsilon }^{2}}{\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}^{2}}\right) . \tag{D.14}
\end{align}
$$

证明:对于任意 $k \in \left\lbrack m\right\rbrack$ ，设 ${S}_{k} = \mathop{\sum }\limits_{{i = 1}}^{k}{V}_{k}$ 。然后，使用 Chernoff 边界技术，对于任意 $t > 0$ ，我们可以写出

$$
\mathbb{P}\left\lbrack {{S}_{m} \geq \epsilon }\right\rbrack \leq {e}^{-{t\epsilon }}\mathbb{E}\left\lbrack {e}^{t{S}_{m}}\right\rbrack
$$

$$
= {e}^{-{t\epsilon }}\mathbb{E}\left\lbrack {{e}^{t{S}_{m - 1}}\mathbb{E}\left\lbrack {{e}^{t{\mathbf{V}}_{m}} \mid {X}_{1},\ldots ,{X}_{m - 1}}\right\rbrack }\right\rbrack
$$

$$
\leq {e}^{-{t\epsilon }}\mathbb{E}\left\lbrack {e}^{t{S}_{m - 1}}\right\rbrack {e}^{{t}^{2}{c}_{m}^{2}/8} \tag{lemma D.6}
$$

$$
\leq {e}^{-{t\epsilon }}{e}^{{t}^{2}\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}^{2}/8} \tag{iterating previous argument}
$$

$$
= {e}^{-2{\epsilon }^{2}/\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}^{2}},
$$

其中我们选择 $t = {4\epsilon }/\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}^{2}$ 以最小化上界。这证明了定理的第一个陈述，第二个陈述以类似的方式证明。