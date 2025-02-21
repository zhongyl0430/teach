---
title: 第五章 大数定律和中心极限定理
---
我们知道,对应于随机试验的一个结果 $\omega$,随机变量序列 ${X}_{1},{X}_{2},\cdots$,就得到一个数列 ${X}_{1}\left( \omega \right),{X}_{2}\left( \omega \right),\cdots$,不同的试验结果对应的数列有所不同,那么在算术平均意义下是否与某一个确定数列相差不大? 若答案是肯定的, 我们就可以近似地用该确定数列的算术平均值代替随机变量序列的算术平均值. 回答这个问题的有关定理和事实, 历史上称之为 “大数定律”, 这里的 “定律” 源自英文 law of large number.

另外, 将该随机变量序列经某种规范化, 会不会在某种意义下收敛到具某一分布已知的随机变量? 回答这个问题的有关定理和事实, 历史上称之为 “中心极限定理" (central limit theorem).

以上两个问题的回答, 是初等概率论中最深入和最精彩的结果, 为此要引入随机变量收敛性的各种定义以及诸如母函数、矩母函数和特征函数等分析工具. 但由于课程内容深度和学时的限制, 我们本章只做简单讨论.

## 5.1 大数定律

### 5.1.1 大数定律问题的提法

设有随机变量序列 ${X}_{1},{X}_{2},\cdots$,试问是否存在确定数列 ${a}_{1},{a}_{2},\cdots$,使得在某种收敛意义下, 有

$$
\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}{n} - \frac{{a}_{1} + {a}_{2} + \cdots  + {a}_{n}}{n} \rightarrow  0\;\left( {n \rightarrow  \infty }\right) ? \tag{5.1.1}
$$

若能在某种条件下,对任意 $\varepsilon  > 0$ 有

$$
\begin{array}{r} \mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\omega  : \left| {\frac{{X}_{1}\left( \omega \right)  + {X}_{2}\left( \omega \right)  + \cdots  + {X}_{n}\left( \omega \right) }{n} - \frac{{a}_{1} + {a}_{2} + \cdots  + {a}_{n}}{n}}\right|  \geq  \varepsilon }\right)  = 0, \\  ({5.1}. \end{array} \tag{5.1.2}
$$

则称 ${X}_{1},{X}_{2},\cdots$ 服从弱大数定律.

若能在某种条件下, 有

$$
P\left( {\omega  : \mathop{\lim }\limits_{{n \rightarrow  \infty }}\left( {\frac{{X}_{1}\left( \omega \right)  + {X}_{2}\left( \omega \right)  + \cdots  + {X}_{n}\left( \omega \right) }{n} - \frac{{a}_{1} + {a}_{2} + \cdots  + {a}_{n}}{n}}\right)  = 0}\right)  = 1, \tag{5.1.3}
$$

则称 ${X}_{1},{X}_{2},\cdots$ 服从强大数定律.

一般地,设有随机变量序列 ${X}_{1},{X}_{2},\cdots$ 和随机变量 $Y$.

(1)如果对任意 $\varepsilon  > 0$ 有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\omega  : \left| {{X}_{n}\left( \omega \right)  - Y\left( \omega \right) }\right|  \geq  \varepsilon }\right)  = 0,
$$

则称 ${X}_{1},{X}_{2},\cdots$ 依概率收敛于 $Y$,记作 ${X}_{n}\overset{P}{ \rightarrow  }Y$.

(2) 如果

$$
P\left( {\omega  : \mathop{\lim }\limits_{{n \rightarrow  \infty }}{X}_{n}\left( \omega \right)  = Y\left( \omega \right) }\right)  = 1,
$$

则称 ${X}_{1},{X}_{2},\cdots$ 以概率 1 收敛 于 $Y$,记作 ${X}_{n}\overset{\text{ a.s }}{ \rightarrow  }Y$.

可以证明,若 ${X}_{n}\overset{\text{ a.s }}{ \rightarrow  }Y$,则 ${X}_{n}\overset{P}{ \rightarrow  }Y$. 这就解释了前述大数定律的 “强” 和 “弱” 称谓的缘由.

### 5.1.2 弱大数定律

引理 5.1.1 (切比雪夫 (Чебышев) 不等式) 设随机变量 $X$ 的方差存在,则对任 $\varepsilon  > 0$ 有

$$
P\left( {\left| {X - E\left\lbrack  X\right\rbrack  }\right|  \geq  \varepsilon }\right)  \leq  \frac{\operatorname{Var}\left\lbrack  X\right\rbrack  }{{\varepsilon }^{2}}. \tag{5.1.4}
$$

证明 只就 $X$ 为连续型随机变量的情形证明.

$$
P\left( {\left| {X - E\left\lbrack  X\right\rbrack  }\right|  \geq  \varepsilon }\right)  = {\int }_{\left| {x - E\left\lbrack  X\right\rbrack  }\right|  \geq  \varepsilon }{f}_{X}\left( x\right) \mathrm{d}x
$$

$$
\leq  {\int }_{\left| {x - E\left\lbrack  X\right\rbrack  }\right|  \geq  \varepsilon }\frac{{\left( x - E\left\lbrack  X\right\rbrack  \right) }^{2}}{{\varepsilon }^{2}}{f}_{X}\left( x\right) \mathrm{d}x
$$

$$
\leq  {\int }_{-\infty }^{\infty }\frac{{\left( x - E\left\lbrack  X\right\rbrack  \right) }^{2}}{{\varepsilon }^{2}}{f}_{X}\left( x\right) \mathrm{d}x
$$

$$
= \frac{1}{{\varepsilon }^{2}}{\int }_{-\infty }^{\infty }{\left( x - E\left\lbrack  X\right\rbrack  \right) }^{2}{f}_{X}\left( x\right) \mathrm{d}x
$$

$$
= \frac{\operatorname{Var}\left\lbrack  X\right\rbrack  }{{\varepsilon }^{2}}.
$$

由引理 5.1.1 立即得到如下定理.

定理 5.1.1 (切比雪夫弱大数定律) 设 ${X}_{1},{X}_{2},\cdots$,为独立随机变量序列, $E\left\lbrack  {X}_{i}\right\rbrack   = \mu,\operatorname{Var}\left\lbrack  {X}_{i}\right\rbrack   \leq  C, i = 1,2,\cdots$,则对任意 $\varepsilon  > 0$ 有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\left| {\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}{n} - \mu }\right|  \geq  \varepsilon }\right)  = 0. \tag{5.1.5}
$$

证明 由于 ${X}_{1},{X}_{2},\cdots$,的独立性有

$$
E\left\lbrack  \frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}{n}\right\rbrack   = \mu,\operatorname{Var}\left\lbrack  \frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}{n}\right\rbrack   = \frac{\mathop{\sum }\limits_{{i = 1}}^{n}\operatorname{Var}\left\lbrack  {X}_{i}\right\rbrack  }{{n}^{2}} \leq  \frac{C}{n}.
$$

所以, 由 (5.1.4) 有

$$
P\left( {\left| {\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}{n} - \mu }\right|  \geq  \varepsilon }\right)  \leq  \frac{C}{n{\varepsilon }^{2}} \rightarrow  0\;\left( {n \rightarrow  \infty }\right).
$$

这说明 (5.1.5) 成立.

对于随机变量序列独立且同分布的情形,辛钦 $\left( {\mathrm{X}}_{\mathrm{{MH}}}\middle| \mathrm{\Psi }\middle| \mathrm{\Psi }\right)$ 给出了下面的定理.

定理 5.1.2 (辛钦弱大数定律) 设 ${X}_{1},{X}_{2},\cdots$,为独立同分布随机变量序列, 具有有限的数学期望 $\mu$,则对任意 $\varepsilon  > 0$ 有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\left| {\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}{n} - \mu }\right|  \geq  \varepsilon }\right)  = 0. \tag{5.1.6}
$$

下面的推论 5.1.1 说明了概率的统计定义的含义.

推论 5.1.1 (伯努利大数定律) 记 ${\nu }_{n}$ 为 $n$ 重独立伯努利试验中成功的次数, $p$ 为一次试验成功的概率,则

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\left| {\frac{{\nu }_{n}}{n} - p}\right|  \geq  \varepsilon }\right)  = 0. \tag{5.1.7}
$$

证明 设 ${X}_{1},{X}_{2},\cdots$ 为独立同分布的随机变量序列,同服从 $B\left( {1, p}\right)$,则

$E\left\lbrack  {X}_{1}\right\rbrack   = p$,且

$$
\frac{{\nu }_{n}}{n} = \frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}{n}
$$

从而由 (5.1.6) 即得 (5.1.7).

### 5.1.3 强大数定律

关于强大数定律,我们不加证明地给出如下的引理 5.1.2、定理 5.1.3 和定理 5.1.4.

引理 5.1.2 (柯尔莫哥洛夫不等式) 设 ${X}_{1},{X}_{2},\cdots$,为独立随机变量序列, 具有有限的数学期望和方差,则对任意 $\varepsilon  > 0$,有

$$
P\left( {\mathop{\sup }\limits_{{1 \leq  k \leq  n}}\left| {\mathop{\sum }\limits_{{i = 1}}^{k}\left( {{X}_{i} - E\left\lbrack  {X}_{i}\right\rbrack  }\right) }\right|  \geq  \varepsilon }\right)  \leq  \frac{\mathop{\sum }\limits_{{k = 1}}^{n}\operatorname{Var}\left\lbrack  {X}_{k}\right\rbrack  }{{\varepsilon }^{2}}.
$$

利用引理 5.1.2 可以证明如下定理.

定理 5.1.3 (柯尔莫哥洛夫强大数定律) 设 ${X}_{1},{X}_{2},\cdots$ 为独立随机变量序列,具有有限的数学期望,且 $\mathop{\sum }\limits_{{n = 1}}^{\infty }\frac{\operatorname{Var}\left\lbrack  {X}_{n}\right\rbrack  }{{n}^{2}} < \infty$,则

$$
P\left( {\mathop{\lim }\limits_{{n \rightarrow  \infty }}{n}^{-1}\mathop{\sum }\limits_{{k = 1}}^{n}\left( {{X}_{k} - E\left\lbrack  {X}_{k}\right\rbrack  }\right)  = 0}\right)  = 1.
$$

对于随机变量序列独立且同分布的情形, 柯尔莫哥洛夫给出了下面的定理.

定理 5.1.4 (柯尔莫哥洛夫强大数定律) 设 ${X}_{1},{X}_{2},\cdots$,为独立同分布随机变量序列,具有有限的数学期望 $\mu$,则

$$
P\left( {\mathop{\lim }\limits_{{n \rightarrow  \infty }}{n}^{-1}\mathop{\sum }\limits_{{k = 1}}^{n}\left( {{X}_{k} - E\left\lbrack  {X}_{k}\right\rbrack  }\right)  = 0}\right)  = 1.
$$

由定理 5.1.4 很容易得到如下的推论 5.1.2, 它的结论比推论 5.1.1 的结论更强, 也更进一步解释了概率的统计定义的含义.

推论 5.1.2 (博雷尔 (Borel) 强大数定律) 记 ${\nu }_{n}$ 为 $n$ 重独立伯努利试验中成功的次数, $p$ 为一次试验成功的概率,则

$$
P\left( {\mathop{\lim }\limits_{{n \rightarrow  \infty }}\frac{{\nu }_{n}}{n} = p}\right)  = 1. \tag{5.1.8}
$$

## 5.2 中心极限定理

若 定义 5.2.1 设 ${X}_{1},{X}_{2},\cdots$ 为随机变量序列,具有有限的数学期望和方差,

$$
\frac{\mathop{\sum }\limits_{{k = 1}}^{n}\left( {{X}_{k} - E\left\lbrack  {X}_{k}\right\rbrack  }\right) }{\sqrt{\operatorname{Var}\left\lbrack  {\mathop{\sum }\limits_{{k = 1}}^{n}{X}_{k}}\right\rbrack  }}\overset{d}{ \rightarrow  }N\left( {0,1}\right), \tag{5.2.1}
$$

则称 ${X}_{1},{X}_{2},\cdots$ 服从中心极限定理.

对于随机变量序列 ${X}_{1},{X}_{2},\cdots$,为独立同分布的情形,林德伯格 (Lindeberg) 和莱维 (Lévy) 得到下列中心极限定理.

定理 5.2.1 (林德伯格 - 莱维定理) 设 ${X}_{1},{X}_{2},\cdots$ 为独立同分布随机变量序列,具有有限的数学期望 $\mu$ 和方差 ${\sigma }^{2}$,则 ${X}_{1},{X}_{2},\cdots$,服从中心极限定理. 即

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\frac{1}{\sigma \sqrt{n}}\left\lbrack  {\mathop{\sum }\limits_{{k = 1}}^{n}{X}_{k} - {n\mu }}\right\rbrack   \leq  x}\right)  = \frac{1}{\sqrt{2\pi }}{\int }_{-\infty }^{x}{\mathrm{e}}^{-\frac{{u}^{2}}{2}}\mathrm{\;d}u. \tag{5.2.2}
$$

根据定理 5.2.1,当 $n$ 很大时,无论独立同分布的随机变量序列服从何种分布, 其部分和的分布都可以近似地用正态分布来代替.

例 5.2.1 已知设 ${X}_{1},{X}_{2},\cdots$ 为独立同分布随机变量序列,具有数学期望 $\mu  = 1$ 和方差 ${\sigma }^{2} = 4$. 试求 $P\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{100} \leq  {125}}\right)$.

解 由于 $n$ 较大,我们用定理 5.2.1 的结论作近似计算. 由题设,(5.2.2) 中的 ${n\mu } = {100},\sigma \sqrt{n} = {20}$,所以由定理 5.2.1 有

$$
P\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{100} \leq  {125}}\right)
$$

$$
= P\left( {\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{100} - {100}}{20} \leq  \frac{{125} - {100}}{20}}\right)
$$

$$
\approx  \Phi \left( {1.25}\right)  = {0.8943502}.
$$

对于独立随机变量序列 ${X}_{1},{X}_{2},\cdots$,同服从 $B\left( {1, p}\right)$ 的情形,棣莫弗 (De Moivre) 和拉普拉斯 (Laplace) 得到了下列中心极限定理.

定理 5.2.2 (棣莫弗-拉普拉斯定理) 设 ${X}_{1},{X}_{2},\cdots$ 为独立同分布随机变量序列,同服从 $B\left( {1, p}\right)$,则 ${X}_{1},{X}_{2},\cdots$,服从中心极限定理,即

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left( {\frac{1}{\sqrt{{np}\left( {1 - p}\right) }}\left\lbrack  {\mathop{\sum }\limits_{{k = 1}}^{n}{X}_{k} - {np}}\right\rbrack   \leq  x}\right)  = \frac{1}{\sqrt{2\pi }}{\int }_{-\infty }^{x}{\mathrm{e}}^{-\frac{{u}^{2}}{2}}\mathrm{\;d}u. \tag{5.2.3}
$$

因为对于 $X \sim  B\left( {1, p}\right)$,有 $E\left\lbrack  X\right\rbrack   = p$ 和 $\operatorname{Var}\left\lbrack  X\right\rbrack   = p\left( {1 - p}\right)$. 显然,定理 5.2.2 是定理 5.2.1 的推论. 但定理 5.2.1 是历史上最早的中心极限定理, 它由棣莫弗 1716 年,对 $p = \frac{1}{2}$ 首次给出了 (5.2.3) 的证明,后来由拉普拉斯推广到一般 $p$ 的情形.

大家知道,二项分布的随机变量是 $n$ 个独立的同服从 $B\left( {1, p}\right)$ 的随机变量的和 (参见例 4.2.3), 所以可由定理 5.2.2 对二项分布作近似计算.

例 5.2.2 设某地区内原有一家小型电影院, 因业务需要, 拟筹建一家较大型电影院. 根据分析,该地区每天看电影者约有 $n = {1600}$ 人,且预计新电影院建成开业后,约有 $\frac{3}{4}$ 的观众会去新影院. 现该影院在计划其座位数,要求座位数尽可能多, 但 “空座多于 200” 的概率又不能超过 0.1, 问该设多少座位?

解 将 1600 位可能去看电影的人编号 $1,2,\cdots,{1600}$,记

$$
{X}_{i} = \left\{  {\begin{array}{ll} 1, & \text{ 若第 }i\text{ 位观众去新影院; } \\  0, & \text{ 其他. } \end{array}\;i = 1,2,\cdots,{1600}.}\right.
$$

由题设, ${X}_{i} \sim  B\left( {1,\frac{3}{4}}\right)$,且假定各位观众是否去新影院相互独立,所以 ${X}_{1},{X}_{2},\cdots,{X}_{1600}$ 相互独立,且 (参见例 4.2.3)

$$
{X}_{1} + {X}_{2} + \cdots  + {X}_{1600} \sim  B\left( {{1600},{0.75}}\right),
$$

现设座位数为 $m$,依题意应有

$$
P\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{1600} \leq  m - {200}}\right)  \leq  {0.1}.
$$

由于要求 $m$ 尽可能大,又要使上式成立,所以应取 $m$ 使得

$$
P\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{1600} \leq  m - {200}}\right)  = {0.1}.
$$

由于 $n$ 较大,我们用定理 5.2.2 的结论作近似计算.

依定理 5.2.2 作近似计算,则 (5.2.3) 中的 ${np} = {1600} \times  \frac{3}{4} = {1200},\sqrt{{np}\left( {1 - p}\right) } =$ ${10}\sqrt{}3$. 所以由定理 5.2.2 有

$$
P\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{1600} \leq  m - {200}}\right)
$$

$$
= P\left( {\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{1600} - {1200}}{{10}\sqrt{3}} \leq  \frac{m - {200} - {1200}}{{10}\sqrt{3}}}\right)
$$

$$
\approx  \Phi \left( \frac{m - {200} - {1200}}{{10}\sqrt{3}}\right).
$$

令 $\Phi \left( x\right)  = {0.1}$,用 $\mathrm{R}$ 软件的 qnorm 函数得 qnorm $\left( {0.1}\right)  =  - {1.281552}$.

于是应有

$$
\frac{m - {200} - {1200}}{{10}\sqrt{3}} =  - {1.281552},
$$

即

$$
m = {1377.803}.
$$

因此该电影院设 1378 个座位为好.

## 第五章小结与注记

(1)最早的大数定律是伯努利大数定律 (参见推论 5.1.1, 发表于 1713 年). 它从理论上阐明了事件 $A$ 发生的 “频率稳定于概率” 的含义. 而后的博雷尔强大数定律 (参见推论 5.1.2, 发表于 1909 年), 更清晰地解释了概率的统计定义的含义. 推而广之, 大数定律回答何时一个随机序列的算术平均值会在某种意义下收敛寸某一确定实数列的算术平均值. 由于随机变量序列以概率 1 收敛必然依概率收敛, 所以若依概率收敛 (参见 (5.1.2)), 则称为弱大数定律成立. 若以概率 1 收敛 (参见 (5.1.3)), 则称为强大数定律成立.

对于大数定律问题的回答, 一般都只能给出使大数定律成立的充分条件, 很难给出必要条件. 另外, 弱大数定律在建立了较为弱的不等式 (参见引理 5.1.1) 之后, 就可以得到相应的大数定律. 但对强大数定律, 要有更强的不等式估计 (参见引理 5.1.2) 和较为复杂的证明才能得到.

需要强调指出的是, 大数定律的结论是某事实成立的概率 (或其极限) 为 0 或 1. 在实际问题和理论分析时, 我们都认为概率为 0 的事件, 每次试验都近乎不会发生; 而概率为 1 的事件, 每次试验近乎必然发生. 即大数定律回答的问题是何时随机事件在试验次数很大时近乎必然发生或不发生, 这在理论和实际应用上都是十分有意义的.

(2)中心极限定理回答的问题,首先是想把诸如伯努利大数定律所对应的伯努利试验的随机变量序列 (即 0,1 随机序列) 的部分和的情形, 推广到一般的随机变量序列部分和的情形. 为了避免出现部分和序列趋于无穷的情形, 自然地, 减去部分和的均值后再除它的标准差, 得到标准化形式. 正如一个正态随机变量减去其期望再除标准差后, 为标准正态的随机变量, 所以中心极限定理回答的问题是, 随机变量序列的部分和标准化后何时以概率 1 收敛到我们熟悉的标准正态随机变量.

本章中仅给出使中心极限定理成立的充分条件, 并且其证明需要引进诸如特征函数等数学工具, 故也略去了. 但需指出, 经过前人不懈的努力, 找到了中心极限定理成立的充要条件, 该条件大致可以叙述为: 若独立随机变量序列有有限的方差, 各分量都很小且 “均匀的小”.

中心极限定理的事实解释了为何正态分布的随机变量是极为常见的, 因为无论满足条件的随机变量序列的每个分量服从何种分布, 它们的部分和的标准化将收敛于标准正态分布.

历史上, 大数定律和中心极限定理还用来做二项分布概率的近似计算 (参见例 5.2.2), 这一点有了方便的计算机软件可用, 意义就不是很大了.

(3) 无论大数定律还是中心极限定理, 其中有一个关键的条件, 那就是随机变量序列的独立性. 从这点讲, 大数定律和中心极限定理都属初等的概率论的范畴.

## 第五章习题

5.1. 假设 $X$ 和 $Y$ 为随机变量,且满足 $E\left\lbrack  X\right\rbrack   =  - 2, E\left\lbrack  Y\right\rbrack   = 2,\operatorname{Var}\left\lbrack  X\right\rbrack   = 1,\operatorname{Var}\left\lbrack  Y\right\rbrack   = 9$, $X$ 与 $Y$ 的相关系数 $r\left( {X, Y}\right)  =  - {0.5}$. 试由切比雪夫不等式确定满足不等式: $P(\left| {X + Y}\right|  \geq$ $6) \leq  c$ 的最小正数 $c$ 之值.

5.2. 设 ${X}_{1},{X}_{2}$ 为随机变量且 $E\left\lbrack  {X}_{i}\right\rbrack   = 0,\operatorname{Var}\left\lbrack  {X}_{i}\right\rbrack   = 1\left( {i = 1,2}\right)$. 证明: 对任意的 $\lambda  > 0$ 有 $P\left( {{X}_{1}^{2} + {X}_{2}^{2} \geq  {2\lambda }}\right)  \leq  \frac{1}{\lambda }$.

5.3. 在一枚均匀正四面体的四个面上分别画上1,2,3,4个点. 现将该四面体重复投掷. 极限. ${X}_{i}\left( {i = 1,2,\cdots }\right)$ 为第 $i$ 次投掷向下一面的点数,试求当 $n \rightarrow  \infty$ 时, $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 依概率收敛的

5.4. 设 $\left\{  {X}_{n}\right\}$ 是独立的随机变量序列,且假设

$$
P\left( {{X}_{n} = \sqrt{\ln n}}\right)  = P\left( {{X}_{n} =  - \sqrt{\ln n}}\right)  = {0.5},\;n = 1,2,\cdots.
$$

问 $\left\{  {X}_{n}\right\}$ 是否服从大数定律.

5.5. 设 $\left\{  {X}_{n}\right\}$ 是独立同分布的随机变量序列,且假设 $E\left\lbrack  {X}_{n}\right\rbrack   = 2,\operatorname{Var}\left\lbrack  {X}_{n}\right\rbrack   = 6$. 证明. 值. $\frac{{X}_{1} + {X}_{2}{X}_{3} + {X}_{4}^{2} + {X}_{5}{X}_{6} + \cdots  + {X}_{{3n} - 2}^{2} + {X}_{{3n} - 1}{X}_{3n}}{n}\xrightarrow[]{P}a, n \rightarrow  \infty$,并确定常数 $a$ 之

5.6. 设随机变量 $X \sim  B\left( {{100},{0.8}}\right)$,试用棣莫弗-拉普拉斯定理求 $P\left( {{80} \leq  X < {100}}\right)$ 的近似值.

5.7. 一仪器同时收到 50 个信号 ${X}_{k}, k = 1,2,\cdots,{50}$. 设 ${X}_{1},\cdots,{X}_{50}$ 相互独立,且都服从区间 $\left\lbrack  {0,9}\right\rbrack$ 上的均匀分布,试求 $P\left( {\mathop{\sum }\limits_{{k = 1}}^{{50}}{X}_{k} > {250}}\right)$ 的近似值.

5.8. 一个复杂的系统由 $n$ 个相互独立起作用的部件所组成,每个部件损坏的概率为 0.10. 为了使整个系统正常运行,至少需要 ${80}\%$ 或 ${80}\%$ 以上的部件正常工作,问 $n$ 至少为多大才能使整个系统正常工作的概率不小于 95%.

5.9. 某大卖场某种商品价格波动为随机变量,设第 $k$ 天 (较前一天) 的价格变化为 ${X}_{k}, k = 1,2,\cdots, n.\;{X}_{1},\cdots,{X}_{n}$ 独立同分布,都服从 $\left\lbrack  {-{0.15},{0.15}}\right\rbrack$ 上的均匀分布,令 ${Y}_{n} = {Y}_{0} + \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 表示第 $n$ 天的价格,而现在价格 ${Y}_{0} = {50}$,用中心极限定理估计概率 $P\left( {{48} \leq  {Y}_{60} \leq  {52}}\right)$ 之值.

5.10. 设某汽车销售点每天出售的汽车数量服从参数为 $\lambda  = 2$ 的泊松分布,若 200 天都经营汽车销售, 且每天出售的汽车数是相互独立的, 求 200 天售出 380 辆以上汽车的概率.

5.11. 假设某洗衣店为第 $i$ 个顾客服务的时间 ${X}_{i}$ 服从区间 $\left\lbrack  {5,{53}}\right\rbrack$ (单位: 分钟) 上的均匀以概率 1 收敛于何值? 分布,且对每个顾客是相互独立的,试问当 $n \rightarrow  \infty$ 时, $n$ 次服务时间的算术平均值 $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$