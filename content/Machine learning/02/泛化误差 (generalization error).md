---
tags:
  - "#teach/ML"
---
> [!definition] 泛化误差 (generalization error)
> 给定
> - 一个假设 $h \in \mathcal{H}$ ，
> - 一个目标概念 $c \in \mathcal{C}$ 
> - 一个潜在分布 $\mathcal{D}$ ，
> - 假设 $h$ 的 **泛化误差 / 风险** 定义为
> $$\begin{align*}
> R\left( h\right) 
> &= \underset{x \sim \mathcal{D}}{\mathbb{P}}\left\lbrack {h\left( x\right) \neq c\left( x\right) }\right\rbrack \\
> &= \underset{x \sim \mathcal{D}}{\mathbb{E}}\left\lbrack {1}_{h\left( x\right) \neq c\left( x\right) }\right\rbrack, \tag{2.1}
> \end{align*}$$
其中 ${1}_{\omega }$ 是事件 $\omega$ 的指示函数

^def-generalization-error

---
> [!remark]
> - 选择 $R$ 而不是 $E$ 来表示误差，可以避免与期望的表示法混淆，并且由于在机器学习和统计学中，风险 （risk）一词也用于指代误差，这一选择进一步得到了证实。 
> - 由于顾及其他相关定义，函数族 $\mathcal{H}$ 和目标概念 $c$ 必须是可测量的。本书中考虑的函数类都具有这一性质。