> [!definition] 定义 B.23 对偶函数
> 与约束优化问题相关的 **（拉格朗日）对偶函数** 定义为 $\forall \mathbf{\alpha } \geq 0$
> $$
> \begin{align}
> &F\left( \mathbf{\alpha }\right) \\
> &= \mathop{\inf }\limits_{{\mathbf{x} \in \mathcal{X}}}\mathcal{L}\left( {\mathbf{x},\mathbf{\alpha }}\right) \\
> &= \mathop{\inf }\limits_{{\mathbf{x} \in \mathcal{X}}}\left( {f\left( \mathbf{x}\right) + \mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i}{g}_{i}\left( \mathbf{x}\right) }\right) . \tag{B.5}
> \end{align}
> $$

注意 $F$ 始终是凹的，因为拉格朗日函数关于 $\mathbf{\alpha }$ 是线性的，并且下确界保持凹性。

我们进一步观察到
$$
F\left( \mathbf{\alpha }\right) \leq {p}^{ * } , \forall \mathbf{\alpha } \geq 0\tag{B.6}
$$
这是因为对于任意可行的 $\mathbf{x}$, $$f\left( \mathbf{x}\right) + \mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i}{g}_{i}\left( \mathbf{x}\right) \leq f\left( \mathbf{x}\right)$$