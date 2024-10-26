---
tags:
  - "#teach/ML"
---
假设的 [[泛化误差 (generalization error)]] 对学习者来说不是直接可访问的，因为分布 $\mathcal{D}$ 和目标概念 $c$ 都是未知的。然而，学习者可以在标记样本 $S$ 上测量假设的经验误差。

> [!definition] 经验误差
> 给定一个假设 $h \in \mathcal{H}$ ，一个目标概念 $c \in \mathcal{C}$ ，以及一个样本 $S = \left( {{x}_{1},\ldots ,{x}_{m}}\right)$ ，经验误差或 $h$ 的经验风险定义为
> $$
> {\widehat{R}}_{S}\left( h\right) = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{1}_{h\left( {x}_{i}\right) \neq c\left( {x}_{i}\right) }. \tag{2.2}
> $$

^def-empirical-error
