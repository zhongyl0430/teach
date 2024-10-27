> [!definition] 定义 B.22 拉格朗日函数
> 与在 (B.21) 中定义的一般约束优化问题相关的**拉格朗日函数** 或 **拉格朗日量** 是定义在 $\mathcal{X} \times {\mathbb{R}}_{ + }$ 上的函数：$\forall \mathbf{x} \in \mathcal{X}, \forall \mathbf{\alpha } \geq 0$
> $$
> \mathcal{L}\left( {\mathbf{x},\mathbf{\alpha }}\right) = f\left( \mathbf{x}\right) + \mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i}{g}_{i}\left( \mathbf{x}\right) ,
> $$
> 
> 其中变量 ${\alpha }_{i}$ 称为 **拉格朗日变量** 或 **对偶变量**，$\mathbf{\alpha } = {\left( {\alpha }_{1},\ldots ,{\alpha }_{m}\right) }^{\top }$。

对于形式为 $g\left( \mathbf{x}\right) = 0$ 的函数 $g$ 的任意等式约束，可以等价地通过两个不等式来表示：
$$
\begin{align}
- g\left( \mathbf{x}\right) &\leq 0 \\
+ g\left( \mathbf{x}\right) &\leq 0 \\
\end{align}
$$
令
- ${\alpha }_{ - } \geq 0$ 为与第一个约束相关的拉格朗日变量，
- ${\alpha }_{ + } \geq 0$ 为与第二个约束相关的拉格朗日变量。

在拉格朗日函数的定义中，与这些约束对应的项的总和可以写作 ${\alpha g}\left( \mathbf{x}\right)$，其中 $\alpha = \left( {{\alpha }_{ + } - {\alpha }_{ - }}\right)$。
因此，通常对于等式约束 $g\left( \mathbf{x}\right) = 0$，拉格朗日函数会增加一项 ${\alpha g}\left( \mathbf{x}\right)$，但此时 $\alpha \in \mathbb{R}$，并不要求为非负数。
请注意，在凸优化问题的情况下，等式约束 $g\left( \mathbf{x}\right)$ 需要是仿射的，因为 $g\left( \mathbf{x}\right)$ 和 $- g\left( \mathbf{x}\right)$ 都需要是凸的。