## §1. 点 估 计

### 知识要点

#### 1. 点估计

设 $\theta$ 是总体 $X$ 的未知参数,用统计量 $\widehat{\theta } = \widehat{\theta }\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 来估计 $\theta$,称 $\widehat{\theta }$ 为 $\theta$ 的估计量. 对于样本的一组观察值 ${x}_{1},{x}_{2},\cdots,{x}_{n}$,代入 $\widehat{\theta }$ 的表达式中所得的具体数值称为 $\theta$ 的估计值. 这样的方法称为参数的点估计.

#### 2. 矩估计

用样本矩去估计相应总体矩, 或者用样本矩的函数去估计总体矩的同一函数的估计方法就是矩估计.

设总体 $X$ 的概率分布含有 $m$ 个未知参数 ${\theta }_{1},{\theta }_{2},\cdots,{\theta }_{m}$,假定总体的 $k$ 阶原点矩存在,记 ${\mu }_{k} =$ $E\left( {X}^{k}\right) \left( {k = 1,2,\cdots, m}\right),{A}_{k} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{k}$ 为样本 $k$ 阶矩,令

$$
{\mu }_{k}\left( {{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{m}}\right)  = {A}_{k}\left( {k = 1,2,\cdots, m}\right),
$$

则此方程组的解 $\left( {{\widehat{\theta }}_{1},{\widehat{\theta }}_{2},\cdots,{\widehat{\theta }}_{m}}\right)$ 称为参数 $\left( {{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{m}}\right)$ 的矩估计量. 矩估计量的观察值称为矩估计值.

#### 3. 最大似然估计 (极大似然估计)

(1)设总体 $X$ 的概率分布为 $p\left( {x;\theta }\right)$ (当 $X$ 为连续型时,其为概率密度函数,当 $X$ 为商散型时,其为分布律), $\theta  = \left( {{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{m}}\right)$ 为未知参数, ${x}_{1},\cdots,{x}_{n}$ 为样本观察值.

$$
L\left( {{x}_{1},\cdots,{x}_{n},\theta }\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}p\left( {{x}_{i};\theta }\right)  = L\left( \theta \right),
$$

称为 $\theta$ 的似然函数.

( 2 )对给定的 ${x}_{1},\cdots,{x}_{n}$,使似然函数达到最大值的 $\widehat{\theta }\left( {{x}_{1},\cdots,{x}_{n}}\right)$ 称为 $\theta$ 的最大似然估计值, 相应地 $\widehat{\theta }\left( {{X}_{1},\cdots,{X}_{n}}\right)$ 称为 $\theta$ 的最大似然估计量.

(3)最大似然估计的常用求解方法. 由于 $\ln L\left( \theta \right)$ 与 $L\left( \theta \right)$ 有相同的最大值点,若 $L\left( \theta \right)$ 可导, 则可由方程组

$$
\frac{\partial \ln L\left( {{\theta }_{1},{\theta }_{2},\cdots,{\theta }_{m}}\right) }{\partial {\theta }_{i}} = 0\;\left( {i = 1,2,\cdots, m}\right),
$$

求出 ${\theta }_{i}$ 的最大似然估计量,需注意的是这一方法并不都是有效的,对于有些似然函数,其驻点或导数不存在, 这时应考虑其他方法求似然函数的最大值点.

### 基本题型

#### 题型 1: 求矩估计

【1.1】设总体 $X$ 的概率密度函数为

$$
f\left( {x;\theta }\right)  = \left\{  {\begin{array}{ll} \theta {x}^{\theta  - 1}, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array}\;\left( {\theta  > 0}\right) }\right.
$$

求未知参数 $\theta$ 的矩估计量.

分析 根据求矩估计量的求解步骤,先求出 $X$ 的数学期望,得到参数 $\theta$ 与期望的关系,然后由样本均值替换总体期望,即是 $\theta$ 的矩估计.

解 ${EX} = {\int }_{-\infty }^{+\infty }x \cdot  f\left( {x;\theta }\right) \mathrm{d}x = {\int }_{0}^{1}{x\theta }{x}^{\theta  - 1}\mathrm{\;d}x = \frac{\theta }{\theta  + 1}$,

令 ${EX} = \bar{X}$,则 $\widehat{\theta } = \frac{\bar{X}}{1 - \bar{X}}$,其中 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$,则 $\widehat{\theta }$ 即为参数 $\theta$ 的矩估计.

【1.2】设总体 $X$ 的分布律为 $P\{ X = x\}  = {\left( 1 - p\right) }^{x - 1}p, x = 1,2,\cdots,\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是来自总体 $X$ 的样本,试求 $p$ 的矩估计量.

分析 对离散型随机变量同样是从求其数学期望出发,得到参数和数学期望之间的关系, 用样本均值替代总体期望.

解 因为 $X$ 服从几何分布,所以由几何分布的数字特征结论.

$E\left( X\right)  = \frac{1}{p}$,令 ${EX} = \bar{X}$.

因此参数 $p$ 的矩估计量 $\widehat{p} = \frac{1}{\bar{X}}$.

【1.3】设总体 $X$ 在 $\left\lbrack  {a, b}\right\rbrack$ 上服从均匀分布, $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本,样本均值 $\bar{X}$,样本方差 ${S}^{2}$,则 $a, b$ 的矩估计 $\widehat{a} = \widehat{a},\widehat{b} =$

解 由均匀分布的数字特征结论:

$$
{EX} = \frac{a + b}{2},\;{DX} = \frac{{\left( b - a\right) }^{2}}{12}.
$$

令 ${EX} = \bar{X},{DX} = {S}^{2}$,解得

$$
\widehat{a} = \bar{X} - \sqrt{3}S,\;\widehat{b} = \bar{X} + \sqrt{3}S,
$$

即为 $a, b$ 的矩估计.

点评 因为需要估计两个参数 $a, b$,所以应该构造两个方程: (1) 求出期望 ${EX}$ 用 $\bar{X}$ 代替; ( 2 )求出方差 ${DX}$ 用 ${S}^{2}$ 代替,也可以求出 $E\left( {X}^{2}\right)$ 用 ${A}_{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 代替,这样结果变成

$$
\widehat{a} = \bar{X} - \sqrt{3{B}_{2}},\;\widehat{b} = \bar{X} + \sqrt{3{B}_{2}},
$$

其中 ${B}_{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}$ 为二阶样本中心距.

【1.4】随机地取 8 只活塞环,测得它们的直径为 (单位:mm)

$\begin{array}{llllllll} {74.001} & {74.005} & {74.003} & {74.001} & {74.000} & {73.993} & {74.006} & {74.002} \end{array}$

试求总体均值 $\mu$ 及方差 ${\sigma }^{2}$ 的矩估计值,并求样本方差 ${S}^{2}$.

解 由矩法估计知

$$
\left\{  \begin{array}{l} {\mu }_{1} = E\left( X\right)  = \mu \\  {\mu }_{2} = E\left( {X}^{2}\right)  = D\left( X\right)  + {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} = {\sigma }^{2} + {\mu }^{2} \end{array}\right.
$$

令 $\left\{  \begin{array}{l} \mu  = {A}_{1} \\  {\sigma }^{2} + {\mu }^{2} = {A}_{2} \end{array}\right.$,解之得

$$
\widehat{\mu } = {A}_{1} = \bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i},
$$

$$
{\widehat{\sigma }}^{2} = {A}_{2} - {A}_{1}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - {\bar{X}}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}.
$$

由题中数据得 $\overset{\Lambda }{\mu } = {74.001},\;{\overset{\Lambda }{\sigma }}^{2} = 6 \times  {10}^{-6}$.

样本方差 ${s}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \bar{x}\right) }^{2} = {6.86} \times  {10}^{-6}$.

题型2: 求最大似然估计

方法与技巧 求最大似然估计的一般步骤为:

(1)构造似然函数；

(2)求似然函数的最大值点,此即所求最大似然估计.

求最大似然估计的三种情形:

(1)解极大似然方程(组);

(2)利用定义 $L\left( \widehat{\theta }\right)  = \max L\left( \theta \right)$;

(3)按照极大似然的不变性.

【1.5】设总体 $X$ 的概率密度为

$$
f\left( {x;\lambda }\right)  = \left\{  \begin{array}{ll} {\lambda \alpha }{x}^{\alpha  - 1}{\mathrm{e}}^{-\lambda {x}^{\alpha }}, & \text{ 若 }x > 0 \\  0, & \text{ 若 }x \leq  0 \end{array}\right.
$$

其中 $\lambda  > 0$ 是未知参数, $\alpha  > 0$ 是已知常数,根据来自总体 $X$ 的简单随机样本 ${X}_{1},{X}_{2},\cdots,{X}_{n}$,求 $\lambda$ 的最大似然估计量 $\widehat{\lambda }$.

分析 求最大似然估计关键是要确定似然函数.

解 由已知条件可得似然函数为

$$
L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\lambda }\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}f\left( {{x}_{i};\lambda }\right)  = {\left( \lambda \alpha \right) }^{n}{\mathrm{e}}^{-\lambda \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}^{\alpha }}\mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}^{\alpha  - 1}.
$$

当 ${x}_{i} > 0$ 时, $L > 0$,且有

$$
\ln L = n\ln \left( {\lambda \alpha }\right)  + \ln \mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}^{\alpha  - 1} - \lambda \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}^{\alpha },
$$

根据对数似然方程

$$
\frac{\mathrm{d}\ln L}{\mathrm{\;d}\lambda } = \frac{n}{\lambda } - \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}^{\alpha } = 0,
$$

解得 $\lambda$ 的最大似然估计 $\widehat{\lambda } = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}^{\alpha }}$. 巴 236

则 $\lambda$ 的最大似然估计量为 $\widehat{\lambda } = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{\alpha }}$.

【1.6】设某种元件的使用寿命 $X$ 的概率密度为

$$
f\left( {x;\theta }\right)  = \left\{  \begin{array}{ll} 2{\mathrm{e}}^{-2\left( {x - \theta }\right) }, & x > \theta \\  0, & x \leq  \theta  \end{array}\right.
$$

其中 $\theta  > 0$ 为未知参数,又设 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 是 $X$ 的一组样本观测值,求参数 $\theta$ 的最大似然估计值.

分析 多数情况下, 最大似然估计值可以由似然函数的驻点求得, 但是在有些情况下, 似然函数的驻点不存在, 此时, 可以通过参数的取值范围求最大似然估计.

解 由题意知, 似然函数为

$$
L\left( \theta \right)  = L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)  = \left\{  \begin{array}{ll} {2}^{n}{\mathrm{e}}^{-2\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{x}_{i} - \theta }\right) }, & {x}_{i} > \theta \left( {i = 1,2,\cdots, n}\right) \\  0, & \text{ 其他 } \end{array}\right.
$$

当 ${x}_{i} > 0$ 时, $L\left( \theta \right)  > 0$,两边取对数

$$
\ln L\left( \theta \right)  = n\ln 2 - 2\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{x}_{i} - \theta }\right),
$$

因为 $\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = {2n} > 0$,所以 $L\left( \theta \right)$ 单调增加.

由于 $\theta$ 要满足 $\theta  < {x}_{i}\left( {i = 1,2,\cdots, n}\right)$,所以当 $\theta$ 取 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 中的最小值时, $L\left( \theta \right)$ 取最大值.

故 $\theta$ 的最大似然估计值为 $\widehat{\theta } = \min \left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$.

【1.7】设总体 $X$ 的概率分布为

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$p$</td><td>${\theta }^{2}$</td><td>${2\theta }\left( {1 - \theta }\right)$</td><td>${\theta }^{2}$</td><td>$1 - {2\theta }$</td></tr></table>

其中 $\theta \left( {0 < \theta  < \frac{1}{2}}\right)$ 是未知参数,利用总体 $X$ 的如下样本值

3,1,3,0,3,1,2,3

求 $\theta$ 的矩估计值和最大似然估计值.

分析 矩估计用基本求解方法即可. 对于最大似然估计, 若似然函数出现多个驻点应该根据题意选择.

解 由离散型随机变量的期望公式

$$
{EX} = 0 \times  {\theta }^{2} + 1 \times  {2\theta }\left( {1 - \theta }\right)  + 2 \times  {\theta }^{2} + 3 \times  \left( {1 - {2\theta }}\right)
$$

$$
= {2\theta } - 2{\theta }^{2} + 2{\theta }^{2} + 3 - {6\theta } = 3 - {4\theta },
$$

令 ${EX} = \bar{X}$,而由样本观测值可得

$$
\bar{X} = \frac{1}{8}\left( {3 + 1 + 3 + 0 + 3 + 1 + 2 + 3}\right)  = \frac{1}{8} \times  {16} = 2,
$$

所以 $\theta$ 的矩估计值为

$$
\widehat{\theta } = \frac{1}{4}\left( {3 - \bar{X}}\right)  = \frac{1}{4}\left( {3 - 2}\right)  = \frac{1}{4}.
$$

根据题意, 似然函数为

$$
L\left( \theta \right)  = 4{\theta }^{6}{\left( 1 - \theta \right) }^{2}{\left( 1 - 2\theta \right) }^{4},
$$

两边取对数可得

$$
\ln L\left( \theta \right)  = \ln 4 + 6\ln \theta  + 2\ln \left( {1 - \theta }\right)  + 4\ln \left( {1 - {2\theta }}\right),
$$

$$
\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = \frac{6}{\theta } - \frac{2}{1 - \theta } - \frac{8}{1 - {2\theta }} = \frac{{24}{\theta }^{2} - {28\theta } + 6}{\theta \left( {1 - \theta }\right) \left( {1 - {2\theta }}\right) },
$$

令 $\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = 0$,得 ${12}{\theta }^{2} - {14\theta } + 3 = 0$,解之得 $\theta  = \frac{7 - \sqrt{13}}{12}$ 或 $\frac{7 + \sqrt{13}}{12}$.

因为已知 $0 < \theta  < \frac{1}{2}$,故 $\theta  = \frac{7 - \sqrt{13}}{12}$.

因此 $\theta$ 的最大似然估计值为 $\widehat{\theta } = \frac{7 - \sqrt{13}}{12}$.

【1.8】设总体 $X$ 的概率密度为

$$
f\left( {x;\theta }\right)  = \left\{  \begin{array}{ll} \theta, & 0 < x < 1 \\  1 - \theta, & 1 \leq  x < 2 \\  0, & \text{ 其他 } \end{array}\right.
$$

其中 $\theta$ 是未知参数 $\left( {0 < \theta  < 1}\right).{X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自总体 $X$ 的简单随机样本,记 $N$ 为样本值 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 中小于 1 的个数. 求

(1) $\theta$ 的矩估计;

(2) $\theta$ 的最大似然估计.

解 (1) 由于

$$
{EX} = {\int }_{-\infty }^{+\infty }{xf}\left( {x;\theta }\right) \mathrm{d}x = {\int }_{0}^{1}{\theta x}\mathrm{\;d}x + {\int }_{1}^{2}\left( {1 - \theta }\right) x\mathrm{\;d}x
$$

$$
= \frac{1}{2}\theta  + \frac{3}{2}\left( {1 - \theta }\right)  = \frac{3}{2} - \theta.
$$

令 $\frac{3}{2} - \theta  = \bar{X}$,解得 $\theta  = \frac{3}{2} - \bar{X}$,所以参数 $\theta$ 的矩估计为 $\widehat{\theta } = \frac{3}{2} - \bar{X}$.

(2)似然函数为

$$
L\left( \theta \right)  = \mathop{\prod }\limits_{{i = 1}}^{n}f\left( {{x}_{i};\theta }\right)  = {\theta }^{N}{\left( 1 - \theta \right) }^{n - N},
$$

取对数, 得

$$
\ln L\left( \theta \right)  = N\ln \theta  + \left( {n - N}\right) \ln \left( {1 - \theta }\right),
$$

两边对 $\theta$ 求导,得

$$
\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = \frac{N}{\theta } - \frac{n - N}{1 - \theta }.
$$

令 $\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = 0$,得 $\theta  = \frac{N}{n}$,

所以 $\theta$ 的最大似然估计为 $\widehat{\theta } = \frac{N}{n}$.

【1.9】设 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),{x}_{1},{x}_{2},\cdots,{x}_{n}$ 为一组样本值,求参数 $\mu,{\sigma }^{2}$ 的极大似然估计.

解 似然函数

$$
L\left( {\mu,{\sigma }^{2}}\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}\frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{\frac{{\left( {x}_{i} - \mu \right) }^{2}}{2{\sigma }^{2}}} = \frac{1}{{\left( \sqrt{2\pi }\sigma \right) }^{n}}{\mathrm{e}}^{\frac{\sum {\left( {x}_{i} - \mu \right) }^{2}}{2{\sigma }^{2}}},
$$

两边取对数得

$$
\ln L\left( {\mu,{\sigma }^{2}}\right)  =  - \frac{n}{2}\ln \left( {{2\pi }{\sigma }^{2}}\right)  - \frac{1}{2{\sigma }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \mu \right) }^{2},
$$

似然方程组为

$$
\left\{  \begin{array}{l} \frac{\partial }{\partial \mu }\ln L = \frac{1}{{\sigma }^{2}}\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} - {n\mu }}\right)  = 0, \\  \frac{\partial }{\partial {\sigma }^{2}}\ln L =  - \frac{n}{2{\sigma }^{2}} + \frac{1}{2{\left( {\sigma }^{2}\right) }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \mu \right) }^{2} = 0. \end{array}\right.
$$

由前一式解得 $\widehat{\mu } = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} = \bar{x}$,代入后一式得 ${\sigma }^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \bar{x}\right) }^{2}$. 因此得 $\mu,{\sigma }^{2}$ 的最大似然估计量为

$$
\widehat{\mu } = \bar{X},\;\widehat{{\sigma }^{2}} = {B}_{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}.
$$

它们与相应的矩估计量相同.

【1.10】设总体 $X$ 在 $\left\lbrack  {a, b}\right\rbrack$ 上服从均匀分布, $a, b$ 未知, ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 是一个样本值. 试求 $a$, $b$ 的最大似然估计量.

解 记 ${x}_{\left( 1\right) } = \min \left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right),{x}_{\left( n\right) } = \max \left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right).X$ 的概率密度是

$$
f\left( {x;a, b}\right)  = \left\{  \begin{array}{ll} \frac{1}{b - a}, & a \leq  x \leq  b \\  0, & \text{ 其他 } \end{array}\right.
$$

由于 $a \leq  {x}_{1},{x}_{2},\cdots,{x}_{n} \leq  b$,等价于 $a \leq  {x}_{\left( 1\right) },{x}_{\left( n\right) } \leq  b$. 似然函数为

$$
L\left( {a, b}\right)  = \frac{1}{{\left( b - a\right) }^{n}},\;a \leq  {x}_{\left( 1\right) }, b \geq  {x}_{\left( n\right) },
$$

于是对于满足条件 $a \leq  {x}_{\left( 1\right) }, b \geq  {x}_{\left( n\right) }$ 的任意 $a, b$ 有

$$
L\left( {a, b}\right)  = \frac{1}{{\left( b - a\right) }^{n}} \leq  \frac{1}{{\left( {x}_{\left( n\right) } - {x}_{\left( 1\right) }\right) }^{n}},
$$

即 $L\left( {a, b}\right)$ 在 $a = {x}_{\left( 1\right) }, b = {x}_{\left( n\right) }$ 时取到最大值 ${\left( {x}_{\left( n\right) } - {x}_{\left( 1\right) }\right) }^{-n}$. 故 $a, b$ 的最大似然估计值为

$$
\widehat{a} = {x}_{\left( 1\right) } = \min \underset{1 \leq  i \leq  n}{\mathrm{n}}{x}_{i},\;\widehat{b} = {x}_{\left( n\right) } = \max {x}_{i}.
$$

$a, b$ 的最大似然估计量为 $\widehat{a} = \min \underset{1 \leq  i \leq  n}{\mathrm{n}}{X}_{i},\;\widehat{b} = \max \underset{1 \leq  i \leq  n}{\mathrm{x}}{X}_{i}$.

【1.11】(1) 设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自概率密度为

$$
f\left( {x;\theta }\right)  = \left\{  \begin{array}{ll} \theta {x}^{\theta  - 1}, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

的总体样本, $\theta$ 未知,求 $U = {\mathrm{e}}^{-\frac{1}{\theta }}$ 的最大似然估计值.

(2)设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自正态总体 $N\left( {\mu,1}\right)$ 的样本. $\mu$ 未知,求 $\theta  = P\{ X > 2\}$ 的最大似然估计值.

解 (1) 先求 $\theta$ 的最大似然估计. 似然函数为

$$
L\left( \theta \right)  = \mathop{\prod }\limits_{{i = 1}}^{n}\theta {x}_{i}^{\theta  - 1} = {\theta }^{n}{\left( \mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}\right) }^{\theta  - 1},
$$

$$
\ln L\left( \theta \right)  = n\ln \theta  + \left( {\theta  - 1}\right) \ln \left( {\mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}}\right).
$$

令

$$
\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = \frac{n}{\theta } + \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i} = 0,
$$

得 $\theta$ 的最大似然估计值为

$$
\widehat{\theta } = \frac{-n}{\mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i}}.
$$

$U = {\mathrm{e}}^{-\frac{1}{\theta }}$ 具有单调反函数,故由最大似然估计的不变性知 $U$ 的最大似然估计值为

$$
\widehat{U} = {\mathrm{e}}^{-\frac{1}{\widehat{\theta }}} = {\mathrm{e}}^{\frac{\mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i}}{n}}.
$$

( 2 )已知 $\mu$ 的最大似然估计为 $\widehat{\mu } = \bar{x}$. 而 $\theta  = P\{ X > 2\}  = 1 - P\{ X \leq  2\}  = 1 - \Phi \left( {2 - \mu }\right)$ 具有单调反函数. 由最大似然估计的不变性得 $\theta  = P\{ X > 2\}$ 的最大似然估计值为

$$
\widehat{\theta } = 1 - \Phi \left( {2 - \widehat{\mu }}\right)  = 1 - \Phi \left( {2 - \bar{x}}\right).
$$

点评 最大似然估计的不变性:

如果 $\widehat{\theta }$ 是 $\theta$ 的最大似然估计,则对 $\theta$ 的任一函数 $g\left( \theta \right)$,其最大似然估计为 $g\left( \widehat{\theta }\right)$.

## $§2$. 估计量的评选标准

### 知识要点

#### 1. 无偏性

设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自总体 $X$ 的样本, $\widehat{\theta }$ 为 $\theta$ 的一个估计量,如果 $E\left( \widehat{\theta }\right)  = \theta$ 成立,则称估计量 $\widehat{\theta }$ 为参数 $\theta$ 的无偏估计.

#### 2. 有效性

设 ${\widehat{\theta }}_{1}\text{、}{\widehat{\theta }}_{2}$ 都为参数 $\theta$ 的无偏估计量,若 $D\left( {\widehat{\theta }}_{1}\right)  \leq  D\left( {\widehat{\theta }}_{2}\right)$,则称 ${\widehat{\theta }}_{1}$ 比 ${\widehat{\theta }}_{2}$ 有效.

特别地,若对于 $\theta$ 的任一无偏估计 $\widehat{\theta }$,有

$$
D\left( {\widehat{\theta }}_{1}\right)  \leq  D\left( \widehat{\theta }\right)
$$

则称 ${\widehat{\theta }}_{1}$ 是 $\theta$ 的最小方差无偏估计 (最佳无偏估计).

#### 3. 一致性

设 $\widehat{\theta }$ 为未知参数 $\theta$ 的估计量,若对任意给定的 $\varepsilon  > 0$,都有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\{ \left| {\widehat{\theta } - \theta }\right|  < \varepsilon \}  = 1,
$$

即 $\widehat{\theta }$ 依概率收敛于参数 $\theta$,则 $\widehat{\theta }$ 称为 $\theta$ 的一致估计或相合估计.


### 基本题型

#### 题型 1: 估计量的无偏性问题

【2.1】已知总体 $X$ 的期望 ${EX} = 0$,方差 ${DX} = {\sigma }^{2},{X}_{1},\cdots,{X}_{n}$ 为其简单样本,均值为 $\bar{X}$,方差为 ${S}^{2}$. 则 ${\sigma }^{2}$ 的无偏估计量为_____.

(A) $n{\bar{X}}^{2} + {S}^{2}$ (B) $\frac{1}{2}n{\bar{X}}^{2} + \frac{1}{2}{S}^{2}$

(C) $\frac{1}{3}n{\bar{X}}^{2} + {S}^{2}$ (D) $\frac{1}{4}n{\bar{X}}^{2} + \frac{1}{4}{S}^{2}$

解 由于

$$
E\bar{X} = {EX} = 0,\;E\left( {\bar{X}}^{2}\right)  = D\bar{X} + {\left( E\bar{X}\right) }^{2},\;D\bar{X} = \frac{{\sigma }^{2}}{n},\;E{S}^{2} = {\sigma }^{2},
$$

所以

$$
E\left( {n{\bar{X}}^{2} + {S}^{2}}\right)  = n \cdot  \frac{{\sigma }^{2}}{n} + {\sigma }^{2} = 2{\sigma }^{2}.
$$

则 $E\left( {\frac{1}{2}n{\bar{X}}^{2} + \frac{1}{2}{S}^{2}}\right)  = {\sigma }^{2}$,故 $\frac{1}{2}n{\bar{X}}^{2} + \frac{1}{2}{S}^{2}$ 为 ${\sigma }^{2}$ 无偏估计.

应选 (B).

【2.2】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是取自总体的样本,为了估计总体方差 ${\sigma }^{2}$,我们利用统计量

$$
\widehat{{\sigma }^{2}} = K\mathop{\sum }\limits_{{i = 1}}^{{n - 1}}{\left( {X}_{i + 1} - {X}_{i}\right) }^{2}
$$

则 $K =$ _____时, $\widehat{{\sigma }^{2}}$ 是 ${\sigma }^{2}$ 的无偏估计量.

解 由题意 $E\left( \widehat{{\sigma }^{2}}\right)  = {\sigma }^{2}$.

因为

$$
E{\left( {X}_{i + 1} - {X}_{i}\right) }^{2} = D\left( {{X}_{i + 1} - {X}_{i}}\right)  + {\left\lbrack  E\left( {X}_{i + 1} - {X}_{i}\right) \right\rbrack  }^{2}
$$

$$
= \left( {D{X}_{i + 1} + D{X}_{i}}\right)  + {\left( E{X}_{i + 1} - E{X}_{i}\right) }^{2} = \left( {{\sigma }^{2} + {\sigma }^{2}}\right)  + 0 = 2{\sigma }^{2},
$$

所以

$$
E\left( \widehat{{\sigma }^{2}}\right)  = K\mathop{\sum }\limits_{{i = 1}}^{{n - 1}}E{\left( {X}_{i + 1} - {X}_{i}\right) }^{2} = K\mathop{\sum }\limits_{{i = 1}}^{{n - 1}}2{\sigma }^{2} = {2K}\left( {n - 1}\right) {\sigma }^{2}.
$$

故 $K = \frac{1}{2\left( {n - 1}\right) }$.

【2.3】设样本 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 来自于参数为 $\lambda$ 的泊松分布.

试证明 $\bar{X}$ 与 ${S}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}$ 都是 $\lambda$ 的无偏估计,且对任一 $a$ 值, $0 \leq  a \leq  1$,统计量 $a\bar{X} + \left( {1 - a}\right) {S}^{2}$ 也是 $\lambda$ 的无偏估计.

证 因为总体 $X \sim  P\left( \lambda \right)$,故 $E\left( X\right)  = \lambda, D\left( X\right)  = \lambda$. 而

$$
E\left( \bar{X}\right)  = E\left( X\right)  = \lambda,\;E\left( {S}^{2}\right)  = D\left( X\right)  = \lambda,
$$

由无偏性定义, $\bar{X}$ 与 ${S}^{2}$ 都是 $\lambda$ 的无偏估计.

当 $0 \leq  a \leq  1$ 时,

$$
E\left\lbrack  {a\bar{X} + \left( {1 - a}\right) {S}^{2}}\right\rbrack   = {aE}\left( \bar{X}\right)  + \left( {1 - a}\right) E\left( {S}^{2}\right)  = {a\lambda } + \left( {1 - a}\right) \lambda  = \lambda.
$$

故 $a\bar{X} + \left( {1 - a}\right) {S}^{2}$ 也是 $\lambda$ 的无偏估计.

【2.4】已知总体 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{\theta }{\mathrm{e}}^{-\frac{x}{\theta }}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

其中未知参数 $\theta  > 0$. 设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为取自总体 $X$ 的一个样本,

(1)求 $\theta$ 的最大似然估计量；

(2)试问该估计量是否为无偏估计量？说明理由.

解 (1) 设 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 为相应于样本 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 的一个样本值,似然函数为

$$
L\left( \theta \right)  = \left\{  \begin{array}{ll} \frac{1}{{\theta }^{n}}{\mathrm{e}}^{-\frac{1}{\theta }\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}, & {x}_{1},{x}_{2},\cdots,{x}_{n} > 0, \\  0, & \text{ 其他 } \end{array}\right.
$$

当 ${x}_{1},{x}_{2},\cdots,{x}_{n} > 0$ 时,有

$$
\ln L\left( \theta \right)  =  - n\ln \theta  - \frac{1}{\theta }\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}.
$$

将上式对 $\theta$ 求导数并令其等于零,得

$$
\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } =  - \frac{n}{\theta } + \frac{1}{{\theta }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} = 0.
$$

解得 $\theta$ 的最大似然估计值为 $\widehat{\theta } = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} = \bar{x}$.

因此, $\theta$ 的最大似然估计量为 $\widehat{\theta } = \bar{X}$.

(2)由于

$$
E\left( \widehat{\theta }\right)  = E\left( \bar{X}\right)  = E\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E\left( {X}_{i}\right)  = E\left( X\right),
$$

而 $X$ 服从指数分布, $E\left( X\right)  = \theta$,所以 $E\left( \widehat{\theta }\right)  = \theta$,故 $\widehat{\theta } = \bar{X}$ 为未知参数 $\theta$ 的无偏估计量.

【2.5】设总体 $X$ 的概率密度为

$$
f\left( {x;\theta }\right)  = \left\{  \begin{array}{ll} \frac{1}{2\theta }, & 0 < x < \theta \\  \frac{1}{2\left( {1 - \theta }\right) }, & \theta  \leq  x < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

其中参数 $\theta \left( {0 < \theta  < 1}\right)$ 未知, ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体 $X$ 的简单随机样本, $\bar{X}$ 是样本均值.

(1)求参数 $\theta$ 的矩估计量 $\widehat{\theta }$;

(2)判断 $4{\bar{X}}^{2}$ 是否为 ${\theta }^{2}$ 的无偏估计量,并说明理由.

解 (1) ${EX} = {\int }_{-\infty }^{+\infty }{xf}\left( {x;\theta }\right) \mathrm{d}x = {\int }_{0}^{\theta }\frac{x}{2\theta }\mathrm{d}x + {\int }_{\theta }^{1}\frac{x}{2\left( {1 - \theta }\right) }\mathrm{d}x = \frac{1}{4} + \frac{\theta }{2}$.

令 $\bar{X} = {EX}$,即 $\bar{X} = \frac{1}{4} + \frac{\theta }{2}$,得 $\theta$ 的矩估计量为

$$
\widehat{\theta } = 2\bar{X} - \frac{1}{2}.
$$

(2)因为

$$
E\left( {4{\bar{X}}^{2}}\right)  = {4E}{\bar{X}}^{2} = 4\left\lbrack  {D\bar{X} + {\left( E\bar{X}\right) }^{2}}\right\rbrack
$$

$$
= 4\left\lbrack  {\frac{1}{n}{DX} + {\left( \frac{1}{4} + \frac{1}{2}\theta \right) }^{2}}\right\rbrack   = \frac{4}{n}{DX} + \frac{1}{4} + \theta  + {\theta }^{2},
$$

又 ${DX} \geq  0,\theta  > 0$,所以 $E\left( {4{\bar{X}}^{2}}\right)  > {\theta }^{2}$,即 $E\left( {4{\bar{X}}^{2}}\right)  \neq  {\theta }^{2}$,

因此 $4{\bar{X}}^{2}$ 不是 ${\theta }^{2}$ 的无偏估计量.

题型2:估计量的有效性问题

【2.6】设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),{X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自总体 $X$ 的样本,当用 $2\bar{X} - {X}_{1},\bar{X}$ 及 $\frac{1}{2}{X}_{1}$ $+ \frac{2}{3}{X}_{2} - \frac{1}{6}{X}_{3}$ 作为 $\mu$ 的估计时,最有效的是哪个估计量?

分析 先验证估计量是否是无偏估计量,再根据有效性的定义判断有效性.

解 由无偏性的定义

$$
E\left( {2\bar{X} - {X}_{1}}\right)  = {2E}\bar{X} - E{X}_{1} = {2\mu } - \mu  = \mu,
$$

$$
E\bar{X} = \mu,
$$

$$
E\left( {\frac{1}{2}{X}_{1} + \frac{2}{3}{X}_{2} - \frac{1}{6}{X}_{3}}\right)  = \frac{1}{2}\mu  + \frac{2}{3}\mu  - \frac{1}{6}\mu  = \mu,
$$

可知 $2\bar{X} - {X}_{1},\bar{X}$ 与 $\frac{1}{2}{X}_{1} + \frac{2}{3}{X}_{2} - \frac{1}{6}{X}_{3}$ 均是 $\mu$ 的无偏估计量.

$$
D\left( {2\bar{X} - {X}_{1}}\right)  = D\left( {\frac{2}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - {X}_{1}}\right)  = D\left\lbrack  {\left( {\frac{2}{n} - 1}\right) {X}_{1} + \frac{2}{n}\mathop{\sum }\limits_{{i = 2}}^{n}{X}_{i}}\right\rbrack
$$

$$
= {\left( \frac{2 - n}{n}\right) }^{2}D{X}_{1} + {\left( \frac{2}{n}\right) }^{2}\mathop{\sum }\limits_{{i = 2}}^{n}D{X}_{i}
$$

$$
= \frac{1}{{n}^{2}}\left\lbrack  {{\left( 2 - n\right) }^{2}{\sigma }^{2} + 4\left( {n - 1}\right) {\sigma }^{2}}\right\rbrack   = {\sigma }^{2},
$$

$$
D\bar{X} = \frac{{\sigma }^{2}}{n},
$$

$$
D\left( {\frac{1}{2}{X}_{1} + \frac{2}{3}{X}_{2} - \frac{1}{6}{X}_{3}}\right)  = \left( {\frac{1}{4}D{X}_{1} + \frac{4}{9}D{X}_{2} + \frac{1}{36}D{X}_{3}}\right)  = \frac{13}{18}{\sigma }^{2}.
$$

经过比较可知 $D\bar{X}$ 最小,因此 $\bar{X}$ 是最有效的估计量.

【2.7】设总体 $X$ 的样本是 ${X}_{1},{X}_{2},\cdots,{X}_{n}$,试证明:

(1) $\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}{X}_{i}\left( {{a}_{i} > 0, i = 1,2,\cdots, n,\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i} = 1}\right)$ 是 $E\left( X\right)$ 的无偏估计量;

( 2 )在 $E\left( X\right)$ 的所有形如 $\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}{X}_{i}$ 的无偏估计量中, $\bar{X}$ 为最有效的估计.

分析 证明估计量的有效性时, 需要证明不等式成立, 因此采用 Cauchy - Schwarz 公式是很有效的方法

证 (1) 根据无偏性估计的定义有

$$
E\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}{X}_{i}}\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}E\left( {X}_{i}\right)  = E\left( X\right) \mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i} = E\left( X\right),
$$

故 $\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}{X}_{i}$ 是 $E\left( X\right)$ 的无偏估计量.

(2)由样本均值的性质可知

$$
E\left( \bar{X}\right)  = \frac{1}{n}E\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} = {EX},
$$

因此 $\bar{X}$ 也是 $E\left( X\right)$ 的无偏估计量.

又由 Cauchy- Schwarz 不等式

$$
{\left( \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}{y}_{i}\right) }^{2} \leq  \left( {\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}^{2}}\right) \left( {\mathop{\sum }\limits_{{i = 1}}^{n}{y}_{i}^{2}}\right),
$$

令 ${x}_{i} = {a}_{i},{y}_{i} = 1$,则

$$
{\left( \mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}\right) }^{2} = 1 \leq  n\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}^{2},
$$

故

$$
D\left( \bar{X}\right)  = \frac{1}{n}D\left( X\right)  = \frac{1}{n}D\left( X\right) {\left( \mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}\right) }^{2}
$$

$$
\leq  D\left( X\right) \left( {\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}^{2}}\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}D\left( {{a}_{i}{X}_{i}}\right)  = D\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}{X}_{i}}\right).
$$

证毕.

点评 本题也可以用导数知识求 $\mathop{\sum }\limits_{{i = 1}}^{n}{a}_{i}^{2}$ 的最小值,从而得出结论. 另外本题的结论可以记住并当作定理应用, 见下面例题.

【2.8】设 $\left( {{X}_{1},{X}_{2},{X}_{3}}\right)$ 是来自总体 $X$ 的一个简单样本,则在下列 ${EX}$ 的估计量中,最有效的估计量是(   ).

(A) $\frac{1}{4}\left( {{X}_{1} + 2{X}_{2} + {X}_{3}}\right)$ (B) $\frac{1}{3}\left( {{X}_{1} + {X}_{2} + {X}_{3}}\right)$

(C) $\frac{1}{5}\left( {{X}_{1} + 3{X}_{2} + {X}_{3}}\right)$ (D) $\frac{1}{5}\left( {2{X}_{1} + 2{X}_{2} + {X}_{3}}\right)$

解 可以将 4 个选项中统计量的方差求出,经比较,(B) 中统计量 $\bar{X}$ 的方差 $\frac{D\left( X\right) }{3}$ 为最小, 故最有效.

也可以直接利用上题的结论, 选择 (B).

#### 题型 3:估计量的相合性(一致性)问题

方法与技巧 相合性的证明一般有两种方法:

方法一 利用定义证明, 往往需要结合大数定律;

方法二 利用定理证明, 结论如下:

设 ${\widehat{\theta }}_{n}$ 是 $\theta$ 的一个估计量,若

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}E\left( {\widehat{\theta }}_{n}\right)  = \theta,\;\mathop{\lim }\limits_{{n \rightarrow  \infty }}D\left( {\widehat{\theta }}_{n}\right)  = 0,
$$

则 ${\widehat{\theta }}_{n}$ 是 $\theta$ 的相合估计.

【2.9】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是取自正态总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 的样本,证明 ${S}^{2}$ 是 ${\sigma }^{2}$ 的一致估计.

证法一 由大数定律

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\left| {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \mu }\right|  < \varepsilon }\right\}   = 1,
$$

所以 $\bar{X}$ 是 $\mu$ 的一致估计.

同理,因 ${X}_{1}^{2},{X}_{2}^{2},\cdots,{X}_{n}^{2}$ 也独立同分布,故 $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 是 $E\left( {X}^{2}\right)$ 的一致估计.

而

$$
{S}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} = \frac{n}{n - 1}\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - {\bar{X}}^{2}}\right),
$$

故当 $n \rightarrow  \infty$ 时,

$$
\frac{n}{n - 1} \rightarrow  1,\;\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}\overset{P}{ \rightarrow  }E\left( {X}^{2}\right),\;{\bar{X}}^{2}\overset{P}{ \rightarrow  }{\mu }^{2},
$$

即 ${S}^{2}\overset{P}{ \rightarrow  }E\left( {X}^{2}\right)  - {\mu }^{2} = {\sigma }^{2}$. 则 ${S}^{2}$ 是 ${\sigma }^{2}$ 的一致估计.

证法二 因为 $E\left( {S}^{2}\right)  = {\sigma }^{2}, D\left( {S}^{2}\right)  = \frac{2{\sigma }^{4}}{n - 1}$,故

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}E\left( {S}^{2}\right)  = {\sigma }^{2},\;\mathop{\lim }\limits_{{n \rightarrow  \infty }}D\left( {S}^{2}\right)  = \mathop{\lim }\limits_{{n \rightarrow  \infty }}\frac{2{\sigma }^{4}}{n - 1} = 0,
$$

由定理可知, ${S}^{2}$ 是 ${\sigma }^{2}$ 的一致估计.

## §3. 区间估计

### 知识要点

#### 1. 区间估计

设 $\theta$ 为总体的未知参数, ${\widehat{\theta }}_{1}$ 和 ${\widehat{\theta }}_{2}$ 均为估计量,若对于给定的 $\alpha \left( {0 < \alpha  < 1}\right)$,满足 $P\left\{  {{\widehat{\theta }}_{1} \leq  \theta }\right.$ $\left. { \leq  {\widehat{\theta }}_{2}}\right\}   = 1 - \alpha$,则称 $\left\lbrack  {{\widehat{\theta }}_{1},{\widehat{\theta }}_{2}}\right\rbrack$ 为 $\theta$ 的置信度为 $1 - \alpha$ 的置信区间. 通过构造一个置信区间对未知参数进行估计的方法称为区间估计.

#### 2. 单个正态总体的区间估计

设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自 $N\left( {\mu,{\sigma }^{2}}\right)$ 的样本,则

(1)当 ${\sigma }^{2}$ 已知时, $\mu$ 的置信度为 $1 - \alpha$ 的置信区间为

$$
\left\lbrack  {\bar{X} - \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}},\;\bar{X} + \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}}}\right\rbrack .
$$

(2)当 ${\sigma }^{2}$ 未知时, $\mu$ 的置信度为 $1 - \alpha$ 的置信区间为

$$
\left\lbrack  {\bar{X} - \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right),\;\bar{X} + \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right) }\right\rbrack .
$$

(3)当 $\mu$ 已知时, ${\sigma }^{2}$ 的置信度为 $1 - \alpha$ 的置信区间为

$$
\left\lbrack  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( n\right) },\;\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right) }}\right\rbrack .
$$

(4)当 $\mu$ 未知时, ${\sigma }^{2}$ 的置信度为 $1 - \alpha$ 的置信区间为

$$
\left\lbrack  {\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) },\;\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}\right\rbrack .
$$

#### 3. 双正态总体的区间估计

设 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right),{X}_{1},{X}_{2},\cdots,{X}_{{n}_{1}}$ 为其样本, $Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right),{Y}_{1},{Y}_{2},\cdots,{Y}_{{n}_{2}}$ 为其样本,且 $X$ 与 $Y$ 独立.

(1) ${\sigma }_{1}^{2}$, ${\sigma }_{2}^{2}$ 都为已知: ${\mu }_{1} - {\mu }_{2}$ 的 $1 - \alpha$ 置信区间为

$$
\left\lbrack  {\bar{X} - \bar{Y} - {u}_{\frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{{n}_{1}} + \frac{{\sigma }_{2}^{2}}{{n}_{2}}},\bar{X} - \bar{Y} + {u}_{\frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{{n}_{1}} + \frac{{\sigma }_{2}^{2}}{{n}_{2}}}}\right\rbrack .
$$

(2) ${\sigma }_{1}^{2}$, ${\sigma }_{2}^{2}$ 都未知: ${\mu }_{1} - {\mu }_{2}$ 的 $1 - \alpha$ 置信区间为

$$
\left\lbrack  {\bar{X} - \bar{Y} - {t}_{\frac{\alpha }{2}}\left( \gamma \right) \sqrt{\frac{{S}_{1}^{2}}{{n}_{1}} + \frac{{S}_{2}^{2}}{{n}_{2}}},\;\bar{X} - \bar{Y} + {t}_{\frac{\alpha }{2}}\left( \gamma \right) \sqrt{\frac{{S}_{1}^{2}}{{n}_{1}} + \frac{{S}_{2}^{2}}{{n}_{2}}}}\right\rbrack .
$$

其中 $\gamma  = \left\lbrack  \frac{{\left( \frac{{S}_{1}^{2}}{{n}_{1}} + \frac{{S}_{2}^{2}}{{n}_{2}}\right) }^{2}}{\frac{{\left( \frac{{S}_{1}^{2}}{{n}_{1}}\right) }^{2}}{{n}_{1} - 1} + \frac{{\left( \frac{{S}_{2}^{2}}{{n}_{2}}\right) }^{2}}{{n}_{2} - 1}}\right\rbrack$ (取整).

特殊情形:

① ${\sigma }_{1}^{2},{\sigma }_{2}^{2}$ 未知,但 ${n}_{1},{n}_{2}$ 较大时: ${\mu }_{1} - {\mu }_{2}$ 的 $1 - \alpha$ 置信区间为

$$
\left\lbrack  {\bar{X} - \bar{Y} - {u}_{\frac{\alpha }{2}}\sqrt{\frac{{S}_{1}^{2}}{{n}_{1}} + \frac{{S}_{2}^{2}}{{n}_{2}}},\;\bar{X} - \bar{Y} + {u}_{\frac{\alpha }{2}}\sqrt{\frac{{S}_{1}^{2}}{{n}_{1}} + \frac{{S}_{2}^{2}}{{n}_{2}}}}\right\rbrack .
$$

② ${\sigma }_{1}^{2} = {\sigma }_{2}^{2} = {\sigma }^{2}$ 未知: ${\mu }_{1} - {\mu }_{2}$ 的 $1 - \alpha$ 置信区间为

$$
\left\lbrack  {\bar{X} - \bar{Y} - {t}_{\frac{\alpha }{2}}{S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}},\;\bar{X} - \bar{Y} + {t}_{\frac{\alpha }{2}}{S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}}\right\rbrack ,
$$

其中 ${S}_{w}^{2} = \frac{\left( {{n}_{1} - 1}\right) {S}_{1}^{2} + \left( {{n}_{2} - 1}\right) {S}_{2}^{2}}{{n}_{1} + {n}_{2} - 2}, t$ 分布为 $t\left( {{n}_{1} + {n}_{2} - 2}\right)$.

(3) ${\mu }_{1},{\mu }_{2}$ 已知: $\frac{{\sigma }_{1}^{2}}{{\sigma }_{2}^{2}}$ 的 $1 - \alpha$ 置信区间为

$$
\left\lbrack  {\frac{\frac{1}{{n}_{1}}\mathop{\sum }\limits_{{i = 1}}^{{n}_{1}}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{\frac{1}{{n}_{2}}\mathop{\sum }\limits_{{j = 1}}^{{n}_{2}}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}}{F}_{1 - \frac{\alpha }{2}}\left( {{n}_{2},{n}_{1}}\right),\;\frac{\frac{1}{{n}_{1}}\mathop{\sum }\limits_{{i = 1}}^{{n}_{1}}{\left( {X}_{i} - {\mu }_{1}\right) }^{2}}{\frac{1}{{n}_{2}}\mathop{\sum }\limits_{{j = 1}}^{{n}_{2}}{\left( {Y}_{j} - {\mu }_{2}\right) }^{2}}{F}_{\frac{\alpha }{2}}\left( {{n}_{2},{n}_{1}}\right) }\right\rbrack .
$$

(4) ${\mu }_{1},{\mu }_{2}$ 未知: $\frac{{\sigma }_{1}^{2}}{{\sigma }_{2}^{2}}$ 的 $1 - \alpha$ 置信区间为

$$
\left\lbrack  {\frac{{S}_{1}^{2}}{{S}_{2}^{2}}{F}_{1 - \frac{\alpha }{2}}\left( {{i}_{2} - 1,{n}_{1} - 1}\right),\;\frac{{S}_{1}^{2}}{{S}_{2}^{2}}{F}_{\frac{\alpha }{2}}\left( {{n}_{2} - 1,{n}_{1} - 1}\right) }\right\rbrack .
$$

#### 4. $\left( {0 - 1}\right)$ 分布参数的区间估计

设总体 $X \sim  \left( {0 - 1}\right)$ 分布, $P\{ X = 1\}  = p, P\{ X = 0\}  = 1 - p,{X}_{1},{X}_{2},\cdots,{X}_{n}\left( {n \geq  {50}}\right)$ 为其样本,则 $p$ 的 $1 - \alpha$ 置信区间为

$$
\left\lbrack  {\bar{X} - {u}_{\frac{\alpha }{2}}\sqrt{\frac{\bar{X}\left( {1 - \bar{X}}\right) }{n}},\bar{X} + {u}_{\frac{\alpha }{2}}\sqrt{\frac{\bar{X}\left( {1 - \bar{X}}\right) }{n}}}\right\rbrack .
$$

#### 5. 单侧置信区间

设 $\theta$ 为总体的未知参数,对于给定值 $\alpha \left( {0 < \alpha  < 1}\right)$,若 $P\{ \theta  \geq  \underline{\theta }\}  = 1 - \alpha$,则称 $\lbrack \underline{\theta }, + \infty )$ 为 $\theta$ 的满足置信度 $1 - \alpha$ 的单侧置信区间, $\theta$ 称为单侧置信下限. 若 $P\{ \theta  \leq  \bar{\theta }\}  = 1 - \alpha$,则称 $( - \infty,\bar{\theta }\rbrack$ 为 $\theta$ 的满足置信度 $1 - \alpha$ 的单侧置信区间, $\bar{\theta }$ 称为单侧置信上限.

例如,对于正态分布 $N\left( {\mu,{\sigma }^{2}}\right),{\sigma }^{2}$ 未知,可得 $\mu$ 的置信水平为 $1 - \alpha$ 的单侧置信区间为

① $\left( {-\infty,\bar{X} + {t}_{\alpha }\left( {n - 1}\right) \frac{S}{\sqrt{n}}}\right)$,单侧置信上限为 $\bar{\mu } = \bar{X} + {t}_{\alpha }\left( {n - 1}\right) \frac{S}{\sqrt{n}}$.

② $\left( {\bar{X} - {t}_{\alpha }\left( {n - 1}\right) \frac{S}{\sqrt{n}}, + \infty }\right)$,单侧置信下限为 $\underline{\mu } = \bar{X} - {t}_{\alpha }\left( {n - 1}\right) \frac{S}{\sqrt{n}}$.

也即只需将双侧置信区间的上下限中的“ $\frac{\alpha }{2}$ ” 改成“ $\alpha$ ”,就得到相应的单侧置信上下限了.

### 基本题型

方法与技巧 求未知参数的置信区间是区间估计的基本内容, 常用方法如下:

 (1)一般方法

① 寻求一个样本 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 的函数 (枢轴变量)

$$
W = W\left( {{X}_{1},{X}_{2},\cdots,{X}_{n};\theta }\right)
$$

它包含待估参数 $\theta$,而不含其他未知参数,并且 $W$ 的分布已知且不依赖于任何未知参数(当然不依赖于待估参数 $\theta$ );

② 对于给定的置信水平 $1 - \alpha$,定出两个常数 $a, b$,使

$$
P\left\{  {a < W\left( {{X}_{1},{X}_{2},\cdots,{X}_{n};\theta }\right)  < b}\right\}   = 1 - \alpha;
$$

③ 若能从 $a < W\left( {{X}_{1},{X}_{2},\cdots,{X}_{n};\theta }\right)  < b$ 得到等价的不等式 $\underline{\theta } < \theta  < \bar{\theta }$,其中

$$
\underline{\theta } = \underline{\theta }\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right),\;\bar{\theta } = \bar{\theta }\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)
$$

都是统计量,那么 $\left( {\underline{\theta },\bar{\theta }}\right)$ 就是 $\theta$ 的一个置信水平为 $1 - \alpha$ 的置信区间.

函数 $W\left( {{X}_{1},{X}_{2},\cdots,{X}_{n};\theta }\right)$ 的构造,通常可以从 $\theta$ 的点估计着手考虑. 常用的正态总体参数的置信区间可以用上述步骤推得.

(2)正态总体参数的置信区间

利用一般方法推出了参数的置信区间公式, 针对具体题目, 可以分清类型, 代入公式计算.

(3)非正态总体参数的置信区间

情形比较复杂, 一般采用大样本, 利用中心极限定理近似视为正态分布, 借用正态总体的某些特殊结论.

题型 1: 正态总体参数 $\mu$ 的区间估计

【3.1】设由来自正态总体 $X \sim  N\left( {\mu,{0.9}^{2}}\right)$ 容量为 9 的简单随机样本,得样本均值 $\bar{X} = 5$,则未知参数 $\mu$ 的置信度为 0.95 的置信区间是_____.

分析 本题是一个正态总体在方差已知的情况下求期望值 $\mu$ 的置信区间的问题,由公式

$$
\left\lbrack  {\bar{X} - \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}},\bar{X} + \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}}}\right\rbrack
$$

求解该置信区间.

解 由置信度 $1 - \alpha  = {0.95}$ 可得 $\alpha  = {0.05}$.

查 $N\left( {0,1}\right)$ 分布表得到 ${u}_{0.025} = {1.96}$.

代入 $\bar{X} = 5, n = 9,\sigma  = {0.9}$ 得

$$
\left\lbrack  {5 - \frac{0.9}{\sqrt{9}} \times  {1.96},\;5 + \frac{0.9}{\sqrt{9}} \times  {1.96}}\right\rbrack ,
$$

因此参数 $\mu$ 置信度 0.95 的置信区间为 $\left\lbrack  {{4.412},{5.588}}\right\rbrack$.

【3.2】设一批零件的长度服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$,其中 $\mu,{\sigma }^{2}$ 均未知,现从中随机抽取 16 个零件,测得样本均值 $\bar{x} = {20}\left( \mathrm{\;{cm}}\right)$,样本标准差 $s = 1\left( \mathrm{\;{cm}}\right)$. 则 $\mu$ 的置信度为 0.90 的置信区间是 (   ).

(A) $\left( {{20} - \frac{1}{4}{t}_{0.05}\left( {16}\right),{20} + \frac{1}{4}{t}_{0.05}\left( {16}\right) }\right)$

(B) $\left( {{20} - \frac{1}{4}{t}_{0.1}\left( {16}\right),{20} + \frac{1}{4}{t}_{0.1}\left( {16}\right) }\right)$

(C) $\left( {{20} - \frac{1}{4}{t}_{0.05}\left( {15}\right),{20} + \frac{1}{4}{t}_{0.05}\left( {15}\right) }\right)$

(D) $\left( {{20} - \frac{1}{4}{t}_{0.1}\left( {15}\right),{20} + \frac{1}{4}{t}_{0.1}\left( {15}\right) }\right)$

解 经过分析本题属于在方差未知情况下求一个正态总体期望的置信区间, 其公式为

$$
\left( {\bar{X} - \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right),\;\bar{X} + \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right) }\right).
$$

根据题意 $\bar{x} = {20}, s = 1, n = {16},\frac{\alpha }{2} = {0.05}$,代入公式.

可知应选(C).

【3.3】设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,已知 ${\sigma }^{2}$. 则样本容量 $n$ 至少为_____时,才能保证 $\mu$ 的置信度 $1 - \alpha$ 的置信区间长度不大于 $d$.

解 因为 $\mu$ 的置信区间为

$$
\left\lbrack  {\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}},\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}}\right\rbrack
$$

所以区间长度为 $2{u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}$,则 $2{u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}} \leq  d$,故 $n \geq  {\left( \frac{2{u}_{\frac{\alpha }{2}}\sigma }{d}\right) }^{2}$.

【3.4】从总体 ${X}_{1} \sim  N\left( {{\mu }_{1},{25}}\right)$ 中取出一容量为 ${n}_{1} = {10}$ 的样本,其样本均值 ${\bar{X}}_{1} = {19.8}$; 从总体 ${X}_{2} \sim  N\left( {{\mu }_{2},{36}}\right)$ 中取出容量为 ${n}_{2} = {12}$ 的样本,其样本均值 ${\bar{X}}_{2} = {24.0}$,已知两个样本之间相互独立,求 ${\mu }_{1} - {\mu }_{2}$ 的 0.90 置信区间.

解 这是 ${\sigma }_{1}^{2},{\sigma }_{2}^{2}$ 都为已知时,求均值差的区间估计问题.

由于 $1 - \alpha  = {0.90}$,故 $\frac{\alpha }{2} = {0.05},{u}_{\frac{\alpha }{2}} = {1.645}$,

又因为 ${n}_{1} = {10},{n}_{2} = {12},{\sigma }_{1}^{2} = {25},{\sigma }_{2}^{2} = {36}$,所以

$$
\sqrt{\frac{{\sigma }_{1}^{2}}{{n}_{1}} + \frac{{\sigma }_{2}^{2}}{{n}_{2}}} = \sqrt{\frac{25}{10} + \frac{36}{12}} = \sqrt{5.5} = {2.345},
$$

$$
{\bar{X}}_{1} - {\bar{X}}_{2} - {u}_{\frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{{n}_{1}} + \frac{{\sigma }_{2}^{2}}{{n}_{2}}} = {19.8} - {24.0} - {1.645} \times  {2.345}
$$

$$
=  - {4.2} - {3.858} =  - {8.06}\text{,}
$$

$$
{\bar{X}}_{1} - {\bar{X}}_{2} + {u}_{\frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{{n}_{1}} + \frac{{\sigma }_{2}^{2}}{{n}_{2}}} =  - {4.2} + {3.858} =  - {0.34}.
$$

因此,所求的 ${\mu }_{1} - {\mu }_{2}$ 的 0.90 置信区间为 $\left\lbrack  {-{8.06}, - {0.34}}\right\rbrack$.

【3.5】设有甲、乙两种安眠药,随机变量 $X, Y$ 分别表示患者服用甲、乙药后睡眠时间的延长数,并假设 $X \sim  N\left( {{\mu }_{1},{\sigma }^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }^{2}}\right)$. 为比较两种药品的疗效,随机地从服用甲药的患者中选取 10 人,从服用乙药的患者中选取 10 人,分别测得睡眠延长时间的均值与方差: $\overline{X} = {2.33},{S}_{1}^{2}$ $= {\left( {1.9}\right) }^{2};\bar{Y} = {0.75},{S}_{2}^{2} = {\left( {28.9}\right) }^{2}$. 试求方差未知情况下 ${\mu }_{1} - {\mu }_{2}$ 的 ${95}\%$ 置信区间.

解 两正态总体的方差未知但相等,小样本,取

$$
T = \frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}} \sim  t\left( {{n}_{1} + {n}_{2} - 2}\right) \;\text{(这里}{n}_{1} = {n}_{2} = {10}\text{),}
$$

$$
P\left\{  {\left| T\right|  < {t}_{\frac{\alpha }{2}}\left( {18}\right) }\right\}   = 1 - \alpha \;\left( {\alpha  = {0.05}}\right),
$$

查得 ${t}_{0.025}\left( {18}\right)  = {2.101}$. 于是算得置信下限、上限分别为

$$
\left( {\bar{x} - \bar{y}}\right)  - {t}_{0.025}\left( {18}\right)  \cdot  {S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}
$$

$$
= \left( {{2.33} - {0.75}}\right)  - {2.101} \times  \sqrt{\frac{{36.1} + {28.9}}{18}} \times  \sqrt{\frac{2}{10}}
$$

$$
= {1.58} - {1.78} =  - {0.20}\text{,}
$$

$$
\left( {\bar{x} - \bar{y}}\right)  + {t}_{0.025}\left( {18}\right)  \cdot  {S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}} = {1.58} + {1.78} = {3.36}.
$$

从而得 ${\mu }_{1} - {\mu }_{2}$ 的 ${95}\%$ 置信区间为 $\left( {-{0.20},{3.36}}\right)$.

【3.6】为研究正常成年男、女血液红细胞的平均数的差别, 检查某地正常成年男子 156 名, 正常成年女子 74 名,计算得男性红细胞平均数为 465.13 万 $/{\mathrm{{mm}}}^{3}$,样本标准差为 54.80 万 $/{\mathrm{{mm}}}^{3}$; 女子红细胞平均数为 422.16 万 $/{\mathrm{{mm}}}^{3}$,样本标准差为 49.20 万 $/{\mathrm{{mm}}}^{3}$. 试问能否以 95% 的把握判定男子血红细胞均值高于女子血红细胞均值?

解 设正常成年男女血红细胞数构成的两个总体为 $X, Y$,则 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right), Y \sim  N\left( {\mu }_{2}\right.$, $\left. {\sigma }_{2}^{2}\right)$, $X$ 与 $Y$ 独立,由 $1 - \alpha  = {0.95}$,得 $\alpha  = {0.05}$, ${u}_{\frac{\alpha }{2}} = {1.96}$,又 ${n}_{1} = {156},{n}_{2} = {74}$, $\bar{x} = {465.13}$, $\bar{y} = {422.16},{s}_{1} = {54.80},{s}_{2} = {49.20}$. 虽然 ${\sigma }_{1}^{2},{\sigma }_{2}^{2}$ 未知,但因为两组样本都属于大样本,故 ${\sigma }_{1}^{2} \approx  {s}_{1}^{2}$, ${\sigma }_{2}^{2} \approx  {s}_{2}^{2}$. 则 ${\mu }_{1} - {\mu }_{2}$ 的置信限为: $\left( {\bar{X} - \bar{Y}}\right)  \pm  {u}_{\frac{\alpha }{2}}\sqrt{\frac{{S}_{1}^{2}}{{n}_{1}} + \frac{{S}_{2}^{2}}{{n}_{2}}}$.

代入数值:

$$
\left( {\bar{x} - \bar{y}}\right)  - {u}_{\frac{\alpha }{2}}\sqrt{\frac{{s}_{1}^{2}}{{n}_{1}} + \frac{{s}_{2}^{2}}{{n}_{2}}} \approx  {28.04},\;\left( {\bar{x} - \bar{y}}\right)  + {u}_{\frac{\alpha }{2}}\sqrt{\frac{{s}_{1}^{2}}{{n}_{1}} + \frac{{s}_{2}^{2}}{{n}_{2}}} \approx  {57.1},
$$

因此, ${\mu }_{1} - {\mu }_{2}$ 的 95 % 置信区间为 $\left\lbrack  {{28.04},{57.1}}\right\rbrack$.

因置信下限 28.04>0,从而 ${\mu }_{1} > {\mu }_{2}$,所以有 95% 的把握判定男性血红细胞均值高于女性血红细胞均值.

题型2: 正态总体参数 ${\sigma }^{2}$ 的区间估计

【3.7】若在某学校中, 随机抽取 25 名同学测量身高数据, 假设所测身高近似服从正态分布, 算得平均高为 ${170}\mathrm{\;{cm}}$,标准差为 ${12}\mathrm{\;{cm}}$,试求该班学生身高标准差 $\sigma$ 的 0.95 置信区间.

分析 根据题意分析,本题属于正态总体 $\mu$ 未知,求方差 ${\sigma }^{2}$ 的区间估计,其置信区间公式为

$$
\left( {\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) },\;\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}\right).
$$

解 取统计量

$$
{\chi }^{2} = \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right),
$$

根据 $P\left\{  {{\chi }^{2} > {\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) }\right\}   = P\left\{  {{\chi }^{2} < {\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }\right\}   = \frac{\alpha }{2}$.

经过查 ${\chi }^{2}$ 分布表,得 $\;{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right)  = {\chi }_{0.975}^{2}\left( {24}\right)  = {12.401}$,

$$
{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right)  = {\chi }_{0.025}^{2}\left( {24}\right)  = {39.364},
$$

因此参数 ${\sigma }^{2}$ 的置信度为 $1 - \alpha  = {0.95}$ 的置信区间为

$$
\left( {\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) },\;\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}\right)  = \left( {{87.80},{278.69}}\right),
$$

故 $\sigma$ 的 0.95 的置信区间为 $\left( {\sqrt{87.80},\sqrt{278.69}}\right)  \approx  \left( {{9.34},{16.69}}\right)$.

【3.8】冷抽铜丝的折断力服从正态分布. 从一批铜丝中任取 10 根,测试折断力,得数据(单位:kg)如下:

$$
{578},{572},{570},{568},{572},{570},{570},{596},{584},{572}
$$

求方差 ${\sigma }^{2}$ 和标准差 $\sigma$ 的 ${90}\%$ 的置信区间.

解 $\bar{X} = \frac{1}{10}\left( {{578} + {572} + {570} + {568} + {572} + {570} + {570} + {596} + {584} + {572}}\right)  = {575.2}$,

$$
{S}^{2} = \frac{1}{{10} - 1}\left\lbrack  {{\left( {578} - {575.2}\right) }^{2} + {\left( {572} - {575.2}\right) }^{2} + {\left( {570} - {575.2}\right) }^{2} + {\left( {568} - {575.2}\right) }^{2}}\right.
$$

$$
+ {\left( {572} - {575.2}\right) }^{2} + {\left( {570} - {575.2}\right) }^{2} + {\left( {570} - {575.2}\right) }^{2} + {\left( {596} - {575.2}\right) }^{2}
$$

$$
\left. {+{\left( {584} - {575.2}\right) }^{2} + {\left( {572} - {575.2}\right) }^{2}}\right\rbrack
$$

$$
= {75.73}\text{,}
$$

查 ${\chi }^{2}$ 分布表得

$$
{\chi }_{\frac{\alpha }{2}}^{2}\left( 9\right)  = {\chi }_{0.05}^{2}\left( 9\right)  = {16.919},\;{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( 9\right)  = {\chi }_{0.95}^{2}\left( 9\right)  = {3.325}\text{,}
$$

故

$$
\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( 9\right) } = \frac{9 \times  {75.73}}{16.919} = {40.28},\;\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( 9\right) } = \frac{9 \times  {75.73}}{3.325} = {204.98},
$$

于是得 ${\sigma }^{2}$ 的 ${90}\%$ 的置信区间为 $\left\lbrack  {{40.28},{240.98}}\right\rbrack .\sigma$ 的 ${90}\%$ 置信区间为 $\left\lbrack  {{6.35},{14.32}}\right\rbrack$.

【3.9】两个正态总体 $N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right) \text{、}N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$ 的参数均未知,分别从两个总体中抽取容量为 25 和 15 的两个独立样本,测得样本方差分别为 6.38,5.15,求 $\frac{{\sigma }_{1}^{2}}{{\sigma }_{2}^{2}}$ 的置信区间 $\left( {\alpha  = {0.10}}\right)$.

解 ${n}_{1} = {25},{S}_{1}^{2} = {6.38},{n}_{2} = {15},{S}_{2}^{2} = {5.15},\alpha  = {0.10},\frac{\alpha }{2} = {0.05}$,

查 $F$ 分布表得

$$
{F}_{0.05}\left( {24.14}\right)  = {2.35},\;{F}_{0.05}\left( {14.24}\right)  = {2.13},
$$

而 $\frac{{S}_{1}^{2}}{{S}_{2}^{2}} = \frac{6.38}{5.15} \approx  {1.24}$.

由置信区间公式得 $\frac{{\sigma }_{1}^{2}}{{\sigma }_{2}^{2}}$ 的 ${90}\%$ 置信区间为

$$
\left( {\frac{{S}_{1}^{2}}{{S}_{2}^{2}}{F}_{0.95}\left( {{14},{24}}\right),\frac{{S}_{1}^{2}}{{S}_{2}^{2}}{F}_{0.05}\left( {{14},{24}}\right) }\right)  = \left( {{0.528},{2.641}}\right).
$$

【3. 10】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自分布 $N\left( {\mu,{\sigma }^{2}}\right)$ 的样本, $\mu$ 已知, $\sigma$ 未知.

( 1 )验证 $\mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {X}_{i} - \mu \right) }^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( n\right)$. 利用这一结果构造 ${\sigma }^{2}$ 的置信水平为 $1 - \alpha$ 的置信区间.

(2)设 $\mu  = {6.5}$,且有样本值7.5,2.0,12.1,8.8,9.4,7.3,1.9,2.8,7.0,7.3,试求 $\sigma$ 的置信水平为 0.95 的置信区间.

解 (1) 因 ${X}_{i} \sim  N\left( {\mu,{\sigma }^{2}}\right)$,故

$$
\frac{{X}_{i} - \mu }{\sigma } \sim  N\left( {0,1}\right),\;i = 1,2,\cdots, n.
$$

由 $\frac{{X}_{1} - \mu }{\sigma },\frac{{X}_{2} - \mu }{\sigma },\cdots,\frac{{X}_{n} - \mu }{\sigma }$ 相互独立,得

$$
\mathop{\sum }\limits_{{i = 1}}^{n}{\left( \frac{{X}_{i} - \mu }{\sigma }\right) }^{2} \sim  {\chi }^{2}\left( n\right).
$$

于是有

$$
P\left\{  {{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right)  < \mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {X}_{i} - \mu \right) }^{2}}{{\sigma }^{2}} < {\chi }_{\frac{\alpha }{2}}^{2}\left( n\right) }\right\}   = 1 - \alpha,
$$

即有

$$
P\left\{  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( n\right) } < {\sigma }^{2} < \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right) }}\right\}   = 1 - \alpha.
$$

得 ${\sigma }^{2}$ 的置信水平为 $1 - \alpha$ 的置信区间为

$$
\left( {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( n\right) },\;\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( n\right) }}\right).
$$

(2)现在 $n = {10},\mu  = {6.5},1 - \alpha  = {0.95},\alpha  = {0.05}$,由样本值经计算得 $\mathop{\sum }\limits_{{i = 1}}^{{10}}{\left( {X}_{i} - \mu \right) }^{2} = {102}$. 69,查表知, ${\chi }_{0.025}^{2}\left( {10}\right)  = {20.483},{\chi }_{0.975}^{2}\left( {10}\right)  = {3.247}$.

于是 ${\sigma }^{2}$ 的置信水平为 0.95 的置信区间为 $\left( {{5.013},{31.626}}\right).\sigma$ 的置信水平为 0.95 的置信区间为 $\left( {{2.239},{5.624}}\right)$.

#### 题型 3: 单侧置信限问题

【3.11】从一批电子元件中随机地抽取 10 只作寿命试验,其寿命 (以小时计) 如下:

$\begin{array}{llllllllll} {1498} & {1499} & {1501} & {1503} & {1500} & {1499} & {1499} & {1498} & {1500} & {1503} \end{array}$

设寿命服从正态分布,试求其平均寿命的 95% 置信下限.

解 本例中,总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,且方差 ${\sigma }^{2}$ 未知,故应使用 $t$ 分布. 因

$$
\frac{\left( {\bar{X} - \mu }\right)  \cdot  \sqrt{n}}{S} \sim  t\left( {n - 1}\right),
$$

此时要求

$$
P\left\{  {\frac{\left( {\bar{X} - \mu }\right) \sqrt{n}}{S} < {t}_{\alpha }\left( {n - 1}\right) }\right\}   = 1 - \alpha,
$$

于是得 $\mu$ 的置信度 $1 - \alpha$ 单侧置信区间为

$$
\left( {\bar{X} - {t}_{\alpha }\left( {n - 1}\right)  \cdot  \frac{S}{\sqrt{n}}, + \infty }\right).
$$

对于给定的数据, 具体计算如下:

$$
\bar{x} = \frac{1}{10}\left( {{1498} + {1499} + {1501} + {1503} + {1500} + {1499} + {1499} + {1498} + {1500} + {1503}}\right)  = {1500}\text{,}
$$

$$
{s}^{2} = \frac{1}{{10} - 1}\left\lbrack  {{\left( {1498} - {1500}\right) }^{2} + {\left( {1499} - {1500}\right) }^{2} + {\left( {1501} - {1500}\right) }^{2}}\right.
$$

$$
+ {\left( {1503} - {1500}\right) }^{2} + {\left( {1500} - {1500}\right) }^{2} + {\left( {1499} - {1500}\right) }^{2} + {\left( {1499} - {1500}\right) }^{2}
$$

$$
\left. {+{\left( {1498} - {1500}\right) }^{2} + {\left( {1500} - {1500}\right) }^{2} + {\left( {1503} - {1500}\right) }^{2}}\right\rbrack
$$

$$
= \frac{10}{3}\text{,}
$$

又

$$
1 - \alpha  = {0.95},\alpha  = {0.05},{t}_{0.05}\left( {{10} - 1}\right)  = {1.8331}\text{,}
$$

故寿命均值的 95% 单侧置信区间为

$$
\left( {{1500} - \frac{1}{\sqrt{10}} \times  \sqrt{\frac{10}{3}} \times  {1.8331}, + \infty }\right)  \approx  \left( {{1498.942}, + \infty }\right).
$$

1498.942 就是所求的置信下限.

#### 题型 4 : 非正态总体参数的区间估计

【3.12】在一大批产品中取 100 件,经检验有 92 件正品,若记这批产品的正品率为 $p$,求 $p$ 的置信度 0.95 的置信区间.

解 本题中的正品率 $p$ 就是 $\left( {0 - 1}\right)$ 分布中的参数 $p$,而 $n = {100}$ 属于大样本.

由 $1 - \alpha  = {0.95}$ 知 $\alpha  = {0.05}$,查得 ${u}_{0.025} = {1.96}$,而样本中平均正品率 $\bar{x} = \frac{92}{100}$,代入公式

$$
\bar{p} = \bar{x} + {u}_{\frac{\alpha }{2}}\sqrt{\frac{x\left( {1 - x}\right) }{n}} = {0.92} + {1.96}\sqrt{\frac{{0.92} \times  {0.08}}{100}} = {0.97},
$$

$$
\underline{p} = \bar{x} - {u}_{\frac{\alpha }{2}}\sqrt{\frac{x\left( {1 - x}\right) }{n}} = {0.92} - {1.96}\sqrt{\frac{{0.92} \times  {0.08}}{100}} = {0.87},
$$

所以 $p$ 的置信度 0.95 的置信区间为 $\left( {{0.87},{0.97}}\right)$.

【3.13】设总体 $X$ 的方差 ${\sigma }^{2} = 1$,根据来自 $X$ 的容量为 100 的简单样本,测得样本均值为 5, 则 $X$ 的数学期望的置信度近似等于 0.95 的置信区间为_____.

解 设 ${EX} = \mu$,由中心极限定理 $U = \frac{\bar{X} - \mu }{\frac{\sigma }{\sqrt{n}}}$ 近似服从 $N\left( {0,1}\right)$,

令

$$
P\left\{  {\left| U\right|  < {u}_{\frac{\alpha }{2}}}\right\}   \approx  1 - {0.05} = {0.95},
$$

查正态分布表,得 ${u}_{\frac{\alpha }{2}} = {1.96}$,代入 $X$ 的数学期望的置信区间

$$
\left\lbrack  {\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}},\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}}\right\rbrack ,
$$

经计算为 $\left( {{4.804},{5.196}}\right)$.

故应填 (4.804,5.196).

点评 本题未说明总体 $X$ 为正态分布,因此直接套用正态总体 $\mu$ 的置信区间公式不妥,应该先用中心极限定理取近似, 再根据定义求出置信区间.

## $§4$. 综合提高题型

题型1: 关于点估计

【4.1】设总体 $X$ 的概率密度为

$$
f\left( {x;\theta }\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-\left( {x - \theta }\right) }, & \text{ 若 }x \geq  \theta \\  0, & \text{ 若 }x < \theta  \end{array}\right.
$$

而 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体 $X$ 的简单随机样本,则未知参数 $\theta$ 的矩估计量为_____.

解 ${EX} = {\int }_{0}^{+\infty }x{\mathrm{e}}^{-\left( {x - \theta }\right) }\mathrm{d}x = \theta  + 1$,即 $\theta  = {EX} - 1$.

因此 $\theta$ 的矩估计量为

$$
\widehat{\theta } = \bar{X} - 1 = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - 1.
$$

【4.2】设总体 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{6x}{{\theta }^{3}}\left( {\theta  - x}\right), & 0 < x < \theta \\  0, & \text{ 其他 } \end{array}\right.
$$

${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是取自总体 $X$ 的简单随机样本.

(1)求 $\theta$ 的矩估计量 $\widehat{\theta }$;

(2) 求 $\widehat{\theta }$ 的方差 $D\left( \widehat{\theta }\right)$.

解 (1) ${EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = {\int }_{0}^{\theta }\frac{6{x}^{2}}{{\theta }^{3}}\left( {\theta  - x}\right) \mathrm{d}x = {\int }_{0}^{\theta }\left( {\frac{6{x}^{2}}{{\theta }^{2}} - \frac{6{x}^{3}}{{\theta }^{3}}}\right) \mathrm{d}x = \frac{\theta }{2}$,

因此 $\theta  = {2EX}$,所以 $\theta$ 的矩估计量为 $\widehat{\theta } = 2\bar{X}$.

(2)由(1)可知,

$$
{EX} = \frac{\theta }{2},\;E{X}^{2} = {\int }_{0}^{\theta }\frac{6{x}^{3}}{{\theta }^{3}}\left( {\theta  - x}\right) \mathrm{d}x = \frac{6{\theta }^{2}}{20},
$$

故

$$
{DX} = E{X}^{2} - {\left( EX\right) }^{2} = \frac{6{\theta }^{2}}{20} - {\left( \frac{\theta }{2}\right) }^{2} = \frac{{\theta }^{2}}{20},
$$

因此

$$
D\left( \widehat{\theta }\right)  = D\left( {2\bar{X}}\right)  = {4D}\left( \bar{X}\right)  = \frac{4}{n}D\left( X\right)  = \frac{4}{n} \times  \frac{{\theta }^{2}}{20} = \frac{{\theta }^{2}}{5n}.
$$

【4.3】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为总体的一个样本,求下列各总体的密度函数或分布律中的未知参数的矩估计量和最大似然估计量.

(1) $f\left( x\right)  = \left\{  \begin{array}{ll} \theta {c}^{\theta }{x}^{-\left( {\theta  + 1}\right) }, & x > c \\  0, & \text{ 其他 } \end{array}\right.$,其中 $c > 0$ 为已知, $\theta  > 1$, $\theta$ 为未知参数.

(2) $f\left( x\right)  = \left\{  \begin{array}{ll} \sqrt{\theta }{x}^{\sqrt{\theta } - 1}, & 0 \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.$,其中 $\theta  > 0,\theta$ 为未知参数.

(3) $P\{ X = x\}  = {C}_{m}^{x}{p}^{x}{\left( 1 - p\right) }^{m - x}, x = 0,1,2,\cdots, m,0 < p < 1, p$ 为未知参数.

解 (1) $E\left( X\right)  = {\int }_{c}^{\infty }{x\theta }{c}^{\theta }{x}^{-\left( {\theta  + 1}\right) }\mathrm{d}x = {\int }_{c}^{\infty }\theta {c}^{\theta }{x}^{-\theta }\mathrm{d}x = \theta {c}^{\theta }{\int }_{c}^{\theta }{x}^{-\theta }\mathrm{d}x = {\left. \theta {c}^{\theta }\frac{{x}^{-\theta  + 1}}{-\theta  + 1}\right| }_{c}^{+\infty }$

$= \frac{\theta c}{\theta  - 1}$.

令 $\frac{\theta c}{\theta  - 1} = \bar{X}$,解得 $\widehat{\theta } = \frac{\bar{X}}{\bar{X} - c}$,即为 $\theta$ 的矩估计量.

似然函数为

$$
L\left( \theta \right)  = \mathop{\prod }\limits_{{i = 1}}^{n}\theta  \cdot  {c}^{\theta }{x}_{i}^{-\left( {\theta  + 1}\right) } = {\theta }^{n}{c}^{n\theta }\mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}^{-\left( {\theta  + 1}\right) },
$$

而

$$
\ln L\left( \theta \right)  = n\ln \theta  + {n\theta }\ln c - \left( {\theta  + 1}\right) \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i},
$$

令

$$
\frac{\mathrm{d}}{\mathrm{d}\theta }\ln L\left( \theta \right)  = \frac{n}{\theta } + n\ln c - \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i} = 0,
$$

解得 $\theta$ 的最大似然估计量 $\widehat{\theta } = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}\ln {X}_{i} - n\ln c}$.

(2) ${EX} = {\int }_{0}^{1}x\sqrt{\theta }{x}^{\sqrt{\theta } - 1}\mathrm{\;d}x = {\int }_{0}^{1}\sqrt{\theta }{x}^{\sqrt{\theta }}\mathrm{d}x = {\left. \frac{\sqrt{\theta }}{\sqrt{\theta } + 1}{x}^{\sqrt{\theta } + 1}\right| }_{0}^{1} = \frac{\sqrt{\theta }}{\sqrt{\theta } + 1}$.

令 $\frac{\sqrt{\theta }}{\sqrt{\theta } + 1} = \bar{X}$,解得 $\widehat{\theta } = {\left( \frac{\bar{X}}{\bar{X} - 1}\right) }^{2}$,即为 $\theta$ 的矩估计量.

似然函数为:

$$
L\left( \theta \right)  = \mathop{\prod }\limits_{{i = 1}}^{n}\sqrt{\theta }{x}_{i}^{\sqrt{\theta } - 1} = {\theta }^{\frac{n}{2}}\mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}^{\sqrt{\theta } - 1},
$$

对数似然函数为:

$$
\ln L\left( \theta \right)  = \frac{n}{2}\ln \theta  + \left( {\sqrt{\theta } - 1}\right) \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i},
$$

对数似然方程为:

$$
\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = \frac{n}{2\theta } + \frac{\mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i}}{2\sqrt{\theta }} = 0,
$$

其最大似然估计值为 $\widehat{\theta } = \frac{{n}^{2}}{{\left( \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i}\right) }^{2}},\widehat{\theta } = \frac{{n}^{2}}{{\left( \mathop{\sum }\limits_{{i = 1}}^{n}\ln {X}_{i}\right) }^{2}}$ 即为 $\theta$ 的最大似然估计量.

(3)因为 $X \sim  B\left( {m, p}\right)$,所以

$$
E\left( X\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}x{C}_{m}^{x}{p}^{x}{\left( 1 - p\right) }^{m - x} = {mp},
$$

所以 ${mp} = \bar{X},\widehat{p} = \frac{\bar{X}}{m}$ 为 $p$ 的矩估计.

似然函数为:

$$
L\left( p\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}{C}_{ml}^{{x}_{i}}{p}^{{x}_{i}}{\left( 1 - p\right) }^{m - {x}_{i}} = {p}_{i = 1}^{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}{\left( 1 - p\right) }^{{nm} - \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}\mathop{\prod }\limits_{{i = 1}}^{n}{C}_{m\ell }^{{x}_{i}},
$$

对数似然函数为:

$$
\ln L\left( p\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}\ln p + \left( {{nm} - \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}\right) \ln \left( {1 - p}\right)  + \mathop{\sum }\limits_{{i = 1}}^{n}\ln {C}_{ni}^{{x}_{i}},
$$

对数似然方程为:

$$
\frac{\mathrm{d}\ln L\left( p\right) }{\mathrm{d}p} = \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}{p} + \frac{{nm} - \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}{1 - p}\left( {-1}\right)  = 0,
$$

则 $\widehat{p} = \frac{\bar{x}}{m}$ 为 $p$ 的最大似然估计值. $\widehat{p} = \frac{\bar{X}}{m}$ 为 $p$ 的最大似然估计量.

【4.4】某工程师为了解一台天平的精度,用该天平对一物体的质量做 $n$ 次测量,该物质的质量 $\mu$ 是已知的,设 $n$ 次测量结果 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 相互独立且均服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$. 该工程师记录的是 $n$ 次测量的绝对误差 ${Z}_{i} = \left| {{X}_{i} - \mu }\right| \left( {i = 1,2,\cdots, n}\right)$,利用 ${Z}_{1},{Z}_{2},\cdots,{Z}_{n}$ 估计 $\sigma$.

(1)求 ${Z}_{1}$ 的概率密度；(2)利用一阶矩求 $\sigma$ 的矩估计量；(3)求 $\sigma$ 的最大似然估计量.

解 (1) ${Z}_{1}$ 的分布函数为

$$
F\left( z\right)  = P\left\{  {{Z}_{1} \leq  z}\right\}   = P\left\{  {\left| {{X}_{1} - \mu }\right|  \leq  z}\right\}   = \left\{  \begin{array}{ll} {2\Phi }\left( \frac{z}{\sigma }\right)  - 1, & z \geq  0, \\  0, & z < 0, \end{array}\right.
$$

所以 ${Z}_{1}$ 的概率密度为

$$
f\left( z\right)  = \left\{  \begin{array}{ll} \frac{2}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{-\frac{{z}^{2}}{2{\sigma }^{2}}}, & z \geq  0, \\  0, & z < 0 \end{array}\right.
$$

(2) $E{Z}_{1} = {\int }_{-\infty }^{+\infty }{zf}\left( z\right) \mathrm{d}z = \frac{2}{\sqrt{2\pi }\sigma }{\int }_{-\infty }^{+\infty }z{\mathrm{e}}^{-\frac{{z}^{2}}{2{\sigma }^{2}}}\mathrm{\;d}z = \frac{2}{\sqrt{2\pi }}\sigma$.

$\sigma  = \frac{\sqrt{2\pi }}{2}E{Z}_{1}$,令 $\bar{Z} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{Z}_{i}$,得 $\sigma$ 的矩估计量为 $\widehat{\sigma } = \frac{\sqrt{2\pi }}{2}\bar{Z}$.

(3)记 ${z}_{1},{z}_{2},\cdots,{z}_{n}$ 为样本 ${Z}_{1},{Z}_{2},\cdots,{Z}_{n}$ 的观测值,则似然函数为

$$
L\left( \sigma \right)  = \mathop{\prod }\limits_{{i = 1}}^{n}f\left( {z}_{i}\right)  = {\left( \frac{2}{\sqrt{2\pi }}\right) }^{n}{\sigma }^{-n}{\mathrm{e}}^{-\frac{1}{2{\sigma }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2}},
$$

对数似然函数为 $\ln L\left( \sigma \right)  = n\ln \frac{2}{\sqrt{2\pi }} - n\ln \sigma  - \frac{1}{2{\sigma }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2}$.

令 $\frac{\mathrm{d}\ln L\left( \sigma \right) }{\mathrm{d}\sigma } =  - \frac{n}{\sigma } + \frac{1}{{\sigma }^{3}}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2} = 0$,得 $\sigma$ 的最大似然估计值为 $\sigma  = \sqrt{\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2}}$,所以 $\sigma$ 的最大似然估计量为 $\widehat{\sigma } = \sqrt{\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2}}$.

【4.5】设总体 $X$ 的概率密度为

$$
f\left( {x;\theta }\right)  = \left\{  \begin{matrix} \frac{{\theta }^{2}}{{x}^{3}}{\mathrm{e}}^{-\frac{\theta }{x}}, & x > 0, \\  0, & \text{ 其他,} \end{matrix}\right.
$$

其中 $\theta$ 为未知参数且大于零, ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自总体 $X$ 的简单随机样本.

(1)求 $\theta$ 的矩估计量；

(2)求 $\theta$ 的最大似然估计量.

解 (1) ${EX} = {\int }_{0}^{+\infty }x \cdot  \frac{{\theta }^{2}}{{x}^{3}}{\mathrm{e}}^{-\frac{\theta }{x}}\mathrm{\;d}x$

$$
= {\int }_{0}^{+\infty }\frac{{\theta }^{2}}{{x}^{2}}{\mathrm{e}}^{-\frac{\theta }{x}}\mathrm{\;d}x = \theta.
$$

所以 $\theta$ 的矩估计量为 $\widehat{\theta } = \bar{X}$,其中 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$.

(2)设 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 为样本观测值,似然函数为

$$
L\left( \theta \right)  = \mathop{\prod }\limits_{{i = 1}}^{n}f\left( {{x}_{i};\theta }\right)
$$

$$
= \left\{  \begin{array}{ll} \frac{{\theta }^{2n}}{{\left( {x}_{1}{x}_{2}\cdots {x}_{n}\right) }^{3}}{\mathrm{e}}^{-\theta \mathop{\sum }\limits_{{i = 1}}^{n}\frac{1}{{x}_{i}}}, & {x}_{1},{x}_{2},\cdots,{x}_{n} > 0, \\  0, & \text{ 其他. } \end{array}\right.
$$

当 ${x}_{1},{x}_{2},\cdots,{x}_{n} > 0$ 时, $\ln L\left( \theta \right)  = {2n}\ln \theta  - \theta \mathop{\sum }\limits_{{i = 1}}^{n}\frac{1}{{x}_{i}} - 3\mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i}$.

令 $\frac{\mathrm{d}\ln L\left( \theta \right) }{\mathrm{d}\theta } = \frac{2n}{\theta } - \mathop{\sum }\limits_{{i = 1}}^{n}\frac{1}{{x}_{i}} = 0$,得 $\theta$ 的最大似然估计值为 $\widehat{\theta } = \frac{2n}{\mathop{\sum }\limits_{{i = 1}}^{n}\frac{1}{{x}_{i}}}$,所以 $\theta$ 的最大似然估

计量为 $\widehat{\theta } = \frac{2n}{\mathop{\sum }\limits_{{i = 1}}^{n}\frac{1}{{X}_{i}}}$.

【4.6】设总体 $X$ 服从几何分布 $P\{ X = k\}  = p{\left( 1 - p\right) }^{k - 1}, k = 1,2,\cdots$. 又 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 是来自 $X$ 的样本值,则 $p$ 与 ${EX}$ 的最大似然估计分别为多少?

解 $L\left( p\right)  = {p}^{n}{\left( 1 - p\right) }^{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} - n}$,

令 $\frac{\mathrm{d}\ln L}{\mathrm{\;d}p} = 0$,解得 $p = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}} = \frac{1}{\bar{X}}$,故 $\widehat{p} = \frac{1}{\bar{X}}$ 即为 $p$ 的最大似然估计.

而 ${EX} = \frac{1}{p}$,故由最大似然估计不变性 $\overset{⏜}{EX} = \frac{1}{\widehat{p}} = \bar{X}$ 为 ${EX}$ 的最大似然估计.

【4.7】设总体 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} {\lambda }^{2}x{\mathrm{e}}^{-{\lambda x}}, & x > 0 \\  0, & \text{ 其他 } \end{array}\right.
$$

其中参数 $\lambda \left( {\lambda  > 0}\right)$ 未知, ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体 $X$ 的简单随机样本.

(1)求参数 $\lambda$ 的矩估计量；

(2)求参数 $\lambda$ 的最大似然估计量.

解 (1) ${EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }{\lambda }^{2}{x}^{2}{\mathrm{e}}^{-{\lambda x}}\mathrm{\;d}x = \frac{2}{\lambda }$.

令 $\bar{X} = {EX}$,即 $\bar{X} = \frac{2}{\lambda }$,得 $\lambda$ 的矩估计量为 $\widehat{\lambda } = \frac{2}{\bar{X}}$.

(2)设 ${x}_{1},{x}_{2},\cdots,{x}_{n}\left( {{x}_{i} > 0, i = 1,2,\cdots, n}\right)$ 为样本观测值,则似然函数为

$$
L\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\lambda }\right)  = {\lambda }^{2n}{\mathrm{e}}^{-\lambda \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}\mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i},
$$

$$
\ln L = {2n}\ln \lambda  - \lambda \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} + \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i},
$$

由 $\frac{\mathrm{d}\ln L}{\mathrm{\;d}\lambda } = \frac{2n}{\lambda } - \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i} = 0$,得 $\lambda$ 的最大似然估计量为 $\widehat{\lambda } = \frac{2}{\bar{X}}$.

【4.8】设随机变量 $X$ 的分布函数为

$$
F\left( {x;\alpha,\beta }\right)  = \left\{  \begin{array}{ll} 1 - {\left( \frac{\alpha }{x}\right) }^{\beta }, & x > \alpha \\  0, & x \leq  \alpha  \end{array}\right.
$$

其中参数 $\alpha  > 0,\beta  > 1$,设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自总体 $X$ 的简单随机样本.

(1)当 $\alpha  = 1$ 时,求未知参数 $\beta$ 的矩估计量；

(2)当 $\alpha  = 1$ 时,求未知参数 $\beta$ 的最大似然估计量；

(3)当 $\beta  = 2$ 时,求未知参数 $\alpha$ 的最大似然估计量.

解 (1) 由已知 $X$ 的分布函数可得其概率密度为

$$
f\left( {x;\alpha,\beta }\right)  = \left\{  \begin{array}{ll} \frac{\beta {\alpha }^{\beta }}{{x}^{\beta  + 1}}, & x > \alpha \\  0, & x \leq  \alpha  \end{array}\right.
$$

当 $\alpha  = 1$ 时, $X$ 的概率密度为

$$
f\left( {x;\beta }\right)  = \left\{  {\begin{array}{ll} \frac{\beta }{{x}^{\beta  + 1}}, & x > 1 \\  0, & x \leq  1 \end{array},}\right.
$$

$$
{EX} = {\int }_{-\infty }^{+\infty }{xf}\left( {x;\beta }\right) \mathrm{d}x = {\int }_{1}^{+\infty }\frac{\beta }{{x}^{\beta }}\mathrm{d}x = \frac{\beta }{\beta  - 1},
$$

令 $\frac{\beta }{\beta  - 1} = \bar{X}$,解得 $\beta  = \frac{\bar{X}}{\bar{X} - 1}$,所以 $\beta$ 的矩估计量为 $\widehat{\beta } = \frac{\bar{X}}{\bar{X} - 1}$,其中 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$.

(2)对于总体 $X$ 的样本值 ${x}_{1},{x}_{2},\cdots,{x}_{n}$,似然函数为

$$
L\left( \beta \right)  = \left\{  \begin{array}{ll} \frac{{\beta }^{n}}{{\left( {x}_{1}{x}_{2}\cdots {x}_{n}\right) }^{\beta  + 1}}, & {x}_{i} > 1\left( {i = 1,2,\cdots, n}\right) \\  0, & \text{ 其他 } \end{array}\right.
$$

当 ${x}_{i} > 1$ 时,两边取对数得

$$
\ln L\left( \beta \right)  = n\ln \beta  - \left( {\beta  + 1}\right) \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i},\;\frac{\mathrm{d}\ln L\left( \beta \right) }{\mathrm{d}\beta } = \frac{n}{\beta } - \mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i},
$$

令 $\frac{\mathrm{d}\ln L\left( \beta \right) }{\mathrm{d}\beta } = 0$,解之得 $\beta  = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i}}$.

故 $\beta$ 的最大似然估计量为 $\widehat{\beta } = \frac{n}{\mathop{\sum }\limits_{{i = 1}}^{n}\ln {X}_{i}}$.

(3)当 $\beta  = 2$ 时, $X$ 的概率密度为

$$
f\left( {x;\alpha }\right)  = \left\{  \begin{array}{ll} \frac{2{\alpha }^{2}}{{x}^{3}}, & x > \alpha \\  0, & x \leq  \alpha  \end{array}\right.
$$

对于总体 $X$ 的样本值 ${x}_{1},{x}_{2},\cdots,{x}_{n}$,其似然函数为

$$
L\left( \alpha \right)  = \left\{  \begin{array}{ll} \frac{{2}^{n}{\alpha }^{2n}}{{\left( {x}_{1}{x}_{2}\cdots {x}_{n}\right) }^{3}}, & {x}_{i} > \alpha \left( {i = 1,2,\cdots, n}\right) \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
\ln L\left( \alpha \right)  = n\ln 2 + {2n}\ln \alpha  - 3\mathop{\sum }\limits_{{i = 1}}^{n}\ln {x}_{i},\;\frac{\mathrm{d}\ln L\left( \alpha \right) }{\mathrm{d}\alpha } = \frac{2n}{\alpha } > 0,
$$

所以 $L\left( \alpha \right)$ 单调递增.

当 ${x}_{i} > \alpha \left( {i = 1,2,\cdots, n}\right)$ 时, $\alpha$ 越大, $L\left( \alpha \right)$ 就越大,因此 $\alpha$ 的最大似然估计值为

$$
\widehat{\alpha } = \min \left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right).
$$

则 $\alpha$ 的最大似然估计量为 $\widehat{\alpha } = \min \left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$.

【4.9】设某种电子器件的寿命 (以小时计) $T$ 服从双参数的指数分布,其概率密度为

$$
f\left( t\right)  = \left\{  \begin{array}{ll} \frac{1}{\theta }{\mathrm{e}}^{-\frac{t - c}{\theta }}, & t \geq  c \\  0, & \text{ 其他 } \end{array}\right.
$$

其中 $c,\theta \left( {c,\theta  > 0}\right)$ 为未知参数,自一批这种器件中随机地取 $n$ 件进行寿命试验. 设它们的失效时间依次为 ${x}_{1} \leq  {x}_{2} \leq  \cdots  \leq  {x}_{n}$.

(1)求 $\theta$ 与 $c$ 的最大似然估计;

(2)求 $\theta$ 与 $c$ 的矩估计.

解 (1) 似然函数为

$$
L\left( {\theta, c}\right)  = \left\{  \begin{array}{ll} \frac{1}{{\theta }^{n}}{\mathrm{e}}^{-\frac{1}{\theta }\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{x}_{i} - c}\right) }, & {x}_{i} \geq  c, i = 1,2,\cdots, n \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} \frac{1}{{\theta }^{n}}{\mathrm{e}}^{-\frac{1}{\theta }\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{x}_{i} - c}\right) }, & {x}_{n} \geq  {x}_{n - 1} \geq  \cdots  \geq  {x}_{2} \geq  {x}_{1} \geq  c \\  0, & \text{ 其他 } \end{array}\right.
$$

对数似然函数为:

$$
\ln L\left( {\theta, c}\right)  =  - n\ln \theta  - \frac{1}{\theta }\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{x}_{i} - c}\right),
$$

对数似然方程为:

$$
\frac{\partial \ln L\left( {\theta, c}\right) }{\partial c} = \frac{n}{\theta } > 0,
$$

故 $\ln L\left( {\theta, c}\right)$ 关于 $c$ 单调增加,故 $\widehat{c} = {x}_{1}$.

由

$$
\frac{\partial \ln L\left( {\theta, c}\right) }{\partial \theta } =  - \frac{n}{\theta } + \frac{1}{{\theta }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{x}_{i} - c}\right)  = 0,
$$

得 $\theta$ 的最大似然估计值为 $\widehat{\theta } = \bar{x} - {x}_{1}$.

(2) ${EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = {\int }_{c}^{+\infty }\frac{x}{\theta }{\mathrm{e}}^{-\frac{x - c}{\theta }}\mathrm{d}x = \theta  + c$,

$$
E\left( {X}^{2}\right)  = {\int }_{c}^{+\infty }\frac{{x}^{2}}{\theta }{\mathrm{e}}^{-\frac{x - c}{\theta }}\mathrm{\;d}x = {\theta }^{2} + {\left( \theta  + c\right) }^{2},
$$

令 ${EX} = \bar{x}, E\left( {X}^{2}\right)  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}^{2}$,那么 $\theta$ 和 $c$ 的矩估计为

$$
\widehat{\theta } = \sqrt{\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \bar{x}\right) }^{2}},\;\widehat{c} = \bar{x} - \sqrt{\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \bar{x}\right) }^{2}}.
$$

【4. 10】设总体 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} 2{\mathrm{e}}^{-2\left( {x - \theta }\right) }, & x > \theta \\  0, & x \leq  \theta  \end{array}\right.
$$

其中 $\theta  > 0$ 是未知参数,从总体中抽取简单随机样本 ${X}_{1},{X}_{2},\cdots,{X}_{n}$. 记 $\widehat{\theta } = \min \left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$.

(1)求总体 $X$ 的分布函数 $F\left( x\right)$;

(2)求统计量 $\widehat{\theta }$ 的分布函数 ${F}_{\widehat{\theta }}\left( x\right)$;

(3)如果用 $\widehat{\theta }$ 作为 $\theta$ 的估计量,讨论它是否具有无偏性.

解 (1) 由总体 $X$ 的概率密度可得

$$
F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-2\left( {x - \theta }\right) }, & x \geq  \theta \\  0, & x < \theta  \end{array}\right.
$$

(2) ${F}_{\widehat{\theta }}\left( x\right)  = P\{ \widehat{\theta } \leq  x\}  = P\left\{  {\min \left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)  \leq  x}\right\}$

$$
= 1 - P\left\{  {\min \left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)  > x}\right\}
$$

$$
= 1 - P\left\{  {{X}_{1} > x,{X}_{2} > x,\cdots,{X}_{n} > x}\right\}
$$

$$
= 1 - P\left\{  {{X}_{1} > x}\right\}  P\left\{  {{X}_{2} > x}\right\}  \cdots P\left\{  {{X}_{n} > x}\right\} .
$$

由于 $P\left\{  {{X}_{i} > x}\right\}   = 1 - P\left\{  {{X}_{i} \leq  x}\right\}   = 1 - F\left( x\right)$,因此 $F\partial \left( x\right)  = 1 - {\left\lbrack  1 - F\left( x\right) \right\rbrack  }^{n}$.

即 ${F}_{\widehat{\theta }}\left( x\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{2n}\left( {x - \theta }\right) }, & x \geq  \theta \\  0, & x < \theta  \end{array}\right.$

(3) 由 ${F}_{\widehat{\theta }}\left( x\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{2n}\left( {x - \theta }\right) }, & x \geq  \theta \\  0, & x < \theta  \end{array}\right.$,可得 $\widehat{\theta }$ 的概率密度为

$$
{f}_{\widehat{\theta }}\left( x\right)  = {F}_{\widehat{\theta }}^{\prime }\left( x\right)  = \left\{  \begin{array}{ll} {2n}{\mathrm{e}}^{-{2n}\left( {x - \theta }\right) }, & x \geq  \theta \\  0, & x < \theta  \end{array}\right.
$$

则

$$
E\widehat{\theta } = {\int }_{-\infty }^{\infty }{xf}\widehat{\theta }\left( x\right) \mathrm{d}x = {\int }_{\theta }^{\infty }{2nx}{\mathrm{e}}^{-{2n}\left( {x - \theta }\right) }\mathrm{d}x = \theta  + \frac{1}{2n},
$$

故 $E\widehat{\theta } \neq  \theta$. 因此 $\widehat{\theta }$ 不是 $\theta$ 的无偏估计.

【4.11】设总体 $X$ 的概率密度为

$$
f\left( {x;\theta }\right)  = \left\{  \begin{array}{ll} \frac{2x}{3{\theta }^{2}}, & \theta  < x < {2\theta }, \\  0, & \text{ 其他,} \end{array}\right.
$$

其中 $\theta$ 是未知参数, ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自总体 $X$ 的简单随机样本. 若 $c\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 是 ${\theta }^{2}$ 的无偏估计, 则 $c =$ _____.

解 $E\left( {c\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}}\right)  = c\mathop{\sum }\limits_{{i = 1}}^{n}E\left( {X}_{i}^{2}\right)  = c\mathop{\sum }\limits_{{i = 1}}^{n}E\left( {X}^{2}\right)$

$$
= {cn}{\int }_{-\infty }^{+\infty }{x}^{2}f\left( x\right) \mathrm{d}x = {cn}{\int }_{\theta }^{2\theta }{x}^{2} \cdot  \frac{2x}{3{\theta }^{2}}\mathrm{\;d}x = {cn} \cdot  \frac{5}{2}{\theta }^{2}.
$$

因为 $c\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 是 ${\theta }^{2}$ 的无偏性估计,所以 $E\left( {c\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}}\right)  = {\theta }^{2}$.

即 ${cn} \cdot  \frac{5}{2}{\theta }^{2} = {\theta }^{2}$,所以 $c = \frac{2}{5n}$.

故应填 $\frac{2}{5n}$.

【4.12】设总体 $X$ 服从 $\left\lbrack  {0,\theta }\right\rbrack$ 上的均匀分布, $\theta$ 未知 $\left( {\theta  > 0}\right)$, ${X}_{1}$, ${X}_{2}$, ${X}_{3}$ 是取自 $X$ 的一个样本.

(1)试证 ${\widehat{\theta }}_{1} = \frac{4}{3}\mathrm{\;m}\mathrm{a}\underset{1 \leq  i \leq  3}{\mathrm{x}}{X}_{i},{\widehat{\theta }}_{2} = 4\mathrm{\;m}\mathrm{i}\underset{1 \leq  i \leq  3}{\mathrm{n}}{X}_{i}$ 都是 $\theta$ 的无偏估计;

(2)上述两个估计中哪个更有效？

证 (1) 设 $F\left( x\right)$ 是 $X$ 的分布函数,则

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 1, & x > \theta \\  \frac{x}{\theta }, & 0 \leq  x \leq  \theta \\  0, & x < 0 \end{array}\right.
$$


$$
Y = \max \underset{1 \leq  i \leq  3}{\mathrm{x}}{X}_{i},\;Z = \min \underset{1 \leq  i \leq  3}{\mathrm{n}}{X}_{i},
$$

$$
{F}_{Y}\left( x\right)  = {\left\lbrack  F\left( x\right) \right\rbrack  }^{3},\;{f}_{Y}\left( {x,\theta }\right)  = \left\{  \begin{array}{ll} 3{\left( \frac{x}{\theta }\right) }^{2} \cdot  \frac{1}{\theta }, & 0 \leq  x \leq  \theta \\  0, & \text{ 其他 } \end{array}\right.
$$

故 $\;{EY} = \frac{3}{{\theta }^{3}}{\int }_{0}^{\theta }{x}^{3}\mathrm{\;d}x = \frac{3}{4}\theta$,则 $E\left( {\widehat{\theta }}_{1}\right)  = E\left( {\frac{4}{3}\max {X}_{i}}\right)  = \theta$,

同理 ${EZ} = \frac{3}{{\theta }^{3}}{\int }_{0}^{\theta }x{\left( \theta  - x\right) }^{2}\mathrm{\;d}x = \frac{1}{4}\theta$,则 $E\left( {\widehat{\theta }}_{2}\right)  = E\left( {4\min {X}_{i}}\right)  = \theta$.

(2) ${DY} = E{Y}^{2} - {\left( EY\right) }^{2} = \frac{3}{\theta }{\int }_{0}^{\theta }{x}^{2}{\left( \frac{x}{\theta }\right) }^{2}\mathrm{\;d}x - {\left( \frac{3}{4}\theta \right) }^{2} = \frac{3}{80}{\theta }^{2}$,

故 $\;D\left( {\widehat{\theta }}_{1}\right)  = D\left( {\frac{4}{3}\max {X}_{i}}\right)  = \frac{16}{9}{DY} = \frac{1}{15}{\theta }^{2}$,

同理 ${DZ} = \frac{3}{80}{\theta }^{2}$,故 $D\left( {\widehat{\theta }}_{2}\right)  = D\left( {4\min {X}_{i}}\right)  = {16DZ} = \frac{3}{5}{\theta }^{2} > D\left( {\widehat{\theta }}_{1}\right)$,

故 ${\widehat{\theta }}_{1}$ 更有效.

【4.13】设随机变量 $X$ 与 $Y$ 相互独立且分别服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$ 与 $N\left( {\mu,2{\sigma }^{2}}\right)$,其中 $\sigma$ 是未知参数且 $\sigma  > 0$,记 $Z = X - Y$.

(1)求 $Z$ 的概率密度 $f\left( z\right)$;

( 2 )设 ${Z}_{1},{Z}_{2},\cdots,{Z}_{n}$ 为来自总体 $Z$ 的简单随机样本,求 ${\sigma }^{2}$ 的最大似然估计量 ${\sigma }^{2}$;

(3)证明 ${\sigma }^{2}$ 为 ${\sigma }^{2}$ 的无偏估计量.

解 (1)因为 $X$ 与 $Y$ 相互独立且分别服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$ 与 $N\left( {\mu,2{\sigma }^{2}}\right)$,则 $Z = X - Y$ 服从正态分布 $N\left( {0,3{\sigma }^{2}}\right)$,故 $Z$ 的概率密度

$$
f\left( z\right)  = \frac{1}{\sqrt{6\pi }\sigma }{\mathrm{e}}^{-\frac{{z}^{2}}{6{\sigma }^{2}}}, - \infty  < z <  + \infty.
$$

(2)设 ${z}_{1},{z}_{2},\cdots,{z}_{n}$ 是样本 ${Z}_{1},{Z}_{2},\cdots,{Z}_{n}$ 所对应的一个样本值,则似然函数为

$L\left( {\sigma }^{2}\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}f\left( {z}_{i}\right)  = \frac{1}{{\left( \sqrt{6\pi }\right) }^{n}{\left( {\sigma }^{2}\right) }^{\frac{n}{2}}}{\mathrm{e}}^{\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2}}{6{\sigma }^{2}}},$

$\ln L\left( {\sigma }^{2}\right)  =  - \frac{n}{2}\ln \left( {6\pi }\right)  - \frac{n}{2}\ln {\sigma }^{2} - \frac{1}{6{\sigma }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2}$

令 $\frac{\mathrm{d}\ln L\left( {\sigma }^{2}\right) }{\mathrm{d}\left( {\sigma }^{2}\right) } = \frac{1}{6{\sigma }^{4}}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2} - \frac{n}{2{\sigma }^{2}} = 0$,

得 ${\sigma }^{2} = \frac{1}{3n}\mathop{\sum }\limits_{{i = 1}}^{n}{z}_{i}^{2}$

故 ${\sigma }^{2}$ 的最大似然估计量为 $\widehat{{\sigma }^{2}} = \frac{1}{3n}\mathop{\sum }\limits_{{i = 1}}^{n}{Z}_{i}^{2}$.

(3) 因为 $E\left( {\sigma }^{2}\right)  = E\left( {\frac{1}{3n}\mathop{\sum }\limits_{{i = 1}}^{n}{Z}_{i}^{2}}\right)  = \frac{1}{3n}E\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{Z}_{i}^{2}}\right)  = \frac{1}{3}E\left( {Z}^{2}\right)  = \frac{1}{3}D\left( Z\right)  = {\sigma }^{2}$,

故 ${\sigma }^{2}$ 为 ${\sigma }^{2}$ 的无偏估计量.

【4.14】设总体 $X$ 的概率分布为

<table><tr><td>$X$</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>$1 - \theta$</td><td>$\theta  - {\theta }^{2}$</td><td>${\theta }^{2}$</td></tr></table>

其中参数 $\theta  \in  \left( {0,1}\right)$ 未知,以 ${N}_{i}$ 表示来自总体 $X$ 的简单随机样本 (样本容量为 $n$ ) 中等于 $i$ 的个数 $\left( {i = 1,2,3}\right)$,试求常数 ${a}_{1},{a}_{2},{a}_{3}$,使 $T = \mathop{\sum }\limits_{{i = 1}}^{3}{a}_{i}{N}_{i}$ 为 $\theta$ 的无偏估计量,并求 $T$ 的方差.

解 根据简单随机样本的性质,样本 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 相互独立且与总体 $X$ 同分布,因此, $P\left\{  {{X}_{i} = 1}\right\}   = 1 - \theta, P\left\{  {{X}_{i} \neq  1}\right\}   = \theta, i = 1,2,\cdots, n$,则在 $n$ 次独立观测中取 1 的个数 ${N}_{1}$ 是个随机变量,且 ${N}_{1} \sim  B\left( {n,1 - \theta }\right)$,同理 ${N}_{2} \sim  B\left( {n,\theta  - {\theta }^{2}}\right),{N}_{3} \sim  B\left( {n,{\theta }^{2}}\right)$,所以

$$
{ET} = E\left( {\mathop{\sum }\limits_{{i = 1}}^{3}{a}_{i}{N}_{i}}\right)  = {a}_{1}E{N}_{1} + {a}_{2}E{N}_{2} + {a}_{3}E{N}_{3}
$$

$$
= {a}_{1}n\left( {1 - \theta }\right)  + {a}_{2}n\left( {\theta  - {\theta }^{2}}\right)  + {a}_{3}n{\theta }^{2}
$$

$$
= n{a}_{1} + n\left( {{a}_{2} - {a}_{1}}\right) \theta  + n\left( {{a}_{3} - {a}_{2}}\right) {\theta }^{2}
$$

由 $T$ 是 $\theta$ 的无偏估计量,可知 ${ET} = \theta$,

则 $\left\{  \begin{array}{l} n{a}_{1} = 0, \\  n\left( {{a}_{2} - {a}_{1}}\right)  = 1, \\  n\left( {{a}_{3} - {a}_{2}}\right)  = 0, \end{array}\right.$ 即 $\left\{  \begin{array}{l} {a}_{1} = 0, \\  {a}_{2} = \frac{1}{n}, \\  {a}_{3} = \frac{1}{n}. \end{array}\right.$

故 $T = 0 \times  {N}_{1} + \frac{1}{n} \times  {N}_{2} + \frac{1}{n} \times  {N}_{3} = \frac{1}{n}\left( {{N}_{2} + {N}_{3}}\right)  = \frac{1}{n}\left( {n - {N}_{1}}\right)$.

${DT} = D\left\lbrack  {\frac{1}{n}\left( {n - {N}_{1}}\right) }\right\rbrack   = \frac{1}{{n}^{2}}D{N}_{1} = \frac{1}{{n}^{2}} \cdot  n \cdot  \left( {1 - \theta }\right)  \cdot  \theta  = \frac{1}{n}\theta \left( {1 - \theta }\right).$

【4.15】设 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$ 是来自均值为 $\theta$ 的指数分布总体的样本,其中 $\theta$ 未知. 设有估计量

$$
{T}_{1} = \frac{1}{6}\left( {{X}_{1} + {X}_{2}}\right)  + \frac{1}{3}\left( {{X}_{3} + {X}_{4}}\right),\;{T}_{2} = \frac{{X}_{1} + 2{X}_{2} + 3{X}_{3} + 4{X}_{4}}{5},
$$

$$
{T}_{3} = \frac{{X}_{1} + {X}_{2} + {X}_{3} + {X}_{4}}{4}.
$$

(1) 指出 ${T}_{1},{T}_{2},{T}_{3}$ 中哪几个是 $\theta$ 的无偏估计量;

(2)在上述 $\theta$ 的无偏估计中指出哪一个较为有效.

解 (1) $E{T}_{1} = \frac{1}{6}\left( {E{X}_{1} + E{X}_{2}}\right)  + \frac{1}{3}\left( {E{X}_{3} + E{X}_{4}}\right)  = \frac{1}{6}\left( {\theta  + \theta }\right)  + \frac{1}{3}\left( {\theta  + \theta }\right)  = \theta$,

$$
E{T}_{2} = \frac{1}{5}\left( {E{X}_{1} + {2E}{X}_{2} + {3E}{X}_{3} + {4E}{X}_{4}}\right)  = \frac{1}{5}\left( {\theta  + {2\theta } + {3\theta } + {4\theta }}\right)  = {2\theta },
$$

$$
E{T}_{3} = \frac{1}{4}\left( {E{X}_{1} + E{X}_{2} + E{X}_{3} + E{X}_{4}}\right)  = \frac{1}{4}\left( {\theta  + \theta  + \theta  + \theta }\right)  = \theta.
$$

故 ${T}_{1},{T}_{3}$ 为 $\theta$ 的无偏估计量.

(2) $D{T}_{1} = \frac{1}{36}\left( {D{X}_{1} + D{X}_{2}}\right)  + \frac{1}{9}\left( {D{X}_{3} + D{X}_{4}}\right)  = \frac{1}{36}\left( {{\theta }^{2} + {\theta }^{2}}\right)  + \frac{1}{9}\left( {{\theta }^{2} + {\theta }^{2}}\right)  = \frac{5}{18}{\theta }^{2}$,

$$
D{T}_{3} = \frac{1}{16}\left( {D{X}_{1} + D{X}_{2} + D{X}_{3} + D{X}_{4}}\right)  = \frac{1}{16}\left( {{\theta }^{2} + {\theta }^{2} + {\theta }^{2} + {\theta }^{2}}\right)  = \frac{1}{4}{\theta }^{2},
$$

$D{T}_{1} > D{T}_{3}$.

故 ${T}_{3}$ 较 ${T}_{1}$ 更有效.

【4.16】设 $\widehat{\theta }$ 是参数 $\theta$ 的无偏估计,且有 $D\left( \widehat{\theta }\right)  > 0$,试证 ${\left( \widehat{\theta }\right) }^{2}$ 不是 ${\theta }^{2}$ 的无偏估计.

证 $E\left( {\widehat{\theta }}^{2}\right)  = D\left( \widehat{\theta }\right)  + {\left( E\widehat{\theta }\right) }^{2} = D\left( \widehat{\theta }\right)  + {\theta }^{2} > {\theta }^{2}\;\left( {D\left( \widehat{\theta }\right)  > 0}\right)$,

所以 ${\widehat{\theta }}^{2}$ 不是 ${\theta }^{2}$ 的无偏估计量.

【4.17】设总体 $X$ 的均值为 $\mu$,统计量 ${\widehat{\mu }}_{1}$ 和 ${\widehat{\mu }}_{2}$ 是参数 $\mu$ 的两个无偏估计量,它们的方差分别为 ${\sigma }_{1}^{2},{\sigma }_{2}^{2}$,相关系数为 $\rho$,试确定常数 ${c}_{1} > 0,{c}_{2} > 0,{c}_{1} + {c}_{2} = 1$,使得 ${c}_{1}\overset{\Lambda }{{\mu }_{1}} + {c}_{2}\overset{\Lambda }{{\mu }_{2}}$ 有最小方差.

解 $D\left( {{c}_{1}{\overset{\Lambda }{\mu }}_{1} + {c}_{2}{\overset{\Lambda }{\mu }}_{2}}\right)  = {c}_{1}^{2}D\left( {\overset{\Lambda }{\mu }}_{1}\right)  + {c}_{2}^{2}D\left( {\overset{\Lambda }{\mu }}_{2}\right)  + 2{c}_{1}{c}_{2}\operatorname{Cov}\left( {{\overset{\Lambda }{\mu }}_{1},{\overset{\Lambda }{\mu }}_{2}}\right)$

$$
= {c}_{1}^{2}{\sigma }_{1}^{2} + {c}_{2}^{2}{\sigma }_{2}^{2} + 2{c}_{1}{c}_{2}\rho {\sigma }_{1}{\sigma }_{2},
$$

利用高等数学知识,求 $D\left( {{c}_{1}{\widehat{\mu }}_{1} + {c}_{2}{\widehat{\mu }}_{2}}\right)$ 在 ${c}_{1} + {c}_{2} = 1\left( {{c}_{1} > 0,{c}_{2} > 0}\right)$ 条件下的最小值点,一种方法是使用拉格朗日乘数法,另一种方法是将 ${c}_{2} = 1 - {c}_{1}$ 代入化成无条件极值问题,最终解得

$$
{c}_{1} = \frac{{\sigma }_{2}\left( {{\sigma }_{2} - \rho {\sigma }_{1}}\right) }{{\sigma }_{1}^{2} - {2\rho }{\sigma }_{1}{\sigma }_{2} + {\sigma }_{2}^{2}},\;{c}_{2} = \frac{{\sigma }_{1}\left( {{\sigma }_{1} - \rho {\sigma }_{2}}\right) }{{\sigma }_{1}^{2} - {2\rho }{\sigma }_{1}{\sigma }_{2} + {\sigma }_{2}^{2}}.
$$

此时 ${c}_{1}{\widehat{\mu }}_{1} + {c}_{2}{\widehat{\mu }}_{2}$ 的方差达到最小.

【4.18】设总体 $X \sim  U\left( {\theta,{2\theta }}\right)$,其中 $\theta  > 0$ 是未知参数,又 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为取自该总体的样本,证明 $\widehat{\theta } = \frac{2}{3}\bar{X}$ 是 $\theta$ 的无偏估计和相合估计.

证

$$
E\left( \widehat{\theta }\right)  = \frac{2}{3}E\left( \bar{X}\right)  = \frac{2}{3}E\left( X\right)  = \frac{2}{3} \cdot  \frac{\theta  + {2\theta }}{2} = \theta,
$$

故 $\widehat{\theta }$ 是 $\theta$ 的无偏估计.

$$
D\left( \widehat{\theta }\right)  = \frac{4}{9}D\left( \bar{X}\right)  = \frac{4}{9} \cdot  \frac{D\left( X\right) }{n} = \frac{4}{9n} \cdot  \frac{{\theta }^{2}}{12} = \frac{{\theta }^{2}}{27n}.
$$

当 $n \rightarrow  \infty$ 时, $D\left( \widehat{\theta }\right)  \rightarrow  0$,故 $\widehat{\theta }$ 是 $\theta$ 的相合估计.

【4.19】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是总体为 $N\left( {\mu,{\sigma }^{2}}\right)$ 的简单随机样本,记

$$
\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i},\;{S}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2},\;T = {\bar{X}}^{2} - \frac{1}{n}{S}^{2},
$$

(1)证明 $T$ 是 ${\mu }^{2}$ 的无偏估计量；

(2)当 $\mu  = 0,\sigma  = 1$ 时,求 ${DT}$.

证 $\left( 1\right) E\left( T\right)  = E\left( {{\bar{X}}^{2} - \frac{1}{n}{S}^{2}}\right)  = E{\bar{X}}^{2} - E\left( {\frac{1}{n}{S}^{2}}\right)  = E{\bar{X}}^{2} - \frac{1}{n}{\sigma }^{2}$,

因为: $X \sim  N\left( {\mu,{\sigma }^{2}}\right),\bar{X} \sim  N\left( {\mu,\frac{{\sigma }^{2}}{n}}\right)$,而

$$
E{\bar{X}}^{2} = D\bar{X} + {\left( E\bar{X}\right) }^{2} = \frac{1}{n}{\sigma }^{2} + {\mu }^{2},\;E\left( T\right)  = \frac{1}{n}{\sigma }^{2} + {\mu }^{2} - \frac{1}{n}{\sigma }^{2} = {\mu }^{2},
$$

所以 $T$ 是 ${\mu }^{2}$ 的无偏估计.

解 (2) ${DT} = E{T}^{2} - {\left( ET\right) }^{2}, E\left( T\right)  = 0, E{T}^{2} = E\left( {{\bar{X}}^{4} - \frac{2}{n}{\bar{X}}^{2} \cdot  {S}^{2} + \frac{{S}^{4}}{{n}^{2}}}\right)$,

因为 $\bar{X} \sim  N\left( {0,\frac{1}{n}}\right),\frac{\bar{X}}{\frac{1}{\sqrt{n}}} \sim  N\left( {0,1}\right)$,

令 $X = \frac{\bar{X}}{\frac{1}{\sqrt{n}}}, E\left( {X}^{4}\right)  = {\int }_{-\infty }^{+\infty }\frac{{x}^{4}}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x = {\int }_{-\infty }^{+\infty }\frac{3{x}^{2}}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x = {3E}{X}^{2} = 3$,

所以 $E{\bar{X}}^{4} = \frac{3}{{n}^{2}}$,

$$
E\left( {\frac{2}{n}{\bar{X}}^{2} \cdot  {S}^{2}}\right)  = \frac{2}{n}E{\bar{X}}^{2} \cdot  E{S}^{2} = \frac{2}{n}\left\lbrack  {D\bar{X} + {\left( E\bar{X}\right) }^{2}}\right\rbrack   = \frac{2}{n}\left( {\frac{1}{n} + 0}\right)  = \frac{2}{{n}^{2}},
$$

$$
E\left( \frac{{S}^{4}}{{n}^{2}}\right)  = \frac{1}{{n}^{2}}E{S}^{4},\;E{S}^{4} = D{S}^{2} + {\left( E{S}^{2}\right) }^{2} = D{S}^{2} + 1.
$$

因为 $W = \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)$,且 ${\sigma }^{2} = 1$,

所以 ${DW} = {\left( n - 1\right) }^{2}D{S}^{2} = 2\left( {n - 1}\right), D{S}^{2} = \frac{2}{n - 1}, E{S}^{4} = \frac{2}{n - 1} + 1 = \frac{n + 1}{n - 1}$,

故 $E{T}^{2} = \frac{3}{{n}^{2}} - \frac{2}{{n}^{2}} + \frac{1}{{n}^{2}} \cdot  \frac{n + 1}{n - 1} = \frac{2}{n\left( {n - 1}\right) }$.

#### 题型 2: 关于区间估计

【4.20】从长期生产实践知道,某厂生产的 ${100}\mathrm{\;W}$ 灯泡的使用寿命 $X \sim  N\left( {\mu,{100}^{2}}\right)$ (单位: h), 现从某一批灯泡中抽取 5 只, 测得使用寿命如下:

$\begin{array}{lllll} {1455} & {1502} & {1370} & {1610} & {1430} \end{array}$

试求这批灯泡平均使用寿命 $\mu$ 的置信区间 ( $\alpha$ 分别为 0.1 和 0.05).

解 由样本值得

$$
\bar{X} = \frac{1}{5}\left( {{1455} + {1502} + {1370} + {1610} + {1430}}\right)  = {1473.4},
$$

当 $\alpha  = {0.1}$,查表得 ${u}_{\frac{\alpha }{2}} = {1.64}$,故

$$
\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}} = {1473.4} - {1.64} \times  \frac{100}{\sqrt{5}} = {1400.1},
$$

$$
\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}} = {1473.4} + {1.64} \times  \frac{100}{\sqrt{5}} = {1546.7},
$$

于是置信度 90% 下,平均使用寿命 $\mu$ 的置信区间为 [1400.1,1546.7].

当 $\alpha  = {0.05}$ 时,查表得 ${u}_{\frac{\alpha }{2}} = {1.96}$,故

$$
\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}} = {1473.4} - {1.96} \times  \frac{100}{\sqrt{5}} = {1385.7},
$$

$$
\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}} = {1473.4} + {1.96} \times  \frac{100}{\sqrt{5}} = {1561.1},
$$

于是置信度 95% 下,平均使用寿命 $\mu$ 的置信区间为[1385.7,1561.1].

【4.21】设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),{x}_{1},{x}_{2},\cdots,{x}_{15}$ 是其一组样本值,已知

$$
\mathop{\sum }\limits_{{i = 1}}^{{15}}{x}_{i} = {8.7},\;\mathop{\sum }\limits_{{i = 1}}^{{15}}{x}_{i}^{2} = {25.05},
$$

求置信水平为 0.95 的 $\mu$ 和 ${\sigma }^{2}$ 的置信区间.

解 $\bar{x} = \frac{1}{15}\mathop{\sum }\limits_{{i = 1}}^{{15}}{x}_{i} = \frac{1}{15} \times  {8.7} = {0.58}$,

$$
{S}^{2} = \frac{1}{14}\mathop{\sum }\limits_{{i = 1}}^{{15}}{\left( {x}_{i} - \bar{x}\right) }^{2} = \frac{1}{14}\left( {\mathop{\sum }\limits_{{i = 1}}^{{15}}{x}_{i}^{2} - {15}{\bar{x}}^{2}}\right)  = {1.429},
$$

查表得 ${t}_{\frac{\alpha }{2}}\left( {n - 1}\right)  = {t}_{0.025}\left( {14}\right)  = {2.1448}$,

$$
{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right)  = {\chi }_{0.975}^{2}\left( {14}\right)  = {5.629},\;{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right)  = {\chi }_{0.025}^{2}\left( {14}\right)  = {26.119}\text{,}
$$

代入公式可得置信区间为

$$
\mu  : \left\lbrack  {\bar{X} \pm  {t}_{\frac{\alpha }{2}}\left( {n - 1}\right) \frac{S}{\sqrt{n}}}\right\rbrack   = \left\lbrack  {-{0.082},{1.242}}\right\rbrack ,
$$

$$
{\sigma }^{2} : \left\lbrack  {\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) },\;\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}\right\rbrack   = \left\lbrack  {{0.766},{3.554}}\right\rbrack .
$$

【4.22】假如0.50,1.25,0.80,2.00是来自总体 $X$ 的简单随机样本值,已知 $Y = \ln X$ 服从正态分布 $N\left( {\mu,1}\right)$.

(1)求 $X$ 的数学期望 ${EX}$ (记 ${EX}$ 为 $b$ );

(2)求 $\mu$ 的置信度为 0.95 的置信区间；

(3)利用上述结果求 $b$ 的置信度为 0.95 的置信区间.

分析 本题是一个正态总体方差已知时求期望值 $\mu$ 的置信区间问题. 在 $\mu$ 的置信区间解得的情况下,利用 $b$ 的表达式中含有 $\mu$ 这一特点,代入 $\mu$ 的置信区间即可得 $b$ 的置信区间.

解 (1) 由题意知 $Y$ 的概率密度为

$$
f\left( y\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{\left( y - \mu \right) }^{2}}{2}}.
$$

又由 $Y = \ln X$,得 $X = {\mathrm{e}}^{Y}$,故

$$
b = {EX} = E{\mathrm{e}}^{Y} = {\int }_{-\infty }^{+\infty }\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{y}{\mathrm{e}}^{-\frac{{\left( y - \mu \right) }^{2}}{2}}\mathrm{\;d}y
$$

$$
= {\mathrm{e}}^{\mu  + \frac{1}{2}}{\int }_{-\infty }^{+\infty }\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{1}{2}{\left\lbrack  y - \left( \mu  + 1\right) \right\rbrack  }^{2}}\mathrm{\;d}y = {\mathrm{e}}^{\mu  + \frac{1}{2}}.
$$

(2)经过分析, $\mu$ 的置信区间公式为 $\left( {\bar{Y} - \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}},\bar{Y} + \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}}}\right)$.

由 $1 - \alpha  = {0.95}$,查表得 ${u}_{\frac{\alpha }{2}} = {1.96}$.

代入 $\sigma  = 1, n = 4,\bar{y} = \frac{1}{4}\left( {\ln {0.5} + \ln {1.25} + \ln {0.8} + \ln 2}\right)  = 0$,

得 $\left( {-\frac{1}{2} \times  {1.96},\frac{1}{2} \times  {1.96}}\right)$.

故 $\mu$ 的置信度为 0.95 的置信区间为 $\left( {-{0.98},{0.98}}\right)$.

(3)由(1)可知, $b = {EX} = {\mathrm{e}}^{\mu  + \frac{1}{2}}$,又由(2)知, $\mu$ 的置信区间为(-0.98,0.98),

因为 ${\mathrm{e}}^{x}$ 为严格增函数,所以 $b$ 的置信区间为 $\left( {{\mathrm{e}}^{-{0.98} + \frac{1}{2}},{\mathrm{e}}^{{0.98} + \frac{1}{2}}}\right)$,

即为 $\left( {{\mathrm{e}}^{-{0.48}},{\mathrm{e}}^{1.48}}\right)$.

【4.23】随机地取某种炮弹 9 发做实验,得炮口速度的样本标准差 $s = {11}\left( {\mathrm{\;m}/\mathrm{s}}\right)$,设炮口速度服从正态分布,求这种炮弹的炮口速度的标准差 $\sigma$ 的置信度为 0.95 的置信区间.

解 由 ${\sigma }^{2}$ 的置信区间公式知, $\sigma$ 的置信度为 0.95 的置信区间为

$$
\left( {\frac{\sqrt{n - 1}S}{\sqrt{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) }},\frac{\sqrt{n - 1}S}{\sqrt{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}}\right).
$$

其中 $s = {11}, n - 1 = 8,1 - \alpha  = {0.95},\alpha  = {0.05},\frac{\alpha }{2} = {0.025}$.

查表得 ${\chi }_{\frac{\alpha }{2}}^{2}\left( 8\right)  = {17.535},{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( 8\right)  = {2.180}$,代入得到 $\sigma$ 的置信区间为 $\left( {{7.4},{21.1}}\right)$.

【4.24】分别使用金球和铂球测定引力常数 (单位: ${10}^{-{11}}{\mathrm{\;m}}^{3} \cdot  {\mathrm{{kg}}}^{-1} \cdot  {\mathrm{s}}^{-1}$ ).

(1)用金球测定观察值为6.683,6.681,6.676,6.678,6.679,6.672.

(2)用铂球测定观察值为6.661,6.661,6.667,6.667,6.664.

设测定值总体为 $N\left( {\mu,{\sigma }^{2}}\right),\mu,{\sigma }^{2}$ 均为未知,试就 (1),(2) 两种情况分别求 $\mu$ 的置信度为 0.9 的置信区间,并求 ${\sigma }^{2}$ 的置信度为 0.9 的置信区间.

解 (1) $\mu,{\sigma }^{2}$ 均未知时, $\mu$ 的置信度为 0.9 的置信区间为

$$
\left\lbrack  {\bar{X} - \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right),\bar{X} + \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right) }\right\rbrack ,
$$

这里 $1 - \alpha  = {0.9},\alpha  = {0.1},\frac{\alpha }{2} = {0.05},{n}_{1} = 6,{n}_{2} = 5,{n}_{1} - 1 = 5,{n}_{2} - 1 = 4$.

$$
{\bar{x}}_{1} = \frac{1}{6}\mathop{\sum }\limits_{{i = 1}}^{6}{x}_{i} = \frac{1}{6}\left( {{6.683} + \cdots  + {6.672}}\right)  = {6.678},
$$

$$
{s}_{1}^{2} = \frac{1}{5}\mathop{\sum }\limits_{{i = 1}}^{6}{\left( {x}_{i} - {\bar{x}}_{1}\right) }^{2} = {0.15} \times  {10}^{-4},
$$

$$
{\bar{x}}_{2} = \frac{1}{5}\mathop{\sum }\limits_{{i = 1}}^{5}{x}_{i} = \frac{1}{5}\left( {{6.661} + \cdots  + {6.664}}\right)  = {6.664},
$$

$$
{s}_{2}^{2} = \frac{1}{4}\mathop{\sum }\limits_{{i = 1}}^{5}{\left( {x}_{i} - {\bar{x}}_{2}\right) }^{2} = {0.9} \times  {10}^{-5},
$$

$$
{t}_{\frac{\alpha }{2}}\left( 5\right)  = {2.0150},{t}_{\frac{\alpha }{2}}\left( 4\right)  = {2.1318}.
$$

代入得,用金球测定时, $\mu$ 的置信区间是 $\left\lbrack  {{6.675},{6.681}}\right\rbrack$.

用铂球测定时, $\mu$ 的置信区间为 $\left\lbrack  {{6.661},{6.667}}\right\rbrack$.

(2) $\mu,{\sigma }^{2}$ 均未知时, ${\sigma }^{2}$ 的置信度为 0.9 的置信区间为

$$
\left\lbrack  {\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right) },\;\frac{\left( {n - 1}\right) {S}^{2}}{{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( {n - 1}\right) }}\right\rbrack ,
$$

这里 ${n}_{1} - 1 = 5,{n}_{2} - 1 = 4,\frac{\alpha }{2} = {0.05}$.

查表得: ${\chi }_{\frac{\alpha }{2}}^{2}\left( 5\right)  = {11.071},{\chi }_{\frac{\alpha }{2}}^{2}\left( 4\right)  = {9.488},{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( 5\right)  = {1.145},{\chi }_{1 - \frac{\alpha }{2}}^{2}\left( 4\right)  = {0.711}$.

将这些值以及上面 (1) 中算得的 ${S}_{1}^{2},{S}_{2}^{2}$ 代入上区间得

用金球测定时, ${\sigma }^{2}$ 的置信区间是 $\left\lbrack  {{6.774} \times  {10}^{-6},{6.550} \times  {10}^{-5}}\right\rbrack$.

用铂球测定时, ${\sigma }^{2}$ 的置信区间是 $\left\lbrack  {{3.794} \times  {10}^{-6},{5.063} \times  {10}^{-5}}\right\rbrack$.

【4.25】设 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 为来自总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 的简单随机样本,样本均值 $\bar{x} = {9.5}$,参数 $\mu$ 的置信度为 0.95 的双侧置信区间的置信上限为 10.8,则 $\mu$ 的置信度为 0.95 的双侧置信区间为 _____.

解 设 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,其中 ${\sigma }^{2}$ 未知,则 $\mu$ 的置信区间为

$$
\left( {\bar{x} - {t}_{\frac{\alpha }{2}}\left( {n - 1}\right) \frac{S}{\sqrt{n}},\bar{x} + {t}_{\frac{\alpha }{2}}\left( {n - 1}\right) \frac{S}{\sqrt{n}}}\right).
$$

已知 $\bar{x} = {9.5}$,置信上限为 10.8,则

${t}_{\frac{\alpha }{2}}\left( {n - 1}\right) \frac{S}{\sqrt{n}} = {1.3}$,置信下限为 8.2.

故应填 $\left( {{8.2},{10.8}}\right)$.

【4. 26】设某种清漆的 9 个样品,其干燥时间(单位:h) 分别为

$\begin{array}{lllllllll} {6.0} & {5.7} & {5.8} & {6.5} & {7.0} & {6.3} & {5.6} & {6.1} & {5.0} \end{array}$

设干燥时间总体服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$,求 $\mu$ 的置信度为 0.95 的置信区间.

(1)若由以往经验知 $\sigma  = {0.6}$ (小时);

(2)若 $\sigma$ 为未知.

解 (1) 当方差 ${\sigma }^{2}$ 已知时, $\mu$ 的置信度为 0.95 的置信区间为

$$
\left\lbrack  {\bar{X} - \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}},\;\bar{X} + \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}}}\right\rbrack ,
$$

这里, $1 - \alpha  = {0.95},\alpha  = {0.05},\frac{\alpha }{2} = {0.025}, n = 9,\sigma  = {0.6},\bar{x} = \frac{1}{9}\left( {{6.0} + {5.7} + \cdots  + {5.0}}\right)  = 6$,

查正态分布表得 ${u}_{\frac{\alpha }{2}} = {1.96}$.

将这些值代入公式得 $\left\lbrack  {{5.608},{6.392}}\right\rbrack$.

(2)当方差 ${\sigma }^{2}$ 未知时, $\mu$ 的置信度为 0.95 的置信区间为

$$
\left\lbrack  {\bar{X} - \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right),\;\bar{X} + \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right) }\right\rbrack ,
$$

这里, $1 - \alpha  = {0.95},\alpha  = {0.05},\frac{\alpha }{2} = {0.025}, n - 1 = 8$.

查表得 ${t}_{\frac{\alpha }{2}}\left( {n - 1}\right)  = {2.3060}$,

$$
\bar{x} = \frac{1}{9}\left( {{6.0} + {5.7} + \cdots  + {5.0}}\right)  = 6,\;{s}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \bar{x}\right) }^{2} = {0.33}.
$$

将这些值代入公式得 $\left\lbrack  {{5.558},{6.442}}\right\rbrack$.

【4.27】随机地从 $A$ 批导线中抽取 4 根,又从 $B$ 批导线中抽取 5 根,测得电阻 (单位: $\Omega$ ) 为

$A$ 批导线: 0.143 0.142 0.143 0.137

$B$ 批导线: $\begin{array}{lllll} {0.140} & {0.142} & {0.136} & {0.138} & {0.140} \end{array}$

设测定数据分别来自分布 $N\left( {{\mu }_{1},{\sigma }^{2}}\right), N\left( {{\mu }_{2},{\sigma }^{2}}\right)$,且两样本相互独立,又 ${\mu }_{1},{\mu }_{2},{\sigma }^{2}$ 均为未知, 试求 ${\mu }_{1} - {\mu }_{2}$ 的置信度为 0.95 的置信区间.

解 ${\mu }_{1} - {\mu }_{2}$ 的置信区间为

$$
\left\lbrack  {\bar{X} - \bar{Y} - {t}_{\frac{\alpha }{2}}\left( {{n}_{1} + {n}_{2} - 2}\right) {S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}},\;\bar{X} - \bar{Y} + {t}_{\frac{\alpha }{2}}\left( {{n}_{1} + {n}_{2} - 2}\right) {S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}}\right\rbrack ,
$$

在这里 $\bar{X} = \frac{1}{4}\mathop{\sum }\limits_{{i = 1}}^{4}{Xi} = \frac{1}{4}\left( {{0.143} + \cdots  + {0.137}}\right)  = {0.1413}$,

$$
\bar{Y} = \frac{1}{5}\left( {{0.140} + \cdots  + {0.140}}\right)  = {0.1392},
$$

$$
{n}_{1} = 4,{n}_{2} = 5,{n}_{1} + {n}_{2} - 2 = 7;1 - \alpha  = {0.95},\alpha  = {0.05},\frac{\alpha }{2} = {0.025}\text{.}
$$

查表得 ${t}_{\frac{\alpha }{2}}\left( 7\right)  = {2.3646}$,

$$
{s}_{w}^{2} = \frac{\left( {{n}_{1} - 1}\right) {s}_{1}^{2} + \left( {{n}_{2} - 1}\right) {s}_{2}^{2}}{{n}_{1} + {n}_{2} - 2} = {6.509} \times  {10}^{-6},\;{s}_{w} = \sqrt{{6.509} \times  {10}^{-6}} = {2.551} \times
$$

${10}^{-3}$.

将这些值代入上区间得 $\left( {-{0.002},{0.006}}\right)$.

【4.28】研究两种固体燃料火箭推进器的燃烧率, 设两者都服从正态分布, 并且已知燃烧率的标准差均近似地为 ${0.05}\mathrm{\;{cm}}/\mathrm{s}$,取样本容量为 ${n}_{1} = {n}_{2} = {20}$,得燃烧率的样本均值分别为 ${x}_{1} =$ ${18}\mathrm{\;{cm}}/\mathrm{s},{x}_{2} = {24}\mathrm{\;{cm}}/\mathrm{s}$,求两燃烧率总体均值差 ${\mu }_{1} - {\mu }_{2}$ 的置信度为 0.99 的置信区间.

解 在此题中, ${\sigma }_{1} = {\sigma }_{2} = {0.05}$,因此, ${\mu }_{1} - {\mu }_{2}$ 的置信度为 0.99 的置信区间

$$
\left( {{\bar{X}}_{1} - {\bar{X}}_{2} - {u}_{\frac{\alpha }{2}}\sigma \sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}},\;{\bar{X}}_{1} - {\bar{X}}_{2} + {u}_{\frac{\alpha }{2}}\sigma \sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}}\right),
$$

这里 ${n}_{1} = {n}_{2} = {20},\alpha  = {0.01},\frac{\alpha }{2} = {0.005}$.

查表得 ${u}_{\frac{\alpha }{2}} = {2.58}$. 代入上区间得 $\left( {-{6.04}, - {5.96}}\right)$.

【4.29】设两位化验员 $A, B$ 独立地对某种聚合物含氯量用相同的方法各作 10 次测定,其测定值的样本方差依次为 ${S}_{A}^{2} = {0.5419},{S}_{B}^{2} = {0.6065}$. 设 ${\sigma }_{A}^{2},{\sigma }_{B}^{2}$ 分别为 $A, B$ 所测定的测定值总体的方差,设总体均为正态分布,求方差比 $\frac{{\sigma }_{A}^{2}}{{\sigma }_{B}^{2}}$ 的置信度为 0.95 的置信区间.

解 $\frac{{\sigma }_{A}^{2}}{{\sigma }_{B}^{2}}$ 的置信区间为

$$
\left\lbrack  {\frac{{S}_{A}^{2}}{{S}_{B}^{2}}\frac{1}{{F}_{\frac{\alpha }{2}}\left( {{n}_{1} - 1,{n}_{2} - 1}\right) },\;\frac{{S}_{A}^{2}}{{S}_{B}^{2}}\frac{1}{{F}_{1 - \frac{\alpha }{2}}\left( {{n}_{1} - 1,{n}_{2} - 1}\right) }}\right\rbrack ,
$$

这里 $1 - \alpha  = {0.95},\alpha  = {0.05},\frac{\alpha }{2} = {0.025}$. 查表得 ${F}_{\frac{\alpha }{2}}\left( {9,9}\right)  = {4.03},{F}_{1 - \frac{\alpha }{2}}\left( {9,9}\right)  = \frac{1}{4.03}$.

代入上式得 $\left( {{0.222},{3.601}}\right)$.

【4. 30】(1)求【4. 26】题中 $\mu$ 的置信度为 0.95 的单侧置信上限；

(2)求【4.27】题中 ${\mu }_{1} - {\mu }_{2}$ 的置信度为 0.95 的单侧置信下限；

(3)求【4.29】题中方差比 $\frac{{\sigma }_{A}^{2}}{{\sigma }_{B}^{2}}$ 的置信度为 0.95 的单侧置信上限.

解 (1) ${\sigma }^{2}$ 已知时,此时 $\frac{\bar{X} - \mu }{\frac{\sigma }{\sqrt{n}}} \sim  N\left( {0,1}\right)$,于是

$$
P\left\{  {\frac{\bar{X} - \mu }{\frac{\sigma }{\sqrt{n}}} > {u}_{1 - \alpha }}\right\}   = 1 - \alpha,\;\text{ 即 }\;P\left\{  {\frac{\bar{X} - \mu }{\frac{\sigma }{\sqrt{n}}} >  - {u}_{\alpha }}\right\}   = 1 - \alpha.
$$

于是, $\mu$ 的置信度为 $1 - \alpha$ 的单侧置信区间为 $\left( {-\infty,\bar{X} + {u}_{\alpha } \cdot  \frac{\sigma }{\sqrt{n}}}\right)$. 则 $\bar{X} + {u}_{\alpha } \cdot  \frac{\sigma }{\sqrt{n}}$ 为其单侧置信上限. 此时 $\alpha  = {0.05}$,查表得 ${u}_{\alpha } = {1.65},\bar{X} = 6,\sigma  = {0.6}, n =$

1. 代入上式得 $\bar{\mu } = \bar{x} + {u}_{\alpha } \cdot  \frac{\sigma }{\sqrt{n}} = {6.33}$.

方差 ${\sigma }^{2}$ 未知,此时 $\frac{\bar{X} - \mu }{\frac{S}{\sqrt{n}}} \sim  t\left( {n - 1}\right)$. 于是 $P\left\{  {\frac{\bar{X} - \mu }{\frac{S}{\sqrt{n}}} > {t}_{1 - \alpha }\left( {n - 1}\right) }\right\}   = 1 - \alpha$,得

$$
\frac{\bar{X} - \mu }{\frac{S}{\sqrt{n}}} > {t}_{1 - \alpha }\left( {n - 1}\right),\;\mu  < \bar{X} - {t}_{1 - \alpha }\left( {n - 1}\right) \frac{S}{\sqrt{n}} = \bar{X} + {t}_{\alpha }\left( {n - 1}\right) \frac{S}{\sqrt{n}}.
$$

此处 $\bar{X} = 6,{S}^{2} = {0.33}, n = 9$. 查表得 ${t}_{0.05}\left( 8\right)  = {1.8598}$.

代入上式得 $\bar{\mu } = \bar{x} + {t}_{\alpha }\left( {n - 1}\right)  \cdot  \frac{s}{\sqrt{n}} = {6.356}$.

(2) 未知,此时

$$
\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}} \sim  t\left( {{n}_{1} + {n}_{2} - 2}\right),
$$

$$
P\left\{  {\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}} < {t}_{\alpha }\left( {{n}_{1} + {n}_{2} - 2}\right) }\right\}   = 1 - \alpha  = {0.95},
$$

由此得 ${\mu }_{1} - {\mu }_{2}$ 的置信度为 0.95 的单侧置信下限为

$$
\bar{X} - \bar{Y} - {S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}} \cdot  {t}_{\alpha }\left( {{n}_{1} + {n}_{2} - 2}\right).
$$

将【4.27】题中的 $\bar{X},\bar{Y},{S}_{w}$ 代入上式得 $\left( {{t}_{\alpha }\left( {{n}_{1} + {n}_{2} - 2}\right)  = {1.8946}}\right)$,

$$
\bar{x} - \bar{y} - {s}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}} \cdot  {t}_{\alpha }\left( {{n}_{1} + {n}_{2} - 2}\right)  =  - {0.0012}.
$$

(3) 此时 $\frac{\frac{{S}_{1}^{2}}{{\sigma }_{1}^{2}}}{\frac{{S}_{2}^{2}}{{\sigma }_{2}^{2}}} \sim  F\left( {{n}_{1} - 1,{n}_{2} - 1}\right)$,于是

$$
P\left\{  {\frac{\frac{{S}_{1}^{2}}{{\sigma }_{1}^{2}}}{\frac{{S}_{2}^{2}}{{\sigma }_{2}^{2}}} > {F}_{1 - \alpha }\left( {{n}_{1} - 1,{n}_{2} - 1}\right) }\right\}   = 1 - \alpha,
$$

由此得 $\frac{{\sigma }_{1}^{2}}{{\sigma }_{2}^{2}}$ 的置信度为 0.95 的单侧置信上限为

$$
\frac{{S}_{1}^{2}}{{S}_{2}^{2}}\frac{1}{{F}_{1 - \alpha }\left( {{n}_{1} - 1,{n}_{2} - 1}\right) } = \frac{{S}_{1}^{2}}{{S}_{2}^{2}} \cdot  {F}_{\alpha }\left( {{n}_{2} - 1,{n}_{1} - 1}\right),
$$

查表得 ${F}_{\alpha }\left( {{n}_{2} - 1,{n}_{1} - 1}\right)  = {3.18}$.

将【4.29】题中的 ${S}_{1}^{2},{S}_{2}^{2}$ 值及 ${F}_{\alpha }\left( {{n}_{2} - 1,{n}_{1} - 1}\right)$ 代入上式得,单侧置信上限为 2.84.

【4.31】为研究某种汽车轮胎的磨损特性, 随机地选择 16 只轮胎, 每只轮胎行驶到磨坏为止, 记录所行驶路径(以公里计) 如下:

$\begin{array}{llllllll} {41250} & {40187} & {43175} & {41010} & {39265} & {41872} & {42654} & {41287} \end{array}$

$\begin{array}{llllllll} {38970} & {40200} & {42550} & {41095} & {40680} & {43500} & {39775} & {40400} \end{array}$

假设这些数据来自正态总体 $N\left( {\mu,{\sigma }^{2}}\right)$,其中 $\mu,{\sigma }^{2}$ 未知,试求 $\mu$ 的置信度为 0.95 的单侧置信下限.

解 $\sigma$ 未知,此时

$$
\frac{\bar{X} - \mu }{\frac{S}{\sqrt{n}}} \sim  t\left( {n - 1}\right),\;P\left\{  {\frac{\bar{X} - \mu }{\frac{S}{\sqrt{n}}} < {t}_{\alpha }\left( {n - 1}\right) }\right\}   = 1 - \alpha,
$$

由此得 $\mu$ 的置信度为 $1 - \alpha$ 的单侧置信下限为 $\bar{X} - {t}_{\alpha }\left( {n - 1}\right)  \cdot  \frac{S}{\sqrt{n}}$,

这里 $\bar{x} = \frac{1}{16}\left( {{41250} + \cdots  + {40400}}\right)  = {41117}, s = {1347}$,

查表得 ${t}_{0.05}\left( {15}\right)  = {1.7531}$,代入上式得 $\bar{x} - {t}_{\alpha }\left( {n - 1}\right)  \cdot  \frac{s}{\sqrt{n}} = {40526}$.

#### 题型 3: 与置信度、样本容量及区间长度有关的题目

【4.32】从正态总体 $N\left( {\mu,{6}^{2}}\right)$ 中抽取容量为 $n$ 的样本. 若保证 $\mu$ 的 95% 的置信区间的长度不大于 2,问 $n$ 至少应取多大?

解 由 ${\sigma }^{2} = {6}^{2}$ 得 $\frac{\bar{X} - \mu }{6}\sqrt{n} \sim  N\left( {0,1}\right)$,故置信区间为

$$
\left\lbrack  {\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}},\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}}\right\rbrack .
$$

从而得均值 $\mu$ 的置信区间的长度为

$$
2{u}_{\frac{\alpha }{2}} \cdot  \frac{\sigma }{\sqrt{n}} \leq  2
$$

即 $n \geq  {\left( {u}_{\frac{\alpha }{2}} \cdot  \sigma \right) }^{2} = {\left( {1.96} \times  6\right) }^{2} \approx  {139}$.

【4.33】设总体 $X \sim  N\left( {\mu,8}\right),\left( {{X}_{1},\cdots,{X}_{36}}\right)$ 为其简单随机样本,若 $\left\lbrack  {\bar{X} - 1,\bar{X} + 1}\right\rbrack$ 作为 $\mu$ 的置信区间,则置信度为_____.

解 本题属于已知 ${\sigma }^{2}$,估计 $\mu$ 的类型.

$\mu$ 的满足置信度为 $1 - \alpha$ 的置信区间应为

$$
\left\lbrack  {\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}},\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}}\right\rbrack .
$$

由题意, ${u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}} = 1$,且 $\sigma  = \sqrt{8}, n = {36}$.

故 ${u}_{\frac{\alpha }{2}} = {2.12}$,查表可得置信度 $1 - \alpha  = {0.966}$.

【4.34】设 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),{\sigma }^{2}$ 已知,若样本容量 $n$ 和置信度 $1 - \alpha$ 均不变,则对于不同的样本观测值, $\mu$ 的置信区间长度(   ).

(A) 变长 (B) 变短 (C) 保持不变 (D) 不能确定

解 $\mu$ 的置信区间是

$$
\left\lbrack  {\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}},\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}}\right\rbrack ,
$$

因为 $n$ 和 $1 - \alpha$ 不变,所以长度 $l = 2{u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}$ 保持不变.

故应选(C).

【4.35】设样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 的样本,其中 $\mu,{\sigma }^{2}$ 为未知参数,设随机变量 $L$ 是关于 $\mu$ 的置信度为 $1 - \alpha$ 的置信区间的长度,求 $E\left( {L}^{2}\right)$.

解 取 $T = \frac{\bar{X} - \mu }{S}\sqrt{n}$,则 $T \sim  t\left( {n - 1}\right)$.

由 $P\left\{  {\left| T\right|  < {t}_{\frac{\alpha }{2}}\left( {n - 1}\right) }\right\}   = 1 - \alpha$ 可得 $\mu$ 的 $1 - \alpha$ 置信区间为

$$
\left( {\bar{X} - {t}_{\frac{\alpha }{2}}\left( {n - 1}\right)  \cdot  \frac{S}{\sqrt{n}},\;\bar{X} + {t}_{\frac{\alpha }{2}}\left( {n - 1}\right)  \cdot  \frac{S}{\sqrt{n}}}\right),
$$

易见区间长度 $L = 2{t}_{\frac{\alpha }{2}}\left( {n - 1}\right)  \cdot  \frac{S}{\sqrt{n}}$,

故 $E\left( {L}^{2}\right)  = E\left\lbrack  {4{t}_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right)  \cdot  \frac{{S}^{2}}{n}}\right\rbrack   = \frac{4}{n}{t}_{\frac{\alpha }{2}}^{2}\left( {n - 1}\right)  \cdot  {\sigma }^{2}$.

【4.36】假定到某地旅游的一个游客的消费额 $X$ 服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$,且 $\sigma  = {500}$, $\mu$ 未知. 要对平均消费额 $\mu$ 进行估计,使这个估计的绝对误差小于 50 元,且置信度不小于 0.95, 问至少需要随机调查多少个游客?

解 本题是求样本容量的最小值,因此,不妨设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是取自该总体的样本. 样本均值为 $\bar{X}$,且已知 $\widehat{\mu } = \bar{X}$,依题意,即可由 $P\{ \left| {\bar{X} - \mu }\right|  < {50}\}  \geq  {0.95}$ 去求最小样本容量.

设 $n$ 为需要调查的游客人数,要使

$$
P\{ \left| {\bar{X} - \mu }\right|  < {50}\}  \geq  {0.95},\text{ 即 }P\left\{  {\frac{\left| \bar{X} - \mu \right| }{\frac{\sigma }{\sqrt{n}}} < \frac{50}{\frac{\sigma }{\sqrt{n}}}}\right\}   \geq  {0.95},
$$

因为 $\frac{\bar{X} - \mu }{\frac{\sigma }{\sqrt{n}}} = U \sim  N\left( {0,1}\right)$,由 $P\left\{  {\left| U\right|  < {u}_{\frac{\alpha }{2}}}\right\}   = 1 - \alpha  = {0.95}$,其中 $\alpha  = {0.05}$,得

$$
\frac{50}{\frac{\sigma }{\sqrt{n}}} \geq  {u}_{\frac{0.05}{2}} \Rightarrow  \sqrt{n} \geq  \frac{1.96\sigma }{50} \Rightarrow  n \geq  {\left( \frac{1.96\sigma }{50}\right) }^{2} = {\left( \frac{{1.96} \times  {500}}{50}\right) }^{2} = {384.16}\text{.}
$$

这就是随机调查游客人数不少于 385 人,就有不小于 0.95 的把握,使得用调查所得的 $\bar{x}$ 去估计平均消费额的真相 $\mu$,其绝对误差小于 50 元.

