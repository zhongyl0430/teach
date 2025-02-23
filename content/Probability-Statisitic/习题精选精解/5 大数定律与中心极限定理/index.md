### 知识要点

#### 1. 切比雪夫不等式

假设随机变量 $X$ 具有数学期望 ${EX}$ 及方差 ${DX}$,则对任意的 $\varepsilon  > 0$,有

$$
P\{ \left| {X - {EX}}\right|  \geq  \varepsilon \}  \leq  \frac{DX}{{\varepsilon }^{2}}.
$$

或者有时候也可以写成

$$
P\{ \left| {X - {EX}}\right|  < \varepsilon \}  \geq  1 - \frac{DX}{{\varepsilon }^{2}}.
$$

#### 2. 大数定律

(1)切比雪夫大数定律

如果随机变量序列 $\left\{  {X}_{n}\right\}$ 相互独立,各随机变量的期望和方差都有限,而且方差有公共上界,即 $D{X}_{i} \leq  l, i = 1,2,\cdots$,其中 $l$ 是与 $i$ 无关的常数,则对任意的 $\varepsilon  > 0$,有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\left| {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E{X}_{i}}\right|  < \varepsilon }\right\}   = 1.
$$

切比雪夫大数定律的特例: 设随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n},\cdots$ 相互独立,且 $E\left( {X}_{i}\right)  = \mu, D\left( {X}_{i}\right)  = {\sigma }^{2}$ $\left( {i = 1,2,\cdots }\right)$,则对任意的 $\varepsilon  > 0$,总有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\left| {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \mu }\right|  < \varepsilon }\right\}   = 1.
$$

该定律说明: 在定律的条件下,当 $n$ 充分大时, $n$ 个独立随机变量的平均数的离散程度很小.

(2)伯努利大数定律

如果 ${u}_{n}$ 是 $n$ 次重复独立试验中事件 $A$ 发生的次数, $p$ 是事件 $A$ 在每次试验中发生的概率,则对任意给定的 $\varepsilon  > 0$,有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\left| {\frac{{u}_{n}}{n} - p}\right|  < \varepsilon }\right\}   = 1.
$$

该定律说明: 在试验条件不改变的情况下, 将试验重复进行多次, 则随机事件的频率在它发生的概率附近摆动.

(3)辛钦大数定律

如果 $\left\{  {X}_{n}\right\}$ 是相互独立同分布的随机变量序列,其数学期望 $E{X}_{i} = \mu, i = 1,2,\cdots$,则对任意给定的 $\varepsilon  > 0$,有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\left| {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \mu }\right|  < \varepsilon }\right\}   = 1.
$$

该定律说明: 对独立同分布的随机变量序列, 只要验证数学期望是否存在, 就可判定其是否服从大数定律.

#### 3. 中心极限定理

(1)列维一林德伯格定理(独立同分布的中心极限定理)

设随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n},\cdots$ 独立同分布,且 $E\left( {X}_{i}\right)  = \mu, D\left( {X}_{i}\right)  = {\sigma }^{2} <  + \infty \left( {i = 1,2,\cdots }\right)$,则对任意实数 $x$,有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - {n\mu }}{\sqrt{n}\sigma } \leq  x}\right\}   = {\int }_{-\infty }^{x}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{t}^{2}}{2}}\mathrm{\;d}t = \Phi \left( x\right).
$$

(2)李雅普诺夫定理

若随机变量序列 $\left\{  {X}_{n}\right\}$ 相互独立,每个随机变量有期望值 $E{X}_{n} = {\mu }_{n}$ 及方差 $D{X}_{n} = {\sigma }_{n}^{2} <  + \infty, n =$ $1,2,\cdots$,若每个 ${X}_{n}$ 对总和 $\mathop{\sum }\limits_{{n = 1}}^{m}{X}_{n}$ 影响不大,记 ${S}_{m} = {\left( \mathop{\sum }\limits_{{n = 1}}^{m}{\sigma }_{n}^{2}\right) }^{\frac{1}{2}}$,则

$$
\mathop{\lim }\limits_{{m \rightarrow  \infty }}P\left\{  {\frac{1}{{S}_{m}}\mathop{\sum }\limits_{{n = 1}}^{m}\left( {{X}_{n} - {\mu }_{n}}\right)  \leq  x}\right\}   = \frac{1}{\sqrt{2\pi }}{\int }_{-\infty }^{x}{\mathrm{e}}^{-\frac{{t}^{2}}{2}}\mathrm{\;d}t = \Phi \left( x\right).
$$

(3)棣莫弗一拉普拉斯定理

设随机变量 ${Y}_{1},{Y}_{2},\cdots$ 服从参数为 $n, p$ 的二项分布,则对于任何实数 $x$,有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{{Y}_{n} - {np}}{\sqrt{npq}} \leq  x}\right\}   = {\int }_{-\infty }^{x}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{\frac{{t}^{2}}{2}}\mathrm{\;d}t = \Phi \left( x\right).
$$

其中 $q = 1 - p$.

### 基本题型

#### 题型 1. 利用切比雪夫不等式估计概率

【1.1】设随机变量 $X$ 的数学期望 ${EX} = \mu$,方差 ${DX} = {\sigma }^{2}$,则由切比雪夫不等式,有 $P\{ \left| {X - \mu }\right|  \geq  {3\sigma }\}  \leq$ _____.

解 由切比雪夫不等式

$$
P\left\{  {\left| {X - \mu }\right|  \geq  {3\sigma }}\right\}   \leq  \frac{DX}{{\left( 3\sigma \right) }^{2}} = \frac{{\sigma }^{2}}{9{\sigma }^{2}} = \frac{1}{9}.
$$

点评 此类题型的求解方法比较单一,在随机变量 $X$ 的期望 ${EX}$ 和方差 ${DX}$ 已知的情况下,直接应用切比雪夫不等式即可; 若 ${EX}$ 和 ${DX}$ 未知,当根据题意并结合数学期望和方差的性质计算出 ${EX}$ 和 ${DX}$,然后再套用切比雪夫不等式.

【1.2】设随机变量 $X$ 的方差为 2,则根据切比雪夫不等式估计 $P\{ \left| {X - E\left( X\right) }\right|  \geq  2\}  \leq$ _____.

解 根据切比雪夫不等式有

$$
P\{ \left| {X - E\left( X\right) }\right|  \geq  2\}  \leq  \frac{D\left( X\right) }{{2}^{2}} = \frac{2}{4} = \frac{1}{2}.
$$

【1.3】设随机变量 $X$ 和 $Y$ 的数学期望分别为 -2 和 2,方差分别为 1 和 4,而相关系数为 -0.5,则根据切比雪夫不等式 $P\{ \left| {X + Y}\right|  \geq  6\}  \leq$ _____.

解 根据期望和方差的性质

$$
E\left( {X + Y}\right)  = {EX} + {EY} =  - 2 + 2 = 0,
$$

$D\left( {X + Y}\right)  = {DX} + {DY} + 2\operatorname{Cov}\left( {X, Y}\right)  = {DX} + {DY} + 2{\rho }_{XY}\sqrt{DX}\sqrt{DY}$

$$
= 1 + 4 + 2 \times  \left( {-{0.5}}\right)  \times  \sqrt{1} \times  \sqrt{4} = 3.
$$

那么 $P\{ \left| {X + Y}\right|  \geq  6\}  \leq  \frac{D\left( {X + Y}\right) }{{6}^{2}} = \frac{3}{{6}^{2}} = \frac{1}{12}$.

【1.4】已知正常男性成人血液中,每一毫升白细胞数平均是 7300,均方差是 700,利用切比雪夫不等式估计每毫升含白细胞数在 ${5200} \sim  {9400}$ 之间的概率 $p$.

解 假设正常男性成人血液中每毫升白细胞数为 $X$,依题设 $E\left( X\right)  = {7300}, D\left( X\right)  = {700}^{2}$,于是

$$
P\{ {5200} < X < {9400}\}  = P\{ \left| {X - {7300}}\right|  < {2100}\}  \geq  1 - \frac{{700}^{2}}{{2100}^{2}} = \frac{8}{9},
$$

即每毫升含白细胞数在 5200 ~ 9400 之间的概率不低于 $\frac{8}{9}$.

【1.5】设随机变量 $X \sim  B\left( {n, p}\right)$,试用切比雪夫不等式证明

$$
P\left\{  {\left| {X - {np}}\right|  \geq  \sqrt{n}}\right\}   \leq  \frac{1}{4}.
$$

证 $E\left( X\right)  = {np}, D\left( X\right)  = {np}\left( {1 - p}\right)$,由切比雪夫不等式,

$$
P\left\{  {\left| {X - {EX}}\right|  \geq  \sqrt{n}}\right\}   \leq  \frac{DX}{{\left( \sqrt{n}\right) }^{2}},
$$

即

$$
P\left\{  {\left| {X - {np}}\right|  \geq  \sqrt{n}}\right\}   \leq  p\left( {1 - p}\right)  \leq  \frac{1}{4},
$$

其中最后的不等式来自二次函数的极值.

#### 题型 2. 关于大数定律

【1.6】设总体 $X$ 服从参数为 2 的指数分布, ${X}_{1}$, ${X}_{2}$, $\cdots$, ${X}_{n}$ 为来自总体的简单随机样本,则当 $n \rightarrow$ $\infty$ 时, ${Y}_{n} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 依概率收敛于_____.

解 因为 ${X}_{i} \sim  E\left( 2\right)$,所以 $E\left( {X}_{i}\right)  = \frac{1}{2}, D\left( {X}_{i}\right)  = \frac{1}{4}$.

由已知 ${X}_{1}^{2},{X}_{2}^{2},\cdots,{X}_{n}^{2}$ 独立同分布,且

$$
E\left( {X}_{i}^{2}\right)  = D{X}_{i} + {\left( E{X}_{i}\right) }^{2} = \frac{1}{4} + \frac{1}{4} = \frac{1}{2},
$$

由大数定律得: ${Y}_{n} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 依概率收敛于 $\frac{1}{2}$.

故应填 $\frac{1}{2}$.

【1.7】设随机变量 ${X}_{1},\cdots,{X}_{n},\cdots$ 是独立同分布的随机变量,其分布函数为 $F\left( x\right)  = A +$ $\frac{1}{\pi }\arctan \frac{x}{B}$,其中 $B \neq  0$,则辛钦大数定律对此序列(   ).

(A) 适用 (B) 当常数 $A$ 、 $B$ 取适当数值时适用

(C) 无法判断 (D) 不适用

分析 辛钦大数定律成立的条件有两条: (1) 随机变量序列 $\left\{  {X}_{n}\right\}$ 独立同分布; (2) 数学期望 $E{X}_{n}$, $n = 1,2,\cdots$ 存在.

判断随机变量序列是否服从辛钦大数定律, 只要验证上述两个条件即可.

解 根据题意,只需判断 $E\left( {X}_{n}\right)$ 是否存在,即广义积分 ${\int }_{-\infty }^{+\infty }\left| {x\frac{\mathrm{d}F\left( x\right) }{\mathrm{d}x}}\right| \mathrm{d}x$ 是否收敛即可.

因为 $f\left( x\right)  = \frac{\mathrm{d}F\left( x\right) }{\mathrm{d}x} = \frac{B}{\pi \left( {{B}^{2} + {x}^{2}}\right) }$,那么

$$
{\int }_{-\infty }^{+\infty }\left| {x\frac{\mathrm{d}F\left( x\right) }{\mathrm{d}x}}\right| \mathrm{d}x = {\int }_{-\infty }^{+\infty }\frac{\left| B\right| \left| x\right| }{\pi \left( {{B}^{2} + {x}^{2}}\right) }\mathrm{d}x = \frac{2\left| B\right| }{\pi }{\int }_{0}^{+\infty }\frac{x}{{B}^{2} + {x}^{2}}\mathrm{\;d}x
$$

$$
= \frac{\left| B\right| }{\pi }{\int }_{0}^{+\infty }\frac{\mathrm{d}\left( {{B}^{2} + {x}^{2}}\right) }{{B}^{2} + {x}^{2}} = \frac{\left| B\right| }{\pi }\mathop{\lim }\limits_{{a \rightarrow   + \infty }}{\int }_{0}^{a}\frac{\mathrm{d}\left( {{B}^{2} + {x}^{2}}\right) }{{B}^{2} + {x}^{2}}
$$

$$
= \frac{\left| B\right| }{\pi }\mathop{\lim }\limits_{{a \rightarrow   + \infty }}\ln \left( {1 + \frac{{a}^{2}}{{B}^{2}}}\right)  =  + \infty.
$$

即辛钦大数定律不满足.

故应选(D).

#### 题型 3. 与中心极限定理条件及结论有关的题目

【1.8】设随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 相互独立, ${S}_{n} = {X}_{1} + {X}_{2} + \cdots  + {X}_{n}$,则根据列维一林德伯格 (Levy-Lindberg) 中心极限定理,当 $n$ 充分大时, ${S}_{n}$ 近似服从正态分布,只要 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ (   ).

(A) 有相同的数学期望 (B) 有相同的方差

(C) 服从同一指数分布 (D) 服从同一离散型分布

分析 列维一林德伯格定理成立的条件有三条: (1) 随机变量序列 $\left\{  {X}_{n}\right\}$ 相互独立; (2) 各随机变量服从同一分布; (3) 各随机变量的数学期望和方差存在.

要判定当 $n$ 充分大时, ${S}_{n} = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 是否近似服从正态分布,只需验证随机变量序列 $\left\{  {X}_{n}\right\}$ 是否满足上述三个条件即可.

解 根据题意知,选项(A)、(B) 不能保证 ${X}_{1},\cdots,{X}_{n},\cdots$ 同分布; 选项(D) 不能保证数学期望存在.

因此应选(C).

【1.9】设 ${X}_{1},{X}_{2},\cdots,{X}_{n},\cdots$ 为独立同分布的随机变量序列,且均服从参数为 $\lambda \left( {\lambda  > 1}\right)$ 的指数分布,记 $\Phi \left( x\right)$ 为标准正态分布函数,则 (   ).

(A) $\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - {n\lambda }}{\lambda \sqrt{n}} \leq  x}\right\}   = \Phi \left( x\right)$ (B) $\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - {n\lambda }}{\sqrt{n\lambda }} \leq  x}\right\}   = \Phi \left( x\right)$

(C) $\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{\lambda \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - n}{\sqrt{n}} \leq  x}\right\}   = \Phi \left( x\right)$ (D) $\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \lambda }{\sqrt{n\lambda }} \leq  x}\right\}   = \Phi \left( x\right)$

解 根据题意知, 该随机变量序列满足列维一林德伯格中心极限定理. 因为

$$
E\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}E{X}_{i} = \frac{n}{\lambda },\;D\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}D{X}_{i} = \frac{n}{{\lambda }^{2}},
$$

所以

$$
\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \frac{n}{\lambda }}{\sqrt{\frac{n}{{\lambda }^{2}}}} = \frac{\lambda \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - n}{\sqrt{n}}
$$

的极限分布为标准正态分布.

故应选(C).

【1.10】假设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是来自总体 $X$ 的简单随机样本; 已知 $E{X}^{k} = {a}_{k}\left( {k = 1,2,3,4}\right)$,并且 ${a}_{4}$ $- {a}_{2}^{2} > 0$. 证明当 $n$ 充分大时,随机变量 ${Z}_{n} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 近似服从正态分布,并指出其分布参数.

证 根据简单随机样本的特性, ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 独立同分布,那么 ${X}_{1}^{2},{X}_{2}^{2},\cdots,{X}_{n}^{2}$ 也独立同分布. 由 $E{X}^{k} = {a}_{k}, k = 1,2,3,4$,有

$$
E{Z}_{n} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}E{X}_{i}^{2} = {a}_{2},
$$

并且也有

$$
D{Z}_{n} = \frac{1}{{n}^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}D{X}_{i}^{2} = \frac{1}{{n}^{2}}\mathop{\sum }\limits_{{i = 1}}^{n}\left\lbrack  {E{X}_{i}^{4} - {\left( E{X}_{i}^{2}\right) }^{2}}\right\rbrack   = \frac{1}{n}\left( {{a}_{4} - {a}_{2}^{2}}\right)  > 0.
$$

所以根据中心极限定理 $\frac{{Z}_{n} - {a}_{2}}{\sqrt{\frac{{a}_{4} - {a}_{2}^{2}}{n}}}$ 的极限分布为标准正态分布,即 ${Z}_{n} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}^{2}$ 近似服从正态

分布 $\left( {n\text{充分大时}}\right)$,其分布参数为 $\left( {{a}_{2},\frac{{a}_{4} - {a}_{2}^{2}}{n}}\right)$.

#### 题型 4. 利用中心极限定理求概率

方法与技巧 中心极限定理常用来解决概率的近似计算问题, 使用方法如下:

(1)列维一林德伯格定理用于随机变量之和或均值的概率的近似计算.

列维一林德伯格中心极限定理表明,当 $n$ 充分大时,相互独立服从同一分布且存在有限期望与方差的随机变量之和近似服从正态分布, 该定理实质上提供了计算独立同分布的随机变量之和的概率的近似方法,若 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 独立同分布且 $E{X}_{i} = \mu, D{X}_{i} = {\sigma }^{2}, i = 1,2,\cdots, n$,则 ${S}_{n} = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 近似服从 $N\left( {{n\mu }, n{\sigma }^{2}}\right)$,因此当 $n$ 比较大时,求 $P\left\{  {a \leq  {S}_{n} \leq  b}\right\}$ 需首先将 ${S}_{n}$ 标准化,也就是说

$$
P\left\{  {a \leq  {S}_{n} \leq  b}\right\}   = \left\{  {\frac{a - {n\mu }}{\sigma \sqrt{n}} \leq  \frac{{S}_{n} - {n\mu }}{\sigma \sqrt{n}} \leq  \frac{b - {n\mu }}{\sigma \sqrt{n}}}\right\}   \approx  \Phi \left( \frac{b - {n\mu }}{\sigma \sqrt{n}}\right)  - \Phi \left( \frac{a - {n\mu }}{\sigma \sqrt{n}}\right),
$$

其中 $\Phi \left( x\right)$ 是标准正态分布函数.

定理的另一种形式为: 当 $n$ 充分大时, $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 近似服从 $N\left( {\mu,\frac{{\sigma }^{2}}{n}}\right)$,该形式可近似计算关于均值的概率.

(2)棣莫弗一拉普拉斯定理用于二项分布的近似计算. 定理表明:设 $X \sim  B\left( {n, p}\right)$,则当 $n$ 充分大时, $X$ 近似服从 $N\left( {{np},{np}\left( {1 - p}\right) }\right)$.

【1.11】一生产线生产的产品成箱包装,每箱的重量是随机的,假设每箱平均重 50 千克,标准差为 5 千克,若用最大载重量为 5 吨的汽车承运,试利用中心极限定理说明每辆车最多可以装多少箱,才能保障不超载的概率大于 0.977. ( $\Phi \left( 2\right)  = {0.977}$,其中的 $\Phi \left( x\right)$ 是标准正态分布函数).

解 设 ${X}_{i} =$ “装运的第 $i$ 箱的重量(单位:千克)”, $i = 1,2,\cdots, n$. $n$ 为箱数. 根据题意, ${X}_{1},{X}_{2},\cdots$, ${X}_{n}$ 独立同分布,而 $n$ 箱的总重量可记为 ${U}_{n} = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$. 因为 $E{X}_{i} = {50},\sqrt{D{X}_{i}} = 5$,所以

$$
E{U}_{n} = \mathop{\sum }\limits_{{i = 1}}^{n}E{X}_{i} = {50n},\;\sqrt{D{U}_{n}} = \sqrt{\mathop{\sum }\limits_{{i = 1}}^{n}D{X}_{i}} = 5\sqrt{n},
$$

那么由列维一林德伯格中心极限定理知, ${U}_{n}$ 近似服从于 $N\left( {{50n},{25n}}\right)$. 而所求的箱数 $n$ 取决于条件

$$
P\left\{  {{U}_{n} \leq  {5000}}\right\}   = P\left\{  {\frac{{U}_{n} - {50n}}{5\sqrt{n}} \leq  \frac{{5000} - {50n}}{5\sqrt{n}}}\right\}   \approx  \Phi \left( \frac{{1000} - {10n}}{\sqrt{n}}\right)  > {0.977} = \Phi \left( 2\right).
$$

所以 $\frac{{1000} - {10n}}{\sqrt{n}} > 2$,即 $n < {98.0199}$. 亦即每辆车最多可以装 98 箱.

【1.12】某单位设置一电话总机,共有 200 个电话分机,设每个电话分机有 5% 的时间要使用外线通话, 假设每个分机是否使用外线通话是相互独立的. 问总机要多少外线才能以 90% 的概率保证每个分机要使用外线时可供使用.

解 设同时使用外线的分机的台数为 $X$,则 $X \sim  B\left( {n, p}\right)$,其中 $n = {200}, p = {0.05},{np} = {10}$, $\sqrt{{np}\left( {1 - p}\right) } = {3.08}.$

又设该单位安装 $N$ 条外线,依题意,求 $P\{ X \leq  N\}  \geq  {0.9}$ 的最小 $N$,由棣莫弗一拉普拉斯中心极限定理

$$
P\{ X \leq  N\}  = P\left\{  {\frac{X - {np}}{\sqrt{{np}\left( {1 - p}\right) }} \leq  \frac{N - {np}}{\sqrt{{np}\left( {1 - p}\right) }}}\right\}   \approx  \Phi \left( \frac{N - {10}}{3.08}\right).
$$

查标准正态分布表,可知 $\Phi \left( {1.28}\right)  = {0.9}$,故 $N$ 应满足

$$
\frac{N - {10}}{3.08} \geq  {1.28}\text{ 即 }N \geq  {10} + {1.28} \times  {3.08} = {13.94}.
$$

取 $N = {14}$,即至少要安装 14 条外线.

【1.13】测量某物体的长度时, 由于存在测量误差, 每次测得的长度只能是近似值. 现进行多次测量,然后取这些测量值的平均值作为实际长度的估计值,假定 $n$ 个测量值 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是独立同分布的随机变量,具有共同的期望 $\mu$ (即实际长度) 及方差 $\sigma  = 1$,试问要以 95% 的把握可以确信其估计值精确到 $\pm  {0.2}$ 以内,必须测量多少次?

解 考虑用中心极限定理来估计, 则有

$$
P\left\{  {\left| {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \mu }\right|  \leq  {0.2}}\right\}   = P\left\{  {\left| \frac{\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - \mu }{\frac{\sigma }{\sqrt{n}}}\right|  \leq  \frac{{0.2}\sqrt{n}}{\sigma }}\right\}   \approx  {2\Phi }\left( \frac{{0.2}\sqrt{n}}{\sigma }\right)  - 1
$$

$$
= {2\Phi }\left( {{0.2}\sqrt{n}}\right)  - 1\;\left( {\text{ 由 }\sigma  = 1}\right)
$$

要求 ${2\Phi }\left( {{0.2}\sqrt{n}}\right)  - 1 = {0.95\Phi }\left( {{0.2}\sqrt{n}}\right)  = {0.975}$

所以 ${0.2}\sqrt{n} = {1.96}$,

解得 $n \geq  {96.04}$.

需要测量 97 次以上,以 95% 的把握确信估计值与真值之差的绝对值不超过 0.2.

#### 题型 5. 综合提高题型

【1.14】设 ${X}_{1},{X}_{2},\cdots,{X}_{n},\cdots$ 是独立同分布的随机变量序列,且

<table><tr><td>${X}_{i}$</td><td/><td/><td rowspan="2"/></tr><tr><td>$P$</td><td/><td/></tr></table>

令 ${Y}_{n} = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}, n = 1,2,\cdots,\Phi \left( x\right)$ 为标准正态分布函数,则 $\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{{Y}_{n} - {np}}{\sqrt{{np}\left( {1 - p}\right) }} \leq  1}\right\}   =$ (   ).

(A) 0 (B) $\Phi \left( 1\right)$ (C) $1 - \Phi \left( 1\right)$ (D) 1

解 由中心极限定理

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{{Y}_{n} - {np}}{\sqrt{{np}\left( {1 - p}\right) }} \leq  x}\right\}   = \Phi \left( x\right), x\text{为任意实数}
$$

则

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{{Y}_{n} - {np}}{\sqrt{{np}\left( {1 - p}\right) }} \leq  1}\right\}   = \Phi \left( 1\right).
$$

故应选(B).

【1.15】设随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n},\cdots$ 相互独立,且 ${X}_{i}$ 都服从参数为 $\frac{1}{2}$ 的指数分布,则当 $n$ 充分大时,随机变量 ${Z}_{n} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 的概率分布近似服从 (   ).

(A) $N\left( {2,4}\right)$ (B) $N\left( {2,\frac{4}{n}}\right)$ (C) $N\left( {\frac{1}{2},\frac{1}{4n}}\right)$ (D) $N\left( {{2n},{4n}}\right)$

解 因为 ${X}_{i} \sim  E\left( \frac{1}{2}\right)$,所以 $E{X}_{i} = 2, D{X}_{i} = 4$.

由中心极限定理, $\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 近似服从 $N\left( {{2n},{4n}}\right)$,或者 $\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$ 近似服从 $N\left( {2,\frac{4}{n}}\right)$ (当 $n$ 充分大时).

故应选(B).

【1.16】设 $\Phi \left( x\right)$ 为标准正态分布函数,

$$
{X}_{i} = \left\{  {\begin{array}{ll} 0, & A\text{ 不发生 } \\  1, & A\text{ 发生 } \end{array}\;\left( {i = 1,2,\cdots,{100}}\right),}\right.
$$

且 $P\left( A\right)  = {0.8},{X}_{1},{X}_{2},\cdots,{X}_{100}$ 相互独立. 令 $Y = \mathop{\sum }\limits_{{i = 1}}^{{100}}{X}_{i}$,则由中心极限定理知 $Y$ 的分布函数 $F\left( y\right)$ 近似于(   ).

(A) $\Phi \left( y\right)$ (B) $\Phi \left( \frac{y - {80}}{4}\right)$ (C) $\Phi \left( {{16y} + 8}\right)$ (D) $\Phi \left( {{4y} + {80}}\right)$

解 由题意 $Y$ 服从二项分布 $B\left( {{100},{0.8}}\right)$,

$$
{EY} = {80},\;{DY} = {16},
$$

故由中心极限定理可知,当 $n$ 充分大时, $Y$ 近似服从正态分布 $N\left( {{80},{16}}\right)$,

则 $Y$ 的分布函数 $F\left( y\right)  \approx  \Phi \left( \frac{y - {80}}{4}\right)$ (当 $n$ 充分大时).

故应选(B).

【1.17】假设随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n},\cdots$ 独立同分布,且 $E{X}_{n} = 0$,则 $\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} < n}\right\}   =$ (   ).

(A) 0 (B) $\frac{1}{4}$ (C) $\frac{1}{2}$ (D) 1

解 由此题条件及所求概率,考虑用辛钦大数定律:

对 $\forall \varepsilon  > 0,\;\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\left| {\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - E{X}_{n}}\right|  < \varepsilon }\right\}   = 1$.

因为 $E{X}_{n} = 0$,取 $\varepsilon  = 1$,则

$\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\left| {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right|  < n}\right\}   = 1$. 又 $\left\{  {\left| {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right|  < n}\right\}   \subset  \left\{  {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} < n}\right\} ,$

所以 $\mathop{\lim }\limits_{{n \rightarrow  \infty }}\left\{  {\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} < n}\right\}   = 1$.

故应选(D).

【1.18】设随机变量 $X$ 的概率密度为 $f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{2}{x}^{2}{\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\right.$,试用切比雪夫不等式估计概率 $P\{ 1 < X < 5\}  >$ _____.

解 ${EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = 3$,

${DX} = E\left( {X}^{2}\right)  - {\left( EX\right) }^{2} = {\int }_{-\infty }^{+\infty }{x}^{2}f\left( x\right) \mathrm{d}x - 9 = 3.$

则 $P\{ 1 < X < 5\}  = P\{ \left| {X - 3}\right|  < 2\}  > 1 - \frac{DX}{{2}^{2}} = 1 - \frac{3}{4} = \frac{1}{4}$.

故应填 $\frac{1}{4}$.

【1. 19】设 $X \sim  U\left\lbrack  {-1, b}\right\rbrack$,若由切比雪夫不等式有 $P\{ \left| {X - 1}\right|  < \varepsilon \}  \geq  \frac{2}{3}$,则 $b =$ _____； $\varepsilon  =$ _____.

解 因为 ${EX} = \frac{b - 1}{2},{DX} = \frac{{\left( b + 1\right) }^{2}}{12}$,所以 $\frac{b - 1}{2} = 1,1 - \frac{\frac{{\left( b + 1\right) }^{2}}{12}}{{\varepsilon }^{2}} = \frac{2}{3}$,

则 $b = 3,\varepsilon  = 2$.

【1.20】在每次试验中事件 $A$ 发生的概率等于 0.5,利用切比雪夫不等式,则在 1000 次独立试验中事件 $A$ 发生的次数在 450 至 550 之间的概率为_____.

解 设随机变量 $X$ 表示事件 $A$ 在 1000 次试验中发生的次数,则 $X$ 服从二项分布 $B\left( {{1000},{0.5}}\right)$, 易知

$$
E\left( X\right)  = {np} = {1000} \times  {0.5} = {500}.
$$

$$
D\left( X\right)  = {np}\left( {1 - p}\right)  = {1000} \times  {0.5} \times  {0.5} = {250}.
$$

因为 $P\{ {450} \leq  X \leq  {550}\}  = P\{ \left| {X - {500}}\right|  \leq  {50}\}$,由切比雪夫不等式

$$
P\{ \left| {X - E\left( X\right) }\right|  < \varepsilon \}  \geq  1 - \frac{D\left( X\right) }{{\varepsilon }^{2}},
$$

所以 $P\{ \left| {X - {500}}\right|  \leq  {50}\}  \geq  1 - \frac{250}{{50}^{2}} = {0.9}$,即

$$
P\{ {450} \leq  X \leq  {550}\}  \geq  {0.9}.
$$

故应填 0.9.

【1.21】设 ${X}_{1},{X}_{2},\cdots,{X}_{n},\cdots$ 为相互独立的随机变量序列,且 ${X}_{i}\left( {i = 1,2,\cdots }\right)$ 服从参数为 $\lambda$ 的泊

松分布,则 $\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - {n\lambda }}{\sqrt{n\lambda }} \leq  x}\right\}   =$ _____.

解 $E\left( {X}_{i}\right)  = \lambda, D\left( {X}_{i}\right)  = \lambda$,代入独立同分布的中心极限定理,即得

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}P\left\{  {\frac{\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i} - {n\lambda }}{\sqrt{n\lambda }} \leq  x}\right\}   = {\int }_{-\infty }^{x}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{t}^{2}}{2}}\mathrm{\;d}t\text{ 或 }\Phi \left( x\right).
$$

【1.22】一加法器同时收到 20 个噪声电压 ${V}_{i}\left( {i = 1,\cdots,{20}}\right)$. 设它们相互独立且都服从 $\left( {0,{10}}\right)$ 上的均匀分布,则 $P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{{20}}{V}_{i} > {105}}\right\}   =$ _____.

解 因为 $E{V}_{i} = 5, D{V}_{i} = \frac{100}{12}$,由中心极限定理可知 $\mathop{\sum }\limits_{{i = 1}}^{{20}}{V}_{i}$ 近似服从 $N\left( {{100},\frac{500}{3}}\right)$,所以

$$
P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{{20}}{V}_{i} > {105}}\right\}   \approx  1 - \Phi \left\lbrack  \frac{{105} - {100}}{\sqrt{\frac{500}{3}}}\right\rbrack   = 1 - \Phi \left( {0.39}\right)  = {0.3483}.
$$

【1.23】某市有 50 个无线寻呼台,每个寻呼台在每分钟内收到的电话呼叫次数服从参数 $\lambda  = {0.05}$ 的泊松分布,则该市在某时刻一分钟内的呼叫次数的总和大于 3 次的概率是_____.

解 设第 $i$ 个寻呼台在给定时刻一分钟内收到的呼叫次数为 ${X}_{i}\left( {i = 1,2,\cdots,{50}}\right)$,则该市在此时刻一分钟内收到的呼叫总数为 $S = \mathop{\sum }\limits_{{i = 1}}^{{50}}{X}_{i}$,且

$$
E\left( {X}_{i}\right)  = \lambda  = {0.05}
$$

$$
D\left( {X}_{i}\right)  = \lambda  = {0.05}
$$

所以, 根据独立同分布中心极限定理, 有

$S$ 近似服从 $N\left( {{50} \times  {0.05},{50} \times  {0.05}}\right)  = N\left( {{2.5},{2.5}}\right)$

于是,所求概率为

$$
P\{ S > 3\}  = 1 - P\{ S \leq  3\}  \approx  1 - \Phi \left( \frac{3 - {2.5}}{\sqrt{2.5}}\right)  = 1 - \Phi \left( {0.3162}\right)  = {0.3745}.
$$

【1.24】在一家保险公司里有 10000 人参加保险, 每人每年付 12 元保险费. 在一年内一个人死亡的概率为 0.006, 死亡后家属可向保险公司领取 1000 元. 试求:(1) 保险公司亏本的概率；(2) 保险公司一年的利润不少于 60000 元的概率.

解 (1)设参加保险的 10000 人中一年死亡的人数为 $X$,则有 $X \sim  B\left( {{10000},{0.006}}\right),{EX} = {60}$, ${DX} \approx  {7.72}^{2}$

公司一年收保险费 120000 元,付给死者家属 1000X 元. 当 1000X-120000 > 0 时,即 X> 120 时公司就亏本了. 所以亏本的概率为:

$$
P\{ X > {120}\}  = 1 - P\{ X \leq  {120}\}.
$$

由中心极限定理, $X$ 近似服从 $N\left( {{60},{7.72}^{2}}\right)$. 于是

$$
P\{ X > {120}\}  = 1 - P\left\{  {\frac{X - {60}}{7.72} \leq  \frac{{120} - {60}}{7.72}}\right\}   = 1 - P\left\{  {\frac{X - {60}}{7.72} \leq  {7.77}}\right\}
$$

$$
\approx  1 - \Phi \left( {7.77}\right)  \approx  1 - 1 = 0.
$$

电 198

(2)公司年利润不少于 60000 元就是 120000 -1000X $\geq$ 60000,即 0 $\leq  X \leq$ 60,其概率为

$$
P\{ 0 \leq  X \leq  {60}\}  = P\left\{  {\frac{0 - {60}}{7.72} \leq  \frac{X - {60}}{7.72} \leq  \frac{{60} - {60}}{7.72}}\right\}   = P\left\{  {-{7.77} \leq  \frac{X - {60}}{7.72} \leq  0}\right\}
$$

$$
\approx  \Phi \left( 0\right)  - \Phi \left( {-{7.77}}\right)  \approx  {0.5} - 0 = {0.5}\text{.}
$$

【1.25】现有一大批种子,其中良种占 $\frac{1}{6}$,现从中任取 6000 粒. 试分别 (1) 用切比雪夫不等式估计; (2) 用中心极限定理计算: 这 6000 粒中良种所占的比例与 $\frac{1}{6}$ 之差的绝对值不超过 0.01 的概率.

解 设 6000 粒中的良种数量为 $X$,则 $X \sim  B\left( {{6000},\frac{1}{6}}\right)$.

(1)要估计的概率为

$$
P\left\{  {\left| {\frac{X}{6000} - \frac{1}{6}}\right|  < \frac{1}{100}}\right\}   = P\{ \left| {X - {1000}}\right|  < {60}\}
$$

相当于在切比雪夫不等式中取 $\varepsilon  = {60}$,于是由切比雪夫不等式可得

$$
P\left\{  {\left| {\frac{X}{6000} - \frac{1}{6}}\right|  < \frac{1}{100}}\right\}   = P\{ \left| {X - {1000}}\right|  < {60}\}
$$

$$
\geq  1 - \frac{D\left( X\right) }{{60}^{2}} = 1 - \frac{5}{6} \times  {1000} \times  \frac{1}{3600}
$$

$$
= 1 - {0.2315} = {0.7685}\text{,}
$$

即用切比雪夫不等式估计此概率值不小于 0.7685.

( 2 )由拉普拉斯中心极限定理,二项分布 $B\left( {{6000},\frac{1}{6}}\right)$ 可用正态分布 $N\left( {{1000},\frac{5}{6} \times  {1000}}\right)$ 近似, 于是, 所求概率为

$$
P\left\{  {\left| {\frac{X}{6000} - \frac{1}{6}}\right|  < \frac{1}{100}}\right\}   = P\{ \left| {X - {1000}}\right|  < {60}\}  = P\left\{  {\left| \frac{X - {1000}}{\sqrt{\frac{5}{6} \times  {1000}}}\right|  < \frac{60}{\sqrt{\frac{5}{6} \times  {1000}}}}\right\}
$$

$$
\approx  {2\Phi }\left( {2.0784}\right)  - 1 = 2 \times  {0.98124} - 1 \approx  {0.9625}.
$$

比较两个结果, 用切比雪夫不等式估计是比较粗略的.

【1.26】据以往经验, 某种电气元件的寿命服从均值为 100 小时的指数分布, 现随机地取 16 只,设它们的寿命是相互独立的,求这 16 只元件的寿命的总和大于 1920 小时的概率.

解 记 16 只电气元件的寿命分别为 ${X}_{1},{X}_{2},\cdots,{X}_{16}$,则这 16 只元件的寿命之和为 $\mathop{\sum }\limits_{{i = 1}}^{{16}}{X}_{i}$, 依题意, $E\left( {X}_{i}\right)  = {100}, D\left( {X}_{i}\right)  = {100}^{2}$,根据独立同分布的中心极限定理

$$
Z = \frac{\mathop{\sum }\limits_{{i = 1}}^{{16}}{X}_{i} - {16} \times  {100}}{4 \times  {100}} = \frac{X - {1600}}{400}
$$

近似地服从 $N\left( {0,1}\right)$,于是

$$
P\{ X > {1920}\}  = 1 - P\{ X \leq  {1920}\}  = 1 - P\left\{  {\frac{X - {1600}}{400} \leq  \frac{{1920} - {1600}}{400}}\right\}
$$

$$
\approx  1 - \Phi \left( {0.8}\right)  = {0.2119}.
$$

【1.27】某保险公司多年的统计资料表明,在索赔户中被盗索赔户占 20%,以 $X$ 表示在随意抽查的 100 个索赔户中因被盗向保险公司索赔的户数.

(1)写出 $X$ 的概率分布；

(2)利用棣莫弗一拉普拉斯定理,求被盗索赔户不少于 14 户且不多于 30 户的概率的近似值.

附表: 设 $\Phi \left( x\right)$ 是标准正态分布函数

<table><tr><td>$x$</td><td>0</td><td>0.5</td><td>1.0</td><td>1.5</td><td>2.0</td><td>2.5</td><td>3.0</td></tr><tr><td>$\Phi \left( x\right)$</td><td>0.500</td><td>0.692</td><td>0.841</td><td>0.933</td><td>0.977</td><td>0.944</td><td>0.999</td></tr></table>

解 (1) $X$ 服从二项分布,参数 $n = {100}, p = {0.2}$,

$$
P\{ X = k\}  = {C}_{100}^{k}{0.2}^{k}{0.8}^{{100} - k}\;\left( {k = 0,1,\cdots,{100}}\right);
$$

(2) $E\left( X\right)  = {np} = {20}, D\left( X\right)  = {np}\left( {1 - p}\right)  = {16}$.

根据棣莫弗一拉普拉斯定理

$$
P\{ {14} \leq  X \leq  {30}\}  = P\left\{  {\frac{{14} - {20}}{\sqrt{16}} \leq  \frac{X - {20}}{\sqrt{16}} \leq  \frac{{30} - {20}}{\sqrt{16}}}\right\}   = P\left\{  {-{1.5} \leq  \frac{X - {20}}{4} \leq  {2.5}}\right\}
$$

$$
\approx  \Phi \left( {2.5}\right)  - \Phi \left( {-{1.5}}\right)  = \Phi \left( {2.5}\right)  - \left\lbrack  {1 - \Phi \left( {1.5}\right) }\right\rbrack
$$

$$
= {0.994} - \left( {1 - {0.933}}\right)  = {0.927}\text{.}
$$

【1.28】一部件包括 10 部分,每部分的长度是一个随机变量,它们相互独立,且服从同一分布,其数学期望为2mm,均方差为0.05mm,规定总长度为 $\left( {{20} \pm  {0.1}}\right) \mathrm{{mm}}$ 时产品合格,试求产品合格的概率.

解 设 ${X}_{i}$ 表示该部件第 $i$ 部分的长度 $\left( {i = 1,2,\cdots,{10}}\right)$,由题意知 $E{X}_{i} = 2, D{X}_{i} = {0.05}^{2}$, ${X}_{1},{X}_{2},\cdots,{X}_{10}$ 独立同分布,由中心极限定理知, $\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i}$ 近似服从 $N\left( {{10} \times  2,{10} \times  {0.05}^{2}}\right)$ 分布.

$$
P\left\{  {{19.9} < \mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i} < {20.1}}\right\}   = P\left\{  {\frac{{19.9} - {10} \times  2}{\sqrt{10} \times  {0.05}} < \frac{\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i} - {10} \times  2}{\sqrt{10} \times  {0.05}} < \frac{{20.1} - {10} \times  2}{\sqrt{10} \times  {0.05}}}\right\}
$$

$$
= P\left\{  {-{0.6325} < \frac{\mathop{\sum }\limits_{{i = 1}}^{{10}}{X}_{i} - {20}}{\sqrt{10} \times  {0.05}} < {0.6325}}\right\}
$$

$$
\approx  \Phi \left( {0.6235}\right)  - \Phi \left( {-{0.6235}}\right)  = {2\Phi }\left( {0.6235}\right)  - 1
$$

$$
\approx  2 \times  {0.7357} - 1 = {0.4714}.
$$

【1.29】计算器在进行加法时,将每个加数舍入最靠近它的整数. 设所有舍入误差是独立的且在 $\left( {-{0.5},{0.5}}\right)$ 上服从均匀分布. (1) 若将 1500 个数相加,问误差总和的绝对值超过 15 的概率是多少? (2) 最多可有几个数相加使得误差总和的绝对值小于 10 的概率不少于 0.90?

解 设每个加数的舍入误差为 ${X}_{i}\left( {i = 1,2,\cdots,{1500}}\right)$,由题设知 ${X}_{i}$ 独立同分布,且在 $\left( {-{0.5},{0.5}}\right)$ 上服从均匀分布,从而

$$
E\left( {X}_{i}\right)  = \frac{-{0.5} + {0.5}}{2} = 0,\;D\left( {X}_{i}\right)  = \frac{{\left( {0.5} + {0.5}\right) }^{2}}{12} = \frac{1}{12}.
$$

( 1 )设 $X = \mathop{\sum }\limits_{{i = 1}}^{{1500}}{X}_{i}$,由独立同分布的中心极限定理有 $\frac{X - {1500} \times  0}{\sqrt{1500} \times  \sqrt{\frac{1}{12}}}$ 近似地服从 $N\left( {0,1}\right)$,

从而

$$
P\{ \left| X\right|  > {15}\}  = 1 - P\{ \left| X\right|  \leq  {15}\}  = 1 - P\left\{  {-\frac{15}{\sqrt{125}} \leq  \frac{X}{\sqrt{125}} \leq  \frac{15}{\sqrt{125}}}\right\}
$$

$$
\approx  2 - {2\Phi }\left( {1.34}\right)  = {0.1802}.
$$

即误差总和的绝对值超过 15 的概率约为 0.1802.

(2)记 $Y = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$,要使 $P\{ \left| Y\right|  < {10}\}  \geq  {0.90}$. 由独立同分布的中心极限定理,近似地有

$$
P\{ \left| Y\right|  < {10}\}  = P\{  - {10} < Y < {10}\}
$$

$$
= P\left\{  {\frac{-{10}}{\sqrt{\frac{n}{12}}} < \frac{Y}{\sqrt{\frac{n}{12}}} < \frac{10}{\sqrt{\frac{n}{12}}}}\right\}   \approx  {2\Phi }\left( \frac{10}{\sqrt{\frac{n}{12}}}\right)  - 1 \geq  {0.90}
$$

即 $\Phi \left( \frac{10}{\sqrt{\frac{n}{12}}}\right)  \geq  {0.95}$,查表得 $\frac{10}{\sqrt{\frac{n}{12}}} \geq  {1.645}$,

故 $n \leq  {443}$. 即最多有 443 个数相加使得误差总和的绝对值小于 10 的概率不少于 0.90.

【1.30】有一批建筑房屋用的木柱,其中 ${80}\%$ 的长度不小于 $3\mathrm{\;m}$,现在这批木柱中随机地取出 100 根,问其中至少有 30 根短于 $3\mathrm{\;m}$ 的概率是多少?

解 记 $X$ 为 100 根木柱中长度小于 $3\mathrm{\;m}$ 的木柱根数,则 $X \sim  B\left( {{100},{0.2}}\right)$. 由棣莫弗一拉普拉斯中心极限定理知

$$
P\{ X \geq  {30}\}  = 1 - P\{ X < {30}\}  = 1 - P\left\{  {\frac{X - {100} \times  {0.2}}{\sqrt{{100} \times  {0.2} \times  {0.8}}} < \frac{{30} - {100} \times  {0.2}}{\sqrt{{100} \times  {0.2} \times  {0.8}}}}\right\}
$$

$$
= 1 - \Phi \left( \frac{{30} - {20}}{4}\right)  = 1 - \Phi \left( {2.5}\right)  = 1 - {0.9938} = {0.0062}.
$$

【1.31】一公寓有 200 户住户,一户住户拥有汽车辆数 $X$ 的分布律为

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td></tr><tr><td>${p}_{k}$</td><td>0.1</td><td>0.6</td><td>0.3</td></tr></table>

问需要多少车位, 才能使每辆汽车都具有一个车位的概率至少为 0.95.

解 设需要车位数为 $n$,且设第 $i\left( {i = 1,2,\cdots,{200}}\right)$ 户有车辆数为 ${X}_{i}$,则由 ${X}_{i}$ 的分布律知

$$
E\left( {X}_{i}\right)  = 0 \times  {0.1} + 1 \times  {0.6} + 2 \times  {0.3} = {1.2},
$$

$$
E\left( {X}_{i}^{2}\right)  = {0}^{2} \times  {0.1} + {1}^{2} \times  {0.6} + {2}^{2} \times  {0.3} = {1.8},
$$

故

$$
D\left( {X}_{i}\right)  = E\left( {X}_{i}^{2}\right)  - {\left\lbrack  E\left( {X}_{i}\right) \right\rbrack  }^{2} = {1.8} - {1.2}^{2} = {0.36}.
$$

因共有 200 户, 各户占有车位数相互独立. 从而近似地有

$$
\mathop{\sum }\limits_{{i = 1}}^{{200}}{X}_{i} \sim  N\left( {{200} \times  {1.2},{200} \times  {0.36}}\right).
$$

今要求车位数 $n$ 满足

$$
{0.95} \leq  P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{{200}}{X}_{i} \leq  n}\right\} ,
$$

由正态近似知,上式中 $n$ 应满足

$$
{0.95} \leq  \Phi \left( \frac{n - {200} \times  {1.2}}{\sqrt{{200} \times  {0.36}}}\right)  = \Phi \left( \frac{n - {240}}{\sqrt{72}}\right),
$$

因 ${0.95} = \Phi \left( {1.645}\right)$,从而由 $\Phi \left( x\right)$ 的单调性知 $\frac{n - {240}}{\sqrt{72}} \geq  {1.645}$,故

$$
n \geq  {240} + {1.645} \times  \sqrt{72} = {253.96}.
$$

由此知至少需 254 个车位.

【1.32】某种小汽车氧化氮的排放量的数学期望为 ${0.9}\mathrm{\;g}/\mathrm{{km}}$,标准差为 ${1.9}\mathrm{\;g}/\mathrm{{km}}$,某公司有这种汽车 100 辆,以 $\bar{X}$ 表示这些车辆的氧化氮排放量的算数平均,问当 $L$ 何值时, $\bar{X} > L$ 的概率不超过 0.01.

解 设以 ${X}_{i}\left( {i = 1,2,\cdots,{100}}\right)$ 表示第 $i$ 辆小汽车氧化氮的排放量,则

$$
\bar{X} = \frac{1}{100}\mathop{\sum }\limits_{{i = 1}}^{{100}}{X}_{i}
$$

由已知条件 $E\left( {X}_{i}\right)  = {0.9}, D\left( {X}_{i}\right)  = {1.9}^{2}$ 得

$$
E\left( \bar{X}\right)  = {0.9},\;D\left( \bar{X}\right)  = \frac{{1.9}^{2}}{100}.
$$

各辆汽车氧化氮的排放量相互独立, 故可认为近似地有

$$
\bar{X} \sim  N\left( {{0.9},\frac{{1.9}^{2}}{100}}\right).
$$

需要计算的是满足 $P\{ \bar{X} > L\}  \leq  {0.01}$ 的最小值 $L$.

由中心极限定理

$$
P\{ \bar{X} > L\}  = P\left\{  {\frac{\bar{X} - {0.9}}{0.19} > \frac{L - {0.9}}{0.19}}\right\}   \leq  {0.01}.
$$

$L$ 应为满足 $1 - \Phi \left( \frac{L - {0.9}}{0.19}\right)  \leq  {0.01}$ 的最小值,即

$$
\Phi \left( \frac{L - {0.9}}{0.19}\right)  \geq  {0.99} = \Phi \left( {2.33}\right),\text{ 即 }\frac{L - {0.9}}{0.19} \geq  {2.33},
$$

故 $L \geq  {0.9} + {0.19} \times  {2.33} = {1.3427}$,应取 $L = {1.3427}\mathrm{\;g}/\mathrm{{km}}$.

【1.33】随机地选取两组学生,每组 80 人,分别在两个实验室里测量某种化合物的 $\mathrm{{pH}}$ 值. 各人测量的结果是随机变量, 它们相互独立, 且服从同一分布, 其数学期望为 5, 方差为 0.3, 以 $\overline{X},\overline{Y}$ 分别表示第一组和第二组所得结果的算数平均:

(1) 求 $P\{ {4.9} < \bar{X} < {5.1}\}$;

(2) 求 $P\{  - {0.1} < \bar{X} - \bar{Y} < {0.1}\}$.

解 (1)令 ${X}_{i}$ 表示第一组第 $i$ 人测量结果,则 $E{X}_{i} = 5, D{X}_{i} = {0.3},\left( {i = 1,2,\cdots,{80}}\right)$. 由中心极限定理

$$
P\{ {4.9} < \bar{X} < {5.1}\}  = \left\{  {\frac{{4.9} - 5}{\sqrt{\frac{0.3}{80}}} < \frac{\bar{X} - 5}{\sqrt{\frac{0.3}{80}}} < \frac{{5.1} - 5}{\sqrt{\frac{0.3}{80}}}}\right\}   \approx  \Phi \left( \frac{4}{\sqrt{6}}\right)  - \Phi \left( {-\frac{4}{\sqrt{6}}}\right)
$$

$$
= {2\Phi }\left( {1.63}\right)  - 1 = {0.8968}.
$$

(2)令 ${Y}_{j}$ 表示第二组第 $j$ 人测量结果,则 $E{Y}_{j} = 5, D{Y}_{j} = {0.3}\;\left( {j = 1,2,\cdots,{80}}\right)$

$$
E\bar{X} = E\bar{Y} = 5,\;D\bar{X} = D\bar{Y} = \frac{0.3}{80} = \frac{3}{800},
$$

$$
E\left( {\bar{X} - \bar{Y}}\right)  = 0,\;D\left( {\bar{X} - \bar{Y}}\right)  = D\bar{X} + D\bar{Y} = \frac{3}{400},
$$

$$
P\{  - {0.1} < \bar{X} - \bar{Y} < {0.1}\}  = P\left\{  {\frac{-{0.1}}{\sqrt{\frac{3}{400}}} < \frac{\bar{X} - \bar{Y}}{\sqrt{\frac{3}{400}}} < \frac{0.1}{\sqrt{\frac{3}{400}}}}\right\}   \approx  \Phi \left( \frac{2}{\sqrt{3}}\right)  - \Phi \left( {-\frac{2}{\sqrt{3}}}\right)
$$

$$
= {2\Phi }\left( {1.16}\right)  - 1 = {0.754}\text{.}
$$

【1.34】某种电子器件的寿命(小时)具有数学期望 $\mu$ (未知),方差 ${\sigma }^{2} = {400}$. 为了估计 $\mu$,随机地取 $n$ 只这种器件,在时刻 $t = 0$ 投入测试 (设测试是相互独立的) 直至失效,测得其寿命为 ${X}_{1},{X}_{2},\cdots,{X}_{n}$,以 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{k = 1}}^{n}{X}_{k}$ 作为 $\mu$ 的估计. 为了使 $P\{ \left| {\bar{X} - \mu }\right|  < 1\}  \geq  {0.95}$,问 $n$ 至少为多少?

解 ${X}_{k}$ 表示第 $k$ 个器件寿命, $k = 1,2,\cdots, n$,

$$
E{X}_{k} = \mu,\;D{X}_{k} = {400},\;E\bar{X} = \mu,\;D\bar{X} = \frac{D{X}_{k}}{n} = \frac{400}{n},
$$

$$
P\{ \left| {\bar{X} - \mu }\right|  < 1\}  = P\left\{  {\left| \frac{\bar{X} - \mu }{\sqrt{\frac{400}{n}}}\right|  < \frac{1}{\sqrt{\frac{400}{n}}}}\right\}   = \Phi \left( \frac{\sqrt{n}}{20}\right)  - \Phi \left( {-\frac{\sqrt{n}}{20}}\right)
$$

$$
= {2\Phi }\left( \frac{\sqrt{n}}{20}\right)  - 1 \geq  {0.95}\text{.}
$$

故 $\Phi \left( \frac{\sqrt{n}}{20}\right)  \geq  {0.975} = \Phi \left( {1.96}\right)$. 有 $\frac{\sqrt{n}}{20} \geq  {1.96}$,得 $n \geq  {1536.64}$.

因此 $n$ 至少为 1537.

【1.35】一工人修理一台机器需两个阶段,第一阶段所需时间(小时)服从均值为 0.2 的指数分布, 第二阶段服从均值为 0.3 的指数分布, 且与第一阶段独立. 现有 20 台机器需要修理. 求他在 8 小时内完成的概率.

解 设修理第 $i$ 台机器 $\left( {i = 1,2,\cdots,{20}}\right)$ 第一阶段耗时 ${X}_{i}$,第二阶段耗时 ${Y}_{i}$,则共耗时 ${Z}_{i} =$ ${X}_{i} + {Y}_{i}$.

由已知 $E\left( {X}_{i}\right)  = {0.2}, E\left( {Y}_{i}\right)  = {0.3}$,故

$$
E\left( {Z}_{i}\right)  = E\left( {X}_{i}\right)  + E\left( {Y}_{i}\right)  = {0.5},
$$

$$
D\left( {Z}_{i}\right)  = D\left( {X}_{i}\right)  + D\left( {Y}_{i}\right)  = {0.2}^{2} + {0.3}^{2} = {0.13}.
$$

由中心极限定理, 20 台机器需要修理的时间近似服从正态分布, 即

$$
\mathop{\sum }\limits_{{i = 1}}^{{20}}{Z}_{i}\text{ 近似 }N\left( {{20} \times  {0.5},{20} \times  {0.13}}\right)  = N\left( {{10},{2.6}}\right),
$$

所以概率为

$$
P\left\{  {\mathop{\sum }\limits_{{i = 1}}^{{20}}{Z}_{i} \leq  8}\right\}   \approx  \Phi \left( \frac{8 - {10}}{\sqrt{2.6}}\right)  = \Phi \left( {-{1.24}}\right)  = {0.1075}.
$$

【1.36】某药厂断言,该厂生产的某种药品对于医治一种血液病的治愈率为 0.8,医院任意抽查 100 个服用此药品的病人,若其中多于 75 人治愈,就接受此断言,否则就拒绝此断言.

(1)若实际上此药品对该病治愈率是 0.8,求接受此断言的概率；

(2)若实际上此药品对该病治愈率是 0.7,求接受此断言的概率。

解 设 100 人中的治愈人数为 $X$,则 $X \sim  B\left( {{100}, p}\right)$.

(1) $p = {0.8}$,即 $X \sim  B\left( {{100},{0.8}}\right)$.

由中心极限定理, $X$ 近似服从 $N\left( {{80},{4}^{2}}\right)$.

则接受药厂断言的概率为

$$
P\{ X > {75}\}  = 1 - P\{ X \leq  {75}\}  \approx  1 - \Phi \left( \frac{{75} - {80}}{4}\right)
$$

$$
= 1 - \Phi \left( {-\frac{5}{4}}\right)  = \Phi \left( {1.25}\right)  = {0.8944}.
$$

(2) $p = {0.7}$,即 $X \sim  B\left( {{100},{0.7}}\right)$.

由中心极限定理, $X$ 近似服从 $N\left( {{70},{21}}\right)$.

则接受药厂断言的概率为

$$
P\{ X > {75}\}  = 1 - P\{ X \leq  {75}\}  \approx  1 - \Phi \left( \frac{{75} - {70}}{\sqrt{21}}\right)
$$

$$
= 1 - \Phi \left( {1.09}\right)  = 1 - {0.8621} = {0.1379}\text{.}
$$