如果一个随机变量 $X$ 取值为 $0, 1, 2, \cdots, n$, 且
$$
P\left( {X = k}\right)  = \left( \begin{array}{l} n \\  k \end{array}\right) {p}^{k}{\left( 1 - p\right) }^{n - k}, \;k = 0, 1, 2, \cdots, n, \tag{2.2.3}
$$
我们称 $X$ 服从**二项分布**. 
记为 $X \sim  B\left( {n, p}\right)$ ( $\mathrm{R}$ 软件中的分布名为 binom), 其中的 $n$ 和 $p\left( {0 \leq  p \leq  1}\right)$ 称为参数. 

如果 $n = 1$, 则 $X$ 只取 0 和 1 两个值, 我们称 $X$ 服从**两点分布**. 当 $n = 1$ 时, 
- 如果 $p = 0$, 则 $P\left( {X = 0}\right)  = 1$; 
- 如果 $p = 1$, 则 $P\left( {X = 1}\right)  = 1$. 

这两种情况都退化为**单点分布** (即 $X$ 取某个常数 $C$ 的概率为 1 ), 取值已没有随机性了.