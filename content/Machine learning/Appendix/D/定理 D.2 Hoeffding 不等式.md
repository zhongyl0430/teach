> [!theorem] 定理 D.2 Hoeffding 不等式
> - 设 ${X}_{1},\ldots ,{X}_{m}$ 为独立随机变量，
> 	- ${X}_{i}$ 取值在 $\left\lbrack {{a}_{i},{b}_{i}}\right\rbrack$ 内对所有 $i \in \left\lbrack m\right\rbrack$ 成立。
> - 那么，对于任意 $\epsilon > 0$
> 	- 以下不等式对 ${S}_{m} = \mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i}$ 成立:
> $$
> \begin{align}
> \mathbb{P}\left[ {{S}_{m} - \mathbb{E}[ {S}_{m}] \geq \epsilon }\right] &\leq e^{-2{\epsilon }^{2}/\sum_{i=1}^{m}{( {b}_{i} - {a}_{i}) }^{2}} \tag{D.4}\\
> \mathbb{P}\left[ {{S}_{m} - \mathbb{E}[ {S}_{m}] \leq - \epsilon }\right] &\leq e^{-2{\epsilon }^{2}/\sum_{i=1}^{m}{( {b}_{i} - {a}_{i}) }^{2}}. \tag{D.5}
> \end{align}
> $$

^thm-Hoeffding-ineq

`\begin{proof}`
使用 Chernoff 边界技巧和引理 D.1，我们可以写出:
$$
\begin{align}
&\mathbb{P} \left[ S_{m} - \mathbb{E}[S_{m}] \geq \epsilon \right] \\
&\leq e^{-t\epsilon} \mathbb{E} \left[ e^{t(S_{m} - \mathbb{E}[S_{m}])} \right] \\
&= e^{-t\epsilon} \prod_{i=1}^{m} \mathbb{E}\left[ e^{t(X_{i} - \mathbb{E}[X_{i}])} \right] \quad \text{(independence of } X_{i} \text{s)} \\
&\leq e^{-t\epsilon} \prod_{i=1}^{m} e^{t^2 (b_{i} - a_{i})^2/8} \quad (\text{lemma D.1}) \\
&= e^{-t\epsilon} e^{t^2 \sum_{i=1}^{m} (b_{i} - a_{i})^2/8} \\
&\leq e^{-2\epsilon^2/\sum_{i=1}^{m} (b_{i} - a_{i})^2}.
\end{align}
$$
其中我们选择 $t = {4\epsilon }/\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {b}_{i} - {a}_{i}\right) }^{2}$ 以最小化上界。
这证明了定理的第一个陈述，第二个陈述以类似方式证明。
`\end{proof}`