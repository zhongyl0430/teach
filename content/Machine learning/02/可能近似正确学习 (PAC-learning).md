---
tags:
  - "#teach/ML"
---
- 设 $n$ 为一个数，使得
	- 表示任何元素 $x \in \mathcal{X}$ 的计算成本至多为 $O\left( n\right)$
- 记 $\text{size} ( c )$ 为 $c \in \mathcal{C}$ 的计算表示的最大成本。
	- 例如，$x$ 可能是 ${\mathbb{R}}^{n}$ 中的一个向量，对于该向量，基于数组的表示成本将在 $O\left( n\right)$ 内。
- 设 ${h}_{S}$ 表示算法 $\mathcal{A}$ 在接收到标记样本 $S$ 后返回的假设。
	- 为了简化记号，不显式指出 ${h}_{S}$ 对 $\mathcal{A}$ 的依赖性。

> [!definition] PAC学习
> 一个概念类 $\mathcal{C}$ 称为 **PAC 可学习的**， 如果存在
> - 一个算法 $\mathcal{A}$ 
> - 一个多项式函数 poly $\left( {\cdot ,\cdot ,\cdot , \cdot }\right)$
>
>使得对于任何
>- $\epsilon > 0$ 
>- $\delta > 0$
>- 在 $X$ 上的分布 $\mathcal{D}$ 
>- 任何目标概念 $c \in \mathcal{C}$
>
>以下对于任何大小 $m \geq \operatorname{poly}\left( {1/\epsilon ,1/\delta, n,\operatorname{size}\left( c\right) }\right)$ 的样本都成立：
> $$
> \underset{S \sim {\mathcal{D}}^{m}}{\mathbb{P}}\left\lbrack {R\left( {h}_{S}\right) \leq \epsilon }\right\rbrack \geq 1 - \delta . \tag{2.4}
> $$

^def-PAC-learning

> [!definition] 有效 PAC 学习
> 如果 $\mathcal{A}$ 进一步在多项式时间 $\left( {1/\epsilon ,1/\delta, n,\operatorname{size}\left( c\right) }\right)$ 内运行，则称 $\mathcal{C}$ 为 **有效 (efficiently)** PAC可学习的。
> 当存在这样的算法 $\mathcal{A}$ 时，它被称为 $\mathcal{C}$ 的 **PAC学习算法 (PAC-learning algorithm)** 。

^def-efficiently-PAC
> [!remark] PAC 学习的理解
> - 一个概念类 $\mathcal{C}$ 是 PAC 可学习的，
> 	- 如果算法在观察到的点的数量为 $1/\epsilon$ 和 $1/\delta$ 的多项式时
> 	- 返回的假设大致正确（错误至多 $\epsilon$），并且以高概率（至少 $1 - \delta$）成立。
> - 参数 $\delta > 0$ 用于定义置信度 $1 - \delta$ 和精度 $1 - \epsilon$。
> - 如果算法的运行时间是 $1/\epsilon$ 和 $1/\delta$ 的多项式，那么如果算法接收到全部样本，样本大小 $m$ 也必须是多项式级别的。

---
> [!remark]
> PAC 定义的几个关键点值得强调。
> 1. PAC 框架是一个无分布模型：
> 	- 对于从哪个分布 $\mathcal{D}$ 中抽取示例没有任何特定假设。
> 2. 其次，用于定义错误的训练样本和测试示例是根据相同的分布 $\mathcal{D}$ 抽取的。
> 	- 这是在一般情况下实现泛化所必需的自然且必要的假设。
> 	- 它可以放宽以包括有利的领域适应问题。
> 3. 最后，PAC 框架处理的是概念类 $\mathcal{C}$ 的可学习性问题，而不是特定概念。
>	- 算法知道概念类 $\mathcal{C}$，但目标概念 $c \in \mathcal{C}$ 是未知的。
>	- 在许多情况下，特别是当概念的计算表示没有明确讨论或者很简单时，我们可以在 PAC 定义中
>		- 省略对 $n$ 和 $\operatorname{size}\left( c\right)$ 的多项式依赖，
>		- 只关注样本复杂性。