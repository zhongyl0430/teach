## § 1. 数学期望

### 知识要点

#### 1. 离散型随机变量的数学期望

设随机变量 $X$ 的分布律为 $P\left\{  {X = {x}_{k}}\right\}   = {p}_{k}\;\left( {k = 1,2,3,\cdots }\right)$

若级数 $\mathop{\sum }\limits_{k}{x}_{k}{p}_{k}$ 绝对收敛,则称它的和为 $X$ 的数学期望,记作 ${EX}$,即 ${EX} = \mathop{\sum }\limits_{k}{x}_{k}{p}_{k}$.

#### 2. 连续型随机变量的数学期望

设随机变量 $X$ 的概率密度为 $f\left( x\right)$,若积分 ${\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x$ 绝对收敛,则称其值为 $X$ 的数学期望,记作 ${EX}$,则 ${EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x$.

#### 3. 离散型随机变量函数的数学期望

( 1 )一维随机变量函数的期望 设 $X$ 的分布律为 $P\left\{  {X = {x}_{k}}\right\}   = {p}_{k}$,又 $Y = g\left( X\right)$,则 ${EY} = \mathop{\sum }\limits_{k}g\left( {x}_{k}\right) {p}_{k};$

(2)二维随机变量函数的期望 设 $\left( {X, Y}\right)$ 的联合分布律为 $P\left\{  {X = {x}_{i}, Y = {y}_{j}}\right\}   = {p}_{ij}$,又 $Z$ $= g\left( {X, Y}\right)$,则 ${EZ} = \mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}g\left( {{x}_{i},{y}_{j}}\right) {p}_{ij}$.

#### 4. 连续型随机变量函数的数学期望

( 1 )一维随机变量函数的数学期望 设连续型随机变量 $X$ 的概率密度为 $f\left( x\right)$,又 $Y =$ $g\left( X\right)$,则 ${EY} = {\int }_{-\infty }^{+\infty }g\left( x\right)  \cdot  f\left( x\right) \mathrm{d}x$;

(2)二维随机变量函数的数学期望 设连续型二维随机变量 $\left( {X, Y}\right)$ 的联合概率密度为 $f\left( {x, y}\right)$,又 $Z = g\left( {X, Y}\right)$,则 ${EZ} = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }g\left( {x, y}\right)  \cdot  f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y$.

#### 5. 数学期望的性质

(1) $E\left( c\right)  = c$ ( $c$ 为任意常数)

(2) $E\left( {cX}\right)  = {cEX}$ ( $c$ 为任意常数)

(3) $E\left( {X + Y}\right)  = {EX} + {EY}$

(4)若 $X$ 与 $Y$ 相互独立,则有 $E\left( {XY}\right)  = {EX} \cdot  {EY}$

(5) ${\left\lbrack  E\left( XY\right) \right\rbrack  }^{2} \leq  E\left( {X}^{2}\right)  \cdot  E\left( {Y}^{2}\right)$

### 基本题型

#### 题型 1. 求离散型随机变量的数学期望

【1.1】一批零件中有 9 个合格品及 3 个废品, 从中每次任取一个, 如果是废品不再放回, 求取得合格品以前已取出的废品数的数学期望.

解 设废品数为 $X$,可求出 $X$ 的分布律为:

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>$\frac{9}{12}$</td><td>$\frac{9}{44}$</td><td>$\frac{9}{220}$</td><td>$\frac{1}{220}$</td></tr></table>

则 $E\left( X\right)  = \mathop{\sum }\limits_{i}{x}_{i}{p}_{i} = 0 \times  \frac{9}{12} + 1 \times  \frac{9}{44} + 2 \times  \frac{9}{220} + 3 \times  \frac{1}{220} = {0.3}$.

【1.2】设离散型随机变量 $X$ 的分布律为: $P\left\{  {X = {2}^{k}}\right\}   = \frac{2}{{3}^{k}}, k = 1,2,\cdots$,则 $E\left( X\right)  =$ _____.

解 $E\left( X\right)  = \sum {x}_{k}{p}_{k} = \mathop{\sum }\limits_{{k = 1}}^{\infty }{2}^{k} \cdot  \frac{2}{{3}^{k}} = 2\mathop{\sum }\limits_{{k = 1}}^{\infty }{\left( \frac{2}{3}\right) }^{k} = \frac{2 \times  \frac{2}{3}}{1 - \frac{2}{3}} = 4$.

【1.3】设随机变量 $X$ 的分布律为 $P\left\{  {X = {\left( -1\right) }^{k}k}\right\}   = \frac{1}{k\left( {k + 1}\right) }\left( {k = 1,2,\cdots }\right)$. 求 $X$ 的数学期望.

分析 离散型随机变量期望存在的条件是级数绝对收敛.

解 因为 $\mathop{\sum }\limits_{{k = 1}}^{\infty }\left| {{x}_{k}{p}_{k}}\right|  = \mathop{\sum }\limits_{{k = 1}}^{\infty }\left| {{\left( -1\right) }^{k}k \cdot  \frac{1}{k\left( {k + 1}\right) }}\right|  = \mathop{\sum }\limits_{{k = 1}}^{\infty }\frac{1}{k + 1}$.

考察级数 $\mathop{\sum }\limits_{{k = 1}}^{\infty }\frac{1}{k + 1}$,由高等数学级数敛散性知识可知此级数是发散的.

所以级数 $\mathop{\sum }\limits_{{k = 1}}^{\infty }{x}_{k}{p}_{k}$ 不绝对收敛,故 $X$ 的数学期望不存在.

#### 题型 2. 求连续型随机变量的数学期望

【1.4】设在某一规定的时间间隔里,某电气设备用于最大负荷的时间 $X$ (以分计) 是一个随机变量, 其概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{{\left( {1500}\right) }^{2}}x, & 0 \leq  x \leq  {1500} \\  \frac{-1}{{\left( {1500}\right) }^{2}}\left( {x - {3000}}\right), & {1500} < x \leq  {3000} \\  0, & \text{ 其他 } \end{array}\right.
$$

求 $E\left( X\right)$.

解 $E\left( X\right)  = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = {\int }_{0}^{1500}\frac{{x}^{2}}{{\left( {1500}\right) }^{2}}\mathrm{\;d}x + {\int }_{1500}^{3000}\frac{-x}{{\left( {1500}\right) }^{2}}\left( {x - {3000}}\right) \mathrm{d}x = {1500}$ (分).

【1.5】设随机变量 $X$ 的分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 1 - \frac{4}{{x}^{2}}, & x \geq  2 \\  0, & x < 2 \end{array}\right.
$$

求 $X$ 的期望.

解 因为 $X$ 的概率密度为

$$
f\left( x\right)  = {F}^{\prime }\left( x\right)  = \left\{  \begin{array}{ll} \frac{8}{{x}^{3}}, & x \geq  2 \\  0, & x < 2 \end{array}\right.
$$

所以 $E\left( X\right)  = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = {\int }_{2}^{+\infty }\frac{8}{{x}^{2}}\mathrm{\;d}x = 4$.

【1.6】设 $f\left( x\right)$ 为随机变量 $X$ 的密度函数,若对于常数 $c$,有

$$
f\left( {c + x}\right)  = f\left( {c - x}\right),\;x > 0
$$

且 ${EX}$ 存在,试证明 ${EX} = c$.

证 由数学期望的定义知

$$
{EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x\frac{x = c + t}{}{\int }_{-\infty }^{+\infty }\left( {c + t}\right) f\left( {c + t}\right) \mathrm{d}t
$$

$$
= {\int }_{-\infty }^{+\infty }{cf}\left( {c + t}\right) \mathrm{d}t + {\int }_{-\infty }^{+\infty }{tf}\left( {c + t}\right) \mathrm{d}t
$$

而

$$
{\int }_{-\infty }^{+\infty }{cf}\left( {c + t}\right)  = c{\int }_{-\infty }^{+\infty }f\left( {c + t}\right) \mathrm{d}t\frac{x = \left( {c + t}\right) }{}c{\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = c
$$

由题意知:

$$
{\int }_{-\infty }^{0}{tf}\left( {c + t}\right) \mathrm{d}t = {\int }_{-\infty }^{0}{tf}\left( {c - t}\right) \mathrm{d}t\frac{u =  - t}{}{\int }_{0}^{+\infty }{uf}\left( {c + u}\right) \mathrm{d}u =  - {\int }_{0}^{+\infty }{tf}\left( {c + t}\right) \mathrm{d}t
$$

即

$$
{\int }_{-\infty }^{0}{tf}\left( {c + t}\right) \mathrm{d}t + {\int }_{0}^{+\infty }{tf}\left( {c + t}\right) \mathrm{d}t = 0
$$

亦即

$$
{\int }_{-\infty }^{+\infty }{tf}\left( {c + t}\right) \mathrm{d}t = 0
$$

从而证明 ${EX} = c$.

#### 题型 3. 随机变量函数的数学期望

【1.7】设随机变量 $X$ 的分布律为

<table><tr><td>$X$</td><td>-2</td><td>0</td><td>2</td></tr><tr><td>$P$</td><td>0.4</td><td>0.3</td><td>0.3</td></tr></table>

求 $E\left( X\right), E\left( {X}^{2}\right), E\left( {3{X}^{2} + 5}\right)$.

解 $E\left( X\right)  = \left( {-2}\right)  \times  {0.4} + 0 \times  {0.3} + 2 \times  {0.3} =  - {0.2}$

$E\left( {X}^{2}\right)  = {\left( -2\right) }^{2} \times  {0.4} \times   + {0}^{2} \times  {0.3} + {2}^{2} \times  {0.3} = {2.8}$

$E\left( {3{X}^{2} + 5}\right)  = \left\lbrack  {3 \times  {\left( -2\right) }^{2} + 5}\right\rbrack   \times  {0.4} + \left\lbrack  {3 \times  {0}^{2} + 5}\right\rbrack   \times  {0.3} + \left\lbrack  {3 \times  {2}^{2} + 5}\right\rbrack   \times  {0.3} = {13.4}$ 或由期望的性质

$$
E\left( {3{X}^{2} + 5}\right)  = {3E}\left( {X}^{2}\right)  + 5 = 3 \times  {2.8} + 5 = {13.4}.
$$

【1.8】设随机变量 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

求 $\left( 1\right) Y = {2X}$;

(2) $Y = {\mathrm{e}}^{-{2X}}$ 的数学期望.

解 (1) $E\left( Y\right)  = E\left( {2X}\right)  = {\int }_{-\infty }^{+\infty }{2xf}\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }{2x}{\mathrm{e}}^{-x}\mathrm{\;d}x = 2$;

(2) $E\left( Y\right)  = E\left( {\mathrm{e}}^{-{2X}}\right)  = {\int }_{-\infty }^{+\infty }{\mathrm{e}}^{-{2x}}f\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }{\mathrm{e}}^{-{2x}}{\mathrm{e}}^{-x}\mathrm{\;d}x = \frac{1}{3}$.

【1.9】设二维随机变量的联合分布列为

<table><tr><td>Y $X$</td><td>1</td><td>2</td></tr><tr><td>1</td><td>0.25</td><td>0.32</td></tr><tr><td>2</td><td>0.08</td><td>0.35</td></tr></table>

求 $E\left( {{X}^{2} + Y}\right)$.

解 由公式 $E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack   = \mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}g\left( {{x}_{i},{y}_{j}}\right) {p}_{ij}$ :

$E\left( {{X}^{2} + Y}\right)  = \left( {{1}^{2} + 1}\right)  \times  {0.25} + \left( {{1}^{2} + 2}\right)  \times  {0.32} + \left( {{2}^{2} + 1}\right)  \times  {0.08} + \left( {{2}^{2} + 2}\right)  \times  {0.35}$

$= {3.96}$.

【1.10】设二维随机变量 $\left( {X, Y}\right)$ 的联合分布密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{matrix} x + y, & 0 \leq  x \leq  1,0 \leq  y \leq  1 \\  0, & \text{ 其他 } \end{matrix}\right.
$$

求 $E\left( {XY}\right), E\left( X\right), E\left( Y\right)$.

解 由公式 $E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack   = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }g\left( {x, y}\right) f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y$

$$
E\left( {XY}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xyf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}{\int }_{0}^{1}{xy}\left( {x + y}\right) \mathrm{d}x\mathrm{\;d}y = \frac{1}{3}.
$$

求 $E\left( X\right)$ 与 $E\left( Y\right)$ 有两种方法:

方法一 先求出 ${f}_{X}\left( x\right),{f}_{Y}\left( y\right)$,利用公式

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }x{f}_{X}\left( x\right) \mathrm{d}x
$$

求出结论

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  \begin{array}{ll} x + \frac{1}{2}, & 0 \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }x{f}_{X}\left( x\right) \mathrm{d}x = {\int }_{0}^{1}x\left( {x + \frac{1}{2}}\right) \mathrm{d}x = \frac{7}{12}
$$

同理可求 $E\left( Y\right)  = \frac{7}{12}$ 量 142

方法二 直接使用 $E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack$ 公式

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = \frac{7}{12}
$$

$$
E\left( Y\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{yf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = \frac{7}{12}.
$$

点评 当已知 $\left( {X, Y}\right)$ 的概率密度 $f\left( {x, y}\right)$,求 $E\left( X\right) \text{、}E\left( Y\right)$ 时方法二简便.

【1.11】假设随机变量 $Y$ 服从参数为 $\lambda  = 1$ 的指数分布,随机变量

$$
{X}_{k} = \left\{  {\begin{array}{ll} 0, & Y \leq  k \\  1, & Y > k \end{array}\;\left( {k = 1,2}\right) }\right.
$$

(1)求 ${X}_{1}$ 和 ${X}_{2}$ 的联合概率分布；

(2) 求 $E\left( {{X}_{1} + {X}_{2}}\right)$.

解 (1) $Y$ 的分布函数为 $F\left( y\right)  = 1 - {\mathrm{e}}^{-y}\left( {y > 0}\right),\;F\left( y\right)  = 0\left( {y \leq  0}\right)$.

$\left( {{X}_{1},{X}_{2}}\right)$ 有四个可能值: $\left( {0,0}\right),\left( {0,1}\right),\left( {1,0}\right),\left( {1,1}\right)$.

易见

$$
P\left\{  {{X}_{1} = 0,{X}_{2} = 0}\right\}   = P\{ Y \leq  1, Y \leq  2\}  = P\{ Y \leq  1\}  = 1 - {\mathrm{e}}^{-1}
$$

$$
P\left\{  {{X}_{1} = 0,{X}_{2} = 1}\right\}   = P\{ Y \leq  1, Y > 2\}  = 0
$$

$$
P\left\{  {{X}_{1} = 1,{X}_{2} = 0}\right\}   = P\{ Y > 1, Y \leq  2\}  = P\{ 1 < Y \leq  2\}  = {\mathrm{e}}^{-1} - {\mathrm{e}}^{-2}
$$

$$
P\left\{  {{X}_{1} = 1,{X}_{2} = 1}\right\}   = P\{ Y > 1, Y > 2\}  = P\{ Y > 2\}  = {\mathrm{e}}^{-2}
$$

于是, ${X}_{1}$ 和 ${X}_{2}$ 的联合概率分布表如下:

<table><tr><td>${X}_{1}$</td><td>0</td><td>1</td></tr><tr><td>0</td><td>$1 - {\mathrm{e}}^{-1}$</td><td>${\mathrm{e}}^{-1} - {\mathrm{e}}^{-2}$</td></tr><tr><td/><td>0</td><td>${\mathrm{e}}^{-2}$</td></tr></table>

(2)易见, ${X}_{k}\left( {k = 1,2}\right)$ 服从 $0 - 1$ 分布:

$$
{X}_{k} \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  P\{ Y \leq  k\} & P\{ Y > k\}  \end{matrix}\right\rbrack   = \left\lbrack  \begin{matrix} 0 & 1 \\  1 - {\mathrm{e}}^{-k} & {\mathrm{e}}^{-k} \end{matrix}\right\rbrack
$$

因此 $E{X}_{k} = 1 \times  {\mathrm{e}}^{-k} = {\mathrm{e}}^{-k}\;\left( {k = 1,2}\right)$

则 $E\left( {{X}_{1} + {X}_{2}}\right)  = E{X}_{1} + E{X}_{2} = {\mathrm{e}}^{-1} + {\mathrm{e}}^{-2}$.

点评 第二问中 $E\left( {{X}_{1} + {X}_{2}}\right)$ 也可以利用公式

$$
E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack   = \mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}g\left( {{x}_{i},{y}_{j}}\right) {p}_{ij}
$$

直接计算得:

$$
E\left( {{X}_{1} + {X}_{2}}\right)  = 1 \times  \left( {{\mathrm{e}}^{-1} - {\mathrm{e}}^{-2}}\right)  + 2 \times  {\mathrm{e}}^{-2} = {\mathrm{e}}^{-1} + {\mathrm{e}}^{-2}.
$$

#### 题型 4. 利用性质求期望

【1.12】已知离散型随机变量 $X$ 服从参数为 2 的泊松分布,即

$$
P\{ X = k\}  = \frac{{2}^{k}{\mathrm{e}}^{-2}}{k!},\;k = 0,1,2,\cdots,
$$

则随机变量 $Z = {3X} - 2$ 的数学期望 ${EZ} =$ _____.

解 本题要求读者熟悉泊松分布的数字特征, 并会利用数学期望的性质求随机变量线性函数的数学期望.

由于 $X$ 服从参数为 2 的泊松分布,则 ${EX} = 2$,所以

$$
{EZ} = E\left( {{3X} - 2}\right)  = {3EX} - 2 = 4.
$$

【1.13】设随机变量 ${X}_{ij}\left( {i, j = 1,2,\cdots, n;n \geq  2}\right)$ 独立同分布, $E{X}_{ij} = 2$,则行列式

$$
Y = \left| \begin{matrix} {X}_{11} & {X}_{12} & \cdots & {X}_{1n} \\  {X}_{21} & {X}_{22} & \cdots & {X}_{2n} \\  \cdots & \cdots & \cdots & \cdots \\  {X}_{n1} & {X}_{n2} & \cdots & {X}_{nn} \end{matrix}\right|
$$

的数学期望 ${EY} =$ _____.

解 由 $Y = \mathop{\sum }\limits_{{{j}_{1}{j}_{2}\cdots {j}_{n}}}{\left( -1\right) }^{\tau \left( {{j}_{1}{j}_{2}\cdots {j}_{n}}\right) }{X}_{1{j}_{1}}{X}_{2{j}_{2}}\cdots {X}_{n{j}_{n}}$

且随机变量 ${X}_{ij}\left( {i, j = 1,2,\cdots, n}\right)$ 相互独立同分布, $E{X}_{ij} = 2$,有

$$
{EY} = E\mathop{\sum }\limits_{{{j}_{1}{j}_{2}\cdots {j}_{n}}}{\left( -1\right) }^{\tau \left( {{j}_{1}{j}_{2}\cdots {j}_{n}}\right) }{X}_{1{j}_{1}}{X}_{2{j}_{2}}\cdots {X}_{n{j}_{n}}
$$

$$
= \mathop{\sum }\limits_{{{j}_{1}{j}_{2}\cdots {j}_{n}}}{\left( -1\right) }^{\tau \left( {{j}_{1}{j}_{2}\cdots {j}_{n}}\right) }E{X}_{1{j}_{1}}E{X}_{2{j}_{2}}\cdots E{X}_{n{j}_{n}}
$$

$$
= \left| \begin{matrix} E{X}_{11} & E{X}_{12} & \cdots & E{X}_{1n} \\  E{X}_{21} & E{X}_{22} & \cdots & E{X}_{2n} \\  \cdots & \cdots & \cdots & \cdots \\  E{X}_{n1} & E{X}_{n2} & \cdots & E{X}_{nn} \end{matrix}\right|  = \left| \begin{matrix} 2 & 2 & \cdots & 2 \\  2 & 2 & \cdots & 2 \\  \cdots & \cdots & \cdots & \cdots \\  2 & 2 & \cdots & 2 \end{matrix}\right|  = 0.
$$

故应填 0.

【1.14】从甲地到乙地的旅游车上载 20 位旅客自甲地开出,沿途有 10 个车站,如到达一个车站没有旅客下车就不停车. 以 $X$ 表示停车次数,求 $E\left( X\right)$ (设每位旅客在各个车站下车是等可能的).

解 引进随机变量 ${X}_{i} = \left\{  \begin{array}{ll} 0, & \text{ 第 }i\text{ 站没有人下车; } \\  1, & \text{ 第 }i\text{ 站有人下车. } \end{array}\right.$

则

$$
X = {X}_{1} + {X}_{2} + \cdots  + {X}_{10}.
$$

根据题意任一旅客在第 $i$ 站不下车的概率为 $\frac{9}{10}$,因此 20 位旅客在第 $i$ 站不下车的概率为 ${\left( \frac{9}{10}\right) }^{20}$,在第 $i$ 站有人下车的概率为 $1 - {\left( \frac{9}{10}\right) }^{20}$. 即

$$
P\left\{  {{X}_{i} = 0}\right\}   = {\left( \frac{9}{10}\right) }^{20},\;P\left\{  {{X}_{i} = 1}\right\}   = 1 - {\left( \frac{9}{10}\right) }^{20}.\;\left( {i = 1,2,\cdots,{10}}\right)
$$

由此

$$
E\left( {X}_{i}\right)  = 0 \times  {\left( \frac{9}{10}\right) }^{20} + 1 \times  \left\lbrack  {1 - {\left( \frac{9}{10}\right) }^{20}}\right\rbrack   = 1 - {\left( \frac{9}{10}\right) }^{20}
$$

电

$$
{EX} = \mathop{\sum }\limits_{{i = 1}}^{{10}}\left\lbrack  {1 - {\left( \frac{9}{10}\right) }^{20}}\right\rbrack   \approx  {8.8}.
$$

故平均停车 9 次.

点评 将 $X$ 分解成数个随机变量之和,然后利用数学期望的性质求 ${EX}$,这种方法对于不易求分布律的随机变量计算数学期望有很大作用.

【1.15】设 $X, Y$ 相互独立,其密度函数分别为

$$
{f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} {2x}, & 0 \leq  x \leq  1, \\  0, & \text{ 其他,} \end{array}\;{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-\left( {y - 5}\right) }, & y > 5, \\  0, & \text{ 其他 } \end{array}\right. }\right.
$$

求 $E\left( {XY}\right)$.

解法一 因为 $X, Y$ 相互独立,故利用期望性质

$$
E\left( {XY}\right)  = E\left( X\right)  \cdot  E\left( Y\right)  = {\int }_{0}^{1}{x2x}\mathrm{\;d}x{\int }_{5}^{+\infty }y{\mathrm{e}}^{-\left( {y - 5}\right) }\mathrm{d}y = \frac{2}{3} \times  6 = 4.
$$

解法二

$$
E\left( {XY}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xy}{f}_{X}\left( x\right) {f}_{Y}\left( y\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}{\int }_{5}^{+\infty }{xy2x}{\mathrm{e}}^{-\left( {y - 5}\right) }\mathrm{d}x\mathrm{\;d}y = 4.
$$

#### 题型 5. 数学期望的应用

【1.16】游客乘电梯从底层到电视塔顶层观光. 电梯于每个整点的第 5 分钟、 25 分钟和 55 分钟从底层起行,假设一游客在早八点的第 $X$ 分钟到达底层候梯处,且 $X$ 在 $\left\lbrack  {0,{60}}\right\rbrack$ 上均匀分布,求该游客等候时间的数学期望.

解 已知 $X$ 在 $\left\lbrack  {0,{60}}\right\rbrack$ 上服从均匀分布,其密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{60}, & \text{ 若 }0 \leq  x \leq  {60} \\  0, & \text{ 其他 } \end{array}\right.
$$

设 $Y$ 为游客等候电梯的时间 (单位: 分),则

$$
Y = g\left( X\right)  = \left\{  \begin{array}{ll} 5 - X, & 0 < X \leq  5 \\  {25} - X, & 5 < X \leq  {25} \\  {55} - X, & {25} < X \leq  {55} \\  {60} - X + 5, & {55} < X \leq  {60} \end{array}\right.
$$

因此,

$$
E\left( Y\right)  = E\left\lbrack  {g\left( X\right) }\right\rbrack   = {\int }_{-\infty }^{+\infty }g\left( x\right) f\left( x\right) \mathrm{d}x = \frac{1}{60}{\int }_{0}^{60}g\left( x\right) \mathrm{d}x
$$

$$
= \frac{1}{60}\left\lbrack  {{\int }_{0}^{5}\left( {5 - x}\right) \mathrm{d}x + {\int }_{5}^{25}\left( {{25} - x}\right) \mathrm{d}x + {\int }_{25}^{55}\left( {{55} - x}\right) \mathrm{d}x + {\int }_{55}^{60}\left( {{65} - x}\right) \mathrm{d}x}\right\rbrack
$$

$$
= \frac{1}{60}\left\lbrack  {{12.5} + {200} + {450} + {37.5}}\right\rbrack   = {11.67}.
$$

【1.17】设某种商品每周的需求量 $X$ 是服从区间 $\left\lbrack  {{10},{30}}\right\rbrack$ 上均匀分布的随机变量,而经销商店进货数量为区间 $\left\lbrack  {{10},{30}}\right\rbrack$ 中的某一整数,商店每销售 1 单位商品可获利 500 元；若供大于求则削价处理, 每处理 1 单位商品亏损 100 元; 若供不应求, 则可从外部调剂供应, 此时每 1 单位商品仅获利 300 元, 为使商店所获利润期望值不少于 9280 元, 试确定最少进货量.

解 设进货数量为 $a$,则利润为

$$
Y = \left\{  {\begin{array}{ll} {500a} + \left( {X - a}\right) {300}, & a < X \leq  {30} \\  {500X} - \left( {a - X}\right) {100}, & {10} \leq  X \leq  a \end{array} = \left\{  \begin{array}{ll} {300X} + {200a}, & a < X \leq  {30} \\  {600X} - {100a}, & {10} \leq  X \leq  a \end{array}\right. }\right.
$$

利润期望

$$
{EY} = {\int }_{-\infty }^{+\infty }g\left( x\right) f\left( x\right) \mathrm{d}x = {\int }_{10}^{30}\frac{1}{20} \cdot  g\left( x\right) \mathrm{d}x
$$

$$
= \frac{1}{20}{\int }_{10}^{a}\left( {{600x} - {100a}}\right) \mathrm{d}x + \frac{1}{20}{\int }_{a}^{30}\left( {{300x} + {200a}}\right) \mathrm{d}x
$$

$$
= {\left. \frac{1}{20}\left( {600}\frac{{x}^{2}}{2} - {100}ax\right) \right| }_{10}^{a} + {\left. \frac{1}{20}\left( {300}\frac{{x}^{2}}{2} + {200}ax\right) \right| }_{a}^{30}
$$

$$
=  - {7.5}{a}^{2} + {350a} + {5250}.
$$

依题意, 有

$$
- {7.5}{a}^{2} + {350a} + {5250} \geq  {9280}\text{即}{7.5}{a}^{2} - {350a} + {4030} \leq  0\text{,}
$$

解得 ${20}\frac{2}{3} \leq  a \leq  {26}$.

故利润期望值不少于 9280 元的最少进货量为 21 单位.

【1.18】假设一部机器在一天内发生故障的概率为 0.2,机器发生故障时全天停止工作,若一周 5 个工作日里无故障,可获利润 10 万元；发生一次故障仍可获利润 5 万元；发生二次故障所获利润 0 元；发生三次或三次以上故障要亏损 2 万元. 求一周内期望利润是多少?

解 设一周 5 个工作日内发生故障的天数为 $X$,由题意知 $X$ 服从二项分布,

$$
P\{ X = 0\}  = {0.8}^{5} = {0.32768},
$$

$$
P\{ X = 1\}  = {C}_{5}^{1}{0.2} \times  {0.8}^{4} = {0.4096},
$$

$$
P\{ X = 2\}  = {C}_{5}^{2}{0.8}^{3} \times  {0.2}^{2} = {0.2048},
$$

$$
P\{ X \geq  3\}  = 1 - P\{ X = 0\}  - P\{ X = 1\}  - P\{ X = 2\}  = {0.05792}.
$$

假设一周内获利为 $Y$ 万元,可得知以下关系

$$
Y = f\left( X\right)  = \left\{  \begin{array}{ll} {10}, & \text{ 当 }X = 0 \\  5, & \text{ 当 }X = 1 \\  0, & \text{ 当 }X = 2 \\   - 2, & \text{ 当 }X \geq  3 \end{array}\right.
$$

则 $Y$ 的分布律为:

<table><tr><td>$Y$</td><td>10</td><td>5</td><td>0</td><td>-2</td></tr><tr><td>$P$</td><td>0.32768</td><td>0.4096</td><td>0.2048</td><td>0.05792</td></tr></table>

则 ${EY} = {10} \times  {0.32768} + 5 \times  {0.4096} - 2 \times  {0.05792} = {5.20896}$. 146

## §2. 方差

### 知识要点

#### 1. 方差的统一定义和简化公式

若随机变量 $X$ 的数学期望 ${EX}$ 存在,则 $X$ 的方差可用下式统一定义:

$$
{DX} = E{\left( X - EX\right) }^{2}
$$

其简化计算公式为

$$
{DX} = E{X}^{2} - {\left( EX\right) }^{2}
$$

#### 2. 方差的性质

(1) $D\left( c\right)  = 0$ (c 为任意常数)

(2) $D\left( {cX}\right)  = {c}^{2}{DX}$ ( $c$ 为任意常数)

(3)若 $X$ 与 $Y$ 相互独立,则有 $D\left( {X \pm  Y}\right)  = {DX} + {DY}$

#### 3. 常见离散型分布的数字特征

(1)若 $X \sim  B\left( {n, p}\right)$,则 ${EX} = {np},{DX} = {npq}\left( {0 < p < 1, p + q = 1}\right)$

(2)若 $X$ 服从参数为 $\lambda$ 的泊松分布,则 ${EX} = \lambda,{DX} = \lambda \left( {\lambda  > 0}\right)$

(3)若 $X$ 服从参数为 $p$ 的几何分布,则 ${EX} = \frac{1}{p},{DX} = \frac{1 - p}{{p}^{2}}$

#### 4. 常见连续型分布的数字特征

(1)若 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,则 ${EX} = \mu,{DX} = {\sigma }^{2}$

(2)若 $X$ 服从参数为 $\lambda$ 的指数分布,则 ${EX} = \frac{1}{\lambda },{DX} = \frac{1}{{\lambda }^{2}}\left( {\lambda  > 0}\right)$

(3)若 $X$ 服从 $\left\lbrack  {a, b}\right\rbrack$ 上的均匀分布,则 ${EX} = \frac{a + b}{2},{DX} = \frac{{\left( b - a\right) }^{2}}{12}$

### 基本题型

#### 题型 1. 方差的计算

【2.1】计算【1.1】中的方差及标准差.

解 因为

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>$\frac{3}{4}$</td><td>$\frac{9}{44}$</td><td>$\frac{9}{220}$</td><td>$\frac{1}{220}$</td></tr></table>

且 $E\left( X\right)  = {0.3}$. 而

$$
E\left( {X}^{2}\right)  = \mathop{\sum }\limits_{i}{x}_{i}^{2}{p}_{i} = {1}^{2} \times  \frac{9}{44} + {2}^{2} \times  \frac{9}{220} + {3}^{2} \times  \frac{1}{220} = {0.41},
$$

则

$$
D\left( X\right)  = E\left( {X}^{2}\right)  - {\left( EX\right) }^{2} = {0.32}.
$$

标准差为 $\sqrt{D\left( X\right) } = {0.57}$.

【2.2】设随机变量 $X$ 服从几何分布,其分布律为

$$
P\{ X = k\}  = p{\left( 1 - p\right) }^{k - 1},\;k = 1,2,\cdots.
$$

其中 $0 < p < 1$ 是常数,求 $E\left( X\right), D\left( X\right)$.

解 $P\{ X = k\}  = p{q}^{k - 1}\;\left( {k = 1,2,\cdots, n,\cdots }\right)$,其中 $q = 1 - p$,由此得

$$
{EX} = \mathop{\sum }\limits_{{k = 1}}^{\infty }{kp}{q}^{k - 1} = p\mathop{\sum }\limits_{{k = 1}}^{\infty }k{q}^{k - 1},
$$

为了求这无穷级数的和,我们可以用已知的幂级数展开式:

$$
\frac{1}{1 - x} = 1 + x + {x}^{2} + \cdots  + {x}^{k} + \cdots \;\left( {\left| x\right|  < 1}\right)
$$

按幂级数的微分法得

$$
\frac{1}{{\left( 1 - x\right) }^{2}} = 1 + {2x} + 3{x}^{2} + \cdots  + k{x}^{k - 1} + \cdots \;\left( {\left| x\right|  < 1}\right)
$$

因为 $q = 1 - p$,且 $0 < q < 1$,所以有

$$
{EX} = \frac{p}{{\left( 1 - q\right) }^{2}} = \frac{p}{{p}^{2}} = \frac{1}{p}
$$

为了求方差 ${DX}$,先来求 $E\left( {X}^{2}\right)$,即

$$
E\left( {X}^{2}\right)  = \mathop{\sum }\limits_{{k = 1}}^{\infty }{k}^{2}p{q}^{k - 1} = p\mathop{\sum }\limits_{{k = 1}}^{\infty }{k}^{2}{q}^{k - 1} = p\left\lbrack  {\mathop{\sum }\limits_{{k = 1}}^{\infty }{\left( {q}^{k + 1}\right) }^{\prime \prime } - \mathop{\sum }\limits_{{k = 1}}^{\infty }k{q}^{k - 1}}\right\rbrack   = \frac{2 - p}{{p}^{2}}
$$

故 ${DX} = E\left( {X}^{2}\right)  - {\left( EX\right) }^{2} = \frac{1 - p}{{p}^{2}}$.

【2.3】设随机变量 $X$ 的分布密度为 $f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{\pi \sqrt{1 - {x}^{2}}}, & \left| x\right|  < 1 \\  0, & \left| x\right|  \geq  1 \end{array}\right.$,则数学期望 ${EX}$ 和方差 ${DX}$ 分别为_____,_____.

解 因为 $f\left( x\right)$ 是偶函数, ${xf}\left( x\right)$ 是奇函数,所以

$$
{EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = 0,
$$

$$
{DX} = E{X}^{2} - {\left( EX\right) }^{2} = {\int }_{-\infty }^{+\infty }{x}^{2}f\left( x\right) \mathrm{d}x = 2{\int }_{0}^{1}{x}^{2}\frac{1}{\pi \sqrt{1 - {x}^{2}}}\mathrm{\;d}x
$$

$$
= {\left. \frac{1}{\pi }\left( -\frac{x}{2}\sqrt{1 - {x}^{2}} + \frac{1}{2}\arcsin x\right) \right| }_{0}^{1} = \frac{1}{2}\text{.}
$$

【2.4】设二维随机变量 $\left( {X, Y}\right)$ 在 $0 < x < 1,\left| y\right|  < x$ 上服从均匀分布,求 $Z = {2X} + 1$ 的方差.

解 由 $\left( {X, Y}\right)$ 的联合分布密度

$$
\varphi \left( {x, y}\right)  = \left\{  \begin{array}{ll} 1, & 0 < x < 1,\left| y\right|  < x \\  0, & \text{ 其他 } \end{array}\right.
$$

可得到

$$
{\varphi }_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }\varphi \left( {x, y}\right) \mathrm{d}y = {\int }_{-x}^{x}1 \cdot  \mathrm{d}y = {2x}\;\left( {0 < x < 1}\right).
$$

所以

$$
D\left( Z\right)  = D\left( {{2X} + 1}\right)  = {2}^{2}D\left( X\right)  = {4D}\left( X\right)  = 4\left\lbrack  {E\left( {X}^{2}\right)  - {\left( EX\right) }^{2}}\right\rbrack
$$

$$
= 4\left\lbrack  {{\int }_{-\infty }^{+\infty }{x}^{2}{\varphi }_{X}\left( x\right) \mathrm{d}x - {\left( {\int }_{-\infty }^{+\infty }x{\varphi }_{X}\left( x\right) \mathrm{d}x\right) }^{2}}\right\rbrack
$$

$$
= 4\left\lbrack  {{\int }_{0}^{1}{x}^{2} \cdot  {2x}\mathrm{\;d}x - {\left( {\int }_{0}^{1}x2x\mathrm{\;d}x\right) }^{2}}\right\rbrack
$$

$$
= {\left. 4\left( \frac{1}{2}{x}^{4} - \frac{4{x}^{6}}{9}\right) \right| }_{0}^{1} = 4\left( {\frac{1}{2} - \frac{4}{9}}\right)  = \frac{2}{9}.
$$

点评 $E\left( X\right)$ 及 $E\left( {X}^{2}\right)$ 也可利用 $E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack$ 公式计算:

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{x\varphi }\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y.
$$

$$
E\left( {X}^{2}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{x}^{2}\varphi \left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y.
$$

这种解法无需求边缘密度 ${\varphi }_{X}\left( x\right)$.

【2.5】设随机变量 $X$ 在区间 $\left\lbrack  {-1,2}\right\rbrack$ 上服从均匀分布,随机变量

$$
Y = \left\{  \begin{array}{ll} 1, & \text{ 若 }X > 0 \\  0, & \text{ 若 }X = 0 \\   - 1, & \text{ 若 }X < 0 \end{array}\right.
$$

则方差 ${DY} =$ _____.

分析 由 $X$ 的分布得到 $Y$ 的分布律进而求得期望,然后计算方差.

解 根据题意得

$$
P\{ Y = 1\}  = P\{ X > 0\}  = \frac{2}{3},
$$

$$
P\{ Y = 0\}  = P\{ X = 0\}  = 0,
$$

$$
P\{ Y =  - 1\}  = P\{ X < 0\}  = \frac{1}{3},
$$

所以

$$
{EY} = 1 \times  \frac{2}{3} + \left( {-1}\right)  \times  \frac{1}{3} + 0 = \frac{1}{3},
$$

$$
E{Y}^{2} = 1 \times  \frac{2}{3} + {\left( -1\right) }^{2} \times  \frac{1}{3} + 0 = 1,
$$

$$
{DY} = E{Y}^{2} - {\left( EY\right) }^{2} = 1 - \frac{1}{9} = \frac{8}{9}.
$$

#### 题型 2. 期望与方差性质的综合使用

【2.6】设两个相互独立的随机变量 $X$ 和 $Y$ 的方差分别为 4 和 2,则随机变量 ${3X} - {2Y}$ 的方差是 (   ).

(A) 8 (B) 16 (C) 28 (D) 44

解 由方差的性质知

$D\left( {{3X} - {2Y}}\right)  = D\left( {3X}\right)  + D\left( {-{2Y}}\right)  = {3}^{2}D\left( X\right)  + {\left( -2\right) }^{2}D\left( Y\right)  = {36} + 8 = {44}.$

故应选(D).

【2.7】设连续型随机变量 ${X}_{1}$ 与 ${X}_{2}$ 相互独立且方差均存在, ${X}_{1}$ 与 ${X}_{2}$ 的概率密度分别为

${f}_{1}\left( x\right)$ 与 ${f}_{2}\left( x\right)$,随机变量 ${Y}_{1}$ 的概率密度为

$$
{f}_{{Y}_{1}}\left( y\right)  = \frac{1}{2}\left\lbrack  {{f}_{1}\left( y\right)  + {f}_{2}\left( y\right) }\right\rbrack ,
$$

随机变量 ${Y}_{2} = \frac{1}{2}\left( {{X}_{1} + {X}_{2}}\right)$,则_____.

(A) $E{Y}_{1} > E{Y}_{2}, D{Y}_{1} > D{Y}_{2}$ (B) $E{Y}_{1} = E{Y}_{2}, D{Y}_{1} = D{Y}_{2}$

(C) $E{Y}_{1} = E{Y}_{2}, D{Y}_{1} < D{Y}_{2}$ (D) $E{Y}_{1} = E{Y}_{2}, D{Y}_{1} > D{Y}_{2}$

解 $E{Y}_{1} = {\int }_{-\infty }^{+\infty }y{f}_{{Y}_{1}}\left( y\right) \mathrm{d}y = \frac{1}{2}\left\lbrack  {{\int }_{-\infty }^{+\infty }y{f}_{1}\left( y\right) \mathrm{d}y + {\int }_{-\infty }^{+\infty }y{f}_{2}\left( y\right) \mathrm{d}y}\right\rbrack$

$= \frac{1}{2}\left( {E{X}_{1} + E{X}_{2}}\right),$

$E{Y}_{2} = \frac{1}{2}E\left( {{X}_{1} + {X}_{2}}\right)  = \frac{1}{2}\left( {E{X}_{1} + E{X}_{2}}\right)$,故 $E{Y}_{1} = E{Y}_{2}$.

$D{Y}_{1} = E\left( {Y}_{1}^{2}\right)  - {\left( E{Y}_{1}\right) }^{2}, D{Y}_{2} = E\left( {Y}_{2}^{2}\right)  - {\left( E{Y}_{2}\right) }^{2},$

则 $D{Y}_{1} - D{Y}_{2} = E\left( {Y}_{1}^{2}\right)  - E\left( {Y}_{2}^{2}\right)$

$= \frac{1}{2}\left\lbrack  {{\int }_{-\infty }^{+\infty }{y}^{2}{f}_{1}\left( y\right) \mathrm{d}y + {\int }_{-\infty }^{+\infty }{y}^{2}{f}_{2}\left( y\right) \mathrm{d}y}\right\rbrack   - E\left\lbrack  {\frac{1}{4}{\left( {X}_{1} + {X}_{2}\right) }^{2}}\right\rbrack$

$= \frac{1}{2}E\left( {X}_{1}^{2}\right)  + \frac{1}{2}E\left( {X}_{2}^{2}\right)  - \frac{1}{4}E\left\lbrack  {\left( {X}_{1} + {X}_{2}\right) }^{2}\right\rbrack$

$= \frac{1}{4}E\left( {{X}_{1}^{2} + {X}_{2}^{2} - 2{X}_{1}{X}_{2}}\right)$

$= \frac{1}{4}E\left\lbrack  {\left( {X}_{1} - {X}_{2}\right) }^{2}\right\rbrack   > 0,$

即 $D{Y}_{1} > D{Y}_{2}$.

故应选(D).

【2.8】设 $X$ 的均值、方差都存在,且 $D\left( X\right)  \neq  0$,令

$$
Y = \frac{X - E\left( X\right) }{\sqrt{D\left( X\right) }}
$$

则 $E\left( Y\right)  =$ _____, $D\left( Y\right)  =$ _____.

解 $E\left( Y\right)  = E\left( \frac{X - E\left( X\right) }{\sqrt{D\left( X\right) }}\right)  = \frac{1}{\sqrt{D\left( X\right) }}E\left( {X - E\left( X\right) }\right)  = \frac{1}{\sqrt{D\left( X\right) }}\left\lbrack  {E\left( X\right)  - E\left( X\right) }\right\rbrack   = 0$,

$D\left( Y\right)  = D\left( \frac{X - E\left( X\right) }{\sqrt{D\left( X\right) }}\right)  = \frac{1}{D\left( X\right) }D\left( {X - E\left( X\right) }\right)  = \frac{1}{D\left( X\right) }\left\lbrack  {D\left( X\right)  + D\left( {-E\left( X\right) }\right) }\right\rbrack$

$= \frac{D\left( X\right) }{D\left( X\right) } = 1.$

【2.9】设 $X$ 为随机变量, $C$ 是常数,证明

$$
D\left( X\right)  < E\left\{  {\left( X - C\right) }^{2}\right\} ,\;\text{ 对于 }C \neq  E\left( X\right).
$$

(由于 $D\left( X\right)  = E{\left\lbrack  X - E\left( X\right) \right\rbrack  }^{2}$,上式表明 $E\left\{  {\left( X - C\right) }^{2}\right\}$ 当 $C = E\left( X\right)$ 时取到最小值.

$$
\text{证法一}E\left\{  {\left( X - C\right) }^{2}\right\}   = E\left( {{X}^{2} - {2CX} + {C}^{2}}\right)  = E\left( {X}^{2}\right)  - {2CE}\left( X\right)  + {C}^{2}
$$

$$
= E\left( {X}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} + {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} - {2CE}\left( X\right)  + {C}^{2}
$$

$$
= D\left( X\right)  + {\left\lbrack  E\left( X\right)  - C\right\rbrack  }^{2} > D\left( X\right),\;\text{ 当 }E\left( X\right)  \neq  C.
$$

故当 $C = E\left( X\right)$ 时, $E{\left( X - C\right) }^{2}$ 取到最小值 ${DX}$.

证法二 ${DX} = E{\left( X - EX\right) }^{2} = E{\left\lbrack  \left( X - C\right)  + \left( C - EX\right) \right\rbrack  }^{2}$

$$
= E{\left( X - C\right) }^{2} + E{\left( C - EX\right) }^{2} + {2E}\left\lbrack  {\left( {X - C}\right) \left( {C - {EX}}\right) }\right\rbrack
$$

$$
= E{\left( X - C\right) }^{2} - {\left( C - EX\right) }^{2} < E{\left( X - C\right) }^{2}.
$$

【2. 10】设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 是 $n$ 个独立同分布的随机变量, $E\left( {X}_{i}\right)  = \mu, D\left( {X}_{i}\right)  = {\sigma }^{2}, i = 1$, $2,\cdots, n$. 设 $\bar{X} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$,求 $E\left( \bar{X}\right)$ 和 $D\left( \bar{X}\right)$.

解 $E\left( \bar{X}\right)  = E\left\lbrack  {\frac{1}{n}\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}\right) }\right\rbrack   = \frac{1}{n}\left( {E{X}_{1} + E{X}_{2} + \cdots  + E{X}_{n}}\right)$

$$
= \frac{1}{n} \cdot  {n\mu } = \mu.
$$

$D\left( \bar{X}\right)  = D\left\lbrack  {\frac{1}{n}\left( {{X}_{1} + {X}_{2} + \cdots  + {X}_{n}}\right) }\right\rbrack   = \frac{1}{{n}^{2}}\left( {D{X}_{1} + D{X}_{2} + \cdots  + D{X}_{n}}\right) \;$ (由独立性)

$= \frac{1}{{n}^{2}}n{\sigma }^{2} = \frac{{\sigma }^{2}}{n}.$

【2.11】一台设备由三大部件构成,在设备运转中各部件需要调整的概率相应为 0.10,0.20 和 0.30,假设各部件的状态相互独立,以 $X$ 表示同时需要调整的部件数,试求 $X$ 的数学期望 ${EX}$ 和方差 ${DX}$.

解法一 先求 $X$ 的分布律,根据分布律再求期望.

根据 $X$ 的意义,显然有 $X = 0,1,2,3$,事件 ${A}_{i}$ 表示第 $i$ 件需要调整, $i = 1,2,3$,并注意到事件之间的独立性.

$$
P\{ X = 0\}  = P\left( {{\bar{A}}_{1}{\bar{A}}_{2}{\bar{A}}_{3}}\right)  = {0.9} \times  {0.8} \times  {0.7} = {0.504}\text{,}
$$

$$
P\{ X = 1\}  = P\left( {{A}_{1}{\bar{A}}_{2}{\bar{A}}_{3}}\right)  + P\left( {{\bar{A}}_{1}{A}_{2}{\bar{A}}_{3}}\right)  + P\left( {{\bar{A}}_{1}{\bar{A}}_{2}{A}_{3}}\right)
$$

$$
= P\left( {A}_{1}\right) P\left( {\bar{A}}_{2}\right) P\left( {\bar{A}}_{3}\right)  + P\left( {\bar{A}}_{1}\right) P\left( {A}_{2}\right) P\left( {\bar{A}}_{3}\right)  + P\left( {\bar{A}}_{1}\right) P\left( {\bar{A}}_{2}\right) P\left( {A}_{3}\right)
$$

$$
= {0.1} \times  {0.8} \times  {0.7} + {0.9} \times  {0.2} \times  {0.7} + {0.9} \times  {0.8} \times  {0.3} = {0.398}\text{,}
$$

$$
P\{ X = 2\}  = P\left( {{A}_{1}{A}_{2}{\bar{A}}_{3}}\right)  + P\left( {{A}_{1}{\bar{A}}_{2}{A}_{3}}\right)  + P\left( {{\bar{A}}_{1}{A}_{2}{A}_{3}}\right)
$$

$$
= P\left( {A}_{1}\right) P\left( {A}_{2}\right) P\left( {\bar{A}}_{3}\right)  + P\left( {A}_{1}\right) P\left( {\bar{A}}_{2}\right) P\left( {A}_{3}\right)  + P\left( {\bar{A}}_{1}\right) P\left( {A}_{2}\right) P\left( {A}_{3}\right)
$$

$$
= {0.1} \times  {0.2} \times  {0.7} + {0.1} \times  {0.8} \times  {0.3} + {0.9} \times  {0.2} \times  {0.3} = {0.092}\text{,}
$$

$$
P\{ X = 3\}  = P\left( {{A}_{1}{A}_{2}{A}_{3}}\right)  = P\left( {A}_{1}\right) P\left( {A}_{2}\right) P\left( {A}_{3}\right)  = {0.1} \times  {0.2} \times  {0.3} = {0.006}\text{,}
$$

所以

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>0.504</td><td>0.398</td><td>0.092</td><td>0.006</td></tr></table>

$E\left( X\right)  = 0 \times  {0.504} + 1 \times  {0.398} + 2 \times  {0.092} + 3 \times  {0.006} = {0.6}$,

$D\left( X\right)  = E\left( {X}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} = {1}^{2} \times  {0.398} + {2}^{2} \times  {0.092} + {3}^{2} \times  {0.006} - {\left( {0.6}\right) }^{2} = {0.46}$.

解法二 不求 $X$ 的分布律,引进新的随机变量,利用期望、方差的运算性质求出 $X$ 的期望 $E\left( X\right)$,方差 $D\left( X\right)$.

现引进新随机变量 ${X}_{i}$,定义如下:

${X}_{i} = \left\{  \begin{array}{ll} 1, & \text{ 第 }i\text{ 个部件要调整,即 } \\  0, & \text{ 第 }i\text{ 个部件不要调整 } \end{array}\right.$

由此就有

$$
X = \mathop{\sum }\limits_{{i = 1}}^{3}{X}_{i}
$$

而

$$
{X}_{i} \sim  \left( {0 - 1}\right) \text{分布}E\left( {X}_{i}\right)  = P\left\{  {{X}_{i} = 1}\right\}   = P\left( {A}_{i}\right)
$$

所以 $E\left( X\right)  = \mathop{\sum }\limits_{{i = 1}}^{3}P\left( {A}_{i}\right)  = P\left( {A}_{1}\right)  + P\left( {A}_{2}\right)  + P\left( {A}_{3}\right)  = {0.1} + {0.2} + {0.3} = {0.6}$

$D\left( {X}_{i}\right)  = P\left\{  {{X}_{i} = 1}\right\}  P\left\{  {{X}_{i} = 0}\right\}   = P\left( {A}_{i}\right) P\left( {\bar{A}}_{i}\right),\;{X}_{i}$ 之间相互独立

所以

$D\left( X\right)  = \mathop{\sum }\limits_{{i = 1}}^{3}D\left( {X}_{i}\right)  = \mathop{\sum }\limits_{{i = 1}}^{3}P\left( {A}_{i}\right) P\left( {\bar{A}}_{i}\right)  = {0.1} \times  {0.9} + {0.2} \times  {0.8} + {0.3} \times  {0.7} = {0.46}.$

点评 本题中解法二比解法一简单得多,这就是利用性质求 ${EX}$ 和 ${DX}$ 的好处,但如何引进新随机变量是问题的一个难点. 一般地,总是引入 ${X}_{i} \sim  \left( {0 - 1}\right)$ 分布,用 $\sum {X}_{i}$ 来解决问题.

题型 3. 关于重要分布的期望与方差

【2.12】已知随机变量 $X$ 服从二项分布,且 ${EX} = {2.4},{DX} = {1.44}$,则二项分布的参数 $n$, $p$ 的值为 (   ).

(A) $n = 4, p = {0.6}$ (B) $n = 6, p = {0.4}$

(C) $n = 8, p = {0.3}$ (D) $n = {24}, p = {0.1}$

解 因为 $X$ 服从二项分布,参数为 $n, p$,所以 ${EX} = {np},{DX} = {npq}$,且

$\left\{  {\begin{array}{l} {np} = {2.4} \\  {np}\left( {1 - p}\right)  = {1.44} \end{array}\;\text{ 解方程组可得 }\left\{  \begin{array}{l} n = 6 \\  p = {0.4} \end{array}\right. }\right.$

故选 (B).

【2. 13】设 $X$ 服从参数为 $\lambda  > 0$ 的泊松分布,且已知 $E\left\lbrack  {\left( {X - 1}\right) \left( {X - 2}\right) }\right\rbrack   = 1$,则 $\lambda  =$ _____.

解 由 $X \sim  P\left( \lambda \right)$ 有 ${EX} = {DX} = \lambda$ 且

$$
E{X}^{2} = {\left( EX\right) }^{2} + {DX} = {\lambda }^{2} + \lambda
$$

而

$$
E\left\lbrack  {\left( {X - 1}\right) \left( {X - 2}\right) }\right\rbrack   = E\left( {{X}^{2} - {3X} + 2}\right)  = E{X}^{2} - {3EX} + 2 = 1
$$

得

$$
{\lambda }^{2} + \lambda  - {3\lambda } + 2 = 1\;\text{ 即 }{\lambda }^{2} - {2\lambda } + 1 = 0
$$

有 $\lambda  = 1$.

【2. 14】设一次试验成功的概率为 $p$,进行 100 次独立重复试验,当 $p =$ _____时,成功次数的标准差最大,其最大值为_____.

解 成功次数 $X \sim  B\left( {{100}, p}\right),{DX} = {100p}\left( {1 - p}\right)$.

则 $\sqrt{DX} = {10}\sqrt{p\left( {1 - p}\right) }$,显然当 $p = \frac{1}{2}$ 时,标准差 $\sqrt{DX}$ 最大,最大值为 5.

故应填 $\frac{1}{2};5$.

【2.15】已知连续型随机变量 $X$ 的概率密度函数为 $f\left( x\right)  = \frac{1}{\sqrt{\pi }}{\mathrm{e}}^{-{x}^{2} + {2x} - 1}$,则 $X$ 的数学期望为_____； $X$ 的方差为_____.

解 最简便的方法是利用均值为 $\mu$,方差为 ${\sigma }^{2}$ 的正态分布的密度函数为

$$
\frac{1}{\sigma \sqrt{2\pi }}{\mathrm{e}}^{-\frac{{\left( x - \mu \right) }^{2}}{2{\sigma }^{2}}},
$$

由于

$$
f\left( x\right)  = \frac{1}{\sqrt{\pi }}{\mathrm{e}}^{-{x}^{2} + {2x} - 1} = \frac{1}{\sqrt{2\pi } \cdot  \frac{1}{\sqrt{2}}}{\mathrm{e}}^{\frac{{\left( x - 1\right) }^{2}}{2 \cdot  \frac{1}{2}}},
$$

所以 $X$ 的数学期望是 1,方差是 $\frac{1}{2}$.

另外也可由数学期望和方差的定义直接求 ${EX}$ 和 ${DX}$.

【2. 16】设随机变量 $X$ 服从参数为 $\lambda$ 的指数分布,则 $P\{ X > \sqrt{DX}\}  =$ _____.

分析 已知连续型随机变量 $X$ 的分布,求其满足一定条件的概率,转化为定积分计算即可.

解 由题设,知 ${DX} = \frac{1}{{\lambda }^{2}}$,于是

$$
P\{ X > \sqrt{DX}\}  = P\left\{  {X > \frac{1}{\lambda }}\right\}   = {\int }_{\frac{1}{\lambda }}^{+\infty }\lambda {\mathrm{e}}^{-{\lambda x}}\mathrm{\;d}x =  - {\left. {\mathrm{e}}^{-{\lambda \tau }}\right| }_{\frac{1}{\lambda }}^{+\infty } = \frac{1}{\mathrm{e}}.
$$

故应填 $\frac{1}{\mathrm{e}}$.

【2.17】设随机变量 ${X}_{1},{X}_{2},{X}_{3}$ 相互独立,且都服从参数为 $\lambda$ 的泊松分布. 令 $Y = \frac{1}{3}\left( {{X}_{1} + }\right.$ $\left. {{X}_{2} + {X}_{3}}\right)$,则 ${Y}^{2}$ 的数学期望等于_____.

解 根据独立随机变量和的性质以及服从参数为 $\lambda$ 的泊松分布的随机变量数学期望和方差均为 $\lambda$ 知

$$
{EY} = \frac{1}{3}\left( {E{X}_{1} + E{X}_{2} + E{X}_{3}}\right)  = \lambda,
$$

$$
{DY} = \frac{1}{9}\left( {D{X}_{1} + D{X}_{2} + D{X}_{3}}\right)  = \frac{1}{3}\lambda,
$$

故 $E{Y}^{2} = {\left( EY\right) }^{2} + {DY} = {\lambda }^{2} + \frac{1}{3}\lambda$.

【2.18】设电压 $\left( {以V计}\right) X \sim  N\left( {0,9}\right)$,将电压施加于一检波器,其输出电压为 $Y = 5{X}^{2}$,求输出电压的均值.

解 由 $X \sim  N\left( {0,9}\right)$ 知 ${EX} = 0,{DX} = 9$,又 $Y = 5{X}^{2}$,

故 ${EY} = E\left( {5{X}^{2}}\right)  = {5E}{X}^{2} = 5\left\lbrack  {{DX} + {\left( EX\right) }^{2}}\right\rbrack   = 5\left( {9 + 0}\right)  = {45}$.

## $§3$. 协方差与相关系数

### 知识要点

#### 1. 协方差
对于二维随机变量 $\left( {X, Y}\right),\operatorname{Cov}\left( {X, Y}\right)  = E\left\lbrack  {E - E\left( X\right) }\right\rbrack  \left\lbrack  {Y - E\left( Y\right) }\right\rbrack$ 是其协方差,或用 $\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - {EX} \cdot  {EY}$ 表示.

##### 协方差的性质

(1) $\operatorname{Cov}\left( {X, X}\right)  = {DX}$ (2) $\operatorname{Cov}\left( {X, Y}\right)  = \operatorname{Cov}\left( {Y, X}\right)$

(3) $\operatorname{Cov}\left( {{aX},{bY}}\right)  = {ab}\operatorname{Cov}\left( {X, Y}\right)$ (4) $\operatorname{Cov}\left( {{X}_{1} + {X}_{2}, Y}\right)  = \operatorname{Cov}\left( {{X}_{1}, Y}\right)  + \operatorname{Cov}\left( {{X}_{2}, Y}\right)$

(5) $D\left( {X \pm  Y}\right)  = D\left( X\right)  + D\left( Y\right)  \pm  2\operatorname{Cov}\left( {X, Y}\right)$

#### 2. 相关系数

$$
{\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }}\;\left( {D\left( X\right)  > 0, D\left( Y\right)  > 0}\right)
$$

当 ${\rho }_{XY} = 0$ 时, $X$ 与 $Y$ 是不相关的.

相关系数反映了两个随机变量的线性相关程度,当其绝对值越接近 1 时, $X$ 与 $Y$ 的线性相关程度就越强,反之,越接近 0 时, $X$ 与 $Y$ 线性相关程度就越弱.

##### 相关系数的性质

(1) $- 1 \leq  {\rho }_{XY} \leq  1$.

(2)若 $X$ 与 $Y$ 相互独立,则 ${\rho }_{XY} = 0$,即 $X, Y$ 不相关. 反之不一定成立.

(3)若 $X, Y$ 之间有线性关系,即 $Y = {aX} + b\left( {a, b\text{为常数,}a \neq  0}\right)$,则 $\left| {\rho }_{XY}\right|  = 1$,且 $a > 0$ 时, ${\rho }_{XY} = 1;a < 0$ 时, ${\rho }_{XY} =  - 1$.

#### 3. 二维正态分布的参数意义

当 $\left( {X, Y}\right)  \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2};{\mu }_{2},{\sigma }_{2}^{2};\rho }\right)$ 时,

$$
{EX} = {\mu }_{1},\;{EY} = {\mu }_{2},\;{DX} = {\sigma }_{1}^{2},\;{DY} = {\sigma }_{2}^{2},\;{\rho }_{XY} = \rho.
$$

且 $X, Y$ 相互独立 $\Leftrightarrow  X\text{、}Y$ 不相关.

#### 4. 矩

(1)原点矩 设 $X$ 与 $Y$ 是随机变量,如果 $E\left( {{X}^{k}{Y}^{l}}\right) \left( {k, l = 0,1,2,\cdots }\right)$ 存在,则称它为 $X$ 与 $Y$ 的 $k + l$ 阶混合原点矩.

特别地,当 $l = 0$ 时,称 $E{X}^{k}$ 为 $X$ 的 $k$ 阶原点矩.

显然,随机变量 $X$ 的一阶原点矩就是它的数学期望 ${EX}$.

( 2 )中心矩 设随机变量 $X$ 、 $Y$ 的数学期望 ${EX}$ 、 ${EY}$ 存在,且 $E{\left( X - EX\right) }^{k}{\left( Y - EY\right) }^{l}$ 存在, 则称它为 $X$ 与 $Y$ 的 $k + l$ 阶混合中心矩.

特别地,当 $k = l = 1$ 时,就是 $X\text{、}Y$ 的协方差 $E\left( {X - {EX}}\right) \left( {Y - {EY}}\right)$,当 $l = 0$ 时,称 $E(X -$ ${EX}{)}^{k}$ 为 $X$ 的 $k$ 阶中心矩.

显然,随机变量 $X$ 的二阶中心矩就是它的方差 ${DX} = E{\left( X - EX\right) }^{2}$.


#### 5. 协方差矩阵

设 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 为 $n$ 维随机变量,记 ${C}_{ij} = \operatorname{Cov}\left( {{X}_{i},{X}_{j}}\right), i, j = 1,2,\cdots, n$,称

$\left\lbrack  \begin{matrix} {C}_{11} & {C}_{12} & \cdots & {C}_{1n} \\  {C}_{21} & {C}_{22} & \cdots & {C}_{2n} \\  \cdots & \cdots & \cdots & \cdots \\  {C}_{n1} & {C}_{n2} & \cdots & {C}_{nn} \end{matrix}\right\rbrack  \;$ 为 $\left( {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right)$ 的协方差矩阵.

### 基本题型

#### 题型 1. 协方差与相关系数的计算

【3.1】设随机变量 $X$ 和 $Y$ 的联合概率分布为

<table><tr><td>概 Y $X$</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>0</td><td>0.07</td><td>0.18</td><td>0.15</td></tr><tr><td>1</td><td>0.08</td><td>0.32</td><td>0.20</td></tr></table>

则 $X$ 和 $Y$ 的相关系数 $\rho  =$ _____. ${X}^{2}$ 和 ${Y}^{2}$ 的协方差 $\operatorname{Cov}\left( {{X}^{2},{Y}^{2}}\right)  =$ _____.

解 $X$ 的分布律

<table><tr><td>$X$</td><td>0</td><td>1</td></tr><tr><td>$P$</td><td>0.4</td><td>0.6</td></tr></table>

$Y$ 的分布律

$$
E\left( X\right)  = {0.6},
$$

$$
E\left( Y\right)  = {0.35} - {0.15} = {0.2},
$$

$$
E\left( {XY}\right)  = \mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}{x}_{i}{y}_{j}{p}_{ij} =  - {0.08} + {0.20} = {0.12},
$$

$$
\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - E\left( X\right) E\left( Y\right)  = 0.
$$

<table><tr><td>Y</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>$P$</td><td>0.15</td><td>0.5</td><td>0.35</td></tr></table>

所以

$$
E\left( {Y}^{2}\right)  = {0.5},
$$

$$
E\left( {{X}^{2}{Y}^{2}}\right)  = \mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}{x}_{i}^{2}{y}_{j}^{2}{p}_{ij} = {0.28}.
$$

所以

$\operatorname{Cov}\left( {{X}^{2},{Y}^{2}}\right)  = E\left( {{X}^{2}{Y}^{2}}\right)  - E\left( {X}^{2}\right) E\left( {Y}^{2}\right)  =  - {0.02}.$ 故应填 0; 一 0.02 。

【3.2】已知 $X \sim  \left\lbrack  \begin{matrix}  - 1 & 1 \\  \frac{1}{2} & \frac{1}{2} \end{matrix}\right\rbrack , Y \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  \frac{1}{4} & \frac{3}{4} \end{matrix}\right\rbrack , P\{ X = Y\}  = \frac{1}{4}$,则 ${\rho }_{XY} =$ _____.

解 由 $P\{ X = Y\}  = P\{ X = 1, Y = 1\}  = \frac{1}{4}$,可求得 $\left( {X, Y}\right)$ 联合分布律

<table><tr><td>$Y$</td><td>0</td><td>1</td></tr><tr><td>-1</td><td>0</td><td>$\frac{1}{2}$</td></tr><tr><td>1</td><td>$\frac{1}{4}$</td><td>$\frac{1}{4}$</td></tr></table>

故 $E\left( {XY}\right)  =  - \frac{1}{4}$,又

$$
{EX} = 0,\;{DX} = 1,\;{EY} = \frac{3}{4},\;{DY} = \frac{3}{16},
$$

则 ${\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{DX} \cdot  \sqrt{DY}} = \frac{E\left( {XY}\right)  - {EX} \cdot  {EY}}{\sqrt{DX} \cdot  \sqrt{DY}} =  - \frac{\sqrt{3}}{3}$.

【3.3】设随机变量 $\left( {X, Y}\right)$ 具有概率密度函数

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{8}\left( {x + y}\right), & 0 \leq  x \leq  2,0 \leq  y \leq  2 \\  0, & \text{ 其他 } \end{array}\right.
$$

求 $E\left( X\right), E\left( Y\right),\operatorname{Cov}\left( {X, Y}\right),{\rho }_{XY}, D\left( {X + Y}\right)$.

解 由于

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{2}\mathrm{\;d}x{\int }_{0}^{2}\frac{1}{8}x\left( {x + y}\right) \mathrm{d}y = \frac{7}{6}
$$

$$
E\left( Y\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{yf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{2}\mathrm{\;d}x{\int }_{0}^{2}\frac{1}{8}y\left( {x + y}\right) \mathrm{d}y = \frac{7}{6}
$$

$$
E\left( {X}^{2}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{x}^{2}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{2}\mathrm{\;d}x{\int }_{0}^{2}\frac{1}{8}{x}^{2}\left( {x + y}\right) \mathrm{d}y = \frac{10}{6}
$$

同理 $E\left( {Y}^{2}\right)  = \frac{10}{6}$ 故

$$
D\left( X\right)  = E\left( {X}^{2}\right)  - {\left( EX\right) }^{2} = \frac{10}{6} - \frac{49}{36} = \frac{11}{36}.
$$

同理 ${DY} = \frac{11}{36}$.

$E\left( {XY}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xyf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{2}\mathrm{\;d}x{\int }_{0}^{2}\frac{1}{8}{xy}\left( {x + y}\right) \mathrm{d}y = \frac{8}{6}$

故

$$
\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - {EX} \cdot  {EY} = \frac{8}{6} - \frac{49}{36} =  - \frac{1}{36}
$$

$$
{\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{DX} \cdot  \sqrt{DY}} =  - \frac{\frac{1}{36}}{\sqrt{\frac{11}{36} \cdot  \frac{11}{36}}} =  - \frac{1}{11}
$$

$$
D\left( {X + Y}\right)  = {DX} + {DY} + 2\operatorname{Cov}\left( {X, Y}\right)  = \frac{11}{36} + \frac{11}{36} - \frac{2}{36} = \frac{5}{9}.
$$

【3.4】某箱装有 100 件产品,其中一、二和三等品分别为 80、10 和 10 件,现在从中随机抽取一件, 记

$$
{X}_{i} = \left\{  {\begin{array}{ll} 1, & \text{ 若抽到 }i\text{ 等品 } \\  0, & \text{ 其他 } \end{array}\;\left( {i = 1,2,3}\right) }\right.
$$

试求 (1) 随机变量 ${X}_{1}$ 和 ${X}_{2}$ 的联合分布;

(2)随机变量 ${X}_{1}$ 与 ${X}_{2}$ 的相关系数 $\rho$.

解 (1) 设事件 ${A}_{i} =$ “抽到 $i$ 等品” $\left( {i = 1,2,3}\right)$. 由题意知 ${A}_{1},{A}_{2},{A}_{3}$ 两两互不相容.

$P\left( {A}_{1}\right)  = {0.8},\;P\left( {A}_{2}\right)  = P\left( {A}_{3}\right)  = {0.1}.$

易见,

$P\left\{  {{X}_{1} = 0,{X}_{2} = 0}\right\}   = P\left( {A}_{3}\right)  = {0.1},$

$P\left\{  {{X}_{1} = 0,{X}_{2} = 1}\right\}   = P\left( {A}_{2}\right)  = {0.1};$

$P\left\{  {{X}_{1} = 1,{X}_{2} = 0}\right\}   = P\left( {A}_{1}\right)  = {0.8},$

$P\left\{  {{X}_{1} = 1,{X}_{2} = 1}\right\}   = P\left( \varnothing \right)  = 0.$

故 ${X}_{1}$ 和 ${X}_{2}$ 的联合分布为

<table><tr><td>${X}_{1}$ ${X}_{2}$</td><td>0</td><td>1</td></tr><tr><td>0</td><td>0.1</td><td>0.8</td></tr><tr><td>1</td><td>0.1</td><td>0</td></tr></table>

(2) $E{X}_{1} = {0.8},\;E{X}_{2} = {0.1}$,

$D{X}_{1} = {0.8} \times  {0.2} = {0.16},\;D{X}_{2} = {0.1} \times  {0.9} = {0.09},$

$E\left( {{X}_{1}{X}_{2}}\right)  = 0 \times  0 \times  {0.1} + 0 \times  1 \times  {0.1} + 1 \times  0 \times  {0.8} + 1 \times  1 \times  0 = 0,$

$\operatorname{Cov}\left( {{X}_{1},{X}_{2}}\right)  = E\left( {{X}_{1}{X}_{2}}\right)  - E{X}_{1} \cdot  E{X}_{2} = 0 - {0.8} \times  {0.1} =  - {0.08},$

$\rho  = \frac{\operatorname{Cov}\left( {{X}_{1},{X}_{2}}\right) }{\sqrt{D{X}_{1} \cdot  D{X}_{2}}} = \frac{-{0.08}}{\sqrt{{0.16} \times  {0.09}}} =  - \frac{2}{3}.$

#### 题型 2. 关于重要性质及结论

【3.5】设随机变量 $X$ 和 $Y$ 的的相关系数为 0.5, ${EX} = {EY} = 0, E{X}^{2} = E{Y}^{2} = 2$,则 $E{\left( X + Y\right) }^{2} =$ _____.

解法一 由已知条件 ${EX} = {EY} = 0, E{X}^{2} = E{Y}^{2} = 2$,得到,

${DX} = E{X}^{2} - {\left( EX\right) }^{2} = 2$

同理 ${DY} = 2$. 所以

$\operatorname{Cov}\left( {X, Y}\right)  = {\rho }_{XY}\sqrt{DX}\sqrt{DY} = {0.5} \times  2 = 1,$

因此概率论与数理统计习题精选精解

$E{\left( X + Y\right) }^{2} = D\left( {X + Y}\right)  + {\left\lbrack  E\left( X + Y\right) \right\rbrack  }^{2} = D\left( {X + Y}\right)  + {\left( EX + EY\right) }^{2}.$

由 ${EX},{EY} = 0$,得

$$
E{\left( X + Y\right) }^{2} = D\left( {X + Y}\right)  = {DX} + {DY} + 2\operatorname{Cov}\left( {X, Y}\right)  = 2 + 2 + 2 \times  1 = 6.
$$

解法二 $E{\left( X + Y\right) }^{2} = E{X}^{2} + {2E}\left( {XY}\right)  + E{Y}^{2} = 4 + 2\left\lbrack  {\operatorname{Cov}\left( {X, Y}\right)  + {EX} \cdot  {EY}}\right\rbrack$

$= 4 + 2{\rho }_{XY}\sqrt{DX}\sqrt{DY} = 4 + 2 \times  {0.5} \times  2 = 6$.

【3.6】设随机变量 ${X}_{1},{X}_{2},\cdots,{X}_{n}\left( {n > 1}\right)$ 独立同分布,且其方差为 ${\sigma }^{2} > 0$. 令 $Y = \frac{1}{n}$ $\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}$,则_____.

(A) $\operatorname{Cov}\left( {{X}_{1}, Y}\right)  = \frac{{\sigma }^{2}}{n}$ (B) $\operatorname{Cov}\left( {{X}_{1}, Y}\right)  = {\sigma }^{2}$

(C) $D\left( {{X}_{1} + Y}\right)  = \frac{n + 2}{n}{\sigma }^{2}$ (D) $D\left( {{X}_{1} - Y}\right)  = \frac{n + 1}{n}{\sigma }^{2}$

解 本题用方差和协方差的运算性质直接计算即可, 注意利用独立性有:

$$
\operatorname{Cov}\left( {{X}_{1},{X}_{i}}\right)  = 0,\;i = 2,3,\cdots, n
$$

$$
\operatorname{Cov}\left( {{X}_{1}, Y}\right)  = \operatorname{Cov}\left( {{X}_{1},\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}}\right)  = \frac{1}{n}\operatorname{Cov}\left( {{X}_{1},{X}_{1}}\right)  + \frac{1}{n}\mathop{\sum }\limits_{{i = 2}}^{n}\operatorname{Cov}\left( {{X}_{1},{X}_{i}}\right)
$$

$$
= \frac{1}{n}D{X}_{1} = \frac{1}{n}{\sigma }^{2}.
$$

本题 (C), (D) 两个选项的方差也直接计算得到: 如

$$
D\left( {{X}_{1} + Y}\right)  = D\left( {\frac{1 + n}{n}{X}_{1} + \frac{1}{n}{X}_{2} + \cdots  + \frac{1}{n}{X}_{n}}\right)  = \frac{{\left( 1 + n\right) }^{2}}{{n}^{2}}{\sigma }^{2} + \frac{n - 1}{{n}^{2}}{\sigma }^{2}
$$

$$
= \frac{{n}^{2} + {3n}}{{n}^{2}}{\sigma }^{2} = \frac{n + 3}{n}{\sigma }^{2},
$$

$$
D\left( {{X}_{1} - Y}\right)  = D\left( {\frac{n - 1}{n}{X}_{1} - \frac{1}{n}{X}_{2} - \cdots  - \frac{1}{n}{X}_{n}}\right)  = \frac{{\left( n - 1\right) }^{2}}{{n}^{2}}{\sigma }^{2} + \frac{n - 1}{{n}^{2}}{\sigma }^{2}
$$

$$
= \frac{{n}^{2} - n}{{n}^{2}}{\sigma }^{2} = \frac{n - 1}{n}{\sigma }^{2}.
$$

故应选 (A).

【3.7】将一枚硬币重复掷 $n$ 次,以 $X$ 和 $Y$ 分别表示正面向上和反面向上的次数,则 $X$ 和 $Y$ 的相关系数等于_____.

(A) -1 (B) 0 (C) $\frac{1}{2}$ (D) 1

分析 根据本题的特点可通过相关系数的性质 “ $Y = {aX} + b \Rightarrow  \left| {\rho }_{XY}\right|  = 1$ ” 求相关系数,亦可利用公式来求.

解法一 由题意可知 $X$ 和 $Y$ 的函数关系,即

$$
X + Y = n,
$$

又可表示为

$$
Y =  - X + n.
$$

易知 $Y$ 与 $X$ 之间存在线性关系为负相关,

故 ${\rho }_{XY} =  - 1$. 解法二 利用相关系数公式计算.

$$
\operatorname{Cov}\left( {X, Y}\right)  = \operatorname{Cov}\left( {X, n - X}\right)  = \operatorname{Cov}\left( {X, n}\right)  - \operatorname{Cov}\left( {X, X}\right),
$$

由 $\operatorname{Cov}\left( {X, n}\right)  = 0$,得

$$
\operatorname{Cov}\left( {X, Y}\right)  =  - \operatorname{Cov}\left( {X, X}\right)  =  - D\left( X\right).
$$

又由方差性质知 $D\left( Y\right)  = D\left( {-X + n}\right)  = D\left( X\right)$,所以

$$
{\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }} = \frac{-D\left( X\right) }{D\left( X\right) } =  - 1.
$$

故应选 (A). 【3.8】设随机变量 $X$ 和 $Y$ 的相关系数为 0.9,若 $Z = X - {0.4}$,则 $Y$ 与 $Z$ 的相关系数为 _____.

解 由于 ${DZ} = D\left( {X - {0.4}}\right)  = {DX}$,而

$$
\operatorname{Cov}\left( {Y, Z}\right)  = \operatorname{Cov}\left( {Y, X - {0.4}}\right)  = \operatorname{Cov}\left( {Y, X}\right),
$$

因此

$$
{\rho }_{YZ} = \frac{\operatorname{Cov}\left( {Y, Z}\right) }{\sqrt{D\left( Y\right) }\sqrt{D\left( Z\right) }} = \frac{\operatorname{Cov}\left( {Y, X}\right) }{\sqrt{D\left( Y\right) }\sqrt{D\left( X\right) }} = {\rho }_{YX} = {0.9}.
$$

点评 本题也可利用重要结论直接得出: 由于 ${\rho }_{{aX} + b,{cY} + d} = {\rho }_{X, Y}$ (当 $a, c$ 同号时),故

$$
{\rho }_{Y, Z} = {\rho }_{Y, X - {0.4}} = {\rho }_{Y, X} = {0.9}.
$$

【3.9】随机变量 $\left( {X, Y}\right)  \sim  N\left( {0,1;0,4;\rho }\right), D\left( {{2X} - Y}\right)  = 1$,则 $\rho  =$ _____.

解 因为 $\left( {X, Y}\right)  \sim  N\left( {0,1;0,4;\rho }\right)$,故

$$
{EX} = 0,\;{DX} = 1,\;{EY} = 0,\;{DY} = 4.
$$

而 $D\left( {{2X} - Y}\right)  = {4DX} + {DY} - 4\operatorname{Cov}\left( {X, Y}\right)  = 1$,因此

$$
\operatorname{Cov}\left( {X, Y}\right)  = \frac{7}{4},
$$

则

$$
{\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) } \cdot  \sqrt{D\left( Y\right) }} = \frac{\frac{7}{4}}{2} = \frac{7}{8}.
$$

故应填 $\frac{7}{8}$.

【3. 10】已知随机变量 $X$ 和 $Y$ 分别服从正态分布 $N\left( {1,{3}^{2}}\right)$ 和 $N\left( {0,{4}^{2}}\right)$,且 $X$ 与 $Y$ 的相关系数 ${\rho }_{XY} =  - \frac{1}{2}$. 设 $Z = \frac{X}{3} + \frac{Y}{2}$.

(1)求 $Z$ 的数学期望 ${EZ}$ 和方差 ${DZ}$;

(2)求 $X$ 与 $Z$ 的相关系数 ${\rho }_{XZ}$.

解 (1) ${EZ} = \frac{1}{3}{EX} + \frac{1}{2}{EY} = \frac{1}{3} + \frac{0}{2} = \frac{1}{3}$,

${DZ} = \frac{1}{{3}^{2}}{DX} + \frac{1}{{2}^{2}}{DY} + 2\operatorname{Cov}\left( {\frac{X}{3},\frac{Y}{2}}\right)$

$= \frac{{3}^{2}}{{3}^{2}} + \frac{{4}^{2}}{{2}^{2}} + 2\left( {-\frac{1}{2}}\right)  \cdot  \frac{3}{3} \cdot  \frac{4}{2} = 1 + 4 - 2 = 3.$

(2) $\operatorname{Cov}\left( {X, Z}\right)  = \frac{1}{3}\operatorname{Cov}\left( {X, X}\right)  + \frac{1}{2}\operatorname{Cov}\left( {X, Y}\right)  = \frac{1}{3} \cdot  {3}^{2} + \frac{1}{2}\left( {-\frac{1}{2}}\right)  \cdot  3 \cdot  4 = 0$.

所以 ${\rho }_{XZ} = \frac{\operatorname{Cov}\left( {X, Z}\right) }{\sqrt{D\left( X\right) } \cdot  \sqrt{D\left( Z\right) }} = 0$.

【3. 11】设 $X, Y$ 是随机变量,且有 $E\left( X\right)  = 3, E\left( Y\right)  = 1, D\left( X\right)  = 4, D\left( Y\right)  = 9$,令 $Z = {5X}$ $- Y + {15}$,分别在下列三种情况下求 $E\left( Z\right)$ 和 $D\left( Z\right)$.

(1) $X, Y$ 相互独立；

(2) $X, Y$ 不相关;

(3) $X$ 与 $Y$ 的相关系数为 0.25.

解 对于 $E\left( Z\right)$ : 在 (1),(2),(3) 三种情形下都有

$$
E\left( Z\right)  = E\left( {{5X} - Y + {15}}\right)  = {5E}\left( X\right)  - E\left( Y\right)  + {15} = {15} - 1 + {15} = {29}.
$$

对于 $D\left( Z\right)$ :

(1) $X, Y$ 独立,则

$$
D\left( Z\right)  = D\left( {{5X} - Y + {15}}\right)  = D\left( {5X}\right)  + D\left( Y\right)  = {25D}\left( X\right)  + D\left( Y\right)
$$

$$
= {25} \times  4 + 9 = {109}\text{.}
$$

(2) $X, Y$ 不相关,即 $\operatorname{Cov}\left( {X, Y}\right)  = 0$,

$$
D\left( Z\right)  = D\left( {5X}\right)  + D\left( Y\right)  = {109}.
$$

(3) ${\rho }_{XY} = {0.25}$,则 $\operatorname{Cov}\left( {X, Y}\right)  = {\rho }_{XY}\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) } = {1.5}$,

$$
D\left( Z\right)  = D\left( {{5X} - Y + {15}}\right)  = {25D}\left( X\right)  + D\left( Y\right)  - {10}\operatorname{Cov}\left( {X, Y}\right)
$$

$$
= {100} + 9 - {10} \times  {1.5} = {94}\text{.}
$$

#### 题型 3. 独立与不相关的判断

【3.12】设随机变量 $X$ 的概率分布密度为 $f\left( x\right)  = \frac{1}{2}{\mathrm{e}}^{-\left| x\right| }, - \infty  < x <  + \infty$.

(1)求 $X$ 的数学期望 $E\left( X\right)$ 和方差 $D\left( X\right)$.

(2)求 $X$ 与 $\left| X\right|$ 的协方差,并问 $X$ 与 $\left| X\right|$ 是否不相关？

(3) 问 $X$ 与 $\left| X\right|$ 是否相互独立？为什么？

解 (1) ${EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = 0$,

$$
{DX} = {\int }_{-\infty }^{+\infty }{x}^{2}f\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }{x}^{2}{\mathrm{e}}^{-x}\mathrm{\;d}x = 2.
$$

$$
\text{(2)}\operatorname{Cov}\left( {X,\left| X\right| }\right)  = E\left( {X\left| X\right| }\right)  - {EX} \cdot  E\left| X\right|  = E\left( {X\left| X\right| }\right)
$$

$$
= {\int }_{-\infty }^{+\infty }x\left| x\right| f\left( x\right) \mathrm{d}x = 0,
$$

故 $X$ 与 $\left| X\right|$ 不相关.

(3)对于给定 $0 < a <  + \infty$,显然事件 $\{ \left| X\right|  < a\}$ 包含在事件 $\{ X < a\}$ 内,且

$P\{ X < a\}  < 1,0 < P\{ \left| X\right|  < a\}$,故 $P\{ X < a,\left| X\right|  < a\}  = P\{ \left| X\right|  < a\}$,但

$$
P\{ X < a\}  \cdot  P\{ \left| X\right|  < a\}  < P\{ \left| X\right|  < a\},
$$

所以

$$
P\{ X < a,\left| X\right|  < a\}  \neq  P\{ X < a\}  \cdot  P\{ \left| X\right|  < a\},
$$

因此, $X$ 与 $\left| X\right|$ 不独立.

【3. 13】设随机变量 $X$ 和 $Y$ 都服从正态分布,且它们不相关,则_____.

(A) $X$ 与 $Y$ 一定独立

$\left( B\right) \left( {X, Y}\right)$ 服从二维正态分布

(C) $X$ 与 $Y$ 未必独立

(D) $X + Y$ 服从一维正态分布

解 只有当 $\left( {X, Y}\right)$ 服从二维正态分布时,不相关与独立才等价. 而本题仅知 $X$ 和 $Y$ 服从正态分布, 故 (A) 不正确. 从而 (B)、(D) 也不正确. 故应选(C).

【3.14】设二维随机变量 $\left( {X, Y}\right)$ 的联合概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} y{\mathrm{e}}^{-\left( {x + y}\right) }, & x, y > 0 \\  0, & \text{ 其他 } \end{array}\right.
$$

试求 $X, Y$ 是否相关,是否独立.

解 已知 $\left( {X, Y}\right)$ 联合密度为 $f\left( {x, y}\right)  = \left\{  \begin{array}{ll} y{\mathrm{e}}^{-\left( {x + y}\right) }, & x, y > 0 \\  0, & \text{ 其他 } \end{array}\right.$

所以

$$
{EX} = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{+\infty }\mathrm{d}y{\int }_{0}^{+\infty }{xy}{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}x = 1,
$$

${EY} = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{yf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{+\infty }\mathrm{d}x{\int }_{0}^{+\infty }{y}^{2}{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}y = 2,$

$E{X}^{2} = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{x}^{2}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{+\infty }\mathrm{d}y{\int }_{0}^{+\infty }{x}^{2}y{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}x = 2,$

$E{Y}^{2} = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{y}^{2}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{+\infty }\mathrm{d}x{\int }_{0}^{+\infty }{y}^{2}y{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}y = 6,$

故 ${DX} = E{X}^{2} - {\left( EX\right) }^{2} = 2 - 1 = 1$,

${DY} = E{Y}^{2} - {\left( EY\right) }^{2} = 6 - {2}^{2} = 2.$

因为 $E\left( {XY}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xyf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{+\infty }{\int }_{0}^{+\infty }{xy} \cdot  y{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}x\mathrm{\;d}y$

$= {\int }_{0}^{+\infty }x{\mathrm{e}}^{-x}\mathrm{\;d}x{\int }_{0}^{+\infty }{y}^{2}{\mathrm{e}}^{-y}\mathrm{\;d}y = 2,$

所以 $\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - \left( {EX}\right) \left( {EY}\right)  = 0$,

即得 ${\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{DX}\sqrt{DY}} = 0$,

故 $X$ 与 $Y$ 不相关.

下面判断独立性, 应用边缘密度和联合密度的关系.

由已知 $f\left( {x, y}\right)  = \left\{  \begin{array}{ll} y{\mathrm{e}}^{-\left( {x + y}\right) }, & x, y > 0 \\  0, & \text{ 其他 } \end{array}\right.$

所以 ${f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  \begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\right.$

$$
{f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = \left\{  \begin{array}{ll} y{\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0 \end{array}\right.
$$

所以 ${f}_{X}\left( x\right) {f}_{Y}\left( y\right)  = f\left( {x, y}\right)  = \left\{  \begin{array}{ll} y{\mathrm{e}}^{-\left( {x + y}\right) }, & x, y > 0 \\  0, & \text{ 其他 } \end{array}\right.$

因此 $X, Y$ 是相互独立的.

点评 本题也可以先判断出 $X, Y$ 相互独立,既然 $X, Y$ 相互独立,则 $X, Y$ 一定不相关. 这样可以减少计算量.

【3.15】设随机变量 $\left( {X, Y}\right)$ 的分布律为

<table><tr><td>$X$ Y</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>-1</td><td>$\frac{1}{8}$</td><td>$\frac{1}{8}$</td><td>$\frac{1}{8}$</td></tr><tr><td>0</td><td>$\frac{1}{8}$</td><td>0</td><td>$\frac{1}{8}$</td></tr><tr><td>1</td><td>$\frac{1}{8}$</td><td>$\frac{1}{8}$</td><td>$\frac{1}{8}$</td></tr></table>

验证 $X$ 和 $Y$ 是不相关的,但 $X$ 和 $Y$ 不是相互独立的.

证 由 $\left( {X, Y}\right)$ 的分布律得 $X$ 和 $Y$ 的边缘分布分别为

<table><tr><td>$X$-1</td><td>0</td><td>1</td></tr><tr><td>$p$$\frac{3}{8}$</td><td>$\frac{2}{8}$</td><td>$\frac{3}{8}$</td></tr></table>

<table><tr><td>Y</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>$p$</td><td>$\frac{3}{8}$</td><td>$\frac{2}{8}$</td><td>$\frac{3}{8}$</td></tr></table>

显然 $0 = P\{ X = 0, Y = 0\}  \neq  P\{ X = 0\} P\{ Y = 0\}  = \frac{2}{8} \times  \frac{2}{8}$

故 $X$ 和 $Y$ 不是相互独立的.

而

$E\left( X\right)  =  - 1 \times  \frac{3}{8} + 0 \times  \frac{2}{8} + 1 \times  \frac{3}{8} = 0$

$E\left( Y\right)  =  - 1 \times  \frac{3}{8} + 0 \times  \frac{2}{8} + 1 \times  \frac{3}{8} = 0$

$E\left( {XY}\right)  = \left( {-1}\right)  \times  \left( {-1}\right)  \times  \frac{1}{8} + \left( {-1}\right)  \times  1 \times  \frac{1}{8} + 1 \times  \left( {-1}\right)  \times  \frac{1}{8} + 1 \times  1 \times  \frac{1}{8} = 0$

所以 ${\rho }_{XY} = \frac{E\left( {XY}\right)  - E\left( X\right) E\left( Y\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }} = 0$.

从而 $X$ 与 $Y$ 是不相关的.

【3. 16】设 $A$ 和 $B$ 是试验 $E$ 的两个事件,且 $P\left( A\right)  > 0, P\left( B\right)  > 0$,并定义随机变量 $X, Y$ 如下:

$X = \left\{  {\begin{array}{ll} 1, & \text{ 若 }A\text{ 发生 } \\  0, & \text{ 若 }A\text{ 不发生 } \end{array},\;Y = \left\{  \begin{array}{ll} 1, & \text{ 若 }B\text{ 发生 } \\  0, & \text{ 若 }B\text{ 不发生 } \end{array}\right. }\right.$

证明若 ${\rho }_{XY} = 0$,则 $X$ 和 $Y$ 必定相互独立.

证 $X$ 和 $Y$ 的分布律分别为

<table><tr><td>$X$</td><td>1</td><td>0</td></tr><tr><td>$p$</td><td>$P\left( A\right)$</td><td>$P\left( \bar{A}\right)$</td></tr></table>

<table><tr><td/><td>1</td><td>0</td></tr><tr><td>$p$</td><td>$P\left( B\right)$</td><td>$P\left( \bar{B}\right)$</td></tr></table>

则 ${XY}$ 的分布律为

<table><tr><td>${XY}$</td><td>0</td></tr><tr><td/><td>$P\left( {AB}\right) \;1 - P\left( {AB}\right)$</td></tr></table>

从而

$$
E\left( X\right)  = P\left( A\right),\;E\left( Y\right)  = P\left( B\right),\;E\left( {XY}\right)  = P\left( {AB}\right).
$$

如果 ${\rho }_{XY} = 0$,有

$$
E\left( {XY}\right)  = E\left( X\right) E\left( Y\right),\;P\left( {AB}\right)  = P\left( A\right) \left( B\right),
$$

所以事件 $A$ 与 $B$ 是相互独立的. 由此事件 $A$ 与 $\bar{B},\bar{A}$ 与 $\bar{B},\bar{A}$ 与 $B$ 都是相互独立. 故得

$$
P\{ X = 1, Y = 1\}  = P\left( {AB}\right)  = P\left( A\right) P\left( B\right)  = P\{ X = 1\} P\{ Y = 1\}
$$

$$
P\{ X = 1, Y = 0\}  = P\left( {A\bar{B}}\right)  = P\left( A\right) P\left( \bar{B}\right)  = P\{ X = 1\} P\{ Y = 0\}
$$

$$
P\{ X = 0, Y = 1\}  = P\left( {\bar{A}B}\right)  = P\left( \bar{A}\right) P\left( B\right)  = P\{ X = 0\} P\{ Y = 1\}
$$

$$
P\{ X = 0, Y = 0\}  = P\left( {\bar{A}\bar{B}}\right)  = P\left( \bar{A}\right) P\left( \bar{B}\right)  = P\{ X = 0\} P\{ Y = 0\}
$$

因此 $X$ 与 $Y$ 是相互独立的.

#### 题型 4. 关于矩和协方差矩阵

【3.17】设随机变量 $X$ 在 $\left\lbrack  {a, b}\right\rbrack$ 上服从均匀分布,求 $X$ 的 $k$ 阶原点矩和三阶中心矩.

解 $E\left( {X}^{k}\right)  = {\int }_{a}^{b}{x}^{k}\frac{1}{b - a}\mathrm{\;d}x = {\left. \frac{1}{k + 1} \cdot  \frac{{x}^{k + 1}}{b - a}\right| }_{a}^{b} = \frac{1}{k + 1} \cdot  \frac{{b}^{k + 1} - {a}^{k + 1}}{b - a}$,

当 $k = 1$ 时,有 ${EX} = \frac{b + a}{2}$,故

$$
E{\left( X - EX\right) }^{3} = {\int }_{a}^{b}{\left( x - \frac{b + a}{2}\right) }^{3}\frac{1}{b - a}\mathrm{\;d}x = 0.
$$

【3. 18】设 $X \sim  N\left( {0,1}\right)$,求 $X$ 的 $k$ 阶原点矩及中心矩.

解 因为 ${EX} = \mu  = 0$,所以 $X$ 的原点矩及中心矩相同,即

$$
E{\left( X - EX\right) }^{k} = E\left( {X}^{k}\right)  = {\int }_{-\infty }^{+\infty }{x}^{k}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x = \frac{1}{\sqrt{2\pi }}{\int }_{-\infty }^{+\infty }{x}^{k}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x
$$

当 $k$ 为奇数时,上式积分中被积函数为奇函数,故

$$
E\left( {X}^{k}\right)  = 0
$$

当 $k$ 为偶数时,被积函数为偶函数,此时

$$
E\left( {X}^{k}\right)  = \sqrt{\frac{2}{\pi }}{\int }_{0}^{+\infty }{x}^{k}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x
$$

令 $y = \frac{{x}^{2}}{2}$,得

$$
E\left( {X}^{k}\right)  = \frac{1}{\sqrt{\pi }}{2}^{\frac{k}{2}}{\int }_{0}^{+\infty }{y}^{\frac{k - 1}{2}}{\mathrm{e}}^{-y}\mathrm{\;d}y = \frac{1}{\sqrt{\pi }}{2}^{\frac{k}{2}}\Gamma \left( \frac{k + 1}{2}\right)
$$

$$
= \left( {k - 1}\right) \left( {k - 3}\right) \cdots 3 \cdot  1\text{.}
$$

【3.19】设 $\left( {X, Y}\right)$ 的协方差矩阵为 $C = \left( \begin{matrix} 1 &  - 1 \\   - 1 & 9 \end{matrix}\right)$,求 ${\rho }_{XY}$.

解 由协方差矩阵的定义可知:

$$
\operatorname{Cov}\left( {X, Y}\right)  =  - 1,\;D\left( X\right)  = 1,\;D\left( Y\right)  = 9,
$$

则

$$
{\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }} = \frac{-1}{1 \cdot  \sqrt{9}} =  - \frac{1}{3}.
$$

## $§4$. 综合提高题型

#### 题型 1. 关于数字特征的判断与选择

【4.1】设随机变量 $X \sim  N\left( {0,1}\right), Y \sim  N\left( {1,4}\right)$ 且相关系数 ${\rho }_{XY} = 1$,则(   ).

(A) $P\{ Y =  - {2X} - 1\}  = 1$ (B) $P\{ Y = {2X} - 1\}  = 1$

(C) $P\{ Y =  - {2X} + 1\}  = 1$ (D) $P\{ Y = {2X} + 1\}  = 1$

解 由性质: ${\rho }_{XY} = 1 \Rightarrow  P\{ Y = {aX} + b\}  = 1,\left( {a > 0}\right)$. 可排除 (A),(C).

因为 $X \sim  N\left( {0,1}\right)$,所以

$$
{2X} - 1 \sim  N\left( {-1,4}\right),\;{2X} + 1 \sim  N\left( {1,4}\right)
$$

而 $Y \sim  N\left( {1,4}\right)$.

故应选 (D).

【4.2】设随机变量 $X$ 和 $Y$ 独立同分布,记 $U = X - Y, V = X + Y$,则随机变量 $U$ 与 $V$ 必然 (   ).

(A) 不独立 (B) 独立 (C) 相关系数不为零 (D) 相关系数为零

解 $\operatorname{Cov}\left( {U, V}\right)  = E\left( {UV}\right)  - \left\lbrack  {E\left( U\right) E\left( V\right) }\right\rbrack$

$$
= E\left( {{X}^{2} - {Y}^{2}}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} + {\left\lbrack  E\left( Y\right) \right\rbrack  }^{2}
$$

$$
= E\left( {X}^{2}\right)  - E\left( {Y}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} + {\left\lbrack  E\left( Y\right) \right\rbrack  }^{2}
$$

$$
= \left\lbrack  {E\left( {X}^{2}\right)  - {\left( EX\right) }^{2}}\right\rbrack   - \left\lbrack  {E\left( {Y}^{2}\right)  - {\left( EY\right) }^{2}}\right\rbrack   = D\left( X\right)  - D\left( Y\right)  = 0\text{,}
$$

所以

$$
{\rho }_{UV} = \frac{\operatorname{Cov}\left( {U, V}\right) }{\sqrt{D\left( U\right) } \cdot  \sqrt{D\left( V\right) }} = 0.
$$

故应选(D).

点评 当随机变量是线性函数时, 求协方差用性质较为方便:

$\operatorname{Cov}\left( {U, V}\right)  = \operatorname{Cov}\left( {X - Y, X + Y}\right)  = \operatorname{Cov}\left( {X, X}\right)  + \operatorname{Cov}\left( {X, Y}\right)  - \operatorname{Cov}\left( {X, Y}\right)  - \operatorname{Cov}\left( {Y, Y}\right)$

$= {DX} - {DY} = 0$.

【4.3】设二维随机变量 $\left( {X, Y}\right)$ 服从二维正态分布,则随机变量 $\xi  = X + Y$ 与 $\eta  = X - Y$ 不相关的充分必要条件为 (   ).

(A) $E\left( X\right)  = E\left( Y\right)$

(B) $E\left( {X}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} = E\left( {Y}^{2}\right)  - {\left\lbrack  E\left( Y\right) \right\rbrack  }^{2}$

(C) $E\left( {X}^{2}\right)  = E\left( {Y}^{2}\right)$

(D) $E\left( {X}^{2}\right)  + {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} = E\left( {Y}^{2}\right)  + {\left\lbrack  E\left( Y\right) \right\rbrack  }^{2}$

解 ${\rho }_{\xi,\eta } = 0 \Leftrightarrow  \operatorname{Cov}\left( {\xi,\eta }\right)  = 0$,即

$$
\operatorname{Cov}\left( {\xi,\eta }\right)  = {E\xi \eta } - {E\xi } \cdot  {E\eta } = E\left( {{X}^{2} - {Y}^{2}}\right)  - \left( {{EX} + {EY}}\right) \left( {{EX} - {EY}}\right)
$$

$$
= E{X}^{2} - E{Y}^{2} - {\left\lbrack  EX\right\rbrack  }^{2} + {\left\lbrack  EY\right\rbrack  }^{2} = 0\text{,}
$$

也即 $E{X}^{2} - {\left\lbrack  EX\right\rbrack  }^{2} = E{Y}^{2} - {\left\lbrack  EY\right\rbrack  }^{2}$.

故应选 (B).

【4.4】设随机变量 $X$ 和 $Y$ 的方差存在且不等于 0,则 $D\left( {X + Y}\right)  = {DX} + {DY}$ 是 $X$ 和 $Y$ (   ).

(A) 不相关的充分条件, 但不是必要条件

(B) 独立的必要条件, 但不是充分条件

(C) 不相关的充分必要条件

(D) 独立的充分必要条件

解 由公式 $D\left( {X + Y}\right)  = {DX} + {DY} + 2\operatorname{Cov}\left( {X, Y}\right)$

$D\left( {X + Y}\right)  = {DX} + {DY}$ 的充分必要条件是 $\operatorname{Cov}\left( {X, Y}\right)  = 0$.

故应选(C).

【4.5】设 $X$ 是一随机变量, ${EX} = \mu,{DX} = {\sigma }^{2}\left( {\mu,\sigma  > 0\text{常数}}\right)$,则对任意常数 $c$,必有(   ).

(A) $E{\left( X - c\right) }^{2} = E{X}^{2} - {c}^{2}$ (B) $E{\left( X - c\right) }^{2} = E{\left( X - \mu \right) }^{2}$

(C) $E{\left( X - c\right) }^{2} < E{\left( X - \mu \right) }^{2}$ (D) $E{\left( X - c\right) }^{2} \geq  E{\left( X - \mu \right) }^{2}$

解 由于 $E{\left( X - c\right) }^{2} = E{\left( X - \mu  + \mu  - c\right) }^{2} = E{\left( X - \mu \right) }^{2} + E{\left( \mu  - c\right) }^{2} + 2\left( {\mu  - c}\right) E\left( {X - \mu }\right)$

$= E{\left( X - \mu \right) }^{2} + {\left( \mu  - c\right) }^{2}$

即有 $E{\left( X - c\right) }^{2} \geq  E{\left( X - \mu \right) }^{2}$.

故应选(D).

点评 因为 ${DX} = E{\left( X - EX\right) }^{2} = E{\left( X - \mu \right) }^{2}$,所以如果考生对于常见不等式 ${DX} \leq  E{\left( X - c\right) }^{2}$ 比较熟悉的话可以直接选择(D).

【4.6】设随机变量 $X$ 与 $Y$ 相互独立,且 ${EX}$ 与 ${EY}$ 存在,记 $U = \max \{ X, Y\}, V = \min \{ X, Y\}$,则 $E\left( {UV}\right)  =$ _____.

(A) $E\mathrm{U} \cdot  E\mathrm{V}$ (B) ${EX} \cdot  {EY}$ (C) ${EU} \cdot  {EY}$ (D) ${EX} \cdot  {EV}$

解 由于 ${UV} = \max \{ X, Y\} \min \{ X, Y\}  = {XY},$

可知 $E\left( {UV}\right)  = E\left( {\max \{ X, Y\} \min \{ X, Y\} }\right)  = E\left( {XY}\right)  = E\left( X\right) E\left( Y\right)$.

故应选(B).

题型 2. 利用公式求数字特征

【4.7】设随机变量 $X$ 的分布律为

$$
P\{ X = k\}  = \frac{1}{1 + a}{\left( \frac{a}{1 + a}\right) }^{k},\;k = 0,1,2,\cdots
$$

其中 $a > 0$ 为常数,求 $E\left( X\right), D\left( X\right)$.

解法一 将 $X$ 的分布律改写为

$$
P\{ X = k\}  = p{q}^{k},\;k = 0,1,2,\cdots
$$

其中 $p = \frac{1}{1 + a}, q = \frac{a}{1 + a}$.

仿照几何分布的期望与方差计算方法可得:

$$
E\left( X\right)  = \mathop{\sum }\limits_{k}{kp}{q}^{k} = {pq}\mathop{\sum }\limits_{k}k{q}^{k - 1} = {pq}\mathop{\sum }\limits_{k}{\left( {q}^{k}\right) }^{\prime } = {pq}{\left( \frac{1}{1 - q}\right) }^{\prime } = \frac{q}{p} = a.
$$

同理可求 $D\left( X\right)  = E\left( {X}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} = \left( {1 + a}\right) a$.

解法二 直接利用几何分布的期望与方差计算结果.

设 $Y$ 服从参数为 $p$ 的几何分布. 则 $P\{ Y = k\}  = p{q}^{k - 1}, k = 1,2,\cdots$. 且

$$
E\left( Y\right)  = \frac{1}{p},\;D\left( Y\right)  = \frac{q}{{p}^{2}}.
$$

而 $X = Y - 1$,于是

$$
E\left( X\right)  = E\left( {Y - 1}\right)  = E\left( Y\right)  - 1 = \frac{1}{p} - 1 = a,
$$

$$
D\left( X\right)  = D\left( {Y - 1}\right)  = D\left( Y\right)  = \frac{q}{{p}^{2}} = a\left( {a + 1}\right).
$$

【4.8】设 $X \sim  P\left( \lambda \right)$,求 $E\left( \frac{1}{X + 1}\right)$.

解 因为 $X \sim  P\left( \lambda \right)$,故 $P\{ X = k\}  = \frac{{\lambda }^{k}{\mathrm{e}}^{-\lambda }}{k!}, k = 0,1,2,\cdots$

$$
E\left( \frac{1}{X + 1}\right)  = \mathop{\sum }\limits_{{k = 0}}^{\infty }\frac{1}{k + 1}P\{ X = k\}  = \mathop{\sum }\limits_{{k = 0}}^{\infty }\frac{1}{k + 1} \cdot  \frac{{\lambda }^{k}{\mathrm{e}}^{-\lambda }}{k!} = \mathop{\sum }\limits_{{k = 0}}^{\infty }\frac{{\lambda }^{k}{\mathrm{e}}^{-\lambda }}{\left( {k + 1}\right) !}
$$

$$
= \frac{{\mathrm{e}}^{-\lambda }}{\lambda }\mathop{\sum }\limits_{{k = 0}}^{\infty }\frac{{\lambda }^{k + 1}}{\left( {k + 1}\right) !} = \frac{{\mathrm{e}}^{-\lambda }}{\lambda }\mathop{\sum }\limits_{{n = 1}}^{\infty }\frac{{\lambda }^{n}}{n!} = \frac{{\mathrm{e}}^{-\lambda }}{\lambda }\left( {\mathop{\sum }\limits_{{n = 0}}^{\infty }\frac{{\lambda }^{n}}{n!} - 1}\right)
$$

$$
= \frac{{\mathrm{e}}^{-\lambda }}{\lambda }\left( {{\mathrm{e}}^{\lambda } - 1}\right)  = \frac{1}{\lambda }\left( {1 - {\mathrm{e}}^{-\lambda }}\right).
$$

【4.9】设 $\left( {X, Y}\right)$ 的分布律为

<table><tr><td>$X$ Y</td><td>1</td><td>2</td><td>3</td></tr><tr><td>-1</td><td>0.2</td><td>0.1</td><td>0</td></tr><tr><td>0</td><td>0.1</td><td>0</td><td>0.3</td></tr><tr><td>1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr></table>

(1) 求 $E\left( X\right), E\left( Y\right)$;

(2) 设 $Z = \frac{Y}{X}$,求 $E\left( Z\right)$.

解 (1) 由分布律得 $X$ 和 $Y$ 的边缘分布分别为

<table><tr><td>$X$</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$p$</td><td>0.4</td><td>0.2</td><td>0.4</td></tr></table>

<table><tr><td>$Y$</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>$p$</td><td>0.3</td><td>0.4</td><td>0.3</td></tr></table>

从而

$$
E\left( X\right)  = 1 \times  {0.4} + 2 \times  {0.2} + 3 \times  {0.4} = 2,
$$

$$
E\left( Y\right)  =  - 1 \times  {0.3} + 0 \times  {0.4} + 1 \times  {0.3} = 0.
$$

(2) $Z = \frac{Y}{X}$ 的分布律为

<table><tr><td>$Z$</td><td>-1</td><td>$- \frac{1}{2}$</td><td>$- \frac{1}{3}$</td><td>0</td><td>1</td><td>$\frac{1}{2}$</td><td>$\frac{1}{3}$</td></tr><tr><td>${p}_{k}$</td><td>0.2</td><td>0.1</td><td>0</td><td>0.4</td><td>0.1</td><td>0.1</td><td>0.1</td></tr></table>

$E\left( Z\right)  = \left( {-1}\right)  \times  {0.2} - \frac{1}{2} \times  {0.1} - \frac{1}{3} \times  0 + 0 \times  {0.4} + 1 \times  {0.1} + \frac{1}{2} \times  {0.1} + \frac{1}{3} \times  {0.1} =  - \frac{1}{15}.$

点评 第(2) 问可以直接利用公式

$$
E\left( Z\right)  = E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack   = \mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}g\left( {{x}_{i},{y}_{j}}\right) {p}_{ij},
$$

计算过程更加简便.

【4.10】假设随机变量 $U$ 在区间 $\left\lbrack  {-2,2}\right\rbrack$ 上服从均匀分布,随机变量

$$
X = \left\{  {\begin{matrix}  - 1, & \text{ 若 }U \leq   - 1 \\  1, & \text{ 若 }U >  - 1 \end{matrix}\;Y = \left\{  \begin{matrix}  - 1, & \text{ 若 }U \leq  1 \\  1, & \text{ 若 }U > 1 \end{matrix}\right. }\right.
$$

试求: (1) $X$ 和 $Y$ 的联合概率分布;

解 (1) 随机向量 $\left( {X, Y}\right)$ 有四个可能值: $\left( {-1, - 1}\right),\left( {-1,1}\right),\left( {1, - 1}\right),\left( {1,1}\right)$.

$$
P\{ X =  - 1, Y =  - 1\}  = P\{ U \leq   - 1, U \leq  1\}  = \frac{1}{4};
$$

$$
P\{ X =  - 1, Y = 1\}  = P\{ U \leq   - 1, U > 1\}  = 0;
$$

$$
P\{ X = 1, Y =  - 1\}  = P\{ U >  - 1, U \leq  1\}  = \frac{1}{2};
$$

$$
P\{ X = 1, Y = 1\}  = P\{ U >  - 1, U > 1\}  = \frac{1}{4}.
$$

于是,得 $X$ 和 $Y$ 的联合概率分布为

$$
\left( {X, Y}\right)  \sim  \left\lbrack  \begin{matrix} \left( {-1, - 1}\right) & \left( {-1,1}\right) & \left( {1, - 1}\right) & \left( {1,1}\right) \\  \frac{1}{4} & 0 & \frac{1}{2} & \frac{1}{4} \end{matrix}\right\rbrack .
$$

(2)利用公式 $E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack   = \mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}g\left( {{x}_{i},{y}_{j}}\right) {p}_{ij}$

$$
E\left( {X + Y}\right)  =  - \frac{2}{4} + \frac{2}{4} = 0,\;D\left( {X + Y}\right)  = E{\left( X + Y\right) }^{2} = 2.
$$

点评 $E\left( {X + Y}\right), D\left( {X + Y}\right)$ 也可以用性质计算.

【4.11】设随机变量 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} {2}^{-x}\ln 2, & x > 0, \\  0, & x \leq  0. \end{array}\right.
$$

对 $X$ 进行独立重复的观测,直到第 2 个大于 3 的观测值出现时停止,记 $Y$ 为观测次数.

(1)求 $Y$ 的概率分布；

(2) 求 ${EY}$.

解 (1) 每次观测中, 观测值大于 3 的概率为

$$
P\{ X > 3\}  = {\int }_{3}^{+\infty }f\left( x\right) \mathrm{d}x = {\int }_{3}^{+\infty }{2}^{-x}\ln 2\mathrm{\;d}x = \frac{1}{8},
$$

故 $Y$ 的概率分布为

$$
P\{ Y = k\}  = \left( {k - 1}\right) {\left( \frac{7}{8}\right) }^{k - 2}{\left( \frac{1}{8}\right) }^{2}, k = 2,3,\cdots.
$$

(2) ${EY} = \mathop{\sum }\limits_{{k = 2}}^{\infty }k\left( {k - 1}\right) {\left( \frac{7}{8}\right) }^{k - 2}{\left( \frac{1}{8}\right) }^{2}$

$= {\left. {\left( \frac{1}{8}\right) }^{2}{\left( \mathop{\sum }\limits_{{k = 2}}^{\infty }{x}^{k}\right) }^{\prime \prime }\right| }_{x = \frac{7}{8}}$

$= {\left. {\left( \frac{1}{8}\right) }^{2}\frac{2}{{\left( 1 - x\right) }^{3}}\right| }_{x = \frac{7}{8}}$

$= {16}$.

【4.12】设随机变量 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{matrix} a + b{x}^{2}, & 0 < x < 1 \\  0, & \text{ 其他 } \end{matrix}\right.
$$

已知 $E\left( X\right)  = \frac{3}{5}$,则 $D\left( X\right)  =$ _____.

解 由 $1 = {\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = {\int }_{0}^{1}\left( {a + b{x}^{2}}\right) \mathrm{d}x = a + \frac{1}{3}b$,得

$$
{3a} + b = 3
$$

①

再由 $\frac{3}{5} = {EX} = {\int }_{-\infty }^{+\infty }{xf}\left( x\right) \mathrm{d}x = {\int }_{0}^{1}\left( {{ax} + b{x}^{3}}\right) \mathrm{d}x = \frac{1}{2}a + \frac{1}{4}b$ 得

$$
{2a} + b = \frac{12}{5}
$$

②

联立 ①、② 两式解得 $a = \frac{3}{5}, b = \frac{6}{5}$,代入 $f\left( x\right)$ 表达式中即得

$$
{DX} = E{X}^{2} - {\left( EX\right) }^{2} = {\int }_{-\infty }^{+\infty }{x}^{2}f\left( x\right) \mathrm{d}x - {\left( \frac{3}{5}\right) }^{2}
$$

$$
= \frac{3}{5}{\int }_{0}^{1}{x}^{2}\left( {1 + 2{x}^{2}}\right) \mathrm{d}x - \frac{9}{25} = \frac{11}{25} - \frac{9}{25} = \frac{2}{25}\text{.}
$$

【4.13】设随机变量 $X$ 服从参数为 1 的指数分布,则数学期望 $E\left( {X + {\mathrm{e}}^{-{2X}}}\right)  =$ _____.

解 $X$ 服从参数为 1 的指数分布,即知 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

所以

$$
E\left( {X + {\mathrm{e}}^{-{2X}}}\right)  = {\int }_{-\infty }^{+\infty }\left( {x + {\mathrm{e}}^{-{2x}}}\right) f\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }\left( {x + {\mathrm{e}}^{-{2x}}}\right) {\mathrm{e}}^{-x}\mathrm{\;d}x
$$

$$
= {\int }_{0}^{+\infty }x{\mathrm{e}}^{-x}\mathrm{\;d}x + {\int }_{0}^{+\infty }{\mathrm{e}}^{-{3x}}\mathrm{\;d}x = 1 + \frac{1}{3} = \frac{4}{3}.
$$

【4. 14】设随机变量 $X$ 服从标准正态分布,即 $X \sim  N\left( {0,1}\right)$,则 $E\left( {X{\mathrm{e}}^{2X}}\right)  =$ _____.

解 标准正态分布的密度函数为

$$
f\left( x\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}},\; - \infty  < x <  + \infty,
$$

所以

$$
E\left( {X{\mathrm{e}}^{2X}}\right)  = {\int }_{-\infty }^{+\infty }x{\mathrm{e}}^{2x}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x = {\int }_{-\infty }^{+\infty }x\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2} + {2x}}\mathrm{\;d}x
$$

$$
= {\int }_{-\infty }^{+\infty }x\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{\left( x - 2\right) }^{2}}{2} + 2}\mathrm{\;d}x = {\mathrm{e}}^{2}{\int }_{-\infty }^{+\infty }x\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{\left( x - 2\right) }^{2}}{2}}\mathrm{\;d}x = 2{\mathrm{e}}^{2}.
$$

故应填 $2{\mathrm{e}}^{2}$.

【4.15】设随机变量 $\left( {X, Y}\right)$ 的概率分布为

<table><tr><td>$Y$ $X$</td><td>0</td><td>1</td><td>2</td></tr><tr><td>0</td><td>$\frac{1}{4}$</td><td>0</td><td>$\frac{1}{4}$</td></tr><tr><td>1</td><td>0</td><td>$\frac{1}{3}$</td><td>0</td></tr><tr><td>2</td><td>$\frac{1}{12}$</td><td>0</td><td>$\frac{1}{12}$</td></tr></table>

求 (1) $P\{ X = {2Y}\}$; (2) $\operatorname{Cov}\left( {X - Y, Y}\right)$.

解 (1) $P\{ X = {2Y}\}  = P\{ X = 2, Y = 1\}  + P\{ X = 0, Y = 0\}  = \frac{1}{4}$.

(2) $X$ 的边缘分布律

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td></tr><tr><td>$P$</td><td>$\frac{1}{2}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{6}$</td></tr></table>

$Y$ 的边缘分布律

<table><tr><td>$Y$</td><td>0</td><td>1</td><td>2</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td></tr></table>

$\operatorname{Cov}\left( {X - Y, Y}\right)  = \operatorname{Cov}\left( {X, Y}\right)  - D\left( Y\right)$

而 $\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - E\left( X\right) E\left( Y\right)$,

其中 $E\left( {XY}\right)  = 0 \times  \frac{7}{12} + 1 \times  \frac{1}{3} + 2 \times  0 + 4 \times  \frac{1}{12} = \frac{2}{3}$,

$E\left( X\right) E\left( Y\right)  = \left( {0 \times  \frac{1}{2} + 1 \times  \frac{1}{3} + 2 \times  \frac{1}{6}}\right)  \times  \left( {0 \times  \frac{1}{3} + 1 \times  \frac{1}{3} + 2 \times  \frac{1}{3}}\right)  = \frac{2}{3},$

可得 $\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - E\left( X\right) E\left( Y\right)  = \frac{2}{3} - \frac{2}{3} = 0$,

$D\left( Y\right)  = E\left( {Y}^{2}\right)  - {E}^{2}\left( Y\right)  = \left( {0 \times  \frac{1}{3} + {1}^{2} \times  \frac{1}{3} + {2}^{2} \times  \frac{1}{3}}\right)  - {\left( 0 \times  \frac{1}{3} + 1 \times  \frac{1}{3} + 2 \times  \frac{1}{3}\right) }^{2}$

$= \frac{2}{3}$,

可得 $\operatorname{Cov}\left( {X - Y, Y}\right)  = \operatorname{Cov}\left( {X, Y}\right)  - D\left( Y\right)  =  - \frac{2}{3}$.

【4.16】设随机变量 $X$ 和 $Y$ 的联合分布在以点 $\left( {0,1}\right),\left( {1,0}\right),\left( {1,1}\right)$ 为顶点的三角形区域上服从均匀分布. 试求随机变量 $Z = X + Y$ 的方差.

解法一 $\left( {X, Y}\right)$ 的联合密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} 2, & 0 \leq  x \leq  1,1 - x \leq  y \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

由随机变量函数期望公式

$$
E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack   = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }g\left( {x, y}\right) f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y
$$

可知,

$$
{EZ} = E\left( {X + Y}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }\left( {x + y}\right) f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}\mathrm{\;d}y{\int }_{1 - y}^{1}2\left( {x + y}\right) \mathrm{d}x
$$

$$
= {\int }_{0}^{1}\left( {{y}^{2} + {2y}}\right) \mathrm{d}y = \frac{4}{3},
$$

而

$$
E{Z}^{2} = E{\left( X + Y\right) }^{2} = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{\left( x + y\right) }^{2}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}\mathrm{\;d}y{\int }_{1 - y}^{1}2\left( {{x}^{2} + {2xy} + {y}^{2}}\right) \mathrm{d}x
$$

$$
= {\int }_{0}^{1}\left( {{2y} + 2{y}^{2} + \frac{3}{2}{y}^{3}}\right) \mathrm{d}y = \frac{11}{6},
$$

由方差的计算公式 ${DZ} = E{Z}^{2} - {\left( EZ\right) }^{2} = \frac{11}{6} - \frac{16}{9} = \frac{1}{18}$.

解法二 利用 $D\left( {X + Y}\right)  = {DX} + {DY} + 2\operatorname{Cov}\left( {X, Y}\right)$.

以 ${f}_{X}\left( x\right)$ 表示 $X$ 的概率密度,则当 $x \leq  0$ 或 $x \geq  1$ 时, ${f}_{X}\left( x\right)  = 0$; 当 $0 < x < 1$ 时,有

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = {\int }_{1 - x}^{1}2\mathrm{\;d}y = {2x},
$$

因此

$$
{EX} = {\int }_{0}^{1}2{x}^{2}\mathrm{\;d}x = \frac{2}{3},\;E{X}^{2} = {\int }_{0}^{1}2{x}^{3}\mathrm{\;d}x = \frac{1}{2},
$$

$$
{DX} = E{X}^{2} - {\left( EX\right) }^{2} = \frac{1}{2} - \frac{4}{9} = \frac{1}{18}.
$$

同理可得 ${EY} = \frac{2}{3},{DY} = \frac{1}{18}$.

现在求 $X$ 和 $Y$ 的协方差

$$
E\left( {XY}\right)  = {\iint }_{G}{2xy}\mathrm{\;d}x\mathrm{\;d}y = 2{\int }_{0}^{1}x\mathrm{\;d}x{\int }_{1 - x}^{1}y\mathrm{\;d}y = \frac{5}{12}
$$

$$
\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - {EX} \cdot  {EY} = \frac{5}{12} - \frac{4}{9} =  - \frac{1}{36},
$$

于是

$$
{DZ} = D\left( {X + Y}\right)  = {DX} + {DY} + 2\operatorname{Cov}\left( {X, Y}\right)  = \frac{1}{18} + \frac{1}{18} - \frac{2}{36} = \frac{1}{18}.
$$

解法三 由于 $X, Y$ 服从均匀分布,所以当 $z < 1$ 时, $F\left( z\right)  = 0$;

当 $z > 2$ 时, $F\left( z\right)  = 1$;

当 $1 \leq  z \leq  2$ 时, $F\left( z\right)  = P\{ X + Y \leq  z\}  = \frac{{S}_{D}{}^{\prime }}{{S}_{D}}$,

因为 ${S}_{D}{}^{\prime } = \frac{1}{2} - {S}_{\Delta } = \frac{1}{2} - \frac{1}{2}{\left( 2 - z\right) }^{2},{S}_{D} = \frac{1}{2}$,

所以 $F\left( z\right)  = 1 - {\left( 2 - z\right) }^{2}$,

故 $f\left( z\right)  = {F}^{\prime }\left( z\right)  = \left\{  \begin{array}{ll} 2\left( {2 - z}\right), & 1 \leq  z \leq  2 \\  0, & \text{ 其他 } \end{array}\right.$

所以 $E\left( Z\right)  = \frac{4}{3}, E\left( {Z}^{2}\right)  = \frac{11}{6}$.

故 $D\left( Z\right)  = D\left( {X + Y}\right)  = E\left( {Z}^{2}\right)  - {\left( E\left( Z\right) \right) }^{2} = \frac{1}{18}$.

点评 对本题而言, 解法一最为简洁.

【4.17】设 $\left( {X, Y}\right)$ 的概率密度为 $f\left( {x, y}\right)  = \left\{  \begin{array}{ll} {12}{y}^{2}, & 0 \leq  y \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.$

求 $E\left( X\right), E\left( Y\right), E\left( {XY}\right), E\left( {{X}^{2} + {Y}^{2}}\right)$.

解 $X$ 的概率密度为

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} {\int }_{0}^{x}{12}{y}^{2}\mathrm{\;d}y = 4{x}^{3}, & 0 \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

$Y$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {12}{y}^{2}\left( {1 - y}\right), & 0 \leq  y \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }x{f}_{X}\left( x\right) \mathrm{d}x = {\int }_{0}^{1}x \cdot  4{x}^{3}\mathrm{\;d}x = {\int }_{0}^{1}4{x}^{4}\mathrm{\;d}x = \frac{4}{5},
$$

$$
E\left( Y\right)  = {\int }_{-\infty }^{+\infty }y{f}_{Y}\left( y\right) \mathrm{d}y = {\int }_{0}^{1}y \cdot  {12}{y}^{2}\left( {1 - y}\right) \mathrm{d}y = {\int }_{0}^{1}{12}{y}^{3}\left( {1 - y}\right) \mathrm{d}y = \frac{3}{5},
$$

$$
E\left( {XY}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xyf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}{\int }_{0}^{x}{xy} \cdot  {12}{y}^{2}\mathrm{\;d}y\mathrm{\;d}x = {\int }_{0}^{1}3{x}^{5}\mathrm{\;d}x = \frac{1}{2}\text{,}
$$

$$
E\left( {{X}^{2} + {Y}^{2}}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }\left( {{x}^{2} + {y}^{2}}\right) f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}{\int }_{0}^{x}\left( {{x}^{2} + {y}^{2}}\right)  \cdot  {12}{y}^{2}\mathrm{\;d}y\mathrm{\;d}x
$$

$$
= {\int }_{0}^{1}\frac{32}{5}{x}^{5}\mathrm{\;d}x = \frac{32}{5} \times  \frac{1}{6} = \frac{16}{15}.
$$

点评 本题也可以不求 ${f}_{X}\left( x\right),{f}_{Y}\left( y\right)$,直接利用 $f\left( {x, y}\right)$ 求 $E\left( X\right), E\left( Y\right)$ :

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y,
$$

$$
E\left( Y\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{yf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y.
$$

【4.18】设两个随机变量 $X$ 、 $Y$ 相互独立,且都服从均值为 0,方差为 $\frac{1}{2}$ 的正态分布,求随机变量 $\left| {X - Y}\right|$ 的期望与方差.

解法一 按照一维变量的函数处理.

令 $Z = X - Y$,由于 $X \sim  N\left( {0,\frac{1}{2}}\right), Y \sim  N\left( {0,\frac{1}{2}}\right)$,且 $X$ 和 $Y$ 相互独立,故 $Z \sim  N\left( {0,1}\right)$.

$$
E\left( \left| {X - Y}\right| \right)  = E\left( \left| Z\right| \right)  = {\int }_{-\infty }^{+\infty }\left| z\right| \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{z}^{2}}{2}}\mathrm{\;d}z = \frac{2}{\sqrt{2\pi }}{\int }_{0}^{+\infty }z{\mathrm{e}}^{-\frac{{z}^{2}}{2}}\mathrm{\;d}z = \sqrt{\frac{2}{\pi }}
$$

因为

$$
D\left( \left| {X - Y}\right| \right)  = D\left( \left| Z\right| \right)  = E\left( {\left| Z\right| }^{2}\right)  - {\left\lbrack  E\left( \left| Z\right| \right) \right\rbrack  }^{2} = E\left( {Z}^{2}\right)  - {\left\lbrack  E\left( \left| Z\right| \right) \right\rbrack  }^{2}
$$

而 $E\left( {Z}^{2}\right)  = D\left( Z\right)  = 1$

所以 $D\left( \left| {X - Y}\right| \right)  = 1 - \frac{2}{\pi }$.

解法二 按照二维随机变量的函数处理.

利用公式

$$
E\left\lbrack  {g\left( {X, Y}\right) }\right\rbrack   = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }g\left( {x, y}\right) f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y,
$$

$E\left( \left| {X - Y}\right| \right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }\left| {x - y}\right| f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }\left| {x - y}\right|  \cdot  \frac{1}{\pi }{\mathrm{e}}^{-\left( {{x}^{2} + {y}^{2}}\right) }\mathrm{d}x\mathrm{\;d}y$

$= \sqrt{\frac{2}{\pi }}\;$ (利用极坐标计算)

$E\left( {\left| X - Y\right| }^{2}\right)  = E\left\lbrack  {\left( X - Y\right) }^{2}\right\rbrack   = D\left( {X - Y}\right)  + {\left\lbrack  E\left( X - Y\right) \right\rbrack  }^{2} = 1$

故 $D\left( \left| {X - Y}\right| \right)  = 1 - \frac{2}{\pi }$.

点评 解法一比解法二简便.

【4.19】设随机变量 $X$ 与 $Y$ 相互独立,且都服从参数为 1 的指数分布. 记

$$
U = \max \{ X, Y\}, V = \min \{ X, Y\}.
$$

(1)求 $V$ 的概率密度 ${f}_{V}\left( v\right)$;

(2) 求 $E\left( {U + V}\right)$.

解 (1) 因为 $X, Y$ 的分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

则 $V = \min \{ X, Y\}$ 的分布函数为

$$
{F}_{V}\left( v\right)  = 1 - {\left\lbrack  1 - F\left( v\right) \right\rbrack  }^{2} = \left\{  {\begin{matrix} 1 - {\mathrm{e}}^{-{2v}}, & v > 0 \\  0, & v \leq  0 \end{matrix},}\right.
$$

故 $V$ 的概率密度为

$$
{f}_{V}\left( v\right)  = {F}_{V}^{\prime }\left( v\right)  = \left\{  {\begin{matrix} 2{\mathrm{e}}^{-{2v}}, & v > 0 \\  0, & v \leq  0 \end{matrix}.}\right.
$$

( 2 )同理可求 $U = \max \{ X, Y\}$ 的概率密度为 ${f}_{U}\left( u\right)  = \left\{  \begin{matrix} 2\left( {1 - {\mathrm{e}}^{-u}}\right) {\mathrm{e}}^{-u}, & u > 0 \\  0, & u \leq  0 \end{matrix}\right.$,

故 $E\left( {U + V}\right)  = E\left( U\right)  + E\left( V\right)  = {\int }_{-\infty }^{+\infty }u{f}_{U}\left( u\right) \mathrm{d}u + {\int }_{-\infty }^{+\infty }v{f}_{V}\left( v\right) \mathrm{d}v = \frac{3}{2} + \frac{1}{2} = 2$.

或者 $U + V = \max \{ X, Y\}  + \min \{ X, Y\}  = X + Y$,

故 $E\left( {U + V}\right)  = E\left( {X + Y}\right)  = {EX} + {EY} = 2$.

【4.20】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} k\sin \left( {x + y}\right), & 0 \leq  x, y \leq  \frac{\pi }{2} \\  0, & \text{ 其他 } \end{array}\right.
$$

求 $k$ 值, $\operatorname{Cov}\left( {X, Y}\right)$ 和 ${\rho }_{XY}$.

解 由 ${\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = 1$,可知, ${\int }_{0}^{\frac{\pi }{2}}{\int }_{0}^{\frac{\pi }{2}}k\sin \left( {x + y}\right) \mathrm{d}x\mathrm{\;d}y = 1$,得 $k = \frac{1}{2}$.

因此, $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{2}\sin \left( {x + y}\right), & 0 \leq  x, y \leq  \frac{\pi }{2} \\  0, & \text{ 其他 } \end{array}\right.
$$

所以

$$
E\left( X\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{\frac{\pi }{2}}{\int }_{0}^{\frac{\pi }{2}}x \cdot  \frac{1}{2}\sin \left( {x + y}\right) \mathrm{d}x\mathrm{\;d}y = \frac{\pi }{4},
$$

$$
E\left( {X}^{2}\right)  = {\int }_{0}^{\frac{\pi }{2}}{\int }_{0}^{\frac{\pi }{2}}{x}^{2} \cdot  \frac{1}{2}\sin \left( {x + y}\right) \mathrm{d}x\mathrm{\;d}y = \frac{{\pi }^{2}}{8} + \frac{\pi }{2} - 2,
$$

$$
D\left( X\right)  = E\left( {X}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} = \frac{{\pi }^{2}}{16} + \frac{\pi }{2} - 2.
$$

同理可得

$$
E\left( Y\right)  = \frac{\pi }{4},\;D\left( Y\right)  = \frac{{\pi }^{2}}{16} + \frac{\pi }{2} - 2,
$$

$$
E\left( {XY}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xyf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{\frac{\pi }{2}}{\int }_{0}^{\frac{\pi }{2}}{xy} \cdot  \frac{1}{2}\sin \left( {x + y}\right) \mathrm{d}x\mathrm{\;d}y = \frac{\pi }{2} - 1.
$$

所以

$$
\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - E\left( X\right) E\left( Y\right)  = \frac{\pi }{2} - 1 - \frac{\pi }{4} \cdot  \frac{\pi }{4} = \frac{\pi }{2} - \frac{{\pi }^{2}}{16} - 1,
$$

因此 ${\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }} = \frac{\frac{\pi }{2} - \frac{{\pi }^{2}}{16} - 1}{\frac{{\pi }^{2}}{16} + \frac{\pi }{2} - 2} = \frac{{8\pi } - {\pi }^{2} - {16}}{{\pi }^{2} + {8\pi } - {32}}$.

【4.21】箱中装有 6 个球, 其中红、白、黑球的个数分别为 1, 2, 3 个. 现从箱中随机地取出 2 个球, 记 $X$ 为取出的红球个数, $Y$ 为取出的白球个数.

(1)求随机变量 $\left( {X, Y}\right)$ 的概率分布;

(2) 求 $\operatorname{Cov}\left( {X, Y}\right)$

解 (1) 随机变量 $\left( {X, Y}\right)$ 的概率分布为

<table><tr><td>Y $X$</td><td>0</td><td>1</td><td>2</td></tr><tr><td>0</td><td>$\frac{1}{5}$</td><td>$\frac{2}{5}$</td><td>$\frac{1}{15}$</td></tr><tr><td>1</td><td>$\frac{1}{5}$</td><td>$\frac{2}{15}$</td><td>0</td></tr></table>

(2) $P\{ X = 0\}  = \frac{2}{3},\;P\{ X = 1\}  = \frac{1}{3},\;{EX} = 0 \times  \frac{2}{3} + 1 \times  \frac{1}{3} = \frac{1}{3}$.

$P\{ Y = 0\}  = \frac{2}{5},\;P\{ Y = 1\}  = \frac{8}{15},\;P\{ Y = 2\}  = \frac{1}{15},$

${EY} = 0 \times  \frac{2}{5} + 1 \times  \frac{8}{15} + 2 \times  \frac{1}{15} = \frac{2}{3}.$

$E\left( {XY}\right)  = 1 \times  1 \times  \frac{2}{15} = \frac{2}{15}.$

$\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - {EX} \cdot  {EY} = \frac{2}{15} - \frac{1}{3} \times  \frac{2}{3} =  - \frac{4}{45}.$

【4.22】假设二维随机变量 $\left( {X, Y}\right)$ 在矩形 $G = \{ \left( {x, y}\right)  \mid  0 \leq  x \leq  2,0 \leq  y \leq  1\}$ 上服从均匀分布, 记

$$
U = \left\{  {\begin{array}{ll} 0, & \text{ 若 }X \leq  Y \\  1, & \text{ 若 }X > Y \end{array},\;V = \left\{  {\begin{array}{ll} 0, & \text{ 若 }X \leq  {2Y} \\  1, & \text{ 若 }X > {2Y} \end{array}.}\right. }\right.
$$

(1)求 $U$ 和 $V$ 的联合分布；

(2) 求 $U$ 和 $V$ 的相关系数 $\rho$.

解 由题设及图 4-4.22, 可得

$$
P\{ X \leq  Y\}  = \frac{1}{4},\;P\{ X > {2Y}\}  = \frac{1}{2},\;P\{ Y < X \leq  {2Y}\}  = \frac{1}{4}.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_173_626_1284_455_281_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_173_626_1284_455_281_0.jpg)

图 4-4.22

(1) $\left( {U, V}\right)$ 有四个可能值: $\left( {0,0}\right),\left( {0,1}\right),\left( {1,0}\right),\left( {1,1}\right)$.

$$
P\{ U = 0, V = 0\}  = P\{ X \leq  Y, X \leq  {2Y}\}  = P\{ X \leq  Y\}  = \frac{1}{4};
$$

$$
P\{ U = 0, V = 1\}  = P\{ X \leq  Y, X > {2Y}\}  = 0;
$$

$$
P\{ U = 1, V = 0\}  = P\{ X > Y, X \leq  {2Y}\}  = P\{ Y < X \leq  {2Y}\}  = \frac{1}{4};
$$

$$
P\{ U = 1, V = 1\}  = 1 - \left( {\frac{1}{4} + \frac{1}{4}}\right)  = \frac{1}{2}.
$$

(2)由以上可见 ${UV}$ 以及 $U$ 和 $V$ 的分布为

$$
{UV} \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  \frac{1}{2} & \frac{1}{2} \end{matrix}\right\rbrack ;\;U \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  \frac{1}{4} & \frac{3}{4} \end{matrix}\right\rbrack ,\;V \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  \frac{1}{2} & \frac{1}{2} \end{matrix}\right\rbrack .
$$

于是, 有

$$
{EU} = \frac{3}{4},\;{DU} = \frac{3}{16},\;{EV} = \frac{1}{2},\;{DV} = \frac{1}{4},\;E\left( {UV}\right)  = \frac{1}{2};
$$

$$
\operatorname{Cov}\left( {U, V}\right)  = E\left( {UV}\right)  - {EU} \cdot  {EV} = \frac{1}{8};
$$

$$
\rho  = \frac{\operatorname{Cov}\left( {U, V}\right) }{\sqrt{{DU} \cdot  {DV}}} = \frac{1}{\sqrt{3}}.
$$

【4.23】设 $X \sim  N\left( {0,1}\right)$,而 $Y = {X}^{n}$ ( $n$ 为正整数),求 ${\rho }_{XY}$.

解 因为 $X \sim  N\left( {0,1}\right)$,则 $E\left( X\right)  = 0, D\left( X\right)  = 1$. 另外当 $X \sim  N\left( {0,1}\right)$ 时,可利用分部积分法或者 $\Gamma$ 函数的公式得到下面结论:

$$
E\left( {X}^{{2n} + 1}\right)  = 0,
$$

$$
E\left( {X}^{2n}\right)  = \left( {{2n} - 1}\right) !! = \left( {{2n} - 1}\right) \left( {{2n} - 3}\right) \cdots \cdots 3 \cdot  1.
$$

故

$$
{\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{DX} \cdot  \sqrt{DY}} = \frac{E\left( {XY}\right)  - {EX} \cdot  {EY}}{\sqrt{DX} \cdot  \sqrt{DY}} = \frac{E\left( {X}^{n + 1}\right) }{\sqrt{D\left( {X}^{n}\right) }} = \frac{E\left( {X}^{n + 1}\right) }{\sqrt{E\left( {X}^{2n}\right)  - {\left( E{X}^{n}\right) }^{2}}}
$$

$= \left\{  \begin{array}{ll} 0, & \text{ 当 }n\text{ 为偶数时 } \\  \frac{n!!}{\sqrt{\left( {{2n} - 1}\right) !!}}, & \text{ 当 }n\text{ 为奇数时 } \end{array}\right.$

#### 题型 3. 利用性质求数字特征

【4.24】设随机变量 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$ 相互独立,且有 $E\left( {X}_{i}\right)  = i, D\left( {X}_{i}\right)  = 5 - i, i = 1,2,3,4$. 设 $Y = 2{X}_{1} - {X}_{2} + 3{X}_{3} - \frac{1}{2}{X}_{4}$. 求 $E\left( Y\right), D\left( Y\right)$.

解 $E\left( Y\right)  = E\left( {2{X}_{1} - {X}_{2} + 3{X}_{3} - \frac{1}{2}{X}_{4}}\right)  = {2E}\left( {X}_{1}\right)  - E\left( {X}_{2}\right)  + {3E}\left( {X}_{3}\right)  - \frac{1}{2}E\left( {X}_{4}\right)$

$$
= 2 \times  1 - 2 + 3 \times  3 - \frac{1}{2} \times  4 = 7.
$$

由于 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$ 相互独立,所以 $2{X}_{1},{X}_{2},3{X}_{3},\frac{1}{2}{X}_{4}$ 也相互独立,则

$$
D\left( Y\right)  = D\left( {2{X}_{1} - {X}_{2} + 3{X}_{3} - \frac{1}{2}{X}_{4}}\right)  = {4D}\left( {X}_{1}\right)  + D\left( {X}_{2}\right)  + {9D}\left( {X}_{3}\right)  + \frac{1}{4}D\left( {X}_{4}\right)
$$

$= 4 \times  \left( {5 - 1}\right)  + \left( {5 - 2}\right)  + 9 \times  \left( {5 - 3}\right)  + \frac{1}{4}\left( {5 - 4}\right)  = {37.25}$.

【4.25】设随机变量 $X, Y$ 不相关,且 ${EX} = 2,{EY} = 1,{DX} = 3$,则 $E\left\lbrack  {X\left( {X + Y - 2}\right) }\right\rbrack   =$ _____.

(A) -3 (B) 3 (C) -5 (D) 5

解 因为 $X, Y$ 不相关,所以

$$
\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - {EX} \cdot  {EY} = 0,
$$

即 $E\left( {XY}\right)  = {EX} \cdot  {EY}$,则

$$
E\left\lbrack  {X\left( {X + Y - 2}\right) }\right\rbrack   = E\left( {{X}^{2} + {XY} - {2X}}\right)  = E\left( {X}^{2}\right)  + E\left( {XY}\right)  - {2EX}
$$

$$
= \left\lbrack  {{DX} + {\left( EX\right) }^{2}}\right\rbrack   + {EX} \cdot  {EY} - {2EX} = 5\text{. 故应选 (D).}
$$

【4. 26】将 $n$ 只球 $\left( {1 \sim  n\text{号}}\right)$ 随机地放进 $n$ 只盒子 $\left( {1 \sim  n\text{号}}\right)$ 中去,一只盒子装一只球. 若一只球装入与球同号的盒子中,称为一个配对,记 $X$ 为总的配对数,求 $E\left( X\right)$.

解 引进随机变量

$$
{X}_{i} = \left\{  {\begin{array}{ll} 1, & \text{ 第 }i\text{ 号球恰装入第 }i\text{ 号盒子 } \\  0, & \text{ 第 }i\text{ 号球不是装入第 }i\text{ 号盒子 } \end{array}, i = 1,2,\cdots, n.}\right.
$$

则 $X = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i}, E\left( X\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}E\left( {X}_{i}\right)$,而 ${X}_{i}$ 显然服从 $\left( {0 - 1}\right)$ 分布,

$E\left( {X}_{i}\right)  = 1 \times  \frac{1}{n} = \frac{1}{n},$

从而 $E\left( X\right)  = \mathop{\sum }\limits_{{i = 1}}^{n}\frac{1}{n} = 1$.

【4.27】若有 $n$ 把看上去样子相同的钥匙,其中只有一把能打开门上的锁,用它们去试开门上的锁,设取到每只钥匙是等可能的,若每把钥匙试开一次后除去,试用下面两种方法求试开次数 $X$ 的期望:

(1)写出 $X$ 的分布律；

(2)不写出 $X$ 的分布律.

解 (1) 因为是不重复抽样,而取到每只钥匙是等可能的,故试开次数 $X$ 的分布律为

<table><tr><td>$X$</td><td>1</td><td>2</td><td>...</td><td>$i$</td><td>...</td><td>$n$</td></tr><tr><td>$p$</td><td>$\frac{1}{n}$</td><td>$\frac{1}{n}$</td><td>...</td><td>$\frac{1}{n}$</td><td>...</td><td>$\frac{1}{n}$</td></tr></table>

从而

$$
{EX} = \frac{1}{n} + \frac{2}{n} + \cdots  + \frac{i}{n} + \cdots  + \frac{n}{n} = \frac{1}{n}\left( {1 + \cdots  + n}\right)  = \frac{1}{2}\left( {n + 1}\right).
$$

(2)引进随机变量

$$
{X}_{i} = \left\{  {\begin{array}{ll} i, & \text{ 第 }i\text{ 把钥匙把门打开 } \\  0, & \text{ 第 }i\text{ 把钥匙未把门打开 } \end{array},\;i = 1,2,\cdots, n}\right.
$$

则试开次数

$$
X = \mathop{\sum }\limits_{{i = 1}}^{n}{X}_{i},\;{EX} = \mathop{\sum }\limits_{{i = 1}}^{n}E{X}_{i}
$$

而电 176

<table><tr><td>${X}_{i}$</td><td>$i$</td><td>0</td></tr><tr><td>$P$</td><td/><td>$1 - \frac{1}{n}$</td></tr></table>

故 $E{X}_{i} = \frac{i}{n}$

则 ${EX} = \mathop{\sum }\limits_{{i = 1}}^{n}\frac{i}{n} = \frac{n + 1}{2}$.

【4.28】设随机变量 ${X}_{1},{X}_{2}$ 的概率密度分别为

$$
{f}_{1}\left( x\right)  = \left\{  {\begin{array}{ll} 2{\mathrm{e}}^{-{2x}}, & x > 0 \\  0, & x \leq  0 \end{array},\;{f}_{2}\left( x\right)  = \left\{  \begin{array}{ll} 4{\mathrm{e}}^{-{4x}}, & x > 0 \\  0, & x \leq  0 \end{array}\right. }\right.
$$

(1)求 $E\left( {{X}_{1} + {X}_{2}}\right), E\left( {2{X}_{1} - 3{X}_{2}^{2}}\right)$;

(2)又设 ${X}_{1},{X}_{2}$ 相互独立,求 $E\left( {{X}_{1}{X}_{2}}\right)$.

解 (1) $E{X}_{1} = {\int }_{-\infty }^{+\infty }x \cdot  {f}_{1}\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }{2x}{\mathrm{e}}^{-{2x}}\mathrm{\;d}x = {\left. x{\mathrm{e}}^{-{2x}}\right| }_{0}^{+\infty } + {\int }_{0}^{+\infty }{\mathrm{e}}^{-{2x}}\mathrm{\;d}x = \frac{1}{2}$

$$
E{X}_{2} = {\int }_{-\infty }^{+\infty }x \cdot  {f}_{2}\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }{4x}{\mathrm{e}}^{-{4x}}\mathrm{\;d}x =  - {\left. x{\mathrm{e}}^{-{4x}}\right| }_{0}^{+\infty } + {\int }_{0}^{+\infty }{\mathrm{e}}^{-{4x}}\mathrm{\;d}x = \frac{1}{4}
$$

$$
E{X}_{2}^{2} = {\int }_{-\infty }^{+\infty }{x}^{2} \cdot  {f}_{2}\left( x\right) \mathrm{d}x = {\int }_{0}^{+\infty }4{x}^{2}{\mathrm{e}}^{-{4x}}\mathrm{\;d}x =  - {\left. {x}^{2}{\mathrm{e}}^{-{4x}}\right| }_{0}^{+\infty } + {\int }_{0}^{+\infty }{2x}{\mathrm{e}}^{-{4x}}\mathrm{\;d}x
$$

$$
=  - {\left. \frac{1}{2}x{\mathrm{e}}^{-{4x}}\right| }_{0}^{+\infty } + {\int }_{0}^{+\infty }\frac{1}{2}{\mathrm{e}}^{-{4x}}\mathrm{\;d}x = \frac{1}{8},
$$

所以

$$
E\left( {{X}_{1} + {X}_{2}}\right)  = E{X}_{1} + E{X}_{2} = \frac{1}{2} + \frac{1}{4} = \frac{3}{4},
$$

$$
E\left( {2{X}_{1} - 3{X}_{2}^{2}}\right)  = {2E}{X}_{1} - {3E}{X}_{2}^{2} = 2 \times  \frac{1}{2} - 3 \times  \frac{1}{8} = \frac{5}{8}.
$$

(2)由 ${X}_{1},{X}_{2}$ 相互独立,则

$$
E\left( {{X}_{1}{X}_{2}}\right)  = E{X}_{1} \cdot  E{X}_{2} = \frac{1}{2} \times  \frac{1}{4} = \frac{1}{8}.
$$

【4.29】已知三个随机变量 $X, Y, Z$ 中, $E\left( X\right)  = E\left( Y\right)  = 1, E\left( Z\right)  =  - 1, D\left( X\right)  = D\left( Y\right)  =$ $D\left( Z\right)  = 1,{\rho }_{XY} = 0,{\rho }_{XZ} = \frac{1}{2},{\rho }_{YZ} =  - \frac{1}{2}$,设 $W = X + Y + Z$,求 $E\left( W\right), D\left( W\right)$.

解 $E\left( W\right)  = E\left( {X + Y + Z}\right)  = {EX} + {EY} + {EZ} = 1$

$D\left( W\right)  = D\left( {X + Y + Z}\right)  = {DX} + {DY} + {DZ} + 2\operatorname{Cov}\left( {X, Y}\right)  + 2\operatorname{Cov}\left( {X, Z}\right)  + 2\operatorname{Cov}\left( {Y, Z}\right)$

而

$$
\operatorname{Cov}\left( {X, Y}\right)  = {\rho }_{XY}\sqrt{DX} \cdot  \sqrt{DY} = 0
$$

$$
\operatorname{Cov}\left( {X, Z}\right)  = {\rho }_{XZ}\sqrt{DX} \cdot  \sqrt{DZ} = \frac{1}{2}
$$

$$
\operatorname{Cov}\left( {Y, Z}\right)  = {\rho }_{YZ}\sqrt{DY} \cdot  \sqrt{DZ} =  - \frac{1}{2}
$$

故 $D\left( W\right)  = 3$.

【4. 30】设 $W = {\left( aX + 3Y\right) }^{2}, E\left( X\right)  = E\left( Y\right)  = 0, D\left( X\right)  = 4, D\left( Y\right)  = {16},{\rho }_{XY} =  - {0.5}$,求常数

$a$ 使 $E\left( W\right)$ 为最小,并求 $E\left( W\right)$ 的最小值.

解 根据 $D\left( X\right)  = E\left( {X}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2},\;D\left( Y\right)  = E\left( {Y}^{2}\right)  - {\left\lbrack  E\left( Y\right) \right\rbrack  }^{2}$,

$$
\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - E\left( X\right)  \cdot  E\left( Y\right),
$$

$$
{\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }}
$$

有 $E\left( W\right)  = E{\left( aX + 3Y\right) }^{2} = D\left( {{aX} + {3Y}}\right)  + {\left\lbrack  E\left( aX + 3Y\right) \right\rbrack  }^{2}$

$= {a}^{2}D\left( X\right)  + {9D}\left( Y\right)  + 2\operatorname{Cov}\left( {{aX},{3Y}}\right)  + {\left\lbrack  aE\left( X\right)  + 3E\left( Y\right) \right\rbrack  }^{2}$

$= {a}^{2}D\left( X\right)  + {9D}\left( Y\right)  + {6a}{\rho }_{XY}\sqrt{D\left( X\right)  \cdot  D\left( Y\right) }$

$= 4{a}^{2} + 9 \times  {16} + {6a}\left( {-{0.5}}\right) \sqrt{4 \times  {16}} = 4{a}^{2} - {24a} + {144}$

$= {\left( 2a - 6\right) }^{2} + {108} \geq  {108}$.

因此当 $a = 3$ 时, $E\left( W\right)$ 最小值为 108.

【4.31】设随机变量 $X \sim  N\left( {\mu,{\sigma }^{2}}\right), Y \sim  N\left( {\mu,{\sigma }^{2}}\right)$,且设 $X, Y$ 相互独立,试求 ${Z}_{1} = {\alpha X} + {\beta Y}$ 和 ${Z}_{2}$ $= {\alpha X} - {\beta Y}$ 的相关系数 (其中 $\alpha,\beta$ 是不为零的常数).

解 由于 $X, Y \sim  N\left( {\mu,{\sigma }^{2}}\right)$,可得

$$
{EX} = {EY} = \mu,{DX} = {DY} = {\sigma }^{2}
$$

${Z}_{1}$ 和 ${Z}_{2}$ 的相关系数:

$$
{\rho }_{{Z}_{1}{Z}_{2}} = \frac{\operatorname{Cov}\left( {{Z}_{1},{Z}_{2}}\right) }{\sqrt{D{Z}_{1}} \cdot  \sqrt{D{Z}_{2}}} = \frac{E\left( {{Z}_{1}{Z}_{2}}\right)  - E{Z}_{1} \cdot  E{Z}_{2}}{\sqrt{D{Z}_{1}} \cdot  \sqrt{D{Z}_{2}}}
$$

由 $E{Z}_{1} = E\left( {{\alpha X} + {\beta Y}}\right)  = {\alpha EX} + {\beta EY} = \left( {\alpha  + \beta }\right) \mu$

$$
E{Z}_{2} = E\left( {{\alpha X} - {\beta Y}}\right)  = {\alpha EX} - {\beta EY} = \left( {\alpha  - \beta }\right) \mu
$$

又

$E\left( {{Z}_{1}{Z}_{2}}\right)  = E\left( {{\alpha X} + {\beta Y}}\right) \left( {{\alpha X} - {\beta Y}}\right)  = E\left( {{\alpha }^{2}{X}^{2} - {\beta }^{2}{Y}^{2}}\right)  = {\alpha }^{2}E{X}^{2} - {\beta }^{2}E{Y}^{2}$

$$
= \left( {{\alpha }^{2} - {\beta }^{2}}\right) \left( {{\sigma }^{2} + {\mu }^{2}}\right)
$$

$$
D\left( {Z}_{1}\right)  = D\left( {{\alpha X} + {\beta Y}}\right)  = {\alpha }^{2}{DX} + {\beta }^{2}{DY} = \left( {{\alpha }^{2} + {\beta }^{2}}\right) {\sigma }^{2}
$$

$D\left( {Z}_{2}\right)  = D\left( {{\alpha X} - {\beta Y}}\right)  = \left( {{\alpha }^{2} + {\beta }^{2}}\right) {\sigma }^{2}$

于是

$$
{\rho }_{{Z}_{1}{Z}_{2}} = \frac{\left( {{\alpha }^{2} - {\beta }^{2}}\right) \left( {{\sigma }^{2} + {\mu }^{2}}\right)  - \left( {\alpha  + \beta }\right) \mu \left( {\alpha  - \beta }\right) \mu }{\sqrt{\left( {{\alpha }^{2} + {\beta }^{2}}\right) {\sigma }^{2}} \cdot  \sqrt{\left( {{\alpha }^{2} + {\beta }^{2}}\right) {\sigma }^{2}}} = \frac{\left( {{\alpha }^{2} - {\beta }^{2}}\right) {\sigma }^{2}}{\left( {{\alpha }^{2} + {\beta }^{2}}\right) {\sigma }^{2}} = \frac{{\alpha }^{2} - {\beta }^{2}}{{\alpha }^{2} + {\beta }^{2}}.
$$

点评 因为 $X$ 与 $Y$ 相互独立,所以利用性质求 $\operatorname{Cov}\left( {{Z}_{1},{Z}_{2}}\right)$ 更加简便.

$$
\operatorname{Cov}\left( {{Z}_{1},{Z}_{2}}\right)  = \operatorname{Cov}\left( {{\alpha X} + {\beta Y},{\alpha X} - {\beta Y}}\right)  = {\alpha }^{2}\operatorname{Cov}\left( {X, X}\right)  - {\beta }^{2}\operatorname{Cov}\left( {Y, Y}\right)
$$

$$
= {\alpha }^{2}D\left( X\right)  - {\beta }^{2}D\left( Y\right)  = \left( {{\alpha }^{2} - {\beta }^{2}}\right) {\sigma }^{2}.
$$

【4.32】将长度为 1m 的木棒随机地截成两段,则两段长度的相关系数为_____.

(A) 1 (B) $\frac{1}{2}$ (C) $- \frac{1}{2}$ (D) -1

解 设两段长度分别为 $X$ 和 $Y$,则 $Y = 1 - X$,利用相关系数的性质或者计算公式 ${\rho }_{XY} =$ $\frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{DX}\sqrt{DY}}$,可得相关系数为 -1.

故应选(D). 178

【4.33】设随机变量 $X$ 与 $Y$ 相互独立,且 $X \sim  N\left( {1,2}\right)$, $Y \sim  N\left( {1,4}\right)$,则 $D\left( {XY}\right)  =$ _____.

(A) 6 (B) 8 (C) 14 (D) 15

解 由方差计算公式以及 $X, Y$ 的独立性:

$$
P\left( {XY}\right)  = E\left\lbrack  {\left( XY\right) }^{2}\right\rbrack   - {\left\lbrack  E\left( XY\right) \right\rbrack  }^{2} = E\left( {{X}^{2}{Y}^{2}}\right)  - {\left( EX \cdot  EY\right) }^{2}
$$

$= E\left( {X}^{2}\right)  \cdot  E\left( {Y}^{2}\right)  - {\left( EX \cdot  EY\right) }^{2} = 3 \times  5 - 1 = {14}$.

故应选(C).

#### 题型 4. 关于重要分布的数字特征

【4.34】设随机变量 $X$ 服从参数为 1 的泊松分布,则 $P\left\{  {X = E{X}^{2}}\right\}   =$ _____.

解 因为 $X \sim  P\left( 1\right)$,故 ${EX} = {DX} = 1$,则

$$
E\left( {X}^{2}\right)  = {DX} + {\left( EX\right) }^{2} = 2.
$$

所以

$$
P\left\{  {X = E\left( {X}^{2}\right) }\right\}   = P\{ X = 2\}  = \frac{{1}^{2} \cdot  {\mathrm{e}}^{-1}}{2!} = \frac{1}{2\mathrm{e}}.
$$

【4.35】设随机变量 $X$ 的分布函数为 $F\left( x\right)  = {0.3\Phi }\left( x\right)  + {0.7\Phi }\left( \frac{x - 1}{2}\right)$,其中 $\Phi \left( x\right)$ 为标准正态分布函数,则 ${EX} =$ (   ).

(A) 0 (B) 0.3 (C) 0.7 (D) 1

解 因为 $F\left( x\right)  = {0.3\Phi }\left( x\right)  + {0.7\Phi }\left( \frac{x - 1}{2}\right)$,所以

$$
{F}^{\prime }\left( x\right)  = {0.3}{\Phi }^{\prime }\left( x\right)  + \frac{0.7}{2}{\Phi }^{\prime }\left( \frac{x - 1}{2}\right)  = {0.3}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{\frac{{x}^{2}}{2}} + {0.7}\frac{1}{2\sqrt{2\pi }}{\mathrm{e}}^{\frac{{\left( x - 1\right) }^{2}}{2 \times  {2}^{2}}},
$$

由于 $\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}$ 是 $N\left( {0,1}\right)$ 的密度函数,故其随机变量的期望为 0,

$\frac{1}{2\sqrt{2\pi }}{\mathrm{e}}^{\frac{{\left( x - 1\right) }^{2}}{2 \times  {2}^{2}}}$ 是 $N\left( {1,{2}^{2}}\right)$ 的密度函数,其随机变量的期望为 1,

所以

$$
{EX} = {\int }_{-\infty }^{+\infty }x{F}^{\prime }\left( x\right) \mathrm{d}x = {0.3} \times  0 + {0.7} \times  1 = {0.7},
$$

故选(C).

【4.36】设 $X$ 表示 10 次独立重复射击命中目标的次数,每次射中目标的概率为 0.4,则 ${X}^{2}$ 的数学期望 $E\left( {X}^{2}\right)  =$ _____.

分析 利用二项分布的方差和期望公式.

解 由于 $X$ 服从二项分布 $B\left( {{10},{0.4}}\right)$,所以

${DX} = {npq} = {10} \times  {0.4} \times  \left( {1 - {0.4}}\right)  = {2.4}$.

由方差公式 $E{X}^{2} = {DX} + {\left( EX\right) }^{2}$ 得,

$$
E{X}^{2} = {2.4} + {4}^{2} = {18.4}.
$$

【4.37】设随机变量 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{2}\cos \frac{x}{2}, & 0 \leq  x < \pi \\  0, & \text{ 其他 } \end{array}\right.
$$

对 $X$ 独立地重复观察 4 次,用 $Y$ 表示观察值大于 $\frac{\pi }{3}$ 的次数,求 ${Y}^{2}$ 的数学期望.

解法一 由于 $P\left\{  {X > \frac{\pi }{3}}\right\}   = {\int }_{\frac{\pi }{3}}^{\pi }\frac{1}{2}\cos \frac{x}{2}\mathrm{\;d}x = \frac{1}{2}, Y \sim  B\left( {4,\frac{1}{2}}\right)$,因此

$$
{EY} = 4 \times  \frac{1}{2} = 2,\;{DY} = 4 \times  \frac{1}{2} \times  \left( {1 - \frac{1}{2}}\right)  = 1,
$$

所以

$$
E{Y}^{2} = {DY} + {\left( EY\right) }^{2} = 1 + {2}^{2} = 5.
$$

解法二 由于 $P\left\{  {X > \frac{\pi }{3}}\right\}   = {\int }_{\frac{\pi }{3}}^{\pi }\frac{1}{2}\cos \frac{x}{2}\mathrm{\;d}x = \frac{1}{2}, Y \sim  B\left( {4,\frac{1}{2}}\right)$,

因此, $Y$ 的概率分布为

<table><tr><td>$Y$</td><td>0</td><td>1</td><td>2</td><td>3</td><td>4</td></tr><tr><td>$P$</td><td>$\frac{1}{16}$</td><td>$\frac{4}{16}$</td><td>$\frac{6}{16}$</td><td>$\frac{4}{16}$</td><td>$\frac{1}{16}$</td></tr></table>

所以

$E{Y}^{2} = \frac{1}{16}\left( {0 \times  1 + 1 \times  4 + {2}^{2} \times  6 + {3}^{2} \times  4 + {4}^{2} \times  1}\right)  = 5.$

【4.38】已知 $\left( {X, Y}\right)$ 服从二维正态分布 $N\left( {0,0;{1}^{2},{2}^{2};\frac{1}{2}}\right)$. 若 $Z = {aX} + Y$ 与 $Y$ 独立, 则 $a$ 等于(   ).

(A) 2 (B) -2 (C) 4 (D) -4

解 由题设 $\left( {X, Y}\right)  \sim  N\left( {0,0;1,4;\frac{1}{2}}\right),{EX} = {EY} = 0,{DX} = 1,{DY} = 4,{\rho }_{XY} = \frac{1}{2}$,

若 $Z$ 与 $Y$ 独立,则 $Z$ 与 $Y$ 不相关,即 $\operatorname{Cov}\left( {Z, Y}\right)  = 0$.

$\operatorname{Cov}\left( {Z, Y}\right)  = \operatorname{Cov}\left( {{aX} + Y, Y}\right)  = a\operatorname{Cov}\left( {X, Y}\right)  + {DY} = a{\rho }_{XY}\sqrt{DX}\sqrt{DY} + {DY}$

$= a \cdot  \frac{1}{2} \cdot  2 + 4 = 0 \Rightarrow  a =  - 4.$

故应选(D).

【4. 39】设 $X \sim  P\left( {16}\right), Y \sim  E\left( 2\right),{\rho }_{XY} =  - {0.5}$,则 $\operatorname{Cov}\left( {X, Y + 1}\right)  =$ _____, $E\left( {{Y}^{2} + {XY}}\right)$ $=$ _____, $D\left( {X - {2Y}}\right)  =$ _____.

解 由已知, ${EX} = {DX} = {16},{EY} = \frac{1}{2},{DY} = \frac{1}{4}$,则

$\operatorname{Cov}\left( {X, Y + 1}\right)  = \operatorname{Cov}\left( {X, Y}\right)  = {\rho }_{XY} \cdot  \sqrt{DX} \cdot  \sqrt{DY} =  - 1;$

$E\left( {{Y}^{2} + {XY}}\right)  = E\left( {Y}^{2}\right)  + E\left( {XY}\right)  = \left\lbrack  {{DY} + {\left( EY\right) }^{2}}\right\rbrack   + \left\lbrack  {\operatorname{Cov}\left( {X, Y}\right)  + {EX} \cdot  {EY}}\right\rbrack   = \frac{15}{2};$

$D\left( {X - {2Y}}\right)  = {DX} + {4DY} - 4\operatorname{Cov}\left( {X, Y}\right)  = {21}.$

【4.40】设一物体是圆截面,测量其直径,设其直径 $X$ 服从 $\left\lbrack  {0,3}\right\rbrack$ 上的均匀分布,则求横截面积 $Y$ 的数学期望和方差.

解 由题意可知甲 180

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{3}, & 0 \leq  x \leq  3 \\  0, & \text{ 其他 } \end{array}\right.
$$

利用均匀分布的数字特征公式,所以

$$
{EX} = \frac{3}{2},\;{DX} = \frac{3}{4}.
$$

由横截面积 $Y = \pi  \cdot  \frac{{X}^{2}}{4}$ 得,

$$
{EY} = \frac{\pi }{4}E{X}^{2} = \frac{\pi }{4}\left\lbrack  {{DX} + {\left( EX\right) }^{2}}\right\rbrack   = \frac{\pi }{4}\left( {\frac{3}{4} + \frac{9}{4}}\right)  = \frac{3}{4}\pi,
$$

$$
{DY} = E{Y}^{2} - {\left( EY\right) }^{2} = \frac{{\pi }^{2}}{16}E{X}^{4} - \frac{9}{16}{\pi }^{2} = \frac{{\pi }^{2}}{16}{\int }_{0}^{3}{x}^{4} \cdot  \frac{1}{3}\mathrm{\;d}x - \frac{9}{16}{\pi }^{2} = \frac{9}{20}{\pi }^{2}.
$$

【4.41】设二维随机变量 $\left( {X, Y}\right)$ 服从 $N\left( {\mu,\mu;{\sigma }^{2},{\sigma }^{2};0}\right)$,则 $E\left( {X{Y}^{2}}\right)  =$ _____.

解 由于 $\rho  = 0$,由二维正态分布的性质可知随机变量 $X, Y$ 独立.

因此 $E\left( {X{Y}^{2}}\right)  = {EX} \cdot  E{Y}^{2}$. 由于 $\left( {X, Y}\right)$ 服从 $N\left( {\mu,\mu;{\sigma }^{2},{\sigma }^{2};0}\right)$,可知 ${EX} = \mu, E{Y}^{2} = {DY} + {\left( EY\right) }^{2}$ $= {\mu }^{2} + {\sigma }^{2}$,则

$$
E\left( {X{Y}^{2}}\right)  = \mu \left( {{\mu }^{2} + {\sigma }^{2}}\right)  = {\mu }^{3} + \mu {\sigma }^{2}.
$$

故应填 ${\mu }^{3} + \mu {\sigma }^{2}$.

【4.42】一本 500 页的书共有 100 个错误,设每页上错误的个数为随机变量 $X$,已知它服从泊松分布, 现随机地取 1 页, 求下列事件的概率:

(1)该页上没有错误；

(2)这页上错误不少于 2 个.

解 因为 $X \sim  P\left( \lambda \right)$,故 ${EX} = \lambda$. 由题意可知每页上平均有 $\frac{1}{5}$ 个错误,即 ${EX} = \frac{1}{5}$,则 $\lambda  = \frac{1}{5}$.

(1) $P\{ X = 0\}  = \frac{{\left( \frac{1}{5}\right) }^{ \circ  }{\mathrm{e}}^{-\frac{1}{5}}}{0!} = {\mathrm{e}}^{-\frac{1}{5}}$.

(2) $P\{ X \geq  2\}  = 1 - P\{ X = 0\}  - P\{ X = 1\}  = 1 - \frac{6}{5}{\mathrm{e}}^{-\frac{1}{5}}$

或查表得 $P\{ X \geq  2\}  = {0.0175}$.

#### 题型 5. 数字特征应用题

【4.43】设某企业生产线上产品合格率为 0.96,不合格产品中只有 $\frac{3}{4}$ 产品可进行再加工,且再加工的合格率为 0.8,其余均为废品,每件合格品获利 80 元,每件废品亏损 20 元,为保证该企业每天平均利润不低于 2 万元, 问企业每天至少生产多少产品?

解法一 设每天至少生产 $x$ 件产品. 则合格产品为

$$
{0.96x} + \left( {1 - {0.96}}\right) x \cdot  \frac{3}{4} \cdot  {0.8} = {0.984x},
$$

废品为 $x - {0.984x} = {0.016x}$,由题意知

$$
{80} \times  {0.984x} - {20} \times  {0.016x} \geq  2 \times  {10}^{4},
$$

解得 $x \geq  {255.10}$, 概率论与数理统计习题精选精解

因为 $x$ 为整数,所以 $x = {256}$.

解法二 进行再加工后, 产品的合格率

$$
p = {0.96} + {0.04} \times  {0.75} \times  {0.8} = {0.984}.
$$

记 $X$ 为 $n$ 件产品中的合格产品数, $T\left( n\right)$ 为 $n$ 件产品的利润,则

$$
X \sim  B\left( {n, p}\right),
$$

$$
{EX} = {np} = {0.984n},
$$

$$
T\left( n\right)  = {80X} - {20}\left( {n - X}\right),
$$

$$
{ET}\left( n\right)  = {80}\mathrm{{EX}} - {20n} + {20}\mathrm{{EX}} = {100}\mathrm{{EX}} - {20n} = {78.4n}\text{,}
$$

要 ${ET}\left( n\right)  \geq  {20000}$,则 $n \geq  {256}$,即该企业每天至少应生产 256 件产品.

【4.44】一商店经销某种商品,每周进货的数量 $X$ 与顾客对该种商品的需求量 $Y$ 是相互独立的随机变量,且都服从区间 $\left\lbrack  {{10},{20}}\right\rbrack$ 上的均匀分布. 商店每售出一单位商品可得利润 1000 元; 若需求量超过了进货量,商店可从其他商店调剂供应,这时每单位商品获利润500元. 试计算此商店经销该种商品每周所得利润的期望值.

解 设 $Z$ 表示商店每周所得的利润,则

$$
Z = \left\{  \begin{array}{ll} {1000Y}, & Y \leq  X \\  {1000X} + {500}\left( {Y - X}\right)  = {500}\left( {X + Y}\right), & Y > X \end{array}\right.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_181_1040_699_303_286_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_181_1040_699_303_286_0.jpg)

图 4-4.44

由于 $X$ 与 $Y$ 的联合概率密度为:

$$
\varphi \left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{100}, & {10} \leq  x \leq  {20},{10} \leq  y \leq  {20} \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
E\left( Z\right)  = {\iint }_{{D}_{1}}{1000y} \times  \frac{1}{100}\mathrm{\;d}x\mathrm{\;d}y + {\iint }_{{D}_{2}}{500}\left( {x + y}\right)  \times  \frac{1}{100}\mathrm{\;d}x\mathrm{\;d}y
$$

$$
= {10}{\int }_{10}^{20}\mathrm{\;d}y{\int }_{y}^{20}y\mathrm{\;d}x + 5{\int }_{10}^{20}\mathrm{\;d}y{\int }_{10}^{y}\left( {x + y}\right) \mathrm{d}x
$$

$$
= {10}{\int }_{10}^{20}y\left( {{20} - y}\right) \mathrm{d}y + 5{\int }_{10}^{20}\left( {\frac{3}{2}{y}^{2} - {10y} - {50}}\right) \mathrm{d}y
$$

$$
= \frac{20000}{3} + 5 \times  {1500} \approx  {14166.67}\text{ (元). }
$$

【4.45】一工厂生产的某种设备的寿命 $X$ (以年计) 服从指数分布,概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{4}{\mathrm{e}}^{-\frac{x}{4}} & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

工厂规定, 出售的设备若在一年之内损坏可予以调换. 若工厂售出一台设备赢利 100 元, 调换一台设备厂方需花费 300 元. 试求厂方出售一台设备净赢利的数学期望.

解 出售的设备在售出一年之内调换的概率为

$$
{p}_{1} = P\{ X \leq  1\}  = {\int }_{0}^{1}f\left( x\right) \mathrm{d}x = {\int }_{0}^{1}\frac{1}{4}{\mathrm{e}}^{-\frac{x}{4}}\mathrm{\;d}x = 1 - {\mathrm{e}}^{-\frac{1}{4}}
$$

不需调换的概率为 ${p}_{2} = 1 - {p}_{1} = {\mathrm{e}}^{-\frac{1}{4}}$

记 $Y$ 为工厂出售一台设备的净赢利,则 $Y$ 的分布律为

<table><tr><td>$Y$</td><td>100</td><td>$- {300} + {100}$</td></tr><tr><td>$P$</td><td>${\mathrm{e}}^{-\frac{1}{4}}$</td><td>$1 - {\mathrm{e}}^{-\frac{1}{4}}$</td></tr></table>

从而厂方出售一台设备净赢利的数学期望

$$
E\left( Y\right)  = {100}{\mathrm{e}}^{-\frac{1}{4}} - {200}\left( {1 - {\mathrm{e}}^{-\frac{1}{4}}}\right)  = {33.64}.
$$

【4.46】某流水生产线上每个产品不合格的概率为 $p\left( {0 < p < 1}\right)$,各产品合格与否相互独立,当出现一个不合格产品时即停机检修. 设开机后第一次停机时已生产了的产品个数为 $X$,求 $X$ 的数学期望 $E\left( X\right)$ 和方差 $D\left( X\right)$.

解 记 $q = 1 - p, X$ 的概率分布为

$$
P\{ X = i\}  = {q}^{i - 1}p,\;i = 1,2,\cdots.
$$

$X$ 的数学期望为

$$
E\left( X\right)  = \mathop{\sum }\limits_{{i = 1}}^{\infty }i{q}^{i - 1}p = p\mathop{\sum }\limits_{{i = 1}}^{\infty }{\left( {q}^{i}\right) }^{\prime } = p{\left( \mathop{\sum }\limits_{{i = 1}}^{\infty }{q}^{i}\right) }^{\prime } = p{\left( \frac{q}{1 - q}\right) }^{\prime } = \frac{1}{p}.
$$

因为

$$
E\left( {X}^{2}\right)  = \mathop{\sum }\limits_{{i = 1}}^{\infty }{i}^{2}{q}^{i - 1}p = p{\left\lbrack  q{\left( \mathop{\sum }\limits_{{i = 1}}^{\infty }{q}^{i}\right) }^{\prime }\right\rbrack  }^{\prime } = p{\left\lbrack  \frac{q}{{\left( 1 - q\right) }^{2}}\right\rbrack  }^{\prime } = \frac{2 - p}{{p}^{2}},
$$

所以 $X$ 的方差为

$$
D\left( X\right)  = E\left( {X}^{2}\right)  - {\left\lbrack  E\left( X\right) \right\rbrack  }^{2} = \frac{2 - p}{{p}^{2}} - \frac{1}{{p}^{2}} = \frac{1 - p}{{p}^{2}}.
$$

【4.47】已知甲、乙两箱中装有同种产品,其中甲箱中装有 3 件合格品和 3 件次品,乙箱中仅装有 3 件合格品. 从甲箱中任取 3 件产品放入乙箱后, 求

(1)乙箱中次品件数 $X$ 的数学期望；

(2)从乙箱中任取一件产品是次品的概率.

解法一(1) $X$ 的可能取值为 $0,1,2,3, X$ 的概率分布为

$P\{ X = k\}  = \frac{{C}_{3}^{k}{C}_{3}^{3 - k}}{{C}_{6}^{3}},\;k = 0,1,2,3,\;$ 即

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>$\frac{1}{20}$</td><td>$\frac{9}{20}$</td><td>$\frac{9}{20}$</td><td>$\frac{1}{20}$</td></tr></table>

因此

$$
{EX} = 0 \times  \frac{1}{20} + 1 \times  \frac{9}{20} + 2 \times  \frac{9}{20} + 3 \times  \frac{1}{20} = \frac{3}{2}.
$$

(2)设 $A$ 表示事件“从乙箱中任意取出的一件产品是次品”,根据全概率公式,有

$P\left( A\right)  = \mathop{\sum }\limits_{{k = 0}}^{3}P\{ X = k\} P\{ A \mid  X = k\}  = \frac{1}{20} \times  0 + \frac{9}{20} \times  \frac{1}{6} + \frac{9}{20} \times  \frac{2}{6} + \frac{1}{20} \times  \frac{3}{6} = \frac{1}{4}.$

解法二 (1) 设 ${X}_{i} = \left\{  \begin{array}{ll} 0, & \text{ 从甲箱中取出的第 }i\text{ 件产品是合格品 } \\  1, & \text{ 从甲箱中取出的第 }i\text{ 件产品是次品 } \end{array}\right.$,则 $X$ 则 ${X}_{i}$ 的概率分布为

<table><tr><td>${X}_{i}$</td><td>0</td><td/><td rowspan="2"/></tr><tr><td>$P$</td><td/><td/></tr></table>

且 $E{X}_{i} = \frac{1}{2}\left( {i = 1,2,3}\right)$.

因为 $X = {X}_{1} + {X}_{2} + {X}_{3}$,所以

$$
{EX} = E\left( {{X}_{1} + {X}_{2} + {X}_{3}}\right)  = E{X}_{1} + E{X}_{2} + E{X}_{3} = \frac{3}{2}.
$$

( 2 )设 $A$ 表示事件“从乙箱中任意取出的一件产品是次品”,由于 $\{ X = 0\},\{ X = 1\},\{ X = 2\}$ 和 $\{ X$ $= 3\}$ 构成完全事件组,因此根据全概率公式,有

$$
P\left( A\right)  = \mathop{\sum }\limits_{{k = 0}}^{3}P\{ X = k\} P\{ A \mid  X = k\}  = \mathop{\sum }\limits_{{k = 0}}^{3}P\{ X = k\}  \cdot  \frac{k}{6} = \frac{1}{6}\mathop{\sum }\limits_{{k = 0}}^{3}{kP}\{ X = k\}
$$

$$
= \frac{1}{6}{EX} = \frac{1}{6} \cdot  \frac{3}{2} = \frac{1}{4}\text{.}
$$

【4.48】假设由自动线加工的某种零件的内径 $X$ (毫米) 服从正态分布 $N\left( {\mu,1}\right)$,内径小于 10 或大于 12 的为不合格品, 其余为合格品, 销售每件合格品获利, 销售每件不合格品亏损. 已知销售利润 $T$ (单位:元) 与销售零件的内径 $X$ 有如下关系:

$$
T = \left\{  \begin{array}{ll}  - 1, & \text{ 若 }X < {10} \\  {20}, & \text{ 若 }{10} \leq  X \leq  {12} \\   - 5, & \text{ 若 }X > {12} \end{array}\right.
$$

问平均内径 $\mu$ 取何值时,销售一个零件的平均利润最大?

解 由条件知, 平均利润为

$$
E\left( T\right)  = {20P}\{ {10} \leq  X \leq  {12}\}  - P\{ X < {10}\}  - {5P}\{ X > {12}\}
$$

$$
= {20}\left\lbrack  {\Phi \left( {{12} - \mu }\right)  - \Phi \left( {{10} - \mu }\right) }\right\rbrack   - \Phi \left( {{10} - \mu }\right)  - 5\left\lbrack  {1 - \Phi \left( {{12} - \mu }\right) }\right\rbrack
$$

$$
= {25\Phi }\left( {{12} - \mu }\right)  - {21\Phi }\left( {{10} - \mu }\right)  - 5\text{,}
$$

其中 $\Phi \left( x\right)$ 是标准正态分布函数,设 $\varphi \left( x\right)$ 为标准正态密度,则有

$$
\frac{\mathrm{d}E\left( T\right) }{\mathrm{d}\mu } =  - {25\varphi }\left( {{12} - \mu }\right)  + {21\varphi }\left( {{10} - \mu }\right)
$$

令其等于 0,得

$$
\frac{-{25}}{\sqrt{2\pi }}{\mathrm{e}}^{\frac{{\left( {12} - \mu \right) }^{2}}{2}} + \frac{21}{\sqrt{2\pi }}{\mathrm{e}}^{\frac{{\left( {10} - \mu \right) }^{2}}{2}} = 0,
$$

即 ${25}{\mathrm{e}}^{\frac{{\left( {12} - \mu \right) }^{2}}{2}} = {21}{\mathrm{e}}^{\frac{{\left( {10} - \mu \right) }^{2}}{2}}$,

由此得 $\mu  = {\mu }_{0} = {11} - \frac{1}{2}\ln \frac{25}{11} \approx  {10.9}$.

由题意知,当 $\mu  = {\mu }_{0} \approx  {10.9}$ 毫米时,平均利润最大.

【4.49】从学校乘汽车到火车站的途中有 3 个交通岗, 假设在各个交通岗遇到红灯的事件是相互独立的,并且概率都是 $\frac{2}{5}$,设 $X$ 为途中遇到红灯的次数,求随机变量 $X$ 的分布律、分布函数和数学期望.

解 $X$ 服从二项分布 $B\left( {3,\frac{2}{5}}\right), X$ 可能取值为0,1,2,3,从而

$$
P\{ X = 0\}  = {\left( 1 - \frac{2}{5}\right) }^{3} = \frac{27}{125}
$$

$$
P\{ X = 1\}  = {C}_{3}^{1} \cdot  \frac{2}{5} \cdot  {\left( 1 - \frac{2}{5}\right) }^{2} = \frac{54}{125}
$$

$$
P\{ X = 2\}  = {C}_{3}^{2} \cdot  {\left( \frac{2}{5}\right) }^{2} \cdot  \left( {1 - \frac{2}{5}}\right)  = \frac{36}{125}
$$

$$
P\{ X = 3\}  = {\left( \frac{2}{5}\right) }^{3} = \frac{8}{125}
$$

即 $X$ 的分布律为

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>$\frac{27}{125}$</td><td>$\frac{54}{125}$</td><td>$\frac{36}{125}$</td><td>$\frac{8}{125}$</td></tr></table>

因此, $X$ 的分布函数为

$$
F\left( x\right)  = P\{ X \leq  x\}  = \left\{  \begin{array}{ll} 0, & x < 0 \\  \frac{27}{125}, & 0 \leq  x < 1 \\  \frac{81}{125}, & 1 \leq  x < 2 \\  \frac{117}{125}, & 2 \leq  x < 3 \\  1, & x \geq  3 \end{array}\right.
$$

$X$ 的数学期望为 $E\left( X\right)  = 3 \cdot  \frac{2}{5} = \frac{6}{5}$.

【4.50】两台同样的自动记录仪,每台无故障工作的时间服从参数为 5 的指数分布；首先开动其中一台,当其发生故障时停用而另一台自动开动,试求两台记录仪无故障工作的总时间 $T$ 的概率密度 $f\left( t\right)$,数学期望和方差.

解 以 ${X}_{1}$ 和 ${X}_{2}$ 表示先后开动的记录仪无故障工作的时间,则 $T = {X}_{1} + {X}_{2}$,由条件知 ${X}_{i}(i =$ 1,2 ) 的概率密度为

$$
{p}_{i}\left( x\right)  = \left\{  \begin{array}{ll} 5{\mathrm{e}}^{-{5x}}, & \text{ 若 }x > 0 \\  0, & \text{ 若 }x \leq  0 \end{array}\right.
$$

两台仪器无故障工作时间 ${X}_{1}$ 和 ${X}_{2}$ 显然相互独立.

利用二独立随机变量和的密度公式求 $T$ 的概率密度,对于 $t > 0$,有

$$
f\left( t\right)  = {\int }_{-\infty }^{+\infty }{p}_{1}\left( x\right) {p}_{2}\left( {t - x}\right) \mathrm{d}x = {25}{\int }_{0}^{t}{\mathrm{e}}^{-{5x}}{\mathrm{e}}^{-5\left( {t - x}\right) }\mathrm{d}x = {25}{\mathrm{e}}^{-{5t}}{\int }_{0}^{t}\mathrm{\;d}x
$$

$$
= {25t}{\mathrm{e}}^{-{5t}}
$$

当 $t \leq  0$ 时,显然 $f\left( t\right)  = 0$,于是,得

$$
f\left( t\right)  = \left\{  \begin{array}{ll} {25t}{\mathrm{e}}^{-{5t}}, & \text{ 若 }t > 0 \\  0, & \text{ 若 }t \leq  0 \end{array}\right.
$$

由于 ${X}_{i}$ 服从参数为 $\lambda  = 5$ 的指数分布,知

$$
E{X}_{i} = \frac{1}{5};\;D{X}_{i} = \frac{1}{25}\;\left( {i = 1,2}\right)
$$

因此, 有

$$
{ET} = E\left( {{X}_{1} + {X}_{2}}\right)  = E{X}_{1} + E{X}_{2} = \frac{2}{5}
$$

由于 ${X}_{1}$ 和 ${X}_{2}$ 独立,可见

$$
{DT} = D\left( {{X}_{1} + {X}_{2}}\right)  = D{X}_{1} + D{X}_{2} = \frac{2}{25}.
$$

点评 ${ET}$ 和 ${DT}$ 也可由 $T$ 的密度 $f\left( t\right)$ 求得:

$$
{ET} = {\int }_{-\infty }^{+\infty }{tf}\left( t\right) \mathrm{d}t
$$

$$
E\left( {T}^{2}\right)  = {\int }_{-\infty }^{+\infty }{t}^{2}f\left( t\right) \mathrm{d}t
$$

$$
{DT} = E\left( {T}^{2}\right)  - {\left( ET\right) }^{2}
$$

#### 题型 6. 独立与不相关

【4.51】若 $X \sim  N\left( {0,1}\right)$,且 $Y = {X}^{2}$,问 $X$ 与 $Y$ 是否不相关? 是否相互独立? 解 因为 $X \sim  N\left( {0,1}\right)$,密度函数 $f\left( x\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{\frac{{x}^{2}}{2}}$ 为偶函数,所以 $E\left( X\right)  = E\left( {X}^{3}\right)  = 0$. 于是由

$$
\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - E\left( X\right) E\left( Y\right)  = E\left( {X}^{3}\right)  - E\left( X\right) E\left( {X}^{2}\right)  = 0
$$

得 ${\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }} = 0$. 这说明 $X$ 与 $Y$ 是不相关的,但 $Y = {X}^{2}$,显然, $X$ 与 $Y$ 是不相互独立的. 【4.52】若 $X \sim  U\left( {0,1}\right), Y = {X}^{2}$,问 $X$ 与 $Y$ 是否不相关? 是否独立? 解 因为 $X \sim  U\left( {0,1}\right)$,故

$$
E\left( X\right)  = \frac{1}{2},
$$

$$
E\left( Y\right)  = E\left( {X}^{2}\right)  = {\int }_{0}^{1}{x}^{2}\mathrm{\;d}x = \frac{1}{3},
$$

$$
E\left( {XY}\right)  = E\left( {X}^{3}\right)  = {\int }_{0}^{1}{x}^{3}\mathrm{\;d}x = \frac{1}{4},
$$

则 $\operatorname{Cov}\left( {X, Y}\right)  = E\left( {XY}\right)  - E\left( X\right)  \cdot  E\left( Y\right)  \neq  0$. 故 $X, Y$ 不是不相关,从而 $X, Y$ 不独立. 【4.53】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{\pi }, & {x}^{2} + {y}^{2} \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

试验证 $X$ 和 $Y$ 是不相关的,但 $X$ 和 $Y$ 不是相互独立的. 解 由于 ${f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  \begin{array}{ll} \frac{1}{\pi }{\int }_{-\sqrt{1 - {x}^{2}}}^{\sqrt{1 - {x}^{2}}}\mathrm{\;d}y = \frac{2}{\pi }\sqrt{1 - {x}^{2}}, &  - 1 \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.$ 由 $X$ 和 $Y$ 的对称性,同理可得

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{2}{\pi }\sqrt{1 - {y}^{2}}, &  - 1 \leq  y \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

显然, $f\left( {x, y}\right)  \neq  {f}_{X}\left( x\right) {f}_{Y}\left( y\right)$,故 $X$ 和 $Y$ 不是相互独立的.

又 $E\left( X\right)  = {\int }_{-\infty }^{+\infty }x{f}_{X}\left( x\right) \mathrm{d}x = {\int }_{-1}^{1}\frac{2}{\pi }x\sqrt{1 - {x}^{2}}\mathrm{\;d}x = 0$

同理 $E\left( Y\right)  = 0$.

$$
E\left( {XY}\right)  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xyf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = \frac{1}{\pi }{\int }_{-1}^{1}\mathrm{\;d}x{\int }_{-\sqrt{1 - {x}^{2}}}^{\sqrt{1 - {x}^{2}}}{xy}\mathrm{\;d}y = 0
$$

从而 ${\rho }_{XY} = \frac{\operatorname{Cov}\left( {X, Y}\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }} = \frac{E\left( {XY}\right)  - E\left( X\right) E\left( Y\right) }{\sqrt{D\left( X\right) }\sqrt{D\left( Y\right) }} = 0$. 故 $X$ 和 $Y$ 不相关.

【4.54】设 $\left( {X, Y}\right)$ 服从二维正态分布,且有 $D\left( X\right)  = {\sigma }_{X}^{2}, D\left( Y\right)  = {\sigma }_{Y}^{2}$,证明当 ${a}^{2} = \frac{{\sigma }_{X}^{2}}{{\sigma }_{Y}^{2}}$ 时随机变量 $W = X - {aY}$ 与 $V = X + {aY}$ 相互独立.

解 $E\left( W\right)  = E\left( X\right)  - {aE}\left( Y\right)  = {\mu }_{X} - a{\mu }_{Y}$

$E\left( V\right)  = E\left( X\right)  + {aE}\left( Y\right)  = {\mu }_{X} + a{\mu }_{Y}$

$D\left( W\right)  = D\left( X\right)  + {a}^{2}D\left( Y\right)  - {2a}\operatorname{Cov}\left( {X, Y}\right)  = {\sigma }_{X}^{2} + {a}^{2}{\sigma }_{Y}^{2} - {2a}{\rho }_{XY}{\sigma }_{X}{\sigma }_{Y}$

$D\left( V\right)  = D\left( X\right)  + {a}^{2}D\left( Y\right)  + {2a}\operatorname{Cov}\left( {X, Y}\right)  = {\sigma }_{X}^{2} + {a}^{2}{\sigma }_{Y}^{2} + {2a}{\rho }_{XY}{\sigma }_{X}{\sigma }_{Y}$

$E\left( {WV}\right)  = E\left( {{X}^{2} - {a}^{2}{Y}^{2}}\right)  = E\left( {X}^{2}\right)  - {a}^{2}E\left( {Y}^{2}\right)  = D\left( X\right)  + {\mu }_{X}^{2} - {a}^{2}\left\lbrack  {D\left( Y\right)  + {\mu }_{Y}^{2}}\right\rbrack$

$= {\sigma }_{X}^{2} + {\mu }_{X}^{2} - {a}^{2}{\sigma }_{Y}^{2} - {a}^{2}{\mu }_{Y}^{2}$

$$
\operatorname{Cov}\left( {W, V}\right)  = E\left( {WV}\right)  - E\left( W\right) E\left( V\right)  = {\sigma }_{X}^{2} + {\mu }_{X}^{2} - {a}^{2}{\sigma }_{Y}^{2} - {a}^{2}{\mu }_{Y}^{2} - \left( {{\mu }_{X} - a{\mu }_{Y}}\right) \left( {{\mu }_{X} + a{\mu }_{Y}}\right)
$$

$$
= {\sigma }_{X}^{2} - {a}^{2}{\sigma }_{Y}^{2}
$$

由于 $\left( {W, V}\right)$ 服从二维正态分布, $W$ 与 $V$ 相互独立的充要条件是 $W$ 与 $V$ 不相关,即 $\operatorname{Cov}\left( {W, V}\right)  =$ 0,则 ${\sigma }_{X}^{2} - {a}^{2}{\sigma }_{Y}^{2} = 0$,即

$$
{a}^{2} = \frac{{\sigma }_{X}^{2}}{{\sigma }_{Y}^{2}}.
$$

【4.55】设 $A, B$ 是二随机事件; 随机变量

$$
X = \left\{  {\begin{array}{ll} 1, & \text{ 若 }A\text{ 出现 } \\   - 1, & \text{ 若 }A\text{ 不出现 } \end{array}\;Y = \left\{  \begin{array}{ll} 1, & \text{ 若 }B\text{ 出现 } \\   - 1, & \text{ 若 }B\text{ 不出现 } \end{array}\right. }\right.
$$

试证明随机变量 $X$ 和 $Y$ 不相关的充分必要条件是 $A$ 与 $B$ 相互独立.

证 记 $P\left( A\right)  = {p}_{1} \cdot , P\left( B\right)  = {p}_{2}, P\left( {AB}\right)  = {p}_{12}$,由数学期望的定义,可见

$$
{EX} = P\left( A\right)  - P\left( \bar{A}\right)  = 2{p}_{1} - 1,
$$

$$
{EY} = 2{p}_{2} - 1
$$

现在求 ${EXY}$. 由于 ${XY}$ 只有两个可能值 1 和 -1,可见

$$
P\{ {XY} = 1\}  = P\left( {AB}\right)  + P\left( {\bar{A}\bar{B}}\right)  = 2{p}_{12} - {p}_{1} - {p}_{2} + 1
$$

$$
P\{ {XY} =  - 1\}  = 1 - P\{ {XY} = 1\}  = {p}_{1} + {p}_{2} - 2{p}_{12}
$$

$$
{EXY} = P\{ {XY} = 1\}  - P\{ {XY} =  - 1\}  = 4{p}_{12} - 2{p}_{1} - 2{p}_{2} + 1
$$

从而

$$
\operatorname{Cov}\left( {X, Y}\right)  = {EXY} - {EX} \cdot  {EY} = 4{p}_{12} - 4{p}_{1}{p}_{2}
$$

因此, $\operatorname{Cov}\left( {X, Y}\right)  = 0$ 当且仅当 ${p}_{12} = {p}_{1}{p}_{2}$,即 $X$ 和 $Y$ 不相关当且仅当事件 $A$ 和 $B$ 相互独立.

【4.56】设二维随机变量 $\left( {X, Y}\right)$ 的密度函数为

$$
f\left( {x, y}\right)  = \frac{1}{2}\left\lbrack  {{\varphi }_{1}\left( {x, y}\right)  + {\varphi }_{2}\left( {x, y}\right) }\right\rbrack ,
$$

其中 ${\varphi }_{1}\left( {x, y}\right)$ 和 ${\varphi }_{2}\left( {x, y}\right)$ 都是二维正态密度函数,且它们对应的二维随机变量的相关系数分别为 $\frac{1}{3}$ 和 $- \frac{1}{3}$,它们的边缘密度函数所对应的随机变量的数学期望都是零,方差都是 1.

(1)求随机变量 $X$ 和 $Y$ 的密度函数 ${f}_{1}\left( x\right)$ 和 ${f}_{2}\left( y\right)$,及 $X$ 和 $Y$ 的相关系数 $\rho$ (可以直接利用二维正态密度的性质).

(2)问 $X$ 和 $Y$ 是否独立？为什么?

解 (1)由于二维正态密度函数的两个边缘密度都是正态密度函数,因此 ${\varphi }_{1}\left( {x, y}\right)$ 和 ${\varphi }_{2}\left( {x, y}\right)$ 的两个边缘密度为标准正态密度函数, 故

$$
{f}_{1}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \frac{1}{2}\left\lbrack  {{\int }_{-\infty }^{+\infty }{\varphi }_{1}\left( {x, y}\right) \mathrm{d}y + {\int }_{-\infty }^{+\infty }{\varphi }_{2}\left( {x, y}\right) \mathrm{d}y}\right\rbrack
$$

$$
= \frac{1}{2}\left\lbrack  {\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}} + \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}}\right\rbrack   = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}
$$

同理, ${f}_{2}\left( y\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{y}^{2}}{2}}$.

由于 $X \sim  N\left( {0,1}\right), Y \sim  N\left( {0,1}\right)$,可见 ${EX} = {EY} = 0,{DX} = {DY} = 1$. 随机变量 $X$ 和 $Y$ 的相关系数

$$
\rho  = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xyf}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y
$$

$$
= \frac{1}{2}\left\lbrack  {{\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xy}{\varphi }_{1}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y + {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }{xy}{\varphi }_{2}\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y}\right\rbrack
$$

$$
= \frac{1}{2}\left\lbrack  {\frac{1}{3} - \frac{1}{3}}\right\rbrack   = 0.
$$

(2) 由题设

$$
f\left( {x, y}\right)  = \frac{3}{{8\pi }\sqrt{2}}\left\lbrack  {{\mathrm{e}}^{-\frac{9}{16}\left( {{x}^{2} - \frac{2}{3}{xy} + {y}^{2}}\right) } + {\mathrm{e}}^{-\frac{9}{16}\left( {{x}^{2} + \frac{2}{3}{xy} + {y}^{2}}\right) }}\right\rbrack ,
$$

$$
{f}_{1}\left( x\right)  \cdot  {f}_{2}\left( y\right)  = \frac{1}{2\pi }{\mathrm{e}}^{-\frac{{x}^{2}}{2}} \cdot  {\mathrm{e}}^{-\frac{{y}^{2}}{2}} = \frac{1}{2\pi }{\mathrm{e}}^{-\frac{\left( {x}^{2} + {y}^{2}\right) }{2}},
$$

$$
f\left( {x, y}\right)  \neq  {f}_{1}\left( x\right)  \cdot  {f}_{2}\left( y\right).
$$

所以 $X$ 与 $Y$ 不独立.

【4.57】对于任意二事件 $A$ 和 $B,0 < P\left( A\right)  < 1,0 < P\left( B\right)  < 1$,

$$
\rho  = \frac{P\left( {AB}\right)  - P\left( A\right) P\left( B\right) }{\sqrt{P\left( A\right) P\left( B\right) P\left( \bar{A}\right) P\left( \bar{B}\right) }}
$$

称做事件 $A$ 和 $B$ 的相关系数.

(1)证明事件 $A$ 和 $B$ 独立的充分必要条件是其相关系数等于零；

(2)利用随机变量相关系数的基本性质,证明 $\left| \rho \right|  \leq  1$. 量 188

证 (1)由 $\rho$ 的定义,可见 $\rho  = 0$ 当且仅当 $P\left( {AB}\right)  - P\left( A\right) P\left( B\right)  = 0$,而这恰好是二事件 $A$ 和 $B$ 独立的定义,即 $\rho  = 0$ 是 $A$ 和 $B$ 独立的充分必要条件.

(2)考虑随机变量 $X$ 和 $Y$ :

$$
X = \left\{  {\begin{array}{ll} 1, & \text{ 若 }A\text{ 出现 } \\  0, & \text{ 若 }A\text{ 不出现 } \end{array},\;Y = \left\{  {\begin{array}{ll} 1, & \text{ 若 }B\text{ 出现 } \\  0, & \text{ 若 }B\text{ 不出现 } \end{array}.}\right. }\right.
$$

由条件知, $X$ 和 $Y$ 都服从 $0 \sim  1$ 分布:

$$
X \sim  \left( \begin{matrix} 0 & 1 \\  1 - P\left( A\right) & P\left( A\right)  \end{matrix}\right),\;Y \sim  \left( \begin{matrix} 0 & 1 \\  1 - P\left( B\right) & P\left( B\right)  \end{matrix}\right).
$$

易知

$$
{EX} = P\left( A\right),\;{EY} = P\left( B\right);
$$

$$
{DX} = P\left( A\right) P\left( \bar{A}\right),\;D\left( Y\right)  = P\left( B\right) P\left( \bar{B}\right);
$$

$$
E\left( {XY}\right)  = P\left( {AB}\right),
$$

$$
\operatorname{Cov}\left( {X, Y}\right)  = P\left( {AB}\right)  - P\left( A\right) P\left( B\right).
$$

因此,事件 $A$ 和 $B$ 的相关系数就是随机变量 $X$ 和 $Y$ 的相关系数.

于是由二随机变量相关系数的基本性质,可见 $\left| \rho \right|  \leq  1$.