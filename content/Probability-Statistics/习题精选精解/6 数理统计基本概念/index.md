### 知识要点

1. 总体 是指研究对象的某个性能指标的全体,通常用一随机变量 $X$ 代表总体.

2. 个体 是指每一个研究对象.

3. 样本 从总体中取 $n$ 个个体,称作来自总体的容量为 $n$ 的样本.

简单随机样本 是指 $n$ 个相互独立,而且与总体 $X$ 同分布的随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n}$,简称随机样本,也常以随机向量 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 表示. 它们的一组观察值 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 称为样本值.

1. 统计量 称不含未知参数的样本函数 $g\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为统计量.

常见统计量 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 为样本均值,

${S}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}$ 为样本方差,

$S = \sqrt{{S}^{2}}$ 称为样本标准差,

${A}_{k} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{k}$ 为 $k$ 阶样本原点矩,

${B}_{k} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{k}$ 为 $k$ 阶样本中心矩,

其中 ${B}_{2} = {S}_{n}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} = \frac{n - 1}{n}{S}^{2}$.

#### 5. 经验分布函数

从总体 $X$ 中抽取一个容量为 $n$ 的样本,将其观察值 $\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)$ 按大小顺序,重新排列如下

$$
{x}_{1}^{ * } \leq  {x}_{2}^{ * } \leq  \cdots  \leq  {x}_{n}^{ * },
$$

对于任意的实数 $x$,定义函数

$$
{F}_{n}\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < {x}_{1}^{ * } \\  \frac{k}{n}, & {x}_{k}^{ * } \leq  x < {x}_{k + 1}^{ * },\;k = 1,2,\cdots, n - 1 \\  1, & {x}_{n}^{ * } \leq  x \end{array}\right.
$$

称 ${F}_{n}\left( x\right)$ 为总体 $X$ 由 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 所决定的样本分布函数或经验分布函数.

格列汶科定理 当 $n \rightarrow  \infty$ 时, ${F}_{n}\left( x\right)$ 依概率 1 关于 $x$ 均匀地收敛于 $F\left( x\right)$. 即说明: 当 $n$ 很大时,样本分布函数 ${F}_{n}\left( x\right)$ 近似于总体分布函数 $F\left( x\right)$.

6. ${\chi }^{2}$ 分布

(1)定义: 设随机变量 ${X}_{1},\cdots,{X}_{n}$ 相互独立同分布 $N\left( {0,1}\right)$,若有 ${\chi }^{2} = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$,则随机变量 ${\chi }^{2}$ 概率论与数理统计习题精选精解的分布称为 $n$ 个自由度的 ${\chi }^{2}$ 分布. 即 ${\chi }^{2} \sim  {\chi }^{2}\left( n\right)$. 其概率密度函数为

$$
\varphi \left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{{2}^{\frac{n}{2}}\Gamma \left( \frac{n}{2}\right) }{x}^{\frac{n}{2} - 1}{\mathrm{e}}^{-\frac{x}{2}}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

用图形表示其密度函数为图 6-1.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_205_535_405_603_299_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_205_535_405_603_299_0.jpg)

图 6-1

(2) 性质: ① $E\left( {{\chi }^{2}\left( n\right) }\right)  = n, D\left( {{\chi }^{2}\left( n\right) }\right)  = {2n}$.

② 设 $X \sim  {\chi }^{2}\left( m\right), Y \sim  {\chi }^{2}\left( n\right)$,且 $X$ 与 $Y$ 相互独立. 则

$$
X + Y \sim  {\chi }^{2}\left( {m + n}\right).
$$

(3)上 $\alpha$ 分位点:对于给定的正数 $\alpha \left( {0 < \alpha  < 1}\right)$,称满足条件

$$
P\left\{  {{\chi }^{2} > {\chi }_{\alpha }^{2}\left( n\right) }\right\}   = \alpha
$$

的点 ${\chi }_{\alpha }^{2}\left( n\right)$ 为 ${\chi }^{2}$ 分布的上 $\alpha$ 分位点.

7. $t$ 分布

(1)定义: 设随机变量 $X$ 与 $Y$ 相互独立. $X \sim  N\left( {0,1}\right), Y \sim  {\chi }^{2}\left( n\right)$,若 $T = \frac{X}{\sqrt{\frac{Y}{n}}}$,则随机变量 $T$ 的分布称为 $n$ 个自由度的 $t$ 分布,即 $T \sim  t\left( n\right)$,其概率密度函数为

$$
\varphi \left( x\right)  = \frac{\Gamma \left( \frac{n + 1}{2}\right) }{\sqrt{n\pi }\Gamma \left( \frac{n}{2}\right) }{\left( 1 + \frac{{x}^{2}}{n}\right) }^{-\frac{n + 1}{2}}\;\left( {-\infty  < x <  + \infty }\right).
$$

用图形表示其概率密度为图 6-2.

(2) 性质: ① $E\left( {t\left( n\right) }\right)  = 0, D\left( {t\left( n\right) }\right)  = \frac{n}{n - 2}\;\left( {n > 2}\right)$;

② $\mathop{\lim }\limits_{{n \rightarrow  \infty }}\varphi \left( x\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}$,故 $n$ 足够大时, $t$ 分布近似于 $N\left( {0,1}\right)$;

③ 若 $T \sim  t\left( n\right)$,则 ${T}^{2} \sim  F\left( {1, n}\right)$;

(3)上 $\alpha$ 分位点: $t\left( n\right)$ 分布的上 $\alpha$ 分位点 ${t}_{\alpha }\left( n\right)$ 是指满足

$$
P\left\{  {T > {t}_{\alpha }\left( n\right) }\right\}   = \alpha \;\left( {0 < \alpha  < 1}\right) \;\text{ 的点 }{t}_{\alpha }\left( n\right).
$$

其中 ${t}_{1 - \alpha }\left( n\right)  =  - {t}_{\alpha }\left( n\right)$.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_206_556_180_466_437_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_206_556_180_466_437_0.jpg)

图 6-2

8. $F$ 分布

(1)定义: 设随机变量 $X$ 与 $Y$ 相互独立,且分别服从 ${\chi }^{2}\left( m\right)$ 和 ${\chi }^{2}\left( n\right)$ 分布,若 $F = \frac{\frac{X}{m}}{\frac{Y}{n}}$,则 $F$ 服从自由度为 $m, n$ 的 $F$ 分布. 即 $F \sim  F\left( {m, n}\right)$,其概率密度函数为

$$
\varphi \left( x\right)  = \left\{  \begin{array}{ll} \frac{\Gamma \left( \frac{m + n}{2}\right) }{\Gamma \left( \frac{m}{2}\right) \Gamma \left( \frac{n}{2}\right) }{m}^{\frac{m}{2}}{n}^{\frac{n}{2}}\frac{{x}^{\frac{m}{2} - 1}}{{\left( mx + n\right) }^{\frac{m + n}{2}}}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

用图形表示其概率密度函数为图 6-3.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_206_599_1084_364_295_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_206_599_1084_364_295_0.jpg)

图 6-3

(2)性质:① 若 $X \sim  F\left( {m, n}\right)$,则

$$
E\left( X\right)  = \frac{n}{n - 2}\;\left( {n > 2}\right),
$$

$$
D\left( X\right)  = \frac{{n}^{2}\left( {{2m} + {2n} - 4}\right) }{m{\left( n - 2\right) }^{2}\left( {n - 4}\right) }\;\left( {n > 4}\right);
$$

② 若 $X \sim  F\left( {m, n}\right)$,则 $\frac{1}{X} \sim  F\left( {n, m}\right)$;

(3)上 α 分位点:满足 $P\left\{  {F > {F}_{\alpha }\left( {m, n}\right) }\right\}   = \alpha \;\left( {0 < \alpha  < 1}\right)$ 的点 ${F}_{\alpha }\left( {m, n}\right)$ 称为上 $\alpha$ 分位点, 且 ${F}_{1 - \alpha }\left( {m, n}\right)  = \frac{1}{{F}_{\alpha }\left( {n, m}\right) }$.

#### 9. 正态总体的常用结论

(1)若总体 $X$ 服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right),{X}_{1},\cdots,{X}_{n}$ 是其样本, $\bar{X}$ 和 ${S}^{2}$ 分别为样本均值和方差, 则

① $\bar{X} \sim  N\left( {\mu,\frac{{\sigma }^{2}}{n}}\right)$ 或 $\frac{\bar{X} - \mu }{\sigma }\sqrt{n} \sim  N\left( {0,1}\right)$;

② $\frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)$;

③ $\frac{\bar{X} - \mu }{S}\sqrt{n} \sim  t\left( {n - 1}\right)$;

④ $\bar{X}$ 与 ${S}^{2}$ 相互独立.

( 2 )若 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 和 ${Y}_{1},{Y}_{2},\cdots,{Y}_{m}$ 分别表示取自两个正态总体 $N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right)$ 和 $N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$ 的简单随机样本, $\bar{X},\bar{Y}$ 和 ${S}_{1}^{2},{S}_{2}^{2}$ 分别表示其样本均值和方差,则有

① $\frac{\frac{{S}_{1}^{2}}{{\sigma }_{1}^{2}}}{\frac{{S}_{2}^{2}}{{\sigma }_{2}^{2}}} \sim  F\left( {n - 1, m - 1}\right)$;

② $\sqrt{\frac{{mn}\left( {n + m - 2}\right) }{n + m}}\frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{\sqrt{\left( {n - 1}\right) {S}_{1}^{2} + \left( {m - 1}\right) {S}_{2}^{2}}} \sim  t\left( {n + m - 2}\right)$. (当 ${\sigma }_{1}^{2} = {\sigma }_{2}^{2}$ 时)

### 基本题型

#### 题型 1. 判断抽样分布

方法与技巧 判断统计量服从什么抽样分布是本章的重点题型之一. 要做到判断准确, 必须首先将 ${\chi }^{2}$ 分布, $t$ 分布, $F$ 分布的定义及性质熟记,其次正态总体下的抽样分布结论要掌握.

【1.1】设随机变量 $X$ 和 $Y$ 都服从标准正态分布,则(   ).

(A) $X + Y$ 服从正态分布 (B) ${X}^{2} + {Y}^{2}$ 服从 ${\chi }^{2}$ 分布

(C) ${X}^{2}$ 和 ${Y}^{2}$ 都服从 ${\chi }^{2}$ 分布 (D) $\frac{{X}^{2}}{{Y}^{2}}$ 服从 $F$ 分布

分析 利用正态分布的性质和 ${\chi }^{2}$ 分布的表达式判断.

解 因为 $X$ 与 $Y$ 是否相互独立不确定,故 $X + Y$ 不一定服从正态分布,同理 ${X}^{2} + {Y}^{2}$ 不一定服从 ${\chi }^{2}$ 分布, $\frac{{X}^{2}}{{Y}^{2}}$ 服从 $F$ 分布也不确定. 而 ${X}^{2} \sim  {\chi }^{2}\left( 1\right),{Y}^{2} \sim  {\chi }^{2}\left( 1\right)$.

故答案为(C).

【1.2】设总体 $X$ 服从正态分布 $N\left( {0,{2}^{2}}\right)$,而 ${X}_{1},{X}_{2},\cdots,{X}_{15}$ 是来自总体 $X$ 的简单随机样本, 则随机变量

$$
Y = \frac{{X}_{1}^{2} + \cdots  + {X}_{10}^{2}}{2\left( {{X}_{11}^{2} + \cdots  + {X}_{15}^{2}}\right) }
$$

服从_____分布,参数为_____.

分析 利用 ${\chi }^{2}$ 分布与 $F$ 分布的定义可判断分布并解得参数.

解 由于 ${X}_{1},{X}_{2},\cdots,{X}_{15}$ 是简单随机样本,所以 ${X}_{i}\left( {i = 1,2,\cdots,{15}}\right)$ 相互独立且服从 $N(0$, $\left. {2}^{2}\right)$ 分布,因此 ${X}_{1}^{2} + \cdots  + {X}_{10}^{2}$ 与 ${X}_{11}^{2} + \cdots  + {X}_{15}^{2}$ 也相互独立,而

$$
\frac{{X}_{i}}{2} \sim  N\left( {0,1}\right) \;\left( {i = 1,2,\cdots,{15}}\right),
$$

故

$$
{\left( \frac{{X}_{1}}{2}\right) }^{2} + \cdots  + {\left( \frac{{X}_{10}}{2}\right) }^{2} = \frac{1}{4}\left( {{X}_{1}^{2} + \cdots  + {X}_{10}^{2}}\right)  \sim  {\chi }^{2}\left( {10}\right),
$$

$$
{\left( \frac{{X}_{11}}{2}\right) }^{2} + \cdots  + {\left( \frac{{X}_{15}}{2}\right) }^{2} = \frac{1}{4}\left( {{X}_{11}^{2} + \cdots  + {X}_{15}^{2}}\right)  \sim  {\chi }^{2}\left( 5\right),
$$

所以有

$$
\frac{\frac{1}{4}\left( {{X}_{1}^{2} + \cdots  + {X}_{10}^{2}}\right) \frac{1}{10}}{\frac{1}{4}\left( {{X}_{11}^{2} + \cdots  + {X}_{15}^{2}}\right) \frac{1}{5}} = \frac{{X}_{1}^{2} + \cdots  + {X}_{10}^{2}}{2\left( {{X}_{11}^{2} + \cdots  + {X}_{15}^{2}}\right) } \sim  F\left( {{10},5}\right),
$$

故 $Y$ 服从 $F$ 分布,参数为 $\left( {{10},5}\right)$.

【1.3】设 ${X}_{1},{X}_{2},\cdots,{X}_{9}$ 是总体 $X$ 的一个简单随机样本, $X$ 服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right),{Y}_{1} =$ $\frac{1}{6}\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{6}}\right),{Y}_{2} = \frac{1}{3}\left( {{X}_{7} + {X}_{8} + {X}_{9}}\right),{S}^{2} = \frac{1}{2}\mathop{\sum }\limits_{{i = 7}}^{9}{\left( {X}_{i} - {Y}_{2}\right) }^{2}, T = \frac{\sqrt{2}\left( {{Y}_{1} - {Y}_{2}}\right) }{S}$.

证明 $T \sim  t\left( 2\right)$.

证 因为 $X \sim  N\left( {\mu,{\sigma }^{2}}\right),{X}_{i} \sim  N\left( {\mu,{\sigma }^{2}}\right)$,所以 ${Y}_{1} \sim  N\left( {\mu,\frac{{\sigma }^{2}}{6}}\right),{Y}_{2} \sim  N\left( {\mu,\frac{{\sigma }^{2}}{3}}\right)$,

故 ${Y}_{1} - {Y}_{2} \sim  N\left( {0,\frac{{\sigma }^{2}}{2}}\right)$,因此有

$$
\frac{{Y}_{1} - {Y}_{2}}{\frac{\sigma }{\sqrt{2}}} = \frac{\sqrt{2}\left( {{Y}_{1} - {Y}_{2}}\right) }{\sigma } \sim  N\left( {0,1}\right).
$$

又由于

$$
{S}^{2} = \frac{1}{2}\mathop{\sum }\limits_{{i = 7}}^{9}{\left( {X}_{i} - {Y}_{2}\right) }^{2} = \frac{1}{3 - 1}\mathop{\sum }\limits_{{i = 7}}^{9}{\left( {X}_{i} - {Y}_{2}\right) }^{2},
$$

而

$$
\frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right),
$$

所以 $\frac{2{S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( 2\right)$.

因为 ${Y}_{2}$ 和 ${S}^{2}$ 相互独立,而且 ${Y}_{1}$ 与 ${Y}_{2},{Y}_{1}$ 与 ${S}^{2}$ 也相互独立,所以 ${Y}_{1} - {Y}_{2}$ 与 ${S}^{2}$ 相互独立. 则有 $\frac{\sqrt{2}\left( {{Y}_{1} - {Y}_{2}}\right) }{\sigma }$ 与 $\frac{2{S}^{2}}{{\sigma }^{2}}$ 相互独立.

那么

$$
T = \frac{\sqrt{2}\left( {{Y}_{1} - {Y}_{2}}\right) }{S} = \frac{\frac{\sqrt{2}\left( {{Y}_{1} - {Y}_{2}}\right) }{\sigma }}{\sqrt{\frac{2{S}^{2}}{2{\sigma }^{2}}}} \sim  t\left( 2\right),
$$

故 $T$ 服从自由度为 2 的 $t$ 分布.

【1.4】设 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$ 为来自总体 $X \sim  N\left( {1,{\sigma }^{2}}\right)$ 的简单随机样本,则统计量 $\frac{{X}_{1} - {X}_{2}}{\left| {X}_{3} + {X}_{4} - 2\right| }$ 的分布为_____.

(A) $N\left( {0,1}\right)$ (B) $t\left( 1\right)$ (C) ${\chi }^{2}\left( 1\right)$ (D) $F\left( {1,1}\right)$

解 $\frac{{X}_{1} - {X}_{2}}{\left| {X}_{3} + {X}_{4} - 2\right| } = \frac{\frac{{X}_{1} - {X}_{2}}{\sqrt{2}\sigma }}{\sqrt{{\left( \frac{{X}_{3} + {X}_{4} - 2}{\sqrt{2}\sigma }\right) }^{2}}}$,

因为 $\frac{{X}_{1} - {X}_{2}}{\sqrt{2}\sigma } \sim  N\left( {0,1}\right),\frac{{X}_{3} + {X}_{4} - 2}{\sqrt{2}\sigma } \sim  N\left( {0,1}\right),{\left( \frac{{X}_{3} + {X}_{4} - 2}{\sqrt{2}\sigma }\right) }^{2} \sim  {\chi }^{2}\left( 1\right)$,

所以 $\frac{{X}_{1} - {X}_{2}}{\left| {X}_{3} + {X}_{4} - 2\right| } = \frac{\frac{{X}_{1} - {X}_{2}}{\sqrt{2}\sigma }}{\sqrt{{\left( \frac{{X}_{3} + {X}_{4} - 2}{\sqrt{2}\sigma }\right) }^{2}}} \sim  t\left( 1\right)$.

故应选 (B).

【1.5】设随机变量 $X \sim  t\left( n\right) \left( {n > 1}\right), Y = \frac{1}{{X}^{2}}$,则 (   ).

(A) $Y \sim  {\chi }^{2}\left( n\right)$ (B) $Y \sim  {\chi }^{2}\left( {n - 1}\right)$

(C) $Y \sim  F\left( {n,1}\right)$ (D) $Y \sim  F\left( {1, n}\right)$

解法一 利用 $t$ 分布和 $F$ 分布的性质求解.

因为 $X \sim  t\left( n\right)$,由 $t$ 分布性质可得 ${X}^{2} \sim  F\left( {1, n}\right)$.

又根据 $F$ 分布的性质

$$
\frac{1}{{X}^{2}} \sim  F\left( {n,1}\right),
$$

故 $Y = \frac{1}{{X}^{2}} \sim  F\left( {n,1}\right)$ 分布,答案为 (C).

解法二 利用 $t$ 分布和 $F$ 分布的定义求解.

因 $X \sim  t\left( n\right)$,所以 $X$ 具有如下结构:

$$
X = \frac{U}{\sqrt{\frac{V}{n}}},
$$

其中 $U \sim  N\left( {0,1}\right), V \sim  {\chi }^{2}\left( n\right)$,且 $U$ 与 $V$ 相互独立. 从而

$$
{X}^{2} = \frac{{U}^{2}}{\frac{V}{n}}\text{ 即 }\frac{1}{{X}^{2}} = \frac{\frac{V}{n}}{{U}^{2}}.
$$

${U}^{2} \sim  {\chi }^{2}\left( 1\right)$,且 ${U}^{2}$ 与 $V$ 也相互独立,由定义

$$
\frac{1}{{X}^{2}} = \frac{\frac{V}{n}}{\frac{{U}^{2}}{1}} \sim  F\left( {n,1}\right).
$$

【1.6】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 的一个样本,样本均值和方差分别为 $\bar{X}$ 和 ${S}^{2},{X}_{n + 1}$ 为对 $X$ 的又一独立观测值,求统计量 $Y = \frac{{X}_{n + 1} - \bar{X}}{S}\sqrt{\frac{n}{n + 1}}$ 的分布.

解 因为 $\bar{X} \sim  N\left( {\mu,\frac{{\sigma }^{2}}{n}}\right),{X}_{n + 1} \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 且两者独立.

所以

$$
{X}_{n + 1} - \bar{X} \sim  N\left( {0,\frac{n + 1}{n}{\sigma }^{2}}\right),
$$

$$
U = \frac{{X}_{n + 1} - \bar{X}}{\sqrt{\frac{n + 1}{n}}\sigma } \sim  N\left( {0,1}\right),
$$

而 ${\chi }^{2} = \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)$ 且与 $U$ 独立,则由 $t$ 分布定义可知,

$$
\frac{U}{\sqrt{\frac{{\chi }^{2}}{n - 1}}} = \sqrt{\frac{n}{n + 1}} \cdot  \frac{{X}_{n + 1} - \bar{X}}{S} \sim  t\left( {n - 1}\right).
$$

#### 题型 2. 利用抽样分布确定参数

【1.7】设 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$ 是来自正态总体 $N\left( {0,{2}^{2}}\right)$ 的简单随机样本,

$$
X = a{\left( {X}_{1} - 2{X}_{2}\right) }^{2} + b{\left( 3{X}_{3} - 4{X}_{4}\right) }^{2},
$$

则当 $a =$ _____, $b =$ _____时,统计量 $X$ 服从 ${\chi }^{2}$ 分布,其自由度为_____.

解 令 ${Y}_{1} = {X}_{1} - 2{X}_{2}$,则 $\frac{{Y}_{1}}{\sqrt{20}} \sim  N\left( {0,1}\right)$,

所以 $a = \frac{1}{20}$ 时, $\sqrt{a}\left( {{X}_{1} - 2{X}_{2}}\right)  \sim  N\left( {0,1}\right)$.

同样令 ${Y}_{2} = 3{X}_{3} - 4{X}_{4}$,则 $\frac{{Y}_{2}}{10} \sim  N\left( {0,1}\right)$,

所以 $b = \frac{1}{100}$ 时, $\sqrt{b}\left( {3{X}_{3} - 4{X}_{4}}\right)  \sim  N\left( {0,1}\right)$,此时 $X = \frac{{Y}_{1}^{2}}{20} + \frac{{Y}_{2}^{2}}{100} \sim  {\chi }^{2}\left( 2\right)$.

故应填 $\frac{1}{20},\frac{1}{100},2$.

【1.8】设 ${X}_{1},{X}_{2},\cdots,{X}_{5}$ 是取自正态分布 $N\left( {0,{\sigma }^{2}}\right)$ 的一个简单随机样本,若 $\frac{a\left( {{X}_{1} + {X}_{2}}\right) }{\sqrt{{X}_{3}^{2} + {X}_{4}^{2} + {X}_{5}^{2}}}$ 服从 $t$ 分布,则 $a =$ _____.

解 因为

$$
\frac{{X}_{1} + {X}_{2}}{\sqrt{2}\sigma } \sim  N\left( {0,1}\right),\;\frac{1}{{\sigma }^{2}}\left( {{X}_{3}^{2} + {X}_{4}^{2} + {X}_{5}^{2}}\right)  \sim  {\chi }^{2}\left( 3\right)
$$

且 $\frac{{X}_{1} + {X}_{2}}{\sqrt{2}\sigma }$ 与 $\frac{1}{{\sigma }^{2}}\left( {{X}_{3}^{2} + {X}_{4}^{2} + {X}_{5}^{2}}\right)$ 独立,于是

$$
\frac{\frac{{X}_{1} + {X}_{2}}{\sqrt{2}\sigma }}{\sqrt{\frac{\frac{1}{{\sigma }^{2}}\left( {{X}_{3}^{2} + {X}_{4}^{2} + {X}_{5}^{2}}\right) }{3}}} = \frac{\sqrt{\frac{3}{2}}\left( {{X}_{1} + {X}_{2}}\right) }{\sqrt{{X}_{3}^{2} + {X}_{4}^{2} + {X}_{5}^{2}}} \sim  t\left( 3\right)  \Rightarrow  a = \sqrt{\frac{3}{2}}.
$$

#### 题型 3. 利用抽样分布求概率

【1.9】在总体 $N\left( {{12},4}\right)$ 中随机抽一容量为 5 的样本 ${X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}$.

(1)求样本均值与总体均值之差的绝对值大于 1 的概率.

(2)求概率 $P\left\{  {\max \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)  > {15}}\right\}$.

(3)求概率 $P\left\{  {\min \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)  < {10}}\right\}$.

解 (1) 因 $\bar{X} \sim  N\left( {{12},\frac{4}{5}}\right)$,所以

$$
P\{ \left| {\bar{X} - {12}}\right|  > 1\}  = P\left\{  {\left| \frac{\bar{X} - {12}}{\sqrt{\frac{4}{5}}}\right|  > \frac{\sqrt{5}}{2}}\right\}
$$

$$
= 2 - {2\Phi }\left( \frac{\sqrt{5}}{2}\right)  = 2 \times  \left\lbrack  {1 - \Phi \left( {1.12}\right) }\right\rbrack   = 2 \times  \left( {1 - {0.8686}}\right)  = 0.
$$

$$
\text{2628.}
$$

$$
\text{(2)}P\left\{  {\max \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)  > {15}}\right\}
$$

$$
= 1 - P\left\{  {{X}_{1} \leq  {15},{X}_{2} \leq  {15},{X}_{3} \leq  {15},{X}_{4} \leq  {15},{X}_{5} \leq  {15}}\right\}
$$

$$
= 1 - \mathop{\prod }\limits_{{i = 1}}^{5}P\left\{  {{X}_{i} \leq  {15}}\right\}   = 1 - \mathop{\prod }\limits_{{i = 1}}^{5}P\left\{  {\frac{{X}_{i} - {12}}{2} \leq  \frac{{15} - {12}}{2}}\right\}
$$

$$
= 1 - {\left\lbrack  \Phi \left( {1.5}\right) \right\rbrack  }^{5} = 1 - {\left( {0.9332}\right) }^{5} = {0.2923}\text{.}
$$

(3) $P\left\{  {\min \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)  < {10}}\right\}$

$$
= 1 - P\left\{  {{X}_{1} \geq  {10},{X}_{2} \geq  {10},{X}_{3} \geq  {10},{X}_{4} \geq  {10},{X}_{5} \geq  {10}}\right\}
$$

$$
= 1 - \mathop{\prod }\limits_{{i = 1}}^{5}P\left\{  {{X}_{i} \geq  {10}}\right\}   = 1 - \mathop{\prod }\limits_{{i = 1}}^{5}P\left\{  {\frac{{X}_{i} - {12}}{2} \geq  \frac{{10} - {12}}{2}}\right\}
$$

$$
= 1 - {\left\lbrack  1 - \Phi \left( -1\right) \right\rbrack  }^{5} = 1 - {\left\lbrack  \Phi \left( 1\right) \right\rbrack  }^{5}
$$

$$
= 1 - {\left( {0.8413}\right) }^{5} = {0.5785}.
$$

点评 本题 (2)、(3) 也可利用第三章的公式:

$M = \max \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)$ 的分布函数为

$$
{F}_{M}\left( z\right)  = {\left\lbrack  F\left( z\right) \right\rbrack  }^{5}.
$$

$N = \min \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)$ 的分布函数为

$$
{F}_{N}\left( z\right)  = 1 - {\left\lbrack  1 - F\left( z\right) \right\rbrack  }^{5}.
$$

则 (2) $P\{ M > {15}\}  = 1 - {F}_{M}\left( {15}\right)$.

(3) $P\{ N < {10}\}  = {F}_{N}\left( {10}\right)$.

【1. 10】设 $X \sim  N\left( {0,{0.3}^{2}}\right),\left( {{X}_{1},{X}_{2},\cdots,{X}_{10}}\right)$ 是取自 $X$ 的一个样本,求

$$
P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}^{2} > {1.44}}\right\} .
$$

解 由 ${X}_{i} \sim  N\left( {0,{0.3}^{2}}\right)$ 知

$$
\frac{{X}_{i}}{0.3} \sim  N\left( {0,1}\right),\;i = 1,2,\cdots,{10}
$$

故

$$
\mathop{\sum }\limits_{{i = 1}}^{{10}}{\left( \frac{{X}_{i}}{0.3}\right) }^{2} = \frac{1}{0.09} \cdot  \mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}^{2} \sim  {\chi }^{2}\left( {10}\right),
$$

$$
P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}^{2} > {1.44}}\right\}   = P\left\{  {\frac{1}{0.09}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}^{2} > \frac{1.44}{0.09}}\right\}
$$

$$
= P\left\{  {\frac{1}{0.09}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}^{2} > {16}}\right\}   = {0.1}.
$$

【1.11】从正态总体 $N\left( {{3.4},{6}^{2}}\right)$ 中抽取容量为 $n$ 的样本,如果要求其样本均值位于区间 $\left( {1,4,5,4}\right)$ 内的概率不小于 0.95,问样本容量 $n$ 至少应取多大?

附表:标准正态分布表

$$
\Phi \left( z\right)  = {\int }_{-\infty }^{z}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{t}^{2}}{2}}\mathrm{\;d}t
$$

<table><tr><td>$z$</td><td>1.28</td><td>1. 645</td><td>1.96</td><td>2.33</td></tr><tr><td>$\Phi \left( z\right)$</td><td>0.900</td><td>0.950</td><td>0.975</td><td>0.990</td></tr></table>

解 以 $\bar{X}$ 表示该样本均值,则

$$
\bar{X} \sim  N\left( {{3.4},\frac{{6}^{2}}{n}}\right),
$$

从而有

$$
P\{ {1.4} < \bar{X} < {5.4}\}  = P\{  - 2 < \bar{X} - {3.4} < 2\}  = P\{ \left| {\bar{X} - {3.4}}\right|  < 2\}
$$

$$
= P\left\{  {\frac{\left| \bar{X} - {3.4}\right| }{6}\sqrt{n} < \frac{2\sqrt{n}}{6}}\right\}   = {2\Phi }\left( \frac{\sqrt{n}}{3}\right)  - 1 \geq  {0.95}.
$$

故 $\Phi \left( \frac{\sqrt{n}}{3}\right)  \geq  {0.975}$. 由此得 $\frac{\sqrt{n}}{3} \geq  {1.96}$.

即 $n \geq  {\left( {1.96} \times  3\right) }^{2} \approx  {34.57}$,所以 $n$ 至少应取 35.

【1.12】从方差为 20 和 35 的正态总体分别抽取容量为 8 和 10 的两个样本. 试求第一个样本方差大于等于第二个样本方差两倍的概率.

分析 本题考察 $F$ 分布的判断以及 $F$ 分布表的熟练掌握程度.

解 由题意可知

$$
P\left\{  {{S}_{1}^{2} \geq  2{S}_{2}^{2}}\right\}   = P\left\{  {\frac{{S}_{1}^{2}}{{S}_{2}^{2}} \geq  2}\right\}
$$

$$
= P\left\{  {\frac{\frac{{S}_{1}^{2}}{20}}{\frac{{S}_{2}^{2}}{35}} \geq  2 \times  \frac{35}{20}}\right\}  \text{ (因为 }\frac{\frac{{S}_{1}^{2}}{{\sigma }_{1}^{2}}}{\frac{{S}_{2}^{2}}{{\sigma }_{2}^{2}}} \sim  F\left( {{n}_{1} - 1,{n}_{2} - 1}\right) \text{ ) }
$$

$$
= P\{ F \geq  {3.5}\} \text{,}
$$

其中 $F \sim  F\left( {7,9}\right)$ 分布,查 $F$ 分布表可得

$$
{F}_{0.05}\left( {7,9}\right)  = {3.29}, P\{ F > {3.29}\}  = {0.05},
$$

$$
{F}_{0.025}\left( {7,9}\right)  = {4.20}, P\{ F > {4.20}\}  = {0.025}.
$$

因为 ${3.29} < {3.5} < {4.20}$,所以 ${0.025} < P\{ F \geq  {3.5}\}  < {0.05}$.

根据插值求得 $P\{ F \geq  {3.5}\}  = {0.0276}$,即 $P\left\{  {{S}_{1}^{2} \geq  2{S}_{2}^{2}}\right\}   = {0.0276}$.

9 【1.13】设随机变量 $X \sim  t\left( n\right)$, $Y \sim  F\left( {1, n}\right)$,给定 $\alpha \left( {0 < \alpha  < {0.5}}\right)$,常数 $c$ 满足 $P\{ X > c\}  =$ $\alpha$,则 $P\left\{  {Y > {c}^{2}}\right\}   =$ _____.

(A) $\alpha$ (B) $1 - \alpha$ (C) ${2\alpha }$ (D) $1 - {2\alpha }$

解 $X \sim  t\left( n\right), Y \sim  F\left( {1, n}\right)$,则 ${X}^{2} \sim  F\left( {1, n}\right)$ 与 $Y$ 同分布.

所以 $P\left\{  {Y > {c}^{2}}\right\}   = P\left\{  {{X}^{2} > {c}^{2}}\right\}   = P\{ X > c\}  + P\{ X <  - c\}  = {2P}\{ X > c\}  = {2\alpha }$,

故应选(C).

点评 不同分布之间的关系也是考研中的常考题型. 本题考查的便是 $t$ 分布和 $F$ 分布之间的关系.

若 $X \sim  t\left( n\right)$,则 ${X}^{2} \sim  F\left( {1, n}\right)$.

另外,本题也用到了 $t$ 分布的对称性,即 $P\{ X > c\}  = P\{ X <  - c\}  = \alpha$. 如图所示.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_213_692_595_287_215_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_213_692_595_287_215_0.jpg)

【1.14】设在总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 中抽取一个容量为 16 的样本,求 $P\left\{  {\frac{{S}^{2}}{{\sigma }^{2}} \leq  {1.664}}\right\}$.

解 因为 $\frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)$,所以

$$
P\left\{  {\frac{{S}^{2}}{{\sigma }^{2}} \leq  {1.664}}\right\}   = P\left\{  {\frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \leq  \left( {n - 1}\right)  \times  {1.664}}\right\}
$$

$$
= P\left\{  {\frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \leq  {15} \times  {1.664}}\right\}
$$

$$
= P\left\{  {{\chi }^{2}\left( {n - 1}\right)  \leq  {24.96}}\right\}   = 1 - P\left\{  {{\chi }^{2}\left( {15}\right)  > {24.96}}\right\}
$$

$$
= 1 - {0.05} = {0.95}
$$

(其中 ${\chi }_{0.05}^{2}\left( {15}\right)  = {24.996}$ ).

【1.15】设 $X \sim  F\left( {n, n}\right),{p}_{1} = P\{ X \geq  1\},{p}_{2} = P\{ X \leq  1\}$,则(   ).

(A) ${p}_{1} < {p}_{2}$ (B) ${p}_{1} = {p}_{2}$ (C) ${p}_{1} > {p}_{2}$ (D) ${p}_{1}\text{、}{p}_{2}$ 无法比较

解 因为 $X \sim  F\left( {n, n}\right)$,所以 $\frac{1}{X} \sim  F\left( {n, n}\right)$,故

$$
{p}_{1} = P\{ X \geq  1\}  = P\left\{  {\frac{1}{X} \leq  1}\right\}   = P\{ X \leq  1\}  = {p}_{2}.
$$

则应选 (B).

【1.16】某厂生产的灯泡使用寿命 $X \sim  N\left( {{2250},{250}^{2}}\right)$ 分布,现进行质量检查,方法如下:任意挑选若干个灯泡,如果这些灯泡的平均寿命超过 2200 小时,就认为该厂生产的灯泡质量合格, 若要使检查能通过的概率超过 0.997, 问至少应检查多少个灯泡?

解 设至少应检查 $n$ 个灯泡,依题意有 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 均服从 $N\left( {{2250},{250}^{2}}\right)$,且相互独立.

$$
\bar{X} \sim  N\left( {{2250},\frac{{250}^{2}}{n}}\right),\;\frac{\bar{X} - {2250}}{\frac{250}{\sqrt{n}}} \sim  N\left( {0,1}\right),
$$

$$
P\{ \bar{X} > {2200}\}  = P\left\{  {\frac{\bar{X} - {2250}}{\frac{250}{\sqrt{n}}} > \frac{{2200} - {2250}}{\frac{250}{\sqrt{n}}}}\right\}
$$

$$
= 1 - P\left\{  {\frac{\bar{X} - {2250}}{\frac{250}{\sqrt{n}}} \leq  \frac{{2200} - {2250}}{\frac{250}{\sqrt{n}}}}\right\}
$$

$$
= 1 - \Phi \left( {-\frac{\sqrt{n}}{5}}\right)  = 1 - \left\lbrack  {1 - \Phi \left( \frac{\sqrt{n}}{5}\right) }\right\rbrack   = \Phi \left( \frac{\sqrt{n}}{5}\right)  \geq  {0.997}\text{,}
$$

查表得: $\frac{\sqrt{n}}{5} \geq  {2.75}, n \geq  {189.1}$,取 $n = {190}$.

即至少应检查 190 个灯泡.

#### 题型 4. 统计量求数字特征

方法与技巧 统计量求期望, 方差等数字特征是数理统计中的基本题型. 另外在后面的有关估计量的无偏性及有效性内容当中也会用到此类计算. 统计量求数字特征时经常用到以下公式, 需熟记:

$$
E\left( \bar{X}\right)  = E\left( X\right) \left( {\text{ 或 }\mu }\right),
$$

$$
D\left( \bar{X}\right)  = \frac{D\left( X\right) }{n}\left( {\text{ 或 }\frac{{\sigma }^{2}}{n}}\right),
$$

$$
E\left( {S}^{2}\right)  = D\left( X\right) \text{(或}{\sigma }^{2}\text{),}
$$

【1.17】设总体 $X$ 服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right),{X}_{1},{X}_{2},\cdots,{X}_{n}$ 为其样本, $\bar{X}$ 为均值, ${S}^{2}$ 为样本方差. 试求:

(1) $\bar{X}$ 的数学期望与方差.

(2) ${S}^{2}$ 的数学期望.

分析 本题既可以利用公式 $E\left( \bar{X}\right)  = E\left( X\right) \text{、}D\left( \bar{X}\right)  = \frac{D\left( X\right) }{n}\text{、}E\left( {S}^{2}\right)  = D\left( X\right)$ 直接计算,也可利用期望与方差的性质推导,其中在求 ${S}^{2}$ 的期望时,采用 ${S}^{2}$ 的另一种表达式,即

$$
{S}^{2} = \frac{1}{n - 1}\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - n{\bar{X}}^{2}}\right),
$$

问题就变得简单了.

解 (1) ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 相互独立且与 $X$ 有相同的分布,所以

$$
E\left( {X}_{i}\right)  = E\left( X\right),
$$

$$
E\left( \bar{X}\right)  = E\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E\left( {X}_{i}\right)  = \frac{1}{n}{nE}\left( X\right)  = E\left( X\right).
$$

故 $\;E\left( \bar{X}\right)  = E\left( X\right)  = \mu$.

又因为 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 相互独立,而且与 $X$ 分布相同,所以

$$
D\left( {X}_{i}\right)  = D\left( X\right) \;\left( {i = 1,2,\cdots, n}\right),
$$

$$
D\left( \bar{X}\right)  = D\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{{n}^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}D\left( {X}_{i}\right)  = \frac{1}{{n}^{2}}{nD}\left( X\right)  = \frac{1}{n}D\left( X\right).
$$

故 $\;D\left( \bar{X}\right)  = \frac{{\sigma }^{2}}{n}$.

(2) $E\left( {S}^{2}\right)  = E\left\lbrack  {\frac{1}{n - 1}\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - n{\bar{X}}^{2}}\right) }\right\rbrack   = \frac{1}{n - 1}\left\lbrack  {\mathop{\sum }\limits_{{i = 1}}^{n}E\left( {X}_{i}^{2}\right)  - {nE}\left( {\bar{X}}^{2}\right) }\right\rbrack$.

因为

$$
E\left( {X}_{i}^{2}\right)  = D\left( {X}_{i}\right)  + {\left\lbrack  E\left( {X}_{i}\right) \right\rbrack  }^{2}\;\left( {i = 1,2,\cdots, n}\right),
$$

$$
E\left( {\bar{X}}^{2}\right)  = D\left( \bar{X}\right)  + {\left\lbrack  E\left( \bar{X}\right) \right\rbrack  }^{2},
$$

因此

$$
E\left( {X}_{i}^{2}\right)  = D\left( X\right)  + {\left\lbrack  E\left( X\right) \right\rbrack  }^{2}\;\left( {i = 1,2,\cdots, n}\right),
$$

$$
E\left( {\bar{X}}^{2}\right)  = \frac{1}{n}D\left( X\right)  + {\left\lbrack  E\left( X\right) \right\rbrack  }^{2},
$$

故

$$
E\left( {S}^{2}\right)  = \frac{1}{n - 1}\left\{  {{nD}\left( X\right)  + n{\left\lbrack  E\left( X\right) \right\rbrack  }^{2} - D\left( X\right)  - n{\left\lbrack  E\left( X\right) \right\rbrack  }^{2}}\right\}   = D\left( X\right),
$$

所以 $E\left( {S}^{2}\right)  = {\sigma }^{2}$.

【1.18】设 ${X}_{1},{X}_{2},\cdots,{X}_{m}$ 为来自二项分布总体 $B\left( {n, p}\right)$ 的简单随机样本, $\bar{X}$ 和 ${S}^{2}$ 分别为样本均值和样本方差. 记统计量 $T = \bar{X} - {S}^{2}$,则 $E\left( T\right)  =$ _____.

解 因为 $X \sim  B\left( {n, p}\right)$,则 ${EX} = {np},{DX} = {np}\left( {1 - p}\right)$.

则 $E\left( T\right)  = E\left( {\bar{X} - {S}^{2}}\right)  = E\left( \bar{X}\right)  - E\left( {S}^{2}\right)$

$= {EX} - {DX} = {np} - {np}\left( {1 - p}\right)  = n{p}^{2}.$

故应填 $n{p}^{2}$.

【1.19】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为来自总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 的简单随机样本,记统计量 $T = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$, 则 $E\left( T\right)  =$ _____.

解 因为 ${X}_{i} \sim  N\left( {\mu,{\sigma }^{2}}\right)$,所以 $E{X}_{i} = \mu, D{X}_{i} = {\sigma }^{2}$. 则

$$
E\left( T\right)  = E\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}}\right)  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E\left( {X}_{i}^{2}\right)
$$

$$
= \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left\lbrack  {D{X}_{i} + {\left( E{X}_{i}\right) }^{2}}\right\rbrack   = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{\sigma }^{2} + {\mu }^{2}}\right)
$$

$$
= {\sigma }^{2} + {\mu }^{2}\text{.}
$$

9 【1. 20】设总体 $X$ 的概率密度为 $f\left( x\right)  = \frac{1}{2}{\mathrm{e}}^{-\left| x\right| }\left( {-\infty  < x <  + \infty }\right),{X}_{1},{X}_{2},\cdots,{X}_{n}$ 为总体 $X$ 的简单随机样本,其样本方差为 ${S}^{2}$,则 $E{S}^{2} =$ _____.

解 因为 $E\left( {S}^{2}\right)  = {DX}$,而

$$
{EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = 0,
$$

$E\left( {X}^{2}\right)  = {\int }_{-\infty }^{+\infty }{x}^{2}f\left( x\right) \mathrm{d}x = {\int }_{-\infty }^{+\infty }{x}^{2} \cdot  \frac{1}{2}{\mathrm{e}}^{-\left| x\right| }\mathrm{d}x$ 电 216

$$
= {\int }_{0}^{+\infty }{x}^{2}{\mathrm{e}}^{-x}\mathrm{\;d}x =  - {\left. {x}^{2}{\mathrm{e}}^{-x}\right| }_{0}^{+\infty } + {\int }_{0}^{+\infty }{2x}{\mathrm{e}}^{-x}\mathrm{\;d}x = 2,
$$

$$
{DX} = E\left( {X}^{2}\right)  - {\left( EX\right) }^{2} = 2,
$$

则 $E\left( {S}^{2}\right)  = 2$.

【1.21】设总体 $X$ 服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right) \left( {\sigma  > 0}\right)$. 从该总体中抽取简单随机样本 ${X}_{1},{X}_{2}$,

$\cdots,{X}_{2n}\left( {n \geq  2}\right)$. 其样本均值为 $\bar{X} = \frac{1}{2n}\mathop{\sum }\limits_{{i = 1}}^{{2n}}{X}_{i}$,试求统计量

$$
Y = \mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} + {X}_{n + i} - 2\bar{X}\right) }^{2}
$$

的数学期望 $E\left( Y\right)$.

解法一 由已知条件 ${X}_{1},{X}_{2},\cdots,{X}_{2n}$ 均服从 $N\left( {\mu,{\sigma }^{2}}\right)$ 且相互独立,

所以 $\left( {{X}_{1} + {X}_{n + 1}}\right),\left( {{X}_{2} + {X}_{n + 2}}\right),\cdots,\left( {{X}_{n} + {X}_{2n}}\right)$ 相互独立且服从 $N\left( {{2\mu },2{\sigma }^{2}}\right)$,故

$$
\left( {{X}_{1} + {X}_{n + 1}}\right),\left( {{X}_{2} + {X}_{n + 2}}\right),\cdots,\left( {{X}_{n} + {X}_{2n}}\right)
$$

可作为来自总体 $N\left( {{2\mu },2{\sigma }^{2}}\right)$ 的样本.

其样本均值为

$$
\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left( {{X}_{i} + {X}_{n + i}}\right)  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{{2n}}{X}_{i} = 2\bar{X},
$$

其样本方差为

$$
\frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} + {X}_{n + i} - 2\bar{X}\right) }^{2} = \frac{1}{n - 1}Y,
$$

因为 $E\left( {S}^{2}\right)  = {\sigma }^{2}$,故

$$
E\left( {\frac{1}{n - 1}Y}\right)  = 2{\sigma }^{2},\;\text{ 得 }\;E\left( Y\right)  = 2\left( {n - 1}\right) {\sigma }^{2}.
$$

解法二 记 ${\bar{X}}^{\prime } = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i},{\bar{X}}^{\prime \prime } = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{n + i}$,

显然有 $2\bar{X} = {\bar{X}}^{\prime } + {\bar{X}}^{\prime \prime }$. 因此

$$
E\left( Y\right)  = E\left\lbrack  {\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} + {X}_{n + i} - 2\bar{X}\right) }^{2}}\right\rbrack
$$

$$
= E\left\{  {\mathop{\sum }\limits_{{i = 1}}^{n}{\left\lbrack  \left( {X}_{i} - {\bar{X}}^{\prime }\right)  + \left( {X}_{n + i} - {\bar{X}}^{\prime \prime }\right) \right\rbrack  }^{2}}\right\}
$$

$$
= E\left\{  {\mathop{\sum }\limits_{{i = 1}}^{n}\left\lbrack  {{\left( {X}_{i} - {\bar{X}}^{\prime }\right) }^{2} + 2\left( {{X}_{i} - {\bar{X}}^{\prime }}\right) \left( {{X}_{n + i} - {\bar{X}}^{\prime \prime }}\right)  + {\left( {X}_{n + i} - {\bar{X}}^{\prime \prime }\right) }^{2}}\right\rbrack  }\right\}
$$

$$
= E\left\lbrack  {\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - {\bar{X}}^{\prime }\right) }^{2}}\right\rbrack   + 0 + E\left\lbrack  {\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{n + i} - {\bar{X}}^{\prime \prime }\right) }^{2}}\right\rbrack
$$

$$
= \left( {n - 1}\right) {\sigma }^{2} + \left( {n - 1}\right) {\sigma }^{2} = 2\left( {n - 1}\right) {\sigma }^{2}.
$$

解法三 $Y = \mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} + {X}_{n + i} - 2\bar{X}\right) }^{2}$

$$
= \mathop{\sum }\limits_{{i = 1}}^{n}\left( {{X}_{i}^{2} + {X}_{n + i}^{2} + 2{X}_{i}{X}_{n + i} - 4\bar{X}{X}_{i} - 4\bar{X}{X}_{n + i} + 4{\bar{X}}^{2}}\right)
$$

$$
= \mathop{\sum }\limits_{{i = 1}}^{{2n}}{X}_{i}^{2} + 2\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}{X}_{n + i} - 4\bar{X}\mathop{\sum }\limits_{{i = 1}}^{{2n}}{X}_{i} + {4n}{\bar{X}}^{2}
$$

$$
= \mathop{\sum }\limits_{{i = 1}}^{{2n}}{X}_{i}^{2} + 2\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}{X}_{n + i} - {4n}{\bar{X}}^{2}.
$$

又由 $D\bar{X} = E\left( {\bar{X}}^{2}\right)  - {\left( E\bar{X}\right) }^{2}$ 可得, $E\left( {\bar{X}}^{2}\right)  = \frac{{\sigma }^{2}}{2n} + {\mu }^{2}$.

同理 $E{X}_{i}^{2} = {\mu }^{2} + {\sigma }^{2}$.

因此 $E\left( Y\right)  = \mathop{\sum }\limits_{{i = 1}}^{{2n}}E{X}_{i}^{2} + 2\mathop{\sum }\limits_{{i = 1}}^{n}E{X}_{i}E{X}_{n + i} - {4nE}\left( {\bar{X}}^{2}\right)$

$= {2n}\left( {{\sigma }^{2} + {\mu }^{2}}\right)  + {2n}{\mu }^{2} - {4n}\left( {\frac{{\sigma }^{2}}{2n} + {\mu }^{2}}\right)  = 2\left( {n - 1}\right) {\sigma }^{2}.$

点评 本题方法一和方法二都用到了 $E\left( {S}^{2}\right)  = {\sigma }^{2}$ 这个结论,非常方便.

【1.22】设总体 $X$ 服从参数 $\lambda \left( {\lambda  > 0}\right)$ 的泊松分布, ${X}_{1},{X}_{2},\cdots,{X}_{n}\left( {n \geq  2}\right)$ 为来自总体的简单随机样本,则对于统计量 ${T}_{1} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i},{T}_{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{{n - 1}}{X}_{i} + \frac{1}{n}{X}_{n}$ 有_____.

(A) $E{T}_{1} > E{T}_{2}, D{T}_{1} > D{T}_{2}$ (B) $E{T}_{1} > E{T}_{2}, D{T}_{1} < D{T}_{2}$

(C) $E{T}_{1} < E{T}_{2}, D{T}_{1} > D{T}_{2}$ (D) $E{T}_{1} < E{T}_{2}, D{T}_{1} < D{T}_{2}$

解 由 ${X}_{1},\cdots,{X}_{n} \sim  P\left( \lambda \right)$ 知

$$
E{X}_{i} = \lambda, D{X}_{i} = \lambda, i = 1,2,\cdots, n.
$$

从而 $E{T}_{1} = E\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \lambda$,

$$
E{T}_{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{{n - 1}}E{X}_{i} + \frac{1}{n}E{X}_{n} = \lambda  + \frac{\lambda }{n},
$$

故 $E{T}_{1} < E{T}_{2}$,

$$
D{T}_{1} = \frac{1}{{n}^{2}}D\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{n\lambda }{{n}^{2}} = \frac{\lambda }{n},
$$

$$
D{T}_{2} = \frac{1}{{\left( n - 1\right) }^{2}}\mathop{\sum }\limits_{{i = 1}}^{{n - 1}}D{X}_{i} + \frac{1}{{n}^{2}}D{X}_{n}
$$

$$
= \frac{\lambda }{n - 1} + \frac{\lambda }{{n}^{2}} > \frac{\lambda }{n} = D{T}_{1}.
$$

故应选(D).

【1.23】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是取自 $N\left( {0,{\sigma }^{2}}\right)$ 的简单样本, ${\bar{X}}_{k} = \frac{1}{k}\mathop{\sum }\limits_{{i = 1}}^{k}{X}_{i},1 \leq  k \leq  n$,则 $\operatorname{Cov}\left( {{\bar{X}}_{k},{\bar{X}}_{k + 1}}\right)  =$ (   ).

(A) ${\sigma }^{2}$ (B) $\frac{{\sigma }^{2}}{k}$ (C) $\frac{{\sigma }^{2}}{k + 1}$ (D) $\frac{{\sigma }^{2}}{k\left( {k + 1}\right) }$

解 $\operatorname{Cov}\left( {{\bar{X}}_{k},{\bar{X}}_{k + 1}}\right)  = \frac{1}{k\left( {k + 1}\right) }\operatorname{Cov}\left( {\mathop{\sum }\limits_{{i = 1}}^{k}{X}_{i},\mathop{\sum }\limits_{{i = 1}}^{k}{X}_{i} + {X}_{k + 1}}\right)$

$= \frac{1}{k\left( {k + 1}\right) }\operatorname{Cov}\left( {\mathop{\sum }\limits_{{i = 1}}^{k}{X}_{i},\mathop{\sum }\limits_{{i = 1}}^{k}{X}_{i}}\right)  = \frac{1}{k\left( {k + 1}\right) }D\left( {\mathop{\sum }\limits_{{i = 1}}^{k}{X}_{i}}\right)$

$= \frac{1}{k\left( {k + 1}\right) } \cdot  k{\sigma }^{2} = \frac{{\sigma }^{2}}{k + 1}.$

故应选(C).


【1.24】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 的样本,记 $Y = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left| {{X}_{i} - \mu }\right|$,试证:

$$
E\left( Y\right)  = \sqrt{\frac{2}{\pi }}\sigma,\;D\left( Y\right)  = \left( {1 - \frac{2}{\pi }}\right) \frac{{\sigma }^{2}}{n}.
$$

分析 ${Y}_{i} = {X}_{i} - \mu  \sim  N\left( {0,{\sigma }^{2}}\right), E\left( \left| {Y}_{i}\right| \right)  = \frac{2}{\sqrt{2\pi }\sigma }{\int }_{0}^{+\infty }y{\mathrm{e}}^{\frac{{y}^{2}}{2{\sigma }^{2}}}\mathrm{\;d}y$.

证 记 ${Y}_{i} = {X}_{i} - \mu$,得 ${Y}_{i} \sim  N\left( {0,{\sigma }^{2}}\right), i = 1,2,\cdots, n$.

$$
E\left( \left| {{X}_{i} - \mu }\right| \right)  = E\left( \left| {Y}_{i}\right| \right)  = \frac{1}{\sqrt{2\pi }\sigma }{\int }_{-\infty }^{+\infty }\left| y\right| {\mathrm{e}}^{-\frac{{y}^{2}}{2{\sigma }^{2}}}\mathrm{d}y = \frac{2}{\sqrt{2\pi }\sigma }{\int }_{0}^{+\infty }y{\mathrm{e}}^{-\frac{{y}^{2}}{2{\sigma }^{2}}}\mathrm{\;d}y
$$

$$
=  - {\left. \frac{2\sigma }{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{y}^{2}}{2{\sigma }^{2}}}\right| }_{0}^{+\infty } = \sqrt{\frac{2}{\pi }}\sigma.
$$

$$
D\left( \left| {{X}_{i} - \mu }\right| \right)  = D\left( \left| {Y}_{i}\right| \right)  = E\left( {Y}_{i}^{2}\right)  - {\left\lbrack  E\left( \left| {Y}_{i}\right| \right) \right\rbrack  }^{2}
$$

$$
= D\left( {Y}_{i}\right)  + {\left( E{Y}_{i}\right) }^{2} - {\left( \sqrt{\frac{2}{\pi }}\sigma \right) }^{2}
$$

$$
= {\sigma }^{2} + 0 - \frac{2}{\pi }{\sigma }^{2} = \left( {1 - \frac{2}{\pi }}\right) {\sigma }^{2}.
$$

所以 $E\left( Y\right)  = E\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left| {{X}_{i} - \mu }\right| }\right)  = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E\left( \left| {{X}_{i} - \mu }\right| \right)$

$$
= \frac{1}{n} \cdot  n\sqrt{\frac{2}{\pi }}\sigma  = \sqrt{\frac{2}{\pi }}\sigma,
$$

$$
D\left( Y\right)  = D\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left| {{X}_{i} - \mu }\right| }\right)  = \frac{1}{{n}^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}D\left( \left| {{X}_{i} - \mu }\right| \right)
$$

$$
= \left( {1 - \frac{2}{\pi }}\right) \frac{{\sigma }^{2}}{n}.
$$

题型 5. 关于分位点

【1.25】设 $F \sim  F\left( {m, n}\right)$,证明: ${F}_{1 - \alpha }\left( {m, n}\right)  = \frac{1}{{F}_{\alpha }\left( {n, m}\right) }$.

证 由分位点定义:

$$
1 - \alpha  = P\left\{  {F > {F}_{1 - \alpha }\left( {m, n}\right) }\right\}   = P\left\{  {\frac{1}{F} < \frac{1}{{F}_{1 - \alpha }\left( {m, n}\right) }}\right\}
$$

$$
= 1 - P\left\{  {\frac{1}{F} > \frac{1}{{F}_{1 - \alpha }\left( {m, n}\right) }}\right\} ,
$$

则 $P\left\{  {\frac{1}{F} > \frac{1}{{F}_{1 - \alpha }\left( {m, n}\right) }}\right\}   = \alpha$,

由 $F$ 分布性质可知 $\frac{1}{F} \sim  F\left( {n, m}\right)$,故 $\frac{1}{{F}_{1 - \alpha }\left( {m, n}\right) } = {F}_{\alpha }\left( {n, m}\right)$,

即 ${F}_{1 - \alpha }\left( {m, n}\right)  = \frac{1}{{F}_{\alpha }\left( {n, m}\right) }$.

#### 题型 6. 关于样本及统计量

【1.26】设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,其中 $\mu$ 和 ${\sigma }^{2}$ 都是未知参数,随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体的样本.

(1)写出样本 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的样本空间和联合分布密度；

(2)指出下列样本函数哪些是统计量,哪些不是统计量.

$$
{T}_{1} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}
$$

$$
{T}_{3} = 2{X}_{2} + {X}_{3},
$$

$$
{T}_{4} = \max \left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right),
$$

$$
{T}_{5} = \frac{{X}_{1} - \mu }{\sigma },\;{T}_{6} = \mathop{\sum }\limits_{{i = 1}}^{n}{\left( \frac{{X}_{i}}{\sigma }\right) }^{2}.
$$

解 (1) 样本空间

$$
\Omega  = \left\{  {\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)  \mid  {x}_{i} \in  R, i = 1,2,\cdots, n}\right\}   = {R}^{n}.
$$

联合分布密度

$$
f\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}f\left( {x}_{i}\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}\frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{\frac{{\left( {x}_{i} - \mu \right) }^{2}}{2{\sigma }^{2}}}
$$

$$
= \frac{1}{{\left( 2\pi \right) }^{\frac{n}{2}}{\sigma }^{n}}{\mathrm{e}}^{-\frac{1}{2{\sigma }^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {x}_{i} - \mu \right) }^{2}}.
$$

(2) 因为 ${T}_{1},{T}_{3},{T}_{4}$ 中不含未知参数,故 ${T}_{1},{T}_{3},{T}_{4}$ 是统计量,而 ${T}_{2},{T}_{5},{T}_{6}$ 中含未知参数 (其中 ${T}_{2}$ 中 $E{X}_{1} = \mu$ ),故 ${T}_{2},{T}_{5},{T}_{6}$ 不是统计量.

【1.27】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 和 ${Y}_{1},{Y}_{2},\cdots,{Y}_{n}$ 是两个样本,且有如下关系: ${Y}_{i} = \frac{1}{b}\left( {{X}_{i} - a}\right)$ $\left( {i = 1,2,\cdots, n, a, b\text{不等于零都为常数}}\right)$,试求样本均值 $\bar{X}$ 和 $\bar{Y}$,修正的样本方差 ${S}_{X}^{2}$ 与 ${S}_{Y}^{2}$ 之间的关系.

解 $\bar{Y} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{Y}_{i} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\frac{1}{b}\left( {{X}_{i} - a}\right)  = \frac{1}{b}\left( {\bar{X} - a}\right)$.

则得 $\bar{X} = b\bar{Y} + a$.

$$
{S}_{Y}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {Y}_{i} - \bar{Y}\right) }^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( \frac{{X}_{i} - a}{b} - \frac{\bar{X} - a}{b}\right) }^{2}
$$

$$
= \frac{1}{{b}^{2}}\frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} = \frac{1}{{b}^{2}}{S}_{X}^{2}.
$$

即得 ${S}_{X}^{2} = {b}^{2}{S}_{Y}^{2}$.

点评 当样本值 ${x}_{1},{x}_{2},\cdots,{x}_{n}$ 中的每一个分量过大或过小时,为了计算简便,提高精度,可适当选择常数 $a, b \neq  0$,作线性变换 ${y}_{i} = \frac{1}{b}\left( {{x}_{i} - a}\right) \left( {i = 1,2,\cdots, n}\right)$,使变换后的数据 ${y}_{1},{y}_{2},\cdots$, ${y}_{n}$ 大小适中,首先计算 $\bar{Y},{S}_{Y}^{2}$,只需做上述线性变换即得 $\bar{X}$ 和 ${S}_{X}^{2}$ 的值.

#### 题型 7. 求经验分布函数

【1.28】设对总体 $X$ 得到一个容量为 10 的样本,样本值分别为

$$
{4.5},2,1,{1.5},{3.5},{4.5},{6.5},5,{3.5},4
$$

分别计算样本均值, 样本方差和经验分布函数.

解 因为 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$,所以 $\bar{x} = \frac{1}{10}\mathop{\sum }\limits_{{i = 1}}^{{10}}{x}_{i} = {3.6}$.

因为 ${S}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}$,所以

$$
{s}^{2} = \frac{1}{9}\mathop{\sum }\limits_{{i = 1}}^{{10}}{\left( {x}_{i} - \bar{x}\right) }^{2}\text{ 或 }\frac{1}{9}\left( {\mathop{\sum }\limits_{{i = 1}}^{{10}}{x}_{i}^{2} - {10}{\bar{x}}^{2}}\right)
$$

$= {2.88}$.

将 10 个样本值由小到大排序为

$$
1 < {1.5} < 2 < {3.5} = {3.5} < 4 < {4.5} = {4.5} < 5 < {6.5}\text{,}
$$

其经验分布函数为

$$
{F}_{n}\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 1 \\  \frac{1}{10}, & 1 \leq  x < {1.5} \\  \frac{2}{10}, & {1.5} \leq  x < 2 \\  \frac{3}{10}, & 2 \leq  x < {3.5} \\  \frac{5}{10}, & {3.5} \leq  x < 4 \\  \frac{6}{10}, & 4 \leq  x < {4.5} \\  \frac{8}{10}, & {4.5} \leq  x < 5 \\  \frac{9}{10}, & 5 \leq  x < {6.5} \\  \frac{9}{10}, & 5 \leq  x < {6.5} \end{array}\right.
$$

#### 题型 8. 画直方图

【1.29】下面列出了 30 个美国NBA球员的体重(以磅计,1 磅 = 0.454kg)数据. 这些数据是从美国NBA球队 1990 ~ 1991 赛季的花名册中抽样得到的.

<table><tr><td>225</td><td>232</td><td>232</td><td>245</td><td>235</td><td>245</td><td>270</td><td>225</td><td>240</td><td>240</td></tr><tr><td>217</td><td>195</td><td>225</td><td>185</td><td>200</td><td>220</td><td>200</td><td>210</td><td>271</td><td>240</td></tr><tr><td>220</td><td>230</td><td>215</td><td>252</td><td>225</td><td>220</td><td>206</td><td>185</td><td>227</td><td>236</td></tr></table>

画出这些数据的频率直方图(提示: 最大和最小观察值分别为 271 和 185,区间[184.5,271.5] 包含所有数据,将整个区间分为 5 等份,为计算方便,将区间调整为 (179.5,279.5)).

解 最大和最小观察值分别为 271 和 185, 考虑到这些数据是将实测数据经四舍五入后得到的,取区间 $I = \left\lbrack  {{184.5},{271.5}}\right\rbrack$ 使得所有实测数据都落在 $I$ 上. 将区间 $I$ 等分为若干小区间,小区间的个数与数据个数 $n$ 有关,取为 $\sqrt{n}$ 左右为佳. 现在取小区间的个数为 5,于是小区间的长度为 $\frac{{271.5} - {184.5}}{5} = {17.4}$. 这一长度使用起来不方便. 为此,将区间 $I$ 的下限延伸至179.5,上限延伸至 279.5,这样小区间的长度调整为

$$
\Delta  = \frac{{279.5} - {179.5}}{5} = {20}.
$$

数出落在每小区间内的数据的个数 ${f}_{i}, i = 1,2,3,4,5$,算出数据落在各个小区间的频率 $\frac{{f}_{i}}{n}$ ( $n$ $= {30}, i = 1,2,3,4,5)$,所得结果列表如下:

<table><tr><td>组 限</td><td>频数 ${f}_{i}$</td><td>频率 $\frac{{f}_{i}}{n}$</td><td>累积频率</td></tr><tr><td>179.5 ~ 199.5</td><td>3</td><td>0.1</td><td>0.10</td></tr><tr><td>199.5 ~ 219.5</td><td>6</td><td>0.2</td><td>0.30</td></tr><tr><td>219.5 ~ 239.5</td><td>13</td><td>0.43</td><td>0.73</td></tr><tr><td>239.5 ~ 259.5</td><td>6</td><td>0.2</td><td>0.93</td></tr><tr><td>259.5 ~ 279.5</td><td>2</td><td>0.07</td><td>1</td></tr></table>

在每个小区间上作以对应的频率为高 (或者以 $\frac{{f}_{i}}{n\Delta }$ 为高) 以小区间为底的小长方形,这就是所求的频率直方图 (如图 6-1.29).

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_221_553_689_571_276_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_221_553_689_571_276_0.jpg)

图 6-1.29

【1.30】观察一个连续型随机变量, 抽到 100 株豫农一号玉米的穗位(单位:cm), 得到下列表中所列数据,按区间 $\lbrack {70},{80})$, $\lbrack {80},{90})$, $\cdots$, $\lbrack {150},{160})$,将 100 个数据分成 9 个组,列出分组数据的统计表 (包括频率及累积频率), 并画出频率的直方图.

<table><tr><td>127</td><td>118</td><td>121</td><td>113</td><td>145</td><td>125</td><td>87</td><td>94</td><td>118</td><td>111</td></tr><tr><td>102</td><td>72</td><td>113</td><td>76</td><td>101</td><td>134</td><td>107</td><td>118</td><td>114</td><td>128</td></tr><tr><td>118</td><td>114</td><td>117</td><td>120</td><td>128</td><td>94</td><td>124</td><td>87</td><td>88</td><td>105</td></tr><tr><td>115</td><td>134</td><td>89</td><td>141</td><td>114</td><td>119</td><td>150</td><td>107</td><td>126</td><td>95</td></tr><tr><td>137</td><td>108</td><td>129</td><td>136</td><td>98</td><td>121</td><td>91</td><td>111</td><td>134</td><td>123</td></tr><tr><td>103</td><td>104</td><td>107</td><td>121</td><td>94</td><td>126</td><td>108</td><td>114</td><td>103</td><td>129</td></tr><tr><td>109</td><td>84</td><td>117</td><td>112</td><td>112</td><td>125</td><td>94</td><td>73</td><td>93</td><td>94</td></tr><tr><td>102</td><td>108</td><td>158</td><td>89</td><td>127</td><td>115</td><td>112</td><td>94</td><td>118</td><td>114</td></tr><tr><td>88</td><td>111</td><td>111</td><td>104</td><td>101</td><td>129</td><td>144</td><td>128</td><td>131</td><td>142</td></tr></table>

解 分组数据统计表为 122 2 频率直方图和累积频率直方图分别为如下图 6-1.30-1 及 6-1.30-2 所示. 题型 9. 综合提高题型

<table><tr><td>分组编号</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td><td>9</td></tr><tr><td/><td>70</td><td>80</td><td>90</td><td>100</td><td>110</td><td>120</td><td>130</td><td>140</td><td>150</td></tr><tr><td>组 限</td><td>80</td><td>│ 90</td><td>100</td><td>110</td><td>│ 120</td><td>130</td><td>│ 140</td><td>│ 150</td><td>│ 160</td></tr><tr><td>组中值</td><td>75</td><td>85</td><td>95</td><td>105</td><td>115</td><td>125</td><td>135</td><td>145</td><td>155</td></tr><tr><td>组频数</td><td>3</td><td>9</td><td>13</td><td>16</td><td>26</td><td>20</td><td>7</td><td>4</td><td>2</td></tr><tr><td>组频率(%)</td><td>3</td><td>9</td><td>13</td><td>16</td><td>26</td><td>20</td><td>7</td><td>4</td><td>2</td></tr><tr><td>累积频率(%)</td><td>3</td><td>12</td><td>25</td><td>41</td><td>67</td><td>87</td><td>94</td><td>98</td><td>100</td></tr></table>

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_222_318_622_446_396_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_222_318_622_446_396_0.jpg)

图 6-1.30-1

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_222_793_588_440_431_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_222_793_588_440_431_0.jpg)

图 6-1.30-2

【1.31】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自正态总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 的简单随机样本, $\bar{X}$ 是样本均值,记

${S}_{1}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2},$ ${S}_{2}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2},$

${S}_{3}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2},$ ${S}_{4}^{2} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2},$

则服从自由度为 $n - 1$ 的 $t$ 分布的随机变量是 (   ).

(A) $t = \frac{\bar{X} - \mu }{\frac{{S}_{1}}{\sqrt{n - 1}}}$ (B) $t = \frac{\bar{X} - \mu }{\frac{{S}_{2}}{\sqrt{n - 1}}}$ (C) $t = \frac{\bar{X} - \mu }{\frac{{S}_{3}}{\sqrt{n}}}$ (D) $t = \frac{\bar{X} - \mu }{\frac{{S}_{4}}{\sqrt{n}}}$.

分析 根据 $t$ 分布的表达形式及推导可判断出正确选项.

解 因为 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 服从 $N\left( {\mu,{\sigma }^{2}}\right)$ 分布,所以有

$\frac{\bar{X} - \mu }{\sigma }\sqrt{n} \sim  N\left( {0,1}\right),\;\mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {X}_{i} - \bar{X}\right) }^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right),$

$$
\frac{\bar{X} - \mu }{\sqrt{\frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}}}\sqrt{n} \sim  t\left( {n - 1}\right),
$$

所以

$$
\frac{\left( {\bar{X} - \mu }\right) \sqrt{n}}{\sqrt{\frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}}} = \frac{\bar{X} - \mu }{\sqrt{\frac{1}{n} \cdot  \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}}} = \frac{\bar{X} - \mu }{\frac{{S}_{2}}{\sqrt{n - 1}}} \sim  t\left( {n - 1}\right).
$$

故答案为 (B).

点评 如果牢记正态总体抽样分布的有关结论, 则此题也直接选 (B).

【1.32】设随机变量 $X$ 和 $Y$ 相互独立且都服从正态分布 $N\left( {0,{3}^{2}}\right)$,而 ${X}_{1},\cdots,{X}_{9}$ 和 ${Y}_{1},\cdots$, ${Y}_{9}$ 分别是来自总体 $X$ 和 $Y$ 的简单随机样本,则统计量 $U = \frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{9}}{\sqrt{{Y}_{1}^{2} + {Y}_{2}^{2} + \cdots  + {Y}_{9}^{2}}}$ 服从_____分布,参数为_____.

分析 ${X}_{1},\cdots,{X}_{9}$ 相互独立且与 $X$ 同分布,所以 $\frac{1}{9}\left( {{X}_{1} + \cdots  + {X}_{9}}\right)  \sim  N\left( {0,1}\right)$,同理 $\frac{1}{9}\left( {{Y}_{1}^{2} + }\right.$ $\left. {\cdots  + {Y}_{9}^{2}}\right)  \sim  {\chi }^{2}\left( 9\right)$.

解 因为 ${X}_{i} \sim  N\left( {0,{3}^{2}}\right) \left( {i = 1,\cdots,9}\right)$,所以 ${X}_{1} + {X}_{2} + \cdots  + {X}_{9} \sim  N\left( {0,{9}^{2}}\right)$,则

$$
\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{9}}{9} \sim  N\left( {0,1}\right).
$$

因为 ${Y}_{i} \sim  N\left( {0,{3}^{2}}\right)$,所以 $\frac{{Y}_{i}}{3} \sim  N\left( {0,1}\right)$,则

$$
\frac{1}{9}\left( {{Y}_{1}^{2} + {Y}_{2}^{2} + \cdots  + {Y}_{9}^{2}}\right)  \sim  {\chi }^{2}\left( 9\right).
$$

由 $t$ 分布的定义可知

$$
\frac{{X}_{1} + {X}_{2} + \cdots  + {X}_{9}}{\sqrt{{Y}_{1}^{2} + {Y}_{2}^{2} + \cdots  + {Y}_{9}^{2}}} = \frac{\frac{1}{9}\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{9}}\right) }{\frac{1}{9}\sqrt{{Y}_{1}^{2} + {Y}_{2}^{2} + \cdots  + {Y}_{9}^{2}}} \sim  t\left( 9\right),
$$

因此 $U$ 服从 $t$ 分布,参数为 9.

【1.33】设 ${X}_{1},{X}_{2},\cdots,{X}_{10}$ 是来自标准正态总体的一组简单随机样本,

$$
Y = \frac{1}{2}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}^{2} + \mathop{\sum }\limits_{{i = 1}}^{5}{X}_{{2i} - 1}{X}_{2i},
$$

则 ${EY} = \underline{\;};Y$ 服从_____分布；参数是_____.

解 因为 $E{X}_{i} = 0, E{X}_{i}^{2} = D{X}_{i} = 1$,所以 ${EY} = 5$;

$$
Y = {\left( \frac{{X}_{1} + {X}_{2}}{\sqrt{2}}\right) }^{2} + \cdots  + {\left( \frac{{X}_{9} + {X}_{10}}{\sqrt{2}}\right) }^{2} \sim  {\chi }^{2}\left( 5\right).
$$

其中 $\frac{{X}_{1} + {X}_{2}}{\sqrt{2}} \sim  N\left( {0,1}\right),\cdots,\frac{{X}_{9} + {X}_{10}}{\sqrt{2}} \sim  N\left( {0,1}\right)$.

【1.34】设 ${X}_{1},{X}_{2},\cdots \cdots,{X}_{n}\left( {n \geq  2}\right)$ 为来自总体 $N\left( {\mu,1}\right)$ 的简单随机样本,记 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$, 则下列结论中不正确的是_____.


224 (A) $\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2}$ 服从 ${\chi }^{2}$ 分布 (B) $2{\left( {X}_{n} - {X}_{1}\right) }^{2}$ 服从 ${\chi }^{2}$ 分布

(C) $\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}$ 服从 ${\chi }^{2}$ 分布 (D) $n{\left( \bar{X} - \mu \right) }^{2}$ 服从 ${\chi }^{2}$ 分布

解 ${X}_{i} - \mu  \sim  N\left( {0,1}\right)$,则 $\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \mu \right) }^{2} \sim  {\chi }^{2}\left( n\right)$,故 (A) 正确;

$\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} = \left( {n - 1}\right) {S}^{2} \sim  {\chi }^{2}\left( {n - 1}\right),$,故 (C) 正确;

$\bar{X} \sim  N\left( {\mu,\frac{1}{n}}\right)$,则 $\frac{\bar{X} - \mu }{1/\sqrt{n}} \sim  N\left( {0,1}\right)$,

故 $n{\left( \bar{X} - \mu \right) }^{2} \sim  {\chi }^{2}\left( 1\right),\left( \mathrm{D}\right)$ 正确;

因为 ${X}_{n} - {X}_{1} \sim  N\left( {0,2}\right)$,故 $\frac{{X}_{n} - {X}_{1}}{\sqrt{2}} \sim  N\left( {0,1}\right)$,则 $\frac{{\left( {X}_{n} - {X}_{1}\right) }^{2}}{2} \sim  {\chi }^{2}\left( 1\right)$,故 (B) 不正确.

【1.35】设 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$ 是来自总体 $N\left( {0,{2}^{2}}\right)$ 的样本.

( 1 )求常数 $C$,使 $Y = C\left\lbrack  {{\left( {X}_{1} - {X}_{2}\right) }^{2} + {\left( {X}_{3} + {X}_{4}\right) }^{2}}\right\rbrack$ 服从 ${\chi }^{2}$ 分布,并指出自由度是多少？

(2)证明 $Z = \frac{{\left( {X}_{1} - {X}_{2}\right) }^{2}}{{\left( {X}_{3} + {X}_{4}\right) }^{2}}$ 服从 $F\left( {1,1}\right)$.

(1)解 因为 ${X}_{i} \sim  N\left( {0,{2}^{2}}\right), i = 1,2,3,4$. 故

$$
{X}_{1} - {X}_{2} \sim  N\left( {0,8}\right),\;{X}_{3} + {X}_{4} \sim  N\left( {0,8}\right).
$$

则

$$
\frac{{X}_{1} - {X}_{2}}{\sqrt{8}} \sim  N\left( {0,1}\right),\;\frac{{X}_{3} + {X}_{4}}{\sqrt{8}} \sim  N\left( {0,1}\right),
$$

所以

$$
\frac{{\left( {X}_{1} - {X}_{2}\right) }^{2}}{8} + \frac{{\left( {X}_{3} + {X}_{4}\right) }^{2}}{8} \sim  {\chi }^{2}\left( 2\right).
$$

故 $C = \frac{1}{8}, n = 2$.

(2) 证 因为 $\frac{{\left( {X}_{1} - {X}_{2}\right) }^{2}}{8} \sim  {\chi }^{2}\left( 1\right),\frac{{\left( {X}_{3} + {X}_{4}\right) }^{2}}{8} \sim  {\chi }^{2}\left( 1\right)$.

由 $F$ 分布的定义可知: $Z = \frac{{\left( {X}_{1} - {X}_{2}\right) }^{2}}{{\left( {X}_{3} + {X}_{4}\right) }^{2}}$ 服从 $F\left( {1,1}\right)$.

【1.36】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}\left( {n \geq  2}\right)$ 为来自总体 $N\left( {0,1}\right)$ 的简单随机样本, $\bar{X}$ 为样本均值, ${S}^{2}$ 为样本方差, 则 (   ).

(A) $n\bar{X} \sim  N\left( {0,1}\right)$ (B) $n{S}^{2} \sim  {\chi }^{2}\left( n\right)$

(C) $\frac{\left( {n - 1}\right) \bar{X}}{S} \sim  t\left( {n - 1}\right)$ (D) $\frac{\left( {n - 1}\right) {X}_{1}^{2}}{\mathop{\sum }\limits_{{i = 2}}^{n}{X}_{i}^{2}} \sim  F\left( {1, n - 1}\right)$

解 因为 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为总体 $N\left( {0,1}\right)$ 的简单随机样本,所以

$$
\bar{X} \sim  N\left( {0,\frac{1}{n}}\right),\;n\bar{X} \sim  N\left( {0, n}\right),
$$

$$
\left( {n - 1}\right) {S}^{2} = \mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} \sim  {\chi }^{2}\left( {n - 1}\right),
$$

$$
\frac{\bar{X}}{\frac{S}{\sqrt{n}}} = \frac{\sqrt{n}\bar{X}}{S} \sim  t\left( {n - 1}\right),
$$

故 (A)、(B)、(C) 不正确.

而

$$
{X}_{1}^{2} \sim  {\chi }^{2}\left( 1\right),\;\mathop{\sum }\limits_{{i = 2}}^{n}{X}_{i}^{2} \sim  {\chi }^{2}\left( {n - 1}\right),
$$

$$
\frac{{X}_{1}^{2}}{\frac{\mathop{\sum }\limits_{{i = 2}}^{n}{X}_{i}^{2}}{n - 1}} = \frac{\left( {n - 1}\right) {X}_{1}^{2}}{\mathop{\sum }\limits_{{i = 2}}^{n}{X}_{i}^{2}} \sim  F\left( {1, n - 1}\right).
$$

故答案为(D).

【1.37】设总体 $X$ 服从正态分布 $N\left( {0,{\sigma }^{2}}\right) \left( {\sigma }^{2}\right)$ 已知 $),{X}_{1},\cdots,{X}_{n}$ 是取自总体 $X$ 的简单随机样本, ${S}^{2}$ 为样本方差,则 (   ).

(A) $\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} \sim  {\chi }^{2}\left( n\right)$ (B) ${\left( \frac{{X}_{i}}{\sigma }\right) }^{2} + \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( n\right)$

(C) $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( \frac{{X}_{i}}{\sigma }\right) }^{2} + \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( n\right)$ (D) $\frac{1}{n}{\left( \mathop{\sum }\limits_{{i = 1}}^{n}\frac{{X}_{i}}{\sigma }\right) }^{2} + \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( n\right)$

解 ${X}_{i} \sim  N\left( {0,{\sigma }^{2}}\right),\;\frac{{X}_{i}}{\sigma } \sim  N\left( {0,1}\right),\;\bar{X} \sim  N\left( {0,\frac{{\sigma }^{2}}{n}}\right)$,

$$
\frac{\left( n - 1\right) }{{\sigma }^{2}}{S}^{2} = \mathop{\sum }\limits_{{i = 1}}^{n}{\left( \frac{{X}_{i} - \bar{X}}{\sigma }\right) }^{2} \sim  {\chi }^{2}\left( {n - 1}\right),
$$

$$
\frac{\sqrt{n}\bar{X}}{\sigma } = \frac{1}{\sqrt{n}}\mathop{\sum }\limits_{{i = 1}}^{n}\frac{{X}_{i}}{\sigma } \sim  N\left( {0,1}\right),
$$

故有 $\frac{1}{n}{\left( \mathop{\sum }\limits_{{i = 1}}^{n}\frac{{X}_{i}}{\sigma }\right) }^{2} \sim  {\chi }^{2}\left( 1\right)$,由 $\bar{X}$ 与 ${S}^{2}$ 独立,所以

$$
n{\left( \frac{\bar{X}}{\sigma }\right) }^{2} + \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} = \frac{1}{n}{\left( \mathop{\sum }\limits_{{i = 1}}^{n}\frac{{X}_{i}}{\sigma }\right) }^{2} + \frac{\left( {n - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( n\right).
$$

因此答案为(D)

【1.38】设 ${X}_{1},{X}_{2},\cdots,{X}_{m}$ 和 ${Y}_{1},{Y}_{2},\cdots,{Y}_{n}$ 分别是从正态总体 $X \sim  N\left( {{\mu }_{1},{\sigma }^{2}}\right)$ 和总体 $Y \sim$ $N\left( {{\mu }_{2},{\sigma }^{2}}\right)$ 中抽取的两个独立样本. $\bar{X}$ 和 $\bar{Y}$ 分别表示 $X$ 和 $Y$ 的样本均值, ${S}_{1}^{2}$ 和 ${S}_{2}^{2}$ 分别表示 $X$ 和 $Y$ 的修正的样本方差, $a$ 和 $b$ 是两个非零实数. 试求

$$
Z = \frac{a\left( {\bar{X} - {\mu }_{1}}\right)  + b\left( {\bar{Y} - {\mu }_{2}}\right) }{\sqrt{\frac{\left( {m - 1}\right) {S}_{1}^{2} + \left( {n - 1}\right) {S}_{2}^{2}}{m + n - 2}}\sqrt{\frac{{a}^{2}}{m} + \frac{{b}^{2}}{n}}}
$$

的概率分布.

证 因为总体 $X \sim  N\left( {{\mu }_{1},{\sigma }^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }^{2}}\right)$,所以

$$
\bar{X} \sim  N\left( {{\mu }_{1},\frac{{\sigma }^{2}}{m}}\right),\;\bar{Y} \sim  N\left( {{\mu }_{2},\frac{{\sigma }^{2}}{n}}\right)
$$

且知 $\bar{X}$ 与 $\bar{Y}$ 相互独立.

又

$$
E\left\lbrack  {a\left( {\bar{X} - {\mu }_{1}}\right)  + b\left( {\bar{Y} - {\mu }_{2}}\right) }\right\rbrack   = 0;
$$

$$
D\left\lbrack  {a\left( {\bar{X} - {\mu }_{1}}\right)  + b\left( {\bar{Y} - {\mu }_{2}}\right) }\right\rbrack   = {a}^{2}D\left( {\bar{X} - {\mu }_{1}}\right)  + {b}^{2}D\left( {\bar{Y} - {\mu }_{2}}\right)
$$

$$
= {a}^{2}\frac{{\sigma }^{2}}{m} + {b}^{2}\frac{{\sigma }^{2}}{n} = \left( {\frac{{a}^{2}}{m} + \frac{{b}^{2}}{n}}\right) {\sigma }^{2}.
$$

因为相互独立的正态随机变量的线性组合仍是正态随机变量, 所以

$$
a\left( {\bar{X} - {\mu }_{1}}\right)  + b\left( {\bar{Y} - {\mu }_{2}}\right)  \sim  N\left\lbrack  {0,\left( {\frac{{a}^{2}}{m} + \frac{{b}^{2}}{n}}\right) {\sigma }^{2}}\right\rbrack ,
$$

于是

$$
\frac{a\left( {\bar{X} - {\mu }_{1}}\right)  + b\left( {\bar{Y} - {\mu }_{2}}\right) }{\sqrt{\frac{{a}^{2}}{m} + \frac{{b}^{2}}{n}}\sigma }\overset{\text{ 记 }}{ = }U \sim  N\left( {0,1}\right).
$$

又知 $\bar{X}$ 与 ${S}_{1}^{2}$ 独立, $\bar{Y}$ 与 ${S}_{2}^{2}$ 独立,且

$$
\frac{\left( {m - 1}\right) {S}_{1}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {m - 1}\right),\;\frac{\left( {n - 1}\right) {S}_{2}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right),
$$

由两个样本 ${X}_{1},{X}_{2},\cdots,{X}_{m}$ 与 ${Y}_{1},{Y}_{2},\cdots,{Y}_{n}$ 相互独立知道 ${S}_{1}^{2}$ 与 ${S}_{2}^{2}$ 相互独立,由 ${\chi }^{2}$ 分布性质可知

$$
\frac{\left( {m - 1}\right) {S}_{1}^{2}}{{\sigma }^{2}} + \frac{\left( {n - 1}\right) {S}_{2}^{2}}{{\sigma }^{2}}\overset{\text{ 记 }}{ = }W \sim  {\chi }^{2}\left( {m + n - 2}\right),
$$

又由上述证明可知 $U$ 与 $W$ 相互独立,由 $t$ 分布的定义可知

$$
\frac{U}{\sqrt{\frac{W}{m + n - 2}}} = \frac{a\left( {\bar{X} - {\mu }_{1}}\right)  + b\left( {\bar{Y} - {\mu }_{2}}\right) }{\sqrt{\frac{\left( {m - 1}\right) {S}_{1}^{2} + \left( {n - 1}\right) {S}_{2}^{2}}{m + n - 2}}\sqrt{\frac{{a}^{2}}{m} + \frac{{b}^{2}}{n}}} \sim  t\left( {m + n - 2}\right).
$$

【1.39】在天平上重复称量一重为 $a$ 的物品,假设各次称量结果相互独立且同服从正态分布 $N\left( {a,{0.2}^{2}}\right)$. 若以 ${\bar{X}}_{n}$ 表示 $n$ 次称量结果的算术平均值,则为使 $P\left\{  {\left| {{\bar{X}}_{n} - a}\right|  < {0.1}}\right\}   \geq  {0.95}, n$ 的最小值应不小于自然数_____.

解 设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 为相互独立的随机变量,且 ${X}_{i} \sim  N\left( {a,{0.2}^{2}}\right)$,则

$$
{\bar{X}}_{n} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} \sim  N\left( {a,\frac{{0.2}^{2}}{n}}\right),
$$

有

$$
U = \frac{{\bar{X}}_{n} - a}{\frac{0.2}{\sqrt{n}}} \sim  N\left( {0,1}\right),\;P\{ \left| U\right|  < {1.96}\}  \geq  {0.95},
$$

于是有

$$
P\left\{  {\left| {{\bar{X}}_{n} - a}\right|  < {0.1}}\right\}   = P\left\{  {\frac{\sqrt{n}\left| {\bar{X} - a}\right| }{0.2} < \frac{\sqrt{n}}{2}}\right\}   \geq  {0.95},
$$

得 $\frac{\sqrt{n}}{2} \geq  {1.96}, n \geq  {15.3664}$. 则有 $n$ 的最小值应不小于 16.

故应填 16.

【1.40】在总体 $N\left( {{52},{6.3}^{2}}\right)$ 中随机抽一容量为 36 的样本,求样本均值 $\bar{X}$ 落在 50.8 到 53. 8 之间的概率.

解 因 $\bar{X} \sim  N\left( {{52},\frac{{6.3}^{2}}{36}}\right)$,所以

$$
P\{ {50.8} < \bar{X} < {53.8}\}  = P\left\{  {\frac{{50.8} - {52}}{\frac{6.3}{6}} < \frac{\bar{X} - {52}}{\frac{6.3}{6}} < \frac{{53.8} - {52}}{\frac{6.3}{6}}}\right\}
$$

$$
= P\left\{  {-\frac{8}{7} < \frac{\bar{X} - {52}}{\frac{6.3}{6}} < \frac{12}{7}}\right\}
$$

$$
= \Phi \left( \frac{12}{7}\right)  - \Phi \left( {-\frac{8}{7}}\right)  = \Phi \left( \frac{12}{7}\right)  + \Phi \left( \frac{8}{7}\right)  - 1
$$

$$
\approx  {0.9564} + {0.8729} - 1
$$

$$
= {0.8293}\text{.}
$$

【1.41】设在总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 中抽取一容量为 16 的样本. 这里 $\mu,{\sigma }^{2}$ 均为未知.

(1)求 $P\left\{  {\frac{{S}^{2}}{{\sigma }^{2}} \leq  {2.041}}\right\}$,其中 ${S}^{2}$ 为样本方差；

(2) 求 $D\left( {S}^{2}\right)$.

解 (1) 由样本来自总体 $N\left( {\mu,{\sigma }^{2}}\right)$ 知, $\frac{\left( {{16} - 1}\right) {S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {{16} - 1}\right)$. 从而

$$
P\left\{  {\frac{{S}^{2}}{{\sigma }^{2}} \leq  {2.041}}\right\}   = P\left\{  {\frac{{15}{S}^{2}}{{\sigma }^{2}} \leq  {15} \times  {2.041}}\right\}
$$

$$
= 1 - P\left\{  {\frac{{15}{S}^{2}}{{\sigma }^{2}} > {30.615}}\right\}   = 1 - P\left\{  {{\chi }^{2}\left( {15}\right)  > {30.615}}\right\}
$$

$$
= 1 - {0.01} = {0.99}\text{.}
$$

(2) 由 $\left( {n - 1}\right) \frac{{S}^{2}}{{\sigma }^{2}} \sim  {\chi }^{2}\left( {n - 1}\right)$,有 $D\left\lbrack  {\left( {n - 1}\right) \frac{{S}^{2}}{{\sigma }^{2}}}\right\rbrack   = 2\left( {n - 1}\right)$,

即 $\frac{{\left( n - 1\right) }^{2}}{{\sigma }^{4}}D\left( {S}^{2}\right)  = 2\left( {n - 1}\right)$,从而 $D\left( {S}^{2}\right)  = \frac{2{\sigma }^{4}}{n - 1}$,

当 $n = {16}$ 时, $D\left( {S}^{2}\right)  = \frac{2}{15}{\sigma }^{4}$.

【1.42】求总体 $N\left( {{20},3}\right)$ 的容量分别为 10,15 的两独立样本均值差的绝对值大于 0.3 的概率.

解 记 $\bar{X} = \frac{1}{10}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i},\bar{Y} = \frac{1}{15}\mathop{\sum }\limits_{{i = 1}}^{{15}}{Y}_{i},\bar{X}$ 与 $\bar{Y}$ 独立,且 $\bar{X} \sim  N\left( {{20},\frac{3}{10}}\right),\bar{Y} \sim  N\left( {{20},\frac{3}{15}}\right)$, 则 $\bar{X} - \bar{Y} \sim  N\left( {0,\frac{1}{2}}\right)$,于是

$$
P\{ \left| {\bar{X} - \bar{Y}}\right|  > {0.3}\}  = \left\{  {\left| \frac{\bar{X} - \bar{Y}}{\frac{1}{\sqrt{2}}}\right|  > {0.3} \times  \sqrt{2}}\right\}
$$

$$
= 2 \times  \left\lbrack  {1 - \Phi \left( {{0.3} \times  \sqrt{2}}\right) }\right\rbrack   \approx  2 \times  \left\lbrack  {1 - \Phi \left( {0.4243}\right) }\right\rbrack
$$

$$
= 2 \times  \left( {1 - {0.6628}}\right)  = {0.6744}.
$$

【1.43】设 ${X}_{1},{X}_{2},\cdots,{X}_{8}$ 为 $N\left( {0,{0.2}^{2}}\right)$ 的一个样本,求 $a$,使 $P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{8}{X}_{i}^{2} < a}\right\}   = {0.95}$.

解 由 ${X}_{1},{X}_{2},\cdots,{X}_{8}$ 独立同服从 $N\left( {0,{0.2}^{2}}\right)$ 分布,知

$$
\mathop{\sum }\limits_{{i = 1}}^{8}{\left( \frac{{X}_{i}}{0.2}\right) }^{2} = \frac{1}{{0.2}^{2}}\mathop{\sum }\limits_{{i = 1}}^{8}{X}_{i}^{2} \sim  {\chi }^{2}\left( 8\right),
$$

因此

$$
P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{8}{X}_{i}^{2} < a}\right\}   = P\left\{  {\frac{1}{{0.2}^{2}}\mathop{\sum }\limits_{{i = 1}}^{8}{X}_{i}^{2} < \frac{a}{{0.2}^{2}}}\right\}
$$

$$
= P\left\{  {{\chi }^{2}\left( 8\right)  < \frac{a}{0.04}}\right\}   = {0.95},
$$

即 $P\left\{  {{\chi }^{2}\left( 8\right)  > \frac{a}{0.04}}\right\}   = {0.05}$,故 $\frac{a}{0.04} = {\chi }_{0.05}^{2}\left( 8\right)  = {15.507}$,

则 $a = {0.04} \times  {15.507} = {0.62028}$.

【1.44】设总体 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$,从两个总体中分别抽样得: ${n}_{1} = 8,{S}_{1}^{2} = 8$. ${75};{n}_{2} = {10},{S}_{2}^{2} = {2.66}$. 求概率 $P\left\{  {{\sigma }_{1}^{2} > {\sigma }_{2}^{2}}\right\}$.

解 因为

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_228_670_696_236_127_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_228_670_696_236_127_0.jpg)

所以

$$
P\left\{  {{\sigma }_{1}^{2} > {\sigma }_{2}^{2}}\right\}   = P\left\{  {\frac{{\sigma }_{2}^{2}}{{\sigma }_{1}^{2}} < 1}\right\}   = P\left\{  {\frac{\frac{{S}_{1}^{2}}{{\sigma }_{1}^{2}}}{\frac{{S}_{2}^{2}}{{\sigma }_{2}^{2}}} < \frac{{S}_{1}^{2}}{{S}_{2}^{2}}}\right\}
$$

$$
= P\left\{  {F\left( {7,9}\right)  < \frac{8.75}{2.66}}\right\}   = P\{ F\left( {7,9}\right)  < {3.829}\}
$$

$$
= 1 - P\{ F\left( {7,9}\right)  \geq  {3.289}\}  = 1 - {0.05} = {0.95}\text{.}
$$

【1.45】设总体 $X$ 服从正态分布 $N\left( {{\mu }_{1},{\sigma }^{2}}\right)$,总体 $Y$ 服从正态分布 $N\left( {{\mu }_{2},{\sigma }^{2}}\right),{X}_{1},{X}_{2},\cdots$, ${X}_{{n}_{1}}$ 和 ${Y}_{1},{Y}_{2},\cdots,{Y}_{{n}_{2}}$ 分别是来自总体 $X$ 和 $Y$ 的简单随机样本,则

$$
E\left\lbrack  \frac{\mathop{\sum }\limits_{{i = 1}}^{{n}_{1}}{\left( {X}_{i} - \bar{X}\right) }^{2} + \mathop{\sum }\limits_{{j = 1}}^{{n}_{2}}{\left( {Y}_{j} - \bar{Y}\right) }^{2}}{{n}_{1} + {n}_{2} - 2}\right\rbrack   =
$$

解 因为 ${S}^{2}$ 是 ${\sigma }^{2}$ 的无偏估计,即 $E\left( {S}^{2}\right)  = {\sigma }^{2}$.

所以

$$
E\left\lbrack  {\frac{1}{{n}_{1} - 1}\mathop{\sum }\limits_{{i = 1}}^{{n}_{1}}{\left( {X}_{i} - \bar{X}\right) }^{2}}\right\rbrack   = {\sigma }^{2},\;E\left\lbrack  {\frac{1}{{n}_{2} - 1}\mathop{\sum }\limits_{{j = 1}}^{{n}_{2}}{\left( {Y}_{j} - \bar{Y}\right) }^{2}}\right\rbrack   = {\sigma }^{2},
$$

则

$$
E\left\lbrack  \frac{\mathop{\sum }\limits_{{i = 1}}^{{n}_{1}}{\left( {X}_{i} - \bar{X}\right) }^{2} + \mathop{\sum }\limits_{{j = 1}}^{{n}_{2}}{\left( {Y}_{j} - \bar{Y}\right) }^{2}}{{n}_{1} + {n}_{2} - 2}\right\rbrack   = {\sigma }^{2}.
$$

故应填 ${\sigma }^{2}$.

【1.46】设总体 $X \sim  N\left( {\mu,{2}^{2}}\right),{X}_{1},{X}_{2},\cdots,{X}_{n}$ 为取自总体的一个样本, $\bar{X}$ 为样本均值,要使 $E{\left( \bar{X} - \mu \right) }^{2} \leq  {0.1}$ 成立,则样本容量 $n$ 至少应取_____.

解 $E{\left( \bar{X} - \mu \right) }^{2} = D\bar{X} = \frac{1}{n}{DX} = \frac{1}{n} \cdot  {2}^{2} \leq  {0.1}$,得 $n \geq  {40}$.

或 $E{\left( \bar{X} - \mu \right) }^{2} = E\left\lbrack  {{\left( \bar{X}\right) }^{2} - {2\mu }\left( \bar{X}\right)  + {\mu }^{2}}\right\rbrack   = E\left\lbrack  {\left( \bar{X}\right) }^{2}\right\rbrack   - {2\mu E}\left( \bar{X}\right)  + E\left( {\mu }^{2}\right)$

$$
= D\left( \bar{X}\right)  + {\left\lbrack  E\left( \bar{X}\right) \right\rbrack  }^{2} - {2\mu EX} + {\mu }^{2} = \frac{DX}{n} + {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} - 2{\mu }^{2} + {\mu }^{2}
$$

$$
= \frac{{2}^{2}}{n} + {\mu }^{2} - 2{\mu }^{2} + {\mu }^{2} = \frac{4}{n} \leq  {0.1}.
$$

故 $n \geq  {40}$.

【1.47】设总体 $X \sim  B\left( {1, p}\right),{X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自 $X$ 的样本.

(1)求 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的分布律；

(2) 求 $\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 的分布律;

(3)求 $E\left( \bar{X}\right), D\left( \bar{X}\right), E\left( {S}^{2}\right)$.

解 (1) $P\left\{  {{X}_{1} = {x}_{1},{X}_{2} = {x}_{2},\cdots,{X}_{n} = {x}_{n}}\right\}$

$= P\left\{  {{X}_{1} = {x}_{1}}\right\}  P\left\{  {{X}_{2} = {x}_{2}}\right\}  \cdots P\left\{  {{X}_{n} = {x}_{n}}\right\}$

$= {p}_{i = 1}^{\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}{\left( 1 - p\right) }^{n - \mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}},\;{x}_{i} = 0,1;i = 1,2,\cdots, n.$

( 2 ) ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 独立同服从 $B\left( {1, p}\right)$,则 $X = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} \sim  B\left( {n, p}\right)$,因此

$$
P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} = k}\right\}   = {C}_{n}^{k}{p}^{k}{\left( 1 - p\right) }^{n - k}\;\left( {k = 0,1,2,\cdots, n}\right).
$$

(3)由于 $\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} \sim  B\left( {n, p}\right)$,所以

$$
E\left( \bar{X}\right)  = E\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{n}E\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{n} \cdot  {np} = p;
$$

$$
D\left( \bar{X}\right)  = D\left( {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{{n}^{2}}D\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{{n}^{2}}{np}\left( {1 - p}\right)  = \frac{p\left( {1 - p}\right) }{n};
$$

$$
E\left( {S}^{2}\right)  = E\left( {\frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2}}\right)  = \frac{1}{n - 1}E\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - n{\bar{X}}^{2}}\right)
$$

$$
= \frac{1}{n - 1}\left( {\mathop{\sum }\limits_{{i = 1}}^{n}E{X}_{i}^{2} - {nE}{\bar{X}}^{2}}\right)
$$

$$
= \frac{1}{n - 1}\left\{  {\mathop{\sum }\limits_{{i = 1}}^{n}\left\lbrack  {D{X}_{i} + {\left( E{X}_{i}\right) }^{2}}\right\rbrack   - n\left\lbrack  {D\bar{X} + {\left( E\bar{X}\right) }^{2}}\right\rbrack  }\right\}
$$

$$
= \frac{n}{n - 1}\left\lbrack  {p\left( {1 - p}\right)  + {p}^{2} - \frac{p\left( {1 - p}\right) }{n} - {p}^{2}}\right\rbrack   = p\left( {1 - p}\right).
$$

【1.48】设总体 $X \sim  {\chi }^{2}\left( n\right),{X}_{1},{X}_{2},\cdots,{X}_{10}$ 是来自 $X$ 的样本,求 $E\left( \bar{X}\right), D\left( \bar{X}\right), E\left( {S}^{2}\right)$.

解 $E{X}_{i} = {EX} = n, D{X}_{i} = {DX} = {2n}$,则

$$
E\left( \bar{X}\right)  = E\left( {\frac{1}{10}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}}\right)  = \frac{1}{10}\mathop{\sum }\limits_{{i = 1}}^{{10}}E{X}_{i} = n.
$$

$$
D\left( \bar{X}\right)  = D\left( {\frac{1}{10}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}}\right)  = \frac{1}{{10}^{2}}\mathop{\sum }\limits_{{i = 1}}^{{10}}D{X}_{i} = \frac{1}{100} \times  {10} \times  {2n} = \frac{n}{5}.
$$

$$
E\left( {S}^{2}\right)  = \frac{1}{{10} - 1}E\left( {\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}^{2} - {10}{\bar{X}}^{2}}\right)  = \frac{1}{9}\left( {\mathop{\sum }\limits_{{i = 1}}^{{10}}E{X}_{i}^{2} - {10E}{\bar{X}}^{2}}\right)
$$

$$
= \frac{1}{9}\left\{  {\mathop{\sum }\limits_{{i = 1}}^{{10}}\left\lbrack  {D{X}_{i} + {\left( E{X}_{i}\right) }^{2}}\right\rbrack   - {10}\left\lbrack  {D\bar{X} + {\left( E\bar{X}\right) }^{2}}\right\rbrack  }\right\}
$$

$$
= \frac{1}{9} \times  \left\lbrack  {{10} \times  \left( {{2n} + {n}^{2}}\right)  - {10} \times  \left( {\frac{n}{5} + {n}^{2}}\right) }\right\rbrack   = {2n}.
$$

点评 上述两题也可直接用公式

$$
E\left( \bar{X}\right)  = {EX},\;D\left( \bar{X}\right)  = \frac{DX}{n},\;E\left( {S}^{2}\right)  = {DX}
$$

进行计算, 简化推导过程.

【1.49】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}\left( {n > 2}\right)$ 为来自总体 $N\left( {0,{\sigma }^{2}}\right)$ 的简单随机样本,其样本均值为 $\bar{X}$. 记 ${Y}_{i} = {X}_{i} - \bar{X}, i = 1,2,\cdots, n$.

(1)求 ${Y}_{i}$ 的方差 $D{Y}_{i}, i = 1,2,\cdots, n$;

(2)求 ${Y}_{1}$ 与 ${Y}_{n}$ 的协方差 $\operatorname{Cov}\left( {{Y}_{1},{Y}_{n}}\right)$;

(3)若 $c{\left( {Y}_{1} + {Y}_{n}\right) }^{2}$ 是 ${\sigma }^{2}$ 的无偏估计量,求常数 $c$.

解 (1) $D{Y}_{i} = D\left( {{X}_{i} - \bar{X}}\right)  = D\left\lbrack  {\left( {1 - \frac{1}{n}}\right) {X}_{i} - \frac{1}{n}\mathop{\sum }\limits_{{k \neq  i}}{X}_{k}}\right\rbrack   = \frac{n - 1}{n}{\sigma }^{2},\;i = 1,2,\cdots, n$.

(2) $\operatorname{Cov}\left( {{Y}_{1},{Y}_{n}}\right)  = E\left( {{Y}_{1} - E{Y}_{1}}\right) \left( {{Y}_{n} - E{Y}_{n}}\right)  = E\left( {{X}_{1} - \bar{X}}\right) \left( {{X}_{n} - \bar{X}}\right)$

$$
= E\left( {{X}_{1}{X}_{n}}\right)  + E\left( {\bar{X}}^{2}\right)  - E\left( {{X}_{1}\bar{X}}\right)  - E\left( {{X}_{n}\bar{X}}\right)
$$

$$
= E{X}_{1}E{X}_{n} + D\bar{X} - \frac{1}{n}E\left( {X}_{1}^{2}\right)  - \frac{1}{n}\mathop{\sum }\limits_{{i = 2}}^{n}E\left( {{X}_{1}{X}_{i}}\right)
$$

$$
- \frac{1}{n}E\left( {X}_{n}^{2}\right)  - \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{{n - 1}}E\left( {{X}_{i}{X}_{n}}\right)
$$

$$
=  - \frac{1}{n}{\sigma }^{2}\text{.}
$$

(3) $E\left\lbrack  {c{\left( {Y}_{1} + {Y}_{n}\right) }^{2}}\right\rbrack   = {cD}\left( {{Y}_{1} + {Y}_{n}}\right)  = c\left\lbrack  {D{Y}_{1} + D{Y}_{n} + 2\operatorname{Cov}\left( {{Y}_{1},{Y}_{n}}\right) }\right\rbrack$

$$
= c\left\lbrack  {\frac{n - 1}{n} + \frac{n - 1}{n} - \frac{2}{n}}\right\rbrack  {\sigma }^{2}
$$

$= \frac{2\left( {n - 2}\right) }{n}c{\sigma }^{2} = {\sigma }^{2}$,(无偏性定义见第七章)

故 $c = \frac{n}{2\left( {n - 2}\right) }$.

点评 本题 (1)、(2) 也可利用性质计算:

$$
D{Y}_{i} = D\left( {{X}_{i} - \bar{X}}\right)  = D\left( {X}_{i}\right)  + D\left( \bar{X}\right)  - 2\operatorname{Cov}\left( {{X}_{i},\bar{X}}\right)
$$

$$
= D\left( {X}_{i}\right)  + \frac{D\left( X\right) }{n} - \frac{2}{n}D\left( {X}_{i}\right)  = \frac{n - 1}{n}{\sigma }^{2}.
$$

$$
\operatorname{Cov}\left( {{Y}_{1},{Y}_{n}}\right)  = \operatorname{Cov}\left( {{X}_{1} - \bar{X},{X}_{n} - \bar{X}}\right)
$$

$$
=  - \operatorname{Cov}\left( {{X}_{1},\bar{X}}\right)  - \operatorname{Cov}\left( {{X}_{n},\bar{X}}\right)  + \operatorname{Cov}\left( {\bar{X},\bar{X}}\right)
$$

$$
=  - \frac{1}{n}D\left( {X}_{1}\right)  - \frac{1}{n}D\left( {X}_{n}\right)  + D\left( \bar{X}\right)
$$

$$
=  - \frac{2}{n}D\left( X\right)  + \frac{1}{n}D\left( X\right)  =  - \frac{1}{n}{\sigma }^{2}.
$$

【1.50】设总体服从泊松分布 $P\left( \lambda \right),{X}_{1},{X}_{2},\cdots,{X}_{n}$ 是一样本.

(1)写出 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 的概率分布.

(2) 计算 $E\left( \bar{X}\right), D\left( \bar{X}\right)$ 和 $E\left( {S}^{2}\right)$.

(3)设总体的容量为 10 的一组样本观察值为 $\left( {1,2,4,3,3,4,5,6,4,8}\right)$,试计算样本均值、样本方差和经验分布函数.

解 (1) 由于 $P\left\{  {{X}_{i} = {x}_{i}}\right\}   = \frac{{\lambda }^{{x}_{i}}}{{x}_{i}!}{\mathrm{e}}^{-\lambda },\;\left( {{x}_{i} = 0,1,2,\cdots }\right) \lambda  > 0$

因此 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的概率分布为

$$
p\left( {{x}_{1},{x}_{2},\cdots,{x}_{n}}\right)  = \mathop{\prod }\limits_{{i = 1}}^{n}\frac{{\lambda }^{{x}_{i}}}{{x}_{i}!}{\mathrm{e}}^{-\lambda } = \frac{{\mathrm{e}}^{-{n\lambda }}{\lambda }_{i}\mathop{\sum }\limits_{{i = 1}}^{n}{x}_{i}}{\mathop{\prod }\limits_{{i = 1}}^{n}{x}_{i}!}.
$$

(2) 由于 $X \sim  P\left( \lambda \right)$,所以 $E\left( X\right)  = D\left( X\right)  = \lambda$,则有

$$
E\left( \bar{X}\right)  = E\left( X\right)  = \lambda,\;D\left( \bar{X}\right)  = \frac{D\left( X\right) }{n} = \frac{\lambda }{n},\;E\left( {S}^{2}\right)  = D\left( X\right)  = \lambda.
$$

(3) $\bar{X} = \frac{1}{10}\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i} = 4$,

$$
{S}^{2} = \frac{1}{n - 1}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( {X}_{i} - \bar{X}\right) }^{2} = \frac{1}{n - 1}\left\lbrack  {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2} - n{\bar{X}}^{2}}\right\rbrack   = 4.
$$

经验分布函数 ${F}_{10}\left( x\right)$ 为

$$
{F}_{10}\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 1 \\  \frac{1}{10}, & 1 \leq  x < 2 \\  \frac{2}{10}, & 2 \leq  x < 3 \\  \frac{4}{10}, & 3 \leq  x < 4 \\  \frac{7}{10}, & 4 \leq  x < 5 \\  \frac{8}{10}, & 5 \leq  x < 6 \\  \frac{9}{10}, & 6 \leq  x < 8 \\  \frac{9}{10}, & 6 \leq  x < 8 \end{array}\right.
$$

【1.51】测得 20 个毛坯重量(单位:g),列成简单表如下

<table><tr><td>毛坯重量</td><td>185</td><td>187</td><td>192</td><td>195</td><td>200</td><td>202</td><td>205</td><td>206</td></tr><tr><td>频数</td><td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>2</td><td>1</td><td>1</td></tr><tr><td>毛坯重量</td><td>207</td><td>208</td><td>210</td><td>214</td><td>215</td><td>216</td><td>218</td><td>220</td></tr><tr><td>频数</td><td>2</td><td>1</td><td>1</td><td>1</td><td>2</td><td>1</td><td>2</td><td>1</td></tr></table>

将其按区间 $\lbrack {183.5},{192.5}),\cdots,\lbrack {219.5},{228.5})$ 分为 5 组,列出分组统计表,并画出频率直方图.

解 分组统计表为

<table><tr><td>分组编号</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td></tr><tr><td rowspan="2">组 限</td><td>183.5</td><td>192.5</td><td>201.5</td><td>210.5</td><td>219.5</td></tr><tr><td>192.5</td><td>201.5</td><td>210.5</td><td>219.5</td><td>228.5</td></tr><tr><td>组中值</td><td>188</td><td>197</td><td>206</td><td>215</td><td>224</td></tr><tr><td>组频数</td><td>3</td><td>2</td><td>8</td><td>6</td><td>1</td></tr><tr><td>组频率(%)</td><td>15</td><td>10</td><td>40</td><td>30</td><td>5</td></tr></table>

频率直方图如图 6-1.51 所示.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_232_583_544_387_296_0.jpg](reference/attach/images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_232_583_544_387_296_0.jpg)

图 6-1.51

【1.52】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体 $X$ 的样本,总体 $X$ 的分布函数为 $F\left( x\right)$,密度函数为 $f\left( x\right)$,记 $Y = \max \left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right),\;Z = \min \left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$, 试求 $Y, Z$ 的密度函数及 $\left( {Y, Z}\right)$ 的联合密度函数.

解 因为 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 独立同分布,且 ${X}_{i}$ 分布函数为 $F\left( x\right)$,则由第三章公式可得:

$$
{F}_{Y}\left( y\right)  = {\left\lbrack  F\left( y\right) \right\rbrack  }^{n},\;{F}_{Z}\left( z\right)  = 1 - {\left\lbrack  1 - F\left( z\right) \right\rbrack  }^{n},
$$

故 ${f}_{Y}\left( y\right)  = {F}_{Y}^{\prime }\left( y\right)  = n{F}^{n - 1}\left( y\right) f\left( y\right)$,

${f}_{Z}\left( z\right)  = {F}_{Z}^{\prime }\left( z\right)  = n{\left\lbrack  1 - F\left( z\right) \right\rbrack  }^{n - 1}f\left( z\right).$

设 $\left( {Y, Z}\right)$ 的联合分布函数为 $G\left( {y, z}\right), G\left( {y, z}\right)  = P\{ Y \leq  y, Z \leq  z\}$,

当 $y < z$ 时, $G\left( {y, z}\right)  = P\{ Y \leq  y\}  = {F}_{Y}\left( y\right)  = {\left\lbrack  F\left( y\right) \right\rbrack  }^{n}$,

当 $y \geq  z$ 时, $G\left( {y, z}\right)  = P\{ Y \leq  y, Z \leq  z\}  = P\{ Y \leq  y\}  - P\{ Y \leq  y, Z > z\}$

$= P\{ Y \leq  y\}  - P\left\{  {\max \left( {X}_{i}\right)  \leq  y,\min \left( {X}_{i}\right)  > z}\right\}$

$= P\left\{  {Y \leq  y}\right\}   - P\left\{  {z < {X}_{1} \leq  y, z < {X}_{2} \leq  y,\cdots, z < {X}_{n} \leq  y}\right\}$

$= P\{ Y \leq  y\}  - {\left\lbrack  P\left\{  z < {X}_{i} \leq  y\right\}  \right\rbrack  }^{n}$

$= {\left\lbrack  F\left( y\right) \right\rbrack  }^{n} - {\left\lbrack  F\left( y\right)  - F\left( z\right) \right\rbrack  }^{n},$

即 $G\left( {y, z}\right)  = \left\{  \begin{matrix} {\left\lbrack  F\left( y\right) \right\rbrack  }^{n}, & y < z \\  {\left\lbrack  F\left( y\right) \right\rbrack  }^{n} - {\left\lbrack  F\left( y\right)  - F\left( z\right) \right\rbrack  }^{n}, & y \geq  z \end{matrix}\right.$

故 $\left( {Y, Z}\right)$ 的联合密度为

$$
g\left( {y, z}\right)  = \frac{{\partial }^{2}G}{\partial y\partial z} = \left\{  \begin{array}{ll} n\left( {n - 1}\right) f\left( y\right) f\left( z\right) {\left\lbrack  F\left( y\right)  - F\left( z\right) \right\rbrack  }^{n - 2}, & y \geq  z \\  0, & y < z \end{array}\right.
$$

第七章 参数估计

§ 1. 点 估 计

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