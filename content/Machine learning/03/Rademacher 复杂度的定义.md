
> [!definition] 经验 Rademacher 复杂度
> 设
> - $\mathcal{G}$ 为从 $\mathcal{Z}$ 映射到区间 $\left\lbrack {a,b}\right\rbrack$ 的函数族
> - $S = \left( {{z}_{1},\ldots ,{z}_{m}}\right)$ 为包含 $\mathcal{Z}$ 中元素的固定大小为 $m$ 的样本。
> 那么，$\mathcal{G}$ 关于样本 $S$ 的 **经验 Rademacher 复杂度** 定义为：
> $${\widehat{\mathfrak{R}}}_{S}\left( \mathcal{G}\right) = \underset{\mathbf{\sigma }}{\mathbb{E}}\left\lbrack {\mathop{\sup }\limits_{{g \in \mathcal{G}}}\frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{\sigma }_{i}g\left( {z}_{i}\right) }\right\rbrack \tag{3.1}$$
> 其中，
> - $\mathbf{\sigma } = {\left( {\sigma }_{1},\ldots ,{\sigma }_{m}\right) }^{\top}$，
> - ${\sigma }_{i}$ 是取值于 $\{ - 1, + 1\}$ 的独立均匀随机变量。
> 	- 这些随机变量 ${\sigma }_{i}$ 被称为 **Rademacher 变量**。

- 设 ${\mathbf{g}}_{S}$ 表示函数 $g$ 在样本 $S$ 上取值的向量：
$${\mathbf{g}}_{S} = {\left( g\left( {z}_{1}\right) ,\ldots ,g\left( {z}_{m}\right) \right) }^{\top} .$$
- 则经验 Rademacher 复杂度可以重写为：
$${\widehat{\mathfrak{R}}}_{S}\left( \mathcal{G}\right) = \underset{\mathbf{\sigma }}{\mathbb{E}}\left\lbrack {\mathop{\sup }\limits_{{g \in \mathcal{G}}}\frac{\mathbf{\sigma } \cdot {\mathbf{g}}_{S}}{m}}\right\rbrack .$$
	- 内积 $\mathbf{\sigma } \cdot {\mathbf{g}}_{S}$ 衡量了 ${\mathbf{g}}_{S}$ 与随机噪声向量 $\mathbf{\sigma }$ 的相关性。
	- 上确界 $\mathop{\sup }\limits_{{g \in \mathcal{G}}}\frac{\mathbf{\sigma } \cdot {\mathbf{g}}_{S}}{m}$ 是一个度量函数类 $\mathcal{G}$ 在样本 $S$ 上与 $\mathbf{\sigma }$ 相关性的指标。
	- 因此，经验 Rademacher 复杂度平均衡量了 *函数类 $\mathcal{G}$ 在样本 $S$ 上与随机噪声的相关性*。
- 这描述了函数族 $\mathcal{G}$ 的丰富性：
	- 更丰富或更复杂的函数族 $\mathcal{G}$ 能够生成更多的向量 ${\mathbf{g}}_{S}$，
	- 因此能够平均上更好地与随机噪声相关。

> [!definition] Rademacher 复杂度
> - 设 $\mathcal{D}$ 表示用于抽取样本的分布。
> - 对于任意整数 $m \geq 1$，函数族 $\mathcal{G}$ 的 Rademacher 复杂度是:
> 	- 根据分布 $\mathcal{D}$ 抽取的大小为 $m$ 的所有样本上
> 	- 经验 Rademacher 复杂度的期望值:
> $${\mathfrak{R}}_{m}\left( \mathcal{G}\right) = \underset{S \sim {\mathcal{D}}^{m}}{\mathbb{E}}\left\lbrack {{\widehat{\mathfrak{R}}}_{S}\left( \mathcal{G}\right) }\right\rbrack \tag{3.2}$$
