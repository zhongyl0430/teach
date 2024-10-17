
> [!theorem] 定理 2.5 (学习界限 —  $\mathcal{H}$ 有限一致情况)
> 设
> - $\mathcal{H}$ 为从 $\mathcal{X}$ 到 $\mathcal{Y}$ 的函数的有限集合
> - $\mathcal{A}$ 为一个算法：
> 	- 对于任何
> 		- 目标概念 $c \in \mathcal{H}$ 
> 		- 独立同分布样本 $S$ 
> 	- 它返回一个一致假设 ${h}_{S} : {\widehat{R}}_{S}\left( {h}_{S}\right) = 0$
> 
> 那么，对于任何 $\epsilon ,\delta > 0$ ，如果
> $$
> m \geq \frac{1}{\epsilon }\left( {\log \left| \mathcal{H}\right| + \log \frac{1}{\delta }}\right) \tag{2.8}
> $$
> 我们有
> $$
> \mathbb{P}_{S \sim \mathcal{D}^m} \left[ R(h_S) \leq \epsilon \right] \geq 1 - \delta .
> $$

^thm-2-5

> [!remark] 等价描述
> 样本复杂性结果允许以下等价陈述作为一般化界限：对于任何 $\epsilon ,\delta > 0$ ，以至少 $1 - \delta$ 的概率，
> $$
> R\left( {h}_{S}\right) \leq \frac{1}{m}\left( {\log \left| \mathcal{H}\right| + \log \frac{1}{\delta }}\right) \tag{2.9}
> $$

^eq-2-9

`\begin{proof}`
- 固定 $\epsilon > 0$ 。
- 我们不知道算法 $\mathcal{A}$ 选择了哪个一致假设 ${h}_{S} \in \mathcal{H}$ 。
	- 这个假设依赖于训练样本 $S$ 。
- 我们需要给出一个统一的收敛界限，即对所有一致假设集都成立的界限，这自然包含 ${h}_{S}$ 。
- 我们将界定某些 $h \in \mathcal{H}$ 的一致性概率及其误差超过 $\epsilon$ 的可能性。
---
- 对于任意 $\epsilon > 0$ ， 
- 通过 ${\mathcal{H}}_{\epsilon } = \{ h \in \mathcal{H} : R\left( h\right) > \epsilon \}$ 定义 ${\mathcal{H}}_{\epsilon }$ 。
- 在从 $S$ 中独立同分布地抽取的训练样本上， 一个假设 $h$ 在 ${\mathcal{H}}_{\epsilon }$ 中的一致性可以被如下界定：
$$
\mathbb{P}\left\lbrack {{\widehat{R}}_{S}\left( h\right) = 0}\right\rbrack \leq {\left( 1 - \epsilon \right) }^{m}
$$
---
因此，根据并集界定，以下成立：
$$
\begin{aligned}
&\mathbb{P}\left\lbrack {\exists h \in {\mathcal{H}}_{\epsilon } : {\widehat{R}}_{S}\left( h\right) = 0}\right\rbrack \\
= & \mathbb{P}\left\lbrack {{\widehat{R}}_{S}\left( {h}_{1}\right) = 0 \vee \cdots \vee {\widehat{R}}_{S}\left( {h}_{\left| {\mathcal{H}}_{\epsilon }\right| }\right) = 0}\right\rbrack \\
\leq &\mathop{\sum }\limits_{{h \in {\mathcal{H}}_{\epsilon }}}\mathbb{P}\left\lbrack {{\widehat{R}}_{S}\left( h\right) = 0}\right\rbrack \\
\leq & \mathop{\sum }\limits_{{h \in {\mathcal{H}}_{\epsilon }}}{\left( 1 - \epsilon \right) }^{m} \\
\leq &\left| \mathcal{H}_{\epsilon}\right| {\left( 1 - \epsilon \right) }^{m} \\
\leq &\left| \mathcal{H}\right| {e}^{-{m\epsilon }}.
\end{aligned}
$$
将右侧设置为等于 $\delta$ 并求解 $\epsilon$，证明结束。 
`\end{proof}`

---
> [!remark] 样本大小对学习界的影响
> 定理表明，
> - 当假设集 $\mathcal{H}$ 是有限的时候，
> - 一个一致算法 $\mathcal{A}$ 是一个PAC学习算法，
> 	- 因为由 [[#^thm-2-5|(2.8)]] 给出的样本复杂度被 $1/\epsilon$ 和 $1/\delta$ 的多项式主导。
> 
> 如  [[#^eq-2-9|(2.9)]]  所示，一致假设的泛化误差被一个随样本大小 $m$ 减小的项界定。
> 
> 这是一个普遍的事实：
> - 如预期的那样，学习算法从更大的标记训练样本中获益。
> - 然而，本定理保证的 $O\left( {1/m}\right)$ 的减少率特别有利。

---
> [!remark] 代价
> 为提出一个一致算法所付出的代价是
> - 使用一个包含目标概念的更大假设集 $\mathcal{H}$ 。
> - 上界 [[#^eq-2-9|(2.9)]] 随着 $\left| \mathcal{H}\right|$ 的增加而增加。
> 	- 然而，这种依赖关系是对数级别的。
> 	-  $\log \left| \mathcal{H}\right|$ 可以解释为表示 $\mathcal{H}$ 所需的位数。
> - 因此，定理的泛化保证由这个位数 ${\log }_{2}\left| \mathcal{H}\right|$ 与样本大小 $m$ 的比例控制。
