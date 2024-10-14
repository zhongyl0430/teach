## B.1 微分和无约束优化

我们从一些微分的基本定义开始，这些定义对于提出费马定理和描述凸函数的一些性质是必要的。

定义 B.1(梯度)设 $f : x \subseteq {\mathbb{R}}^{N} \rightarrow \mathbb{R}$ 是一个可微函数。那么，$f$ 在 $\mathbf{x} \in X$ 处的梯度是 ${\mathbb{R}}^{N}$ 中的向量，表示为 $\nabla f\left( \mathbf{x}\right)$，并定义为

$$
\nabla f\left( \mathbf{x}\right) = \left\lbrack \begin{matrix} \frac{\partial f}{\partial {\mathbf{x}}_{1}}\left( \mathbf{x}\right) \\ \vdots \\ \frac{\partial f}{\partial {\mathbf{x}}_{N}}\left( \mathbf{x}\right) \end{matrix}\right\rbrack
$$

定义 B.2(Hessian)设 $f : x \subseteq {\mathbb{R}}^{N} \rightarrow \mathbb{R}$ 是一个二阶可微函数。那么，$f$ 在 $\mathbf{x} \in X$ 处的Hessian矩阵是 ${\mathbb{R}}^{N \times N}$ 中的矩阵，表示为 ${\nabla }^{2}f\left( \mathbf{x}\right)$，并定义为

$$
{\nabla }^{2}f\left( \mathbf{x}\right) = {\left\lbrack \frac{{\partial }^{2}f}{\partial {\mathbf{x}}_{i},{\mathbf{x}}_{j}}\left( \mathbf{x}\right) \right\rbrack }_{1 \leq i, j \leq N}.
$$

接下来，我们介绍无约束优化的一个经典结果。

定理 B.3(费马定理)设 $f$ : $X \subseteq {\mathbb{R}}^{N} \rightarrow \mathbb{R}$ 是一个可微函数。如果 $f$ 在 ${\mathbf{x}}^{ * } \in X$ 处有一个局部极值，那么 $\nabla f\left( {\mathbf{x}}^{ * }\right) = 0$，即 ${\mathbf{x}}^{ * }$ 是一个驻点。