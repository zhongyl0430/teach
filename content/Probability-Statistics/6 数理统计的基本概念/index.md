---
title: 第六章 数理统计的基本概念
---
数理统计是统计学的重要分支, 具有广泛的应用. 大家知道, 现场统计是流水账式的统计, 它记录所有发生的结果, 比如一个生产班组的领取原料的件数或数量、产品件数及各项指标等都一一作记录. 再比如一批产品的各个产品的每项技术指标都作记录. 数理统计有别于现场统计的最本质特征可以概括为 “用局部推断整体”. 比如,从一批产品中抽取 $n$ 件做检验后,来推断该批产品的合格品率. 这就使得数理统计所作推断的结论不可避免地存在偏差或错误, 而刻画或把握这种偏差的有效方法就是概率论. 概率论通过给出各种各样的统计量所服从的分布或数字特征, 来演绎地评价各种统计方法的优劣或置信程度. 一般来讲, 数理统计的方法大多来自简单的直观想法或概率论的有关基本事实 (比如大数定律、中心极限定理或某些渐近分布), 而要评价这些方法则需要比较艰深的概率论推导或证明.

本章介绍数理统计的基本概念, 包括总体、样本、统计量等, 着重介绍三种重要的分布,即 ${\chi }^{2}$ 分布、 $t$ 分布和 $F$ 分布,并介绍正态总体的样本均值、样本方差及其有关统计量的分布.

## 6.1 总体、样本和统计量

### 6.1.1 总体与样本

前面我们已经提到, 数理统计的基本特征是用局部推断整体. 这个整体在数理统计中我们称之为总体, 也就是为了某一目的而要研究的对象的全体, 而将每个对象称为个体. 但是, 实际中我们往往关心的研究对象某方面的数量特征, 比如灯泡的寿命、一台机器正常工作的持续时间、某种药物的疗效等. 由于在对一个个体进行试验或观测结束之前, 我们无法预知该数量的取值, 这一点类似于我们前节所介绍的随机变量. 所以, 我们可以认为总体就是一个随机变量, 每次试验后, 获得的一个个体的具体取值就是该随机变量的一次观测值. 另外, 若我们准备抽取 $n$ 个个体进行试验或观测,会得到 $n$ 个数值,我们称之为样本. 但在试验或观测结束之前, 也无法预知各个的取值, 所以从概率分析的角度讲, 样本是一个随机变量.

总之,我们以后所说的总体,就是一个随机变量 $X$,通常记 $X$ 的分布函数为 ${F}_{X}\left( {\cdot,\theta }\right)$,其中 $\theta  \in  \Theta$ 为参数, $\Theta$ 称为参数空间,它可能包含多个参数. 样本为 $n$ 维随机向量 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right), n$ 称为样本容量. 样本的一次具体取值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 称为样本观测值. 数理统计就是从样本出发,推断总体的分布或数字特征. 为处理方便,初等数理统计中都假定 ${X}_{i}\left( {i = 1,2,\cdots, n}\right)$ 与 $X$ 同分布, 且相互独立. 此时我们称 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为简单随机样本,简称为样本.

基于以上讨论和随机变量独立性的定义 (定义 3.1.3) 和定理 3.1.2, 我们有命题 6.1.1.

命题 6.1.1 设总体 $X \sim  {F}_{X}\left( {\cdot,\theta }\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本,则

$$
{F}_{{X}_{1},{X}_{2},\cdots,{X}_{n}}\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\theta }\right)  = {F}_{X}\left( {{x}_{1},\theta }\right) {F}_{X}\left( {{x}_{2},\theta }\right) \cdots {F}_{{X}_{n}}\left( {x,\theta }\right), \tag{6.1.1}
$$

其中的 ${F}_{X}\left( {\cdot,\theta }\right)$ 可以是分布函数,也可以是分布密度函数 (对于连续型随机变量) 或概率分布 (对于离散型随机变量).

例 6.1.1 设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本,则 $\left( {{X}_{1},{X}_{2},\cdots }\right.$, $\left. {X}_{n}\right)$ 的联合分布密度函数为

$$
{f}_{{X}_{1},{X}_{2},\cdots,{X}_{n}}\left( {{x}_{1},{x}_{2},\cdots,{x}_{n};\mu,{\sigma }^{2}}\right)
$$

$$
= {f}_{X}\left( {{x}_{1},\mu,{\sigma }^{2}}\right) {f}_{X}\left( {{x}_{2},\mu,{\sigma }^{2}}\right) \cdots {f}_{X}\left( {{x}_{n},\mu,{\sigma }^{2}}\right)
$$

$$
= \frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{-\frac{{\left( {x}_{1} - \mu \right) }^{2}}{2{\sigma }^{2}}} \cdot  \frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{-\frac{{\left( {x}_{2} - \mu \right) }^{2}}{2{\sigma }^{2}}}\cdots \frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{-\frac{{\left( {x}_{n} - \mu \right) }^{2}}{2{\sigma }^{2}}}
$$

$$
= {\left( 2\pi {\sigma }^{2}\right) }^{-\frac{n}{2}}\exp \left( {-\frac{1}{2{\sigma }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \mu \right) }^{2}}\right).
$$

### 6.1.2 统计量

按上所述,总体 $X$ 是我们研究的目标,而出发点是样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$, 那么研究的途径或手段就是所谓的统计量. 它的直观意思是要通过对样本观测值的处理, 来回答或推断总体的分布、数字特征、参数等. 所以统计量就是样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的一个函数,但其中不能含未知参数,否则由观测值得不出任何结果.

常用的统计量有以下几种:

(1) 样本均值: $\bar{X} = \frac{1}{n}\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}\right)  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$. R 软件中用 mean(x) 来计算,其中 $\mathrm{x}$ 为样本观测值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ (下同).

(2) 样本方差: ${S}_{n}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} \cdot  \mathrm{R}$ 软件中用 $\mathrm{n}/\left( {\mathrm{n} - 1}\right)  * \operatorname{var}\left( \mathrm{x}\right)$ 来计算. 修正样本方差: ${S}_{n}^{*2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} \cdot  \mathrm{R}$ 软件中用 $\operatorname{var}\left( \mathrm{x}\right)$ 来计算. 显然, $n{S}_{n}^{2} = \left( {n - 1}\right) {S}_{n}^{*2}$.

(3) 样本 $k$ 阶原点矩: $\overline{{X}^{k}} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{k}$.

(4) 样本 $k$ 阶中心矩: $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{k}$.

(5) 顺序统计量: ${X}_{\left( 1\right) } \leq  {X}_{\left( 2\right) } \leq  \cdots  \leq  {X}_{\left( n\right) }$,其中 ${X}_{\left( 1\right) } = \min \left\{  {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right\}$, ${X}_{\left( n\right) } = \max \left\{  {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right\}$,而 ${X}_{\left( k\right) }$ 是将 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 的取值从小到大排列第 $k$ 位的值.

(6) 样本中位数:

$$
\widetilde{X} = \left\{  \begin{array}{ll} {X}_{\left( \frac{n + 1}{2}\right) }, & \text{ 若 }n\text{ 为奇数,} \\  \frac{1}{2}\left( {{X}_{\left( \frac{n}{2}\right) } + {X}_{\left( \frac{n}{2} + 1\right) }}\right), & \text{ 若 }n\text{ 为偶数. } \end{array}\right.
$$

$\mathrm{R}$ 软件中用 median(x)来计算.

(7) 样本极差: ${R}_{n}^{X} = {X}_{\left( n\right) } - {X}_{\left( 1\right) } \cdot  \mathrm{R}$ 软件中用 $\max \left( \mathrm{x}\right)  - \min \left( \mathrm{x}\right)$ 来计算.

## 6.2 经验分布函数

前已指出, 数理统计的核心任务是 “从局部推断整体”, 具体地讲, 从样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 出发,推断总体 $X$ 的统计特性. 在中学教材中,大家学过的频率直方图就是一种用样本观测值近似拟合总体分布密度函数的直观方法. 那么, 从理论上讲,从局部能够推断整体吗? 或者说样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 何时才能近似反映总体 $X$ 的特性呢?

本节所介绍的经验分布的逼近性质从理论上给出了肯定的答案.

设总体 $X$ 的样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的一次观测值为 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$,将其从小到大排列为 ${x}_{\left( 1\right) } \leq  {x}_{\left( 2\right) } \leq  \cdots  \leq  {x}_{\left( n\right) }$. 令

$$
{F}_{n}^{X}\left( x\right)  = \left\{  \begin{matrix} 0, & x < {x}_{\left( 1\right) }, \\  \frac{1}{n}, & {x}_{\left( 1\right) } \leq  x < {x}_{\left( 2\right) }, \\  \vdots & \vdots \\  \frac{k}{n}, & {x}_{\left( k\right) } \leq  x < {x}_{\left( k + 1\right) }, \\  \vdots & \vdots \\  1, & {x}_{\left( n\right) } > {x}_{\left( n\right) }. \end{matrix}\right.
$$

称 ${F}_{n}^{X}$ 为总体 $X$ 的一个经验分布函数 (或样本分布函数).

设总体 $X$ 的分布函数为 ${F}_{X}$,利用伯努利大数定律 (参见推论 5.1.1) 容易证明,对任意 $\varepsilon  > 0$,有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\left| {{F}_{n}^{X}\left( x\right)  - {F}_{X}\left( x\right) }\right|  \geq  \varepsilon }\right)  = 0,\;\forall x \in  \left( {-\infty,\infty }\right). \tag{6.2.1}
$$

另外,格里汶科 $\left( {\Gamma }_{\text{JIMBEHKO }}\right)$ 证明了更强的结果,即

$$
P\left( {\mathop{\lim }\limits_{{n \rightarrow  \infty }}\mathop{\sup }\limits_{{-\infty  < x < \infty }}\left| {{F}_{n}^{X}\left( x\right)  - {F}_{X}\left( x\right) }\right|  = 0}\right)  = 1. \tag{6.2.2}
$$

以上的事实 (6.2.1) 和 (6.2.2) 都表明,当样本容量 $n$ 足够大时,经验分布函数与总体的分布函数差距很小. 这从理论上说明, 当样本容量较大时, 近似推断总体是可能的.

## 6.3 抽样分布

为了用概率方法来探讨一个统计量在推断总体时的性能或把握推断结论的置信程度, 我们必须要知道统计量的分布或近似分布. 所以我们下面先讨论一些具体统计量的分布, 通常称为抽样分布.

我们先讨论统计量的数字特征.

### 6.3.1 样本均值与样本方差的数字特征

${\sigma }^{2}$. 则 命题 6.3.1 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是来自总体 $X$ 的样本, $E\left\lbrack  X\right\rbrack   = \mu,\operatorname{Var}\left\lbrack  X\right\rbrack   =$

(1)

$$
E\left\lbrack  \bar{X}\right\rbrack   = \mu,\;\operatorname{Var}\left\lbrack  \bar{X}\right\rbrack   = \frac{{\sigma }^{2}}{n}; \tag{6.3.1}
$$

(2)

$$
E\left\lbrack  {S}_{n}^{2}\right\rbrack   = \frac{n - 1}{n}{\sigma }^{2},\;E\left\lbrack  {S}_{n}^{*2}\right\rbrack   = {\sigma }^{2}. \tag{6.3.2}
$$

证明 (1) $E\left\lbrack  \bar{X}\right\rbrack   = E\left\lbrack  {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right\rbrack   = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E\left\lbrack  {X}_{i}\right\rbrack   = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\mu  = \mu$.

$$
\operatorname{Var}\left\lbrack  \bar{X}\right\rbrack   = \operatorname{Var}\left\lbrack  {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right\rbrack   = \frac{1}{{n}^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}\operatorname{Var}\left\lbrack  {X}_{i}\right\rbrack   = \frac{1}{{n}^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{\sigma }^{2} = \frac{{\sigma }^{2}}{n}.
$$

(2) 由于

$$
{S}_{n}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{X}_{i}^{2} - 2\bar{X} \cdot  {X}_{i} + {\bar{X}}^{2}}\right)
$$

$$
= \frac{1}{n}\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - 2\bar{X} \cdot  \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} + n{\bar{X}}^{2}}\right)
$$

$$
= \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - {\bar{X}}^{2}
$$

所以

$$
E\left\lbrack  {S}_{n}^{2}\right\rbrack   = E\left\lbrack  {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - {\bar{X}}^{2}}\right\rbrack   = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E\left\lbrack  {X}_{i}^{2}\right\rbrack   - E\left\lbrack  {\bar{X}}^{2}\right\rbrack
$$

$$
= \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left( {\operatorname{Var}\left\lbrack  {X}_{i}\right\rbrack   + {\left( E\left\lbrack  {X}_{i}\right\rbrack  \right) }^{2}}\right)  - \left( {\operatorname{Var}\left\lbrack  \bar{X}\right\rbrack   + E{\left\lbrack  \bar{X}\right\rbrack  }^{2}}\right)
$$

$$
= \frac{1}{n}\left( {n{\sigma }^{2} + n{\mu }^{2}}\right)  - \frac{{\sigma }^{2}}{n} - {\mu }^{2}
$$

$$
= \frac{n - 1}{n}{\sigma }^{2}.
$$

$$
E\left\lbrack  {S}_{n}^{*2}\right\rbrack   = E\left\lbrack  {\frac{n}{n - 1}{S}_{n}^{2}}\right\rbrack   = \frac{n}{n - 1}E\left\lbrack  {S}_{n}^{2}\right\rbrack   = {\sigma }^{2}.
$$

### 6.3.2 三种重要的概率分布

#### 1. ${\chi }^{2}$ 分布

在例 2.4.2 中我们提到,若 $X \sim  N\left( {0,1}\right)$,则

$$
{X}^{2} \sim  \Gamma \left( {\frac{1}{2},\frac{1}{2}}\right). \tag{6.3.3}
$$

一般地,若 $X$ 的分布密度为

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{{\lambda }^{\alpha }}{\Gamma \left( \alpha \right) }{x}^{\alpha  - 1}{\mathrm{e}}^{-{\lambda x}}, & x > 0, \\  0, & \text{ 其他. } \end{array}\right.  \tag{6.3.4}
$$

则称 $X$ 服从参数为 $\alpha  > 0$ 和 $\lambda  > 0$ 的 $\Gamma$ 分布,记为 $X \sim  \Gamma \left( {\alpha,\lambda }\right),\mathrm{R}$ 软件中的分

布名为 gamma. 此时

$$
E\left\lbrack  X\right\rbrack   = \frac{\alpha }{\lambda },\;\operatorname{Var}\left\lbrack  X\right\rbrack   = \frac{\alpha }{{\lambda }^{2}}. \tag{6.3.5}
$$

利用 3.4 节给出的独立随机变量和的分布密度的卷积公式 (3.4.5), 经简单推导可得 $\Gamma$ 分布的可加性,即若 ${X}_{1} \sim  \Gamma \left( {{\alpha }_{1},\lambda }\right),{X}_{2} \sim  \Gamma \left( {{\alpha }_{2},\lambda }\right)$,且 ${X}_{1}$ 与 ${X}_{2}$ 相互

独立, 则

(6.3.6)

$$
{X}_{1} + {X}_{2} \sim  \Gamma \left( {{\alpha }_{1} + {\alpha }_{2},\lambda }\right).
$$

由式 (6.3.3) 和式 (6.3.6) 我们得到命题 6.3.2.

命题 6.3.2 设总体 $X \sim  N\left( {0,1}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其简单随机样本,则

$$
{X}_{1}^{2} + {X}_{2}^{2} + \cdots  + {X}_{n}^{2} \sim  \Gamma \left( {\frac{n}{2},\frac{1}{2}}\right). \tag{6.3.7}
$$

在数理统计中,若 $X \sim  \Gamma \left( {\frac{n}{2},\frac{1}{2}}\right)$,则称 $X$ 服从自由度为 $n$ 的 ${\chi }^{2}$ 分布,记为 $X \sim  {\chi }^{2}\left( n\right),\mathrm{R}$ 软件中的分布名为 chisq,其分布密度函数为

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{{2}^{n}\Gamma \left( \frac{n}{2}\right) }{x}^{\frac{n}{2} - 1}{\mathrm{e}}^{-x/2}, & x > 0; \\  0, & \text{ 其他. } \end{array}\right.  \tag{6.3.8}
$$

图形如图 6.1 所示.

![01938b00-6b6a-7014-9166-35043ab11e9a_104_588_544_433_268_0.jpg](teach/Probability-Statistics/images/01938b00-6b6a-7014-9166-35043ab11e9a_104_588_544_433_268_0.jpg)

图 ${6.1}{\chi }^{2}\left( n\right)$ 分布密度函数示意图

由式 (6.3.5) 和式 (6.3.6) 容易看出 ${\chi }^{2}$ 分布具有如下性质:

(1) 若 $X \sim  {\chi }^{2}\left( n\right)$,则 $E\left\lbrack  X\right\rbrack   = n,\operatorname{Var}\left\lbrack  X\right\rbrack   = {2n}$.

(2) 若 ${X}_{1} \sim  {\chi }^{2}\left( {n}_{1}\right),{X}_{2} \sim  {\chi }^{2}\left( {n}_{2}\right)$,则 ${X}_{1} + {X}_{2} \sim  {\chi }^{2}\left( {{n}_{1} + {n}_{2}}\right)$.

另外, 利用命题 6.3.2 和中心极限定理 (定理 5.2.1) 容易看出

(3) 若 $X \sim  {\chi }^{2}\left( n\right)$ 分布,则当 $n$ 趋于无穷时, $\left( {X - n}\right) /\sqrt{2n}$ 近似地服从 $N\left( {0,1}\right)$.

#### 2. $t$ 分布

命题 6.3.3 设 $X \sim  N\left( {0,1}\right), Y \sim  {\chi }^{2}\left( n\right)$,且 $X$ 与 $Y$ 相互独立,令

$$
T = \frac{X}{\sqrt{Y/n}}
$$

则 $T$ 的分布密度函数 ${f}_{T}$ 为

$$
{f}_{T}\left( x\right)  = \frac{\Gamma \left( \frac{n + 1}{2}\right) }{\sqrt{n\pi }\Gamma \left( \frac{n}{2}\right) }{\left( 1 + \frac{{x}^{2}}{2}\right) }^{-\frac{n + 1}{2}}. \tag{6.3.9}
$$

命题 6.3.3 的证明也是初等的,但需稍繁的积分计算,我们在此从略. 若 $X$ 的分布密度函数如 (6.3.9),则称 $X$ 服从自由度为 $n$ 的 $t$ 分布,记为 $t\left( n\right) \mathrm{B}$ 软件中的分布名为 $\mathrm{t}$.

$t\left( n\right)$ 分布的密度函数图形如图 6.2 所示,它是关于原点对称的. 简单的求极限可知,当 $n \rightarrow  \infty$ 时, $t\left( n\right)$ 分布渐近于 $N\left( {0,1}\right)$. 另外,经简单积分可知,若

$X \sim  t\left( n\right)$,则

$$
E\left\lbrack  X\right\rbrack   = 0\left( {n > 1}\right),\;\operatorname{Var}\left\lbrack  X\right\rbrack   = \frac{2}{n - 2}\left( {n > 2}\right). \tag{6.3.10}
$$

![01938b00-6b6a-7014-9166-35043ab11e9a_105_621_290_378_273_0.jpg](teach/Probability-Statistics/images/01938b00-6b6a-7014-9166-35043ab11e9a_105_621_290_378_273_0.jpg)

图 ${6.2t}\left( n\right)$ 分布密度函数示意图

3. $F$ 分布

命题 6.3.4 若 $X \sim  {\chi }^{2}\left( m\right), Y \sim  {\chi }^{2}\left( n\right)$,且 $X$ 与 $Y$ 独立. 令

$$
Z = \frac{X/m}{Y/n}
$$

则 $Z$ 的分布密度函数为

$$
{f}_{Z}\left( x\right)  = \left\{  \begin{array}{ll} \frac{\Gamma \left( \frac{m + n}{2}\right) }{\Gamma \left( \frac{m}{2}\right) \Gamma \left( \frac{n}{2}\right) }{m}^{m/2}{n}^{n/2}\frac{{x}^{\frac{m}{2} - 1}}{{\left( mx + n\right) }^{\left( {m + n}\right) /2}}, & x > 0. \\  0, & x \leq  0. \end{array}\right.  \tag{6.3.11}
$$

命题 6.3.4 的证明中用到的积分计算稍繁,我们在此从略. 若 $Z$ 的分布密度函数如式 (6.3.11),则称 $Z$ 所服从的分布为 第一自由度为 $m$ 、第二自由度为 $n$ 的 $F$ 分布,记为 $Z \sim  F\left( {m, n}\right),\mathrm{R}$ 软件中的分布名为 $\mathrm{f}.F$ 分布的密度函数如图 6.3 所示,显然 $F$ 分布具有性质:

![01938b00-6b6a-7014-9166-35043ab11e9a_105_612_1257_436_346_0.jpg](teach/Probability-Statistics/images/01938b00-6b6a-7014-9166-35043ab11e9a_105_612_1257_436_346_0.jpg)

图 ${6.3}\;F\left( {m, n}\right)$ 分布密度函数示意图

若 $Z \sim  F\left( {m, n}\right)$,则 $\frac{1}{Z} \sim  F\left( {n, m}\right)$.

### 6.3.3 分位数

在统计推断过程中 (比如后文介绍的参数的区间估计和假设检验中). 已知总体 $X$ 的分布及某概率值 $\alpha$,需要知道 $X$ 小于和等于哪个数的概率为 $\alpha$. 这个数称为 $X$ 的 $\alpha$ 分位数,亦即,

设 $X \sim  \psi \left( n\right)$ ( $\psi$ 为某种分布, $n$ 为有关自由度), $0 < \alpha  < 1$. 称满足

$$
P\left( {X \leq  {\psi }_{\alpha }\left( n\right) }\right)  = \alpha
$$

的数 ${\psi }_{\alpha }\left( n\right)$ 为分布 $\psi \left( n\right)$ 的 $\alpha$ 分位数 (或分位点)

几种常用分布的分位数如图 6.4 - 图 6.7 所示.

![01938b00-6b6a-7014-9166-35043ab11e9a_106_364_577_398_292_0.jpg](teach/Probability-Statistics/images/01938b00-6b6a-7014-9166-35043ab11e9a_106_364_577_398_292_0.jpg)

图 ${6.4N}\left( {0,1}\right)$ 分布分位点示意图.

![01938b00-6b6a-7014-9166-35043ab11e9a_106_857_649_403_235_0.jpg](teach/Probability-Statistics/images/01938b00-6b6a-7014-9166-35043ab11e9a_106_857_649_403_235_0.jpg)

图 ${6.5}{\chi }^{2}\left( n\right)$ 分布分位点示意图.

![01938b00-6b6a-7014-9166-35043ab11e9a_106_350_976_408_263_0.jpg](teach/Probability-Statistics/images/01938b00-6b6a-7014-9166-35043ab11e9a_106_350_976_408_263_0.jpg)

图 ${6.6t}\left( n\right)$ 分布分位点示意图.

![01938b00-6b6a-7014-9166-35043ab11e9a_106_854_1029_386_222_0.jpg](teach/Probability-Statistics/images/01938b00-6b6a-7014-9166-35043ab11e9a_106_854_1029_386_222_0.jpg)

图 ${6.7}\;F\left( {m, n}\right)$ 分布分位点示意图.

由于 $N\left( {0,1}\right),{\chi }^{2}\left( n\right), t\left( n\right)$ 和 $F\left( {m, n}\right)$ 的分布密度函数的积分较为复杂 (或个可能),有关概率的计算只能查表,这些表是经数值计算得到的. 如用 $\mathrm{R}$ 软件则不用查表, 而是调用专门的分位数函数, 它们的格式是 quantile(分位数) 的第一个字母 q 后续分布名及圆括弧 (   ) 内写概率值 $\alpha$ 和有关参数值,如 qnorm $\left( \alpha \right)$. $\mathrm{{qt}}\left( {\alpha,\mathrm{n}}\right),\mathrm{{qf}}\left( {\alpha,\mathrm{m},\mathrm{n}}\right)$ 等.

如需查表, 我们需要说明几点:

(i) 对于 $t\left( n\right)$ 分布,由于当 $n$ 趋于无穷时,其极限分布为 $N\left( {0,1}\right)$,所以自由度较大时,用标准正态分布的分位数 ${u}_{\alpha }$ 代替 ${t}_{\alpha }\left( n\right)$ 的分位数.

(ii) 若 $X \sim  {\chi }^{2}\left( n\right)$ 分布,则当 $n$ 趋于无穷时, $\left( {X - n}\right) /\sqrt{2n}$ 近似地服从 $N\left( {0,1}\right)$,所以当自由度较大时,近似地有 ${\chi }_{\alpha }^{2}\left( n\right)  = {u}_{\alpha }\sqrt{2n} + n$.

(iii) 对于 $F\left( {m, n}\right)$ 分布和 $\alpha \left( {0 < \alpha  < 1}\right)$,有 ${F}_{\alpha }\left( {m, n}\right)  = 1/{F}_{1 - \alpha }\left( {n, m}\right)$.

例 6.3.1 查表或用 R 软件,求

(1) ${\chi }_{0.99}^{2}\left( {10}\right),{\chi }_{0.05}^{2}\left( {20}\right)$ 和 ${\chi }_{0.95}^{2}\left( {60}\right)$.

(2) ${t}_{0.95}\left( {10}\right),{t}_{0.10}\left( {20}\right)$ 和 ${t}_{0.90}\left( {50}\right)$.

(3) ${F}_{0.99}\left( {5,4}\right),{F}_{0.05}\left( {3,7}\right)$.

解 (1)

$$
{\chi }_{0.99}^{2}\left( {10}\right)  = \operatorname{qchisq}\left( {{0.99},{10}}\right)  = {23.20925},
$$

$$
{\chi }_{0.05}^{2}\left( {20}\right)  = \operatorname{qchisq}\left( {{0.05},{20}}\right)  = {10.85081},
$$

$$
{\chi }_{0.95}^{2}\left( {60}\right)  = \text{ qchisq }\left( {{0.95},{60}}\right)  = {79.08194}.
$$

查表时,一般查不到 ${\chi }_{0.95}^{2}\left( {60}\right)$,而是用正态分布近似,即 ${\chi }_{\alpha }^{2}\left( n\right)  \approx  {u}_{\alpha }\sqrt{2n} + n$.

$$
{\chi }_{0.95}^{2}\left( {60}\right)  \approx  \text{ qnorm }\left( {0.95}\right) \sqrt{2 \times  {60}} + {60} = {78.01847}.
$$

(2)

$$
{t}_{0.95}\left( {10}\right)  = \operatorname{qt}\left( {{0.95},{10}}\right)  = {1.812461},
$$

$$
{t}_{0.10}\left( {20}\right)  = \mathrm{{qt}}\left( {{0.10},{20}}\right)  =  - {1.325341},
$$

$$
{t}_{0.90}\left( {50}\right)  = \operatorname{qt}\left( {{0.90},{50}}\right)  = {1.298714}.
$$

查表时,一般查不到 ${t}_{0.90}\left( {50}\right)$,而是用正态分布近似,即 ${t}_{\alpha }\left( n\right)  \approx  {u}_{\alpha }$.

$$
{t}_{0.90}\left( {50}\right)  \approx  {u}_{0.90} = \text{ qnorm }\left( {0.90}\right)  = {1.281552}.
$$

(3)

$$
{F}_{0.99}\left( {5,4}\right)  = \operatorname{qf}\left( {{0.99},5,4}\right)  = {15.52186},
$$

$$
{F}_{0.05}\left( {3,7}\right)  = \operatorname{qf}\left( {{0.05},3,7}\right)  = {0.1125272}.
$$

查表时,一般查不到 ${F}_{0.05}\left( {3,7}\right)$,而是用 ${F}_{\alpha }\left( {m, n}\right)  = 1/{F}_{1 - \alpha }\left( {n, m}\right)$,

$$
{F}_{0.05}\left( {3,7}\right)  = \frac{1}{{F}_{0.95}\left( {7,3}\right) } = \frac{1}{\operatorname{qf}\left( {{0.95},7,3}\right) } = {0.1125272}.
$$

### 6.3.4 正态总体的抽样分布

定理 6.3.1 (抽样分布基本定理) 设总体 $X \sim  N\left( {0,1}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本,则样本均值 $\bar{X} \sim  N\left( {0,\frac{1}{n}}\right), n{S}_{n}^{2} \sim  {\chi }^{2}\left( {n - 1}\right)$,并且 $\bar{X}$ 与 ${S}_{n}^{2}$ 相互独立.

由于篇幅限制, 我们略去定理 6.3.1 的证明, 但从中我们看到正态分布的极

(1) 由于 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 独立且都服从正态分布,从而 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 服从 $n$ 维正态分布. 由命题 3.4.1 知, $\bar{X} = \frac{1}{n}{X}_{1} + \frac{1}{n}{X}_{2} + \cdots  + \frac{1}{n}{X}_{n}$ 服从正态分布.

(2) ${S}_{n}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}$,即 ${S}_{n}^{2}$ 是 $\bar{X}$ 的函数,二者却相互独立.

从定理 6.3.1 的事实出发, 利用命题 6.3.2、命题 6.3.3 和命题 6.3.4 中给出的 ${\chi }^{2}$ 分布、 $t$ 分布和 $F$ 分布的定义,容易证明如下四个推论,它们在后文的分析过论中将发挥关键性的作用.

相互独立, 开且 推论 6.3.1 设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本,则 $\bar{X}$ 与 ${S}_{n}^{2}$

$$
\bar{X} \sim  N\left( {\mu,\frac{{\sigma }^{2}}{n}}\right), \tag{6.3.12}
$$

$$
\frac{n{S}_{n}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)  \tag{6.3.13}
$$

推论 6.3.2 设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为其样本,则

$$
\frac{\bar{X} - \mu }{{S}_{n}^{ * }}\sqrt{n} = \frac{\bar{X} - \mu }{{S}_{n}}\sqrt{n - 1} \sim  t\left( {n - 1}\right). \tag{6.3.14}
$$

推论 6.3.3 设总体 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{m}}\right)$ 为其样本. 样本均值为 $X$,样本方差为 ${S}_{1m}^{2}$; 另有与 $X$ 独立的总体 $Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right),\left( {{Y}_{1},{Y}_{2},\cdots,{Y}_{m}}\right)$ 为具样本,样本均值为 $\bar{Y}$,样本方差为 ${S}_{2m}^{2}$. 则

$$
\frac{m{S}_{1m}^{2}}{n{S}_{2n}^{2}} \cdot  \frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \cdot  \frac{n - 1}{m - 1} = \frac{{S}_{1m}^{*2}}{{S}_{2n}^{*2}} \cdot  \frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} \sim  F\left( {m - 1, n - 1}\right). \tag{6.3.15}
$$

推论 6.3.4 在推论 6.3.3 的假定中,若 ${\sigma }_{1}^{2} = {\sigma }_{2}^{2}$,则

$$
\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{m} + \frac{1}{n}}} \sim  t\left( {m + n - 2}\right), \tag{6.3.16}
$$

其中 ${S}_{w} = \sqrt{\frac{m{S}_{1m}^{2} + n{S}_{2n}^{2}}{m + n - 2}}$.

对于顺序统计量, 用初等概率论的一般方法, 容易证明命题 6.3.5.

命题 6.3.5 设总体 $X$ 的分布函数为 ${F}_{X}$,分布密度函数为 ${f}_{X}$,则

$$
{f}_{{X}_{\left( k\right) }}\left( x\right)  = \frac{n!}{\left( {n - k}\right) !\left( {k - 1}\right) !}{\left\lbrack  {F}_{X}\left( x\right) \right\rbrack  }^{k - 1}{\left\lbrack  1 - {F}_{X}\left( x\right) \right\rbrack  }^{n - k}{f}_{X}\left( x\right),\;k = 1,2,\cdots, n.
$$

(6.3.17)特别地,

$$
{f}_{{X}_{\left( 1\right) }}\left( x\right)  = n{\left\lbrack  1 - {F}_{X}\left( x\right) \right\rbrack  }^{n - 1}{f}_{X}\left( x\right), \tag{6.3.18}
$$

$$
{f}_{{X}_{\left( n\right) }}\left( x\right)  = n{\left\lbrack  {F}_{X}\left( x\right) \right\rbrack  }^{n - 1}{f}_{X}\left( x\right). \tag{6.3.19}
$$

## 第六章小结与注记

(1)总体与样本是数理统计最基本的两个概念,其直观意义很明确. 但只有把它们归结为一个随机变量和一个随机向量, 才便于对统计方法和结果作概率上的分析论证. 基于数学工具的限制, 我们不得不限制样本为 “简单随机样本”, 亦即, 各分量间相互独立, 且都与总体同分布. 试想一批产品有 100 件, 从中抽取 10 件做检验, 来推断该批产品的不合格品率. 有放回抽取较为准确还是无放回较为准确？有放回抽取是独立试验还是无放回抽取是独立试验？

我们说, 数理统计就是 “由局部推断整体”. 现在就可以具体化为: 总体是数理统计的研究目标, 而样本是数理统计的出发点.

(2)统计量则是由出发点到目标的途径. 直观上, 统计量就是样本的函数, 也就是要对样本经过处理才能说明总体. 当然, 直观和理论上, 我们都不希望它包含未知参数, 否则就得不出结果, 一切都是徒劳的.

(3)由于我们通过统计量来说明总体,所以把握统计量的统计特性就非常重要. 遗憾的是, 对于一般分布的总体, 其统计量的分布很难得到, 即使对样本均值和样本方差这样简单的统计量也是如此. 对这种总体的处理, 往往用 “大样本埋论”来研究, 即样本容量较大时, 通过求统计量的近似分布来完成对统计方法的

只有对正态总体, 其样本均值、样本方差的分布可以求得, 且二者独立 (见抽样分布基本定理),从而根据几个特殊的分布 $\left( {\chi }^{2}\right.$ 分布、 $t$ 分布和 $F$ 分布) 的定义, 我们得到了几种重要的样本函数的分布 (参见推论 6.2.1 - 推论 6.3.4), 它们在后续参数的区间估计和假设检验中起到关键作用.

(4)顺序统计量也有直观的应用, 但其分布往往难以求得, 甚至于正态总体的顺序统计量的分布都没有显式表达式. 一般较少用到.

## 第六章习题

6.1. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是来自总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 的样本,并设

$$
{T}_{1} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i},\;{T}_{2} = {T}_{1} - \mu,\;{T}_{3} = \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}}{{\sigma }^{2}},\;{T}_{4} = \frac{\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - {T}_{1}\right) }^{2}}{{\sigma }^{2}}.
$$

试在下列情形下指出哪些随机变量是统计量:

(1) 在 ${\sigma }^{2}$ 已知, $\mu$ 未知的情形下. (2) 在 $\mu,{\sigma }^{2}$ 均未知的情形下.

6.2. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{5}}\right)$ 是来自总体 $N\left( {0,4}\right)$ 的一个样本,且

$$
Y = a{X}_{1}^{2} + b{\left( 2{X}_{2} + 3{X}_{3}\right) }^{2} + c{\left( 4{X}_{4} - {X}_{5}\right) }^{2},
$$

问非零常数 $a, b, c$ 取何值时,随机变量 $Y$ 服从 ${\chi }^{2}$ 分布?

6.3. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{8}}\right)$ 是来自总体 $N\left( {0,1}\right)$ 的简单随机样本. 求常数 $c$,使得

$$
\frac{c\left( {{X}_{1}^{2} + {X}_{2}^{2}}\right) }{{\left( {X}_{3} + {X}_{4} + {X}_{5}\right) }^{2} + {\left( {X}_{6} + {X}_{7} + {X}_{8}\right) }^{2}}
$$

服从 $F$ 分布,并指出其自由度.

6.4. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{9}}\right)$ 是来自总体 $N\left( {0,1}\right)$ 的简单随机样本. 试确定正数 $c$. 使得 $\frac{c\left( {{X}_{1} + {X}_{2} + {X}_{3}}\right) }{\sqrt{{\left( {X}_{4} + {X}_{5}\right) }^{2} + {\left( {X}_{6} + {X}_{7}\right) }^{2} + {\left( {X}_{8} + {X}_{9}\right) }^{2}}}$ 服从 $t$ 分布,并指出其自由度.

6.5. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{10}}\right)$ 是来自总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 的一个样本,记

$$
\bar{X} = \frac{1}{9}\mathop{\sum }\limits_{{i = 1}}^{9}{X}_{i},\;{S}_{9}^{*2} = \frac{1}{8}\mathop{\sum }\limits_{{i = 1}}^{9}{\left( {X}_{i} - \bar{X}\right) }^{2},\;T = \frac{3\left( {{X}_{10} - \bar{X}}\right) }{{S}_{9}^{ * }\sqrt{10}}
$$

确定 $T$ 服从何种分布,并说明缘由.

6.6. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{20}}\right)$ 是来自总体 $X \sim  N\left( {0,1}\right)$ 的一个样本,记

$$
Y = \frac{1}{10}{\left( \mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}\right) }^{2} + \frac{1}{10}{\left( \mathop{\sum }\limits_{{i = {11}}}^{{20}}{X}_{i}\right) }^{2},
$$

试确定 $Y$ 所服从的分布.

6.7. 设总体 $X \sim  N\left( {0,{\sigma }^{2}}\right)$,从 $X$ 中抽得样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{14}}\right)$,记

$$
{Y}_{1} = \frac{1}{5}\mathop{\sum }\limits_{{i = 1}}^{5}{X}_{i},\;{Y}_{2} = \frac{1}{5}\mathop{\sum }\limits_{{i = {10}}}^{{14}}{X}_{i},\;{Z}_{1} = \mathop{\sum }\limits_{{i = 1}}^{5}{\left( {X}_{i} - {Y}_{1}\right) }^{2},
$$

$$
{Z}_{2} = \mathop{\sum }\limits_{{i = {10}}}^{{14}}{\left( {X}_{i} - {Y}_{2}\right) }^{2},\;{Z}_{3} = \mathop{\sum }\limits_{{i = 6}}^{9}{X}_{i}^{2},\;T = \frac{{Z}_{1} + {Z}_{2}}{2{Z}_{3}},
$$

确定 $T$ 服从何种分布,并说明缘由.

6.8. 设总体 $X \sim  \operatorname{Exp}\left( \lambda \right)$,从 $X$ 中抽取样本 $\left( {{X}_{1},{X}_{2}}\right)$,记

$$
{Y}_{1} = \min \left\{  {{X}_{1},{X}_{2}}\right\} ,\;{Y}_{2} = \max \left\{  {{X}_{1},{X}_{2}}\right\}
$$

求 (1) ${Y}_{1}$ 和 ${Y}_{2}$ 的分布密度函数. (2) $E{Y}_{1}, E{Y}_{2}$.

6.9. 设总体 $X$ 的密度函数为

$$
f\left( x\right)  = \left\{  \begin{matrix} {2x}, & 0 < x < 1, \\  0, & \text{ 其他. } \end{matrix}\right.
$$

$\left( {{X}_{1},{X}_{2},{X}_{3}}\right)$ 是来自 $X$ 的简单随机样本,求 (1) ${X}_{\left( 3\right) }$ 的分布密度函数. (2) $\operatorname{Var}\left\lbrack  {X}_{\left( 3\right) }\right\rbrack$.

6.10. 设总体 $X$ 的概率分布为 $P\left( {X = i}\right)  = \frac{1}{3}, i = 1,2,3.\left( {{X}_{1},{X}_{2},{X}_{3}}\right)$ 为来自 $X$ 的样本,求 (1) $E\left\lbrack  {X}_{\left( 1\right) }\right\rbrack$. (2) $\operatorname{Var}\left\lbrack  {X}_{\left( 3\right) }\right\rbrack$.

6.11. 设 ${\bar{X}}_{n},{S}_{n}^{2}$ 分别为样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的均值与方差,而 ${X}_{n + 1}$ 是第 $n + 1$ 次观测量, 试证:

(1) ${\bar{X}}_{n + 1} = \frac{n}{n + 1}{\bar{X}}_{n} + \frac{1}{n + 1}{X}_{n + 1}$.

(2) ${S}_{n + 1}^{2} = \frac{n}{n + 1}\left\lbrack  {{S}_{n}^{2} + \frac{1}{n + 1}{\left( {X}_{n + 1} - {\bar{X}}_{n}\right) }^{2}}\right\rbrack$.

6.12. 设总体 $X \sim  B\left( {m, p}\right)$,而 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是来自 $X$ 的样本,(1) 求 $E\left\lbrack  X\right\rbrack ,\operatorname{Var}\left\lbrack  X\right\rbrack$. (2) 求 $E\left\lbrack  {S}_{n}^{2}\right\rbrack$.

6.13. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 是来自 $0 - 1$ 分布 $B\left( {1, p}\right)$ 的简单随机样本, $X,{S}_{n}^{2}$ 分别为样本均值与样本方差.

(2) 求 $E\left\lbrack  {S}_{n}^{2}\right\rbrack$. (3) 证明: ${S}_{n}^{2} = \bar{X}\left( {1 - \bar{X}}\right)$.

6.14. 设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为来自 $X$ 的样本, $\bar{X},{S}_{n}^{2}$ 分别为样本均值与方差,求 (1) $E\left\lbrack  {\bar{X}}^{2}\right\rbrack$ 之值,(2) $E\left\lbrack  {{\bar{X}}^{2}{S}_{n}^{2}}\right\rbrack$ 之值.

6.15. 请查表或利用 $\mathrm{R}$ 软件给出下列分位数:

(1) ${u}_{0.05}.\;\left( 2\right) {t}_{0.975}\left( 8\right).\;\left( 3\right) {t}_{0.05}\left( 9\right).\;(4$ (4) ${\chi }_{0.975}^{2}\left( 5\right)$. (5) ${F}_{0.025}\left( {6,5}\right)$.

6.16. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{11}}\right)$ 为来自 $X \sim  N\left( {-1,4}\right)$ 的样本, $\bar{X} = \frac{1}{10}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}$. 求

(1) $P\left( {{X}_{10} - \bar{X} < {0.5}}\right)$ 之值. (2) $P\left( {{X}_{11} - \bar{X} < {0.5}}\right)$ 之值.

6.17. 设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{8}}\right)$ 为来自 $X$ 的样本, ${S}_{8}^{*2} = \frac{1}{7}\mathop{\sum }\limits_{{i = 1}}^{8}{\left( {X}_{i} - \bar{X}\right) }^{2}$, 求 $P\left( {\sqrt{8}\left( {\bar{X} - \mu }\right)  <  - {1.9}{S}_{8}^{ * }}\right)$ 之值.

6.18. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{9}}\right)$ 为来自 $N\left( {2,4}\right)$ 的样本, $\left( {{Y}_{1},{Y}_{2},\cdots,{Y}_{17}}\right)$ 为来自 $N\left( {3,9}\right)$ 的

样本,且两样本独立,令 $F = \frac{\mathop{\sum }\limits_{{i = 1}}^{9}{\left( {X}_{i} - 2\right) }^{2}}{\mathop{\sum }\limits_{{i = 1}}^{{17}}{\left( {Y}_{i} - \bar{Y}\right) }^{2}}$,求 $P\{ {0.0836} < F < {0.9450}\}$ 之值.

6.19. 设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{10}}\right)$ 为来自 $N\left( {-1,9}\right)$ 的样本,求

(1) $P\left( {\mathop{\sum }\limits_{{i = 1}}^{{10}}{\left( {X}_{i} + 1\right) }^{2} \geq  {112.941}}\right)$ 之值.

(2) $P\left( {\mathop{\sum }\limits_{{i = 1}}^{{10}}{\left( {X}_{i} - \bar{X}\right) }^{2} \geq  {53.091}}\right)$.