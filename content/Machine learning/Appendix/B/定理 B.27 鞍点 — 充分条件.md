> [!theorem] 定理 B.27 鞍点 — 充分条件
> 取 $P$ 为 $\mathcal{X} = {\mathbb{R}}^{N}$ 上的约束优化问题。
> 如果 $\left( {{\mathbf{x}}^{ * },{\mathbf{\alpha }}^{ * }}\right)$ 是相关拉格朗日的鞍点，即，
> 
> $\forall \mathbf{x} \in {\mathbb{R}}^{N}$, $\forall \mathbf{\alpha} \geq 0$, 
> $$
> \mathcal{L}\left( {{\mathbf{x}}^{ * },\mathbf{\alpha }}\right) \leq \mathcal{L}\left( {{\mathbf{x}}^{ * },{\mathbf{\alpha }}^{ * }}\right) \leq \mathcal{L}\left( {\mathbf{x},{\mathbf{\alpha }}^{ * }}\right) \tag{B.9}
> $$
> 
> 那么 ${\mathbf{x}}^{ * }$ 是问题 $P$ 的解。

`\begin{proof}`
根据第一个不等式，以下成立:
$$
\begin{align}
&\forall \mathbf{\alpha } \geq 0,\; \mathcal{L}\left( \mathbf{x}^{*}, \mathbf{\alpha} \right) \leq \mathcal{L}\left( \mathbf{x}^{*}, \mathbf{\alpha}^{*} \right) \\
&\Rightarrow \forall \mathbf{\alpha } \geq 0,\; \mathbf{\alpha } \cdot g\left( \mathbf{x}^{*} \right) 
\leq \mathbf{\alpha}^{*} \cdot g\left( \mathbf{x}^{*} \right) \\
&\Rightarrow g\left( \mathbf{x}^{*} \right) \leq 0 \land \mathbf{\alpha}^{*} \cdot g\left( \mathbf{x}^{*} \right) = 0. \tag{B.10}
\end{align}
$$
其中
- $g\left( {\mathbf{x}}^{ * }\right) \leq 0$ 在 (B.10) 中通过令 $\mathbf{\alpha } \rightarrow + \infty$ 得出，
-  ${\mathbf{\alpha }}^{ * } \cdot g\left( {\mathbf{x}}^{ * }\right) = 0$ 通过令 $\mathbf{\alpha } \rightarrow 0$ 得出。

鉴于 (B.10)，(B.9) 中的第二个不等式给出，
$$
\begin{align}
&\forall \mathbf{x},\; \mathcal{L}\left( \mathbf{x}^{*}, \mathbf{\alpha}^{*} \right) \leq \mathcal{L}\left( \mathbf{x}, \mathbf{\alpha}^{*} \right) \\
&\Rightarrow \forall \mathbf{x},\; f\left( \mathbf{x}^{*} \right) 
\leq f\left( \mathbf{x} \right) + \mathbf{\alpha}^{*} \cdot g\left( \mathbf{x} \right).
\end{align}
$$
因此，对于所有满足约束的 $\mathbf{x}$ ，即 $g\left( \mathbf{x}\right) \leq 0$ ，我们有
$$
f\left( {\mathbf{x}}^{ * }\right) \leq f\left( \mathbf{x}\right)
$$

这完成了证明。
`\end{proof}`