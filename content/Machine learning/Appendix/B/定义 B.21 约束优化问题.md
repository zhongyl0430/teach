> [!definition] 定义B.21 约束优化问题
> 令 $\mathcal{X} \subseteq {\mathbb{R}}^{N}$ 和 $f, {g}_{i} : \mathcal{X} \rightarrow \mathbb{R}$，对于所有 $i \in \left\lbrack m\right\rbrack$。
> 那么，一个约束优化问题具有以下形式:
> $$
> \mathop{\min }\limits_{{\mathbf{x} \in \mathcal{X}}}f\left( \mathbf{x}\right)
> $$
> subject to:
> $$
> {g}_{i}\left( \mathbf{x}\right) \leq 0,\quad \forall i \in \{ 1,\ldots , m\} \text{.}
> $$

这个一般公式没有做任何凸性假设，并且可以增加等式约束。
它与稍后引入的相关问题相对，被称为 **原问题**。
我们将用 ${p}^{ * }$ 表示目标函数的最优值。

对于任意 $\mathbf{x} \in \mathcal{X}$，我们用 $g\left( \mathbf{x}\right)$ 表示向量 $${\left( {g}_{1}\left( \mathbf{x}\right) ,\ldots ,{g}_{m}\left( \mathbf{x}\right) \right) }^{\top }$$
因此，约束条件可以写作 $$\mathbf{g} \left( \mathbf{x}\right) \leq \mathbf{0} .$$