---
tags:
  - "#teach/ML"
---
- 学习者考虑一个固定的可能概念集 $\mathcal{H}$，称为**假设集 (hypothesis set)**，
	- 这个集不一定与 $\mathcal{C}$ 重合。
- 学习者接收到
	- 根据 $\mathcal{D}$ 独立同分布采样的样本 $S = \left( {{x}_{1},\ldots ,{x}_{m}}\right)$ 
	- 基于特定目标概念 $c \in \mathcal{C}$ 的标签 $\left( {c\left( {x}_{1}\right) ,\ldots, c\left( {x}_{m}\right) }\right)$。
- 任务是使用标记样本 $S$ 来选择一个假设 ${h}_{S} \in \mathcal{H}$，该假设相对于概念 $c$ 具有较小的 [[泛化误差 (generalization error)]]。