---
title: 第七章 参数估计
---
本章介绍经典的估计方法, 主要介绍总体参数的估计, 包括参数的点估计和区间估计. 点估计中将介绍矩法估计、最大似然估计和顺序统计量估计等方法可估计(可估计)可估计量优劣的基本标准. 区间估计主要介绍正态总体参数的区分间估计.

## 7.1 参数的点估计

简单地讲, 所谓参数的点估计, 就是找一个合适的统计量, 将样本观测值代人该统计量得到的值就作为该参数的估计, 而参数的区间估计则是找两个统计其中可以其中一个为左端点、另一个为右端点, 构成一个可能包含该参数的一个随

在不考虑估计量优劣时, 参数的点估计方法都是很直观的, 或者说其思想都是很基本的, 这一点请读者留意体会.

### 7.1.1 矩法估计

矩法估计的想法来自大数定律 (参见 5.1 节的定理 5.1.1 和定理 5.1.2). 如果总体 $X$ 存在 $k$ 阶矩,则由定理 5.1.1 知,对任 $\varepsilon  > 0$ 有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\left| {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{k} - E\left\lbrack  {X}^{k}\right\rbrack  }\right|  \geq  \varepsilon }\right)  = 0. \tag{7.1.1}
$$

这说明,当样本容量较大时,样本 $k$ 阶矩 $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{k}$ 与总体 $k$ 阶矩 $E\left\lbrack  {X}^{k}\right\rbrack$ 差别很

所谓矩法估计,就是用样本 $k$ 阶矩估计总体 $k$ 阶矩. (7.1.1) 说明这种估计方法是有理论依据的. 另外, 通常总体各阶矩都与总体参数有关, 从而可以通过用样本 $k$ 阶矩估计总体 $k$ 阶矩来实现对参数的估计.

设总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right)$,通常用 ${\widehat{\theta }}_{M}$ 来记 $\theta$ 的矩法估计量,它是样本 $\left( {{X}_{1},{X}_{2},\cdots }\right.$ $\left. {X}_{n}\right)$ 的一个函数,比如记为 ${\widehat{\theta }}_{M} = T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$,从而 ${\widehat{\theta }}_{M}$ 是一个随机变量行件不观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 代入估计量 ${\widehat{\theta }}_{M}$ 所得的数值 $T\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$,我们称为参数 $\theta$ 的矩法估计值.

下面我们通过几个例子, 进一步说明矩法估计.

例 7.1.1 试用参数的矩法估计, 估计一批某种产品的不合格品率.

解 由于一件产品要么为合格品要么为不合格品,所以此时总体 $X \sim  B\left( {1, p}\right)$, 抽到不合格品时 $X$ 取值为 1,否则取值为 0. 即不合格品率 $p = P\left( {X = 1}\right)$.

现设我们通过抽取,得到了样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$. 由于 $E\left\lbrack  X\right\rbrack   = p$,则由矩法估计的想法,就该用样本均值 $\bar{X}$ 来估计 $p$,亦即 ${\widehat{p}}_{M} = \bar{X}$. 也就是说,如果我们抽取了 100 件产品, 发现其中恰有 3 件不合格品, 则认为该批产品的不合格品率为 $3\%$.

例 7.1.2 长期的生产经验告诉我们, 水泥厂成品打包机装袋的重量服从正态分布, 试用矩法估计来估计一台打包机装袋的重量的均值和标准差.

解 设装袋的重量为 $X$,样本为 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$,由题设 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 和 $E\left\lbrack  X\right\rbrack   = \mu,\operatorname{Var}\left\lbrack  X\right\rbrack   = {\sigma }^{2}$,即

$$
\begin{cases} \mu &  = E\left\lbrack  X\right\rbrack , \\  {\sigma }^{2} &  = E\left\lbrack  {X}^{2}\right\rbrack   - {\left( E\left\lbrack  X\right\rbrack  \right) }^{2}. \end{cases}
$$

从而, 依矩法估计, 应有

$$
\begin{cases} {\widehat{\mu }}_{M} &  = \bar{X}, \\  {\widehat{{\sigma }^{2}}}_{M} &  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}^{2} - {\left( \bar{X}\right) }^{2}. \end{cases}
$$

由于 $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - {\left( \bar{X}\right) }^{2} = {S}_{n}^{2}$,所以

$$
\left\{  \begin{array}{l} {\widehat{\mu }}_{M} = \bar{X}, \\  {\widehat{\sigma }}_{M} = {S}_{n}. \end{array}\right.
$$

在例 7.1.2 中, 我们通过用样本 1,2 阶原点矩分别估计总体 1,2 阶原点矩, 得到的方差 ${\sigma }^{2}$ (总体 2 阶中心矩) 的估计量恰好也是样本 2 阶中心矩 ${S}_{n}^{2}$. 这一事实不是巧合而是必然的, 容易证明, 如果我们用样本各阶矩估计总体各阶矩, 则必然是用样本各阶中心矩估计总体各阶中心矩. 反之亦然.

例 7.1.3 设总体在某一区间上均匀取值, 试用矩法估计该区间的左、右端点.

解 由题意设 $X \sim  U\left\lbrack  {a, b}\right\rbrack$,则 $E\left\lbrack  X\right\rbrack   = \frac{a + b}{2},\operatorname{Var}\left\lbrack  X\right\rbrack   = \frac{{\left( b - a\right) }^{2}}{12}$,即

$$
\left\{  \begin{array}{l} a = E\left\lbrack  X\right\rbrack   - \sqrt{3\operatorname{Var}\left\lbrack  X\right\rbrack  }, \\  b = E\left\lbrack  X\right\rbrack   + \sqrt{3\operatorname{Var}\left\lbrack  X\right\rbrack  }. \end{array}\right.
$$

从而,依矩法估计,应有 (从此二元一次方程解出 $a$ 和 $b$,并用 $\bar{X}$ 代替 $E\left\lbrack  X\right\rbrack$,用 ${S}_{n}^{2}$ 代替 $\operatorname{Var}\left\lbrack  X\right\rbrack$,再用 ${\widehat{a}}_{M}$ 代替 $a$,用 ${\widehat{b}}_{M}$ 代替 $b$ )

$$
\left\{  \begin{array}{l} {\widehat{a}}_{M} = \bar{X} - \sqrt{3}{S}_{n}, \\  {\widehat{b}}_{M} = \bar{X} + \sqrt{3}{S}_{n}. \end{array}\right.
$$

例 7.1.4 设总体 $X$ 的分布密度函数为

$$
{f}_{X}\left( {x,\theta }\right)  = \frac{\theta }{2}{\mathrm{e}}^{-\theta \left| x\right| },\; - \infty  < x < \infty,\theta  > 0.
$$

试求 $\theta$ 的矩法估计.

解 先求 $E\left\lbrack  X\right\rbrack$,看看它与参数 $\theta$ 的关系. 由于

$$
E\left\lbrack  X\right\rbrack   = {\int }_{-\infty }^{\infty }x\frac{\theta }{2}{\mathrm{e}}^{-\theta \left| x\right| }\mathrm{d}x = 0
$$

与参数 $\theta$ 无关,我们想到试算 $E\left\lbrack  \left| X\right| \right\rbrack$. 由于

$$
E\left\lbrack  \left| X\right| \right\rbrack   = {\int }_{-\infty }^{\infty }\left| x\right| \frac{\theta }{2}{\mathrm{e}}^{-\theta \left| x\right| }\mathrm{d}x = {\int }_{0}^{\infty }{x\theta }{\mathrm{e}}^{-{\theta x}}\mathrm{\;d}x = \frac{1}{\theta },
$$

即 $\theta  = \frac{1}{E\left\lbrack  \left| X\right| \right\rbrack  }$,从而,依矩法估计,应有

$$
{\widehat{\theta }}_{M} = \frac{1}{\left| \bar{X}\right| } = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}\left| {X}_{i}\right| }.
$$

在例 7.1.4 中, 还可由

$$
E\left\lbrack  {X}^{2}\right\rbrack   = {\int }_{-\infty }^{\infty }{x}^{2}\frac{\theta }{2}{\mathrm{e}}^{-\theta \left| x\right| }\mathrm{d}x = {\int }_{0}^{\infty }{x}^{2}\theta {\mathrm{e}}^{-{\theta x}}\mathrm{\;d}x = \frac{2}{{\theta }^{2}}
$$

得到 $\theta$ 的另外一个矩法估计量为 $\sqrt{{2n}/\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}}$.

由以上的例子, 我们可以总结出如下矩法估计的一般步骤.

设总体 $X \sim  {F}_{X}\left( {\cdot,{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{l}}\right)$,先计算 $X$ 的从 1 到 $l$ 的各阶矩,得到各阶

矩与参数的关系

$$
\begin{cases} E\left\lbrack  X\right\rbrack   = & {g}_{1}\left( {{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{l}}\right), \\  E\left\lbrack  {X}^{2}\right\rbrack   = & {g}_{2}\left( {{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{l}}\right), \\   & \cdots \cdots \\  E\left\lbrack  {X}^{l}\right\rbrack   = & {g}_{l}\left( {{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{l}}\right). \end{cases} \tag{7.1.2}
$$

由这些关系式中解出

$$
\left\{  \begin{matrix} {\theta }_{1} = {h}_{1}\left( {E\left\lbrack  X\right\rbrack , E\left\lbrack  {X}^{2}\right\rbrack ,\cdots, E\left\lbrack  {X}^{l}\right\rbrack  }\right), \\  {\theta }_{2} = {h}_{2}\left( {E\left\lbrack  X\right\rbrack , E\left\lbrack  {X}^{2}\right\rbrack ,\cdots, E\left\lbrack  {X}^{l}\right\rbrack  }\right), \\  \cdots \cdots \\  {\theta }_{l} = {h}_{l}\left( {E\left\lbrack  X\right\rbrack , E\left\lbrack  {X}^{2}\right\rbrack ,\cdots, E\left\lbrack  {X}^{l}\right\rbrack  }\right). \end{matrix}\right.  \tag{7.1.3}
$$

最后, 将 (7.1.3) 右端函数中的总体各阶原点矩用样本各阶原点矩代替, 再将 ${\theta }_{1},{\theta }_{2},\cdots,{\theta }_{l}$ 换成 ${\widehat{{\theta }_{1}}}_{M},{\widehat{{\theta }_{2}}}_{M},\cdots,{\widehat{{\theta }_{l}}}_{M}$ 即得.

### 7.1.2 最大似然估计

参数的最大似然估计的想法基于大家普遍接受的一个事实, 这个事实为 “小概率事件在一次试验中几乎不可能发生”. 换言之, 在一次试验中发生的事件, 其发生的概率应该比较大. 所以,若总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right)$,当我们有了一组样本观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 时, $\theta$ 的取值应该使得样本观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 出现的可能性较大. 为确定出 $\theta$ 的具体估计量,我们要求 $\theta$ 的取值应该使得样本观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 出现的可能性达到最大.

我们以总体 $X$ 为连续型随机变量的情形来解释如何得到参数的最大似然估计.

设 $X$ 的分布密度函数为 ${f}_{X}\left( {\cdot,\theta }\right)$,大家知道,若 ${f}_{X}\left( {x,\theta }\right)$ 在 $x = {x}_{0}$ 处取值较大,则 $X$ 取值为 ${x}_{0}$ 附近的概率也较大. 于是我们要求 $\theta$ 的取值使得 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的联合密度函数在样本观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 处取到最大. 记 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的联合密度函数为 $L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)$,则由命题 6.1.1 知,

$$
L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}{f}_{X}\left( {{x}_{i},\theta }\right). \tag{7.1.4}
$$

我们称 $L$ 为 $X$ 的似然函数.

至此,我们将求参数 $\theta$ 的最大似然估计的问题,归结为在已有样本观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 前提下,寻求 $L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)$ 的最大值点 $\theta$ 的问题. 记该最大值点为 $\theta  = T\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$,则 $\theta$ 的最大似然估计量就为

$$
{\widehat{\theta }}_{L} = T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right). \tag{7.1.5}
$$

为了求得 $L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)$ 的最大值点,往往通过求它的驻点. 即关于 $\theta$ 的导数为 0 的点,但 (7.1.4) 为 $n$ 个函数的乘积,求导比较繁琐. 通常可利用对数函数 $\ln$ 的单调性,将问题转化为求 $\ln \left( {L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right) }\right)$ 的最大值点.

例 7.1.5 据经验, 进入稳态期的生产线生产出的液晶电视机的使用寿命服从指数分布, 试用最大似然估计方法估计该厂生产线生产出的液晶电视机的平均寿命.

解 由题意设 $X \sim  \operatorname{Exp}\left( \lambda \right)$,样本观测值为 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$,当 ${x}_{i} > 0(i =$ $1,2,\cdots, n)$ 时, $X$ 的似然函数为

$$
L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\lambda }\right)  = \lambda {\mathrm{e}}^{-\lambda {x}_{1}}\lambda {\mathrm{e}}^{-\lambda {x}_{2}}\cdots \lambda {\mathrm{e}}^{-\lambda {x}_{n}} = {\lambda }^{n}{\mathrm{e}}^{-\lambda \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}.
$$

从而

$$
\ln \left( {L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\lambda }\right) }\right)  = n\ln \left( \lambda \right)  - \lambda \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}.
$$

上式两边关于 $\lambda$ 求导数,并令其为 0 得

$$
\frac{\partial \ln L}{\partial \lambda } = \frac{n}{\lambda } - \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} = 0
$$

即

$$
\lambda  = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}},
$$

最终得 $\lambda$ 的最大似然估计量为

$$
{\widehat{\lambda }}_{L} = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}} = \frac{1}{\bar{X}}.
$$

也就是, 该厂生产线生产出的液晶电视机的平均寿命的最大似然估计量为 $1/X$.

例 7.1.6 据多年观测记录的经验, 每年广州出现暴雨天气的天数服从泊松分布, 试用最大似然法估计广州每年出现暴雨天气的平均天数.

解 由题意设 $X \sim  \operatorname{Pois}\left( \lambda \right)$,样本观测值为 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$,则 $X$ 的似然函数为

$$
L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\lambda }\right)  = \frac{{\lambda }^{{x}_{1}}{\mathrm{e}}^{-\lambda }}{{x}_{1}!}\frac{{\lambda }^{{x}_{2}}{\mathrm{e}}^{-\lambda }}{{x}_{2}!}\cdots \frac{{\lambda }^{{x}_{n}}{\mathrm{e}}^{-\lambda }}{{x}_{n}!} = \frac{{\mathrm{e}}^{-{n\lambda }}{\lambda }^{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}}{{x}_{1}!{x}_{2}!\cdots {x}_{n}!}.
$$

从而,

$$
\ln \left( {L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\lambda }\right) }\right)  =  - {n\lambda } + \ln \left( \lambda \right)  \cdot  \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} - \ln \left( {\mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}!}\right).
$$

上式两边关于 $\lambda$ 求导数,并令其为 0 得

$$
\frac{\partial \ln L}{\partial \lambda } =  - n + \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}{\lambda } = 0,
$$

即

$$
\lambda  = \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}{n}
$$

最终得 $\theta$ 的最大似然估计量为

$$
{\widehat{\lambda }}_{L} = \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}{n} = \bar{X}.
$$

也就是,广州每年出现暴雨天气的平均天数的最大似然估计量为 $\bar{X}$.

例 7.1.7 据产品检验部门的经验, 某便携式电脑的液晶显示屏出现的亮点或黑点, 在从屏幕左侧开始的每个水平线的一段上均匀出现, 试用最大似然法和矩法分别估计该水平线段的最右端点的值.

解 由题意设 $X \sim  U\left\lbrack  {0,\theta }\right\rbrack$,样本观测值为 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$,则 $X$ 的似然函

数为

$$
L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)  = \left\{  \begin{array}{ll} \frac{1}{{\theta }^{n}}, & {x}_{1},{x}_{2},\cdots,{x}_{n} \in  \left( {0,\theta }\right), \\  0, & \text{ 其他. } \end{array}\right.
$$

显然,为要 $L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)$ 取到最大值,就应当是在包含所有的 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 的区间 $\left( {0,\theta }\right)$ 中找一个最短的,所以应有

$$
\theta  = \max \left\{  {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right\}
$$

最终得 $\theta$ 的最大似然估计量为

$$
{\widehat{\theta }}_{L} = \max \left\{  {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right\}   = {X}_{\left( n\right) }.
$$

也就是,该水平线段的最右端点的值的最大似然估计量为顺序统计量 ${X}_{\left( n\right) }$.

另外, 由于

$$
E\left\lbrack  X\right\rbrack   = \frac{\theta }{2}
$$

即

$$
\theta  = {2E}\left\lbrack  X\right\rbrack
$$

从而得 $\theta$ 的矩法估计量为

$$
{\widehat{\theta }}_{M} = 2\bar{X}
$$

也就是,该水平线段的最右端点的值的矩法估计量为 $2\bar{X}$.

### 7.1.3 顺序统计量估计

利用顺序统计量作参数估计,其想法是若对总体 $X$ 作 $n$ 次观测 (即抽取容量为 $n$ 的样本),则 $X$ 的中位数应近乎在这 $n$ 个观测值的中间位置,并且这 $n$ 个观测值越集中,则 $X$ 的方差应越小.

由于总体为连续型随机变量且分布密度对称时, 总体中位数就是均值. 此时可用样本中位数来估计总体均值, 并用样本极差来估计总体标准差, 即

$$
\left\{  \begin{matrix} \widehat{E}\left\lbrack  X\right\rbrack   = \widetilde{X}, \\  \sqrt{\operatorname{Var}\left\lbrack  X\right\rbrack  } = {R}_{n}^{X}, \end{matrix}\right.
$$

其中 $\widehat{x}$ 表示 $x$ 的估计量,样本中位数 $\widetilde{X}$ 和样本极差 ${R}_{n}^{X}$ 的定义参见 6.1 节.

由于对于一般总体,样本中位数 $\widetilde{X}$ 极差 ${R}_{n}^{X}$ 的精确分布难以得到,从而难以把握其估计的偏差, 用这种方法估计均值和标准差, 只是对总体均值和标准差的一个大概了解, 所以一般少用这种方法.

## 7.2 估计量优劣性的评价

我们知道, 数理统计就是用局部数据推断总体, 推断的结论总会存在偏差. 参数的点估计就是基于某种想法,构造样本的函数 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 来实现对未知参数 $\theta$ 的估计,从而由不同的样本观测值得到的参数估计值总是与实际参数值有偏差, 这一点是无法避免的.

然而, 对于总体的同一个参数, 不同的估计方法也许偏差有所不同, 我们希望找一个比较偏差大小的标准. 最直观和基本的标准是,尽管 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 有时大于 $\theta$,有时小于 $\theta$,但平均下来,应与 $\theta$ 无差别. 这就是估计量的无偏性.

定义 7.2.1 设总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right),\theta  \in  \Theta, g$ 为 $\theta$ 的函数, $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为一统计量. 如果

$$
{E}_{\theta }\left\lbrack  {T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right) }\right\rbrack   = g\left( \theta \right), \tag{7.2.1}
$$

则称 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为 $g\left( \theta \right)$ 的无偏估计量. 如果

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}{E}_{\theta }\left\lbrack  {T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right) }\right\rbrack   = g\left( \theta \right), \tag{7.2.2}
$$

则称 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为 $g\left( \theta \right)$ 的渐近无偏估计量.

定义 7.2.1 中的 ${E}_{\theta }$ 表示在总体的参数真为 $\theta$ 时所确定的概率分布下求数学期望,而 $g\left( \theta \right)$ 则是待估计参数一般表示,即我们不仅求 $\theta$ 本身的估计,还可能估计 $\theta$ 的某个函数.

例 7.2.1 (例 7.1.7 续) 设总体 $X \sim  U\left\lbrack  {0,\theta }\right\rbrack$. 在例 7.1.7 中我们得到, ${\widehat{\theta }}_{M} =$ $2\bar{X},{\widehat{\theta }}_{L} = {X}_{\left( n\right) }$. 试问这两个估计量是否为无偏估计量.

解 由于

$$
{E}_{\theta }\left\lbrack  {\widehat{\theta }}_{M}\right\rbrack   = {E}_{\theta }\left\lbrack  {2\bar{X}}\right\rbrack   = \frac{2}{n}\left\{  {{E}_{\theta }\left\lbrack  {X}_{1}\right\rbrack   + {E}_{\theta }\left\lbrack  {X}_{2}\right\rbrack   + \cdots  + {E}_{\theta }\left\lbrack  {X}_{n}\right\rbrack  }\right\}   = \frac{2}{n} \cdot  n \cdot  \frac{\theta }{2} = \theta,
$$

所以, ${\widehat{\theta }}_{M} = 2\bar{X}$ 是 $\theta$ 的无偏估计量.

为计算 ${E}_{\theta }\left\lbrack  {\widehat{\theta }}_{L}\right\rbrack$,我们先求 ${X}_{\left( n\right) }$ 的分布密度函数. 由于

$$
{F}_{X}\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0, \\  \frac{x}{\theta }, & 0 \leq  x < \theta, \\  1, & x \geq  \theta, \end{array}\right.
$$

所以, 利用 (6.3.19) 有

$$
{f}_{{X}_{\left( n\right) }}\left( x\right)  = \left\{  \begin{array}{lll} n{\left( \frac{x}{\theta }\right) }^{n - 1} & \frac{1}{\theta }, & 0 \leq  x < \theta, \\  0, & & \text{ 其他. } \end{array}\right.
$$

从而

$$
{E}_{\theta }\left\lbrack  {\widehat{\theta }}_{L}\right\rbrack   = {E}_{\theta }\left\lbrack  {X}_{\left( n\right) }\right\rbrack   = {\int }_{0}^{\theta }{xn}\frac{{x}^{n - 1}}{{\theta }^{n}}\mathrm{\;d}x = \frac{n}{{\theta }^{n}}\frac{{\theta }^{n + 1}}{n + 1} = \frac{n}{n + 1}\theta,
$$

所以 ${\widehat{\theta }}_{L} = {X}_{\left( n\right) }$ 不是 $\theta$ 的无偏估计量,只是 $\theta$ 的渐近无偏估计量.

在例 7.2.1 中,虽然 ${\widehat{\theta }}_{L} = {X}_{\left( n\right) }$ 不是 $\theta$ 的无偏估计量,但是令 $\widehat{\theta } = \frac{n + 1}{n}{\widehat{\theta }}_{L}$,

则有

$$
{E}_{\theta }\left\lbrack  \widehat{\theta }\right\rbrack   = {E}_{\theta }\left\lbrack  {\frac{n + 1}{n}{\widehat{\theta }}_{L}}\right\rbrack   = \frac{n + 1}{n}{E}_{\theta }\left\lbrack  {X}_{\left( n\right) }\right\rbrack   = \frac{n + 1}{n}\frac{n}{n + 1}\theta  = \theta,
$$

即 $\widehat{\theta } = \frac{n + 1}{m}{\widehat{\theta }}_{L}$ 是 $\theta$ 的无偏估计量.

至此,对例 7.1.7 中的总体,我们得到两个无偏估计量 ${\widehat{\theta }}_{M} = 2\bar{X}$ 和 $\widehat{\theta } =$ $\frac{n + 1}{n}{X}_{\left( n\right) }$. 一个自然的问题是哪一个比较 “好” 呢? 对这两个均值都为 $\theta$ 的随机变量, 自然地我们认为, 方差较小的应当是比较 “好” 的.

下面我们来计算它们的方差.

$$
{\operatorname{Var}}_{\theta }\left\lbrack  {\widehat{\theta }}_{M}\right\rbrack   = {\operatorname{Var}}_{\theta }\left\lbrack  {2\bar{X}}\right\rbrack   = \frac{{2}^{2}}{{n}^{2}}\left\{  {{\operatorname{Var}}_{\theta }\left\lbrack  {X}_{1}\right\rbrack   + {\operatorname{Var}}_{\theta }\left\lbrack  {X}_{2}\right\rbrack   + \cdots  + {\operatorname{Var}}_{\theta }\left\lbrack  {X}_{n}\right\rbrack  }\right\}   = \frac{4}{{n}^{2}} \cdot  n \cdot  \frac{{\theta }^{2}}{12} = \frac{{\theta }^{2}}{3n}.
$$

120 而

$$
{\operatorname{Var}}_{\theta }\left\lbrack  \widehat{\theta }\right\rbrack   = \frac{{\left( n + 1\right) }^{2}}{{n}^{2}}{\operatorname{Var}}_{\theta }\left\lbrack  {X}_{\left( n\right) }\right\rbrack
$$

$$
= \frac{{\left( n + 1\right) }^{2}}{{n}^{2}}\left\{  {{E}_{\theta }\left\lbrack  {X}_{\left( n\right) }^{2}\right\rbrack   - {\left( {E}_{\theta }\left\lbrack  {X}_{\left( n\right) }\right\rbrack  \right) }^{2}}\right\}
$$

$$
= \frac{{\left( n + 1\right) }^{2}}{{n}^{2}}\left\{  {{\int }_{0}^{\theta }{x}^{2}n\frac{{x}^{n - 1}}{{\theta }^{n}}\mathrm{\;d}x - \frac{{n}^{2}}{{\left( n + 1\right) }^{2}}{\theta }^{2}}\right\}
$$

$$
= \frac{{\left( n + 1\right) }^{2}}{{n}^{2}}\left\{  {\frac{n}{n + 2}{\theta }^{2} - \frac{{n}^{2}}{{\left( n + 1\right) }^{2}}{\theta }^{2}}\right\}
$$

$$
= \frac{{\theta }^{2}}{n\left( {n + 2}\right) }.
$$

可见,只要 $n > 1$,就有

$$
{\operatorname{Var}}_{\theta }\left\lbrack  \widehat{\theta }\right\rbrack   < {\operatorname{Var}}_{\theta }\left\lbrack  {\widehat{\theta }}_{M}\right\rbrack
$$

亦即,我们认为 $\widehat{\theta } = \frac{n + 1}{n}{X}_{\left( n\right) }$ 比 ${\widehat{\theta }}_{M} = 2\bar{X}$ 要 “好”.

如果 ${T}_{1}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 和 ${T}_{2}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 都是待估计参数 $g\left( \theta \right)$ 的无偏估计,但 ${\operatorname{Var}}_{\theta }\left\lbrack  {T}_{1}\right\rbrack   \leq  {\operatorname{Var}}_{\theta }\left\lbrack  {T}_{2}\right\rbrack$,我们称 ${T}_{1}$ 比 ${T}_{2}$ 有效. 一个自然的问题是. 对于待估计参数 $g\left( \theta \right)$,能否找到最有效的估计量呢? 这个问题引出如下的定义 7.2.2.

定义 7.2.2 设总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right),\theta  \in  \Theta$. 若 ${T}_{0}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为 $g\left( \theta \right)$ 的无偏估计量,且对 $g\left( \theta \right)$ 的任意无偏估计量 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 都有

$$
{\operatorname{Var}}_{\theta }\left\lbrack  {T}_{0}\right\rbrack   \leq  {\operatorname{Var}}_{\theta }\left\lbrack  T\right\rbrack ,\;\forall \theta  \in  \Theta.
$$

则称 ${T}_{0}$ 为 $g\left( \theta \right)$ 的一致最小方差无偏估计量 (记为 UMVUE,它是 Uniformlv Minimum Variance Unbiased Estimate 的缩写).

可惜的是,对于一般的总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right) \left( {\theta  \in  \Theta }\right)$,目前还没有一个寻找 $g\left( \theta \right)$ 的一致最小方差无偏估计量的普遍可行的、构造性的方法. 已有的研究结果中只是对于一些特殊的总体类型有比较深刻或较为一般的结论或方法. 比如克拉默 - 拉奥 (Cramér-Rao) 定理, 就是对满足某种性质的总体分布类型, 事先得到参数 $g\left( \theta \right)$ 的无偏估计量方差的下界,如果找到的无偏估计量 ${T}_{0}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的万差已达到该下界,那么 ${T}_{0}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 就是 $g\left( \theta \right)$ 的最有效估计量了. 再比如, 对于总体的分布为指数分布族, 通过寻找充分完备统计量, 可以达到寻找一致最小方差无偏估计量的目的. 我们熟悉的分布 $\operatorname{Exp}\left( \lambda \right),\operatorname{Pois}\left( \lambda \right), B\left( {n, p}\right)$ 和 $N\left( {\mu,{\sigma }^{2}}\right)$ 等都属指数分布族,其参数的最大似然估计量 (对这些分布,矩法估计量与最大似然估计量相同), 都是一致最小方差无偏估计量.

另外, 需要指出的是, 虽然无偏性是对估计量的直观合理的要求. 但是下面的例 7.2.2 表明, 在有些情况下, 一个无偏估计量也许是具有 “很大偏差” 的.

例 7.2.2 设总体 $X \sim  \operatorname{Pois}\left( \lambda \right)$,参数 $\lambda  > 0,\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本,则 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)  = {\left( -2\right) }^{{X}_{1}}$ 是 ${\mathrm{e}}^{-{3\lambda }}$ 的无偏估计量.

事实上,

$$
E\left\lbrack  {T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right) }\right\rbrack
$$

$$
= E\left\lbrack  {\left( -2\right) }^{{X}_{1}}\right\rbrack   = \mathop{\sum }\limits_{{n = 0}}^{\infty }{\left( -2\right) }^{n}\frac{{\mathrm{e}}^{-\lambda }{\lambda }^{n}}{n!}
$$

$$
= {\mathrm{e}}^{-\lambda }\mathop{\sum }\limits_{{n = 0}}^{\infty }\frac{{\left( -2\lambda \right) }^{n}}{n!} = {\mathrm{e}}^{-\lambda }{\mathrm{e}}^{-{2\lambda }}
$$

$$
= {\mathrm{e}}^{-{3\lambda }}\text{.}
$$

注意到 ${\mathrm{e}}^{-{3\lambda }} > 0$,但 ${\left( -2\right) }^{{X}_{1}}$ 却在 ${X}_{1}$ 为奇数时取负值,可见偏差之大.

另外一种评价估计量的想法是当样本容量较大时, 考查估计量与待估计参数的差距, 也就是统计量的相合性.

定义 7.2.3 设总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right),\theta  \in  \Theta$. 并设 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为 $g\left( \theta \right)$ 的估计量,如果对任意 $\varepsilon  > 0$ 有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\left| {T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)  - g\left( \theta \right) }\right|  \geq  \varepsilon }\right)  = 0,\;\forall \theta  \in  \Theta. \tag{7.2.3}
$$

则称 $T\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为 $g\left( \theta \right)$ 的相合估计量.

显然,若总体 $X$ 存在 $k$ 阶矩,则由大数定律 (参见 5.1 节的定理 5.1.1) 和相合性的定义知,样本 $k$ 阶原点矩 $\overline{{X}^{k}} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}^{k}$ 是总体 $k$ 阶原点矩 $E\left\lbrack  {X}^{k}\right\rbrack$ 的相合估计量, 进而大多矩法估计量都是相合估计量.

## 7.3 参数的区间估计

与参数的点估计不同,区间估计是以两个统计量 ${T}_{1}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 和 ${T}_{2}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为左右端点构成一个随机区间,并且要求该随机区间包含待估计参数的概率满足一定的要求.

定义 7.3.1 设总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right),\theta  \in  \Theta, g$ 为 $\theta$ 的函数. 若有统计量 ${T}_{1}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 和 ${T}_{2}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 使得对给定的 $\alpha \left( {0 < \alpha  < 1}\right)$ 有

$$
P\left( {{T}_{1}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)  \leq  g\left( \theta \right)  \leq  {T}_{2}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right) }\right)  = 1 - \alpha, \tag{7.3.1}
$$

则称 $\left\lbrack  {{T}_{1}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right),{T}_{2}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right) }\right\rbrack$ 为 $g\left( \theta \right)$ 的置信度为 $1 - \alpha$ 的区间估计 (或估计区间, 置信区间).

由于代入一次具体的抽样得到的样本观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 计算出的区间

$$
\left\lbrack  {{T}_{1}\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right),{T}_{2}\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right) }\right\rbrack
$$

是一个确定的区间,它要么包含 $g\left( \theta \right)$,要么不包含 $g\left( \theta \right)$,不能说它包含 $g\left( \theta \right)$ 的概举为 $1 - \alpha$. 但在寻求统计量 ${T}_{1}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 和 ${T}_{2}\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 时 $\nabla$ 与 $\alpha$ 的大小有关,所以我们把 $1 - \alpha$ 称为的区间估计的置信度.

相联系和比较. 另外,(7.3.1) 右端写为 $1 - \alpha$ 是便于与第八章介绍的假设检验的相应表达式

本节给出的例子都是简单套用公式的示例,都可以用 $\mathrm{R}$ 软件轻松求解. 有关用 $\mathrm{R}$ 软件实现的实例请读者参见第九章.

### 7.3.1 单个正态总体参数的区间估计

以关于正态总体的抽样基本定理及其推论 (见 6.3 节) 作基础, 可求出该总体有关统计量或样本函数的精确分布, 从而使得正态总体参数的区间估计很容勿待到.

#### 1. $\mu$ 的区间估计 $\left( {{\sigma }^{2} = {\sigma }_{0}^{2}}\right.$ 已知 $)$

设总体 $X \sim  N\left( {\mu,{\sigma }_{0}^{2}}\right)$,参数 $\mu$ 未知, ${\sigma }_{0}^{2}$ 已知. $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本 我们来寻求 $\mu$ 的置信度为 $1 - \alpha$ 的区间估计.

由推论 6.3.1 知, $\bar{X} \sim  N\left( {\mu,\frac{{\sigma }_{0}^{2}}{n}}\right)$,从而

$$
U = \frac{\bar{X} - \mu }{\sqrt{\frac{{\sigma }_{0}^{2}}{n}}} \sim  N\left( {0,1}\right). \tag{7.3.2}
$$

由

$$
P\left( {\left| U\right|  \leq  {u}_{1 - \frac{\alpha }{2}}}\right)  = 1 - \alpha, \tag{7.3.3}
$$

查标准正态分布表 (或用 $\mathrm{R}$ 软件的 $\mathfrak{q}$ norm $\left( {1 - \frac{\alpha }{2}}\right)$,得 ${u}_{1 - \frac{\alpha }{2}}$ (例如 ${u}_{0.975} = {1.96}$ ),

亦即

$$
P\left( {\left| \frac{\bar{X} - \mu }{\sqrt{\frac{{\sigma }_{0}^{2}}{n}}}\right|  \leq  {u}_{1 - \frac{\alpha }{2}}}\right)  = 1 - \alpha  \tag{7.3.4}
$$

$$
P\left( {\bar{X} - {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{0}^{2}}{n}} \leq  \mu  \leq  \bar{X} + {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{0}^{2}}{n}}}\right)  = 1 - \alpha.
$$

至此,我们得到 $\mu$ 的置信度为 $1 - \alpha$ 的区间估计为

$$
\left\lbrack  {\bar{X} - {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{0}^{2}}{n}},\;\bar{X} + {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{0}^{2}}{n}}}\right\rbrack . \tag{7.3.5}
$$

总结一下,我们是如何得到 $\mu$ 的区间估计的. 首先我们得到了 (7.3.2),即得到了仅含待估计参数、不含其他未知参数的一个样本函数, 并且求得了它的分布. 其次是利用 (7.3.3) 经查表 (或计算) 得到分位点 ${u}_{1 - \frac{\alpha }{2}}$. 最后利用 (7.3.4) 作等式变形, 得到所要区间左右端点.

例 7.3.1 已知某厂生产的滚珠直径 $X \sim  N\left( {\mu,{0.06}}\right)$. 从某天生产的滚珠中随机地抽取 6 只, 测得直径为 (单位: mm)

$\begin{array}{llllll} {14.6} & {15.1} & {14.9} & {14.8} & {15.2} & {15.1} \end{array}$

试求 $\mu$ 的置信度为 0.95 的区间估计.

解 由于

$$
\bar{x} = \frac{1}{6}\left( {{14.6} + {15.1} + {14.9} + {14.8} + {15.2} + {15.1}}\right)  = {14.95},
$$

$\sigma  = \sqrt{0.06},\alpha  = {0.05}$,查表或用 $\mathrm{R}$ 软件计算得 ${u}_{0.975} = {1.96}$,用 (7.3.5) 得到 $\mu$ 的置信度为 0.95 的区间估计 [14.754, 15.146].

另外,请读者执行如下 $\mathrm{R}$ 程序,看有什么结果.

---

x<-c(14.6,15.1,14.9,14.8,15.2,15.1)

sigma<-sqrt(0.06)

	alpha<-0.05

			$\mathrm{z}1 <  - \mathrm{{mean}}\left( \mathrm{x}\right)$

			z2<-qnorm(1-alpha/2)*sigma/sqrt(length(x))

			list(c.i=c(z1-z2, z1+z2))

---

#### 2. $\mu$ 的区间估计 $\left( {\sigma }^{2}\right.$ 未知)

此时,欲模仿 (7.3.2) 寻求待估计参数 $\mu$ 的样本函数,但现在 ${\sigma }^{2}$ 未知,(7.3.2) 的样本函数中有未知参数,将来得不到 $\mu$ 的区间估计,于是想到用 ${\sigma }^{2}$ 的点估计量 ${S}_{n}^{2}$ 代替 ${\sigma }^{2}$,而此时的分布不再是 $N\left( {0,1}\right)$ 了,好在我们有推论 6.3.2,它告诉

我们

$$
\frac{\bar{X} - \mu }{{S}_{n}}\sqrt{n - 1} \sim  t\left( {n - 1}\right)
$$

对于给定的置信度 $1 - \alpha$,由

$$
P\left( {\left| {\frac{\bar{X} - \mu }{{S}_{n}}\sqrt{n - 1}}\right|  \leq  {t}_{1 - \frac{\alpha }{2}}\left( {n - 1}\right) }\right)  = 1 - \alpha,
$$

查表或用 $\mathrm{R}$ 软件计算得 ${t}_{1 - \frac{\alpha }{2}}\left( {n - 1}\right)$,进而经等式变形得到 $\mu$ 的区间估计

$$
\left\lbrack  {\bar{X} - {t}_{1 - \frac{\alpha }{2}}\left( {n - 1}\right) \frac{{S}_{n}}{\sqrt{n - 1}},\bar{X} + {t}_{1 - \frac{\alpha }{2}}\left( {n - 1}\right) \frac{{S}_{n}}{\sqrt{n - 1}}}\right\rbrack . \tag{7.3.6}
$$

由以上推导方法大家看到, 最关键的是要找到一个仅含待估计参数. 不含其他未知参数的样本函数, 并且求得它的分布. 而寻求这样的样本函数的思路很简甲, 就是考虑未知参数的点估计量. 于是对于一个正态总体、两个独立正态总体的有关参数的区间估计,依据 6.3 节的定理 6.3.1 及推论 6.3.1 或 10 。推论 6.3.4 就可知有关样本函数及其分布. 至于接下来要做的求分位点和等式变形就是初等运算 J.

例 7.3.2 在例 7.3.1 中若 ${\sigma }^{2}$ 未知,试求 $\mu$ 的置信度为 0.95 的区间估计.

解 由 $\bar{x} = {14.95}$ 和

$$
{s}_{n}^{2} = \frac{1}{6}\left\lbrack  {{\left( {14.6} - {14.95}\right) }^{2} + {\left( {15.1} - {14.95}\right) }^{2} + {\left( {14.9} - {14.95}\right) }^{2} + {\left( {14.8} - {14.95}\right) }^{2} + }\right.
$$

$$
\left. {{\left( {15.2} - {14.95}\right) }^{2} + {\left( {15.1} - {14.95}\right) }^{2}}\right\rbrack   = {0.206}^{2}.
$$

$\alpha  = {0.05}$,查表或用 $\mathrm{R}$ 软件计算的 ${t}_{0.975}\left( 5\right)  = {2.570582}$,用 (7.3.6) 得到 $\mu$ 的置信度为 0.95 的置信区间 [14.713, 15.187].

另外,请读者执行如下两个 $\mathrm{R}$ 程序,看有什么结果.

---

						x<-c(14.6,15.1,14.9,14.8,15.2,15.1)

						sigma<-sd(x)

						alpha<-0.05

				$n <  - {length}\left( x\right)$

			$\mathrm{z}1 <  - \mathrm{{mean}}\left( \mathrm{x}\right)$

		z2<-qt(1-alpha/2, n-1)*sigma/sqrt(n)

list(c.i=c(z1-z2, z1+z2))

---

或者

x<-c(14.6,15.1,14.9,14.8,15.2,15.1)

t.test(x,, ) \$conf

#### 3. ${\sigma }^{2}$ 的区间估计 $\left( {\mu  = {\mu }_{0}}\right.$ 已知 $)$

此时由 $X \sim  N\left( {{\mu }_{0},{\sigma }^{2}}\right)$ 知,

$$
\frac{{X}_{i} - {\mu }_{0}}{\sigma } \sim  N\left( {0,1}\right),\;i = 1,2,\cdots, n,
$$

所以

$$
\mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {X}_{i} - {\mu }_{0}\right) }^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( n\right)
$$

再令

$$
P\left( {{\chi }_{\frac{\alpha }{2}}^{2}\left( n\right)  \leq  \mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {X}_{i} - {\mu }_{0}\right) }^{2}}{{\sigma }^{2}} \leq  {\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right) }\right)  = 1 - \alpha,
$$

求出分位点 ${\chi }_{\frac{\alpha }{2}}^{2}\left( n\right)$ 和 ${\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right)$ 并作等式变形立得 ${\sigma }^{2}$ 的区间估计为

$$
\left\lbrack  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - {\mu }_{0}\right) }^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right) },\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - {\mu }_{0}\right) }^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( n\right) }}\right\rbrack . \tag{7.3.7}
$$

例 7.3.3 已知某厂生产的零件尺寸 $X \sim  N\left( {{12.5},{\sigma }^{2}}\right)$. 从某天生产的零件中随机地抽取 4 只, 测得样本观测值

$\begin{array}{llll} {12.6} & {13.4} & {12.8} & {13.2} \end{array}$

试求 ${\sigma }^{2}$ 的置信度为 0.95 的区间估计.

解 由

$$
\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - {\mu }_{0}\right) }^{2} = {\left( {12.6} - {12.5}\right) }^{2} + {\left( {13.4} - {12.5}\right) }^{2} + {\left( {12.8} - {12.5}\right) }^{2} + {\left( {13.2} - {12.5}\right) }^{2} = {1.4},
$$

和 $\alpha  = {0.05}$,查表或用 $\mathrm{R}$ 软件计算的 ${\chi }_{0.975}^{2}\left( 4\right)  = {11.14329}$ 和 ${\chi }_{0.025}^{2}\left( 4\right)  =$ 0.4844186,用 (7.3.7) 得到 ${\sigma }^{2}$ 的置信度为 0.95 的区间估计 $\left\lbrack  {{0.13},{2.89}}\right\rbrack$.

另外,请读者执行如下 $\mathrm{R}$ 程序,看有什么结果.

---

x<-c(12.6,13.4,12.8,13.2)

	mu0<-12.5

		alpha<-0.05

			n<-length(x)

					z1<-sum((x-mu0)^2)

							list(c.i=c(z1/qchisq(1-alpha/2, n), z1/qchisq(alpha/2, n)))

---

#### 4. ${\sigma }^{2}$ 的区间估计 $\left( {\mu \text{未知}}\right)$

此时由抽样分布基本定理 (见定理 6.3.1) 知

$$
\frac{n{S}_{n}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)
$$

经令

$$
P\left( {{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right)  \leq  \frac{n{S}_{n}^{2}}{{\sigma }^{2}} \leq  {\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }\right)  = 1 - \alpha,
$$

求出分位点 ${\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right)$ 和 ${\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right)$ 并作等式变形立得 ${\sigma }^{2}$ 的区间估计为

$$
\left\lbrack  {\frac{n{S}_{n}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) },\frac{n{S}_{n}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}\right\rbrack . \tag{7.3.8}
$$

请读者用例 7.3.3 的数据,但 $\mu$ 未知,求 ${\sigma }^{2}$ 的置信度为 0.95 的区间估计.

### 7.3.2 两个正态总体参数的区间估计

设 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$,且 $X$ 与 $Y$ 相互独立,样本分别为 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{m}}\right)$ 和 $\left( {{Y}_{1},{Y}_{2},\cdots,{Y}_{n}}\right)$. 样本均值与样本方差为

$\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i},\;\bar{Y} = \frac{1}{n}\mathop{\sum }\limits_{{j = 1}}^{n}{Y}_{j},\;{S}_{1m}^{2} = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - \bar{X}\right) }^{2},\;{S}_{2n}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - \bar{Y}\right) }^{2}.$

#### 1. ${\mu }_{1} - {\mu }_{2}$ 的区间估计 $\left( {{\sigma }_{1}^{2},{\sigma }_{2}^{2}}\right.$ 已知 $)$

由于 $\bar{X} \sim  N\left( {{\mu }_{1},\frac{{\sigma }_{1}^{2}}{m}}\right),\bar{Y} \sim  N\left( {{\mu }_{2},\frac{{\sigma }_{2}^{2}}{n}}\right)$,且由 $X$ 与 $Y$ 相互独立知 $\bar{X}$ 与 $\bar{Y}$

独立, 于是有

$$
\bar{X} - \bar{Y} \sim  N\left( {{\mu }_{1} - {\mu }_{2},\frac{{\sigma }_{1}^{2}}{m} + \frac{{\sigma }_{2}^{2}}{n}}\right),
$$

亦即

$$
\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{\sqrt{\frac{{\sigma }_{1}^{2}}{m} + \frac{{\sigma }_{2}^{2}}{n}}} \sim  N\left( {0,1}\right),
$$

由此令

$$
P\left( {\left| \frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{\sqrt{\frac{{\sigma }_{1}^{2}}{m} + \frac{{\sigma }_{2}^{2}}{n}}}\right|  \leq  {u}_{1 - \frac{\alpha }{2}}}\right)  = 1 - \alpha,
$$

求出分位点 ${u}_{1 - \frac{\alpha }{2}}$ 并作等式变形立得 ${\mu }_{1} - {\mu }_{2}$ 的区间估计

$$
\left\lbrack  {\left( {\bar{X} - \bar{Y}}\right)  - {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{m} + \frac{{\sigma }_{2}^{2}}{n}},\;\left( {\bar{X} - \bar{Y}}\right)  + {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{m} + \frac{{\sigma }_{2}^{2}}{n}}}\right\rbrack . \tag{7.3.9}
$$

#### 2. ${\mu }_{1} - {\mu }_{2}$ 的区间估计 $\left( {{\sigma }_{1}^{2} = {\sigma }_{2}^{2} = {\sigma }^{2}}\right.$ 未知 $)$

由推论 6.3.4 知

$$
\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{m} + \frac{1}{n}}} \sim  t\left( {m + n - 2}\right),
$$

由此令

$$
P\left( {\left| \frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{m} + \frac{1}{n}}}\right|  \leq  {t}_{1 - \frac{\alpha }{2}}\left( {m + n - 2}\right) }\right)  = 1 - \alpha,
$$

求出分位点 ${t}_{1 - \frac{\alpha }{2}}$ 并作等式变形立得 ${\mu }_{1} - {\mu }_{2}$ 的区间估计

$$
\begin{array}{r} \left\lbrack  {\left( {\bar{X} - \bar{Y}}\right)  - {t}_{1 - \frac{\alpha }{2}}\left( {m + n - 2}\right) {S}_{w}\sqrt{\frac{1}{m} + \frac{1}{n}},\left( {\bar{X} - \bar{Y}}\right)  + {t}_{1 - \frac{\alpha }{2}}\left( {m + n - 2}\right) {S}_{w}\sqrt{\frac{1}{m} + \frac{1}{n}}}\right\rbrack , \\  \left( {7.3.10}\right)  \end{array} \tag{7.3.10}
$$

其中 ${S}_{w} = \sqrt{\frac{m{S}_{1m}^{2} + n{S}_{2n}^{2}}{m + n - 2}}$.

例 7.3.4 两台机床生产同一型号的滚珠, 从甲机床和乙机床生产的滚珠中分别抽取 8 个和 9 个, 测得滚珠直径如下 (单位: mm)

甲机床: 15.0 14.8 15.2 15.4 14.9 15.1 15.2 14.8

乙机床: 15.2 15.0 14.8 15.1 15.0 14.6 14.8 15.1 14.5

已知两台机床生产的滚珠的直径都服从正态分布, 试求这两台机床生产的滚珠直径均值差的区间估计, 置信度为 0.90.

(1)已知甲、乙机床生产的滚珠直径的标准差分别为 ${\sigma }_{1} = {0.18}\mathrm{\;{mm}}$ 及 ${\sigma }_{2} =$ ${0.24}\mathrm{\;{mm}}$.

(2) ${\sigma }_{1},{\sigma }_{2}$ 未知,但知 ${\sigma }_{1} = {\sigma }_{2}$.

解 设甲、乙机床生产的滚珠直径分别为 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right)$ 和 $Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$, 由题意, $X$ 与 $Y$ 相互独立, $m = 8, n = 9$. 经计算得

$$
\bar{x} = {15.05},\;\bar{y} = {14.90},\;{s}_{1m}^{2} = {0.0457},\;{s}_{2n}^{2} = {0.0575}.
$$

(1) $\alpha  = {0.10}$,查表或用 $\mathrm{R}$ 软件计算的 ${u}_{0.95} = {1.645}$,用 (7.3.9) 得到 ${\mu }_{1} - {\mu }_{2}$ 的置信度为 0.90 的区间估计 $\left\lbrack  {-{0.018},{0.318}}\right\rbrack$.

(2) $\alpha  = {0.10}$,查表或用 $\mathrm{R}$ 软件计算的 ${t}_{0.95}\left( {15}\right)  = {1.75305}$,用 (7.3.10) 得到 ${\mu }_{1} - {\mu }_{2}$ 的置信度为 0.90 的区间估计 $\left\lbrack  {-{0.044},{0.344}}\right\rbrack$.

另外,请读者执行如下两个 $\mathrm{R}$ 程序,看有什么结果.

---

$x <  - c\left( {{15.0},{14.8},{15.2},{15.4},{14.9},{15.1},{15.2},{14.8}}\right)$

	$y <  - c\left( {{15.2},{15.0},{14.8},{15.1},{15.0},{14.6},{14.8},{15.1},{14.5}}\right)$

		sigma1<-0.18; sigma2<-0.24

			alpha<-0.10

			n1<-length(x); n2<-length(y)

			z1<-mean(x)-mean(y)

					z2<-qnorm(1-alpha/2)*sqrt(sigma1^2/n1+sigma2^2/n2)

						list(c.i1=c(z1-z2, z1+z2))

							z3<-qt(1-alpha/2, n1+n2-2)*sqrt((1/n1+1/n2)*((n1-1)*var(x)

								$+ \left( {{n2} - 1}\right)  * \operatorname{var}\left( y\right) )/\left( {{n1} + {n2} - 2}\right) )$

								list(c.i2=c(z1-z3, z1+z3))

---

128

或者

$x <  - c\left( {{15.0},{14.8},{15.2},{15.4},{14.9},{15.1},{15.2},{14.8}}\right)$

$y <  - c\left( {{15.2},{15.0},{14.8},{15.1},{15.0},{14.6},{14.8},{15.1},{14.5}}\right)$

sigma1<-0.18; sigma2<-0.24

alpha<-0.10

n1<-length(x); n2<-length(y)

z1<-mean(x)-mean(y)

z2<-qnorm(1-alpha/2)*sqrt(sigma1^2/n1+sigma2^2/n2)

list(c.i1=c(z1-z2, z1+z2))

t.test(x, y, conf.level=0.90, var.equal=TRUE)\$conf

#### 3. ${\sigma }_{1}^{2}/{\sigma }_{2}^{2}$ 的区间估计 $\left( {{\mu }_{1},{\mu }_{2}}\right.$ 已知 $)$

由于

$$
\frac{{X}_{i} - {\mu }_{1}}{{\sigma }_{1}} \sim  N\left( {0,1}\right),\;i = 1,2,\cdots, m.\;\frac{{Y}_{j} - {\mu }_{2}}{{\sigma }_{2}} \sim  N\left( {0,1}\right),\;j = 1,2,\cdots, n,
$$

所以

$$
\frac{\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{{\sigma }_{1}^{2}} \sim  {\chi }^{2}\left( m\right),\;\frac{\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}}{{\sigma }_{2}^{2}} \sim  {\chi }^{2}\left( n\right),
$$

从而由 $F$ 分布的定义有

$$
\frac{n}{m}\frac{\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}}\frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \sim  F\left( {m, n}\right),
$$

再令

$$
P\left( {{F}_{\frac{\alpha }{2}}\left( {m, n}\right)  \leq  \frac{n}{m}\frac{\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}}\frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \leq  {F}_{1 - \frac{\alpha }{2}}\left( {m, n}\right) }\right)  = 1 - \alpha,
$$

求出分位点 ${F}_{\frac{\alpha }{2}}\left( {m, n}\right)$ 和 ${F}_{1 - \frac{\alpha }{2}}\left( {m, n}\right)$ 并作等式变形立得 ${\sigma }_{1}^{2}/{\sigma }_{2}^{2}$ 的区间估计为

$$
\left\lbrack  {\frac{1}{{F}_{1 - \frac{\alpha }{2}}\left( {m, n}\right) }\frac{n\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{m\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}},\frac{1}{{F}_{\frac{\alpha }{2}}\left( {m, n}\right) }\frac{n\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{m\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}}}\right\rbrack . \tag{7.3.11}
$$

#### 4. ${\sigma }_{1}^{2}/{\sigma }_{2}^{2}$ 的区间估计 $\left( {{\mu }_{1},{\mu }_{2}}\right.$ 未知 $)$

由推论 6.3.3 知

$$
\frac{m{S}_{1m}^{2}}{n{S}_{2n}^{2}} \cdot  \frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \cdot  \frac{n - 1}{m - 1} = \frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}} \cdot  \frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \sim  F\left( {m - 1, n - 1}\right),
$$

其中 ${S}_{1m}^{*2} = \frac{m}{m - 1}{S}_{1m}^{2},{S}_{2n}^{*2} = \frac{n}{n - 1}{S}_{2n}^{2}$,再令

$$
P\left( {{F}_{\frac{\alpha }{2}}\left( {m - 1, n - 1}\right)  \leq  \frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}} \cdot  \frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \leq  {F}_{1 - \frac{\alpha }{2}}\left( {m - 1, n - 1}\right) }\right)  = 1 - \alpha,
$$

求分位点 $\left( {{F}_{\frac{\alpha }{2}}\left( {m - 1, n - 1}\right) }\right.$ 和 ${F}_{1 - \frac{\alpha }{2}}\left( {m - 1, n - 1}\right)$ 并作等式变形立得 ${\sigma }_{1}^{2}/{\sigma }_{2}^{2}$ 的区间估计为

$$
\left\lbrack  {\frac{1}{{F}_{1 - \frac{\alpha }{2}}\left( {m - 1, n - 1}\right) }\frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}},\;\frac{1}{{F}_{\frac{\alpha }{2}}\left( {m - 1, n - 1}\right) }\frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}}}\right\rbrack . \tag{7.3.12}
$$

我们将 7.3.1 节和 7.3.2 节的结果总结于表 7.1.

表 7.1 正态总体参数的区间估计

<table><tr><td>总体数目</td><td>待估计参数</td><td>用到的样本函数及其分布</td><td>区间估计</td></tr><tr><td rowspan="4">一个总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ ${S}_{n}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}$</td><td>$\mu \left( {{\sigma }^{2} = {\sigma }_{0}^{2}}\right.$ 已知 $)$</td><td>$\frac{\bar{X} - \mu }{\sqrt{\frac{{\sigma }_{0}^{2}}{n}}} \sim  N\left( {0,1}\right)$</td><td>$\left\lbrack  {\bar{X} \pm  {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{0}^{2}}{n}}}\right\rbrack$</td></tr><tr><td>$\mu \left( {\sigma }^{2}\right.$ 未知 $)$</td><td>$\frac{\bar{X} - \mu }{{S}_{n}}\sqrt{n - 1} \sim  t\left( {n - 1}\right)$</td><td/></tr><tr><td>${\sigma }^{2}\left( {\mu  = {\mu }_{0}}\right.$ 已知 $)$</td><td>$\mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {X}_{i} - {\mu }_{0}\right) }^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( n\right)$</td><td>$\frac{\left\lbrack  \bar{X} \pm  {t}_{1 - \frac{\alpha }{2}}\left( n - 1\right) \frac{{S}_{n}}{\sqrt{n - 1}}\right\rbrack  }{\left\lbrack  \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - {\mu }_{0}\right) }^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right) },\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - {\mu }_{0}\right) }^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( n\right) }\right\rbrack  }$</td></tr><tr><td>${\sigma }^{2}\left( {\mu \text{未知}}\right)$</td><td>$\frac{n{S}_{n}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)$</td><td>$\left\lbrack  {\frac{n{S}_{n}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) },\frac{n{S}_{n}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}\right\rbrack$</td></tr><tr><td>两个总体</td><td>${\mu }_{1} - {\mu }_{2}\left( {{\sigma }_{1}^{2},{\sigma }_{2}^{2}}\right.$ 已知 $)$</td><td>$\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{\sqrt{\frac{{\sigma }_{1}^{2}}{m} + \frac{{\sigma }_{2}^{2}}{n}}} \sim  N\left( {0,1}\right)$</td><td>$\left\lbrack  {\left( {\bar{X} - \bar{Y}}\right)  \pm  {u}_{1 - \frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{m} + \frac{{\sigma }_{2}^{2}}{n}}}\right\rbrack$</td></tr><tr><td rowspan="3">$X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right)$ $\bar{X} = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{X}_{i}$ ${S}_{1m}^{2} = \frac{1}{m}\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - \bar{X}\right) }^{2}$ $Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$ $\bar{Y} = \frac{1}{n}\mathop{\sum }\limits_{{j = 1}}^{n}{Y}_{j}$ ${S}_{2n}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{i} - \bar{Y}\right) }^{2}$</td><td>${\mu }_{1} - {\mu }_{2}\left( {{\sigma }_{1}^{2} = {\sigma }_{2}^{2}}\right.$ 未知 $)$</td><td>$\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{m} + \frac{1}{n}}}$ $\sim  t\left( {m + n - 2}\right)$</td><td>$\left( {\bar{X} - \bar{Y}}\right)  \pm  {t}_{1 - \frac{\alpha }{2}}\left( {m + n - 2}\right)$ $\times  {S}_{w}\sqrt{\frac{1}{m} + \frac{1}{n}}$</td></tr><tr><td>$\frac{{\sigma }_{1}^{2}}{{\sigma }_{2}^{2}}\left( {{\mu }_{1},{\mu }_{2}\text{ 已知 }}\right)$</td><td>$\frac{n\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{m\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}}\frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}}$ $\sim  F\left( {m, n}\right)$</td><td>$\frac{1}{{F}_{1 - \frac{\alpha }{2}}\left( {m, n}\right) }\frac{n\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{m\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}},$ $\left. {\frac{1}{{F}_{\frac{\alpha }{2}}\left( {m, n}\right) }\frac{n\mathop{\sum }\limits_{{i = 1}}^{m}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{m\mathop{\sum }\limits_{{j = 1}}^{n}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}},}\right\rbrack$</td></tr><tr><td>$\frac{{\sigma }_{1}^{2}}{{\sigma }_{2}^{2}}\left( {{\mu }_{1},{\mu }_{2}\text{ 未知 }}\right)$</td><td>$\frac{m{S}_{1m}^{2}}{n{S}_{2n}^{2}} \cdot  \frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \cdot  \frac{n - 1}{m - 1} = \frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}} \cdot  \frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}}$ $\sim  F\left( {m - 1, n - 1}\right)$</td><td>$\frac{1}{{F}_{1 - \frac{\alpha }{2}}\left( {m - 1, n - 1}\right) }\frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}},$ $\left. {\frac{1}{{F}_{\frac{\alpha }{2}}\left( {m - 1, n - 1}\right) }\frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}}}\right\rbrack$</td></tr></table>

例 7.3.5 就例 7.3.4 的假设和数据, 试求这两台机床生产的滚珠直径方差比的区间估计, 置信度为 0.90.

(1)已知甲、乙机床生产的滚珠直径的均值分别为 ${\mu }_{1} = {15.0}\mathrm{\;{mm}}$ 及 ${\mu }_{2} =$ ${14.90}\mathrm{\;{mm}}$.

(2) ${\mu }_{1},{\mu }_{2}$ 未知.

解 (1) 沿用例 7.3.4 的记号, 经计算得

$$
\mathop{\sum }\limits_{{i = 1}}^{8}{\left( {x}_{i} - {\mu }_{1}\right) }^{2} = {0.34},\;\mathop{\sum }\limits_{{j = 1}}^{9}{\left( {y}_{j} - {\mu }_{1}\right) }^{2} = {0.46},
$$

$\alpha  = {0.10}$,查表或用 $\mathrm{R}$ 软件计算的 ${F}_{0.95}\left( {8,9}\right)  = {3.229583}$ 和 ${F}_{0.05}\left( {8,9}\right)  = {0.295148}$. 用 (7.3.11) 得到 ${\sigma }_{1}^{2}/{\sigma }_{2}^{2}$ 的置信度为 0.90 的区间估计 $\left\lbrack  {{0.257},{2.817}}\right\rbrack$.

(2) 经计算得

$$
{s}_{1m}^{*2} = {0.0457},\;{s}_{2n}^{*2} = {0.0575},
$$

$\alpha  = {0.10}$,查表或用 $\mathrm{R}$ 软件计算的 ${F}_{0.95}\left( {7,8}\right)  = {3.500464}$ 和 ${F}_{0.05}\left( {7,8}\right)  = {0.2684041}$. 用 (7.3.12) 得到 ${\sigma }_{1}^{2}/{\sigma }_{2}^{2}$ 的置信度为 0.90 的区间估计 $\left\lbrack  {{0.277},{2.962}}\right\rbrack$.

另外,请读者执行如下两个 $\mathrm{R}$ 程序,看有什么结果.

---

													$x <  - c\left( {{15.0},{14.8},{15.2},{15.4},{14.9},{15.1},{15.2},{14.8}}\right)$

												$y <  - c\left( {{15.2},{15.0},{14.8},{15.1},{15.0},{14.6},{14.8},{15.1},{14.5}}\right)$

											mu1<-15.0; mu2<-14.9

												alpha<-0.10

											n1<-length(x); n2<-length(y)

									z1<-sum((x-mu1)^2); z2<-sum((y-mu2)^2)

								list(c.i1=c(n2*z1/(n1*z2*qf(1-alpha/2, n1, n2)),

									n2*z1/(n1*z2*qf(alpha/2, n1, n2)))

							z3<-var(x)/var(y)

							list(c.i2=c(z3/qf(1-alpha/2, n1-1, n2-1), z3/qf(alpha/2, n1-1, n2-1)))

							或者

				$x <  - c\left( {{15.0},{14.8},{15.2},{15.4},{14.9},{15.1},{15.2},{14.8}}\right)$

				$y <  - c\left( {{15.2},{15.0},{14.8},{15.1},{15.0},{14.6},{14.8},{15.1},{14.5}}\right)$

			mu1<-15.0; mu2<-14.9

				alpha<-0.10

		n1<-length(x); n2<-length(y)

	z1<-sum((x-mu1)^2); z2<-sum((y-mu2)^2)

	list(c.i1=c(n2*z1/(n1*z2*qf(1-alpha/2, n1, n2)),

	n2*z1/(n1*z2*qf(alpha/2, n1, n2)))

var.test(x, y, conf.level=0.9) \$conf.int

---

### 7.3.3 单个正态总体参数 $\left( {\mu,{\sigma }^{2}}\right)$ 的联合区间估计

基于抽样分布基本定理 (见定理 6.3.1) 我们还可以得到正态总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 中参数 $\mu$ 和 ${\sigma }^{2}$ 的联合区间估计.

事实上, 若

$$
P\left( {\left| \frac{\bar{X} - \mu }{\sqrt{\frac{{\sigma }^{2}}{n}}}\right|  \leq  l,{k}_{1} \leq  \frac{n{S}_{n}^{2}}{{\sigma }^{2}} \leq  {k}_{2}}\right)  = 1 - \alpha,
$$

由于 $\bar{X}$ 与 ${S}_{n}^{2}$ 独立,则有

$$
P\left( {\left| \frac{\bar{X} - \mu }{\sqrt{\frac{{\sigma }^{2}}{n}}}\right|  \leq  l}\right)  \cdot  P\left( {{k}_{1} \leq  \frac{n{S}_{n}^{2}}{{\sigma }^{2}} \leq  {k}_{2}}\right)  = 1 - \alpha.
$$

若令

$$
P\left( {\left| \frac{\bar{X} - \mu }{\sqrt{\frac{{\sigma }^{2}}{n}}}\right|  \leq  l}\right)  = \sqrt{1 - \alpha }\text{ 和 }P\left( {{k}_{1} \leq  \frac{n{S}_{n}^{2}}{{\sigma }^{2}} \leq  {k}_{2}}\right)  = \sqrt{1 - \alpha },
$$

则有

$$
P\left( {\frac{n{\left( \bar{X} - \mu \right) }^{2}}{{l}^{2}} \leq  {\sigma }^{2}}\right)  = \sqrt{1 - \alpha }\text{ 和 }P\left( {\frac{n{S}_{n}^{2}}{{k}_{2}} \leq  {\sigma }^{2} \leq  \frac{n{S}_{n}^{2}}{{k}_{1}}}\right)  = \sqrt{1 - \alpha }.
$$

由于

$$
\frac{\bar{X} - \mu }{\sqrt{\frac{{\sigma }^{2}}{n}}} \sim  N\left( {0,1}\right) \text{ 和 }\frac{n{S}_{n}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right),
$$

可查表得 $l = {u}_{\frac{1}{2}\left( {1 + \sqrt{1 - \alpha }}\right) },{k}_{1} = {\chi }_{\frac{1}{2}\left( {1 - \sqrt{1 - \alpha }}\right) }^{2}\left( {n - 1}\right),{k}_{2} = {\chi }_{\frac{1}{2}\left( {1 + \sqrt{1 - \alpha }}\right) }^{2}\left( {n - 1}\right)$. 最终我们得到 $\left( {\mu,{\sigma }^{2}}\right)$ 的置信度为 $1 - \alpha$ 联合区间估计,

$$
\left\{  {\left( {\mu,{\sigma }^{2}}\right)  : \frac{n{\left( \bar{X} - \mu \right) }^{2}}{{u}_{\frac{1}{2}\left( {1 + \sqrt{1 - \alpha }}\right) }^{2}} \leq  {\sigma }^{2},\frac{n{S}_{n}^{2}}{{\chi }_{\frac{1}{2}\left( {1 + \sqrt{1 - \alpha }}\right) }^{2}\left( {n - 1}\right) } \leq  {\sigma }^{2} \leq  \frac{n{S}_{n}^{2}}{{\chi }_{\frac{1}{2}\left( {1 - \sqrt{1 - \alpha }}\right) }^{2}\left( {n - 1}\right) }}\right\} .
$$

该联合区间估计在 $\mu  - {\sigma }^{2}$ 平面上区域如图 7.1 所示 (图中 $\left. {\left( {n - 1}\right) {S}_{n}^{*2} = n{S}_{n}^{2}}\right)$.

![01938b00-6b6a-7014-9166-35043ab11e9a_132_615_80_400_274_0.jpg](teach/Probability-Statistic/images/01938b00-6b6a-7014-9166-35043ab11e9a_132_615_80_400_274_0.jpg)

图 7.1 正态总体 $\left( {\mu,{\sigma }^{2}}\right)$ 的联合区间估计示意图.

### 7.3.4 非正态总体参数的区间估计

对于非正态总体, 往往难以得到其有关统计量的精确分布, 一般都是在样本容量较大时, 用近似分布求出参数的区间估计.

一般地,设 $X \sim  {F}_{X}\left( {\cdot,\theta }\right)$,其样本均值为 $\bar{X}$ 和 ${S}_{n}^{2}$,则可以证明. 当样本容量 $n$ 充分大时,近似地有

$$
\frac{\bar{X} - E\left\lbrack  X\right\rbrack  }{{S}_{n}}\sqrt{n} \sim  N\left( {0,1}\right). \tag{7.3.13}
$$

例 7.3.6 (两点分布的参数的区间估计) 设总体 $X \sim  B\left( {1, p}\right)$,试求 $p$ 的置信度为 $1 - \alpha$ 的区间估计.

解 由于 $E\left\lbrack  X\right\rbrack   = p$ 和 ${S}_{n}^{2} = \bar{X}\left( {1 - \bar{X}}\right)$,利用 (7.3.13) 近似地有

$$
\frac{\bar{X} - p}{\sqrt{\bar{X}\left( {1 - \bar{X}}\right) }}\sqrt{n} \sim  N\left( {0,1}\right).
$$

计 对于给定的置信度 $1 - \alpha$,由标准正态分布表查得 ${u}_{1 - \frac{\alpha }{2}}$,就得到 $p$ 的区间估

$$
\left\lbrack  {\bar{X} - {u}_{1 - \frac{\alpha }{2}}\sqrt{\bar{X}\left( {1 - \bar{X}}\right) /n},\bar{X} + {u}_{1 - \frac{\alpha }{2}}\sqrt{\bar{X}\left( {1 - \bar{X}}\right) /n}}\right\rbrack .
$$

## 第七章小结与注记

(1) 本章中关于参数的点估计, 我们介绍了矩法估计、最大似然估计和顺序统计量估计三种方法, 每种方法的想法都很直观并且各不相同. 其中最能反映概率思想的是最大似然估计. 它一方面基于 “小概率事件在一次试验中近乎不发生” 这样一基本认知. 另一方面, 在求参数的最大似然估计时, 用到总体的分布类型, 从这一点上讲, 它一般比矩法估计和顺序统计量估计的性能好一些, 或者说其统计特性更好把握些. 也正是如此, 一般在作进一步的理论分析时, 往往假定有关参数的估计量为最大似然估计量.

(2)评价一个估计量的优劣,比起想起一种估计方法要难得多. 首先要定义优或劣的标准, 再考证一个统计量在该标准下是否比较优. 应当说, 要求一个统计量做到其均值等于待估计参数 (即无偏性), 是一个最起码的要求, 在此基础上找一个方差是最小的也是最朴素的愿望. 遗憾的是, 目前还没有一个构造性的万法 (比如复合函数求导就是构造性的方法, 而求不定积分就没有构造性的方法), 去求得任意总体的参数的一致最小方差无偏估计, 只能分门别类的讨论, 得到稍有普遍意义的方法.

(3) 与参数的点估计不同, 区间估计要求得到的参数估计的随机区间要满足给定的置信度, 这就要求在构造统计量的同时, 要寻求其概率分布. 这一点, 对于一般分布的总体难以做到, 我们只好介绍正态总体参数的区间估计.

(4)对于正态总体参数的区间估计,虽然我们解释了各种情形下区间估计的由来, 但基本上是死搬硬套的, 试想没有第六章的抽样分布基本定理及其推论, 我们将如何做得到!

## 第七章习题

7.1. 设总体 $X$ 的分布密度函数为

$$
f\left( {x,\theta }\right)  = \left\{  \begin{matrix} \theta \left( {\theta  + 1}\right) {x}^{\theta  - 1}\left( {1 - x}\right), & 0 < x \leq  1 \\  0, & \text{ 其他,} \end{matrix}\right.
$$

其中 $\theta  > 0.\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为来自总体 $X$ 的简单随机样本,求未知参数 $\theta$ 的矩估计量.

7.2. 假设每升水中大肠杆菌的数目 $X$ 服从泊松分布 $\operatorname{Pois}\left( \lambda \right)$,其中 $\lambda  > 0$. 为了检验某种自来水消毒设备的效果, 现从消毒后的水中随机抽取 60 个样品 (每个样品为 1 升水) 进行化验, 结果如下:

<table><tr><td>大肠杆菌的个数/升</td><td>0</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td></tr><tr><td>样品数</td><td>16</td><td>22</td><td>10</td><td>7</td><td>3</td><td>2</td></tr></table>

试求未知参数 $\lambda$ 的矩估计值. 7.3. 设总体 $X$ 的分布密度函数为 $f\left( {x,\theta }\right)  = \frac{1}{2\theta }{\mathrm{e}}^{-\frac{\left| x\right| }{\theta }}$,其中 $\theta  > 0$ 是未知参数, $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是 $X$ 的容量为 $n$ 的样本. 求 $\theta$ 的最大似然估计量.

7.4. 设总体 $X$ 的分布密度函数为

$$
f\left( {x,\theta }\right)  = \left\{  \begin{array}{ll} \frac{1}{\theta }{\mathrm{e}}^{-\frac{x - 1}{\theta }}, & x > 1, \\  0, & x \leq  1, \end{array}\right.
$$

其中 $\theta  > 0$ 是未知参数, $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是 $X$ 的容量为 $n$ 的样本. 求 $\theta$ 的最大似然估计量.

7.5. 设总体 $X$ 的分布列为

![01938b00-6b6a-7014-9166-35043ab11e9a_134_585_141_463_88_0.jpg](teach/Probability-Statistic/images/01938b00-6b6a-7014-9166-35043ab11e9a_134_585_141_463_88_0.jpg)

其中 $0 < \theta  < \frac{1}{2}$,今有样本观测值

1,1,1,3,2,1,3,2,2,1,2,2,3,1,1,2

试求 $\theta$ 的最大似然估计值.

7.6. 设总体 $X \sim  B\left( {m, p}\right)$,其中 $0 < p < 1, p$ 为未知参数, $m$ 为正整数且已知. $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是取自总体 $X$ 的样本,求未知参数 $p$ 的矩估计量 ${\widehat{p}}_{M}$ 及最大似然估计量

7.7. 设总体 $X$ 服从区间 $\left\lbrack  {\theta,{2\theta }}\right\rbrack  \left( {\theta  > 0}\right)$ 上的均匀分布, $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是取自总体 $X$ 的样本,试求 $\theta$ 的矩估计量 ${\widehat{\theta }}_{M}$ 及最大似然估计量 ${\widehat{\theta }}_{L}$.

7.8. 设总体 $X \sim  \operatorname{Exp}\left( \lambda \right)$,其中 $\lambda \left( { > 0}\right)$ 为未知参数,现从总体中抽得容量为 8 的样本观测值分别为

$$
{1250},{1265},{1245},{1260},{1275},{1248},{1252},{1261}
$$

试求 $\lambda$ 的矩估计值 ${\widehat{\lambda }}_{M}$ 及最大似然估计值 ${\widehat{\lambda }}_{L}$.

7.9. 设总体 $X$ 的密度函数为

$$
f\left( {x,\alpha,\beta }\right)  = \left\{  \begin{array}{ll} \frac{1}{\beta }{\mathrm{e}}^{-\frac{x - \alpha }{\beta }}, & \alpha  \leq  x,\;\alpha  > 0,\beta  > 0, \\  0, & \text{ 否则,} \end{array}\right.
$$

其中 $\alpha,\beta$ 为未知参数, $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是取自总体 $X$ 的样本,试求 $\alpha,\beta$ 的矩估计量及最大似然估计量.

7.10. 已知某种灯泡的寿命服从指数分布, 现从该种灯泡随机抽取 12 只, 测得寿命分别为 (单位: 小时):

$$
{1120},{1020},{1196},{1126},{1296},{1306},{1095},{1180},{1280},{1322},{1091},{1122}
$$

试用最大似然估计方法估计出这种型号灯泡寿命超过 1500 小时的概率.

7.11. 假设总体 $X$ 服从参数为 $p$ 的 $0 - 1$ 分布 $\left( {0 < p < 1}\right),\left( {{X}_{1},\cdots,{X}_{n}}\right)$ 为来自 $X$ 的样本. (1) 试求 ${p}^{2}$ 的无偏估计. (2) 证明: $1/p$ 的无偏估计不存在.

7.12. 若总体 $X$ 的分布密度函数为

$$
f\left( {x,\theta }\right)  = \left\{  \begin{array}{ll} \frac{x}{\theta }{\mathrm{e}}^{-\frac{{x}^{2}}{2\theta }}, & x > 0, \\  0, & x \leq  0, \end{array}\right.
$$

其中 $\theta \left( { > 0}\right)$ 为未知参数, $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是取自总体 $X$ 的样本,试求 $\theta$ 的无偏估计量.

7.13. 设总体 $X$ 在区间 $\left\lbrack  {0,\theta }\right\rbrack$ 上服从均匀分布,其中参数 $\theta$ 未知, $\left( {{X}_{1},\cdots,{X}_{n}}\right) \left( {n > 2}\right)$ 是从该总体抽取的样本. (1) 证明 ${T}_{1} = 2\bar{X},{T}_{2} = \left( {n + 1}\right) {X}_{\left( 1\right) }$ 均为 $\theta$ 的无偏估计量. (2) 问哪个估计量更为有效？

7.14. 设 $\left( {{X}_{1},\cdots,{X}_{n}}\right)$ 是来自服从区间 $\left\lbrack  {0,{2\theta }}\right\rbrack$ 均匀分布的一个样本,求 $\theta$ 的极大似然估计量,并证明其是 $\theta$ 的相合估计.

7.15. 设 $\left( {{X}_{1},\cdots,{X}_{n}}\right)$ 是来自泊松分布 $\operatorname{Pois}\left( \theta \right)$ 的一个样本,证明: $2\bar{X} + 5$ 是 ${2\theta } + 5$ 的相合估计.

7.16. 设总体 $X$ 服从二项分布 $B\left( {{10},\theta }\right)$,其中 $\theta \left( {0 < \theta  < 1}\right)$ 为未知参数, $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是来自总体 $X$ 的一个样本. (1) 求 $\theta$ 的最大似然估计量. (2) 证明该估计量是无偏的并且为 $\theta$ 的相合估计.

7.17. 设总体 $X \sim  N\left( {\mu,4}\right)$,其中 $\mu$ 未知. $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为来自总体 $X$ 的简单随机样本,则 $\left\lbrack  {\bar{X} - \frac{2{u}_{0.95}}{\sqrt{n}},\bar{X} + \frac{2{u}_{0.95}}{\sqrt{n}}}\right\rbrack$ 作为 $\mu$ 的置信区间,其置信度为多少并说明原因? 要使置信区间的长度不超过 1, 样本容量至少为多少?

7.18. 设总体 $X$ 服从 $N\left( {\mu,1}\right)$,其中 $\mu$ 为未知参数. $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 是来自总体 $X$ 的一个样本观测值. 假定由这组观测值求出 $\mu$ 的置信水平为 $1 - \alpha$ 的置信区间为 $\left\lbrack  {{0.2},5}\right\rbrack$,由这组观测值确定 $\theta  = {3\mu } + 7$ 的置信度为 $1 - \alpha$ 的置信区间.

7.19. 某自动包装机包装洗衣粉,其重量 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,其中 $\mu,\sigma$ 未知. 今随机抽取 12 袋测得其重量,经计算得样本均值 $\bar{x} = {1000.25}\left( \mathrm{\;g}\right)$,修正样本标准差 ${s}_{12}^{ * } = {2.6329}\left( \mathrm{\;g}\right)$,试求

(1) 总体均值 $\mu$ 的置信度为 0.95 的置信区间,

(2) 总体标准差 $\sigma$ 的置信度为 0.95 的置信区间.

7.20. 为了比较甲、乙两类试验田的收获量, 随机抽取甲类试验田 8 块, 乙类试验田 10 块, 测得亩产量如下 (单位: kg):

甲类 :510,628,583,615,554,612,530,525

乙类:433,535,398,470,560,567,498,480,503,426

假定这两类试验田的亩产量都服从正态分布,且方差相同,求两总体均值之差 ${\mu }_{\text{甲 }} - {\mu }_{乙}$ 的置信度为 ${95}\%$ 的置信区间.

7.21. 有两位化验员 $A$ 与 $B$ 独立地对一批聚合物含氯量用同样方法各进行 10 次重复测定,其样本方差分别为 ${S}_{\# }^{*2} = {0.541},{S}_{Z}^{*2} = {0.606}$,若 $A$ 与 $B$ 的测量值都服从正态分布,试求总体方差比 ${\sigma }_{\text{甲 }}^{2}/{\sigma }_{\text{乙 }}^{2}$ 的 ${95}\%$ 的置信区间.