要定义假设集 $\mathcal{H}$ 的 VC 维度，我们首先引入*打碎 (shattering)* 的概念。
回顾上一节，
- 给定一个假设集 $\mathcal{H}$，
- 集合 $S$ 的一个 *二分法* 是使用 $\mathcal{H}$ 中的假设对 $S$ 的点进行标记的所有可能方式。

> [!definition] $\mathcal{H}$ 打碎 $S$
> - 一个 $m \geq 1$ 的点集合 $S$ 被称为 **被假设集 $\mathcal{H}$ 打碎**，
> - 当且仅当 $\mathcal{H}$ 实现了 $S$ 的所有可能的二分法，
> 	- i.e.  ${\Pi }_{\mathcal{H}}\left( m\right) = {2}^{m}$ 

> [!definition] 定义 3.10（VC 维度）
> - 假设集 $\mathcal{H}$ 的 **VC 维度** 是 $\mathcal{H}$ 可以打碎的最大集合的大小：
$$\operatorname{VCdim}\left( \mathcal{H}\right) = \max \left\{ {m : {\Pi }_{\mathcal{H}}\left( m\right) = {2}^{m}}\right\} . \tag{3.24}$$

> [!remark]
> 请注意，根据定义，
> - 如果 $\operatorname{VCdim}\left( \mathcal{H}\right) = d$，
> 	- 则 *存在* 一个大小为 $d$ 的集合可以被打碎。
> - 然而，这并不意味着 *所有* 大小为 $d$ 或更小的集合都被打碎，
> 	- 实际上，通常并非如此。

