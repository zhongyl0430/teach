我们现在定义一个一般的约束优化问题以及与凸约束优化问题相关的特定属性。

> [!definition] 定义B.21 约束优化问题
> 令 $X \subseteq {\mathbb{R}}^{N}$ 和 $f,{g}_{i} : X \rightarrow \mathbb{R}$，对于所有 $i \in \left\lbrack m\right\rbrack$。
> 那么，一个约束优化问题具有以下形式:
> $$
> \mathop{\min }\limits_{{\mathbf{x} \in \mathcal{X}}}f\left( \mathbf{x}\right)
> $$
> subject to:
> $$
> {g}_{i}\left( \mathbf{x}\right) \leq 0,\forall i \in \{ 1,\ldots , m\} \text{.}
> $$

这个一般公式没有做任何凸性假设，并且可以增加等式约束。
它与稍后引入的相关问题相对，被称为 **原问题**。
我们将用 ${p}^{ * }$ 表示目标函数的最优值。

对于任意 $\mathbf{x} \in \mathcal{X}$，我们用 $g\left( \mathbf{x}\right)$ 表示向量 ${\left( {g}_{1}\left( \mathbf{x}\right) ,\ldots ,{g}_{m}\left( \mathbf{x}\right) \right) }^{\top }$。
因此，约束条件可以写作 $g\left( \mathbf{x}\right) \leq \mathbf{0}$。
对于任何约束优化问题，我们可以关联一个拉格朗日函数，这在问题的分析及其与其他相关优化问题的关系中起着重要作用。

> [!definition] 定义 B.22 拉格朗日函数
> 与在 (B.21) 中定义的一般约束优化问题相关的拉格朗日函数或拉格朗日量是定义在 $x \times {\mathbb{R}}_{ + }$ 上的函数：$\forall \mathbf{x} \in \mathcal{X}, \forall \mathbf{\alpha } \geq 0$
> $$
> \mathcal{L}\left( {\mathbf{x},\mathbf{\alpha }}\right) = f\left( \mathbf{x}\right) + \mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i}{g}_{i}\left( \mathbf{x}\right) ,
> $$
> 
> 其中变量 ${\alpha }_{i}$ 称为拉格朗日变量或对偶变量，$\mathbf{\alpha } = {\left( {\alpha }_{1},\ldots ,{\alpha }_{m}\right) }^{\top }$。

对于形式为 $g\left( \mathbf{x}\right) = 0$ 的函数 $g$ 的任意等式约束，可以等价地通过两个不等式来表示：$- g\left( \mathbf{x}\right) \leq 0$ 和 $+ g\left( \mathbf{x}\right) \leq 0$。令 ${\alpha }_{ - } \geq 0$ 为与第一个约束相关的拉格朗日变量，${\alpha }_{ + } \geq 0$ 为与第二个约束相关的拉格朗日变量。因此，在拉格朗日函数的定义中，与这些约束对应的项的总和可以写作 ${\alpha g}\left( \mathbf{x}\right)$，其中 $\alpha = \left( {{\alpha }_{ + } - {\alpha }_{ - }}\right)$。因此，通常对于等式约束 $g\left( \mathbf{x}\right) = 0$，拉格朗日函数会增加一项 ${\alpha g}\left( \mathbf{x}\right)$，但此时 $\alpha \in \mathbb{R}$，并不要求为非负数。请注意，在凸优化问题的情况下，等式约束 $g\left( \mathbf{x}\right)$ 需要是仿射的，因为 $g\left( \mathbf{x}\right)$ 和 $- g\left( \mathbf{x}\right)$ 都需要是凸的。

> [!definition]
> 定义 B.23（对偶函数）与约束优化问题相关的（拉格朗日）对偶函数定义为 $\forall \mathbf{\alpha } \geq 0$
> $$
> \begin{align}
> F\left( \mathbf{\alpha }\right) 
> &= \mathop{\inf }\limits_{{\mathbf{x} \in \mathcal{X}}}\mathcal{L}\left( {\mathbf{x},\mathbf{\alpha }}\right) \\
> &= \mathop{\inf }\limits_{{\mathbf{x} \in \mathcal{X}}}\left( {f\left( \mathbf{x}\right) + \mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i}{g}_{i}\left( \mathbf{x}\right) }\right) . \tag{B.5}
> \end{align}
> $$

注意 $F$ 始终是凹的，因为拉格朗日函数关于 $\mathbf{\alpha }$ 是线性的，并且下确界保持凹性。我们进一步观察到
$$
\forall \mathbf{\alpha } \geq 0,\;F\left( \mathbf{\alpha }\right) \leq {p}^{ * } \tag{B.6}
$$

因为对于任意可行的 $$\mathbf{x}, f\left( \mathbf{x}\right) + \mathop{\sum }\limits_{{i = 1}}^{m}{\alpha }_{i}{g}_{i}\left( \mathbf{x}\right) \leq f\left( \mathbf{x}\right)$$
对偶函数自然引出了以下优化问题。

> [!definition] 定义 B.24 对偶问题
> 与约束优化问题相关的对偶(优化)问题是
$$
\mathop{\max }\limits_{\mathbf{\alpha }}F\left( \mathbf{\alpha }\right)
$$
subject to:
$$
\mathbf{\alpha } \geq 0\text{.}
$$

对偶问题总是一个凸优化问题(作为一个凹问题的最大化)。
令 ${d}^{ * }$ 表示一个最优值。
由 (B.6)，以下不等式总是成立:
$$
{d}^{ * } \leq {p}^{ * } \tag{weak duality.}
$$

差值 $\left( {{p}^{ * } - {d}^{ * }}\right)$ 被称为对偶间隙。等式情况
$$
{d}^{ * } = {p}^{ * } \tag{strong duality}
$$
通常不成立。
然而，在凸问题满足约束资格条件时，强对偶性确实成立。
我们将用 $\operatorname{int}\left( x\right)$ 表示集合 $x$ 的内部。

> [!definition] 定义 B.25 强约束资格
> 假设 $\mathrm{{int}}\left( X\right) \neq \varnothing$. 那么强约束资格或 Slater条件 定义为
> $$
> \exists \overline{\mathbf{x}} \in \operatorname{int}\left( \mathcal{X}\right) : g\left( \overline{\mathbf{x}}\right) < 0. \tag{B.7}
> $$
> 
> 如果一个函数 $h : x \rightarrow \mathbb{R}$ 对于所有 $\mathbf{x} \in x$ 可以由 $h\left( \mathbf{x}\right) = \mathbf{w} \cdot \mathbf{x} + b$ 定义，对于某些 $\mathbf{w} \in {\mathbb{R}}^{N}$ 和 $b \in \mathbb{R}$ ，则称其为仿射函数。

> [!definition] 定义 B.26 弱约束资格
> 假设 $\mathrm{{int}}\left( X\right) \neq \varnothing$. 那么弱约束资格或弱Slater条件定义为
> 
> $$
> \exists \overline{\mathbf{x}} \in \operatorname{int}\left( X\right) : \forall i \in \left\lbrack m\right\rbrack ,\left( {{g}_{i}\left( \overline{\mathbf{x}}\right) < 0}\right) \vee \left( {{g}_{i}\left( \overline{\mathbf{x}}\right) = 0 \land {g}_{i}\text{ affine }}\right) . \tag{B.8}
> $$

我们接下来基于拉格朗日的鞍点和Slater条件，为约束优化问题的解提供充分必要条件。

> [!theorem] 定理 B.27 鞍点 — 充分条件
> 取 $P$ 为 $\mathcal{X} = {\mathbb{R}}^{N}$ 上的约束优化问题。
> 如果 $\left( {{\mathbf{x}}^{ * },{\mathbf{\alpha }}^{ * }}\right)$ 是相关拉格朗日的鞍点，即，
> 
> $$
> \forall \mathbf{x} \in {\mathbb{R}}^{N},\forall \mathbf{\alpha } \geq 0,\;\mathcal{L}\left( {{\mathbf{x}}^{ * },\mathbf{\alpha }}\right) \leq \mathcal{L}\left( {{\mathbf{x}}^{ * },{\mathbf{\alpha }}^{ * }}\right) \leq \mathcal{L}\left( {\mathbf{x},{\mathbf{\alpha }}^{ * }}\right) \tag{B.9}
> $$
> 
> 那么 ${\mathbf{x}}^{ * }$ 是问题 $P$ 的解。

`\begin{proof}`
根据第一个不等式，以下成立:

$$
\forall \mathbf{\alpha } \geq 0,\mathcal{L}\left( {{\mathbf{x}}^{ * },\mathbf{\alpha }}\right) \leq \mathcal{L}\left( {{\mathbf{x}}^{ * },{\mathbf{\alpha }}^{ * }}\right) \Rightarrow \forall \mathbf{\alpha } \geq 0,\mathbf{\alpha } \cdot g\left( {\mathbf{x}}^{ * }\right) \leq {\mathbf{\alpha }}^{ * } \cdot g\left( {\mathbf{x}}^{ * }\right)
$$

$$
\Rightarrow g\left( {\mathbf{x}}^{ * }\right) \leq 0 \land {\mathbf{\alpha }}^{ * } \cdot g\left( {\mathbf{x}}^{ * }\right) = 0 \tag{B.10}
$$

其中 $g\left( {\mathbf{x}}^{ * }\right) \leq 0$ 在 (B.10) 中通过令 $\mathbf{\alpha } \rightarrow + \infty$ 得出，而 ${\mathbf{\alpha }}^{ * } \cdot g\left( {\mathbf{x}}^{ * }\right) = 0$ 通过令 $\mathbf{\alpha } \rightarrow 0$ 得出。鉴于 (B.10)，(B.9) 中的第二个不等式给出，

$$
\forall \mathbf{x},\mathcal{L}\left( {{\mathbf{x}}^{ * },{\mathbf{\alpha }}^{ * }}\right) \leq \mathcal{L}\left( {\mathbf{x},{\mathbf{\alpha }}^{ * }}\right) \Rightarrow \forall \mathbf{x}, f\left( {\mathbf{x}}^{ * }\right) \leq f\left( \mathbf{x}\right) + {\mathbf{\alpha }}^{ * } \cdot g\left( \mathbf{x}\right) .
$$

因此，对于所有满足约束的 $\mathbf{x}$ ，即 $g\left( \mathbf{x}\right) \leq 0$ ，我们有

$$
f\left( {\mathbf{x}}^{ * }\right) \leq f\left( \mathbf{x}\right)
$$

这完成了证明。
`\end{proof}`

> [!definition] 定理B.28 鞍点 — 必要条件
> 假设 $f$ 和 $g_i$, $i \in \left\lbrack m\right\rbrack$， 是凸函数且满足Slater条件。那么，如果 $\mathbf{x}$ 是约束优化问题的解，则存在 $\mathbf{\alpha } \geq 0$ 使得 $\left( {\mathbf{x},\mathbf{\alpha }}\right)$ 是拉格朗日函数的鞍点。

> [!definition] 定理B.29 鞍点 — 必要条件
> 假设 $f$ 和$g_{i}$, $i \in \left\lbrack m \right\rbrack$, 是凸可微函数且满足弱Slater条件。如果 $\mathbf{x}$ 是约束优化问题的解，那么存在 $\mathbf{\alpha } \geq 0$ 使得 $\left( {\mathbf{x},\mathbf{\alpha }}\right)$ 是拉格朗日函数的鞍点。

我们以一个定理作为结尾，该定理在问题是凸的、目标函数可微、约束条件合格的情况下，提供了必要且充分的优化性条件。

> [!theorem] 定理B.30(Karush-Kuhn-Tucker定理)
> 假设 $f$, ${g}_{i}$ :$X \rightarrow \mathbb{R},\forall i \in \left\lbrack m\right\rbrack$, 是凸的且可微，并且约束条件合格。那么 $\overline{\mathbf{x}}$ 是约束程序的解当且仅当存在 $\overline{\mathbf{\alpha }} \geq 0$ 使得，
> 
> $$
> {\nabla }_{\mathbf{x}}\mathcal{L}\left( {\overline{\mathbf{x}},\overline{\mathbf{\alpha }}}\right) = {\nabla }_{\mathbf{x}}f\left( \overline{\mathbf{x}}\right) + \overline{\mathbf{\alpha }} \cdot {\nabla }_{\mathbf{x}}g\left( \overline{\mathbf{x}}\right) = 0 \tag{B.11}
> $$
> 
> $$
> {\nabla }_{\mathbf{\alpha }}\mathcal{L}\left( {\overline{\mathbf{x}},\overline{\mathbf{\alpha }}}\right) = g\left( \overline{\mathbf{x}}\right) \leq 0 \tag{B.12}
> $$
> 
> $$
> \overline{\mathbf{\alpha }} \cdot g\left( \overline{\mathbf{x}}\right) = \mathop{\sum }\limits_{{i = 1}}^{m}{\overline{\mathbf{\alpha }}}_{i}{g}_{i}\left( \overline{\mathbf{x}}\right) = 0. \tag{B.13}
> $$
> 
> 条件B.11-B.13被称为KKT条件。
> 注意，最后两个KKT条件等价于
> 
> $$
> g\left( \overline{\mathbf{x}}\right) \leq 0 \land \left( {\forall i \in \{ 1,\ldots , m\} ,{\bar{\alpha }}_{i}{g}_{i}\left( \overline{\mathbf{x}}\right) = 0}\right) . \tag{B.14}
> $$
> 
> 这些等式被称为互补条件。

`\begin{proof}`
对于正向，由于约束条件合格，如果 $\overline{\mathbf{x}}$ 是解，那么存在 $\overline{\mathbf{\alpha }}$ 使得 $\left( {\overline{\mathbf{x}},\overline{\mathbf{\alpha }}}\right)$ 是拉格朗日函数的鞍点且三个条件均满足(第一个条件由鞍点的定义得出，后两个条件由(B.10)得出)。

在相反的方向，如果条件满足，那么对于任何 $\mathbf{x}$ 使得 $g\left( \mathbf{x}\right) \leq 0$ ，我们可以写出

$$
f\left( \mathbf{x}\right) - f\left( \overline{\mathbf{x}}\right) \geq {\nabla }_{\mathbf{x}}f\left( \overline{\mathbf{x}}\right) \cdot \left( {\mathbf{x} - \overline{\mathbf{x}}}\right) \;\left( {\text{convexity of}f}\right)
$$

$$
= - \mathop{\sum }\limits_{{i = 1}}^{m}{\bar{\alpha }}_{i}{\nabla }_{\mathbf{x}}{g}_{i}\left( \overline{\mathbf{x}}\right) \cdot \left( {\mathbf{x} - \overline{\mathbf{x}}}\right) \;\text{ (first condition) }
$$

$$
\geq - \mathop{\sum }\limits_{{i = 1}}^{m}{\overline{\mathbf{\alpha }}}_{i}\left\lbrack {{g}_{i}\left( \mathbf{x}\right) - {g}_{i}\left( \overline{\mathbf{x}}\right) }\right\rbrack
$$

(convexity of ${g}_{i}\mathrm{\;s}$ )

$$
= - \mathop{\sum }\limits_{{i = 1}}^{m}{\overline{\mathbf{\alpha }}}_{i}{g}_{i}\left( \mathbf{x}\right) \geq 0,\;\text{ (third condition) }
$$

这表明 $f\left( \overline{\mathbf{x}}\right)$ 是满足约束条件点集中 $f$ 的最小值。
`\end{proof}`