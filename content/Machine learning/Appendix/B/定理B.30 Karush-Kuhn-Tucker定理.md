
> [!theorem] 定理B.30 Karush-Kuhn-Tucker定理
> 假设 $f$, ${g}_{i}$ :$X \rightarrow \mathbb{R},\forall i \in \left\lbrack m\right\rbrack$, 
> - 是凸的且可微，
> - 约束条件合格。
> 
> 那么 $\overline{\mathbf{x}}$ 是约束程序的解 当且仅当 存在 $\overline{\mathbf{\alpha }} \geq 0$ 使得，
> $$
> \begin{align}
> {\nabla }_{\mathbf{x}} \mathcal{L}\left( \overline{\mathbf{x}}, \overline{\mathbf{\alpha }} \right) 
> &= {\nabla }_{\mathbf{x}} f\left( \overline{\mathbf{x}} \right) + \overline{\mathbf{\alpha }} \cdot {\nabla }_{\mathbf{x}} g\left( \overline{\mathbf{x}} \right) = 0, \tag{B.11} \\
> {\nabla }_{\mathbf{\alpha }} \mathcal{L}\left( \overline{\mathbf{x}}, \overline{\mathbf{\alpha }} \right) 
> &= g\left( \overline{\mathbf{x}} \right) \leq 0, \tag{B.12} \\
> \overline{\mathbf{\alpha }} \cdot g\left( \overline{\mathbf{x}} \right) 
> &= \mathop{\sum }\limits_{{i = 1}}^{m} {\overline{\mathbf{\alpha }}}_{i} {g}_{i}\left( \overline{\mathbf{x}} \right) = 0. \tag{B.13}
> \end{align}
> $$
> 条件 B.11-B.13 被称为 **KKT条件**。
> 
> 注意，最后两个 KKT条件 等价于
> $$
> g\left( \overline{\mathbf{x}}\right) \leq 0 \land \left( {\forall i \in \{ 1,\ldots , m\} ,{\bar{\alpha }}_{i}{g}_{i}\left( \overline{\mathbf{x}}\right) = 0}\right) . \tag{B.14}
> $$
> 
> 这些等式被称为 **互补条件**。

`\begin{proof}`
对于正向，由于约束条件合格，如果 $\overline{\mathbf{x}}$ 是解，那么存在 $\overline{\mathbf{\alpha }}$ 使得 $\left( {\overline{\mathbf{x}},\overline{\mathbf{\alpha }}}\right)$ 是拉格朗日函数的鞍点且三个条件均满足(第一个条件由鞍点的定义得出，后两个条件由(B.10)得出)。

在相反的方向，如果条件满足，那么对于任何 $\mathbf{x}$ 使得 $g\left( \mathbf{x}\right) \leq 0$ ，我们可以写出
$$
\begin{align}
&f\left( \mathbf{x} \right) - f\left( \overline{\mathbf{x}} \right) \\
&\geq {\nabla }_{\mathbf{x}} f\left( \overline{\mathbf{x}} \right) \cdot \left( \mathbf{x} - \overline{\mathbf{x}} \right) 
\quad \text{(convexity of } f\text{)} \\
&= - \mathop{\sum }\limits_{i = 1}^{m} \overline{\alpha }_{i} {\nabla }_{\mathbf{x}} g_{i}\left( \overline{\mathbf{x}} \right) \cdot \left( \mathbf{x} - \overline{\mathbf{x}} \right) 
\quad \text{(first condition)} \\
&\geq - \mathop{\sum }\limits_{i = 1}^{m} \overline{\mathbf{\alpha }}_{i} \left[ g_{i}\left( \mathbf{x} \right) - g_{i}\left( \overline{\mathbf{x}} \right) \right] 
\quad \text{(convexity of } g_{i}\text{s)} \\
&= - \mathop{\sum }\limits_{i = 1}^{m} \overline{\mathbf{\alpha }}_{i} g_{i}\left( \mathbf{x} \right) \geq 0 
\quad \text{(third condition)}.
\end{align}
$$
这表明 $f\left( \overline{\mathbf{x}}\right)$ 是满足约束条件点集中 $f$ 的最小值。
`\end{proof}`