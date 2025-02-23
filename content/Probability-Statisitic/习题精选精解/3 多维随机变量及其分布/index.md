## § 1. 二维随机变量及其分布

### 知识要点

1. 二维随机变量 设 $E$ 是随机试验,样本空间 $\Omega  = \{ \omega \}$,由 $X = X\left( \omega \right), Y = Y\left( \omega \right)$ 构成的向量 $\left( {X, Y}\right)$ 称为二维随机变量.

2. 联合分布函数 设 $\left( {X, Y}\right)$ 是二维随机变量, $x, y$ 是两个任意实数,则称定义在平面上的二元函数 $P\{ X \leq  x, Y \leq  y\}$ 为 $\left( {X, Y}\right)$ 的分布函数,或称为 $X$ 和 $Y$ 的联合分布函数,记作 $F\left( {x, y}\right)$, 即

$$
F\left( {x, y}\right)  = P\{ X \leq  x, Y \leq  y\}.
$$

$F\left( {x, y}\right)$ 的性质:

(1) $0 \leq  F\left( {x, y}\right)  \leq  1$,且 $F\left( {-\infty, y}\right)  = F\left( {x, - \infty }\right)  = F\left( {-\infty, - \infty }\right)  = 0, F\left( {+\infty, + \infty }\right)$ $= 1$.

(2) $F\left( {x, y}\right)$ 是变量 $x$ 或 $y$ 的单调不减函数.

(3) $F\left( {x, y}\right)  = F\left( {x + 0, y}\right), F\left( {x, y}\right)  = F\left( {x, y + 0}\right), F\left( {x, y}\right)$ 关于 $x$ 或 $y$ 都是右连续的.

(4) 对任意 $\left( {{x}_{1},{y}_{1}}\right),\left( {{x}_{2},{y}_{2}}\right)$ : 当 ${x}_{1} < {x}_{2},{y}_{1} < {y}_{2}$ 时有

$P\left\{  {{x}_{1} < X \leq  {x}_{2},{y}_{1} < Y \leq  {y}_{2}}\right\}   = F\left( {{x}_{2},{y}_{2}}\right)  - F\left( {{x}_{1},{y}_{2}}\right)  - F\left( {{x}_{2},{y}_{1}}\right)  + F\left( {{x}_{1},{y}_{1}}\right).$

1. 二维离散型随机变量 若 $\left( {X, Y}\right)$ 所有可能取值为 $\left( {{x}_{i},{y}_{j}}\right), i, j = 1,2,\cdots$,则 $P\left\{  {X = {x}_{i}}\right.$, $\left. {Y = {y}_{j}}\right\}   = {p}_{ij}$ 称为联合分布律,联合分布律可列表如下:

<table><tr><td>Y $X$</td><td>${y}_{1}$</td><td>...</td><td>${y}_{j}$</td><td>...</td></tr><tr><td>${x}_{1}$</td><td>${p}_{11}$</td><td>...</td><td>${p}_{1j}$</td><td>...</td></tr><tr><td>:</td><td>$\vdots$</td><td/><td>$\vdots$</td><td/></tr><tr><td>${x}_{i}$</td><td>${p}_{i1}$</td><td>...</td><td>${p}_{ij}$</td><td>...</td></tr><tr><td>$\vdots$</td><td>$\vdots$</td><td/><td>$\vdots$</td><td/></tr></table>

联合分布律的性质: ${p}_{ij} \geq  0,\mathop{\sum }\limits_{{i = 1}}^{\infty }\mathop{\sum }\limits_{{j = 1}}^{\infty }{p}_{ij} = 1$.

1. 二维连续型随机变量 若分布函数 $F\left( {x, y}\right)  = {\int }_{-\infty }^{x}{\int }_{-\infty }^{y}f\left( {u, v}\right) \mathrm{d}u\mathrm{\;d}v$,则称 $\left( {X, Y}\right)$ 是连续型随机变量. $f\left( {x, y}\right)$ 称为 $\left( {X, Y}\right)$ 的联合概率密度.

联合概率密度的性质:

(1) $f\left( {x, y}\right)  \geq  0;\;{\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = 1$.

(2)若 $f\left( {x, y}\right)$ 在点 $\left( {x, y}\right)$ 处连续,则 $\frac{{\partial }^{2}F\left( {x, y}\right) }{\partial x\partial y} = f\left( {x, y}\right)$.

(3) 设 $G$ 是 ${xOy}$ 平面上一个区域,则 $P\{ \left( {X, Y}\right)  \in  G\}  = {\iint }_{G}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y$.

### 基本题型

题型 1. 关于分布函数、分布律、概率密度的性质

【1.1】设随机变量 $\left( {X, Y}\right)$ 的分布函数为:

$$
F\left( {x, y}\right)  = A\left( {B + \arctan \frac{x}{2}}\right) \left( {C + \arctan \frac{y}{3}}\right),
$$

求 $A, B, C$ 及 $\left( {X, Y}\right)$ 的联合密度函数.

解 (1) 由联合分布函数的性质知

$$
F\left( {+\infty, + \infty }\right)  = A\left( {B + \frac{\pi }{2}}\right) \left( {C + \frac{\pi }{2}}\right)  = 1,
$$

$$
F\left( {-\infty, + \infty }\right)  = A\left( {B - \frac{\pi }{2}}\right) \left( {C + \frac{\pi }{2}}\right)  = 0,
$$

$$
F\left( {+\infty, - \infty }\right)  = A\left( {B + \frac{\pi }{2}}\right) \left( {C - \frac{\pi }{2}}\right)  = 0,
$$

得 $A = \frac{1}{{\pi }^{2}}, B = \frac{\pi }{2}, C = \frac{\pi }{2}$.

(2) $f\left( {x, y}\right)  = \frac{{\partial }^{2}F}{\partial x\partial y} = \frac{6}{{\pi }^{2}\left( {4 + {x}^{2}}\right) \left( {9 + {y}^{2}}\right) }$

【1.2】设二维连续型随机变量 $\left( {{X}_{1},{X}_{2}}\right)$ 与 $\left( {{Y}_{1},{Y}_{2}}\right)$ 的联合密度分别为 $p\left( {x, y}\right)$ 和 $g\left( {x, y}\right)$, 令 $f\left( {x, y}\right)  = {ap}\left( {x, y}\right)  + {bg}\left( {x, y}\right)$. 要使函数 $f\left( {x, y}\right)$ 是某个二维随机变量的联合密度,则 $a, b$ 应满足(   ).

(A) $a + b = 1$ (B) $a > 0, b > 0$

(C) $0 \leq  a \leq  1,0 \leq  b \leq  1$ (D) $a \geq  0, b \geq  0$,且 $a + b = 1$

解 $f\left( {x, y}\right)$ 为密度函数 $\Leftrightarrow  f\left( {x, y}\right)  \geq  0$ 且 ${\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = 1$,

由此可推得, $1 = a + b$,且 ${ap}\left( {x, y}\right)  + {bg}\left( {x, y}\right)  \geq  0\;\left( {\forall x, y \in  \mathbf{R}}\right)$.

所以选择(D).

对于 $a \geq  0, b \geq  0$,由 $p\left( {x, y}\right)  \geq  0, g\left( {x, y}\right)  \geq  0$ 得

$$
{ap}\left( {x, y}\right)  + {bg}\left( {x, y}\right)  \geq  0\;\left( {\forall x, y \in  \mathbf{R}}\right).
$$

如果 $a < 0$ (或 $b < 0$ ),则对一切 $x, y$ 有

$$
{bg}\left( {x, y}\right)  \geq  \left( {-a}\right) p\left( {x, y}\right) \text{ 或 }{ap}\left( {x, y}\right)  \geq  \left( {-b}\right) g\left( {x, y}\right)
$$

此式未必成立.

故应选(D).

【1.3】设 $\left( {X, Y}\right)$ 的分布律为

<table><tr><td>Y $X$</td><td>1</td><td>2</td><td>3</td></tr><tr><td>-1</td><td>$\frac{1}{3}$</td><td>$\frac{a}{6}$</td><td>$\frac{1}{4}$</td></tr><tr><td>1</td><td>0</td><td>$\frac{1}{4}$</td><td>${a}^{2}$</td></tr></table>

求 $a$ 的值.

解 由分布律性质知:

$$
\frac{1}{3} + \frac{a}{6} + \frac{1}{4} + \frac{1}{4} + {a}^{2} = 1,
$$

即

$$
6{a}^{2} + a - 1 = 0,\;\left( {{3a} - 1}\right) \left( {{2a} + 1}\right)  = 0,
$$

解得 $a = \frac{1}{3}$ 或 $a =  - \frac{1}{2}$.

由 ${p}_{ij} \geq  0$ 可舍去 $a =  - \frac{1}{2}$,所以 $a = \frac{1}{3}$.

#### 题型 2. 求联合分布律

【1.4】盒子里装有 3 只黑球、 2 只红球、 2 只白球,在其中任选 4 只球,以 $X$ 表示取到黑球的只数,以 $Y$ 表示取到红球的只数,求 $X$ 和 $Y$ 的联合分布律.

解 $\left( {X, Y}\right)$ 的所有可能取值为 $\left( {0,0}\right),\left( {0,1}\right),\left( {0,2}\right),\left( {1,0}\right),\left( {1,1}\right),\left( {1,2}\right),\left( {2,0}\right),\left( {2,1}\right)$, $\left( {2,2}\right),\left( {3,0}\right),\left( {3,1}\right),\left( {3,2}\right)$.

按古典概型,显有

$$
P\{ X = 0, Y = 2\}  = \frac{{C}_{3}^{0} \times  {C}_{2}^{2} \times  {C}_{2}^{2}}{{C}_{7}^{4}} = \frac{1}{35}
$$

$$
P\{ X = 1, Y = 1\}  = \frac{{C}_{3}^{1} \times  {C}_{2}^{1} \times  {C}_{2}^{2}}{{C}_{7}^{4}} = \frac{6}{35}
$$

$$
P\{ X = 1, Y = 2\}  = \frac{{C}_{3}^{1} \times  {C}_{2}^{2} \times  {C}_{2}^{1}}{{C}_{7}^{4}} = \frac{6}{35}
$$

$$
P\{ X = 2, Y = 1\}  = \frac{{C}_{3}^{2} \times  {C}_{2}^{1} \times  {C}_{2}^{1}}{{C}_{7}^{4}} = \frac{12}{35}
$$

$$
P\{ X = 2, Y = 0\}  = \frac{{C}_{3}^{2} \times  {C}_{2}^{0} \times  {C}_{2}^{2}}{{C}_{7}^{4}} = \frac{3}{35}
$$

$$
P\{ X = 2, Y = 2\}  = \frac{{C}_{3}^{2} \times  {C}_{2}^{2} \times  {C}_{2}^{0}}{{C}_{7}^{4}} = \frac{3}{35}
$$

$$
P\{ X = 3, Y = 0\}  = \frac{{C}_{3}^{3} \times  {C}_{2}^{0} \times  {C}_{2}^{1}}{{C}_{7}^{4}} = \frac{2}{35}
$$

$$
P\{ X = 3, Y = 1\}  = \frac{{C}_{3}^{3} \times  {C}_{2}^{1} \times  {C}_{2}^{0}}{{C}_{7}^{4}} = \frac{2}{35}
$$

则 $X$ 和 $Y$ 的联合分布律为: 题型 3. 分布函数与概率密度的转化

<table><tr><td>$X$ Y</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>0</td><td>0</td><td>0</td><td>$\frac{3}{35}$</td><td>$\frac{2}{35}$</td></tr><tr><td>1</td><td>0</td><td>$\frac{6}{35}$</td><td>$\frac{12}{35}$</td><td>$\frac{2}{35}$</td></tr><tr><td>2</td><td>$\frac{1}{35}$</td><td>$\frac{6}{35}$</td><td>$\frac{3}{35}$</td><td>0</td></tr></table>

【1.5】设二维随机变量 $\left( {X, Y}\right)$ 的联合分布函数为

$$
F\left( {x, y}\right)  = \left\{  \begin{array}{ll} 1 - {3}^{-x} - {3}^{-y} + {3}^{-x - y}, & x \geq  0, y \geq  0 \\  0, & \text{ 其他. } \end{array}\right.
$$

则二维随机变量 $\left( {X, Y}\right)$ 的联合密度 $\varphi \left( {x, y}\right)$ 为_____.

解 可以验证这是二维连续型随机变量的分布函数, 由公式:

$$
\varphi \left( {x, y}\right)  = \frac{{\partial }^{2}F}{\partial x\partial y}
$$

有

$$
\frac{\partial F}{\partial x} = {3}^{-x}\ln 3 - {3}^{-x - y}\ln 3\;\frac{{\partial }^{2}F}{\partial x\partial y} = {3}^{-x - y}{\left( \ln 3\right) }^{2}
$$

故 $\varphi \left( {x, y}\right)  = \left\{  \begin{array}{ll} {3}^{-x - y}{\left( \ln 3\right) }^{2}, & x \geq  0, y \geq  0 \\  0, & \text{ 其他. } \end{array}\right.$

【1.6】设随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{matrix} A{\mathrm{e}}^{-\left( {{3x} + {4y}}\right) }, & x > 0, y > 0 \\  0, & \text{ 其他. } \end{matrix}\right.
$$

求: (1)A 的值;

(2) $\left( {X, Y}\right)$ 的联合分布函数 $F\left( {x, y}\right)$;

(3) $\left( {X, Y}\right)$ 落在 $G = \{ \left( {x, y}\right)  \mid  0 < x \leq  1,0 < y \leq  2\}$ 中的概率.

解 (1) 由 ${\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = 1$,可得 $\frac{A}{12} = 1$,故 $A = {12}$.

(2)分情况讨论分布函数 $F\left( {x, y}\right)$.

① 当 $x > 0, y > 0$ 时,

$F\left( {x, y}\right)  = {\int }_{-\infty }^{x}{\int }_{-\infty }^{y}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{x}{\int }_{0}^{y}{12}{\mathrm{e}}^{-\left( {{3x} + {4y}}\right) }\mathrm{d}x\mathrm{\;d}y = \left( {1 - {\mathrm{e}}^{-{3x}}}\right) \left( {1 - {\mathrm{e}}^{-{4y}}}\right).$

② 当 $x, y$ 属于其他范围时 $f\left( {x, y}\right)  = 0, F\left( {x, y}\right)  = {\int }_{-\infty }^{x}{\int }_{-\infty }^{y}0\mathrm{\;d}x\mathrm{\;d}y = 0$.

所以 $F\left( {x, y}\right)  = \left\{  \begin{array}{ll} \left( {1 - {\mathrm{e}}^{-{3x}}}\right) \left( {1 - {\mathrm{e}}^{-{4y}}}\right), & x > 0, y > 0 \\  0, & \text{ 其他. } \end{array}\right.$

(3)方法一 利用概率密度:

$$
P\{ 0 < X \leq  1,0 < Y \leq  2\}  = {\int }_{0}^{1}{\int }_{0}^{2}{12}{\mathrm{e}}^{-\left( {{3x} + {4y}}\right) }\mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}{\mathrm{e}}^{-{3x}}\mathrm{\;d}x{\int }_{0}^{2}{12}{\mathrm{e}}^{-{4y}}\mathrm{\;d}y
$$

$$
= \left( {1 - {\mathrm{e}}^{-3}}\right) \left( {1 - {\mathrm{e}}^{-8}}\right) \text{.}
$$


方法二 利用分布函数:

由 $F\left( {x, y}\right)$ 的性质可知

$P\{ 0 < X \leq  1,0 < Y \leq  2\}  = F\left( {1,2}\right)  - F\left( {1,0}\right)  - F\left( {0,2}\right)  + F\left( {0,0}\right)  = \left( {1 - {\mathrm{e}}^{-3}}\right) \left( {1 - {\mathrm{e}}^{-8}}\right).$

点评 在求解二维随机变量在某矩形域的概率时可采用直接计算概率密度函数在矩形域的积分,也可采用分布函数计算,根据具体问题选择不同方法. 注意:非矩形域只能用方法一.

题型 4. 利用分布求概率

【1.7】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} {6x}, & 0 \leq  x \leq  y \leq  1 \\  0, & \text{ 其他. } \end{array}\right.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_84_974_479_332_288_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_84_974_479_332_288_0.jpg)

图 3-1.7

则 $P\{ X + Y \leq  1\}  =$ _____.

解 由题意作图 3-1.7 所示

$$
P\{ X + Y \leq  1\}  = {\iint }_{x + y \leq  1}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y
$$

$$
= {\int }_{0}^{\frac{1}{2}}\mathrm{\;d}x{\int }_{x}^{1 - x}{6x}\mathrm{\;d}y
$$

$$
= {\int }_{0}^{\frac{1}{2}}{6x}\left( {1 - {2x}}\right) \mathrm{d}x = \frac{1}{4}.
$$

点评 利用 $\left( {X, Y}\right)$ 的联合密度 $f\left( {x, y}\right)$ 求 $P\{ \left( {X, Y}\right)  \in  G\}$ 属于基本题型,其中 $P\{ \left( {X, Y}\right)  \in$ $G\}  = {\iint }_{G}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y$ 计算二重积分时,应找出 $G$ 与 $f\left( {x, y}\right)$ 的非零区域的公共部分 $D$,然后在 $D$ 上积分.

【1.8】设随机变量 $\left( {X, Y}\right)$ 的分布函数为

$$
F\left( {x, y}\right)  = \left\{  \begin{array}{ll} 1 - {2}^{-x} - {2}^{-y} + {2}^{-x - y}, & x \geq  0, y \geq  0 \\  0, & \text{ 其他. } \end{array}\right.
$$

求 $P\{ 1 < X \leq  2,3 < Y \leq  5\}$.

解 $P\{ 1 < X \leq  2,3 < Y \leq  5\}  = F\left( {2,5}\right)  - F\left( {1,5}\right)  - F\left( {2,3}\right)  + F\left( {1,3}\right)  = \frac{3}{128}$.

【1.9】设 $\left( {X, Y}\right)$ 的分布律为

<table><tr><td>$Y$ $X$</td><td>1</td><td>2</td><td>3</td></tr><tr><td>0</td><td>0.1</td><td>0.1</td><td>0.3</td></tr><tr><td>1</td><td>0.25</td><td>0</td><td>0.25</td></tr></table>

求: $\left( 1\right) P\{ X = 0\}$; (2) $P\{ Y \leq  2\}$;

(3) $P\{ X < 1, Y \leq  2\}$; (4) $P\{ X + Y = 2\}$.

分析 利用联合分布律求概率公式为

$$
P\{ \left( {X, Y}\right)  \in  G\}  = \mathop{\sum }\limits_{{\left( {{x}_{i},{y}_{j}}\right)  \in  G}}{p}_{ij}.
$$

解 (1) $P\{ X = 0\}  = P\{ X = 0, Y = 1\}  + P\{ X = 0, Y = 2\}  + P\{ X = 0, Y = 3\}$

$= {0.1} + {0.1} + {0.3} = {0.5}$;

(2) $P\{ Y \leq  2\}  = P\{ X = 0, Y = 1\}  + P\{ X = 0, Y = 2\}  + P\{ X = 1, Y = 1\}  + P\{ X = 1, Y = 2\}$

$= {0.1} + {0.1} + {0.25} + 0 = {0.45}$;

(3) $P\{ X < 1, Y \leq  2\}  = P\{ X = 0, Y = 1\}  + P\{ X = 0, Y = 2\}  = {0.1} + {0.1} = {0.2}$;

(4) $P\{ X + Y = 2\}  = P\{ X = 0, Y = 2\}  + P\{ X = 1, Y = 1\}  = {0.1} + {0.25} = {0.35}$.

## §2. 边缘分布

### 知识要点

1. 边缘分布函数 设二维随机变量 $\left( {X, Y}\right)$ 的分布函数为 $F\left( {x, y}\right)$,分别称函数

${F}_{X}\left( x\right)  = \mathop{\lim }\limits_{{y \rightarrow   + \infty }}F\left( {x, y}\right)  = F\left( {x, + \infty }\right)$ 和 ${F}_{Y}\left( y\right)  = \mathop{\lim }\limits_{{x \rightarrow   + \infty }}F\left( {x, y}\right)  = F\left( {+\infty, y}\right)$ 为 $\left( {X, Y}\right)$ 关于 $X$ 和 $Y$ 的边缘分布函数.

1. 边缘分布律 设二维离散型随机变量 $\left( {X, Y}\right)$ 的联合分布律为 $P\left\{  {X = {x}_{i}, Y = {y}_{j}}\right\}   = {p}_{ij}$, 则分别称

$$
{p}_{i \cdot  } = \mathop{\sum }\limits_{{j = 1}}^{\infty }{p}_{ij} = P\left\{  {X = {x}_{i}}\right\}  \;\left( {i = 1,2,3,\cdots }\right)
$$

和

$$
{p}_{\cdot j} = \mathop{\sum }\limits_{{i = 1}}^{\infty }{p}_{ij} = P\left\{  {Y = {y}_{j}}\right\}  \;\left( {j = 1,2,3,\cdots \cdots }\right)
$$

为 $\left( {X, Y}\right)$ 关于 $X$ 和 $Y$ 的边缘分布律.

1. 边缘概率密度 设二维连续型随机变量 $\left( {X, Y}\right)$ 的概率密度为 $f\left( {x, y}\right)$,则 ${f}_{X}\left( x\right)  =$ ${\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y$ 和 ${f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x$ 分别称为 $\left( {X, Y}\right)$ 关于 $X$ 和 $Y$ 的边缘概率密度.

#### 4. 常用的二维分布

(1)二维均匀分布:如果二维随机变量 $\left( {X, Y}\right)$ 有概率密度

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{A}, & \left( {x, y}\right)  \in  G \\  0, & \text{ 其他. } \end{array}\right.
$$

其中 $G$ 为平面有界区域, $A$ 为其面积,则称 $\left( {X, Y}\right)$ 在 $G$ 上服从二维均匀分布.

(2)二维正态分布:如果二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$f\left( {x, y}\right)$

$$
\frac{1}{{2\pi }{\sigma }_{1}{\sigma }_{2}\sqrt{1 - {\rho }^{2}}}\exp \left\{  {-\frac{1}{2\left( {1 - {\rho }^{2}}\right) }\left\lbrack  {\frac{{\left( x - {\mu }_{1}\right) }^{2}}{{\sigma }_{1}^{2}} - {2\rho }\frac{\left( {x - {\mu }_{1}}\right) \left( {y - {\mu }_{2}}\right) }{{\sigma }_{1}{\sigma }_{2}} + \frac{{\left( y - {\mu }_{2}\right) }^{2}}{{\sigma }_{2}^{2}}}\right\rbrack  }\right\}
$$

$$
- \infty  < x, y <  + \infty,
$$

其中 ${\mu }_{1},{\mu }_{2},{\sigma }_{1},{\sigma }_{2},\rho$ 均为常数,且 ${\sigma }_{1} > 0,{\sigma }_{2} > 0, - 1 < \rho  < 1$,则称 $\left( {X, Y}\right)$ 服从参数为 ${\mu }_{1},{\mu }_{2}$, ${\sigma }_{1},{\sigma }_{2},\rho$ 的二维正态分布,记作

$$
\left( {X, Y}\right)  \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2};{\mu }_{2},{\sigma }_{2}^{2};\rho }\right).
$$

特别,当 ${\mu }_{1} = {\mu }_{2} = 0,{\sigma }_{1} = {\sigma }_{2} = 1$ 时,则称 $\left( {X, Y}\right)$ 服从标准正态分布.

性质: $\left( {X, Y}\right)  \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2};{\mu }_{2},{\sigma }_{2}^{2};\rho }\right)  \Rightarrow  X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$. 逆命题不成立.

### 基本题型

#### 题型 1. 联合分布律与边缘分布律

【2.1】设随机变量 $X$ 在1,2,3,4四个整数中随机地取一值,另一随机变量 $Y$ 在 1 到 $X$ 中随机地取一整数. 求 $\left( {X, Y}\right)$ 的分布律及 $X$ 和 $Y$ 的边缘分布.

解 $X$ 可能的取值为 $i = 1,2,3,4, Y$ 可能的取值为 $j = 1,\cdots, i$. 由乘法定理得

$$
P\{ X = i, Y = j\}  = P\{ Y = j \mid  X = i\}  \cdot  P\{ X = i\}  = \left\{  \begin{array}{ll} \frac{1}{4} \cdot  \frac{1}{i}, & j \leq  i \\  0, & j > i \end{array}\right.
$$

故得 $X$ 和 $Y$ 的联合分布律为

<table><tr><td>$X$ Y</td><td>1</td><td>2</td><td>3</td><td>4</td></tr><tr><td>1</td><td>$\frac{1}{4}$</td><td>$\frac{1}{8}$</td><td>$\frac{1}{12}$</td><td>$\frac{1}{16}$</td></tr><tr><td>2</td><td>0</td><td>$\frac{1}{8}$</td><td>$\frac{1}{12}$</td><td>$\frac{1}{16}$</td></tr><tr><td>3</td><td>0</td><td>0</td><td>$\frac{1}{12}$</td><td>$\frac{1}{16}$</td></tr><tr><td>4</td><td>0</td><td>0</td><td>0</td><td>$\frac{1}{16}$</td></tr></table>

利用 ${p}_{i \cdot  } = \mathop{\sum }\limits_{j}{p}_{ij}$ 和 ${p}_{\cdot j} = \mathop{\sum }\limits_{i}{p}_{ij}$,求出 $\left( {X, Y}\right)$ 关于 $X$ 和 $Y$ 的边缘分布律,并写在联合分布律表格的边缘上, 可得下表

<table><tr><td>$X$ Y</td><td>1</td><td>2</td><td>3</td><td>4</td><td>$P\left\{  {Y = {y}_{j}}\right\}   = {p}_{\cdot j}$</td></tr><tr><td>1</td><td>$\frac{1}{4}$</td><td>$\frac{1}{8}$</td><td>$\frac{1}{12}$</td><td>$\frac{1}{16}$</td><td>$\frac{25}{48}$</td></tr><tr><td>2</td><td>0</td><td>$\frac{1}{8}$</td><td>$\frac{1}{12}$</td><td>$\frac{1}{16}$</td><td>$\frac{13}{48}$</td></tr><tr><td>3</td><td>0</td><td>0</td><td>$\frac{1}{12}$</td><td>$\frac{1}{16}$</td><td>$\frac{7}{48}$</td></tr><tr><td>4</td><td>0</td><td>0</td><td>0</td><td>$\frac{1}{16}$</td><td>$\frac{3}{48}$</td></tr><tr><td>$P\left\{  {X = {x}_{i}}\right\}   = {p}_{i}.$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{4}$</td><td>1</td></tr></table>

【2.2】设随机变量 ${X}_{i} \sim  \left\lbrack  \begin{matrix}  - 1 & 0 & 1 \\  \frac{1}{4} & \frac{1}{2} & \frac{1}{4} \end{matrix}\right\rbrack  \left( {i = 1,2}\right)$,且满足 $P\left\{  {{X}_{1}{X}_{2} = 0}\right\}   = 1$,则 $P\left\{  {X}_{1}\right.$ $\left. { = {X}_{2}}\right\}$ 等于(   ).

(A) 0 (B) $\frac{1}{4}$ (C) $\frac{1}{2}$ (D) 1

分析 $P\left\{  {{X}_{1}{X}_{2} = 0}\right\}   = 1$ 是解决本题的关键,隐含了 $P\left\{  {{X}_{1}{X}_{2} \neq  0}\right\}   = 0$. 由此条件再根据联合分布及边缘分布的关系计算.

解 由 $P\left\{  {{X}_{1}{X}_{2} = 0}\right\}   = 1 \Rightarrow  P\left\{  {{X}_{1}{X}_{2} \neq  0}\right\}   = 0$,即

$P\left\{  {{X}_{1} =  - 1,{X}_{2} =  - 1}\right\} , P\left\{  {{X}_{1} =  - 1,{X}_{2} = 1}\right\} , P\left\{  {{X}_{1} = 1,{X}_{2} =  - 1}\right\} , P\left\{  {{X}_{1} = 1,{X}_{2} = 1}\right\}$ 均为 0.

由以上条件求出, ${X}_{1},{X}_{2}$ 的联合概率分布如下表所示

<table><tr><td>${X}_{2}$ ${X}_{1}$</td><td>-1</td><td>0</td><td>1</td><td>${p}_{i \cdot  }$</td></tr><tr><td>-1</td><td>0</td><td>$\frac{1}{4}$</td><td>0</td><td>$\frac{1}{4}$</td></tr><tr><td>0</td><td>$\frac{1}{4}$</td><td>0</td><td>$\frac{1}{4}$</td><td>$\frac{1}{2}$</td></tr><tr><td>1</td><td>0</td><td>$\frac{1}{4}$</td><td>0</td><td>$\frac{1}{4}$</td></tr><tr><td>${p}_{\cdot j}$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{2}$</td><td>$\frac{1}{4}$</td><td>1</td></tr></table>

那么 $P\left\{  {{X}_{1} = {X}_{2}}\right\}   = P\left\{  {{X}_{1} =  - 1,{X}_{2} =  - 1}\right\}   + P\left\{  {{X}_{1} = 0,{X}_{2} = 0}\right\}   + P\left\{  {{X}_{1} = 1,{X}_{2} = 1}\right\}   = 0$.

点评 列表法是解决联合分布和边缘分布问题常用的方法, 直观明显.

【2.3】假设随机变量 $Y$ 服从 $\left( {0,3}\right)$ 上的均匀分布,随机变量

$$
{X}_{k} = \left\{  {\begin{array}{ll} 0, & Y \leq  k \\  1, & Y > k \end{array}\;\left( {k = 1,2}\right).}\right.
$$

求 ${X}_{1}$ 和 ${X}_{2}$ 的联合概率分布和边缘分布.

解 $\left( {{X}_{1},{X}_{2}}\right)$ 有四个可能值: $\left( {0,0}\right),\left( {0,1}\right),\left( {1,0}\right),\left( {1,1}\right)$.

易见

$$
P\left\{  {{X}_{1} = 0,{X}_{2} = 0}\right\}   = P\{ Y \leq  1, Y \leq  2\}  = P\{ Y \leq  1\}  = \frac{1}{3}
$$

$P\left\{  {{X}_{1} = 0,{X}_{2} = 1}\right\}   = P\{ Y \leq  1, Y > 2\}  = 0$

$P\left\{  {{X}_{1} = 1,{X}_{2} = 0}\right\}   = P\{ Y > 1, Y \leq  2\}  = P\{ 1 < Y \leq  2\}  = \frac{1}{3}$

$$
P\left\{  {{X}_{1} = 1,{X}_{2} = 1}\right\}   = P\{ Y > 1, Y > 2\}  = P\{ Y > 2\}  = \frac{1}{3}
$$

于是, ${X}_{1}$ 和 ${X}_{2}$ 联合概率分布表如下:

<table><tr><td>${X}_{1}$</td><td/><td/></tr><tr><td>${X}_{2}$</td><td>0</td><td>1</td></tr><tr><td>0</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td></tr><tr><td>1</td><td>0</td><td>$\frac{1}{3}$</td></tr></table>

由联合分布可求得 ${X}_{1},{X}_{2}$ 的边缘分布,合并列表为:

<table><tr><td>${X}_{1}$ ${X}_{2}$</td><td>0</td><td>1</td><td>${p}_{\cdot j}$</td></tr><tr><td>0</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td><td>$\frac{2}{3}$</td></tr><tr><td>1</td><td>0</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td></tr><tr><td>${p}_{i \cdot  }$</td><td>$\frac{1}{3}$</td><td>$\frac{2}{3}$</td><td>1</td></tr></table>

#### 题型 2. 联合分布函数与边缘分布函数

【2.4】已知二维随机变量 $\left( {X, Y}\right)$ 的分布函数为

$$
F\left( {x, y}\right)  = \frac{1}{{\pi }^{2}}\left( {\frac{\pi }{2} + \arctan \frac{x}{2}}\right) \left( {\frac{\pi }{2} + \arctan \frac{y}{2}}\right)
$$

$$
\left( {-\infty  < x <  + \infty, - \infty  < y <  + \infty }\right).
$$

试求 $\left( {X, Y}\right)$ 关于 $X, Y$ 的边缘分布函数.

解 分别运用公式得

$$
{F}_{X}\left( x\right)  = F\left( {x, + \infty }\right)  = \frac{1}{\pi }\left( {\frac{\pi }{2} + \arctan \frac{x}{2}}\right) \;\left( {-\infty  < x <  + \infty }\right)
$$

$$
{F}_{Y}\left( y\right)  = F\left( {+\infty, y}\right)  = \frac{1}{\pi }\left( {\frac{\pi }{2} + \arctan \frac{y}{2}}\right) \;\left( {-\infty  < y <  + \infty }\right)
$$

#### 题型 3. 联合概率密度与边缘密度

【2.5】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & 0 < x < y \\  0, & \text{ 其他. } \end{array}\right.
$$

(1)求随机变量 $X$ 的密度 ${f}_{X}\left( x\right)$;

(2)求概率 $P\{ X + Y \leq  1\}$.

解 (1) 由联合密度与边缘概率密度关系可知

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y.
$$

当 $x \leq  0$ 时, $f\left( {x, y}\right)  = 0,{f}_{X}\left( x\right)  = 0$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_88_983_1230_329_270_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_88_983_1230_329_270_0.jpg)

图 3-2.5

当 $x > 0$ 时, ${f}_{X}\left( x\right)  = {\int }_{x}^{+\infty }{\mathrm{e}}^{-y}\mathrm{\;d}y = {\mathrm{e}}^{-x}$

所以 ${f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0. \end{array}\right.$

(2)根据题意,作图 3-2.5

$$
P\{ X + Y \leq  1\}  = {\iint }_{x + y \leq  1}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{\frac{1}{2}}\mathrm{\;d}x{\int }_{x}^{1 - x}{\mathrm{e}}^{-y}\mathrm{\;d}y
$$

$$
= 1 - \frac{2}{{\mathrm{e}}^{\frac{1}{2}}} + \frac{1}{\mathrm{e}}
$$

点评 由联合密度求边缘密度时,要注意讨论范围及积分定限,必要时将 $f\left( {x, y}\right)$ 的非零区域用图形表示,便于分析.

【2.6】设平面区域 $D$ 由曲线 $y = \frac{1}{x}$ 及直线 $y = 0, x = 1, x = {\mathrm{e}}^{2}$ 所围成. 二维随机变量 $\left( {X, Y}\right)$ 在区域 $D$ 上服从均匀分布,则 $\left( {X, Y}\right)$ 关于 $X$ 的边缘概率密度在 $x = 2$ 处的值为_____.

解 区域 $D$ 的面积

$$
{S}_{D} = {\int }_{1}^{{\mathrm{e}}^{2}}\frac{1}{x}\mathrm{\;d}x = {\left. \ln x\right| }_{1}^{{\mathrm{e}}^{2}} = 2
$$

所以二维随机变量 $\left( {X, Y}\right)$ 的联合分布密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{2}, & \text{ 当 }\left( {x, y}\right)  \in  D \\  0, & \text{ 其他 } \end{array}\right.
$$

则 $\left( {X, Y}\right)$ 关于 $X$ 的边缘概率密度

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = {\int }_{0}^{\frac{1}{x}}\frac{1}{2}\mathrm{\;d}y = {\left. \frac{1}{2x},\;{f}_{X}\left( x\right) \right| }_{x = 2} = \frac{1}{4}
$$

故应填 $\frac{1}{4}$.

题型 4 : 关于重要的二维分布

【2.7】设 $\left( {X, Y}\right)$ 服从区域 $D$ 上的均匀分布,其中 $D : x \geq  y,0 \leq  x \leq  1, y \geq  0$,求 $P\{ X + Y$ $\leq  1\}$.

解法一 因为 $D$ 的面积 $A = \frac{1}{2}$,所以 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} 2, & \left( {x, y}\right)  \in  D \\  0, & \text{ 其他 } \end{array}\right.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_89_1031_925_312_222_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_89_1031_925_312_222_0.jpg)

图 3-2.7

则 $P\{ X + Y \leq  1\}  = {\iint }_{x + y \leq  1}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y$

$= {\iint }_{{D}_{1}}2\mathrm{\;d}x\mathrm{\;d}y\;$ (如图 3-2.7)

$= 2 \times  \frac{1}{4} = \frac{1}{2}$.

解法二 可利用几何概率计算

$$
P\{ X + Y \leq  1\}  = \frac{S\left( {D}_{1}\right) }{S\left( D\right) } = \frac{1}{2}.
$$

点评 二维均匀分布求概率可以利用几何概型来计算, 更加简便.

【2.8】设 $\left( {X, Y}\right)$ 服从二维正态分布,概率密度为

$$
f\left( {x, y}\right)  = \frac{1}{{2\pi } \times  {10}^{2}}{\mathrm{e}}^{-\frac{{x}^{2} + {y}^{2}}{2 \times  {10}^{2}}},
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_89_1027_1365_314_242_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_89_1027_1365_314_242_0.jpg)

图 3-2.8

求 $P\{ Y \geq  X\}$.

解 $P\{ Y \geq  X\}  = {\iint }_{y \geq  x}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y$ (如图 3-2.8)

$$
= {\iint }_{y \geq  x}\frac{1}{{2\pi } \times  {10}^{2}}{\mathrm{e}}^{\frac{{x}^{2} + {y}^{2}}{2 \times  {10}^{2}}}\mathrm{\;d}x\mathrm{\;d}y
$$

(利用极坐标法)

$$
= \frac{1}{{2\pi } \times  {10}^{2}}{\int }_{\frac{\pi }{4}}^{\frac{5\pi }{4}}\mathrm{\;d}\theta {\int }_{0}^{+\infty }{\mathrm{e}}^{-\frac{{r}^{2}}{2 \times  {10}^{2}}} \cdot  r\mathrm{\;d}r
$$

$$
=  - \frac{1}{2}{\int }_{0}^{+\infty }{\mathrm{e}}^{\frac{{r}^{2}}{2 \times  {10}^{2}}}\mathrm{\;d}\left( {-\frac{{r}^{2}}{2 \times  {10}^{2}}}\right)  =  - {\left. \frac{1}{2}{\mathrm{e}}^{\frac{{r}^{2}}{2 \times  {10}^{2}}}\right| }_{0}^{+\infty }
$$

$$
= \frac{1}{2}\text{.}
$$

## §3. 条件分布

### 知识要点

1. 条件分布律 设 $\left( {X, Y}\right)$ 是二维离散型随机变量,若 $p.j > 0$,则称

$$
{p}_{X \mid  Y}\left( {i \mid  j}\right)  = P\left\{  {X = {x}_{i} \mid  Y = {y}_{j}}\right\}   = \frac{{p}_{ij}}{p \cdot  j}\;\left( {i = 1,2,\cdots }\right)
$$

为在 $\left\{  {Y = {y}_{j}}\right\}$ 条件下随机变量 $X$ 的条件分布律.

若 ${p}_{i}$. > 0,则称

$$
{p}_{Y \mid  X}\left( {j \mid  i}\right)  = P\left\{  {Y = {y}_{j} \mid  X = {x}_{i}}\right\}   = \frac{{p}_{ij}}{{p}_{i}}\;\left( {j = 1,2,\cdots }\right)
$$

为在 $\left\{  {X = {x}_{i}}\right\}$ 条件下随机变量 $Y$ 的条件分布律.

1. 条件概率密度 设 $\left( {X, Y}\right)$ 是二维连续型随机变量,若 ${f}_{Y}\left( y\right)  > 0$,则称

$$
{f}_{X \mid  Y}\left( {x \mid  y}\right)  = \frac{f\left( {x, y}\right) }{{f}_{Y}\left( y\right) }\;\left( {-\infty  < x <  + \infty }\right)
$$

为在 $\{ Y = y\}$ 条件下 $X$ 的条件概率密度.

若 ${f}_{X}\left( x\right)  > 0$,则称

$$
{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{f\left( {x, y}\right) }{{f}_{X}\left( x\right) }\;\left( {-\infty  < y <  + \infty }\right)
$$

为在 $\{ X = x\}$ 条件下 $Y$ 的条件概率密度.

### 基本题型

题型 1. 求条件分布律

【3.1】求 $§2$ 例子【2.1】中的条件分布律: $P\{ Y = k \mid  X = i\}$

解 $P\{ Y = k \mid  X = i\}  = \frac{P\{ Y = k, X = i\} }{P\{ X = i\} }$,而

$$
P\{ X = k, X = i\}  = \frac{1}{i} \cdot  \frac{1}{4},\;i = 1,2,3,4, k \leq  i
$$

$$
P\{ X = i\}  = \frac{1}{4}
$$

所以 $P\{ Y = k \mid  X = i\}  = \frac{1}{i},\;i = 1,2,3,4, k \leq  i$. 即概率论与数理统计习题精选精解

<table><tr><td>$k$</td><td>1</td></tr><tr><td>$P\{ Y = k \mid  X = 1\}$</td><td>1</td></tr></table>

<table><tr><td>$k$</td><td>1</td><td>2</td><td/></tr><tr><td>$P\{ Y = k \mid  X = 3\}$</td><td>$\frac{1}{3}$</td><td/><td/></tr></table>

<table><tr><td>$k$1</td><td>2</td></tr><tr><td>$P\{ Y = k \mid  X = 2\}$$\frac{1}{2}$</td><td>$\frac{1}{2}$</td></tr></table>

<table><tr><td>$k$</td><td/><td/><td/><td/></tr><tr><td>$P\{ Y = k \mid  X = 4\}$</td><td/><td/><td/><td>$\begin{array}{lll} \frac{1}{4} & \frac{1}{4} & \frac{1}{4} \end{array}$</td></tr></table>

#### 题型 2. 条件密度的计算及应用

【3.2】设随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} 1, & \left| y\right|  < x,0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

求条件概率密度 ${f}_{Y \mid  X}\left( {y \mid  x}\right),\;{f}_{X \mid  Y}\left( {x \mid  y}\right)$.

解 由于概率密度 $f\left( {x, y}\right)$ 仅在图 3-3.2 中阴影部分为非零值.

故 $f\left( {x, y}\right)$ 的边缘密度为

$$
{f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} {\int }_{-x}^{x}1\mathrm{\;d}y, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array} = \left\{  \begin{array}{ll} {2x}, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right. }\right.
$$

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\int }_{\left| y\right| }^{1}1\mathrm{\;d}x, &  - 1 < y < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} 1 - \left| y\right|, &  - 1 < y < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_91_1046_681_297_317_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_91_1046_681_297_317_0.jpg)

图 3-3.2

所以当 $0 < x < 1$ 时,

${f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{f\left( {x, y}\right) }{{f}_{X}\left( x\right) } = \left\{  \begin{array}{ll} \frac{1}{2x}, & \left| y\right|  < x \\  0, & \text{ 其他 } \end{array}\right.$

当 $\left| y\right|  < 1$ 时, ${f}_{X \mid  Y}\left( {x \mid  y}\right)  = \frac{f\left( {x, y}\right) }{{f}_{Y}\left( y\right) } = \left\{  \begin{array}{ll} \frac{1}{1 - \left| y\right| }, & \left| y\right|  < x < 1 \\  0, & \text{ 其他 } \end{array}\right.$

【3.3】设二维随机变量 $\left( {X, Y}\right)$ 服从区域 $D : {x}^{2} + {y}^{2} \leq  1$ 上的均匀分布,求条件密度函数和条件概率 $P\left\{  {X > \frac{1}{2} \mid  Y = 0}\right\}$.

解 由于 $\left( {X, Y}\right)$ 服从均匀分布,易知

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{\pi }, & {x}^{2} + {y}^{2} \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

由 ${f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y$,求得

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{2\sqrt{1 - {x}^{2}}}{\pi }, &  - 1 \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

同理可得

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{2\sqrt{1 - {y}^{2}}}{\pi }, &  - 1 \leq  y \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

当 $- 1 < y < 1$ 时

$$
{f}_{X \mid  Y}\left( {x \mid  y}\right)  = \frac{f\left( {x, y}\right) }{{f}_{Y}\left( y\right) } = \left\{  \begin{array}{ll} \frac{1}{2\sqrt{1 - {y}^{2}}}, &  - \sqrt{1 - {y}^{2}} \leq  x \leq  \sqrt{1 - {y}^{2}} \\  0, & \text{ 其他 } \end{array}\right.
$$

同理,当 $- 1 < x < 1$ 时

$$
{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{f\left( {x, y}\right) }{{f}_{X}\left( x\right) } = \left\{  \begin{array}{ll} \frac{1}{2\sqrt{1 - {x}^{2}}}, &  - \sqrt{1 - {x}^{2}} \leq  y \leq  \sqrt{1 - {x}^{2}} \\  0, & \text{ 其他 } \end{array}\right.
$$

当 $y = 0$ 时, ${f}_{X \mid  Y}\left( {x \mid  0}\right)  = \left\{  \begin{array}{ll} \frac{1}{2}, &  - 1 \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.$

$$
P\left\{  {X > \frac{1}{2} \mid  Y = 0}\right\}   = {\int }_{\frac{1}{2}}^{+\infty }{f}_{X \mid  Y}\left( {x \mid  0}\right) \mathrm{d}x = {\int }_{\frac{1}{2}}^{1}\frac{1}{2}\mathrm{\;d}x = \frac{1}{4}.
$$

【3.4】设随机变量 $X$ 在区间 $\left( {0,1}\right)$ 上服从均匀分布,在 $X = x\left( {0 < x < 1}\right)$ 的条件下,随机变量 $Y$ 在区间 $\left( {0, x}\right)$ 上服从均匀分布,求:

(1)随机变量 $X$ 和 $Y$ 的联合概率密度； (2) $Y$ 的概率密度; (3)概率 $P\{ X + Y > 1\}$.

解 (1) $X$ 的概率密度为 ${f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} 1, & 0 < x < 1 \\  0, & \text{ 其他. } \end{array}\right.$

在 $X = x\left( {0 < x < 1}\right)$ 条件下, $Y$ 的条件密度为

$$
{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \left\{  \begin{array}{ll} \frac{1}{x}, & 0 < y < x \\  0, & \text{ 其他 } \end{array}\right.
$$

当 $0 < y < x < 1$ 时,随机变量 $X$ 和 $Y$ 的联合概率密度为

$$
f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{1}{x}
$$

在其他点 $\left( {x, y}\right)$ 处,有 $f\left( {x, y}\right)  = 0$,即

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{x}, & 0 < y < x < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

(2)当 $0 < y < 1$ 时, $Y$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = {\int }_{y}^{1}\frac{1}{x}\mathrm{\;d}x =  - \ln y
$$

当 $y \leq  0$ 或 $y \geq  1$ 时, ${f}_{Y}\left( y\right)  = 0$,因此 ${f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll}  - \ln y, & 0 < y < 1 \\  0, & \text{ 其他 } \end{array}\right.$

(3)所求概率

$$
P\{ X + Y > 1\}  = {\iint }_{x + y > 1}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{\frac{1}{2}}^{1}\mathrm{\;d}x{\int }_{1 - x}^{x}\frac{1}{x}\mathrm{\;d}y = {\int }_{\frac{1}{2}}^{1}\left( {2 - \frac{1}{x}}\right) \mathrm{d}x = 1 - \ln 2.
$$

## § 4. 随机变量的独立性

### 知识要点

1. 随机变量的独立性 若二维随机变量 $\left( {X, Y}\right)$ 对任意实数均有

$P\{ X \leq  x, Y \leq  y\}  = P\{ X \leq  x\} P\{ Y \leq  y\},\;$ 即 $F\left( {x, y}\right)  = {F}_{X}\left( x\right)  \cdot  {F}_{Y}\left( y\right),$ 则 $X$ 与 $Y$ 相互独立.

2. 离散型随机变量相互独立的充要条件

$$
{p}_{ij} = {p}_{i} \cdot  {p}_{\cdot j},\;i, j = 1,2,\cdots.
$$

3. 连续型随机变量相互独立的充要条件

$$
f\left( {x, y}\right)  = {f}_{X}\left( x\right)  \cdot  {f}_{Y}\left( y\right),\;x, y\text{任意实数.}
$$

### 基本题型

#### 题型 1. 随机变量独立性的判断问题

【4.1】设随机变量 ${X}_{1}$ 和 ${Y}_{2}$ 的概率分布为

$$
{X}_{1} \sim  \left\lbrack  \begin{matrix}  - 1 & 0 & 1 \\  \frac{1}{4} & \frac{1}{2} & \frac{1}{4} \end{matrix}\right\rbrack
$$

$$
{X}_{2} \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  \frac{1}{2} & \frac{1}{2} \end{matrix}\right\rbrack
$$

而且 $P\left\{  {{X}_{1}{X}_{2} = 0}\right\}   = 1$.

试求: (1) ${X}_{1}$ 和 ${X}_{2}$ 的联合分布; (2) ${X}_{1}$ 和 ${X}_{2}$ 是否独立?

解 (1) 因为 $P\left\{  {{X}_{1}{X}_{2} = 0}\right\}   = 1$,所以有 $P\left\{  {{X}_{1}{X}_{2} \neq  0}\right\}   = 0$,因此

$$
P\left\{  {{X}_{1} =  - 1,{X}_{2} = 1}\right\}   = P\left\{  {{X}_{1} = 1,{X}_{2} = 1}\right\}   = 0
$$

那么 $P\left\{  {{X}_{1} =  - 1,{X}_{2} = 0}\right\}   = P\left\{  {{X}_{1} =  - 1}\right\}   = \frac{1}{4}$

$$
P\left\{  {{X}_{1} = 0,{X}_{2} = 0}\right\}   = P\left\{  {{X}_{2} = 1}\right\}   = \frac{1}{2}
$$

$$
P\left\{  {{X}_{1} = 1,{X}_{2} = 0}\right\}   = P\left\{  {{X}_{1} = 1}\right\}   = \frac{1}{4}
$$

$$
P\left\{  {{X}_{1} = 0,{X}_{2} = 0}\right\}   = 1 - \left( {\frac{1}{4} + \frac{1}{2} + \frac{1}{4}}\right)  = 0
$$

${X}_{1}$ 和 ${X}_{2}$ 的联合分布列表为

<table><tr><td>${X}_{1}$ ${X}_{2}$</td><td>-1</td><td>0</td><td>1</td><td>$P\left\{  {{X}_{2} = j}\right\}$</td></tr><tr><td>0</td><td>$\frac{1}{4}$</td><td>0</td><td>$\frac{1}{4}$</td><td>$\frac{1}{2}$</td></tr><tr><td>1</td><td>0</td><td>$\frac{1}{2}$</td><td>0</td><td>$\frac{1}{2}$</td></tr><tr><td>$P\left\{  {{X}_{1} = i}\right\}$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{2}$</td><td>$\frac{1}{4}$</td><td>1</td></tr></table>

(2) 由于 $P\left\{  {{X}_{1} = 0,{X}_{2} = 0}\right\}   = 0 \neq  P\left\{  {{X}_{1} = 0}\right\}  P\left\{  {{X}_{2} = 0}\right\}   = \frac{1}{2} \times  \frac{1}{2} = \frac{1}{4}$,所以 ${X}_{1}$ 与 ${X}_{2}$ 不相互独立.

点评 两随机变量独立的充要条件是解决相互独立性问题最直接最重要的方法.

【4.2】设二维随机变量 $\left( {X, Y}\right)$ 的联合概率密度函数为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1 + {xy}}{4}, & \left| x\right|  < 1,\left| y\right|  < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

证明 $X$ 与 $Y$ 不独立,但 ${X}^{2}$ 与 ${Y}^{2}$ 独立.

证 对 $X, Y$ 而言:

$$
{f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} \frac{1}{2}, & \left| x\right|  < 1 \\  0, & \text{ 其他 } \end{array}\;{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{2}, & \left| y\right|  < 1 \\  0, & \text{ 其他 } \end{array}\right. }\right.
$$

因为 $f\left( {x, y}\right)  \neq  {f}_{X}\left( x\right) {f}_{Y}\left( y\right)$,所以 $X, Y$ 不独立.

而

$$
{F}_{U}\left( u\right)  = P\left\{  {{X}^{2} \leq  u}\right\}   = \left\{  \begin{array}{ll} 0, & u < 0 \\  \sqrt{u}, & 0 \leq  u < 1 \\  1, & u \geq  1 \end{array}\right.
$$

$$
{F}_{V}\left( v\right)  = P\left\{  {{Y}^{2} \leq  v}\right\}   = \left\{  \begin{array}{ll} 0, & v < 0 \\  \sqrt{v}, & 0 \leq  v < 1 \\  1, & v \geq  1 \end{array}\right.
$$

$U = {X}^{2}, V = {Y}^{2}$ 的联合分布函数为

$$
F\left( {u, v}\right)  = P\left\{  {{X}^{2} \leq  u,{Y}^{2} \leq  v}\right\}   = \left\{  \begin{array}{ll} 0, & u < 0\text{ 或 }v < 0 \\  \sqrt{uv}, & 0 \leq  u < 1,0 \leq  v < 1 \\  \sqrt{u}, & 0 \leq  u < 1,1 \leq  v \\  \sqrt{v}, & 1 \leq  u,0 \leq  v < 1 \\  1, & 1 \leq  u,1 \leq  v \end{array}\right.
$$

可见,对 $U = {X}^{2}, V = {Y}^{2}$ 而言,有 $F\left( {u, v}\right)  = {F}_{U}\left( u\right) {F}_{V}\left( v\right)$ 即 ${X}^{2}$ 和 ${Y}^{2}$ 相互独立.

【4.3】设随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} {Ax}{y}^{2}, & 0 < x < 1,0 < y < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

求:(1)常数 $A$;(2)证明 $X$ 与 $Y$ 相互独立.

解 (1) 由性质 ${\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = 1$,可知 $\frac{A}{6} = 1$,则 $A = 6$.

(2)边缘密度为

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  \begin{array}{ll} {2x}, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
{f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = \left\{  \begin{array}{ll} 3{y}^{2}, & 0 < y < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

显然, $f\left( {x, y}\right)  = {f}_{X}\left( x\right)  \cdot  {f}_{Y}\left( y\right)$.

故 $X, Y$ 相互独立.

【4.4】一个电子仪器由两个部件构成,以 $X$ 和 $Y$ 分别表示两个部件的寿命(单位:千小时). 已知 $X$ 和 $Y$ 的联合分布函数为:

$$
F\left( {x, y}\right)  = \left\{  \begin{array}{l} 1 - {\mathrm{e}}^{-{0.5x}} - {\mathrm{e}}^{-{0.5y}} + {\mathrm{e}}^{-{0.5}\left( {x + y}\right) }, \\  0, \end{array}\right.
$$

若 $x \geq  0, y \geq  0$ 其他

(1)问 $X$ 和 $Y$ 是否独立?

(2)求两个部件的寿命都超过 100 小时的概率 $\alpha$.

解 (1) 由 $F\left( {x, y}\right)$ 易知 $X, Y$ 的边缘分布函数

$$
{F}_{X}\left( x\right)  = F\left( {x, + \infty }\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{0.5x}}, & x \geq  0 \\  0, & x < 0. \end{array}\right.
$$

$$
{F}_{Y}\left( y\right)  = F\left( {+\infty, y}\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{0.5y}}, & y \geq  0 \\  0, & y < 0. \end{array}\right.
$$

因为若 $x \geq  0, y \geq  0$,有

$$
{F}_{X}\left( x\right) {F}_{Y}\left( y\right)  = \left( {1 - {\mathrm{e}}^{-{0.5x}}}\right) \left( {1 - {\mathrm{e}}^{-{0.5y}}}\right)  = 1 - {\mathrm{e}}^{-{0.5x}} - {\mathrm{e}}^{-{0.5y}} + {\mathrm{e}}^{-{0.5}\left( {x + y}\right) }
$$

当 $x, y$ 为其他情况时, ${F}_{X}\left( x\right) {F}_{Y}\left( y\right)  = 0$.

所以对任意实数 $x, y$ 都有 $F\left( {x, y}\right)  = {F}_{X}\left( x\right) {F}_{Y}\left( y\right)$,故 $X$ 与 $Y$ 相互独立.

(2)由题意可知

$$
\alpha  = P\{ X > {0.1}, Y > {0.1}\}  = P\{ X > {0.1}\} P\{ Y > {0.1}\}
$$

$$
= \left\lbrack  {1 - {F}_{X}\left( {0.1}\right) }\right\rbrack  \left\lbrack  {1 - {F}_{Y}\left( {0.1}\right) }\right\rbrack   = {\mathrm{e}}^{-{0.05}}{\mathrm{e}}^{-{0.05}} = {\mathrm{e}}^{-{0.1}}
$$

#### 题型 2. 独立性的应用

【4.5】设 $\left( {\xi,\eta }\right)$ 的联合分布律为:

<table><tr><td>$\eta$ ξ</td><td>0</td><td>1</td><td>2</td></tr><tr><td>-1</td><td>$\frac{1}{6}$</td><td>$\frac{1}{9}$</td><td>$\frac{1}{18}$</td></tr><tr><td>1</td><td>$\frac{1}{3}$</td><td>$A$</td><td>$B$</td></tr></table>

试求: $A\text{、}B$ 为何值时随机变量 $\xi,\eta$ 相互独立.

分析 对于此类确定概率的问题需要考虑的是 $\xi,\eta$ 独立的充要条件是对一切 $i, j$ 都要满足 ${p}_{ij} = {p}_{i} \cdot  {p}_{\cdot j}.$

解 由 $\left( {\xi,\eta }\right)$ 的联合分布律可得到

$$
{p}_{1}. = \frac{1}{6} + \frac{1}{9} + \frac{1}{18} = \frac{1}{3},\;{p}_{2}. = \frac{1}{3} + A + B,
$$

$$
{p}_{.1} = \frac{1}{6} + \frac{1}{3} = \frac{1}{2},\;{p}_{.2} = \frac{1}{9} + A,\;{p}_{.3} = \frac{1}{18} + B.
$$

若 $\xi,\eta$ 相互独立,则必有对一切 $i, j$ 均满足 ${p}_{ij} = {p}_{i}.{p}_{\cdot j}$,得

$$
\left\{  \begin{array}{l} {p}_{1} \cdot  {p}_{1 \cdot  1} = \frac{1}{3} \times  \frac{1}{2} = \frac{1}{6} \\  {p}_{1} \cdot  {p}_{2 \cdot  2} = \frac{1}{3} \times  \left( {\frac{1}{9} + A}\right)  = \frac{1}{9} \\  {p}_{1} \cdot  {p}_{3 \cdot  2} = \frac{1}{3} \times  \left( {\frac{1}{18} + B}\right)  = \frac{1}{18} \\  {p}_{2} \cdot  {p}_{1 \cdot  1} = \left( {\frac{1}{3} + A + B}\right)  \times  \frac{1}{2} = \frac{1}{3} \\  {p}_{2} \cdot  {p}_{2 \cdot  2} = \left( {\frac{1}{3} + A + B}\right)  \times  \left( {\frac{1}{9} + A}\right)  = A \\  {p}_{3} \cdot  {p}_{3 \cdot  3} = \left( {\frac{1}{3} + A + B}\right)  \times  \left( {\frac{1}{9} + B}\right)  = B \end{array}\right.
$$

解方程组得 $A = \frac{2}{9}, B = \frac{1}{9}$.

【4.6】设随机变量 $X$ 和 $Y$ 相互独立,下表列出随机变量 $\left( {X, Y}\right)$ 联合分布律及关于 $X$ 和 $Y$ 的边缘分布律中的部分数值, 试将其余数值填入表中空白处.

<table><tr><td>Y $X$</td><td>${y}_{1}$</td><td/><td>${y}_{3}$</td><td>$P\left\{  {X = {x}_{i}}\right\}   = {p}_{i}.$</td></tr><tr><td>${x}_{1}$</td><td/><td>$\frac{1}{8}$</td><td/><td/></tr><tr><td>${x}_{2}$</td><td>$\frac{1}{8}$</td><td/><td/><td/></tr><tr><td>$P\left\{  {Y = {y}_{j}}\right\}   = {p}_{\cdot j}$</td><td>$\frac{1}{6}$</td><td/><td/><td>1</td></tr></table>

分析 运用边缘分布公式及随机变量的独立性,题中只有先考察 $j = 1$ 时的情况才可逐次求出其他值.

解 因为 ${p}_{.1} = \mathop{\sum }\limits_{{i = 1}}^{2}{p}_{i1} = \frac{1}{6} = {p}_{11} + {p}_{21} = {p}_{11} + \frac{1}{8}$,得 ${p}_{11} = \frac{1}{24}$.

由独立性, ${p}_{11} = {p}_{1}. \cdot  {p}_{\cdot 1}\;$ 即 $\frac{1}{24} = {p}_{1}. \cdot  \frac{1}{6}$,故 ${p}_{1}. = \frac{1}{4}$.

同理其余值依次求出: ${p}_{13} = \frac{1}{12},\;{p}_{22} = \frac{3}{8},\;{p}_{23} = \frac{1}{4}$

${p}_{.2} = \frac{1}{2},\;{p}_{.3} = \frac{1}{3},\;{p}_{2.} = \frac{3}{4}$

所以列表得概率论与数理统计习题精选精解

<table><tr><td>$Y$ $X$</td><td>${y}_{1}$</td><td>${y}_{2}$</td><td>${y}_{3}$</td><td>$P\left\{  {X = {x}_{i}}\right\}   = {p}_{i}.$</td></tr><tr><td>${x}_{1}$</td><td>$\frac{1}{24}$</td><td>$\frac{1}{8}$</td><td>$\frac{1}{12}$</td><td>$\frac{1}{4}$</td></tr><tr><td>${x}_{2}$</td><td>$\frac{1}{8}$</td><td>$\frac{3}{8}$</td><td>$\frac{1}{4}$</td><td>$\frac{3}{4}$</td></tr><tr><td>$P\left\{  {Y = {y}_{j}}\right\}   = {p}_{\cdot j}$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{2}$</td><td>$\frac{1}{3}$</td><td>1</td></tr></table>

【4.7】设随机变量 $X$ 和 $Y$ 相互独立,它们的密度函数分别为

$$
{f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\;{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0 \end{array}\right. }\right.
$$

求: $\left( 1\right) \left( {X, Y}\right)$ 的密度函数; $\left( 2\right) P\{ X \leq  1 \mid  Y > 0\}$.

解 (1) 因为随机变量 $X$ 和 $Y$ 相互独立,

$$
f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-\left( {x + y}\right) }, & x > 0, y > 0 \\  0, & \text{ 其他 } \end{array}\right.
$$

(2) $P\{ X \leq  1 \mid  Y > 0\}  = \frac{P\{ X \leq  1, Y > 0\} }{P\{ Y > 0\} } = \frac{{\int }_{-\infty }^{1}{\int }_{0}^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y}{{\int }_{0}^{+\infty }{f}_{Y}\left( y\right) \mathrm{d}y} = 1 - {\mathrm{e}}^{-1}$.

或者由独立性:

$$
P\{ X \leq  1 \mid  Y > 0\}  = P\{ X \leq  1\}  = {F}_{X}\left( 1\right)  = 1 - {\mathrm{e}}^{-1}.
$$

【4.8】设随机变量 $X$ 和 $Y$ 相互独立,且 $X$ 和 $Y$ 的概率分布分别为

<table><tr><td>Y</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td></tr></table>

则 $P\{ X + Y = 2\}  =$ _____.

(A) $\frac{1}{12}$ (B) $\frac{1}{8}$ (C) $\frac{1}{6}$ (D) $\frac{1}{2}$

解 $P\{ X + Y = 2\}  = P\{ X = 1, Y = 1\}  + P\{ X = 2, Y = 0\}  + P\{ X = 3, Y =  - 1\}$

$= P\{ X = 1\} P\{ Y = 1\}  + P\{ X = 2\} P\{ Y = 0\}  + P\{ X = 3\} P\{ Y =  - 1\}$

$= \frac{1}{6}$.

故应选 (C).

【4.9】设随机变量 $X$ 与 $Y$ 相互独立,且均服从区间 $\left\lbrack  {0,3}\right\rbrack$ 上的均匀分布,则 $P\{ \max \{ X, Y\}  \leq$ $1\}  =$ _____.

解法一 $X$ 与 $Y$ 具有相同的概率密度

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{3}, & 0 \leq  x \leq  3 \\  0, & \text{ 其他. } \end{array}\right.
$$

则 $P\{ X \leq  1\}  = P\{ Y \leq  1\}  = \frac{1}{3}$. 中 98

由 $X, Y$ 独立性可知:

$$
P\{ \max \{ X, Y\}  \leq  1\}  = P\{ X \leq  1, Y \leq  1\}
$$

$$
= P\{ X \leq  1\} P\{ Y \leq  1\}  = \frac{1}{9}.
$$

解法二 本题也可运用几何概率计算:

$$
P\{ \max \{ X, Y\}  \leq  1\}  = P\{ X \leq  1, Y \leq  1\}  = \frac{S\text{ 阴影 }}{S} = \frac{1}{9}
$$

(图 3-4.9)

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_98_642_498_316_290_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_98_642_498_316_290_0.jpg)

图 3-4.9

## $§5$. 多维随机变量函数的分布

### 知识要点

#### 1. 二维随机变量函数的分布

(1)已知离散型随机变量 $\left( {X, Y}\right)$ 的分布律 $P\left\{  {X = {x}_{i}, Y = {y}_{j}}\right\}   = {p}_{ij}$,则 $Z = g\left( {X, Y}\right)$ 的分布为

$$
P\left\{  {Z = {z}_{k}}\right\}   = P\left\{  {g\left( {X, Y}\right)  = {z}_{k}}\right\}   = \mathop{\sum }\limits_{{g\left( {{x}_{i},{y}_{j}}\right)  = {z}_{k}}}{p}_{ij}
$$

(2)设连续型随机变量 $\left( {X, Y}\right)$ 的概率密度为 $f\left( {x, y}\right)$,则 $Z = g\left( {X, Y}\right)$ 的分布函数为

$$
{F}_{Z}\left( z\right)  = P\{ Z \leq  z\}  = {\iint }_{g\left( {x, y}\right)  \leq  z}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y,
$$

概率密度 ${f}_{Z}\left( z\right)  = {F}_{Z}{}^{\prime }\left( z\right)$.

特殊类型:

① $Z = X + Y$ 密度函数为

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, z - x}\right) \mathrm{d}x = {\int }_{-\infty }^{+\infty }f\left( {z - y, y}\right) \mathrm{d}y,
$$

特别,当 $X$ 与 $Y$ 相互独立时

$$
{f}_{Z}\left( z\right)  = {f}_{X} * {f}_{Y} = {\int }_{-\infty }^{+\infty }{f}_{X}\left( x\right) {f}_{Y}\left( {z - x}\right) \mathrm{d}x = {\int }_{-\infty }^{+\infty }{f}_{X}\left( {z - y}\right) {f}_{Y}\left( y\right) \mathrm{d}y.
$$

概率论与数理统计习题精选精解

② 设 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$,且 $X, Y$ 相互独立,则

$$
{aX} + {bY} \sim  N\left( {a{\mu }_{1} + b{\mu }_{2},{a}^{2}{\sigma }_{1}^{2} + {b}^{2}{\sigma }_{2}^{2}}\right).
$$

③ 设 $X, Y$ 相互独立,分布函数分别为 ${F}_{X}\left( x\right)$ 和 ${F}_{Y}\left( y\right), M = \max \left( {X, Y}\right), N = \min \left( {X, Y}\right)$, 则

$$
{F}_{M}\left( z\right)  = {F}_{X}\left( z\right) {F}_{Y}\left( z\right),
$$

$$
{F}_{N}\left( z\right)  = 1 - \left\lbrack  {1 - {F}_{X}\left( z\right) }\right\rbrack  \left\lbrack  {1 - {F}_{Y}\left( z\right) }\right\rbrack .
$$

④ $Z = \frac{X}{Y}$ 的密度函数为

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| y\right| f\left( {{yz}, y}\right) \mathrm{d}y,
$$

当 $X, Y$ 相互独立时,

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| y\right| {f}_{X}\left( {yz}\right) {f}_{Y}\left( y\right) \mathrm{d}y.
$$

⑤ $Z = \frac{Y}{X}$ 的密度函数为

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| x\right| f\left( {x,{xz}}\right) \mathrm{d}x,
$$

当 $X, Y$ 相互独立时,

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| x\right| {f}_{X}\left( x\right) {f}_{Y}\left( {xz}\right) \mathrm{d}x.
$$

⑥ $Z = {XY}$ 的密度函数为

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\frac{1}{\left| x\right| }f\left( {x,\frac{z}{x}}\right) \mathrm{d}x,
$$

当 $X, Y$ 相互独立时,

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\frac{1}{\left| x\right| }{f}_{X}\left( x\right) {f}_{Y}\left( \frac{z}{x}\right) \mathrm{d}x.
$$

#### 2. 多维随机变量函数的分布

对于相互独立的多维随机变量所构成的简单函数, 可利用二维随机变量的结果加以推广. 常用结论及公式如下:

(1)设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 相互独立,且 ${X}_{i} \sim  N\left( {{\mu }_{i},{\sigma }_{i}^{2}}\right),{k}_{i}$ 为任意常数, $\left( {i = 1,2,\cdots, n}\right)$,则

$$
Z = \mathop{\sum }\limits_{{i = 1}}^{n}{k}_{i}{X}_{i} \sim  N\left( {\mathop{\sum }\limits_{{i = 1}}^{n}{k}_{i}{\mu }_{i},\mathop{\sum }\limits_{{i = 1}}^{n}{k}_{i}^{2}{\sigma }_{i}^{2}}\right).
$$

(2) 设 ${X}_{1},{X}_{2},\cdots,{X}_{n}$ 相互独立,且 ${X}_{i}$ 的分布函数为 ${F}_{{X}_{i}}\left( {x}_{i}\right) \left( {i = 1,2,\cdots, n}\right)$,则 $Z =$ $\max \left\{  {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right\}$ 的分布函数为

$$
{F}_{\max }\left( z\right)  = {F}_{{X}_{1}}\left( z\right) {F}_{{X}_{2}}\left( z\right) \cdots {F}_{{X}_{n}}\left( z\right),
$$

$Z = \min \left\{  {{X}_{1},{X}_{2},\cdots,{X}_{n}}\right\}$ 的分布函数为

$$
{F}_{\min }\left( z\right)  = 1 - \left\lbrack  {1 - {F}_{{X}_{1}}\left( z\right) }\right\rbrack  \left\lbrack  {1 - {F}_{{X}_{2}}\left( z\right) }\right\rbrack  \cdots \left\lbrack  {1 - {F}_{{X}_{n}}\left( z\right) }\right\rbrack .
$$

### 基本题型

#### 题型 1: 求离散型变量函数的分布

【5.1】设两个相互独立的随机变量 $\xi$ 与 $\eta$ 的分布律为

<table><tr><td>$\xi$</td><td/><td/><td>$\eta$</td><td>2</td><td/></tr><tr><td>${p}_{i}$</td><td>0.3</td><td>0.7</td><td>${p}_{j}$</td><td>0.6</td><td>0.4</td></tr></table>

求随机变量 $Z = \xi  + \eta$ 的分布律.

分析 简单的离散型随机变量的求解可直接应用列表的方法.

解 由于 $\xi$ 与 $\eta$ 相互独立,因此有 ${p}_{ij} = {p}_{i} \cdot  {p}_{j}$.

得到二维随机变量的联合分布:

<table><tr><td>$\eta$ ξ</td><td>2</td><td>4</td></tr><tr><td>1</td><td>0.18</td><td>0.12</td></tr><tr><td>3</td><td>0.42</td><td>0.28</td></tr></table>

因为 $Z = \xi  + \eta$,易知 $Z$ 的分布为

<table><tr><td>${p}_{ij}$</td><td>$\left( {\xi,\eta }\right)$</td><td>$Z$</td></tr><tr><td>0.18</td><td>(1,2)</td><td>3</td></tr><tr><td>0.12</td><td>$\left( {1,4}\right)$</td><td>5</td></tr><tr><td>0.42</td><td>(3,2)</td><td>5</td></tr><tr><td>0.28</td><td>(3,4)</td><td>7</td></tr></table>

由离散型随机变量函数的定义 $P\left\{  {Z = {z}_{k}}\right\}   = \mathop{\sum }\limits_{{{x}_{i} + {y}_{j} = {z}_{k}}}P\left\{  {X = {x}_{i}, Y = {y}_{j}}\right\}$,得到 $Z$ 的分布律为

<table><tr><td>$Z$</td><td>3</td><td>5</td><td>7</td></tr><tr><td>$p$</td><td>0.18</td><td>0.54</td><td>0.28</td></tr></table>

【5.2】设随机变量 $X$ 与 $Y$ 相互独立, $X$ 的概率分布为 $P\{ X = 1\}  = P\{ X =  - 1\}  = \frac{1}{2}, Y$ 服从参数为 $\lambda$ 的泊松分布. 令 $Z = {XY}$,求 $Z$ 的概率分布.

解 $Z$ 的所有可能取值为全体整数,

即 $Z$ 取 $0, \pm  1, \pm  2,\cdots \cdots$

$P\{ Z = 0\}  = P\{ {XY} = 0\}  = P\{ Y = 0\}  = {\mathrm{e}}^{-\lambda };$ 概率论与数理统计习题精选精解

对于 $n =  \pm  1, \pm  2,\cdots \cdots$,有

$$
P\{ Z = n\}  = P\{ {XY} = n\}  = P\left\{  {X = \frac{n}{\left| n\right| }, Y = \left| n\right| }\right\}
$$

$$
= P\left\{  {X = \frac{n}{\left| n\right| }}\right\}  P\{ Y = \left| n\right| \}  = \frac{1}{2} \cdot  \frac{{\lambda }^{\left| n\right| }}{\left| n\right| !}{e}^{-\lambda }
$$

【5.3】假设随机变量 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$ 相互独立且同分布, $P\left\{  {{X}_{i} = 0}\right\}   = {0.6}, P\left\{  {{X}_{i} = 1}\right\}   =$ ${0.4}\left( {i = 1,2,3,4}\right)$,求行列式 $X = \left| \begin{array}{ll} {X}_{1} & {X}_{2} \\  {X}_{3} & {X}_{4} \end{array}\right|$ 的概率分布.

解 记 ${Y}_{1} = {X}_{1}{X}_{4},{Y}_{2} = {X}_{2}{X}_{3}$,则 $X = {Y}_{1} - {Y}_{2}$,随机变量 ${Y}_{1}$ 和 ${Y}_{2}$ 独立同分布.

$$
P\left\{  {{Y}_{1} = 1}\right\}   = P\left\{  {{Y}_{2} = 1}\right\}   = P\left\{  {{X}_{2} = 1,{X}_{3} = 1}\right\}   = {0.16}
$$

$$
P\left\{  {{Y}_{1} = 0}\right\}   = P\left\{  {{Y}_{2} = 0}\right\}   = 1 - {0.16} = {0.84}
$$

随机变量 $X = {Y}_{1} - {Y}_{2}$ 有三个可能值-1,0,1,易见

$$
P\{ X =  - 1\}  = P\left\{  {{Y}_{1} = 0,{Y}_{2} = 1}\right\}   = {0.84} \times  {0.16} = {0.1344}
$$

$$
P\{ X = 1\}  = P\left\{  {{Y}_{1} = 1,{Y}_{2} = 0}\right\}   = {0.16} \times  {0.84} = {0.1344}
$$

$$
P\{ X = 0\}  = 1 - 2 \times  {0.1344} = {0.7312}
$$

于是行列式的概率分布为

$$
X = \left| \begin{array}{ll} {X}_{1} & {X}_{2} \\  {X}_{3} & {X}_{4} \end{array}\right|  \sim  \left\lbrack  \begin{matrix}  - 1 & 0 & 1 \\  {0.1344} & {0.7312} & {0.1344} \end{matrix}\right\rbrack
$$

点评 本题将概率论及线性代数很好地结合在一起,有一定的参考价值. 先将行列式求出, 再引入中间变量 ${Y}_{1}\text{、}{Y}_{2}$ 并求出其分布,则问题可解决.

【5.4】设随机变量 $X$ 与 $Y$ 独立同分布,且 $X$ 的概率分布为

<table><tr><td>$X$</td><td>12</td></tr><tr><td>$P$</td><td>$\frac{2}{3}$$\frac{1}{3}$</td></tr></table>

记 $U = \max \{ X, Y\}, V = \min \{ X, Y\}$,求 $\left( {U, V}\right)$ 的概率分布.

解 $\left( {U, V}\right)$ 有三个可能值: $\left( {1,1}\right),\left( {2,1}\right),\left( {2,2}\right)$,而

$$
P\{ U = 1, V = 1\}  = P\{ X = 1, Y = 1\}  = P\{ X = 1\} P\{ Y = 1\}  = \frac{4}{9},
$$

$$
P\{ U = 2, V = 1\}  = P\{ X = 1, Y = 2\}  + P\{ X = 2, Y = 1\}  = \frac{4}{9},
$$

$$
P\{ U = 2, V = 2\}  = P\{ X = 2, Y = 2\}  = P\{ X = 2\} P\{ Y = 2\}  = \frac{1}{9},
$$

故 $\left( {U, V}\right)$ 的概率分布为

<table><tr><td>$V$</td><td>1</td><td>2</td></tr><tr><td>1</td><td>$\frac{4}{9}$</td><td>0</td></tr><tr><td>2</td><td>$\frac{4}{9}$</td><td>$\frac{1}{9}$</td></tr></table>

量 102

【5.5】设二维随机变量 $\left( {X, Y}\right)$ 的概率分布为其中 $a, b, c$ 为常数,且 $X$ 的数学期望 ${EX} =  - {0.2}, P\{ Y \leq  0 \mid  X \leq  0\}  = {0.5}$,记 $Z = X + Y$,求 (1) $a, b, c$ 的值; (2) $Z$ 的概率分布; (3) $P\{ X = Z\}$.

<table><tr><td>Y $X$</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>-1</td><td>$a$</td><td>0</td><td>0.2</td></tr><tr><td>0</td><td>0.1</td><td>$b$</td><td>0.2</td></tr><tr><td>1</td><td>0</td><td>0.1</td><td>$c$</td></tr></table>

解 (1) 由概率分布的性质知, $a + b + c + {0.6} = 1$,即

$$
a + b + c = {0.4}\text{.}
$$

由 ${EX} =  - {0.2}$,可得

$- a + c =  - {0.1}$ (由第四章知识可得)

再由 $P\{ Y \leq  0 \mid  X \leq  0\}  = \frac{P\{ X \leq  0, Y \leq  0\} }{P\{ X \leq  0\} } = \frac{a + b + {0.1}}{a + b + {0.5}} = {0.5}$,得

$$
a + b = {0.3}
$$

解以上关于 $a, b, c$ 的三个方程得

$$
a = {0.2},\;b = {0.1},\;c = {0.1}.
$$

(2) $Z$ 的可能取值为 $- 2, - 1,0,1,2$,

$$
P\{ Z =  - 2\}  = P\{ X =  - 1, Y =  - 1\}  = {0.2},
$$

$$
P\{ Z =  - 1\}  = P\{ X =  - 1, Y = 0\}  + P\{ X = 0, Y =  - 1\}  = {0.1},
$$

$P\{ Z = 0\}  = P\{ X =  - 1, Y = 1\}  + P\{ X = 0, Y = 0\}  + P\{ X = 1, Y =  - 1\}  = {0.3}$

$$
P\{ Z = 1\}  = P\{ X = 1, Y = 0\}  + P\{ X = 0, Y = 1\}  = {0.3},
$$

$$
P\{ Z = 2\}  = P\{ X = 1, Y = 1\}  = {0.1},
$$

即 $Z$ 的概率分布为

<table><tr><td>$Z$</td><td>-2</td><td>-1</td><td>0</td><td>1</td><td>2</td></tr><tr><td>$P$</td><td>0.2</td><td>0.1</td><td>0.3</td><td>0.3</td><td>0.1</td></tr></table>

(3) $P\{ X = Z\}  = P\{ Y = 0\}  = 0 + b + {0.1} = {0.1} + {0.1} = {0.2}$.

#### 题型 2. 求连续型随机变量函数的分布

【5.6】设 $X$ 和 $Y$ 是两个相互独立的随机变量,其概率密度分别为

$$
{f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} 1, & 0 \leq  x \leq  1 \\  0, & \text{ 其他. } \end{array}\;{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0. \end{array}\right. }\right.
$$

试求随机变量 $Z = X + Y$ 的概率密度.

解法一 求随机变量 $Z$ 的概率密度,先求 $Z$ 的分布函数,再用 ${f}_{Z}\left( z\right)  = {F}_{Z}^{\prime }\left( z\right)$ 得到所求的概率密度.

因为 $X$ 和 $Y$ 相互独立,所以联合密度

$$
f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & 0 \leq  x \leq  1, y > 0 \\  0, & \text{ 其他. } \end{array}\right.
$$

对 $Z = X + Y$ 的分布分段讨论,简便起见作图 3-5.6-1 表示.

(1)当 $z < 0$ 时,

$$
{F}_{Z}\left( z\right)  = {\iint }_{x + y \leq  z}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\iint }_{x + y \leq  z}0\mathrm{\;d}x\mathrm{\;d}y = 0
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_103_1028_224_323_306_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_103_1028_224_323_306_0.jpg)

图 3-5.6-1

(2)当 $0 \leq  z < 1$ 时,

$$
{F}_{Z}\left( z\right)  = {\iint }_{x + y \leq  z}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{z}\mathrm{\;d}x{\int }_{0}^{z - x}{\mathrm{e}}^{-y}\mathrm{\;d}y
$$

$$
= z - 1 + \frac{1}{{\mathrm{e}}^{z}}
$$

(3)当 $z \geq  1$ 时,

$$
{F}_{Z}\left( z\right)  = {\iint }_{x + y \leq  z}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}\mathrm{\;d}x{\int }_{0}^{z - x}{\mathrm{e}}^{-y}\mathrm{\;d}y
$$

$$
= 1 + \left( {1 - \mathrm{e}}\right) \frac{1}{{\mathrm{e}}^{z}}.
$$

由 ${f}_{Z}\left( z\right)  = {F}_{Z}{}^{\prime }\left( z\right)$,得 $Z$ 的分布密度为

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 0, & z < 0 \\  1 - {\mathrm{e}}^{-z}, & 0 \leq  z < 1 \\  \left( {\mathrm{e} - 1}\right) {\mathrm{e}}^{-z}, & z \geq  1. \end{array}\right.
$$

解法二 由于 $X$ 和 $Y$ 是相互独立的,故由卷积公式, $Z = X + Y$ 的概率密度

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }{f}_{X}\left( x\right) {f}_{Y}\left( {z - x}\right) \mathrm{d}x
$$

易知仅当 $\left\{  \begin{array}{l} 0 \leq  x \leq  1 \\  z - x > 0 \end{array}\right.$ 即 $\left\{  \begin{array}{l} 0 \leq  x \leq  1 \\  x < z \end{array}\right.$ 时,上述积分的被积函数不为零(参阅图 3-5.6-2). 所以

$$
{f}_{Z}\left( z\right)  = \left\{  {\begin{array}{ll} {\int }_{0}^{x}{f}_{X}\left( x\right) {f}_{Y}\left( {z - x}\right) \mathrm{d}x, & 0 \leq  z \leq  1 \\  {\int }_{0}^{1}{f}_{X}\left( x\right) {f}_{Y}\left( {z - x}\right) \mathrm{d}x, & z > 1 \\  0, & \text{ 其他 } \end{array} = \left\{  \begin{array}{ll} {\int }_{0}^{x}{\mathrm{e}}^{-\left( {z - x}\right) }\mathrm{d}x, & 0 \leq  z \leq  1 \\  {\int }_{0}^{1}{\mathrm{e}}^{-\left( {z - x}\right) }\mathrm{d}x, & z > 1 \\  0, & \text{ 其他 } \end{array}\right. }\right.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_103_619_1101_439_267_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_103_619_1101_439_267_0.jpg)

图 3-5.6-2


$$
= \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-z}, & 0 \leq  z \leq  1 \\  \left( {\mathrm{e} - 1}\right) {\mathrm{e}}^{-z}, & z > 1 \\  0, & \text{ 其他. } \end{array}\right.
$$

【5.7】设 $X$ 与 $Y$ 相互独立,分别服从参数为 ${\lambda }_{1}$ 与 ${\lambda }_{2}$ 的指数分布,求 $Z = \frac{X}{Y}$ 的密度函数.

分析 设 $\left( {X, Y}\right)$ 是二维连续型随机变量,其联合密度函数为 $f\left( {x, y}\right)$,则随机变量 $Z = \frac{X}{Y}$ 的密度函数 ${f}_{Z}\left( z\right)$ 为

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| y\right| f\left( {{zy}, y}\right) \mathrm{d}y.
$$

特别地,如果 $X$ 与 $Y$ 相互独立,则有 $f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y}\left( y\right)$,此时,我们有

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| y\right| {f}_{X}\left( {yz}\right) {f}_{Y}\left( y\right) \mathrm{d}y.
$$

解 ${f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} {\lambda }_{1}{\mathrm{e}}^{-{\lambda }_{1}x} & x > 0 \\  0, & x \leq  0, \end{array}\;{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\lambda }_{2}{\mathrm{e}}^{-{\lambda }_{2}y} & y > 0 \\  0, & y \leq  0 \end{array}\right. }\right.$

设 $Z = \frac{X}{Y}$,由 $X$ 与 $Y$ 独立性,我们有

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| y\right| {f}_{X}\left( {yz}\right) {f}_{Y}\left( y\right) \mathrm{d}y,\;{yz} > 0, y > 0
$$

如图 3-5.7 所示:

(1) 若 $z \leq  0,{f}_{Z}\left( z\right)  = 0$.

(2) 若 $z > 0$,

$$
{f}_{Z}\left( z\right)  = {\int }_{0}^{+\infty }y{\lambda }_{1}{\mathrm{e}}^{-{\lambda }_{1}{yz}}{\lambda }_{2}{\mathrm{e}}^{-{\lambda }_{2}y}\mathrm{\;d}y = {\lambda }_{1}{\lambda }_{2}{\int }_{0}^{+\infty }y{\mathrm{e}}^{-\left( {{\lambda }_{2} + {\lambda }_{1}z}\right) y}\mathrm{\;d}y
$$

$$
= \frac{{\lambda }_{1}{\lambda }_{2}}{{\left( {\lambda }_{2} + {\lambda }_{1}z\right) }^{2}}
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_104_987_930_318_275_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_104_987_930_318_275_0.jpg)

图 3-5.7

则 $Z = \frac{X}{Y}$ 的密度为

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} \frac{{\lambda }_{1}{\lambda }_{2}}{{\left( {\lambda }_{2} + {\lambda }_{1}z\right) }^{2}}, & z > 0 \\  0, & z \leq  0. \end{array}\right.
$$

【5.8】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} 1, & 0 < x < 1,0 < y < {2x} \\  0, & \text{ 其他 } \end{array}\right.
$$

求: (1) $\left( {X, Y}\right)$ 的边缘概率密度 ${f}_{X}\left( x\right),{f}_{Y}\left( y\right)$;

(2) $Z = {2X} - Y$ 的概率密度 ${f}_{Z}\left( z\right)$;

(3) $P\left\{  {Y \leq  \frac{1}{2} \mid  X \leq  \frac{1}{2}}\right\}$.

解 (1) 当 $0 < x < 1$ 时, ${f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = {\int }_{0}^{2x}\mathrm{\;d}y = {2x}$

当 $x \leq  0$ 或 $x \geq  1$ 时, ${f}_{X}\left( x\right)  = 0$,即 ${f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} {2x}, & 0 < x < 1 \\  0 & \text{ 其他 } \end{array}\right.$

当 $0 < y < 2$ 时, ${f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = {\int }_{\frac{y}{2}}^{1}\mathrm{\;d}x = 1 - \frac{y}{2}$

当 $y \leq  0$ 或 $y \geq  1$ 时, ${f}_{Y}\left( y\right)  = 0$,即 ${f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} 1 - \frac{y}{2}, & 0 < y < 2 \\  0, & \text{ 其他 } \end{array}\right.$

(2)解法一 当 $z \leq  0$ 时, ${F}_{Z}\left( z\right)  = 0$

当 $0 < z < 2$ 时, ${F}_{Z}\left( z\right)  = P\{ {2X} - Y \leq  z\}  = {\iint }_{{2x} - y \leq  z}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = z - \frac{{z}^{2}}{4}$

当 $z \geq  2$ 时, ${F}_{Z}\left( z\right)  = 1$,所以 ${f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 1 - \frac{z}{2}, & 0 < z < 2 \\  0, & \text{ 其他 } \end{array}\right.$

解法二 ${f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }f\left( {x,{2x} - z}\right) \mathrm{d}x$,

其中 $\;f\left( {x,{2x} - z}\right)  = \left\{  \begin{array}{ll} 1, & 0 < x < 1,0 < z < {2x} \\  0, & \text{ 其他 } \end{array}\right.$

当 $z \leq  0$ 或 $z \geq  2$ 时, ${f}_{Z}\left( z\right)  = 0$

当 $0 < z < 2$ 时, ${f}_{Z}\left( z\right)  = {\int }_{\frac{z}{2}}^{1}\mathrm{\;d}x = 1 - \frac{z}{2}$,即 ${f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 1 - \frac{z}{2}, & 0 < z < 2 \\  0, & \text{ 其他 } \end{array}\right.$

(3) $P\left\{  {Y \leq  \frac{1}{2} \mid  X \leq  \frac{1}{2}}\right\}   = \frac{P\left\{  {X \leq  \frac{1}{2}, Y \leq  \frac{1}{2}}\right\}  }{P\left\{  {X \leq  \frac{1}{2}}\right\}  } = \frac{\frac{3}{16}}{\frac{1}{4}} = \frac{3}{4}$.

【5.9】设随机变量 $X$ 和 $Y$ 的联合分布是正方形 $G = \{ \left( {x, y}\right)  \mid  1 \leq  x \leq  3,1 \leq  y \leq  3\}$ 上的均匀分布,试求随机变量 $U = \left| {X - Y}\right|$ 的概率密度 $p\left( u\right)$.

解 由条件知 $X$ 和 $Y$ 的联合密度为 $f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{4}, & 1 \leq  x \leq  3,1 \leq  y \leq  3 \\  0, & \text{ 其他 } \end{array}\right.$ 以 $F\left( u\right)  = P\{ U \leq  u\} \left( {-\infty  < u <  + \infty }\right)$ 表示随机变量 $U$ 的分布函数.

显然,当 $u \leq  0$ 时, $F\left( u\right)  = 0$;

当 $u \geq  2$ 时, $F\left( u\right)  = 1$.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_105_969_1247_379_343_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_105_969_1247_379_343_0.jpg)

图 3-5.9

设 $0 < u < 2$,如图 3-5.9 所示,则

$$
F\left( u\right)  = {\iint }_{\left| {x - y}\right|  \leq  u}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\iint }_{\left| {x - y}\right|  \leq  u}\frac{1}{4}\mathrm{\;d}x\mathrm{\;d}y
$$

$$
= \frac{1}{4}\left\lbrack  {4 - {\left( 2 - u\right) }^{2}}\right\rbrack   = 1 - \frac{1}{4}{\left( 2 - u\right) }^{2}
$$

于是,随机变量 $U$ 的密度为

$$
p\left( u\right)  = \left\{  \begin{array}{ll} \frac{1}{2}\left( {2 - u}\right), & 0 < u < 2 \\  0, & \text{ 其他 } \end{array}\right.
$$

【5.10】设二维随机变量 $\left( {X, Y}\right)$ 在矩形 $G = \{ \left( {x, y}\right)  \mid  0 \leq  x \leq  2,0 \leq  y \leq  1\}$ 上服从均匀分布,试求边长为 $X$ 和 $Y$ 的矩形面积 $S$ 的概率密度 $f\left( s\right)$.

解 本题为利用 $\left( {X, Y}\right)$ 的分布,求 $S = {XY}$ 的分布问题. 二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
\varphi \left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{2}, & \left( {x, y}\right)  \in  G \\  0, & \left( {x, y}\right)  \in  G \end{array}\right.
$$

设 $F\left( s\right)  = P\{ S \leq  s\}$ 为 $S$ 的分布函数,则当 $s \leq  0$ 时, $F\left( s\right)  = 0$; 当 $s \geq  2$ 时, $F\left( s\right)  = 1$.

现在,设 $0 < s < 2$,如图 3-5.10 所示,曲线 ${xy} =$ $s$ 与矩形 $G$ 的上边交于点 $\left( {s,1}\right)$; 位于曲线 ${xy} = s$ 上方的点满足 ${xy} > s$,位于下方的点满足 ${xy} < s$,于是

$$
F\left( s\right)  = P\{ S \leq  s\}  = P\{ {XY} \leq  s\}  = 1 - P\{ {XY} >
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_106_904_538_402_319_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_106_904_538_402_319_0.jpg)

图 3-5.10

$s\}$

$$
= 1 - {\iint }_{{xy} \geq  s}\frac{1}{2}\mathrm{\;d}x\mathrm{\;d}y
$$

$$
= 1 - \frac{1}{2}{\int }_{s}^{2}\mathrm{\;d}x{\int }_{\frac{s}{x}}^{1}\mathrm{\;d}y = \frac{s}{2}\left( {1 + \ln 2 - \ln s}\right)
$$

于是 $\;f\left( s\right)  = \left\{  \begin{array}{ll} \frac{1}{2}\left( {\ln 2 - \ln s}\right), & 0 < s < 2 \\  0, & s \leq  0\text{ 或 }s \geq  2 \end{array}\right.$

点评 本题也可利用公式计算:

$$
f\left( s\right)  = {\int }_{-\infty }^{+\infty }\frac{1}{\left| x\right| }\varphi \left( {x,\frac{z}{x}}\right) \mathrm{d}x = \left\{  \begin{array}{ll} \frac{1}{2}\left( {\ln 2 - \ln s}\right), & 0 < s < 2 \\  0, & \text{ 其他 } \end{array}\right.
$$

#### 题型 3. 关于重要结论及公式

【5.11】设两个相互独立的随机变量 $X$ 和 $Y$ 分别服从正态分布 $N\left( {0,1}\right)$ 和 $N\left( {1,1}\right)$, 则 (   ).

(A) $P\{ X + Y \leq  0\}  = \frac{1}{2}$ (B) $P\{ X + Y \leq  1\}  = \frac{1}{2}$

(C) $P\{ X - Y \leq  0\}  = \frac{1}{2}$ (D) $P\{ X - Y \leq  1\}  = \frac{1}{2}$

解 因为 $X + Y \sim  N\left( {1,2}\right), X - Y \sim  N\left( {-1,2}\right)$,利用正态分布几何意义或者结论:

当 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 时, $P\{ X \leq  \mu \}  = \frac{1}{2}$. 则

$$
P\{ X + Y \leq  1\}  = \frac{1}{2}
$$

故应选 (B).

【5.12】设系统 $L$ 由两个相互独立的子系统 ${L}_{1}$ 和 ${L}_{2}$ 连接而成,其连接的方式分别为 (1)串联,(2)并联,如图 3-5.12 所示.

设 ${L}_{1}$ 和 ${L}_{2}$ 的寿命分别为 $X$ 和 $Y$,已知它们的密度函数分别为

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \alpha {\mathrm{e}}^{-{\alpha x}}, & x > 0 \\  0, & x \leq  0, \end{array}\right.
$$

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \beta {\mathrm{e}}^{-{\beta y}}, & y > 0 \\  0, & y \leq  0, \end{array}\right.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_107_923_181_418_276_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_107_923_181_418_276_0.jpg)

图 3-5.12

其中 $\alpha  > 0,\beta  > 0$,试分别就以上两种连接方式写出系统 $L$ 的寿命 $Z$ 的密度函数.

解 (1) 串联的情况

因为当 ${L}_{1}$ 和 ${L}_{2}$ 中有一个损坏时,系统 $L$ 就停止工作,所以 $L$ 的寿命为 $Z = \min \left( {X, Y}\right)$

因 $X$ 和 $Y$ 的分布函数分别为

$$
{F}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} 1 - {\mathrm{e}}^{-{\alpha x}}, & x > 0 \\  0, & x \leq  0, \end{array}\;{F}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{\beta y}}, & y > 0 \\  0, & y \leq  0, \end{array}\right. }\right.
$$

故 $Z$ 的分布函数

$$
{F}_{Z}\left( z\right)  = 1 - \left( {1 - {F}_{X}\left( z\right) }\right) \left( {1 - {F}_{Y}\left( z\right) }\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-\left( {\alpha  + \beta }\right) z}, & z > 0 \\  0, & z \leq  0. \end{array}\right.
$$

于是,得 $Z$ 的密度函数

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} \left( {\alpha  + \beta }\right) {\mathrm{e}}^{-\left( {\alpha  + \beta }\right) z}, & z > 0 \\  0, & z \leq  0. \end{array}\right.
$$

(2)并联的情况

因为当且仅当 ${L}_{1}$ 和 ${L}_{2}$ 都损坏时,系统 $L$ 才停止工作,所以 $L$ 的寿命为 $Z = \max \left( {X, Y}\right)$,由此知, $Z$ 的分布函数

$$
{F}_{Z}\left( z\right)  = {F}_{X}\left( z\right) {F}_{Y}\left( z\right)  = \left\{  \begin{array}{ll} \left( {1 - {\mathrm{e}}^{-{\alpha z}}}\right) \left( {1 - {\mathrm{e}}^{-{\beta z}}}\right), & z > 0 \\  0, & z \leq  0. \end{array}\right.
$$

于是 $Z$ 的密度函数

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} \alpha {\mathrm{e}}^{-{\alpha z}} + \beta {\mathrm{e}}^{-{\beta z}} - \left( {\alpha  + \beta }\right) {\mathrm{e}}^{-\left( {\alpha  + \beta }\right) z}, & z > 0 \\  0, & z \leq  0. \end{array}\right.
$$

【5.13】假设一电路装有 3 个同种电气元件,其工作状态相互独立,且无故障工作时间都服从参数为 $\lambda  > 0$ 的指数分布. 当 3 个元件都无故障时,电路正常工作,否则整个电路不能正常工作. 试求电路正常工作的时间 $T$ 的概率分布.

解法一 以 ${X}_{i}\left( {i = 1,2,3}\right)$ 表示第 $i$ 个电气元件无故障工作的时间,则 ${X}_{1},{X}_{2},{X}_{3}$ 相互独立且同分布, 其分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{\lambda x}}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

设 $G\left( t\right)$ 是 $T$ 的分布函数. 当 $t \leq  0$ 时, $G\left( t\right)  = 0$. 当 $t > 0$ 时,有

$$
G\left( t\right)  = P\{ T \leq  t\}  = 1 - P\{ T > t\}  = 1 - P\left\{  {{X}_{1} > t,{X}_{2} > t,{X}_{3} > t}\right\}
$$

$$
= 1 - P\left\{  {{X}_{1} > t}\right\}  P\left\{  {{X}_{2} > t}\right\}  P\left\{  {{X}_{3} > t}\right\}   = 1 - {\left\lbrack  1 - F\left( t\right) \right\rbrack  }^{3}
$$

$$
= 1 - {\mathrm{e}}^{-{3\lambda t}}
$$

得 $G\left( t\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{3\lambda t}}, & t > 0 \\  0, & t \leq  0 \end{array}\right.$

于是, $T$ 服从参数为 ${3\lambda }$ 的指数分布.

解法二 本题也可直接利用公式计算: 因为 ${X}_{1},{X}_{2},{X}_{3}$ 独立同分布,而 $T = \min \left( {{X}_{1},{X}_{2}}\right.$, $\left. {X}_{3}\right)$,故

$$
G\left( t\right)  = 1 - {\left\lbrack  1 - F\left( t\right) \right\rbrack  }^{3} = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{3\lambda t}}, & t > 0 \\  0, & t \leq  0 \end{array}\right.
$$

题型 4. 特殊类型的变量函数的分布

【5.14】设随机变量 $X$ 与 $Y$ 独立,其中 $X$ 的概率分布为

$$
X \sim  \left( \begin{matrix} 1 & 2 \\  {0.3} & {0.7} \end{matrix}\right)
$$

而 $Y$ 的概率密度为 $f\left( y\right)$,求随机变量 $U = X + Y$ 的概率密度 $g\left( u\right)$.

解 设 $F\left( y\right)$ 是 $Y$ 的分布函数,则由全概率公式,知 $U = X + Y$ 的分布函数为

$$
G\left( u\right)  = P\{ X + Y \leq  u\}
$$

$$
= P\{ X = 1\} P\{ X + Y \leq  u \mid  X = 1\}  + P\{ X = 2\} P\{ X + Y \leq  u \mid  X = 2\}
$$

$$
= {0.3P}\{ X + Y \leq  u \mid  X = 1\}  + {0.7P}\{ X + Y \leq  u \mid  X = 2\}
$$

$$
= {0.3P}\{ Y \leq  u - 1 \mid  X = 1\}  + {0.7P}\{ Y \leq  u - 2 \mid  X = 2\} \text{.}
$$

由于 $X$ 和 $Y$ 独立,可见

$$
G\left( u\right)  = {0.3P}\{ Y \leq  u - 1\}  + {0.7P}\{ Y \leq  u - 2\}
$$

$$
= {0.3F}\left( {u - 1}\right)  + {0.7F}\left( {u - 2}\right) \text{.}
$$

由此,得 $U$ 的概率密度

$$
g\left( u\right)  = {G}^{\prime }\left( u\right)  = {0.3}{F}^{\prime }\left( {u - 1}\right)  + {0.7}{F}^{\prime }\left( {u - 2}\right)
$$

$$
= {0.3f}\left( {u - 1}\right)  + {0.7f}\left( {u - 2}\right) \text{.}
$$

点评 本题属新题型,求两个随机变量和的分布,其中一个是连续型,一个是离散型,需用全概率公式计算, 有一定难度.

另外,也可写成 $G\left( u\right)  = {0.3}{\int }_{-\infty }^{u - 1}f\left( y\right) \mathrm{d}y + {0.7}{\int }_{-\infty }^{u - 2}f\left( y\right) \mathrm{d}y$,同样求出 $g\left( u\right)$.

【5.15】假设一设备开机后无故障工作的时间 $X$ 服从指数分布,平均无故障工作的时间 (EX) 为 5 小时. 设备定时开机. 出现故障时自动关机, 而在无故障的情况下工作 2 小时便关机. 试求该设备每次开机无故障工作的时间 $Y$ 的分布函数 $F\left( y\right)$.

解 设 $X$ 的分布参数为 $\lambda$. 由于 ${EX} = \frac{1}{\lambda } = 5$,可见 $\lambda  = \frac{1}{5}$ (EX 结论见第四章),显然

$$
Y = \min \{ X,2\}.
$$

对于 $y < 0, F\left( y\right)  = 0$; 对于 $y \geq  2, F\left( y\right)  = 1$.

设 $0 \leq  y < 2$,有

$$
F\left( y\right)  = P\{ Y \leq  y\}  = P\{ \min \left( {X,2}\right)  \leq  y\}  = P\{ X \leq  y\}  = 1 - {\mathrm{e}}^{-\frac{y}{5}}.
$$

于是, $Y$ 的分布函数为

$$
F\left( y\right)  = \left\{  \begin{array}{ll} 0, & y < 0 \\  1 - {\mathrm{e}}^{-\frac{y}{5}}, & 0 \leq  y < 2 \\  1, & y \geq  2. \end{array}\right.
$$

点评 本题的关键在于: 一是指数分布的参数与数学期望的关系要熟悉; 二是能将 $Y$ 表示成 $\min \{ X,2\}$.

## $§6$. 综合提高题型

#### 题型 1. 关于多维随机变量的选择与判断

【6.1】设 ${X}_{1}$ 和 ${X}_{2}$ 是任意两个相互独立的连续型随机变量,它们的概率密度分别为 ${f}_{1}\left( x\right)$ 和 ${f}_{2}\left( x\right)$,分布函数分别为 ${F}_{1}\left( x\right)$ 和 ${F}_{2}\left( x\right)$,则 (   ).

(A) ${f}_{1}\left( x\right)  + {f}_{2}\left( x\right)$ 必为某一随机变量的概率密度

(B) ${F}_{1}\left( x\right) {F}_{2}\left( x\right)$ 必为某一随机变量的分布函数

(C) ${F}_{1}\left( x\right)  + {F}_{2}\left( x\right)$ 必为某一随机变量的分布函数

(D) ${f}_{1}\left( x\right) {f}_{2}\left( x\right)$ 必为某一随机变量的概率密度

解 由密度函数及分布函数性质可知: (B) 正确, (A), (C), (D) 不满足性质.

故应选(B).

【6.2】如下四个二元函数,(   )不能作为二维随机变量 $\left( {\xi,\eta }\right)$ 的分布函数.

(A) ${F}_{1}\left( {x, y}\right)  = \left\{  \begin{array}{ll} \left( {1 - {\mathrm{e}}^{-x}}\right) \left( {1 - {\mathrm{e}}^{-y}}\right), & 0 < x <  + \infty,0 < y <  + \infty \\  0, & \text{ 其他 } \end{array}\right.$

(B) ${F}_{2}\left( {x, y}\right)  = \left\{  \begin{array}{ll} \sin x\sin y, & 0 \leq  x \leq  \frac{\pi }{2},0 \leq  y \leq  \frac{\pi }{2} \\  0, & \text{ 其他 } \end{array}\right.$

(C) ${F}_{3}\left( {x, y}\right)  = \left\{  \begin{array}{ll} 1, & x + {2y} \geq  1 \\  0, & x + {2y} < 1 \end{array}\right.$

(D) ${F}_{4}\left( {x, y}\right)  = 1 + {2}^{-x} - {2}^{-y} + {2}^{-x - y}$

解 二维随机变量 $\left( {\xi,\eta }\right)$ 的分布函数具有四条性质,因此只有满足性质的函数才能作为 $\left( {\xi,\eta }\right)$ 的分布函数.

因为对 ${F}_{3}\left( {x, y}\right)$ 取四点 $\left( {1,0}\right),\left( {0,1}\right),\left( {1,1}\right),\left( {0,0}\right)$ 有

$$
F\left( {1,1}\right)  - F\left( {1,0}\right)  - F\left( {0,1}\right)  + F\left( {0,0}\right)  = 1 - 1 - 1 + 0 =  - 1 < 0
$$

即 ${F}_{3}\left( {x, y}\right)$ 不满足性质.

故 (C) 该入选.

【6.3】设随机变量 $X, Y$ 相互独立,且 $X$ 服从正态分布 $N\left( {0,{\sigma }_{1}^{2}}\right), Y$ 服从正态分布 $N\left( {0,{\sigma }_{2}^{2}}\right)$, 则概率 $P\{ \left| {X - Y}\right|  < 1\}$ (   ).

(A) 随 ${\sigma }_{1}$ 与 ${\sigma }_{2}$ 的减少而减少

(B) 随 ${\sigma }_{1}$ 与 ${\sigma }_{2}$ 的增加而增加

(C) 随 ${\sigma }_{1}$ 的增加而减少,随 ${\sigma }_{2}$ 的减少而增加 1. 110

(D) 随 ${\sigma }_{1}$ 的增加而增加,随 ${\sigma }_{2}$ 的减少而减少

解 因为 $X - Y \sim  N\left( {0,{\sigma }_{1}^{2} + {\sigma }_{2}^{2}}\right)$,故

$$
P\{ \left| {X - Y}\right|  < 1\}  = {2\Phi }\left( \frac{1}{\sqrt{{\sigma }_{1}^{2} + {\sigma }_{2}^{2}}}\right)  - 1
$$

即随 ${\sigma }_{1}$ 的增加而减少,随 ${\sigma }_{2}$ 的减少而增加.

故应选(C).

【6.4】设随机变量 $X, Y$ 独立同分布,且 $X$ 的分布函数为 $F\left( x\right)$,则 $Z = \max \{ X, Y\}$ 的分布函数为 (   ).

(A) ${F}^{2}\left( x\right)$ (B) $F\left( x\right) F\left( y\right)$

(C) $1 - {\left\lbrack  1 - F\left( x\right) \right\rbrack  }^{2}$ (D) $\left\lbrack  {1 - F\left( x\right) }\right\rbrack  \left\lbrack  {1 - F\left( y\right) }\right\rbrack$

解 ${F}_{Z}\left( z\right)  = P\{ Z \leq  z\}  = P\{ \max \{ X, Y\}  \leq  z\}  = P\{ X \leq  z, Y \leq  z\}$

$= P\{ X \leq  z\} P\{ Y \leq  z\}  = F\left( z\right) F\left( z\right)  = {F}^{2}\left( z\right).$

故应选(A)

【6.5】设随机变量 ${X}_{1},{X}_{2},{X}_{3}$ 相互独立,并且有相同的概率分布

$$
P\left\{  {{X}_{i} = 1}\right\}   = p,\;P\left\{  {{X}_{i} = 0}\right\}   = q,\;i = 1,2,3, p + q = 1.
$$

考虑随机变量

${Y}_{1} = \left\{  {\begin{array}{ll} 1, & \text{ 若 }{X}_{1} + {X}_{2}\text{ 为奇数 } \\  0, & \text{ 若 }{X}_{1} + {X}_{2}\text{ 为偶数 } \end{array}\;{Y}_{2} = \left\{  \begin{array}{ll} 1, & \text{ 若 }{X}_{2} + {X}_{3}\text{ 为奇数 } \\  0, & \text{ 若 }{X}_{2} + {X}_{3}\text{ 为偶数 } \end{array}\right. }\right.$

则乘积 ${Y}_{1}{Y}_{2}$ 的概率分布为 (   ).

(A) ${Y}_{1}{Y}_{2} \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  1 - {pq} & {pq} \end{matrix}\right\rbrack$ (B) ${Y}_{1}{Y}_{2} \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  {pq} & 1 - {pq} \end{matrix}\right\rbrack$

(C) ${Y}_{1}{Y}_{2} \sim  \left\lbrack  \begin{array}{ll} 0 & 1 \\  p & q \end{array}\right\rbrack$ (D) ${Y}_{1}{Y}_{2} \sim  \left\lbrack  \begin{array}{ll} 0 & 1 \\  q & p \end{array}\right\rbrack$

解 根据 ${Y}_{1}$ 和 ${Y}_{2}$ 的取值情况知, ${Y}_{1}{Y}_{2}$ 只可能取 0 和 1 两个数值. 因此,只要求出 $P\left\{  {{Y}_{1}{Y}_{2}}\right.$ $= 1\}$ 或 $P\left\{  {{Y}_{1}{Y}_{2} = 0}\right\}$ 即可.

因为 $P\left\{  {{Y}_{1}{Y}_{2} = 1}\right\}   + P\left\{  {{Y}_{1}{Y}_{2} = 0}\right\}   = 1$,而事件

$\left\{  {{Y}_{1}{Y}_{2} = 1}\right\}   = \left\{  {{Y}_{1} = 1,{Y}_{2} = 1}\right\}   = \left\{  {{X}_{1} + {X}_{2}}\right.$ 为奇数, $\left. {{X}_{2} + {X}_{3}\text{ 为奇数 }}\right\}$

$= \left\{  {{X}_{1} = 0,{X}_{2} = 1,{X}_{3} = 0}\right\}   \cup  \left\{  {{X}_{1} = 1,{X}_{2} = 0,{X}_{3} = 1}\right\}$

再根据不相容事件和概率的可加性以及 ${X}_{1},{X}_{2},{X}_{3}$ 是相互独立的条件可求出

$P\left\{  {{Y}_{1}{Y}_{2} = 1}\right\}   = P\left\{  {{Y}_{1} = 1,{Y}_{2} = 1}\right\}$

$$
= P\left\{  {{X}_{1} = 0,{X}_{2} = 1,{X}_{3} = 0}\right\}   + P\left\{  {{X}_{1} = 1,{X}_{2} = 0,{X}_{3} = 1}\right\}
$$

$$
= p{q}^{2} + {p}^{2}q = {pq},
$$

$P\left\{  {{Y}_{1}{Y}_{2} = 0}\right\}   = 1 - P\left\{  {{Y}_{1}{Y}_{2} = 1}\right\}   = 1 - {pq}.$

所以 ${Y}_{1}{Y}_{2}$ 的概率分布为 ${Y}_{1}{Y}_{2} \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  1 - {pq} & {pq} \end{matrix}\right\rbrack$.

故应选 (A).

【6.6】假设随机变量 $X$ 服从指数分布,则随机变量 $Y = \min \{ X,2\}$ 的分布函数 (   ). 概率论与数理统计习题精选精解

(A) 是连续函数 (B) 至少有两个间断点

(C) 是阶梯函数 (D) 恰好有一个间断点

解 $Y$ 的分布函数 ${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\{ \min \left( {X,2}\right)  \leq  y\}$

显然 $y < 0$ 时, ${F}_{Y}\left( y\right)  = 0;\;y \geq  2$ 时, ${F}_{Y}\left( y\right)  = 1$;

$0 \leq  y < 2$ 时, ${F}_{Y}\left( y\right)  = P\{ \min \left( {X,2}\right)  \leq  y\}  = P\{ X \leq  y\}  = 1 - {\mathrm{e}}^{-{\lambda y}}$ 故

$$
{F}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} 0, & y < 0 \\  1 - {\mathrm{e}}^{-{\lambda y}}, & 0 \leq  y < 2 \\  1, & y \geq  2 \end{array}\right.
$$

可见 ${F}_{Y}\left( y\right)$ 只在 $y = 2$ 间断.

故应选(D)

【6.7】设随机变量 $X$ 与 $Y$ 相互独立,且 $X$ 服从标准正态分布 $N\left( {0,1}\right), Y$ 的概率分布为 $P\{ Y = 0\}  = P\{ Y = 1\}  = \frac{1}{2}$,记 ${F}_{Z}\left( z\right)$ 为随机变量 $Z = {XY}$ 的分布函数,则函数 ${F}_{Z}\left( z\right)$ 的间断点个数为 (   ).

(A) 0 (B) 1 (C) 2 (D) 3

解 ${F}_{Z}\left( z\right)  = P\left( {{XY} \leq  z}\right)  = P\left( {{XY} \leq  z \mid  Y = 0}\right) P\left( {Y = 0}\right)  + P\left( {{XY} \leq  z \mid  Y = 1}\right) P(Y =$ 1)

$= \frac{1}{2}\left\lbrack  {P\left( {{XY} \leq  z \mid  Y = 0}\right)  + P\left( {{XY} \leq  z \mid  Y = 1}\right) }\right\rbrack$

$= \frac{1}{2}\left\lbrack  {P\left( {X \cdot  0 \leq  z \mid  Y = 0}\right)  + P\left( {X \leq  z \mid  Y = 1}\right) }\right\rbrack .$

由于 $X, Y$ 独立, ${F}_{Z}\left( z\right)  = \frac{1}{2}\left\lbrack  {P\left( {X \cdot  0 \leq  z}\right)  + P\left( {X \leq  z}\right) }\right\rbrack$.

(1)若 $z < 0$,则 ${F}_{Z}\left( z\right)  = \frac{1}{2}\Phi \left( z\right)$;

(2)若 $z \geq  0$,则 ${F}_{Z}\left( z\right)  = \frac{1}{2}\left\lbrack  {1 + \Phi \left( z\right) }\right\rbrack$,所以 $z = 0$ 为间断点.

故选 (B).

【6.8】设二维随机变量 $\left( {X, Y}\right)$ 的概率分布为

<table><tr><td>Y</td><td>0</td><td>1</td></tr><tr><td>0</td><td>0.4</td><td>$a$</td></tr><tr><td>1</td><td>$b$</td><td>0.1</td></tr></table>

已知随机事件 $\{ X = 0\}$ 与 $\{ X + Y = 1\}$ 相互独立,则(   ).

(A) $a = {0.2}, b = {0.3}$ (B) $a = {0.4}, b = {0.1}$

(C) $a = {0.3}, b = {0.2}$ (D) $a = {0.1}, b = {0.4}$

分析 由 $\mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}{p}_{ij} = 1$ 可得 $a$ 和 $b$ 的关系,再由事件 $\{ X = 0\}$ 与 $\{ X + Y = 1\}$ 相互独立得到另外一个关系,由方程组解出 $a, b$ 的值.


解 由 $\mathop{\sum }\limits_{i}\mathop{\sum }\limits_{j}{p}_{ij} = {0.4} + a + b + {0.1} = 1$,得到 $a + b = {0.5}$

由 $\{ X = 0\}$ 与 $\{ X + Y = 1\}$ 相互独立,得到

$$
P\{ X = 0\} P\{ X + Y = 1\}  = P\{ X = 0, X + Y = 1\}
$$

由已知条件可得

$$
P\{ X = 0, X + Y = 1\}  = P\{ X = 0, Y = 1\}  = a
$$

$$
P\{ X = 0\}  = P\{ X = 0, Y = 0\}  + P\{ X = 0, Y = 1\}  = a + {0.4}
$$

$$
P\{ X + Y = 1\}  = P\{ X = 0, Y = 1\}  + P\{ X = 1, Y = 0\}  = a + b = {0.5}
$$

联立方程组 $\left\{  \begin{array}{l} {0.5} \times  \left( {a + {0.4}}\right)  = a \\  a + b = {0.5} \end{array}\right.$ 解之得 $\left\{  \begin{array}{l} a = {0.4} \\  b = {0.1}. \end{array}\right.$

故应选(B)

【6.9】设两个随机变量 $X$ 与 $Y$ 相互独立且同分布,

$$
P\{ X =  - 1\}  = P\{ Y =  - 1\}  = \frac{1}{2},
$$

$P\{ X = 1\}  = P\{ Y = 1\}  = \frac{1}{2}$

则下列各式中成立的是(   ).

(A) $P\{ X = Y\}  = \frac{1}{2}$ (B) $P\{ X = Y\}  = 1$

(C) $P\{ X + Y = 0\}  = \frac{1}{4}$ (D) $P\{ {XY} = 1\}  = \frac{1}{4}$ 解 $X, Y$ 的联合分布

<table><tr><td>$X$</td><td>-1</td><td>1</td></tr><tr><td>-1</td><td>$\frac{1}{4}$</td><td>$\frac{1}{4}$</td></tr><tr><td>1</td><td>$\frac{1}{4}$</td><td>$\frac{1}{4}$</td></tr></table>

因此, $P\{ X = Y\}  = P\{ X =  - 1, Y =  - 1\}  + P\{ X = 1, Y = 1\}  = \frac{1}{4} + \frac{1}{4} = \frac{1}{2}$.

故应选 (A).

#### 题型 2. 多维随机变量的分布工具及工具的转换

【6.10】设某班车起点站上客人数 $X$ 服从参数为 $\lambda \left( {\lambda  > 0}\right)$ 的泊松分布,每位乘客在中途下车的概率为 $p\left( {0 < p < 1}\right)$,且中途下车与否相互独立. 以 $Y$ 表示在中途下车的人数,求:

(1)在发车时有 $n$ 个乘客的条件下,中途有 $m$ 人下车的概率；

(2)二维随机变量 $\left( {X, Y}\right)$ 的概率分布.

解 (1) $P\{ Y = m \mid  X = n\}  = {C}_{n}^{m}{p}^{m}{\left( 1 - p\right) }^{n - m},0 \leq  m \leq  n, n = 0,1,2,\cdots$.

(2) $P\{ X = n, Y = m\}  = P\{ Y = m \mid  X = n\} P\{ X = n\}  = {C}_{n}^{m}{p}^{m}{\left( 1 - p\right) }^{n - m} \cdot  \frac{{\mathrm{e}}^{-\lambda }}{n!}{\lambda }^{n}$

$$
0 \leq  m \leq  n,\;n = 0,1,2,\cdots.
$$

点评 本题将许多基本内容综合在一起:(1)二项分布；(2)泊松分布；(3)乘法公式；(4)二维离散型随机变量的分布律. 很有参考价值.

【6.11】袋中有一个红色球,两个黑色球,三个白球,现有放回的从袋中取两次,每次取一球,以 $X, Y, Z$ 分别表示两次取球的红、黑、白球的个数.

(1) 求 $P\{ X = 1 \mid  Z = 0\}$;

(2)求二维随机变量 $\left( {X, Y}\right)$ 的概率分布.

解 (1) 在没有取白球的情况下取了一次红球, 利用样本空间的缩减法, 相当于只有 1 个红球, 2 个黑球有放回摸两次, 其中摸一个红球的概率, 所以

$$
P\{ X = 1 \mid  Z = 0\}  = \frac{{C}_{2}^{1} \times  2}{{3}^{2}} = \frac{4}{9}.
$$

(2) $X, Y$ 取值范围为0,1,2,故

$$
P\{ X = 0, Y = 0\}  = \frac{{C}_{3}^{1} \times  {C}_{3}^{2}}{{6}^{2}} = \frac{1}{4},\;P\{ X = 1, Y = 0\}  = \frac{{C}_{2}^{1} \times  {C}_{3}^{1}}{{6}^{2}} = \frac{1}{6},
$$

$$
P\{ X = 2, Y = 0\}  = \frac{1}{{6}^{2}} = \frac{1}{36},\;P\{ X = 0, Y = 1\}  = \frac{{C}_{2}^{1} \times  {C}_{2}^{1} \times  {C}_{3}^{1}}{{6}^{2}} = \frac{1}{3},
$$

$$
P\{ X = 1, Y = 1\}  = \frac{{C}_{2}^{1} \times  {C}_{2}^{1}}{{6}^{2}} = \frac{1}{9},\;P\{ X = 2, Y = 1\}  = 0,
$$

$P\{ X = 0, Y = 2\}  = \frac{{C}_{2}^{1} \times  {C}_{2}^{1}}{{6}^{2}} = \frac{1}{9},\;P\{ X = 1, Y = 2\}  = 0,$

$P\{ X = 2, Y = 2\}  = 0.$

<table><tr><td>$X$ Y</td><td>0</td><td>1</td><td>2</td></tr><tr><td>0</td><td>$\frac{1}{4}$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{36}$</td></tr><tr><td>1</td><td>$\frac{1}{3}$</td><td>$\frac{1}{9}$</td><td>0</td></tr><tr><td>2</td><td>$\frac{1}{9}$</td><td>0</td><td>0</td></tr></table>

【6.12】设随机变量 $X$ 与 $Y$ 的概率分布分别为

<table><tr><td>$X$</td><td>0</td><td>1</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{2}{3}$</td></tr></table>

<table><tr><td>$Y$</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td></tr></table>

且 $P\left\{  {{X}^{2} = {Y}^{2}}\right\}   = 1$.

(1)求二维随机变量 $\left( {X, Y}\right)$ 的概率分布；

(2)求 $Z = {XY}$ 的概率分布.

解 (1) 由 $P\left\{  {{X}^{2} = {Y}^{2}}\right\}   = 1$ 可知 $P\left\{  {{X}^{2} \neq  {Y}^{2}}\right\}   = 0$,

于是 $P\{ X = 0, Y = 1\}  = P\{ X = 0, Y =  - 1\}  = P\{ X = 1, Y = 0\}  = 0$,

则 $P\{ X = 1, Y =  - 1\}  = P\{ X =  - 1\}  - P\{ X = 0, Y =  - 1\}  = \frac{1}{3}$,

同理 $P\{ X = 1, Y = 1\}  = P\{ X = 0, Y = 0\}  = \frac{1}{3}$. 即概率分布如下


$§6$. 综合提高题型

<table><tr><td>$Y$ $X$</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>0</td><td>0</td><td>$\frac{1}{3}$</td><td>0</td></tr><tr><td>1</td><td>$\frac{1}{3}$</td><td>0</td><td>$\frac{1}{3}$</td></tr></table>

(2) $Z = {XY}$ 可能的取值为-1,0,1.

$$
P\{ {XY} =  - 1\}  = P\{ X = 1, Y =  - 1\}  = \frac{1}{3},
$$

$$
P\{ {XY} = 1\}  = P\{ X = 1, Y = 1\}  = \frac{1}{3},
$$

$$
P\{ {XY} = 0\}  = 1 - \frac{1}{3} - \frac{1}{3} = \frac{1}{3}.
$$

故 $Z$ 的分布律为

<table><tr><td>$Z$</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td></tr></table>

【6.13】将一枚硬币掷 3 次,以 $X$ 表示前 2 次中出现 $H$ 的次数,以 $Y$ 表示 3 次中出现 $H$ 的次数,求 $X, Y$ 的联合分布律以及边缘分布律.

解 $\left( {X, Y}\right)$ 的所有情形为 ${HHH},{HHT},{HTH},{THH},{HTT},{THT},{TTH},{TTT}$. (其中 $T$ 表示不出现 $H$ 面)

按古典概型,显然有

$$
P\{ X = 0, Y = 0\}  = \frac{1}{8},\;P\{ X = 0, Y = 1\}  = \frac{1}{8},
$$

$$
P\{ X = 1, Y = 1\}  = \frac{2}{8},\;P\{ X = 1, Y = 2\}  = \frac{2}{8},
$$

$$
P\{ X = 2, Y = 2\}  = \frac{1}{8},\;P\{ X = 2, Y = 3\}  = \frac{1}{8}.
$$

那么把 $\left( {X, Y}\right)$ 的联合分布律及边缘分布律列成表格:

<table><tr><td>$X$ Y</td><td>0</td><td>1</td><td>2</td><td>${p}_{\cdot j}$</td></tr><tr><td>0</td><td>$\frac{1}{8}$</td><td>0</td><td>0</td><td>$\frac{1}{8}$</td></tr><tr><td>1</td><td>$\frac{1}{8}$</td><td>$\frac{2}{8}$</td><td>0</td><td>$\frac{3}{8}$</td></tr><tr><td>2</td><td>0</td><td>$\frac{2}{8}$</td><td>$\frac{1}{8}$</td><td>$\frac{3}{8}$</td></tr><tr><td>3</td><td>0</td><td>0</td><td>$\frac{1}{8}$</td><td>$\frac{1}{8}$</td></tr><tr><td>${p}_{i \cdot  }$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{2}$</td><td>$\frac{1}{4}$</td><td>1</td></tr></table>

【6.14】已知随机变量 $X$ 和 $Y$ 的联合概率密度为

$$
\varphi \left( {x, y}\right)  = \left\{  \begin{array}{ll} {4xy}, & 0 \leq  x \leq  1,0 \leq  y \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

求 $X$ 和 $Y$ 的联合分布函数 $F\left( {x, y}\right)$.

解 (1) 对于 $x < 0$ 或 $y < 0$,有 $F\left( {x, y}\right)  = P\{ X \leq  x, Y \leq  y\}  = 0$.

(2)对于 $0 \leq  x \leq  1,0 \leq  y \leq  1$,有 $F\left( {x, y}\right)  = 4{\int }_{0}^{x}{\int }_{0}^{y}{uv}\mathrm{\;d}u\mathrm{\;d}v = {x}^{2}{y}^{2}$.

(3)对于 $x > 1, y > 1$,有 $F\left( {x, y}\right)  = 1$.

(4)对于 $x > 1,0 \leq  y \leq  1$,有 $F\left( {x, y}\right)  = P\{ X \leq  1, Y \leq  y\}  = {y}^{2}$.

(5) 对于 $y > 1,0 \leq  x \leq  1$,有 $F\left( {x, y}\right)  = P\{ X \leq  x, Y \leq  1\}  = {x}^{2}$.

故 $X$ 和 $Y$ 的联合分布函数

$$
F\left( {x, y}\right)  = \left\{  \begin{array}{ll} 0, & x < 0\text{ 或 }y < 0 \\  {x}^{2}{y}^{2}, & 0 \leq  x \leq  1,0 \leq  y \leq  1 \\  {x}^{2}, & 0 \leq  x \leq  1,1 < y \\  {y}^{2}, & 1 < x,0 \leq  y \leq  1 \\  1, & 1 < x,1 < y \end{array}\right.
$$

【6.15】设二维随机变量 $\left( {X, Y}\right)$ 在 $G$ 上服从均匀分布, $G$ 由 $x - y = 0, x + y = 2$ 与 $y = 0$ 围成.

(1)求边缘密度 ${f}_{X}\left( x\right)$;

(2) 求 ${f}_{X \mid  Y}\left( {x \mid  y}\right)$.

解 $\left( 1\right) \left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} 1, & \left( {x, y}\right)  \in  G \\  0, & \text{ 其他 } \end{array}\right.
$$

$X$ 的概率密度

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  \begin{array}{ll} x, & 0 \leq  x \leq  1 \\  2 - x, & 1 < x \leq  2 \\  0, & \text{ 其他 } \end{array}\right.
$$

(2) ${f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = \left\{  \begin{matrix} 2\left( {1 - y}\right), & 0 \leq  y \leq  1 \\  0, & \text{ 其他 } \end{matrix}\right.$

当 $0 < y < 1$ 时, $X$ 的条件概率密度 ${f}_{X \mid  Y}\left( {x \mid  y}\right)  = \frac{f\left( {x, y}\right) }{{f}_{Y}\left( y\right) } = \left\{  \begin{array}{ll} \frac{1}{2\left( {1 - y}\right) }, & y < x < 2 - y \\  0, & \text{ 其他 } \end{array}\right.$

【6. 16】设 $\left( {X, Y}\right)$ 是二维变量, $X$ 的边缘概率密度为 ${f}_{X}\left( x\right)  = \left\{  \begin{matrix} 3{x}^{2}, & 0 < x < 1, \\  0, & \text{ 其他. } \end{matrix}\right.$ 在给定

$X = x\left( {0 < x < 1}\right)$ 的条件下 $Y$ 的条件概率密度为

$$
{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \left\{  \begin{matrix} \frac{3{y}^{2}}{{x}^{3}}, & 0 < y < x, \\  0, & \text{ 其他 } \end{matrix}\right.
$$

(1)求 $\left( {X, Y}\right)$ 的概率密度 $f\left( {x, y}\right)$;

(2)求 $Y$ 的边缘概率密度 ${f}_{Y}\left( y\right)$;

(3) 求 $P\{ X > {2Y}\}$.

解 (1) 由题设得 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y \mid  X}\left( {y \mid  x}\right)  = \left\{  \begin{array}{ll} \frac{9{y}^{2}}{x}, & 0 < y < x,0 < x < 1, \\  0, & \text{ 其他. } \end{array}\right.
$$

(2) $Y$ 的边缘概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  {\begin{array}{ll} {\int }_{y}^{1}\frac{9{y}^{2}}{x}\mathrm{\;d}x, & 0 < y < 1, \\  0, & \text{ 其他 } \end{array} = \left\{  \begin{array}{ll}  - 9{y}^{2}\ln y, & 0 < y < 1, \\  0, & \text{ 其他. } \end{array}\right. }\right.
$$

(3) $P\{ X > {2Y}\}  = {\iint }_{x > {2y}}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}\mathrm{\;d}x{\int }_{0}^{\frac{x}{2}}\frac{9{y}^{2}}{x}\mathrm{\;d}y = \frac{1}{8}$.

【6.17】设随机变量 $\left( {\xi,\eta }\right)$ 的联合分布为

<table><tr><td>$\eta$</td><td>-1</td><td>0</td></tr><tr><td>1</td><td>$\frac{1}{4}$</td><td>$\frac{1}{4}$</td></tr><tr><td>2</td><td>$\frac{1}{6}$</td><td>$k$</td></tr></table>

求:(1)k 值；(2)联合分布函数 $F\left( {x, y}\right)$;(3)边缘分布函数 ${F}_{\xi }\left( x\right)$ 与 ${F}_{\eta }\left( y\right)$.

解 (1) 因为 $\mathop{\sum }\limits_{{i = 1}}^{{+\infty }}\mathop{\sum }\limits_{{j = 1}}^{{+\infty }}{p}_{ij} = 1$

所以由已知条件得 $\frac{1}{4} + \frac{1}{4} + \frac{1}{6} + k = 1$,那么 $k = \frac{1}{3}$

(2)由联合分布函数 $F\left( {x, y}\right)  = P\{ \xi  \leq  x,\eta  \leq  y\}$ 的定义知需对 $x, y$ 的取值范围分别讨论.

当 $x < 1$ 或 $y <  - 1$ 时, $F\left( {x, y}\right)  = P\left( \varnothing \right)  = 0$.

当 $1 \leq  x < 2, - 1 \leq  y < 0$ 时, $F\left( {x, y}\right)  = P\{ \xi  = 1,\eta  =  - 1\}  = \frac{1}{4}$.

当 $x \geq  2, - 1 \leq  y < 0$ 时, $F\left( {x, y}\right)  = P\{ \xi  = 1,\eta  =  - 1\}  + P\{ \xi  = 2,\eta  =  - 1\}$

$= \frac{1}{4} + \frac{1}{6} = \frac{5}{12}$.

当 $1 \leq  x < 2, y \geq  0$ 时, $F\left( {x, y}\right)  = P\{ \xi  = 1,\eta  =  - 1\}  + P\{ \xi  = 1,\eta  = 0\}$

$= \frac{1}{4} + \frac{1}{4} = \frac{1}{2}$.

当 $x \geq  2, y \geq  0$ 时,

$F\left( {x, y}\right)  = P\{ \xi  = 1,\eta  =  - 1\}  + P\{ \xi  = 2,\eta  =  - 1\}  + P\{ \xi  = 1,\eta  = 0\}  + P\{ \xi  = 2,\eta  = 0\}$

$= \frac{1}{4} + \frac{1}{6} + \frac{1}{4} + \frac{1}{3} = 1$.

所以 $F\left( {x, y}\right)  = \left\{  \begin{array}{ll} 0, & x < 1\text{ 或 }y <  - 1 \\  \frac{1}{4}, & 1 \leq  x < 2\text{ 且 } - 1 \leq  y < 0 \\  \frac{5}{12}, & x \geq  2\text{ 且 } - 1 \leq  y < 0 \\  \frac{1}{2}, & 1 \leq  x < 2\text{ 且 }y \geq  0 \\  1, & x \leq  2\text{ 且 }y \geq  0 \end{array}\right.$

(3) ${F}_{\xi }\left( x\right)  = F\left( {x, + \infty }\right)  = \left\{  \begin{array}{ll} 0, & x < 1 \\  \frac{1}{2} & 1 \leq  x < 2 \\  1, & x \geq  2 \end{array}\right.$

$$
{F}_{\eta }\left( y\right)  = F\left( {+\infty, y}\right)  = \left\{  \begin{array}{ll} 0, & y <  - 1 \\  \frac{5}{12} &  - 1 \leq  y < 0 \\  1, & y \geq  0 \end{array}\right.
$$

【6.18】设随机变量 $X$ 的概率密度为

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{2}, &  - 1 < x < 0 \\  \frac{1}{4}, & 0 \leq  x < 2 \\  0, & \text{ 其他 } \end{array}\right.
$$

令 $Y = {X}^{2}, F\left( {x, y}\right)$ 为二维随机变量 $\left( {X, Y}\right)$ 的分布函数. 求

(1) $Y$ 的概率密度 ${f}_{Y}\left( y\right)$;

(2) $F\left( {-\frac{1}{2},4}\right)$.

解 (1) $Y$ 的分布函数为 ${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\left\{  {{X}^{2} \leq  y}\right\}$.

当 $y \leq  0$ 时, ${F}_{Y}\left( y\right)  = 0,{f}_{Y}\left( y\right)  = 0$;

当 $0 < y < 1$ 时,

${F}_{Y}\left( y\right)  = P\{  - \sqrt{y} \leq  X \leq  \sqrt{y}\}  = P\{  - \sqrt{y} \leq  X < 0\}  + P\{ 0 \leq  X \leq  \sqrt{y}\}$

$$
= \frac{1}{2}\sqrt{y} + \frac{1}{4}\sqrt{y} = \frac{3}{4}\sqrt{y},
$$

$$
{f}_{Y}\left( y\right)  = \frac{3}{8\sqrt{y}}
$$

当 $1 \leq  y < 4$ 时,

$$
{F}_{Y}\left( y\right)  = P\{  - 1 \leq  X < 0\}  + P\{ 0 \leq  X \leq  \sqrt{y}\}  = \frac{1}{2} + \frac{1}{4}\sqrt{y},
$$

$$
{f}_{Y}\left( y\right)  = \frac{1}{8\sqrt{y}}
$$

当 $y \geq  4$ 时, ${F}_{Y}\left( y\right)  = 1,{f}_{Y}\left( y\right)  = 0$.

故 $Y$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{3}{8\sqrt{y}}, & 0 < y < 1 \\  \frac{1}{8\sqrt{y}}, & 1 \leq  y < 4 \\  0, & \text{ 其他 } \end{array}\right.
$$

(2) $F\left( {-\frac{1}{2},4}\right)  = P\left\{  {X \leq   - \frac{1}{2}, Y \leq  4}\right\}   = P\left\{  {X \leq   - \frac{1}{2},{X}^{2} \leq  4}\right\}$

$$
= P\left\{  {X \leq   - \frac{1}{2}, - 2 \leq  X \leq  2}\right\}   = P\left\{  {-2 \leq  X \leq   - \frac{1}{2}}\right\}
$$

$$
= P\left\{  {-1 < X \leq   - \frac{1}{2}}\right\}   = \frac{1}{4}.
$$

#### 题型 3. 利用随机变量的分布求概率

【6.19】设随机变量 $X$ 与 $Y$ 相互独立,且都服从区间 $\left( {0,1}\right)$ 上的均匀分布,则 $P\left\{  {{X}^{2} + {Y}^{2} \leq  1}\right\}   =$ _____.

(A) $\frac{1}{4}$ (B) $\frac{1}{2}$ (C) $\frac{\pi }{8}$ (D) $\frac{\pi }{4}$

解 本题求随机事件的概率. 由于给出了边缘分布,结合随机变量 $X$ 与 $Y$ 相互独立的条件可直接得到 $\left( {X, Y}\right)$ 的联合概率密度 $f\left( {x, y}\right)$,然后计算二重积分

$$
P\left\{  {{X}^{2} + {Y}^{2} \leq  1}\right\}   = {\iint }_{{x}^{2} + {y}^{2} \leq  1}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y
$$

即可. 但本题联合分布为均匀分布, 属几何概型, 利用图示法, 即利用面积计算会更简便 (参见图 3-6.19).

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_118_1010_927_303_270_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_118_1010_927_303_270_0.jpg)

图 3-6.19

随机变量 $X$ 与 $Y$ 相互独立,且都服从区间 $\left\lbrack  {0,1}\right\rbrack$ 上的均匀分布,所以 $X$ 与 $Y$ 的联合分布为区域

$$
D = \{ \left( {x, y}\right)  \mid  0 \leq  x \leq  1,0 \leq  y \leq  1\}
$$

上的均匀分布, 于是

$$
P\left\{  {{X}^{2} + {Y}^{2} \leq  1}\right\}   = \frac{S}{{S}_{D}} = \frac{\frac{\pi }{4}}{1} = \frac{\pi }{4}.
$$

故应选(D).

【6.20】设随机变量 $\left( {X, Y}\right)$ 的分布律为

<table><tr><td>$X$ Y</td><td>0</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td></tr><tr><td>0</td><td>0</td><td>0.01</td><td>0.03</td><td>0.05</td><td>0.07</td><td>0.09</td></tr><tr><td>1</td><td>0.01</td><td>0.02</td><td>0.04</td><td>0.05</td><td>0.06</td><td>0.08</td></tr><tr><td>2</td><td>0.01</td><td>0.03</td><td>0.05</td><td>0.05</td><td>0.05</td><td>0.06</td></tr><tr><td>3</td><td>0.01</td><td>0.02</td><td>0.04</td><td>0.06</td><td>0.06</td><td>0.05</td></tr></table>

求 $P\{ X = 2 \mid  Y = 2\},\;P\{ Y = 3 \mid  X = 0\}$.

解 因为 $P\{ X = 2 \mid  Y = 2\}  = \frac{P\{ X = 2, Y = 2\} }{P\{ Y = 2\} }$,由上表可知

$$
P\{ X = 2, Y = 2\}  = {0.05}
$$

$$
P\{ Y = 2\}  = {0.01} + {0.03} + {0.05} + {0.05} + {0.05} + {0.06} = {0.25}
$$

所以 $P\{ X = 2 \mid  Y = 2\}  = \frac{0.05}{0.25} = \frac{1}{5} = {0.2}$

同理 $P\{ X = 0, Y = 3\}  = {0.01}$

$P\{ X = 0\}  = {0.01} + {0.01} + {0.01} = {0.03}$

故 $P\{ Y = 3 \mid  X = 0\}  = \frac{P\{ X = 0, Y = 3\} }{P\{ X = 0\} } = \frac{0.01}{0.03} = \frac{1}{3}$.

【6.21】设随机变量 $\left( {X, Y}\right)  \sim  N\left( {0,{2}^{2};1,{3}^{2};0}\right)$,则 $P\{ \left| {{2X} - Y}\right|  \geq  1\}  =$ _____.

解 因为 $\rho  = 0$,所以 $X$, $Y$ 独立,且 $X \sim  N\left( {0,{2}^{2}}\right), Y \sim  N\left( {1,{3}^{2}}\right)$,则 ${2X} - Y \sim  N\left( {-1,{5}^{2}}\right)$.

故 $\;P\{ \left| {{2X} - Y}\right|  \geq  1\}  = 1 - P\{  - 1 \leq  {2X} - Y \leq  1\}  = 1 - \Phi \left( \frac{2}{5}\right)  + \Phi \left( 0\right)$

$$
= 1 - {0.6554} + {0.5} = {0.8446}
$$

故应填 0.8446.

【6.22】设随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} k\left( {6 - x - y}\right), & 0 < x < 2,2 < y < 4 \\  0, & \text{ 其他 } \end{array}\right.
$$

(1) 确定常数 $k$;

(2) 求 $P\{ X < 1, Y < 3\}$;

(3) 求 $P\{ X < {1.5}\}$;

(4) 求 $P\{ X + Y \leq  4\}$.

解 (1) 因为 ${\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{2}\mathrm{\;d}x{\int }_{2}^{4}k\left( {6 - x - y}\right) \mathrm{d}y = k{\int }_{0}^{2}\left( {6 - {2x}}\right) \mathrm{d}x$

$$
= k\left( {{12} - 4}\right)  = {8k} = 1\text{,}
$$

所以 $k = \frac{1}{8}$.

(2) $P\{ X < 1, Y < 3\}  = {\int }_{0}^{1}\mathrm{\;d}x{\int }_{2}^{3}\frac{1}{8}\left( {6 - x - y}\right) \mathrm{d}y = \frac{1}{8}{\int }_{0}^{1}\left\lbrack  {\left( {6 - x}\right)  - \frac{5}{2}}\right\rbrack  \mathrm{d}x$

$$
= \frac{1}{8}\left( {\frac{7}{2} - \frac{1}{2}}\right)  = \frac{3}{8}\text{.}
$$

(3) $P\{ X < {1.5}\}  = {\int }_{-\infty }^{1.5}{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y\mathrm{\;d}x = {\int }_{0}^{1.5}\left\lbrack  {{\int }_{2}^{4}\frac{1}{8}\left( {6 - x - y}\right) \mathrm{d}y}\right\rbrack  \mathrm{d}x$

$$
= \frac{1}{8}{\int }_{0}^{1.5}\left\lbrack  {2\left( {6 - x}\right)  - 6}\right\rbrack  \mathrm{d}x = \frac{1}{8}{\int }_{0}^{1.5}\left( {6 - {2x}}\right) \mathrm{d}x
$$

$$
= \frac{1}{8}\left\lbrack  {6 \times  {1.5} - {\left( {1.5}\right) }^{2}}\right\rbrack   = \frac{1}{8}\left\lbrack  {9 - \frac{9}{4}}\right\rbrack   = \frac{27}{32}.
$$

(4)将 $\left( {X, Y}\right)$ 看作是平面上随机点的坐标,即有 $\{ X + Y \leq  4\}  = \{ \left( {X, Y}\right)  \in  G\}$,其中 $G$ 为 ${XOY}$ 平面上直线 $x + y = 4$ 下方的部分 (参阅图 3-6.22).

$$
P\{ X + Y \leq  4\}  = P\{ \left( {X, Y}\right)  \in  G\}  = {\iint }_{G}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y
$$

$$
= {\int }_{0}^{2}\mathrm{\;d}x{\int }_{2}^{4 - x}\frac{1}{8}\left( {6 - x - y}\right) \mathrm{d}y
$$

$$
= \frac{1}{8}{\int }_{0}^{2}\left\lbrack  {\left( {6 - x}\right) \left( {2 - x}\right)  - \frac{\left( {6 - x}\right) \left( {2 - x}\right) }{2}}\right\rbrack  \mathrm{d}x
$$

$$
= \frac{1}{16}{\int }_{0}^{2}\left( {{12} - {8x} + {x}^{2}}\right) \mathrm{d}x
$$

$$
= \frac{1}{16}\left\lbrack  {{24} - {16} - \frac{8}{3}}\right\rbrack   = \frac{1}{2} \times  \frac{4}{3} = \frac{2}{3}
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_120_1029_183_284_241_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_120_1029_183_284_241_0.jpg)

图 3-6.22

【6.23】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} 2 - x - y, & 0 < x < 1,0 < y < 1 \\  0, & \text{ 其他. } \end{array}\right.
$$

(1) 求 $P\{ X > {2Y}\}$;

(2)求 $Z = X + Y$ 的概率密度 ${f}_{Z}\left( z\right)$.

解 (1) $P\{ X > {2Y}\}  = {\iint }_{x > {2y}}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{1}\mathrm{\;d}x{\int }_{0}^{\frac{x}{2}}\left( {2 - x - y}\right) \mathrm{d}y$

$$
= {\int }_{0}^{1}\left( {x - \frac{5}{8}{x}^{2}}\right) \mathrm{d}x = \frac{7}{24}.
$$

(2) ${f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, z - x}\right) \mathrm{d}x$,其中

$f\left( {x, z - x}\right)  = \left\{  \begin{array}{ll} 2 - x - \left( {z - x}\right), & 0 < x < 1,0 < z - x < 1 \\  0, & \text{ 其他 } \end{array}\right.$

$$
= \left\{  \begin{array}{ll} 2 - z, & 0 < x < 1,0 < z - x < 1 \\  0, & \text{ 其他,} \end{array}\right.
$$

当 $z \leq  0$ 或 $z \geq  2$ 时, ${f}_{Z}\left( z\right)  = 0$;

当 $0 < z < 1$ 时, ${f}_{Z}\left( z\right)  = {\int }_{0}^{z}\left( {2 - z}\right) \mathrm{d}x = z\left( {2 - z}\right)$;

当 $1 \leq  z < 2$ 时, ${f}_{Z}\left( z\right)  = {\int }_{z - 1}^{1}\left( {2 - z}\right) \mathrm{d}x = {\left( 2 - z\right) }^{2}$,

即 $Z$ 的概率密度为 ${f}_{Z}\left( z\right)  = \left\{  \begin{matrix} z\left( {2 - z}\right), & 0 < z < 1 \\  {\left( 2 - z\right) }^{2}, & 1 \leq  z < 2 \\  0, & \text{ 其他. } \end{matrix}\right.$

#### 题型 4. 关于条件分布

【6.24】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = A{\mathrm{e}}^{-2{x}^{2} + {2xy} - {y}^{2}},\; - \infty  < x <  + \infty, - \infty  < y <  + \infty,
$$

求常数 $A$ 及条件概率密度 ${f}_{Y \mid  X}\left( {y \mid  x}\right)$

解 因 ${f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = A{\int }_{-\infty }^{+\infty }{\mathrm{e}}^{-2{x}^{2} + {2xy} - {y}^{2}}\mathrm{\;d}y = A{\int }_{-\infty }^{+\infty }{\mathrm{e}}^{-{\left( y - x\right) }^{2} - {x}^{2}}\mathrm{\;d}y$

$= A{\mathrm{e}}^{-{x}^{2}}{\int }_{-\infty }^{+\infty }{\mathrm{e}}^{-{\left( y - x\right) }^{2}}\mathrm{\;d}y = A\sqrt{\pi }{\mathrm{e}}^{-{x}^{2}},\; - \infty  < x <  + \infty.$

所以

$$
1 = {\int }_{-\infty }^{+\infty }{f}_{X}\left( x\right) \mathrm{d}x = A\sqrt{\pi }{\int }_{-\infty }^{+\infty }{\mathrm{e}}^{-{x}^{2}}\mathrm{\;d}x = {A\pi },
$$

从而 $A = \frac{1}{\pi }$.

当 $x \in  \left( {-\infty, + \infty }\right)$ 时,

$$
{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{f\left( {x, y}\right) }{{f}_{X}\left( x\right) } = \frac{\frac{1}{\pi }{\mathrm{e}}^{-2{x}^{2} + {2xy} - {y}^{2}}}{\frac{1}{\sqrt{\pi }}{\mathrm{e}}^{-{x}^{2}}} = \frac{1}{\sqrt{\pi }}{\mathrm{e}}^{-{x}^{2} + {2xy} - {y}^{2}}
$$

$$
= \frac{1}{\sqrt{\pi }}{\mathrm{e}}^{-{\left( x - y\right) }^{2}},\; - \infty  < y <  + \infty.
$$

【6.25】设二维随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-x}, & 0 < y < x \\  0, & \text{ 其他. } \end{array}\right.
$$

(1)求条件概率密度 ${f}_{Y \mid  X}\left( {y \mid  x}\right)$;

(2)求条件概率 $P\{ X \leq  1 \mid  Y \leq  1\}$.

解 (1) $X$ 的概率密度

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  {\begin{array}{ll} {\int }_{0}^{x}{\mathrm{e}}^{-x}\mathrm{\;d}y, & x > 0 \\  0, & x \leq  0 \end{array} = \left\{  \begin{array}{ll} x{\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0. \end{array}\right. }\right.
$$

当 $x > 0$ 时, $Y$ 的条件概率密度

$$
{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{f\left( {x, y}\right) }{{f}_{X}\left( x\right) } = \left\{  \begin{array}{ll} \frac{1}{x}, & 0 < y < x \\  0, & \text{ 其他. } \end{array}\right.
$$

(2) $Y$ 的概率密度

$$
{f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0. \end{array}\right.
$$

$$
P\{ X \leq  1 \mid  Y \leq  1\}  = \frac{P\{ X \leq  1, Y \leq  1\} }{P\{ Y \leq  1\} } = \frac{{\int }_{-\infty }^{1}{\int }_{-\infty }^{1}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y}{{\int }_{0}^{1}{\mathrm{e}}^{-y}\mathrm{\;d}y}
$$

$$
= \frac{{\int }_{0}^{1}\mathrm{\;d}x{\int }_{0}^{x}{\mathrm{e}}^{-x}\mathrm{\;d}y}{1 - {\mathrm{e}}^{-1}} = \frac{\mathrm{e} - 2}{\mathrm{e} - 1}.
$$

【6.26】设 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{21}{4}{x}^{2}y, & {x}^{2} \leq  y \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

( 1 )求条件概率密度 ${f}_{Y \mid  X}\left( {y \mid  x}\right)$,特别写出当 $X = \frac{1}{2}$ 时 $Y$ 的条件概率密度；

(2)求条件概率 $P\left\{  {Y \geq  \frac{3}{4} \mid  X = \frac{1}{2}}\right\}$.

解 由

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{21}{4}{x}^{2}y, & {x}^{2} \leq  y \leq  1 \\  0, & \text{ 其他,} \end{array}\right.
$$

可得 ${f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{21}{8}{x}^{2}\left( {1 - {x}^{4}}\right), &  - 1 \leq  x \leq  1 \\  0, & \text{ 其他,} \end{array}\right.$

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{7}{2}{y}^{\frac{5}{2}}, & 0 \leq  y \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

(1) ${f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{f\left( {x, y}\right) }{{f}_{X}\left( x\right) } = \left\{  \begin{matrix} \frac{2y}{1 - {x}^{4}}, & {x}^{2} < y < 1, - 1 < x < 1 \\  0, & \text{ 其他 } \end{matrix}\right.$

$$
{f}_{Y \mid  X}\left( {y \mid  x = \frac{1}{2}}\right)  = \left\{  \begin{array}{ll} \frac{32}{15}y, & \frac{1}{4} < y < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

(2) $P\left\{  {Y \geq  \frac{3}{4}\left| {\;X = \frac{1}{2}}\right. }\right\}   = {\int }_{\frac{3}{4}}^{+\infty }{f}_{Y \mid  X}\left( {y \mid  x = \frac{1}{2}}\right) \mathrm{d}y = {\int }_{\frac{3}{4}}^{1}\frac{32}{15}y\mathrm{\;d}y = \frac{7}{15}$.

【6.27】设随机变量 $\left( {X, Y}\right)$ 服从二维正态分布,且 $X$ 与 $Y$ 不相关, ${f}_{X}\left( x\right),{f}_{Y}\left( y\right)$ 分别表示 $X, Y$ 的概率密度,则在 $Y = y$ 的条件下, $X$ 的条件概率密度 ${f}_{X \mid  Y}\left( {x \mid  y}\right)$ 为(   ).

(A) ${f}_{X}\left( x\right)$ (B) ${f}_{Y}\left( y\right)$ (C) ${f}_{X}\left( x\right) {f}_{Y}\left( y\right)$ (D) $\frac{{f}_{X}\left( x\right) }{{f}_{Y}\left( y\right) }$

解法一 由于 $\left( {X, Y}\right)$ 服从二维正态分布,因此 $X$ 与 $Y$ 不相关可知 $X$ 与 $Y$ 相互独立. 于是有

$$
{f}_{X \mid  Y}\left( {x \mid  y}\right)  = {f}_{X}\left( x\right).
$$

选项(A) 正确.

解法二 由于 $X$ 与 $Y$ 不相关,即 $\rho  = 0$,因此 $\left( {X, Y}\right)$ 的联合密度为

$$
f\left( {x, y}\right)  = \frac{1}{{2\pi }{\sigma }_{1}{\sigma }_{2}}{\mathrm{e}}^{-\frac{1}{2}\left\lbrack  {{\left( \frac{x - {\mu }_{1}}{{\sigma }_{1}}\right) }^{2} + {\left( \frac{y - {\mu }_{2}}{{\sigma }_{2}}\right) }^{2}}\right\rbrack  }.
$$

而 $X, Y$ 的边缘概率密度分别为

$$
{f}_{X}\left( x\right)  = \frac{1}{\sqrt{2\pi }{\sigma }_{1}}{\mathrm{e}}^{-\frac{{\left( x - {\mu }_{1}\right) }^{2}}{2{\sigma }_{1}^{2}}},
$$

$$
{f}_{Y}\left( y\right)  = \frac{1}{\sqrt{2\pi }{\sigma }_{2}}{\mathrm{e}}^{-\frac{{\left( y - {\mu }_{2}\right) }^{2}}{2{\sigma }_{2}^{2}}},
$$

$$
{f}_{X \mid  Y}\left( {x \mid  y}\right)  = \frac{f\left( {x, y}\right) }{{f}_{Y}\left( y\right) } = \frac{1}{\sqrt{2\pi }{\sigma }_{1}}{\mathrm{e}}^{\frac{{\left( x - {\mu }_{1}\right) }^{2}}{2{\sigma }_{1}^{2}}} = {f}_{X}\left( x\right).
$$

故应选 (A).

点评 本题主要考查二维正态分布的性质,我们知道对于任意两个随机变量 $X, Y$ 不相关仅仅是 $X$ 与 $Y$ 独立的必要条件. 但是对于二维正态分布, $X$ 与 $Y$ 不相关是 $X, Y$ 独立的充分必要条件.

题型 5. 与独立性有关的题目

【6.28】设随机变量 $X$ 和 $Y$ 独立,均服从相同的 $\left( {0 - 1}\right)$ 分布:

$$
P\{ X = 1\}  = p,\;P\{ X = 0\}  = 1 - p.
$$

又设 $Z = \left\{  \begin{array}{ll} 0, & X + Y = {偶数} \\  1, & X + Y = {奇数} \end{array}\right.$,则 $p\left( {0 < p < 1}\right)$ 为_____时,能使 $Z$ 和 $X$ 相互独立.

解 由 $X$ 和 $Y$ 独立,易知

$$
P\{ Z = 0\}  = {\left( 1 - p\right) }^{2} + {p}^{2},\;P\{ Z = 1\}  = {2p}\left( {1 - p}\right).
$$

要使 $Z$ 与 $X$ 独立,必须 $P\{ X = i, Z = j\}  = P\{ X = i\} P\{ Z = j\},\;i = 0,1;j = 0,1$,即

$$
\left\{  \begin{array}{l} \left\lbrack  {{\left( 1 - p\right) }^{2} + {p}^{2}}\right\rbrack  \left( {1 - p}\right)  = {\left( 1 - p\right) }^{2} \\  {2p}\left( {1 - p}\right) \left( {1 - p}\right)  = p\left( {1 - p}\right) \\  \left\lbrack  {{\left( 1 - p\right) }^{2} + {p}^{2}}\right\rbrack  p = {p}^{2} \\  {2p}\left( {1 - p}\right) p = p\left( {1 - p}\right)  \end{array}\right.
$$

解得 $p = \frac{1}{2}$.

【6.29】设随机变量 $X$ 与 $Y$ 相互独立,且分别服从参数为 1 与参数为 4 的指数分布,则 $P\{ X$ $< Y\}  =$ _____.

(A) $\frac{1}{5}$ (B) $\frac{1}{3}$ (C) $\frac{2}{3}$ (D) $\frac{4}{5}$

解 因为 $X, Y$ 分别服从参数为 1 与参数为 4 的指数分布,

故 ${f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\;{f}_{Y}\left( y\right)  = \left\{  \begin{matrix} 4{\mathrm{e}}^{-{4y}}, & y > 0 \\  0, & y \leq  0 \end{matrix}\right. }\right.$.

因为 $X$ 与 $Y$ 相互独立,所以 $f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y}\left( y\right)  = \left\{  \begin{matrix} 4{\mathrm{e}}^{-x}{\mathrm{e}}^{-{4y}}, & x > 0, y > 0 \\  0, & \text{ 其他 } \end{matrix}\right.$,

从而 $P\{ X < Y\}  = {\iint }_{x < y}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = {\int }_{0}^{+\infty }\mathrm{d}x{\int }_{0}^{x}4{\mathrm{e}}^{-x - {4y}}\mathrm{\;d}y = \frac{1}{5}$.

故应选 (A).

【6.30】设二维随机变量 $\left( {X, Y}\right)$ 服从正态分布 $N\left( {1,0;1,1;0}\right)$,则 $P\{ {XY} - Y < 0\}  =$ _____.

解 由于相关系数为 0,所以 $X, Y$ 都服从正态分布,即

$$
X \sim  N\left( {1,1}\right), Y \sim  N\left( {0,1}\right),
$$

且 $X$ 和 $Y$ 相互独立.

由 $X \sim  N\left( {1,1}\right)$,可得 $X - 1 \sim  N\left( {0,1}\right)$,所以

$$
P\{ {XY} - Y < 0\}  = P\{ \left( {X - 1}\right) Y < 0\}
$$

$$
= P\{ X - 1 < 0, Y > 0\}  + P\{ X - 1 > 0, Y < 0\}
$$

$$
= P\{ X - 1 < 0\} P\{ Y > 0\}  + P\{ X - 1 > 0\} P\{ Y < 0\}
$$

$$
= \frac{1}{2} \times  \frac{1}{2} + \frac{1}{2} \times  \frac{1}{2} = \frac{1}{2}\text{.}
$$

点评 本题考查了二维正态分布与一维正态分布的重要结论:


① 二维正态分布的边缘分布为一维正态分布,即当 $\left( {X, Y}\right)  \sim  N\left( {{\mu }_{1},{\mu }_{2};{\sigma }_{1}^{2},{\sigma }_{2}^{2};\rho }\right)$ 时,

$$
X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right).
$$

② 二维正态分布独立 $\Leftrightarrow$ 不相关,即 $\rho  = 0 \Leftrightarrow  X$ 与 $Y$ 相互独立.

③ 若 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,则 $P\{ X \leq  \mu \}  = P\{ X > \mu \}  = \frac{1}{2}$. 本题中 $X \sim  N\left( {1,1}\right), Y \sim  N\left( {0,1}\right)$. 则

$$
P\{ X < 1\}  = P\{ X > 1\}  = \frac{1}{2}, P\{ Y < 0\}  = P\{ Y > 0\}  = \frac{1}{2}.
$$

【6.31】设随机变量 $\left( {X, Y}\right)$ 具有分布函数

$$
F\left( {x, y}\right)  = \left\{  {\begin{array}{ll} \left( {1 - {\mathrm{e}}^{-{\alpha x}}}\right) y, & x \geq  0,0 \leq  y \leq  1 \\  1 - {\mathrm{e}}^{-{\alpha x}}, & x \geq  0, y > 1 \\  0, & \text{ 其他 } \end{array},\;\alpha  > 0}\right.
$$

证明 $X, Y$ 相互独立.

解 ${F}_{X}\left( x\right)  = F\left( {x,\infty }\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-{ax}}, & x \geq  0 \\  0, & \text{ 其他. } \end{array}\right.$

$$
{F}_{Y}\left( y\right)  = F\left( {\infty, y}\right)  = \left\{  \begin{array}{ll} y, & 0 \leq  y \leq  1 \\  1, & y > 1 \\  0, & \text{ 其他. } \end{array}\right.
$$

因为对于所有的 $x, y$ 都有 $F\left( {x, y}\right)  = {F}_{X}\left( x\right) {F}_{Y}\left( y\right)$,故 $X, Y$ 相互独立.

【6.32】设 $\left( {X, Y}\right)$ 的联合密度函数为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} A{\mathrm{e}}^{-\left( {{2x} + y}\right) }, & x > 0, y > 0 \\  0, & \text{ 其他. } \end{array}\right.
$$

(1) 确定 $A$;

(2)求 ${f}_{X \mid  Y}\left( {x \mid  y}\right)$ 及 ${f}_{Y \mid  X}\left( {y \mid  x}\right)$,并判断 $X, Y$ 的独立性；

(3) 求 $P\{ X \leq  2 \mid  Y \leq  1\}$;

(4) 求 $P\{ X \leq  2 \mid  Y = 1\}$.

解 (1) 因为 ${\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y = 1$,所以在这里应有

$$
{\int }_{0}^{+\infty }{\int }_{0}^{+\infty }A{\mathrm{e}}^{-\left( {{2x} + y}\right) }\mathrm{d}y\mathrm{\;d}x = \frac{A}{2} = 1
$$

故 $A = 2$.

(2)据公式有

$$
{f}_{X \mid  Y}\left( {x \mid  y}\right)  = \frac{f\left( {x, y}\right) }{{f}_{Y}\left( y\right) },\;{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{f\left( {x, y}\right) }{{f}_{X}\left( x\right) }.
$$

由于 $y \leq  0$ 时, ${f}_{Y}\left( y\right)  = 0, y > 0$ 时, ${f}_{Y}\left( y\right)  = {\int }_{0}^{+\infty }2{\mathrm{e}}^{-\left( {{2x} + y}\right) }\mathrm{d}x = {\mathrm{e}}^{-y}$,所以

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y} & y > 0 \\  0, & y \leq  0. \end{array}\right.
$$

因此, $x > 0, y > 0$ 时, ${f}_{X \mid  Y}\left( {x \mid  y}\right)  = \frac{2{\mathrm{e}}^{-\left( {{2x} + y}\right) }}{{\mathrm{e}}^{-y}} = 2{\mathrm{e}}^{-{2x}}$,所以

$$
{f}_{X \mid  Y}\left( {x \mid  y}\right)  = \left\{  \begin{array}{ll} 2{\mathrm{e}}^{-{2x}}, & x > 0, y > 0 \\  0, & \text{ 其他. } \end{array}\right.
$$

又由于 $x \leq  0$ 时, ${f}_{X}\left( x\right)  = 0, x > 0$ 时, ${f}_{X}\left( x\right)  = {\int }_{0}^{+\infty }2{\mathrm{e}}^{-\left( {{2x} + y}\right) }\mathrm{d}y = 2{\mathrm{e}}^{-{2x}}$,所以

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} 2{\mathrm{e}}^{-{2x}}, & x > 0 \\  0, & x \leq  0. \end{array}\right.
$$

因此, $x > 0, y > 0$ 时, ${f}_{Y \mid  X}\left( {y \mid  x}\right)  = \frac{2{\mathrm{e}}^{-\left( {{2x} + y}\right) }}{2{\mathrm{e}}^{-{2x}}} = {\mathrm{e}}^{-y}$,所以

$$
{f}_{Y \mid  X}\left( {y \mid  x}\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & x > 0, y > 0 \\  0, & \text{ 其他. } \end{array}\right.
$$

从以上所解的结果看出, ${f}_{X \mid  Y}\left( {x \mid  y}\right)  = {f}_{X}\left( x\right),{f}_{Y \mid  X}\left( {y \mid  x}\right)  = {f}_{Y}\left( y\right)$,这说明 $X$ 与 $Y$ 是相互独立的.

(3) 求 $P\{ X \leq  2 \mid  Y \leq  1\}$.

由 (2) 中已判断出 $X, Y$ 相互独立,则

$$
P\{ X \leq  2 \mid  Y \leq  1\}  = P\{ X \leq  2\}  = {F}_{X}\left( 2\right)  = {\int }_{-\infty }^{2}{f}_{X}\left( x\right) \mathrm{d}x = {\int }_{0}^{2}2{\mathrm{e}}^{-{2x}}\mathrm{\;d}x
$$

$$
= 1 - {\mathrm{e}}^{-4} \approx  {0.9817}\text{.}
$$

(4) 求 $P\{ X \leq  2 \mid  Y = 1\}$.

因为 $X, Y$ 相互独立,这个概率与条件 $Y = 1$ 无关.

$$
P\{ X \leq  2 \mid  Y = 1\}  = P\{ X \leq  2 \mid  Y \leq  1\}  = P\{ X \leq  2\}  \approx  {0.9817}.
$$

点评 对于 (2),可以先由 $f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y}\left( y\right)$ 判断出 $X$ 与 $Y$ 相互独立,因此 ${f}_{X \mid  Y}(x \mid$ $\left. y\right)  = {f}_{X}\left( x\right),{f}_{Y \mid  X}\left( {y \mid  x}\right)  = {f}_{Y}\left( y\right)$,计算更加简便.

【6.33】设随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} \frac{1}{2}\left( {x + y}\right) {\mathrm{e}}^{-\left( {x + y}\right) }, & x > 0, y > 0 \\  0, & \text{ 其他 } \end{array}\right.
$$

问 $X$ 和 $Y$ 是否相互独立?

解 $\left( {X, Y}\right)$ 关于 $X$ 的边缘概率密度为

$$
{f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  \begin{array}{ll} {\int }_{0}^{+\infty }\frac{1}{2}\left( {x + y}\right) {\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}y, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} \frac{1}{2}\left( {x + 1}\right) {\mathrm{e}}^{-x}, & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

$\left( {X, Y}\right)$ 关于 $Y$ 的边缘概率密度为

$$
{f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = \left\{  \begin{array}{ll} {\int }_{0}^{+\infty }\frac{1}{2}\left( {x + y}\right) {\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}x, & y > 0 \\  0, & y \leq  0 \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} \frac{1}{2}\left( {y + 1}\right) {\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0 \end{array}\right.
$$

而 ${f}_{X}\left( x\right) {f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{4}\left( {x + 1}\right) \left( {y + 1}\right) {\mathrm{e}}^{-\left( {x + y}\right) }, & x > 0, y > 0 \\  0, & \text{ 其他 } \end{array}\right.$

显然 ${f}_{X}\left( x\right) {f}_{Y}\left( y\right)  \neq  f\left( {x, y}\right)$,故 $X$ 和 $Y$ 不独立.

#### 题型 6. 求多维随机变量函数的分布

【6.34】已知随机变量 $\left( {X, Y}\right)$ 的联合分布律为

<table><tr><td>$X$ Y</td><td>1</td><td>2</td><td>3</td></tr><tr><td>1</td><td>$\frac{1}{5}$</td><td/><td>$\frac{1}{5}$</td></tr><tr><td>2</td><td>$\frac{1}{5}$</td><td>$\frac{1}{5}$</td><td>$\frac{1}{5}$</td></tr></table>

试求 ${Z}_{1} = X + Y,{Z}_{2} = \max \left( {X, Y}\right)$ 的分布律.

解 ${Z}_{1}$ 的所有可能取值为2,3,4,5,而

$P\left\{  {{Z}_{1} = 2}\right\}   = P\{ X + Y = 2\}  = P\{ X = 1, Y = 1\}  = \frac{1}{5}$

$P\left\{  {{Z}_{1} = 3}\right\}   = P\{ X = 1, Y = 2\}  + P\{ X = 2, Y = 1\}  = \frac{1}{5}$

$P\left\{  {{Z}_{1} = 4}\right\}   = P\{ X = 2, Y = 2\}  + P\{ X = 3, Y = 1\}  = \frac{2}{5}$

$P\left\{  {{Z}_{1} = 5}\right\}   = P\{ X = 3, Y = 2\}  = \frac{1}{5}$

因此, ${Z}_{1}$ 的分布律为

<table><tr><td>${Z}_{1}$</td><td>2</td><td>3</td><td>4</td><td>5</td></tr><tr><td>${p}_{k}$</td><td>$\frac{1}{5}$</td><td>$\frac{1}{5}$</td><td>$\frac{2}{5}$</td><td>$\frac{1}{5}$</td></tr></table>

${Z}_{2}$ 的所有可能取值为1,2,3,而

$P\left\{  {{Z}_{2} = 1}\right\}   = P\{ X = 1, Y = 1\}  = \frac{1}{5}$

$P\left\{  {{Z}_{2} = 2}\right\}   = P\{ X = 2, Y = 1\}  + P\{ X = 2, Y = 2\}  + P\{ X = 1, Y = 2\}  = \frac{2}{5}$

$P\left\{  {{Z}_{2} = 3}\right\}   = P\{ X = 3, Y = 1\}  + P\{ X = 3, Y = 2\}  = \frac{2}{5}$

因此, ${Z}_{2}$ 的分布律为

<table><tr><td>${Z}_{2}$1</td><td>2</td><td>3</td></tr><tr><td>${p}_{k}$$\frac{1}{5}$</td><td>$\frac{2}{5}$</td><td>$\frac{2}{5}$</td></tr></table>

【6.35】设 $A, B$ 为随机事件,且 $P\left( A\right)  = \frac{1}{4}, P\left( {B \mid  A}\right)  = \frac{1}{3}, P\left( {A \mid  B}\right)  = \frac{1}{2}$,令

$X = \left\{  {\begin{array}{ll} 1, & A\text{ 发生,} \\  0, & A\text{ 不发生; } \end{array}\;Y = \left\{  \begin{array}{ll} 1, & B\text{ 发生 } \\  0, & B\text{ 不发生 } \end{array}\right. }\right.$

求 (1) 二维随机变量 $\left( {X, Y}\right)$ 的概率分布; $\;\left( 2\right) Z = {X}^{2} + {Y}^{2}$ 的概率分布.

解 (1) 由于 $P\left( {AB}\right)  = P\left( A\right) P\left( {B \mid  A}\right)  = \frac{1}{12}, P\left( B\right)  = \frac{P\left( {AB}\right) }{P\left( {A \mid  B}\right) } = \frac{1}{6}$,所以

$$
P\{ X = 1, Y = 1\}  = P\left( {AB}\right)  = \frac{1}{12},
$$

$$
P\{ X = 1, Y = 0\}  = P\left( {A\bar{B}}\right)  = P\left( A\right)  - P\left( {AB}\right)  = \frac{1}{6},
$$

$$
P\{ X = 0, Y = 1\}  = P\left( {\bar{A}B}\right)  = P\left( B\right)  - P\left( {AB}\right)  = \frac{1}{12},
$$

$P\{ X = 0, Y = 0\}  = P\left( {\bar{A}\bar{B}}\right)  = P\left( \overline{A \cup  B}\right)  = 1 - P\left( {A \cup  B}\right)$

$$
= 1 - \left\lbrack  {P\left( A\right)  + P\left( B\right)  - P\left( {AB}\right) }\right\rbrack   = \frac{2}{3}
$$

$$
\text{(或}P\{ X = 0, Y = 0\}  = 1 - \frac{1}{12} - \frac{1}{6} - \frac{1}{12} = \frac{2}{3}\text{).}
$$

故 $\left( {X, Y}\right)$ 的概率分布为

<table><tr><td>Y</td><td>0</td><td>1</td></tr><tr><td>0</td><td>$\frac{2}{3}$</td><td>$\frac{1}{12}$</td></tr><tr><td>1</td><td>$\frac{1}{6}$</td><td>$\frac{1}{12}$</td></tr></table>

(2) $Z$ 的可能取值为0,1,2,

$$
P\{ Z = 0\}  = P\{ X = 0, Y = 0\}  = \frac{2}{3},
$$

$$
P\{ Z = 1\}  = P\{ X = 0, Y = 1\}  + P\{ X = 1, Y = 0\}  = \frac{1}{4},
$$

$$
P\{ Z = 2\}  = P\{ X = 1, Y = 1\}  = \frac{1}{12},
$$

即 $Z$ 的概率分布为

<table><tr><td>$Z$0</td><td>1</td><td>2</td></tr><tr><td>$p$$\frac{2}{3}$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{12}$</td></tr></table>

【6.36】设随机变量 $X$ 与 $Y$ 相互独立, $X$ 的概率分布为

$$
P\{ X = i\}  = \frac{1}{3}\;\left( {i =  - 1,0,1}\right)
$$

$Y$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} 1, & 0 \leq  y \leq  1 \\  0, & \text{ 其他,} \end{array}\right.
$$

记 $Z = X + Y$.

(1)求 $P\left\{  {\left. {Z \leq  \frac{1}{2}}\right| \;X = 0}\right\}$;

(2)求 $Z$ 的概率密度.

解 (1) $P\left\{  {Z \leq  \frac{1}{2} \mid  X = 0}\right\}   = P\left\{  {X + Y \leq  \frac{1}{2} \mid  X = 0}\right\}   = P\left\{  {Y \leq  \frac{1}{2}}\right\}   = {\int }_{0}^{\frac{1}{2}}1\mathrm{\;d}y = \frac{1}{2}$.

(2)当 $z \geq  2$ 时, $F\left( z\right)  = 1$,

当 $z <  - 1$ 时, $F\left( z\right)  = 0$,

当 $- 1 \leq  z < 2$ 时,

$$
F\left( z\right)  = P\{ Z \leq  z\}  = P\{ X + Y \leq  z\}
$$

$$
= P\{ X + Y \leq  z \mid  X =  - 1\} P\{ X =  - 1\}  + P\{ X + Y \leq  z \mid  X = 0\} P\{ X = 0\}
$$

$$
+ P\{ X + Y \leq  z \mid  X = 1\} P\{ X = 1\}
$$

$$
= \frac{1}{3}\left\lbrack  {P\{ Y \leq  z + 1\}  + P\{ Y \leq  z\}  + P\{ Y \leq  z - 1\} }\right\rbrack
$$

当 $- 1 \leq  z < 0$ 时, $F\left( z\right)  = \frac{1}{3}{\int }_{0}^{z + 1}1\mathrm{\;d}y = \frac{1}{3}\left( {z + 1}\right)$,

当 $0 \leq  z < 1$ 时, $F\left( z\right)  = \frac{1}{3}\left\lbrack  {1 + {\int }_{0}^{z}1\mathrm{\;d}y + 0}\right\rbrack   = \frac{1}{3}\left( {z + 1}\right)$,

当 $1 \leq  z < 2$ 时, $F\left( z\right)  = \frac{1}{3}\left\lbrack  {1 + 1 + {\int }_{0}^{z - 1}1\mathrm{\;d}y}\right\rbrack   = \frac{1}{3}\left( {z + 1}\right)$,

所以 $F\left( z\right)  = \left\{  \begin{array}{ll} 0, & z <  - 1 \\  \frac{1}{3}\left( {z + 1}\right), &  - 1 \leq  z < 2 \\  1, & z \geq  2 \end{array}\right.$

则 $f\left( z\right)  = \left\{  \begin{array}{ll} \frac{1}{3}, &  - 1 \leq  z < 2 \\  0, & \text{ 其他. } \end{array}\right.$

【6.37】某种商品一周的需要量是一个随机变量, 其概率密度为

$$
f\left( t\right)  = \left\{  \begin{array}{ll} t{\mathrm{e}}^{-t} & t > 0 \\  0, & t \leq  0 \end{array}\right.
$$

设各周的需要量是相互独立的, 试求:

(1)两周的需要量的概率密度；

(2)三周的需要量的概率密度.

解 设第 $i$ 周的需求量为 ${T}_{i}\left( {i = 1,2,3}\right)$,由题设知它们是独立同分布的随机变量.

(1)两周的需求量为 ${T}_{1} + {T}_{2}$,其概率密度为

$$
{f}_{{T}_{1} + {T}_{2}}\left( t\right)  = {\int }_{-\infty }^{+\infty }f\left( u\right) f\left( {t - u}\right) \mathrm{d}u = {\int }_{0}^{t}u{\mathrm{e}}^{-u}\left( {t - u}\right) {\mathrm{e}}^{-\left( {t - u}\right) }\mathrm{d}u = \frac{{t}^{3}}{6}{\mathrm{e}}^{-t},\left( {\text{ 当 }t > 0\text{ 时 }}\right)
$$

即 ${f}_{{T}_{1} + {T}_{2}}\left( t\right)  = \left\{  \begin{array}{ll} \frac{1}{6}{t}^{3}{\mathrm{e}}^{-t}, & t > 0 \\  0, & t \leq  0 \end{array}\right.$

(2)三周的需求量为 $\left( {{T}_{1} + {T}_{2}}\right)  + {T}_{3}$,其概率密度为 ${f}_{{T}_{1} + {T}_{2} + {T}_{3}}\left( t\right)  = {\int }_{-\infty }^{+\infty }{f}_{{T}_{1} + {T}_{2}}\left( u\right) f\left( {t - u}\right) \mathrm{d}u = {\int }_{0}^{t}\frac{1}{6}{u}^{3}{\mathrm{e}}^{-u}\left( {t - u}\right) {\mathrm{e}}^{-\left( {t - u}\right) }\mathrm{d}u$

$= \frac{1}{5!}{t}^{5}{\mathrm{e}}^{-t},\;$ 当 $t > 0$ 时

即 ${f}_{{T}_{1} + {T}_{2} + {T}_{3}}\left( t\right)  = \left\{  \begin{array}{ll} \frac{1}{5!}{t}^{5}{\mathrm{e}}^{-t}, & t > 0 \\  0, & t \leq  0 \end{array}\right.$

【6.38】设 $X$ 和 $Y$ 是相互独立的随机变量,其概率密度分别为

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \lambda {\mathrm{e}}^{-{\lambda x}} & x > 0 \\  0, & x \leq  0 \end{array}\right.
$$

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \mu {\mathrm{e}}^{-{\mu y}}, & y > 0 \\  0, & y \leq  0 \end{array}\right.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_129_1048_543_303_312_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_129_1048_543_303_312_0.jpg)

图 3-6.38

其中 $\lambda  > 0,\mu  > 0$ 是常数. 引入随机变量

$$
Z = \left\{  \begin{array}{ll} 1, & X \leq  Y \\  0, & X > Y \end{array}\right.
$$

求 $Z$ 的分布律和分布函数.

解 由于 $Z = \left\{  \begin{array}{ll} 1, & X \leq  Y \\  0, & X > Y \end{array}\right.$ (如图 3-6.38)

$P\{ Z = 1\}  = P\{ X \leq  Y\}  = {\int }_{0}^{+\infty }{\int }_{x}^{+\infty }{\lambda \mu }{\mathrm{e}}^{-\left( {{\lambda x} + {\mu y}}\right) }\mathrm{d}y\mathrm{\;d}x$

$$
= {\int }_{0}^{+\infty }\lambda {\mathrm{e}}^{-\left( {\lambda  + \mu }\right) x}\mathrm{\;d}x
$$

$=  - {\left. \frac{\lambda }{\lambda  + \mu }{\mathrm{e}}^{-\left( {\lambda  + \mu }\right) x}\right| }_{0}^{+\infty } = \frac{\lambda }{\lambda  + \mu }$

$P\{ Z = 0\}  = P\{ X > Y\}  = 1 - P\{ X \leq  Y\}  = 1 - \frac{\lambda }{\lambda  + \mu } = \frac{\mu }{\lambda  + \mu }$

故 $Z$ 的分布律为

<table><tr><td>$Z$</td><td>0</td><td>1</td></tr><tr><td>$p$</td><td/><td/></tr></table>

$Z$ 的分布函数为

$$
{F}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 0, & z < 0 \\  \frac{\mu }{\lambda  + \mu }, & 0 \leq  z < 1 \\  1, & z \geq  1 \end{array}\right.
$$

【6.39】已知随机变量 $X$ 与 $Y$ 相互独立且都服从正态分布 $N\left( {\mu,\frac{1}{2}}\right)$. 如果 $P\{ X + Y \leq  1\}$ $= \frac{1}{2}$,则 $\mu  =$ _____.

解 这是一个反问题,即由 “ $P\{ X + Y \leq  1\}  = \frac{1}{2}$ ” 来确定分布中的未知参数 $\mu$,为此首先要确立 $X + Y$ 的分布,由题设知 $X + Y \sim  N\left( {{2\mu },1}\right)$,因此有

$$
P\{ X + Y \leq  1\}  = \Phi \left( \frac{1 - {2\mu }}{1}\right)  = \frac{1}{2} \Rightarrow  1 - {2\mu } = 0,\;\mu  = \frac{1}{2}.
$$

【6.40】设 $X, Y$ 是相互独立的随机变量, $X \sim  \pi \left( {\lambda }_{1}\right), Y \sim  \pi \left( {\lambda }_{2}\right)$.

证明 $Z = X + Y \sim  \pi \left( {{\lambda }_{1} + {\lambda }_{2}}\right)$.

证 因为 $X, Y$ 分别服从参数 ${\lambda }_{1},{\lambda }_{2}$ 的泊松分布,故 $X, Y$ 的分布律为

$$
P\{ X = k\}  = \frac{{\lambda }_{1}^{k}}{k!}{\mathrm{e}}^{-{\lambda }_{1}},\;{\lambda }_{1} > 0,
$$

$$
P\{ Y = r\}  = \frac{{\lambda }_{2}^{r}}{r!}{\mathrm{e}}^{-{\lambda }_{2}},\;{\lambda }_{2} > 0,
$$

则 $Z = X + Y$ 的分布律为

$$
P\{ Z = i\}  = P\{ X + Y = i\}
$$

$$
= \mathop{\sum }\limits_{{k = 0}}^{i}P\{ X = k\}  \cdot  P\{ Y = i - k\}  = \mathop{\sum }\limits_{{k = 0}}^{i}\frac{{\lambda }_{1}^{k}}{k!}{\mathrm{e}}^{-{\lambda }_{1}} \cdot  \frac{{\lambda }_{2}^{i - k}}{\left( {i - k}\right) !}{\mathrm{e}}^{-{\lambda }_{2}}
$$

$$
= \frac{{\mathrm{e}}^{-\left( {{\lambda }_{1} + {\lambda }_{2}}\right) }}{i!}\mathop{\sum }\limits_{{k = 0}}^{i}\frac{i!}{k!\left( {i - k}\right) !}{\lambda }_{1}^{k}{\lambda }_{2}^{i - k}
$$

$$
= \frac{{\mathrm{e}}^{-\left( {{\lambda }_{1} + {\lambda }_{2}}\right) }}{i!}{\left( {\lambda }_{1} + {\lambda }_{2}\right) }^{i},\;i = 0,1,2,\cdots
$$

即 $Z = X + Y$ 服从参数为 ${\lambda }_{1} + {\lambda }_{2}$ 的泊松分布.

【6.41】设 $X, Y$ 是相互独立的随机变量, $X \sim  B\left( {{n}_{1}, p}\right), Y \sim  B\left( {{n}_{2}, p}\right)$,证明

$$
Z = X + Y \sim  B\left( {{n}_{1} + {n}_{2}, p}\right)
$$

证 $Z$ 的可能值为 $0,1,2,\cdots,{n}_{1} + {n}_{2}$. 因为

$$
\{ Z = i\}  = \{ X + Y = i\}  = \{ X = 0, Y = i\}  \cup  \{ X = 1, Y = i - 1\}  \cup  \cdots  \cup  \{ X = i, Y = 0\}
$$

由于和式中各事件互不相容,且 $X, Y$ 独立,则

$$
P\{ Z = i\}  = \mathop{\sum }\limits_{{k = 0}}^{i}P\{ X = k, Y = i - k\}  = \mathop{\sum }\limits_{{k = 0}}^{i}P\{ X = k\} P\{ Y = i - k\}
$$

$$
= \mathop{\sum }\limits_{{k = 0}}^{i}{C}_{{n}_{1}}^{k}{p}^{k}{\left( 1 - p\right) }^{{n}_{1} - k} \cdot  {C}_{{n}_{2}}^{i - k}{p}^{i - k}{\left( 1 - p\right) }^{{n}_{2} - i + k}
$$

$$
= {p}^{i}{\left( 1 - p\right) }^{{n}_{1} + {n}_{2} - i}\mathop{\sum }\limits_{{k = 0}}^{i}{C}_{{n}_{1}}^{k}{C}_{{n}_{2}}^{i - k}
$$

$$
= {p}^{i}{\left( 1 - p\right) }^{{n}_{1} + {n}_{2} - i} \cdot  {C}_{{n}_{1} + {n}_{2}}^{i},\;i = 0,1,2,\cdots,{n}_{1} + {n}_{2}
$$

上述计算过程中用到了公式 $\mathop{\sum }\limits_{{k = 0}}^{i}{C}_{{n}_{1}}^{k} \cdot  {C}_{{n}_{2}}^{i - k} = {C}_{{n}_{1} + {n}_{2}}^{i}$,所以

$$
Z = X + Y \sim  B\left( {{n}_{1} + {n}_{2}, p}\right)
$$

即 $Z = X + Y$ 服从参数 ${n}_{1} + {n}_{2}, p$ 的二项分布.

【6.42】设随机变量 $X, Y$ 相互独立,且具有相同的分布,它们的概率密度均为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{1 - x}, & x > 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

求 $Z = X + Y$ 的概率密度.

解 由卷积公式

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{\infty }{f}_{X}\left( x\right) {f}_{Y}\left( {z - x}\right) \mathrm{d}x,
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_131_1011_187_332_298_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_131_1011_187_332_298_0.jpg)

图 3-6.42

现在 ${f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{1 - x}, & x > 1 \\  0, & \text{ 其他 } \end{array}\right.$

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{1 - y}, & y > 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

仅当 $\left\{  \begin{array}{l} x > 1 \\  z - x > 1 \end{array}\right.$ 即 $\left\{  \begin{array}{l} x > 1 \\  x < z - 1 \end{array}\right.$ 时,上述积分的被积函数不等于零,由图 3-6.42 即得

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} {\int }_{1}^{z - 1}{\mathrm{e}}^{1 - x}{\mathrm{e}}^{1 - \left( {z - x}\right) }\mathrm{d}x = {\int }_{1}^{z - 1}{\mathrm{e}}^{2 - z}\mathrm{\;d}x, & z > 2 \\  0, & \text{ 其他 } \end{array}\right.
$$

得 ${f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{2 - z}\left( {z - 2}\right), & z > 2 \\  0, & \text{ 其他 } \end{array}\right.$

【6.43】设 $\left( {X, Y}\right)$ 的联合密度函数为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & 0 \leq  x \leq  1, y \geq  0 \\  0, & \text{ 其他 } \end{array}\right.
$$

(1)问 $X, Y$ 是否独立?

( 2 )求 $Z = {2X} + Y$ 的密度函数 ${f}_{Z}\left( z\right)$ 和分布函数 ${F}_{Z}\left( z\right)$;

(3) 求 $P\{ Z > 3\}$.

解 (1) 先求边缘密度函数 ${f}_{X}\left( x\right),{f}_{Y}\left( y\right)$ :

$0 < x < 1$ 时, ${f}_{X}\left( x\right)  = {\int }_{0}^{+\infty }{\mathrm{e}}^{-y}\mathrm{\;d}y = 1$,所以

$$
{f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} 1, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array},\;X \sim  U\left( {0,1}\right).}\right.
$$

$y > 0$ 时, ${f}_{Y}\left( y\right)  = {\int }_{0}^{1}{\mathrm{e}}^{-y}\mathrm{\;d}x = {\mathrm{e}}^{-y}$,所以

$$
{f}_{Y}\left( y\right)  = \left\{  {\begin{array}{ll} {\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0 \end{array}, Y}\right. \text{服从指数分布.}
$$

显然有

$$
{f}_{X}\left( x\right) {f}_{Y}\left( y\right)  = \left\{  {\begin{array}{ll} {\mathrm{e}}^{-y}, & 0 < x < 1, y > 0 \\  0, & \text{ 其他 } \end{array} = f\left( {x, y}\right),}\right.
$$

所以 $X, Y$ 相互独立.

(2) 求 $Z = {2X} + Y$ 的 ${f}_{Z}\left( z\right)$ 和 ${F}_{Z}\left( z\right)$.

方法一

① 先求 ${f}_{Z}\left( z\right)$,因为 $X, Y$ 相互独立,用推广的卷积公式

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }{f}_{X}\left( x\right) {f}_{Y}\left( {z - {2x}}\right) \mathrm{d}x.
$$

首先要进行密度函数非零区域的变换, 由

$$
\left\{  {\begin{array}{l} 0 \leq  x \leq  1 \\  y \geq  0 \end{array} \rightarrow  \left\{  {\begin{array}{l} 0 \leq  x \leq  1 \\  z - {2x} \geq  0 \end{array} \rightarrow  \left\{  \begin{array}{l} 0 \leq  x \leq  1 \\  z \geq  {2x} \end{array}\right. }\right. }\right.
$$

由图 3-6.43-1 看出:

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_132_1034_265_269_324_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_132_1034_265_269_324_0.jpg)

图 3-6.43-1

$z < 0$ 时, ${f}_{Z}\left( z\right)  = 0$

$0 \leq  z \leq  2$ 时, ${f}_{Z}\left( z\right)  = {\int }_{0}^{\frac{z}{2}}{\mathrm{e}}^{-\left( {z - {2x}}\right) }\mathrm{d}x = \frac{1}{2}\left( {1 - {\mathrm{e}}^{-z}}\right)$

$z > 2$ 时, $\;{f}_{Z}\left( z\right)  = {\int }_{0}^{1}{\mathrm{e}}^{-\left( {z - {2x}}\right) }\mathrm{d}x = \frac{1}{2}\left( {{\mathrm{e}}^{2} - 1}\right) {\mathrm{e}}^{-z}$.

所以

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 0, & z < 0 \\  \frac{1}{2}\left( {1 - {\mathrm{e}}^{-z}}\right), & 0 \leq  z \leq  2. \\  \frac{1}{2}\left( {{\mathrm{e}}^{2} - 1}\right) {\mathrm{e}}^{-z}, & z > 2 \end{array}\right.
$$

还可以用另一个卷积公式计算, 由读者自己去做.

② 再求 ${F}_{Z}\left( z\right)$,由 ${f}_{Z}\left( z\right)$ 经过定积分求得

$z < 0$ 时, ${F}_{Z}\left( z\right)  = 0$,

$0 \leq  z \leq  2$ 时, ${F}_{Z}\left( z\right)  = {\int }_{0}^{z}\frac{1}{2}\left( {1 - {\mathrm{e}}^{-z}}\right) \mathrm{d}z = \frac{1}{2}\left( {z - 1 + {\mathrm{e}}^{-z}}\right)$,

$$
{F}_{Z}\left( z\right)  = {\int }_{0}^{2}\frac{1}{2}\left( {1 - {\mathrm{e}}^{-z}}\right) \mathrm{d}z + {\int }_{2}^{z}\frac{1}{2}\left( {{\mathrm{e}}^{2} - 1}\right) {\mathrm{e}}^{-z}\mathrm{\;d}z = 1 + \frac{1}{2}\left( {1 - {\mathrm{e}}^{2}}\right) {\mathrm{e}}^{-z}.
$$

所以

$$
{F}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 0, & z < 0 \\  \frac{1}{2}\left( {z - 1 + {\mathrm{e}}^{-z}}\right), & 0 \leq  z \leq  2. \\  1 + \frac{1}{2}\left( {1 - {\mathrm{e}}^{2}}\right) {\mathrm{e}}^{-z}, & z > 2 \end{array}\right.
$$

方法二

① 先求 ${F}_{Z}\left( z\right)$. 根据 ${F}_{Z}\left( z\right)$ 的定义,用二重积分计算求出.

$$
{F}_{Z}\left( z\right)  = P\{ Z \leq  z\}  = P\{ {2X} + Y \leq  z\}
$$

$$
= {\iint }_{{2x} + y \leq  z}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y.
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_132_1017_1208_286_406_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_132_1017_1208_286_406_0.jpg)

图 3-6.43-2

积分域见图 3-6.43-2.

$z < 0$ 时, ${F}_{Z}\left( z\right)  = 0$,

$0 \leq  z \leq  2$ 时, ${F}_{Z}\left( z\right)  = {\int }_{0}^{\frac{z}{2}}{\int }_{0}^{z - {2x}}{\mathrm{e}}^{-y}\mathrm{\;d}y\mathrm{\;d}x = \frac{1}{2}\left( {z - 1 + {\mathrm{e}}^{-z}}\right)$,

$z > 2$ 时, $\;{F}_{Z}\left( z\right)  = {\int }_{0}^{1}{\int }_{0}^{z - {2x}}{\mathrm{e}}^{-y}\mathrm{\;d}y\mathrm{\;d}x = 1 + \frac{1}{2}\left( {1 - {\mathrm{e}}^{2}}\right) {\mathrm{e}}^{-z}$,

所以

$$
{F}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 0, & z < 0 \\  \frac{1}{2}\left( {z - 1 + {\mathrm{e}}^{-z}}\right), & 0 \leq  z \leq  2. \\  1 + \frac{1}{2}\left( {1 - {\mathrm{e}}^{2}}\right) {\mathrm{e}}^{-z}, & z > 2 \end{array}\right.
$$

② 再求 ${f}_{Z}\left( z\right)$,因为 ${f}_{Z}\left( z\right)  = {F}_{Z}^{\prime }\left( z\right)$,所以

$z < 0$ 时, ${f}_{Z}\left( z\right)  = 0$,

$0 \leq  z \leq  2$ 时, ${f}_{Z}\left( z\right)  = \frac{1}{2}\left( {1 - {\mathrm{e}}^{-z}}\right)$,

$z > 2$ 时, $\;{f}_{Z}\left( z\right)  = \frac{1}{2}\left( {{\mathrm{e}}^{2} - 1}\right) {\mathrm{e}}^{-z}$,

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} 0, & z < 0 \\  \frac{1}{2}\left( {1 - {\mathrm{e}}^{-z}}\right), & 0 \leq  z \leq  2. \\  \frac{1}{2}\left( {{\mathrm{e}}^{2} - 1}\right) {\mathrm{e}}^{-z}, & z > 2 \end{array}\right.
$$

这里所用的方法比方法一好,一是不必记公式,二是求导比积分容易,因此,这是求函数的分布的最好方法.

(3) 求 $P\{ Z > 3\}$

利用已经得出的分布函数 ${F}_{Z}\left( z\right)$,

$$
P\{ Z > 3\}  = 1 - P\{ Z \leq  3\}  = 1 - {F}_{Z}\left( 3\right)  = 1 - \left\lbrack  {1 + \frac{1}{2}\left( {1 - {\mathrm{e}}^{2}}\right) {\mathrm{e}}^{-3}}\right\rbrack
$$

$$
= \frac{1}{2}\left( {{\mathrm{e}}^{2} - 1}\right) {\mathrm{e}}^{-3} \approx  {0.1591}.
$$

【6.44】设随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} b{\mathrm{e}}^{-\left( {x + y}\right) }, & 0 < x < 1,0 < y <  + \infty \\  0, & \text{ 其他 } \end{array}\right.
$$

(1) 试确定常数 $b$;

(2)求边缘概率密度 ${f}_{X}\left( x\right),{f}_{Y}\left( y\right)$;

(3)求函数 $U = \max \left( {X, Y}\right)$ 的分布函数.

解 (1) 由联合概率密度性质知

$$
1 = {\int }_{-\infty }^{+\infty }{\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y
$$

$$
= {\int }_{0}^{1}\left\lbrack  {{\int }_{0}^{+\infty }b{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}y}\right\rbrack  \mathrm{d}x = b{\int }_{0}^{1}{\mathrm{e}}^{-x}\mathrm{\;d}x{\int }_{0}^{+\infty }{\mathrm{e}}^{-y}\mathrm{\;d}y
$$

$$
= \left( {1 - {\mathrm{e}}^{-1}}\right) b
$$

所以 $b = \frac{1}{1 - {\mathrm{e}}^{-1}}$.

(2) ${f}_{X}\left( x\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}y = \left\{  \begin{array}{ll} {\int }_{0}^{+\infty }\frac{1}{1 - {\mathrm{e}}^{-1}}{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}y, & 0 < x < \\  0, & \text{ 其他 } \end{array}\right.$

$$
= \left\{  \begin{array}{ll} \frac{{\mathrm{e}}^{-x}}{1 - {\mathrm{e}}^{-1}}, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
{f}_{Y}\left( y\right)  = {\int }_{-\infty }^{+\infty }f\left( {x, y}\right) \mathrm{d}x = \left\{  \begin{array}{ll} {\int }_{0}^{1}\frac{1}{1 - {\mathrm{e}}^{-1}}{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}x, & y > 0 \\  0, & y \leq  0 \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0 \end{array}\right.
$$

(3) $U = \max \left( {X, Y}\right)$ 的分布函数

$$
{F}_{U}\left( u\right)  = P\{ U \leq  u\}  = P\{ X \leq  u, Y \leq  u\}  = F\left( {u, u}\right)  = {\int }_{-\infty }^{u}{\int }_{-\infty }^{u}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y
$$

$$
= \left\{  \begin{array}{ll} 0, & u \leq  0 \\  {\int }_{0}^{u}{\int }_{0}^{u}\frac{1}{1 - {\mathrm{e}}^{-1}}{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}x\mathrm{\;d}y, & 0 < u < 1 \\  {\int }_{0}^{1}{\int }_{0}^{u}\frac{1}{1 - {\mathrm{e}}^{-1}}{\mathrm{e}}^{-\left( {x + y}\right) }\mathrm{d}x\mathrm{\;d}y, & u \geq  1 \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} 0, & u \leq  0 \\  \frac{1}{1 - {\mathrm{e}}^{-1}}{\int }_{0}^{u}{\mathrm{e}}^{-x}\mathrm{\;d}x{\int }_{0}^{u}{\mathrm{e}}^{-y}\mathrm{\;d}y, & 0 < u < 1 \\  \frac{1}{1 - {\mathrm{e}}^{-1}}{\int }_{0}^{1}{\mathrm{e}}^{-x}\mathrm{\;d}x{\int }_{0}^{u}{\mathrm{e}}^{-y}\mathrm{\;d}y, & u \geq  1 \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} 0, & u \leq  0 \\  \frac{{\left( 1 - {\mathrm{e}}^{-u}\right) }^{2}}{1 - {\mathrm{e}}^{-1}} & 0 < u < 1. \\  1 - {\mathrm{e}}^{-u}, & u \geq  1 \end{array}\right.
$$

【6.45】设某种型号的电子元件的寿命 (以小时计) 近似地服从 $N\left( {{160},{20}^{2}}\right)$ 分布. 随机地选取 4 只. 求其中没有一只寿命小于 180 的概率.

解 随机地取 4 只,记其寿命分别为 ${X}_{1},{X}_{2},{X}_{3},{X}_{4}$,由题设知,它们独立同分布,且

$$
{X}_{i} \sim  N\left( {{160},{20}^{2}}\right),\;i = 1,2,3,4
$$

记 $X = \min \left( {{X}_{1},{X}_{2},{X}_{2},{X}_{4}}\right)$,事件“没有一只寿命小于 180 ” 就是 $\{ X \geq  {180}\}$,从而

$$
P\{ X \geq  {180}\}  = 1 - P\{ X < {180}\}  = {\left\lbrack  1 - F\left( {180}\right) \right\rbrack  }^{4} = {\left\lbrack  1 - \Phi \left( \frac{{180} - {160}}{20}\right) \right\rbrack  }^{4}
$$

$$
= {\left( 1 - {0.8413}\right) }^{4} = {0.000634}.
$$

【6.46】设 $X, Y$ 是相互独立的随机变量,它们都服从正态分布 $N\left( {0,{\sigma }^{2}}\right)$. 试验证随机变量 $Z$ $= \sqrt{{X}^{2} + {Y}^{2}}$ 具有概率密度

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} \frac{z}{{\sigma }^{2}}{\mathrm{e}}^{\frac{-{z}^{2}}{2{\sigma }^{2}}}, & z \geq  0 \\  0, & \text{ 其他 } \end{array}\right.
$$

我们称 $Z$ 服从参数为 $\sigma \left( {\sigma  > 0}\right)$ 的瑞利 (Rayleigh) 分布.

证 由 $X, Y$ 独立同分布有

$$
f\left( {x, y}\right)  = {f}_{X}\left( x\right) {f}_{Y}\left( y\right)  = \frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{\frac{-{x}^{2}}{2{\sigma }^{2}}} \cdot  \frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{\frac{-{y}^{2}}{2{\sigma }^{2}}} = \frac{1}{{2\pi }{\sigma }^{2}}{\mathrm{e}}^{-\frac{1}{2{\sigma }^{2}}\left( {{x}^{2} + {y}^{2}}\right) }
$$

而 $Z = \sqrt{{X}^{2} + {Y}^{2}}$

当 $z < 0$ 时, $\{ Z \leq  z\}$ 是不可能事件, ${F}_{Z}\left( z\right)  = P\{ Z \leq  z\}  = 0$,从而 ${f}_{Z}\left( z\right)  = 0$

当 $z \geq  0$ 时,

$$
{F}_{Z}\left( z\right)  = P\{ Z \leq  z\}  = P\left\{  {\sqrt{{X}^{2} + {Y}^{2}} \leq  z}\right\}   = P\left\{  {{X}^{2} + {Y}^{2} \leq  {z}^{2}}\right\}
$$

$$
= {\iint }_{D}f\left( {x, y}\right) \mathrm{d}x\mathrm{\;d}y\;\left( {D : {x}^{2} + {y}^{2} \leq  {z}^{2}, z \geq  0}\right)
$$

$$
= {\iint }_{D}\frac{1}{{2\pi }{\sigma }^{2}}{\mathrm{e}}^{-\frac{1}{2{\sigma }^{2}}\left( {{x}^{2} + {y}^{2}}\right) }\mathrm{d}x\mathrm{\;d}y
$$

$$
= {\int }_{0}^{2\pi }\mathrm{d}\theta {\int }_{0}^{z}\frac{1}{{2\pi }{\sigma }^{2}}{\mathrm{e}}^{-\frac{{r}^{2}}{2{\sigma }^{2}}}r\mathrm{\;d}r = 1 - {\mathrm{e}}^{-\frac{{z}^{2}}{2{\sigma }^{2}}}
$$

从而 ${f}_{Z}\left( z\right)  = {F}_{Z}{}^{\prime }\left( z\right)  = \frac{z}{{\sigma }^{2}}{\mathrm{e}}^{\frac{-{z}^{2}}{2{\sigma }^{2}}}$

故 $\;{f}_{Z}\left( z\right)  = \left\{  \begin{matrix} \frac{z}{{\sigma }^{2}}{\mathrm{e}}^{\frac{-{z}^{2}}{2{\sigma }^{2}}}, & z \geq  0 \\  0, & \text{ 其他 } \end{matrix}\right.$

【6.47】对某种电子装置的输出测量了 5 次,得到观察 ${X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}$. 设它们是相互独立的随机变量,都服从参数 $\sigma  = 2$ 的瑞利分布 (其密度见上题).

(1)求 $Z = \max \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)$ 的分布函数；

(2) 求 $P\{ Z > 4\}$.

解 由题设知 ${X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}$ 相互独立,且具有相同的密度函数

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{x}{4}{\mathrm{e}}^{-\frac{{x}^{2}}{8}}, & x \geq  0 \\  0, & x < 0 \end{array}\right.
$$

由此得到分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 1 - {\mathrm{e}}^{-\frac{{x}^{2}}{8}}, & x \geq  0 \\  0, & x < 0 \end{array}\right.
$$

(1) $Z = \max \left( {{X}_{1},{X}_{2},{X}_{3},{X}_{4},{X}_{5}}\right)$

${F}_{\max }\left( z\right)  = {\left\lbrack  F\left( z\right) \right\rbrack  }^{5} = {\left( 1 - {\mathrm{e}}^{-\frac{{z}^{2}}{8}}\right) }^{5}$,即 ${F}_{\max }\left( z\right)  = \left\{  \begin{array}{ll} {\left( 1 - {\mathrm{e}}^{-\frac{{z}^{2}}{8}}\right) }^{5}, & z \geq  0 \\  0, & z < 0 \end{array}\right.$

(2) $P\{ Z > 4\}  = 1 - P\{ Z \leq  4\}  = 1 - {F}_{\max }\left( 4\right)  = 1 - {\left( 1 - {\mathrm{e}}^{-2}\right) }^{5} = {0.5167}$.

【6.48】设二维随机变量 $\left( {X, Y}\right)$ 在区域 $D = \left\{  {\left( {x, y}\right)  \mid  0 < x < 1,{x}^{2} < y < \sqrt{x}}\right\}$ 上服从均匀分布,令 $U = \left\{  \begin{array}{l} 1, X \leq  Y, \\  0, X > Y. \end{array}\right.$

(1)写出 $\left( {X, Y}\right)$ 的概率密度;

(2)问 $U$ 与 $X$ 是否相互独立？并说明理由；

(3)求 $Z = U + X$ 的分布函数 $F\left( z\right)$.

解 $\left( 1\right) \left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} 3, & \left( {x, y}\right)  \in  D, \\  0, & \text{ 其他 } \end{array}\right.
$$

(2)对于 $0 < t < 1$,

$$
P\{ U \leq  0, X \leq  t\}  = P\{ X > Y, X \leq  t\}
$$

$$
= {\int }_{0}^{t}\mathrm{\;d}x{\int }_{{x}^{2}}^{x}3\mathrm{\;d}y
$$

$$
= \frac{3}{2}{t}^{2} - {t}^{3},
$$

$$
P\{ U \leq  0\}  = P\{ X > Y\}  = \frac{1}{2},
$$

$$
P\{ X \leq  t\}  = {\int }_{0}^{t}\mathrm{\;d}x{\int }_{{x}^{2}}^{\sqrt{x}}3\mathrm{\;d}y = 2{t}^{\frac{3}{2}} - {t}^{3}.
$$

由于 $P\{ U \leq  0, X \leq  t\}  \neq  P\{ U \leq  0\} P\{ X \leq  t\}$,所以 $U$ 与 $X$ 不相互独立.

(3) 当 $z < 0$ 时, $F\left( z\right)  = 0$; 当 $0 \leq  z < 1$ 时,

$$
F\left( z\right)  = P\{ Z \leq  z\}  = P\{ U + X \leq  z\}  = P\{ U = 0, X \leq  z\}
$$

$$
= P\{ X > Y, X \leq  z\}  = \frac{3}{2}{z}^{2} - {z}^{3};
$$

当 $1 \leq  z < 2$ 时, $F\left( z\right)  = P\{ U + X \leq  z\}  = P\{ U = 0, X \leq  z\}  + P\{ U = 1, X \leq  z - 1\}$

$$
= \frac{1}{2} + 2{\left( z - 1\right) }^{\frac{3}{2}} - \frac{3}{2}{\left( z - 1\right) }^{2};
$$

当 $z \geq  2$ 时, $F\left( z\right)  = P\{ U + X \leq  z\}  = 1$.

所以 $F\left( z\right)  = \left\{  \begin{array}{ll} 0, & z < 0, \\  \frac{3}{2}{z}^{2} - {z}^{3}, & 0 \leq  z < 1, \\  \frac{1}{2} + 2{\left( z - 1\right) }^{\frac{3}{2}} - \frac{3}{2}{\left( z - 1\right) }^{2}, & 1 \leq  z < 2, \\  1, & z \geq  2. \end{array}\right.$

【6.49】设随机变量 $X, Y$ 相互独立,它们的概率密度均为

$$
f\left( x\right)  = \left\{  {\begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & \text{ 其他 } \end{array}.}\right.
$$

求 $Z = \frac{Y}{X}$ 的概率密度.

解 ${f}_{X}\left( x\right)  = \left\{  {\begin{array}{ll} {\mathrm{e}}^{-x}, & x > 0 \\  0, & \text{ 其他 } \end{array},\;{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-y}, & y > 0 \\  0, & \text{ 其他 } \end{array}\right. }\right.$.

由公式

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\left| x\right| {f}_{X}\left( x\right) {f}_{Y}\left( {xz}\right) \mathrm{d}x
$$

仅当 $\left\{  \begin{array}{l} x > 0 \\  {xz} > 0 \end{array}\right.$,即 $\left\{  \begin{array}{l} x > 0 \\  z > 0 \end{array}\right.$ 时,上述积分的被积函数不等于零,于是

当 $z > 0$ 时

$$
{f}_{Z}\left( z\right)  = {\int }_{0}^{\infty }x{\mathrm{e}}^{-x}{\mathrm{e}}^{-{xz}}\mathrm{\;d}x = {\int }_{0}^{\infty }x{\mathrm{e}}^{-x\left( {z + 1}\right) }\mathrm{d}x = \frac{1}{{\left( z + 1\right) }^{2}}.
$$

当 $z \leq  0$ 时, ${f}_{Z}\left( z\right)  = 0$,即

$$
{f}_{Z}\left( z\right)  = \left\{  {\begin{array}{ll} \frac{1}{{\left( z + 1\right) }^{2}}, & z > 0 \\  0, & z \leq  0 \end{array}.}\right.
$$

【6.50】设随机变量 $\left( {X, Y}\right)$ 的概率密度为

$$
f\left( {x, y}\right)  = \left\{  \begin{array}{ll} x + y, & 0 < x < 1,0 < y < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

求 $Z = {XY}$ 的概率密度.

解 利用公式, $Z = {XY}$ 的概率密度

$$
{f}_{Z}\left( z\right)  = {\int }_{-\infty }^{+\infty }\frac{1}{\left| x\right| }f\left( {x,\frac{z}{x}}\right) \mathrm{d}x
$$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_137_1000_598_354_289_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_137_1000_598_354_289_0.jpg)

图 3-6.50

易知仅当 $\left\{  \begin{array}{l} 0 < x < 1 \\  0 < \frac{z}{x} < 1 \end{array}\right.$,即 $\left\{  \begin{array}{l} 0 < x < 1 \\  0 < z < x \end{array}\right.$ 时,

被积函数不等于零, 如图 3-6.50.

$$
{f}_{Z}\left( z\right)  = \left\{  \begin{array}{ll} {\int }_{z}^{1}\frac{1}{x}\left( {x + \frac{z}{x}}\right) \mathrm{d}x, & 0 < z < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} 2\left( {1 - z}\right), & 0 < z < 1 \\  0, & \text{ 其他 } \end{array}\right.
$$

电 138