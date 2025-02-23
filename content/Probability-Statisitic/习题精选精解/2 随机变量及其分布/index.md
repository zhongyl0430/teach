## § 1. 随机变量与分布函数

### 知识要点

#### 1. 随机变量 
设 $E$ 是一个随机试验,其样本空间为 $\Omega  = \{ \omega \}$,如果对于每一个样本点 $\omega  \in$ $\Omega$,都有唯一的一个实数 $X\left( \omega \right)$ 与之对应,则称 $X\left( \omega \right)$ 为一维随机变量. 通常用 $X, Y, Z,\cdots$ 表示随机变量.

#### 2. 分布函数 
设 $X$ 是一个随机变量, $x$ 是任意实数,则函数 $F\left( x\right)  = P\{ X \leq  x\}$ 称为 $X$ 的分布函数.

基本性质

(1)单调性: $F\left( x\right)$ 是一个单调不减的函数,即当 ${x}_{1} < {x}_{2}$ 时, $F\left( {x}_{1}\right)  \leq  F\left( {x}_{2}\right)$

(2) 有界性: $0 \leq  F\left( x\right)  \leq  1$,且

$$
F\left( {+\infty }\right)  = \mathop{\lim }\limits_{{x \rightarrow   + \infty }}F\left( x\right)  = 1
$$

$$
F\left( {-\infty }\right)  = \mathop{\lim }\limits_{{x \rightarrow   - \infty }}F\left( x\right)  = 0
$$

(3)连续性: $F\left( {x + 0}\right)  = F\left( x\right)$,即 $F\left( x\right)$ 是右连续函数.

#### 3. 由分布函数求概率

$$
P\{ a < X \leq  b\}  = P\{ X \leq  b\}  - P\{ X \leq  a\}  = F\left( b\right)  - F\left( a\right).
$$

### 基本题型

#### 题型: 关于分布函数

【1.1】设 ${F}_{1}\left( x\right)$ 与 ${F}_{2}\left( x\right)$ 分别为随机变量 ${X}_{1}$ 与 ${X}_{2}$ 的分布函数. 为使 $F\left( x\right)  = a{F}_{1}\left( x\right)  -$ $b{F}_{2}\left( x\right)$ 是某一随机变量的分布函数,下列给定各组数值中应取 (   ).

(A) $a = \frac{3}{5}, b =  - \frac{2}{5}$ (B) $a = \frac{2}{3}, b = \frac{2}{3}$

(C) $a =  - \frac{1}{2}, b = \frac{3}{2}$ (D) $a = \frac{1}{2}, b =  - \frac{3}{2}$

分析 本题是考查对分布函数性质 $\mathop{\lim }\limits_{{x \rightarrow   + \infty }}F\left( x\right)  = 1$ 的掌握.

解 由 $\mathop{\lim }\limits_{{x \rightarrow   + \infty }}F\left( x\right)  = 1$,结合已知条件得

$$
\mathop{\lim }\limits_{{x \rightarrow   + \infty }}F\left( x\right)  = F\left( {+\infty }\right)  = a{F}_{1}\left( {+\infty }\right)  - b{F}_{2}\left( {+\infty }\right)
$$

因为 $\mathop{\lim }\limits_{{x \rightarrow   + \infty }}F\left( x\right)  = F\left( {+\infty }\right)  = a{F}_{1}\left( {+\infty }\right)  - b{F}_{2}\left( {+\infty }\right)  = 1$,且分布函数非负不减,则必有

$$
a > 0, b < 0, a - b = 1.
$$

经验证, 答案为 (A), 故选 (A).

【1.2】下列函数中,可以做随机变量的分布函数的是(   ).

(A) $F\left( x\right)  = \frac{1}{1 + {x}^{2}}$ (B) $F\left( x\right)  = \frac{3}{4} + \frac{1}{2\pi }\arctan x$

(C) $F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x \leq  0 \\  \frac{x}{1 + x}, & x > 0 \end{array}\right.$ (D) $F\left( x\right)  = \frac{2}{\pi }\arctan x + 1$

解 (A) $F\left( {+\infty }\right)  = 0$,(B) $F\left( {-\infty }\right)  \neq  0,\left( D\right) F\left( {+\infty }\right)  \neq  1$,

对于(C) 满足:

(1) $0 \leq  F\left( x\right)  \leq  1, F\left( {-\infty }\right)  = 0, F\left( {+\infty }\right)  = 1$ (2) ${F}^{\prime }\left( x\right)  > 0$ (3) $F\left( x\right)$ 连续.

故应选(C).

【1.3】设随机变量 $X$ 的分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0 \\  \frac{x}{3}, & 0 \leq  x < 1 \\  \frac{x}{2}, & 1 \leq  x < 2 \\  1, & x \geq  2 \end{array}\right.
$$

求: (1) $P\left\{  {\frac{1}{2} < X \leq  \frac{3}{2}}\right\}$; (2) $P\left\{  {X > \frac{1}{2}}\right\}$; (3) $P\left\{  {X > \frac{3}{2}}\right\}$.

解 (1) $P\left\{  {\frac{1}{2} < X \leq  \frac{3}{2}}\right\}   = F\left( \frac{3}{2}\right)  - F\left( \frac{1}{2}\right)  = \frac{3}{4} - \frac{1}{6} = \frac{7}{12}$;

(2) $P\left\{  {X > \frac{1}{2}}\right\}   = 1 - P\left\{  {X \leq  \frac{1}{2}}\right\}   = 1 - F\left( \frac{1}{2}\right)  = 1 - \frac{1}{6} = \frac{5}{6}$;

(3) $P\left\{  {X > \frac{3}{2}}\right\}   = 1 - F\left( \frac{3}{2}\right)  = 1 - \frac{3}{4} = \frac{1}{4}$.

点评 分布函数可以完整、准确地描述随机变量的取值规律. 利用 $X$ 的分布函数可求如下概率:

${1}^{ \circ  }P\{ X \leq  b\}  = F\left( b\right)$

${2}^{ \circ  }P\{ X > b\}  = 1 - F\left( b\right)$

${3}^{ \circ  }P\{ a < X \leq  b\}  = F\left( b\right)  - F\left( a\right)$

其他情形的概率需根据随机变量的类型——离散型或连续型分别讨论归纳.

【1.4】一个靶子是半径为 2 米的圆盘, 设击中靶上任一同心圆盘上的点的概率与该圆盘的面积成正比,并设射击都能中靶,以 $X$ 表示弹着点与圆心的距离. 试求随机变量 $X$ 的分布函数.

解 若 $x < 0$,则 $\{ X \leq  x\}$ 是不可能事件,于是

$$
F\left( x\right)  = P\{ X \leq  x\}  = 0.
$$

若 $0 \leq  x \leq  2$,由题意, $P\{ 0 \leq  X \leq  x\}  = k{x}^{2}, k$ 是某一常数,为了确定 $k$ 的值,取 $x = 2$,有 $P\{ 0 \leq  X \leq  2\}  = {2}^{2}k$,但已知 $P\{ 0 \leq  X \leq  2\}  = 1$,故得 $k = \frac{1}{4}$,即

$$
P\{ 0 \leq  X \leq  x\}  = \frac{{x}^{2}}{4}
$$

于是

$$
F\left( x\right)  = P\{ X \leq  x\}  = P\{ X < 0\}  + P\{ 0 \leq  X \leq  x\}  =
$$

$\frac{{x}^{2}}{4}$

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_38_960_181_343_238_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_38_960_181_343_238_0.jpg)

图 2-1.4

若 $x > 2$,由题意 $\{ X \leq  x\}$ 是必然事件,于是

$$
F\left( x\right)  = P\{ X \leq  x\}  = 1
$$

综合上述,即得 $X$ 的分布函数

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0 \\  \frac{{x}^{2}}{4}, & 0 \leq  x \leq  2 \\  1, & x > 2 \end{array}\right.
$$

它的图形是一条连续曲线如图 2-1.4 所示.

## § 2. 离散型随机变量及其分布

### 知识要点

#### 1. 一维离散型随机变量

若随机变量 $X$ 的全部可能取值是有限个或可列个,则称 $X$ 为离散型随机变量.

#### 2. 分布律

离散型随机变量 $X$ 所有可能取值为 ${x}_{k}\left( {k = 1,2,\cdots }\right)$,事件 $\left\{  {X = {x}_{k}}\right\}$ 的概率为 $P\left\{  {X = {x}_{k}}\right\}   =$ ${p}_{k}\left( {k = 1,2,\cdots }\right)$,则称 $P\left\{  {X = {x}_{k}}\right\}   = {p}_{k}\left( {k = 1,2,\cdots }\right)$ 为 $X$ 的分布律或分布列. 分布律也可以写成表格形式:

<table><tr><td>$X$</td><td>${x}_{1}$</td><td>${x}_{2}$</td><td>...</td><td>${x}_{k}$</td><td>...</td></tr><tr><td>$P$</td><td>${p}_{1}$</td><td>${p}_{2}$</td><td>...</td><td>${p}_{k}$</td><td>...</td></tr></table>

离散型随机变量的分布律的性质:

(1) $P\left\{  {X = {x}_{k}}\right\}   = {p}_{k} \geq  0, k = 1,2,\cdots$;

(2) $\mathop{\sum }\limits_{k}P\left\{  {X = {x}_{k}}\right\}   = \mathop{\sum }\limits_{k}{p}_{k} = 1$.

#### 3. 离散型随机变量 $X$ 的分布律与分布函数以及事件概率的关系

(1)如果已知 $X$ 的分布律为 $P\left\{  {X = {x}_{k}}\right\}   = {p}_{k}\left( {k = 1,2,\cdots }\right)$,则 $X$ 的分布函数

$$
F\left( x\right)  = P\{ X \leq  x\}  = \mathop{\sum }\limits_{{{x}_{k} \leq  x}}{p}_{k}
$$

而事件 $\{ a < X \leq  b\}$ 的概率为

$$
P\{ a < X \leq  b\}  = \mathop{\sum }\limits_{{a < {x}_{k} \leq  b}}{p}_{k}.
$$

(2)如果已知 $X$ 的分布函数 $F\left( x\right)$,则 $X$ 的分布律为

$$
P\left\{  {X = {x}_{k}}\right\}   = F\left( {x}_{k}\right)  - F\left( {{x}_{k} - 0}\right),\;k = 1,2,\cdots.
$$

概率论与数理统计习题精选精解

#### 4. 重要分布

(1) (0-1)分布: 其分布律为

<table><tr><td>$X$</td><td>1</td><td>0</td></tr><tr><td>$P$</td><td>$p$</td><td>$1 - p$</td></tr></table>

其中 $p$ 为事件 $A$ 出现的概率, $0 < p < 1$.

(2)二项分布:设在 $n$ 重伯努利试验中事件 $A$ 发生的次数为 $X$,则

$$
P\{ X = k\}  = {C}_{n}^{k}{p}^{k}{q}^{n - k},\;k = 0,1,2,\cdots \cdots, n
$$

其中 $p$ 为事件 $A$ 在每次试验中出现的概率, $q = 1 - p$,称随机变量 $X$ 服从二项分布,记为

$$
X \sim  B\left( {n, p}\right).
$$

(3)泊松分布:设随机变量 $X$ 的分布律为:

$$
P\{ X = k\}  = \frac{{\lambda }^{k}{\mathrm{e}}^{-\lambda }}{k!}\;\left( {k = 0,1,2,\cdots }\right)
$$

其中 $\lambda  > 0$ 是常数,则称 $X$ 服从参数为 $\lambda$ 的泊松分布,记为 $X \sim  \pi \left( \lambda \right)$ 或 $P\left( \lambda \right)$.

泊松定理: 设随机变量 ${X}_{n} \sim  B\left( {n,{p}_{n}}\right)$,若 $\mathop{\lim }\limits_{{n \rightarrow  \infty }}n{p}_{n} = \lambda  > 0$,则有

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}{C}_{n}^{i}{p}_{n}^{i}{\left( 1 - {p}_{n}\right) }^{n - i} = \frac{{\lambda }^{i}}{i!}{\mathrm{e}}^{-\lambda }\;\left( {i = 1,2,\cdots }\right)
$$

由泊松定理, 二项分布可以用泊松分布作为近似.

(4)超几何分布:设随机变量 $X$ 的分布列是

$$
P\{ X = i\}  = \frac{{C}_{M}^{i}{C}_{N - M}^{n - i}}{{C}_{N}^{n}},\;\left( {i = 0,1,2,\cdots, l;l = \min \{ n, M\} }\right).
$$

其中 $M\text{、}N\text{、}n$ 都是自然数,且 $n < N, M < N$,则称 $X$ 服从参数为 $N\text{、}M\text{、}n$ 的超几何分布,记作 $X$ $\sim  H\left( {N, M, n}\right)$.

(5)几何分布: 设随机变量 $X$ 的分布列为

$$
P\{ X = i\}  = {\left( 1 - p\right) }^{i - 1}p,\;i = 1,2,3,\cdots,
$$

其中 $0 < p < 1$,则称 $X$ 服从参数为 $p$ 的几何分布,记为 $X \sim  G\left( p\right)$.

### 基本题型

#### 题型 1: 关于分布律的性质

【2. 1】当 $C =$ _____时, $P\{ X = k\}  = C \cdot  {\left( \frac{2}{3}\right) }^{k}\left( {k = 1,2,3,\cdots }\right)$ 才能成为随机变量 $X$ 的分布列.

解 由分布列的性质 $\mathop{\sum }\limits_{k}{p}_{k} = 1$,所以

$$
\mathop{\sum }\limits_{{k = 1}}^{\infty }C \cdot  {\left( \frac{2}{3}\right) }^{k} = 1\;\text{ 即 }C\left\lbrack  {\frac{2}{3} + {\left( \frac{2}{3}\right) }^{2} + \cdots  + {\left( \frac{2}{3}\right) }^{n} + \cdots }\right\rbrack   = 1
$$

所以 $C \cdot  \frac{\frac{2}{3}}{1 - \frac{2}{3}} = 1,\;C = \frac{1}{2}$

所以当 $C = \frac{1}{2}$ 时, $P\{ X = k\}  = C \cdot  {\left( \frac{2}{3}\right) }^{k}$ 才能成为随机变量的分布列.

【2.2】设随机变量 $X$ 的可能取值为-1,0,1,且取这三个值的概率之比为 $1 : 2 : 3$,则 $X$ 的概率分布为_____.

解 记 $X \sim  \left\lbrack  \begin{matrix}  - 1 & 0 & 1 \\  {p}_{1} & {p}_{2} & {p}_{3} \end{matrix}\right\rbrack$,依题意 ${p}_{1} : {p}_{2} : {p}_{3} = 1 : 2 : 3$ 而

$$
{p}_{1} + {p}_{2} + {p}_{3} = 1\;\text{ 即 }{p}_{1} + 2{p}_{1} + 3{p}_{1} = 1
$$

故

$$
{p}_{1} = \frac{1}{6},\;{p}_{2} = \frac{1}{3},\;{p}_{3} = \frac{1}{2}
$$

$$
X \sim  \left\lbrack  \begin{matrix}  - 1 & 0 & 1 \\  \frac{1}{6} & \frac{1}{3} & \frac{1}{2} \end{matrix}\right\rbrack
$$

#### 题型2: 求离散型随机变量的分布律

方法与技巧

求离散型随机变量的分布律, 先要搞清楚其所有可能的取值. 然后计算随机变量取各相应值的概率. 计算应结合求随机事件概率的各种方法和概率基本公式.

【2.3】一袋中有 5 只球,编号为 1,2,3,4,5,在袋中同时取 3 只,以 $X$ 表示取出的 3 只球中的最大号码,写出随机变量 $X$ 的分布律.

解 从 5 只球中任取 3 只,有 ${C}_{5}^{3} = {10}$ 种取法,每种取法的概率为 $\frac{1}{10}$. 随机变量的可能值为 3,4,5.

当 $X = 3$ 时,相当于取出 3 只球的号码为: $\{ 1,2,3\}$,故

$$
P\{ X = 3\}  = \frac{1}{10},
$$

类似地

$$
P\{ X = 4\}  = \frac{3}{10};\;P\{ X = 5\}  = \frac{6}{10},
$$

所以 $X$ 的分布律为

<table><tr><td>$X$</td><td>3</td><td>4</td><td>5</td></tr><tr><td>$P$</td><td>$\frac{1}{10}$</td><td>$\frac{3}{10}$</td><td>$\frac{6}{10}$</td></tr></table>

【2.4】一辆汽车沿一街道行驶,需要通过三个均设有红绿信号灯的路口,每个信号灯为红或绿与其他信号灯为红或绿相互独立,且红绿两种信号显示时间相等. 以 $X$ 表示该汽车首次遇到红灯前已通过的路口的个数,求 $X$ 的概率分布.

分析 $X$ 为离散型随机变量,其全部可能取值是0,1,2,3,再通过概率计算公式求得.

解 设 ${A}_{i}$ 为汽车在第 $i$ 个路口遇到红灯, $i = 1,2,3$. 因为 ${A}_{1},{A}_{2},{A}_{3}$,相互独立,所以

$$
P\{ X = 0\}  = P\left( {A}_{1}\right)  = \frac{1}{2}
$$

$$
P\{ X = 1\}  = P\left( {{\bar{A}}_{1}{A}_{2}}\right)  = P\left( {\bar{A}}_{1}\right) P\left( {A}_{2}\right)  = \frac{1}{2} \times  \frac{1}{2} = \frac{1}{{2}^{2}}
$$

$$
P\{ X = 2\}  = P\left( {{\bar{A}}_{1}{\bar{A}}_{2}{A}_{3}}\right)  = P\left( {\bar{A}}_{1}\right) P\left( {\bar{A}}_{2}\right) P\left( {A}_{3}\right)  = \frac{1}{2} \times  \frac{1}{2} \times  \frac{1}{2} = \frac{1}{{2}^{3}}
$$

$$
P\{ X = 3\}  = P\left( {{\bar{A}}_{1}{\bar{A}}_{2}{\bar{A}}_{3}}\right)  = P\left( {\bar{A}}_{1}\right) P\left( {\bar{A}}_{2}\right) P\left( {\bar{A}}_{3}\right)  = \frac{1}{2} \times  \frac{1}{2} \times  \frac{1}{2} = \frac{1}{{2}^{3}}.
$$

所以 $X$ 的分布律为

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>$\frac{1}{2}$</td><td>$\frac{1}{4}$</td><td>$\frac{1}{8}$</td><td>$\frac{1}{8}$</td></tr></table>

#### 题型 3:离散型随机变量的分布律与分布函数的关系

【2.5】设一盒子内有 5 个小球, 2 个白的和 3 个黑的,如果从中任取 2 个,那么取到黑球数的分布函数是多少?

分析 对于未知概率分布的随机变量要求其分布函数的问题, 需先求出该随机变量的分布律.

解 令 $X$ 表示取到黑球的个数,因为 $X$ 为离散型随机变量,其全部可能取值为0,1,2,所以其分布律为

$$
P\{ X = k\}  = \frac{{C}_{3}^{k}{C}_{2}^{2 - k}}{{C}_{5}^{2}}\;\left( {k = 0,1,2}\right)
$$

得 $P\{ X = 0\}  = {0.1},\;P\{ X = 1\}  = {0.6},\;P\{ X = 2\}  = {0.3}$

由 $X$ 的分布函数为

$$
F\left( x\right)  = P\{ X \leq  x\}  = \mathop{\sum }\limits_{{k \leq  x}}{p}_{k}
$$

得 $F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0 \\  {0.1}, & 0 \leq  x < 1 \\  {0.7}, & 1 \leq  x < 2 \\  1, & x \geq  2 \end{array}\right.$

点评 在求解离散型随机变量的分布函数时, 先通过概率公式求得分布律, 再应用

$$
F\left( x\right)  = P\{ X \leq  x\}  = \mathop{\sum }\limits_{{{x}_{k} \leq  x}}{p}_{k}
$$

这一公式, 这是最基本的方法. 【2.6】设随机变量的分布函数为

$$
F\left( x\right)  = P\{ X \leq  x\}  = \left\{  \begin{array}{ll} 0, & \text{ 若 }x <  - 1 \\  {0.4}, & \text{ 若 } - 1 \leq  x < 1 \\  {0.8}, & \text{ 若 }1 \leq  x < 3 \\  1, & \text{ 若 }x \geq  3. \end{array}\right.
$$

则 $X$ 的概率分布为____

解 方法一:作图法根据题意作出 $X$ 的分布函数 $F\left( x\right)$ 的图像(如图 2-2.6). 因为离散型随机变量的分布函数为阶梯型而且随机变量在间断点处取值概率不为零而是

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_41_996_1319_331_211_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_41_996_1319_331_211_0.jpg)

图 2-2.6


跳跃幅度大小, 所以易得到

$$
P\{ X =  - 1\}  = {0.4},\;P\{ X = 1\}  = {0.4},\;P\{ X = 3\}  = {0.2}.
$$

方法二:公式法

由 $P\{ X = x\}  = P\{ X \leq  x\}  - P\{ X < x\}  = F\left( x\right)  - F\left( {x - 0}\right)$

则 $P\{ X =  - 1\}  = F\left( {-1}\right)  - F\left( {-1 - 0}\right)  = {0.4}$

$$
P\{ X = 1\}  = F\left( 1\right)  - F\left( {1 - 0}\right)  = {0.8} - {0.4} = {0.4}
$$

$P\{ X = 3\}  = F\left( 3\right)  - F\left( {3 - 0}\right)  = 1 - {0.8} = {0.2}.$

点评 利用分布函数求解离散型随机变量的概率分布一般采用作图法或公式法.

离散型随机变量的统计规律一般用分布律来描述, 离散型随机变量的分布函数是阶梯函数, 也是研究随机变量的统计规律的重要工具, 但不如分布律直观简单.

【2.7】设随机变量 $X$ 的分布律为分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} c, & x <  - 1 \\  d, &  - 1 \leq  x < 0 \\  \frac{3}{4}, & 0 \leq  x < 1 \\  e, & x \geq  1 \end{array}\right.
$$

<table><tr><td>$X$</td><td>-1</td><td>0</td><td>1</td></tr><tr><td>$P$</td><td>$\frac{1}{4}$</td><td>$a$</td><td>$b$</td></tr></table>

求 $a, b, c, d, e$.

解 由分布函数性质:

$F\left( {-\infty }\right)  = 0$ 可知 $c = 0$,

$F\left( {+\infty }\right)  = 1$ 可知 $e = 1$,

由分布律与分布函数的关系

$$
F\left( {-1}\right)  = P\{ X \leq   - 1\}  = P\{ X =  - 1\}  = \frac{1}{4},
$$

可知 $d = \frac{1}{4}$.

$$
F\left( 0\right)  = P\{ X \leq  0\}  = P\{ X =  - 1\}  + P\{ X = 0\}  = \frac{1}{4} + a = \frac{3}{4},
$$

可知 $a = \frac{1}{2}$,

由分布律的性质 $\frac{1}{4} + a + b = 1$,可得 $b = \frac{1}{4}$.

#### 题型 4 : 利用分布律求概率

【2.8】已知离散型随机变量 $X$ 的可能取值为 $- 2,0,2,\sqrt{5}$,相应的概率依次为 $\frac{1}{a},\frac{3}{2a},\frac{5}{4a}$, $\frac{7}{8a}$,则 $P\{ \left| X\right|  \leq  2 \mid  X \geq  0\}$ 为(   ).

(A) $\frac{21}{29}$ (B) $\frac{22}{29}$ (C) $\frac{2}{3}$ (D) $\frac{1}{3}$

解 首先根据概率分布的性质求出常数 $a$ 的值,其次确定概率分布的具体形式,然后计算条件概率

$$
\mathop{\sum }\limits_{{i = 1}}^{4}P\left\{  {X = {x}_{i}}\right\}   = \frac{1}{a} + \frac{3}{2a} + \frac{5}{4a} + \frac{7}{8a} = \frac{37}{8a} = 1
$$

解得 $a = \frac{37}{8}$,故

$X \sim  \left\lbrack  \begin{matrix}  - 2 & 0 & 2 & \sqrt{5} \\  \frac{8}{37} & \frac{12}{37} & \frac{10}{37} & \frac{7}{37} \end{matrix}\right\rbrack$

$P\{ \left| X\right|  \leq  2 \mid  X \geq  0\}  = \frac{P\{ \left| X\right|  \leq  2, X \geq  0\} }{P\{ X \geq  0\} } = \frac{P\{ X = 0\}  + P\{ X = 2\} }{P\{ X = 0\}  + P\{ X = 2\}  + P\{ X = \sqrt{5}\} }$

$= \frac{22}{29}$

故应选 (B).

【2.9】设随机变量的分布律为 $P\{ X = k\}  = \frac{1}{{2}^{k}}, k = 1,2,\cdots$,则 $P\{ X =$ 偶数 $\}  =$ _____, $P\{ X \geq  5\}  =$ _____.

解 $P\{ X =$ 偶数 $\}  = \mathop{\sum }\limits_{{k = 1}}^{\infty }P\{ X = {2k}\}  = \mathop{\sum }\limits_{{k = 1}}^{\infty }\frac{1}{{2}^{2k}} = \frac{\frac{1}{4}}{1 - \frac{1}{4}} = \frac{1}{3}$.

$P\{ X \geq  5\}  = \mathop{\sum }\limits_{{k = 5}}^{\infty }P\{ X = k\}  = \mathop{\sum }\limits_{{k = 5}}^{\infty }\frac{1}{{2}^{k}} = \frac{\frac{1}{{2}^{5}}}{1 - \frac{1}{2}} = \frac{1}{16}.$

故应填 $\frac{1}{3};\frac{1}{16}$.

#### 题型 5: 关于常见分布

【2.10】设随机变量 $X$ 服从参数为 $\left( {2, p}\right)$ 的二项分布,随机变量 $Y$ 服从参数为 $\left( {3, p}\right)$ 的二项分布,若 $P\{ X \geq  1\}  = \frac{5}{9}$,则 $P\{ Y \geq  1\}  =$ _____.

解 $\frac{5}{9} = P\{ X \geq  1\}  = 1 - P\{ X < 1\}  = 1 - {C}_{2}^{0}{p}^{0}{\left( 1 - p\right) }^{2} = 1 - {\left( 1 - p\right) }^{2}$

得 $\;\left( {1 - p}\right)  = \frac{2}{3}$

则 $P\{ Y \geq  1\}  = 1 - P\{ Y < 1\}  = 1 - {C}_{3}^{0}{p}^{0}{\left( 1 - p\right) }^{3} = 1 - {\left( \frac{2}{3}\right) }^{3} = \frac{19}{27}$

故应填 $\frac{19}{27}$.

【2.11】随机变量 $X$ 服从泊松分布,并且已知 $P\{ X = 1\}  = P\{ X = 2\}$,则 $P\{ X = 4\}  =$ _____.

解 由题设, $X$ 的分布律为:

$$
P\{ X = k\}  = \frac{{\lambda }^{k}}{k!}{\mathrm{e}}^{-\lambda },\;k = 0,1,2,\cdots
$$

本题的关键为先要求出参数 $\lambda$ 的值. 由 $P\{ X = 1\}  = P\{ X = 2\}$ 得

$$
\lambda {\mathrm{e}}^{-\lambda } = \frac{{\lambda }^{2}}{2}{\mathrm{e}}^{-\lambda }\;\text{ 即 }{\lambda }^{2} - {2\lambda } = 0.
$$

因为 $\lambda  > 0$,得 $\lambda  = 2$. 于是

$$
P\{ X = 4\}  = \frac{{2}^{4}}{4!}{\mathrm{e}}^{-2} = \frac{2}{3}{\mathrm{e}}^{-2} \approx  {0.0902}.
$$

故应填 $\frac{2}{3}{\mathrm{e}}^{-2}$.

【2.12】设某批电子元件的正品率为 $\frac{4}{5}$,次品率为 $\frac{1}{5}$,现对这批元件进行测试,只要测得一个正品就停止测试工作,则测试次数的分布律是_____.

解 设测试次数为 $X$,则 $X$ 的可能值为 $1,2,3,\cdots$. 当 $X = k$ 时,相当于“前 $k - 1$ 次测到的都是次品,而第 $k$ 次测到的是正品”,故

$$
P\{ X = k\}  = {\left( \frac{1}{5}\right) }^{k - 1}\left( \frac{4}{5}\right) \;\left( {k = 1,2,\cdots }\right)
$$

点评 本题中 $X$ 服从几何分布,几何分布的实际背景是重复独立试验下首次成功的概率, 它可作为描述“独立射击,首次击中时的射击次数”；“有放回地抽取产品,首次抽到次品时的抽取次数” 等概率分布的数学模型.

【2.13】有一批产品共 20 件,其中次品 3 件. 现从中任取 4 件(不放回抽样),求其中次品数 $X$ 的分布律; 其中次品数不多于 2 件的概率有多大?

解 共有 20 个元素, 分为两类 (次品与正品), 其中第一类元素 (次品) 有 3 个. 现从中任取 4 个元素,则其中第一类元素数 $X$ 为服从超几何分布的随机变量. 故 $X$ 的分布律为:

$$
P\{ X = k\}  = \frac{{C}_{3}^{k}{C}_{17}^{4 - k}}{{C}_{20}^{4}}\;k = 0,1,2,3
$$

用表格可表示为

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>${p}_{k}$</td><td>$\frac{28}{57}$</td><td>$\frac{8}{19}$</td><td>$\frac{8}{95}$</td><td>$\frac{1}{285}$</td></tr></table>

其中次品数不多于 2 件的概率为

$$
P\{ X \leq  2\}  = P\{ X = 0\}  + P\{ X = 1\}  + P\{ X = 2\}  \approx  {0.996}.
$$

点评 可以证明,当 $N \rightarrow   + \infty$ 时,超几何分布以二项分布为极限,即当 $N$ 充分大, $n$ 相对较小时, $X$ 近似服从 $B\left( {n,\frac{M}{N}}\right)$.

【2.14】一电话交换台每分钟收到呼唤的次数服从参数为 4 的泊松分布,求

(1)某一分钟恰有 8 次呼唤的概率；

(2)某一分钟的呼唤次数大于 3 的概率.

解 用 $X$ 表示每分钟收到呼唤的次数. 则

$$
P\{ X = k\}  = \frac{{4}^{k}}{k!}{\mathrm{e}}^{-4},\;k = 0,1,2,\cdots
$$

(1) $P\{ X = 8\}  = \frac{{4}^{8}}{8!}{\mathrm{e}}^{-4} = {0.0298}$

(2) $P\{ X > 3\}  = \mathop{\sum }\limits_{{k = 4}}^{\infty }\frac{{4}^{k}}{k!}{\mathrm{e}}^{-4} = {0.5665}$

【2.15】一大楼装有 5 个同类型的供水设备,调查表明在任一时刻 $t$ 每个设备被使用的概率

为 0.1, 问在同一时刻:

(1)恰有 2 个设备被使用的概率是多少?

(2)至少有 3 个设备被使用的概率是多少？

(3)至多有 3 个设备被使用的概率是多少？

(4)至少有 1 个设备被使用的概率是多少?

解 设被使用的设备数为 $X$,则 $X \sim  B\left( {5,{0.1}}\right)$,故

(1) $P\{ X = 2\}  = {C}_{5}^{2}{\left( {0.1}\right) }^{2}{\left( {0.9}\right) }^{3} = {0.0729}$

(2) $P\{ X \geq  3\}  = \mathop{\sum }\limits_{{k = 3}}^{5}{C}_{5}^{k}{\left( {0.1}\right) }^{k}{\left( {0.9}\right) }^{5 - k} = {0.00856}$

(3) $P\{ X \leq  3\}  = \mathop{\sum }\limits_{{k = 0}}^{3}{C}_{5}^{k}{\left( {0.1}\right) }^{k}{\left( {0.9}\right) }^{5 - k} = {0.99954}$

(4) $P\{ X \geq  1\}  = 1 - {C}_{5}^{0}{\left( {0.1}\right) }^{0}{\left( {0.9}\right) }^{5} = 1 - {\left( {0.9}\right) }^{5} = {0.40951}$

【2.16】有甲、乙两种味道和颜色都极为相似的名酒各 4 杯. 如果从中挑 4 杯,能将甲种酒全部挑出来, 算是试验成功一次.

(1)某人随机地去猜,问他试验成功一次的概率是多少？

(2)某人声称他通过品尝能区分两种酒. 他连续试验 10 次,成功 3 次. 试推断他是猜对的,还是确有区分的能力 (设各次试验是相互独立的).

解 (1)随机试验是从 8 杯酒中任选 4 杯,从而样本空间的样本点数总数为 ${C}_{8}^{4}$,故试验成功一次的概率为 $p = \frac{1}{{C}_{8}^{4}} = \frac{1}{70}$.

(2)连续试验 10 次,成功 3 次,如果他是猜对的,则猜对的次数 $X \sim  B\left( {{10},\frac{1}{70}}\right)$,猜对 3 次的概率为

$$
P\{ X = 3\}  = {C}_{10}^{3}{\left( \frac{1}{70}\right) }^{3}{\left( \frac{69}{70}\right) }^{7} \approx  \frac{{\left( \frac{1}{7}\right) }^{3}}{3!}{\mathrm{e}}^{-\frac{1}{7}} \approx  3 \times  {10}^{-4},
$$

这个概率很小, 根据实际推断原理, 可以认为他确有区分能力.

#### 题型 6: 关于泊松定理

【2.17】现有同型设备 300 台, 各台设备的工作是相互独立的, 发生故障的概率都是 0.01. 设一台设备的故障可由一名维修工人处理,问至少需配备多少名维修工人,才能保证设备发生故障但不能及时维修的概率小于 0.01 ?

解 设需配备 $N$ 名工人, $X$ 为同一时刻发生故障的设备的台数,则 $X \sim  B\left( {{300},{0.01}}\right)$. 所需解决的问题是确定 $N$ 最小值,使 $P\{ X \leq  N\}  \geq  {0.99}$. 电 46

因 ${np} = \lambda  = 3$,由泊松定理

$$
P\{ X \leq  N\}  \approx  \mathop{\sum }\limits_{{k = 0}}^{N}\frac{{3}^{k}}{k!}{\mathrm{e}}^{-3},
$$

故问题转化为求 $N$ 的最小值,使 $\mathop{\sum }\limits_{{k = 0}}^{N}\frac{{3}^{k}}{k!}{\mathrm{e}}^{-3} \geq  {0.99}$,即

$$
1 - \mathop{\sum }\limits_{{k = 0}}^{N}\frac{{3}^{k}}{k!}{\mathrm{e}}^{-3} = \mathop{\sum }\limits_{{k = N + 1}}^{{+\infty }}\frac{{3}^{k}}{k!}{\mathrm{e}}^{-3} \leq  {0.01}
$$

查表可知,当 $N \geq  8$ 时,上式成立. 因此,为达到上述要求,至少需配备 8 名维修工人.

点评 利用二项分布求概率时, 如果遇到多个概率的和式不易求, 可以运用泊松定理或后面的中心极限定理求其近似值. 本题就是如此,设 $X \sim  B\left( {n, p}\right)$,当 $n$ 较大, $p$ 较小时, $X$ 近似服从 $P\left( {np}\right)$.

## $§3$. 连续型随机变量及其分布

### 知识要点

#### 1. 连续型随机变量的概率密度

如果对于随机变量 $X$ 的分布函数 $F\left( x\right)$,存在非负可积函数 $f\left( x\right)$,使得对任意实数 $x$,有 $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t$ 成立,则称 $X$ 为连续型随机变量,函数 $f\left( x\right)$ 称为 $X$ 的概率密度 (或分布密度).

#### 2. 连续型随机变量的概率密度函数 $f\left( x\right)$ 的性质

(1) $f\left( x\right)  \geq  0$;

(2) ${\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = 1$.

#### 3. 连续型随机变量的概率密度与分布函数以及事件概率的关系

( 1 )若 $X$ 的概率密度为 $f\left( x\right)$,则 $X$ 的分布函数为 $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t$,当 $f\left( x\right)$ 为分段函数时其分布函数 $F\left( x\right)$ 要做分段讨论;

(2)若 $f\left( x\right)$ 在点 $x$ 处连续,则有 ${F}^{\prime }\left( x\right)  = f\left( x\right)$;

(3) $P\{ a < X \leq  b\}  = P\{ a < X < b\}  = P\{ a \leq  X < b\}  = P\{ a \leq  X \leq  b\}$

$$
= F\left( b\right)  - F\left( a\right)  = {\int }_{a}^{b}f\left( x\right) \mathrm{d}x;
$$

(4) $P\{ X = a\}  = 0\left( {-\infty  < a <  + \infty }\right)$.

#### 4. 重要分布

(1)均匀分布:若连续型随机变量 $X$ 的概率密度函数为

$$
f\left( x\right)  = \left\{  {\begin{matrix} \frac{1}{b - a}, & a \leq  x \leq  b \\  0, & \text{ 其他 } \end{matrix}\;\left( {\text{ 如图 }2 - 3 - 1}\right) }\right.
$$

则称 $X$ 服从 $\left\lbrack  {a, b}\right\rbrack$ 上的均匀分布.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_453_181_315_197_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_453_181_315_197_0.jpg)

图 2-3-1

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_962_188_239_192_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_962_188_239_192_0.jpg)

图 $2 - 3 - 2$

(2)指数分布:若连续型随机变量 $X$ 的概率密度函数为

$$
f\left( x\right)  = \left\{  {\begin{array}{ll} \lambda {\mathrm{e}}^{-{\lambda x}}, & x > 0 \\  0, & \text{ 其他 } \end{array}\;\text{ (如图 }2 - 3 - 2\text{ ) }}\right.
$$

其中 $\lambda  > 0$,则称 $X$ 服从参数为 $\lambda$ 的指数分布.

(3)正态分布:若连续型随机变量 $X$ 的概率密度函数为

$$
f\left( x\right)  = \frac{1}{\sqrt{2\pi }\sigma }{\mathrm{e}}^{\frac{{\left( x - \mu \right) }^{2}}{2{\sigma }^{2}}}\;\left( {-\infty  < x <  + \infty }\right) \;\text{(如图 2-3-3)}
$$

其中 $\mu$ 与 $\sigma  > 0$ 都是常数,则称 $X$ 服从参数为 $\mu$ 和 $\sigma$ 的正态分布. 简记为 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_459_792_315_218_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_459_792_315_218_0.jpg)

图 2-3-3

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_854_781_376_233_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_47_854_781_376_233_0.jpg)

图 2-3-4

(4)标准正态分布: 当 $\mu  = 0,\sigma  = 1$ 时称 $X$ 服从标准正态分布,简记为 $X \sim  N\left( {0,1}\right)$,其概率密度函数和分布函数分别用 $\varphi \left( x\right),\Phi \left( x\right)$ 表示,即有

$$
\varphi \left( x\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\;\text{ (如图 2-3-4) }
$$

$$
\Phi \left( x\right)  = \frac{1}{\sqrt{2\pi }}{\int }_{-\infty }^{x}{\mathrm{e}}^{-\frac{{t}^{2}}{2}}\mathrm{\;d}t
$$

性质 ${1\Phi }\left( {-x}\right)  = 1 - \Phi \left( x\right)$

性质 2 当 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$ 时, $U = \frac{X - \mu }{\sigma } \sim  N\left( {0,1}\right)$. 即 $F\left( x\right)  = \Phi \left( \frac{x - \mu }{\sigma }\right)$.

### 基本题型

#### 题型 1: 概率密度的性质

【3.1】下列选项中,能作为连续型随机变量密度函数的是(   ). 中 48

(A) $f\left( x\right)  = \left\{  \begin{matrix} \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}, & x > 0 \\  0, & x \leq  0 \end{matrix}\right.$ (B) $f\left( x\right)  = \left\{  \begin{array}{ll} 1, & \left| x\right|  < 1 \\  0, & \text{ 其他 } \end{array}\right.$

(C) $f\left( x\right)  = \left\{  \begin{array}{ll} \frac{x}{2}, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right.$ (D) $f\left( x\right)  = \frac{1}{2}{\mathrm{e}}^{-\left| x\right| }$

解 只有 (D) 中 $f\left( x\right)$ 满足概率密度的性质:

(1) $f\left( x\right)  \geq  0$; (2) ${\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = 1$.

故应选(D).

【3.2】 $f\left( x\right)  = c{\mathrm{e}}^{-{x}^{2} + x}$ 是随机变量 $X$ 的密度函数,则 $c =$ _____.

解 ${\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = \frac{c}{\sqrt{2}}{\mathrm{e}}^{\frac{1}{4}}{\int }_{-\infty }^{+\infty }{\mathrm{e}}^{-\frac{{t}^{2}}{2}}\mathrm{\;d}t = c \cdot  \sqrt{\pi }{\mathrm{e}}^{\frac{1}{4}} = 1$.

故 $c = \frac{1}{\sqrt{\pi }}{\mathrm{e}}^{-\frac{1}{4}}$.

【3.3】设随机变量 $X$ 的密度函数为 $\varphi \left( x\right)$,且 $\varphi \left( {-x}\right)  = \varphi \left( x\right), F\left( x\right)$ 是 $X$ 的分布函数,则对任意实数 $a$,有(   ).

(A) $F\left( {-a}\right)  = 1 - {\int }_{0}^{a}\varphi \left( x\right) \mathrm{d}x$ (B) $F\left( {-a}\right)  = \frac{1}{2} - {\int }_{0}^{a}\varphi \left( x\right) \mathrm{d}x$

(C) $F\left( {-a}\right)  = F\left( a\right)$ (D) $F\left( {-a}\right)  = {2F}\left( a\right)  - 1$

分析 在对随机变量求密度函数与分布函数问题中多用到高等数学中微积分方面的知识, 本题中需要对积分变量做换元法。

解 由分布函数与密度函数关系可知 $F\left( {-a}\right)  = {\int }_{-\infty }^{-a}\varphi \left( x\right) \mathrm{d}x$.

令 $x =  - t$,得到 $F\left( {-a}\right)  =  - {\int }_{+\infty }^{a}\varphi \left( t\right) \mathrm{d}t = {\int }_{a}^{+\infty }\varphi \left( x\right) \mathrm{d}x$

又因为 ${\int }_{-\infty }^{+\infty }\varphi \left( x\right) \mathrm{d}x = 1$,且有 $\varphi \left( {-x}\right)  = \varphi \left( x\right)$

故 ${\int }_{-\infty }^{-a}\varphi \left( x\right) \mathrm{d}x + {\int }_{-a}^{0}\varphi \left( x\right) \mathrm{d}x = {\int }_{0}^{a}\varphi \left( x\right) \mathrm{d}x + {\int }_{a}^{\infty }\varphi \left( x\right) \mathrm{d}x = \frac{1}{2}{\int }_{-\infty }^{+\infty }\varphi \left( x\right) \mathrm{d}x = \frac{1}{2}$

得 ${\int }_{0}^{a}\varphi \left( x\right) \mathrm{d}x + F\left( {-a}\right)  = \frac{1}{2}$

所以 $F\left( {-a}\right)  = \frac{1}{2} - {\int }_{0}^{a}\varphi \left( x\right) \mathrm{d}x$.

答案为(B)

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_48_939_1395_374_210_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_48_939_1395_374_210_0.jpg)

图 2-3.3

点评 另外还可以根据随机变量 $X$ 的密度函数图形来判定.

由于密度函数 $\varphi \left( x\right)$ 满足 $\varphi \left( x\right)  = \varphi \left( {-x}\right)$ 是关于 $y$ 轴对称的,如图 2-3.3 所示. ${S}_{1},{D}_{1},{D}_{2},{S}_{2}$ 表示图中对应部分的面积. 根据密度函数的性质及 $\varphi \left( {-x}\right)  = \varphi \left( x\right)$ 知

$$
{S}_{1} = {S}_{2},\;{D}_{1} = {D}_{2},\;{S}_{1} + {D}_{1} = {D}_{2} + {S}_{2} = \frac{1}{2}
$$

因此 $F\left( {-a}\right)  = {S}_{1} = {S}_{2} = \frac{1}{2} - {D}_{2} = \frac{1}{2} - {\int }_{0}^{a}\varphi \left( x\right) \mathrm{d}x$

故应选(B).

题型2: 概率密度与分布函数的转化以及求概率

【3.4】设连续型随机变量 $X$ 的分布函数为

$$
F\left( x\right)  = \left\{  \begin{matrix} 0, & x < 0 \\  A{x}^{2} & 0 \leq  x < 1 \\  1, & x \geq  1 \end{matrix}\right.
$$

求 (1) 常数 $A$; $\left( 2\right) X$ 落在 $\left( {-1,\frac{1}{2}}\right)$ 及 $\left( {\frac{1}{3},2}\right)$ 内的概率； ( 3 ) $X$ 的概率密度.

分析 求解分布函数未知参数时要用到分布函数的性质. 由已知分布函数来求概率密度时要对分布函数求导, 其中若分布函数为分段函数, 概率密度也要分区间考虑.

解 (1) 由 $F\left( x\right)$ 的连续性,可知

$$
\mathop{\lim }\limits_{{x \rightarrow  {1}^{ - }}}F\left( x\right)  = F\left( 1\right) \text{,则}\mathop{\lim }\limits_{{x \rightarrow  {1}^{ - }}}A{x}^{2} = 1\text{,可得}A = 1\text{,}
$$

那么分布函数 $F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0 \\  {x}^{2} & 0 \leq  x < 1 \\  1, & x \geq  1 \end{array}\right.$

(2)由于 $X$ 落在 $\left( {-1,\frac{1}{2}}\right)$ 内,则

$$
P\left\{  {-1 < X < \frac{1}{2}}\right\}   = F\left( \frac{1}{2}\right)  - F\left( {-1}\right)  = {\left( \frac{1}{2}\right) }^{2} - 0 = \frac{1}{4}
$$

同理可知

$$
P\left\{  {\frac{1}{3} < X < 2}\right\}   = F\left( 2\right)  - F\left( \frac{1}{3}\right)  = 1 - {\left( \frac{1}{3}\right) }^{2} = \frac{8}{9}.
$$

(3) 因为 $f\left( x\right)  = {F}^{\prime }\left( x\right)$

当 $0 \leq  x < 1$ 时, $f\left( x\right)  = {\left( {x}^{2}\right) }^{\prime } = {2x}$; 其他情况时, $f\left( x\right)  = 0$.

所以 $f\left( x\right)  = \left\{  \begin{array}{ll} {2x}, & 0 \leq  x < 1 \\  0, & \text{ 其他 } \end{array}\right.$

【3.5】设随机变量 $X$ 的概率密度 $f\left( x\right)$ 满足 $f\left( {1 + x}\right)  = f\left( {1 - x}\right)$,且 ${\int }_{0}^{2}f\left( x\right) \mathrm{d}x = {0.6}$,则 $P\{ X < 0\}  =$ (   )

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_49_944_1399_382_225_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_49_944_1399_382_225_0.jpg)

图 2-3.5

(A)0.2. (B) 0.3.

(C) 0.4. (D) 0.5.

解 本题中的概率密度是抽象的, 只给出了一个已知积分, 如果用常规的积分方法求概率较为繁琐, 而利用概率密度的几何意义结合图形求概率非常简便.

已知 $f\left( {1 + x}\right)  = f\left( {1 - x}\right)$,可得 $f\left( x\right)$

关于 $x = 1$ 对称,如图 2-3.5

由 ${\int }_{0}^{2}f\left( x\right) \mathrm{d}x = {0.6}$,可知 $P\{ X < 0\}  = {0.2}$.

【3.6】设随机变量 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{matrix} {kx} + 1, & 0 \leq  x < 2 \\  0, & \text{ 其他 } \end{matrix}\right.
$$

求 (1)k 值;

(2) $X$ 的分布函数；

(3) $P\{ 1 < X < 2\}$.

解 (1)由概率密度性质 ${\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = {\int }_{0}^{2}\left( {{kx} + 1}\right) \mathrm{d}x = {2k} + 2 = 1$,得 $k =  - \frac{1}{2}$;

(2)因为 $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t$,所以当 $x < 0$ 时, $F\left( x\right)  = {\int }_{-\infty }^{x}0\mathrm{\;d}t = 0$;

当 $0 \leq  x < 2$ 时, $F\left( x\right)  = {\int }_{-\infty }^{0}0\mathrm{\;d}t + {\int }_{0}^{x}\left( {-\frac{1}{2}t + 1}\right) \mathrm{d}t =  - \frac{1}{4}{x}^{2} + x$;

当 $x \geq  2$ 时, $F\left( x\right)  = {\int }_{-\infty }^{0}0\mathrm{\;d}t + {\int }_{0}^{2}\left( {-\frac{1}{2}t + 1}\right) \mathrm{d}t + {\int }_{2}^{x}0\mathrm{\;d}t = 1$.

故 $X$ 的分布函数

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0 \\   - \frac{1}{4}{x}^{2} + x, & 0 \leq  x < 2 \\  1, & x \geq  2 \end{array}\right.
$$

(3) $P\{ 1 < X < 2\}  = {\int }_{1}^{2}\left( {-\frac{1}{2}x + 1}\right) \mathrm{d}x = \frac{1}{4}$.

点评 本题也可以用分布函数 $F\left( x\right)$ 求概率 $P\{ 1 < X < 2\}  = F\left( 2\right)  - F\left( 1\right)  = \frac{1}{4}$.

【3.7】设随机变量 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{3}, & \text{ 若 }x \in  \left\lbrack  {0,1}\right\rbrack  \\  \frac{2}{9}, & \text{ 若 }x \in  \left\lbrack  {3,6}\right\rbrack  \\  0, & \text{ 其他 } \end{array}\right.
$$

若 $k$ 使得 $P\{ X \geq  k\}  = \frac{2}{3}$,则 $k$ 的取值范围是_____.

分析 本题中 $f\left( x\right)$ 是分段函数,要求 $k$ 的取值范围,对于 $k$ 要分段来讨论,再由已知条件为限制得到 $k$ 的取值范围.

解 当 $k < 1$ 时, $P\{ X \geq  k\}  > P\{ X \geq  1\}$,因为 $P\{ X \geq  1\}  = \frac{2}{9} \times  \left( {6 - 3}\right)  = \frac{2}{3}$,所以 $P\{ X \geq  k\}  > \frac{2}{3}$;

当 $k > 3$ 时, $P\{ X \geq  k\}  < P\{ X \geq  3\}$,因为 $P\{ X \geq  3\}  = \frac{2}{9} \times  \left( {6 - 3}\right)  = \frac{2}{3}$,所以概率论与数理统计习题精选精解

$P\{ X \geq  k\}  < \frac{2}{3}$

当 $1 \leq  k \leq  3$ 时, $P\{ X \geq  k\}  = P\{ k \leq  X < 3\}  + P\{ X \geq  3\}  = \frac{2}{3}$,所以 $k$ 的取值范围为 $\lbrack 1$,

3].

【3.8】某种型号的电子管其寿命 (以小时计) 为一随机变量. 概率密度函数是

$$
\varphi \left( x\right)  = \left\{  \begin{matrix} \frac{100}{{x}^{2}}, & x \geq  {100} \\  0, & \text{ 其他 } \end{matrix}\right.
$$

某一无线电器材配有三个这种电子管, 求使用 150 小时内不需要更换的概率.

解 每个电子管寿命在 $X \leq  {150}$ 的概率

$$
P\{ X \leq  {150}\}  = {\int }_{100}^{150}\frac{100}{{x}^{2}}\mathrm{\;d}x =  - {\left. \frac{100}{x}\right| }_{100}^{150} = \frac{1}{3}.
$$

每个电子管寿命在 $X > {150}$ 的概率

$$
P\{ X > {150}\}  = 1 - \frac{1}{3} = \frac{2}{3}
$$

某一无线电器材配有三个这种电子管, 150 小时内不需要更换, 即三个电子管的寿命都在 150 小时以外. 所以不需要更换的概率

$$
p = {\left( \frac{2}{3}\right) }^{3} = \frac{8}{27} = {0.296}.
$$

#### 题型 3: 关于重要分布

【3.9】设 $X \sim  N\left( {3,{2}^{2}}\right),\left( 1\right)$ 求 $P\{ 2 < X \leq  5\}, P\{  - 4 < X \leq  {10}\}, P\{ \left| X\right|  > 2\}, P\{ X >$ 3\};

(2)确定 $c$ 使得 $P\{ X > c\}  = P\{ X \leq  c\}$;

(3)设 $d$ 满足 $P\{ X > d\}  \geq  {0.9}$,问 $d$ 至多为多少？

解 当 $X \sim  N\left( {3,{2}^{2}}\right)$ 时,

$$
\frac{X - \mu }{\sigma } = \frac{X - 3}{2} \sim  N\left( {0,1}\right).
$$

(1) $P\{ 2 < X \leq  5\}  = P\left\{  {\frac{2 - 3}{2} < \frac{X - 3}{2} \leq  \frac{5 - 3}{2}}\right\}   = \Phi \left( 1\right)  - \Phi \left( {-\frac{1}{2}}\right)$

$$
= \Phi \left( 1\right)  - \left( {1 - \Phi \left( \frac{1}{2}\right) }\right)  = {0.8413} - 1 + {0.6915} = {0.5328}
$$

$$
P\{  - 4 < X \leq  {10}\}  = P\left\{  {\frac{-4 - 3}{2} < \frac{X - 3}{2} \leq  \frac{{10} - 3}{2}}\right\}   = \Phi \left( \frac{7}{2}\right)  - \Phi \left( {-\frac{7}{2}}\right)
$$

$$
= {2\Phi }\left( \frac{7}{2}\right)  - 1 = {0.9996}
$$

$$
P\{ \left| X\right|  > 2\}  = P\{ X > 2\text{ 或 }X <  - 2\}  = P\{ X > 2\}  + P\{ X <  - 2\}
$$

$$
= 1 - P\{ X \leq  2\}  + P\{ X <  - 2\}
$$

$$
= 1 - P\left\{  {\frac{X - 3}{2} \leq  \frac{2 - 3}{2}}\right\}   + P\left\{  {\frac{X - 3}{2} < \frac{-2 - 3}{2}}\right\}
$$

$$
= 1 - \Phi \left( {-\frac{1}{2}}\right)  + \Phi \left( {-\frac{5}{2}}\right)  = {0.6977}
$$

$P\{ X > 3\}  = 1 - P\{ X \leq  3\}  = 1 - P\left\{  {\frac{X - 3}{2} \leq  \frac{3 - 3}{2}}\right\}   = 1 - \Phi \left( 0\right)  = 1 - {0.5} = {0.5}$

(2) 由 $P\{ X > c\}  = P\{ X \leq  c\}$,则 $1 - P\{ X \leq  c\}  = P\{ X \leq  c\}$

$P\{ X \leq  c\}  = P\left\{  {\frac{X - 3}{2} \leq  \frac{c - 3}{2}}\right\}   = \Phi \left( \frac{c - 3}{2}\right)  = \frac{1}{2}$

查表得 $\frac{c - 3}{2} = 0$,故 $c = 3$.

(3) $P\{ X > d\}  = 1 - P\{ X \leq  d\}  = 1 - P\left\{  {\frac{X - 3}{2} \leq  \frac{d - 3}{2}}\right\}   = 1 - \Phi \left( \frac{d - 3}{2}\right)  \geq  {0.9}$

则 $\Phi \left( \frac{d - 3}{2}\right)  \leq  {0.1}$,所以 $\frac{d - 3}{2} < 0$. 那么 $\Phi \left( \frac{3 - d}{2}\right)  \geq  {0.9}$

查标准正态分布表知 $\Phi \left( {1.29}\right)  = {0.9015}$,取 $\frac{3 - d}{2} \geq  {1.29}$,得到 $d \leq  {0.42}$.

【3.10】设随机变量 $X$ 服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$,则随 $\sigma$ 的增大,概率 $P\left\{  {\left| {X - \mu }\right|  < \sigma }\right\}$ (   ).

(A) 单调增加 (B) 单调减少 (C) 保持不变 (D) 非单调变化

解 $P\{ \left| {X - \mu }\right|  < \sigma \}  = P\left\{  {\left| \frac{X - \mu }{\sigma }\right|  < 1}\right\}   = \Phi \left( 1\right)  - \Phi \left( {-1}\right)$

可见概率 $P\{ \left| {X - \mu }\right|  < \sigma \}$ 不随 $\sigma$ 的增大而改变.

故应选(C)

点评 对于正态分布的题型,普通正态分布化成标准正态分布,往往是解决问题的关键,以上两例说明了这一点.

【3.11】若随机变量 $Y$ 在 $\left( {1,6}\right)$ 上服从均匀分布,则方程 ${x}^{2} + {Yx} + 1 = 0$ 有实根的概率是 _____.

解 从二次代数方程存在实根的判定条件得出 $Y$ 的变化范围,再由 $Y$ 的分布确定此事件的概率.

方程 ${x}^{2} + {Yx} + 1 = 0$ 有实根的条件是: $\Delta  = {Y}^{2} - 4 \geq  0$,即 $Y \geq  2$ 或 $Y \leq   - 2$

由于 $Y$ 服从 $\left( {1,6}\right)$ 均匀分布,故 $Y$ 的密度函数为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{5}, & 1 < y < 6, \\  0, & y \geq  6\text{ 或 }y \leq   \end{array}\right.
$$

所以, $P\left\{  {{x}^{2} + {Yx} + 1 = 0\text{有实根}}\right\}   = P\{ Y \geq  2\}  + P\{ Y \leq   - 2\}  = \frac{4}{5}$.

故应填 $\frac{4}{5}$.

【3.12】设顾客在某银行的窗口等待服务的时间 $X$ (以分计) 服从指数分布,其概率密度为

$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{5}{\mathrm{e}}^{-\frac{x}{5}}, & x > 0 \\  0, & \text{ 其他 } \end{array}\right.
$$

某顾客在窗口等待服务,若超过 10 分钟,他就离开. 他一个月要到银行 5 次,以 $Y$ 表示一个月内他未等到服务而离开窗口的次数,写出 $Y$ 的分布律,并求 $P\{ Y \geq  1\}$.

解 该顾客在窗口未等到服务而离开的概率为

$$
p = P\{ X > {10}\}  = {\int }_{10}^{+\infty }{f}_{X}\left( x\right) \mathrm{d}x = {\int }_{10}^{+\infty }\frac{1}{5}{\mathrm{e}}^{-\frac{x}{5}}\mathrm{\;d}x =  - {\left. {\mathrm{e}}^{-\frac{x}{5}}\right| }_{10}^{+\infty } = {\mathrm{e}}^{-2}
$$

显然 $Y \sim  B\left( {5,{\mathrm{e}}^{-2}}\right)$,故

$$
P\{ Y = k\}  = {C}_{5}^{k}{\mathrm{e}}^{-{2k}}{\left( 1 - {\mathrm{e}}^{-2}\right) }^{5 - k},\;k = 0,1,2,3,4,5
$$

$$
P\{ Y \geq  1\}  = 1 - P\{ Y = 0\}  = 1 - {\left( 1 - {\mathrm{e}}^{-2}\right) }^{5} = {0.5167}.
$$

【3.13】由某机器生产的螺栓的长度 $\left( \mathrm{{cm}}\right)$ 服从参数为 $\mu  = {10.05},\sigma  = {0.06}$ 的正态分布,规定长度在 ${10.05} \pm  {0.12}$ 内为合格. 求一螺栓为不合格品的概率.

解 设螺栓的长度为 $X$,则 $X \sim  N\left( {{10.05},{0.06}^{2}}\right)$,则一螺栓为不合格品的概率为

$$
p = 1 - P\{ {10.05} - {0.12} < X < {10.05} + {0.12}\}
$$

$$
= 1 - \Phi \left( \frac{{10.17} - {10.05}}{0.06}\right)  + \Phi \left( \frac{{10.05} - {0.12} - {10.05}}{0.06}\right)
$$

$$
= 1 - \Phi \left( 2\right)  - \Phi \left( {-2}\right)  = 2 - {2\Phi }\left( 2\right)  = {0.0455}\text{.}
$$

【3.14】一工厂生产的电子管的寿命 $X$ (以小时计) 服从参数为 $\mu  = {160},\sigma$ 的正态分布,若要求 $P\{ {120} < X \leq  {200}\}  \geq  {0.80}$,允许 $\sigma$ 最大为多少?

解 若要求 $P\{ {120} < X \leq  {200}\}  \geq  {0.80}$,即

$$
\Phi \left( \frac{{200} - {160}}{\sigma }\right)  - \Phi \left( \frac{{120} - {160}}{\sigma }\right)  = \Phi \left( \frac{40}{\sigma }\right)  - \Phi \left( {-\frac{40}{\sigma }}\right)  = {2\Phi }\left( \frac{40}{\sigma }\right)  - 1 \geq  {0.80}
$$

$$
\Phi \left( \frac{40}{\sigma }\right)  \geq  {0.9}
$$

从而 $\frac{40}{\sigma } \geq  {1.28},\sigma  \leq  {31.25}$,即允许 $\sigma$ 最大为 31.25.

【3.15】设 ${X}_{1},{X}_{2},{X}_{3}$ 是随机变量,且 ${X}_{1} \sim  N\left( {0,1}\right),{X}_{2} \sim  N\left( {0,{2}^{2}}\right),{X}_{3} \sim  N\left( {5,{3}^{2}}\right),{p}_{i} =$ $P\left\{  {-2 \leq  {X}_{i} \leq  2}\right\}  \left( {i = 1,2,3}\right)$,则(   )

(A) ${p}_{1} > {p}_{2} > {p}_{3}$ (B) ${p}_{2} > {p}_{1} > {p}_{3}$

(C) ${p}_{3} > {p}_{1} > {p}_{2}$ (D) ${p}_{1} > {p}_{3} > {p}_{2}$

解 将所求的概率 ${p}_{i}$ 用标准正态分布 $N\left( {0,1}\right)$ 的分布函数 $\Phi \left( x\right)$ 表示出来,再通过 $\Phi \left( x\right)$ 的几何意义求解.

由题意可得

$$
{p}_{1} = P\left\{  {-2 \leq  {X}_{1} \leq  2}\right\}   = \Phi \left( 2\right)  - \Phi \left( {-2}\right)  = {2\Phi }\left( 2\right)  - 1,
$$

$$
{p}_{2} = P\left\{  {-2 \leq  {X}_{2} \leq  2}\right\}   = P\left\{  {\frac{-2 - 0}{2} \leq  \frac{{X}_{2} - 0}{2} \leq  \frac{2 - 0}{2}}\right\}
$$

$$
= \Phi \left( 1\right)  - \Phi \left( {-1}\right)  = {2\Phi }\left( 1\right)  - 1,
$$

$$
{p}_{3} = P\left\{  {-2 \leq  {X}_{3} \leq  2}\right\}   = P\left\{  {\frac{-2 - 5}{3} \leq  \frac{{X}_{3} - 5}{3} \leq  \frac{2 - 5}{3}}\right\}
$$

$$
= \Phi \left( {-1}\right)  - \Phi \left( {-\frac{7}{3}}\right)  = \Phi \left( \frac{7}{3}\right)  - \Phi \left( 1\right),
$$

由下图 2-3.15 可知, ${p}_{1} > {p}_{2} > {p}_{3}$,

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_54_616_172_351_220_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_54_616_172_351_220_0.jpg)

图 2-3.15

故应选(A).

## § 4. 随机变量函数的分布

### 知识要点

#### 1. 离散型随机变量函数的分布

设随机变量 $X$ 的分布律为 $P\left\{  {X = {x}_{k}}\right\}   = {p}_{k}, k = 1,2,3\cdots$,则当 $Y = g\left( X\right)$ 的所有取值为 ${y}_{j}$ $\left( {j = 1,2,\cdots }\right)$ 时,随机变量 $Y$ 有分布律

$$
P\left\{  {Y = {y}_{j}}\right\}   = \mathop{\sum }\limits_{{g\left( {x}_{k}\right)  = {y}_{j}}}P\left\{  {X = {x}_{k}}\right\} .
$$

#### 2. 连续型随机变量函数的分布

方法一: 设随机变量 $X$ 的概率密度函数为 ${f}_{X}\left( x\right) \left( {-\infty  < x <  + \infty }\right)$,那么 $Y = g\left( X\right)$ 的分布函数为

$$
{F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\{ g\left( X\right)  \leq  y\}  = {\int }_{g\left( x\right)  \leq  y}{f}_{X}\left( x\right) \mathrm{d}x,
$$

其概率密度为 ${f}_{Y}\left( y\right)  = {F}_{Y}{}^{\prime }\left( y\right)$.

方法二: 设随机变量 $X$ 具有概率密度函数 ${f}_{X}\left( x\right) \left( {-\infty  < x <  + \infty }\right), g\left( x\right)$ 为 $\left( {-\infty, + \infty }\right)$ 内的严格单调的可导函数,则随机变量 $Y = g\left( X\right)$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} {f}_{X}\left\lbrack  {h\left( y\right) }\right\rbrack  \left| {{h}^{\prime }\left( y\right) }\right|, & \alpha  < y < \beta \\  0, & \text{ 其他 } \end{array}\right.
$$

其中 $h\left( y\right)$ 是 $g\left( x\right)$ 的反函数, $\alpha  = \min \{ g\left( {-\infty }\right), g\left( {+\infty }\right) \},\beta  = \max \{ g\left( {-\infty }\right), g\left( {+\infty }\right) \}$.

### 基本题型

#### 题型 1:离散型随机变量函数的分布

【4.1】已知 $X$ 的分布律如下表所示

<table><tr><td>$X$</td><td>0</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td></tr><tr><td>$P\{ X = x\}$</td><td>$\frac{1}{12}$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{12}$</td><td>$\frac{2}{9}$</td><td>$\frac{1}{9}$</td></tr></table>

则 $Y = {\left( X - 2\right) }^{2}$ 的分布律为_____.

解 记 $g\left( x\right)  = {\left( x - 2\right) }^{2}$. 由于 $g\left( 0\right)  = g\left( 4\right)  = 4, g\left( 1\right)  = g\left( 3\right)  = 1, g\left( 2\right)  = 0, g\left( 5\right)  =$ 9,因此

$$
P\{ Y = 0\}  = P\{ X = 2\}  = \frac{1}{3}
$$

$$
P\{ Y = 1\}  = P\{ X = 1\}  + P\{ X = 3\}  = \frac{1}{6} + \frac{1}{12} = \frac{1}{4}
$$

$$
P\{ Y = 4\}  = P\{ X = 0\}  + P\{ X = 4\}  = \frac{1}{12} + \frac{2}{9} = \frac{11}{36}
$$

$$
P\{ Y = 9\}  = P\{ X = 5\}  = \frac{1}{9}
$$

故应填

<table><tr><td>$Y$</td><td>0</td><td>1</td><td>4</td><td>9</td></tr><tr><td>$P\{ Y = y\}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{4}$</td><td>$\frac{11}{36}$</td><td>$\frac{1}{9}$</td></tr></table>

点评 求离散型随机变量函数的分布律时, 要注意两种情形:

设 $X$ 为离散型随机变量,其分布律为 $P\left\{  {X = {x}_{k}}\right\}   = {p}_{k}, k = 1,2,\cdots$,则 $Y = g\left( X\right)$ 的分布律为:

(1) 当 ${y}_{k}$ 各不相同时, $P\left\{  {Y = {y}_{k}}\right\}   = P\left\{  {g\left( X\right)  = {y}_{k}}\right\}   = {p}_{k}, k = 1,2,\cdots$

(2)当 ${y}_{k}$ 有重复时, $P\left\{  {Y = {y}_{k}}\right\}   = P\left\{  {g\left( X\right)  = {y}_{k}}\right\}   = \mathop{\sum }\limits_{{g\left( {x}_{i}\right)  = {y}_{k}}}{p}_{i}$.

【4.2】设随机变量 $X$ 的概率分布为 $P\{ X = k\}  = \frac{1}{{2}^{k}}, k = 1,2,3,\cdots$. 试求随机变量 $Y =$ $\sin \left( {\frac{\pi }{2}X}\right)$ 的分布律.

解 $P\{ Y = 0\}  = P\{ X = 2\}  + P\{ X = 4\}  + P\{ X = 6\}  + \cdots  = \frac{1}{{2}^{2}} + \frac{1}{{2}^{4}} + \frac{1}{{2}^{6}} + \cdots  = \frac{1}{3}$.

$P\{ Y =  - 1\}  = P\{ X = 3\}  + P\{ X = 7\}  + P\{ X = {11}\}  + \cdots  = \frac{1}{{2}^{3}} + \frac{1}{{2}^{7}} + \frac{1}{{2}^{11}} + \cdots  =$

$\frac{2}{15}$.

$P\{ Y = 1\}  = 1 - P\{ Y = 0\}  - P\{ Y =  - 1\}  = \frac{8}{15}.$

故 $Y = \sin \left( {\frac{\pi }{2}X}\right)$ 的分布律为:

<table><tr><td>$Y$-1 0 $\frac{1}{3}$</td><td>1</td></tr><tr><td>$P$$\frac{2}{15}$</td><td>$\frac{8}{15}$</td></tr></table>

【4.3】设离散型随机变量 $X$ 服从泊松分布,参数 $\lambda  = 4$,则 ${3X} - 2$ 的分布律为_____.

解 $P\{ Y = k\}  = P\{ {3X} - 2 = k\}  = P\left\{  {X = \frac{k + 2}{3}}\right\}   = \frac{{4}^{\frac{k + 2}{3}}{\mathrm{e}}^{-4}}{\left( \frac{k + 2}{3}\right) !}\;(k = {3n} - 2, n = 0$, $1,2,\cdots )$

故应填 $\frac{{4}^{\frac{k + 2}{3}}{\mathrm{e}}^{-4}}{\left( \frac{k + 2}{3}\right) !}$.

点评 本题中 $X$ 和 $Y = g\left( X\right)$ 均为无限可列的离散型随机变量,对于此类题型只需注意函数关系的转化即可求出分布律.

【4.4】已知 $X$ 的分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x <  - 1 \\  \frac{1}{3}, &  - 1 \leq  x < 0 \\  \frac{1}{2}, & 0 \leq  x < 1 \\  \frac{2}{3}, & 1 \leq  x < 2 \\  1, & 2 \leq  x \end{array}\right.
$$

求 $Y = {\left( \sin \frac{\pi }{6}X\right) }^{2}$ 的分布函数.

解 直接求 $Y$ 的分布函数 ${F}_{Y}\left( y\right)$ 较为困难,可先利用 $X$ 与 $Y$ 分布律之间的关系求出 $Y$ 的分布律.

由题意可得 $X$ 的分布律

<table><tr><td>$X$</td><td>-1</td><td>0</td><td>1</td><td>2</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{3}$</td></tr></table>

则 $Y = {\left( \sin \frac{\pi }{6}X\right) }^{2}$ 的分布律为即

<table><tr><td>$Y$</td><td>$\frac{1}{4}$</td><td>0</td><td>$\frac{1}{4}$</td><td>$\frac{3}{4}$</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{3}$</td></tr></table>

<table><tr><td>$Y$</td><td>0</td><td>$\frac{1}{4}$</td><td>$\frac{3}{4}$</td></tr><tr><td>$P$</td><td>$\frac{1}{6}$</td><td>$\frac{1}{2}$</td><td>$\frac{1}{3}$</td></tr></table>

故 $Y$ 的分布函数为

$$
{F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = \left\{  \begin{array}{ll} 0, & y < 0 \\  \frac{1}{6}, & 0 \leq  y < \frac{1}{4} \\  \frac{2}{3}, & \frac{1}{4} \leq  y < \frac{3}{4} \\  1, & y \geq  \frac{3}{4} \end{array}\right.
$$

#### 题型 2:连续型随机变量函数的分布

【4.5】设随机变量 $X$ 的分布函数为 $F\left( x\right)$,则随机变量 $Y = {2X} + 1$ 的分布函数 $G\left( y\right)  =$ (   ).

(A) $F\left( {\frac{1}{2}y + 1}\right)$ (B) ${2F}\left( y\right)  + 1$ (C) $\frac{1}{2}F\left( y\right)  - \frac{1}{2}$ (D) $F\left( {\frac{1}{2}y - \frac{1}{2}}\right)$

解 $G\left( y\right)  = P\{ Y \leq  y\}  = P\{ {2X} + 1 \leq  y\}  = P\left\{  {X \leq  \frac{y - 1}{2}}\right\}   = F\left( \frac{y - 1}{2}\right)$

故应选(D).

【4.6】设随机变量 $X$ 服从 $\left( {0,2}\right)$ 上的均匀分布,则随机变量 $Y = {X}^{2}$ 的概率密度 ${f}_{Y}\left( y\right)  =$ _____. 解法一 分布函数法(或定义法)

由已知条件可知,

① 当 $y \leq  0$ 时, ${F}_{Y}\left( y\right)  = 0$

② 当 $y \geq  4$ 时, ${F}_{Y}\left( y\right)  = 1$

③ 当 $0 < y < 4$ 时, ${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\left\{  {{X}^{2} \leq  y}\right\}   = P\{ X \leq  \sqrt{y}\}  = {F}_{X}\left( \sqrt{y}\right)$.

由于 $X$ 服从 $\left( {0,2}\right)$ 上的均匀分布,所以

$$
{F}_{Y}\left( y\right)  = {F}_{X}\left( \sqrt{y}\right)  = \frac{\sqrt{y}}{2}.
$$

因此 ${f}_{Y}\left( y\right)  = {F}_{Y}{}^{\prime }\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{4\sqrt{y}}, & 0 < y < 4 \\  0, & \text{ 其他 } \end{array}\right.$

解法二 公式法 (或复合函数求导法)

因为 $y = {x}^{2}$ 在 $\left( {0,4}\right)$ 内单调,其反函数 $x = \sqrt{y}$ 在 $\left( {0,2}\right)$ 内可导,那么

$$
{f}_{Y}\left( y\right)  = {f}_{X}\left( \sqrt{y}\right) {\left( \sqrt{y}\right) }^{\prime } = \frac{1}{2\sqrt{y}} \times  \frac{1}{2} = \frac{1}{4\sqrt{y}},\;\left( {0 < y < 4}\right)
$$

此处对 $\sqrt{y}$ 求导得 $\frac{1}{2\sqrt{y}} > 0$,因 ${f}_{Y}\left( y\right)  \geq  0$,从而符合概率密度非负的性质. 若对反函数求导为负值时,需要取其绝对值. 因此随机变量 $Y$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{matrix} \frac{1}{4\sqrt{y}}, & 0 < y < 4 \\  0, & \text{ 其他 } \end{matrix}\right.
$$

点评 连续型随机变量函数的分布有两种求法,一是先通过随机变量的概率密度或分布函数求出随机变量函数的分布函数, 再求其概率密度. 二是如果随机变量函数是严格单调可导函数. 先求其反函数, 再根据公式算出其概率密度.

【4.7】设随机变量 $X$ 的概率密度为 ${f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} {\mathrm{e}}^{-x}, & x \geq  0; \\  0, & x < 0. \end{array}\right.$ 试求随机变量 $Y = {\mathrm{e}}^{X}$ 的概率密度 ${f}_{Y}\left( y\right)$.

解法一 分段考查 $Y$ 的分布函数.

① 当 $y \leq  1$ 时, ${f}_{X}\left( x\right)  = 0,{F}_{Y}\left( y\right)  = 0$

② 当 $y > 1$ 时, ${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\left\{  {{\mathrm{e}}^{X} \leq  y}\right\}   = P\{ X \leq  \ln y\}  = {\int }_{0}^{\ln y}{\mathrm{e}}^{-x}\mathrm{\;d}x = 1 - {y}^{-1}$

则 ${f}_{Y}\left( y\right)  = {F}_{Y}{}^{\prime }\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{{y}^{2}}, & y > 1 \\  0, & y \leq  1 \end{array}\right.$

解法二 因为 $y = {\mathrm{e}}^{x}$ 在 $\left( {0, + \infty }\right)$ 内是单调的,其反函数 $x = \ln y$ 在 $\left( {1, + \infty }\right)$ 内是可导的,

且 ${x}^{\prime } = \frac{1}{y} > 0$,所以根据复合函数求导公式有, ${f}_{Y}\left( y\right)  = \frac{1}{{y}^{2}}$.

所以 ${f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{{y}^{2}}, & y > 1 \\  0, & y \leq  1 \end{array}\right.$

【4.8】设 $X \sim  N\left( {0,1}\right)$

(1)求 $Y = {\mathrm{e}}^{X}$ 的概率密度；

(2)求 $Y = 2{X}^{2} + 1$ 的概率密度；

(3)求 $Y = \left| X\right|$ 的概率密度.

解 (1) $X$ 的概率密度为 $f\left( x\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}, - \infty  < x <  + \infty$.

因为 $Y = {\mathrm{e}}^{X}$,故 $Y > 0$,所以当 $y \leq  0$ 时, $\{ Y \leq  y\}$ 为不可能事件,

$$
{F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = 0,\;{f}_{Y}\left( y\right)  = {F}_{Y}^{\prime }\left( y\right)  = 0.
$$

当 $y > 0$ 时,由 $y = {\mathrm{e}}^{x}$ 得 $x = \ln y = h\left( y\right),{h}^{\prime }\left( y\right)  = \frac{1}{y}$,由定理得 $Y = {\mathrm{e}}^{x}$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{1}{2}{\left( \ln y\right) }^{2}} \cdot  \frac{1}{y}
$$

故 ${f}_{Y}\left( y\right)  = \left\{  \begin{matrix} \frac{1}{\sqrt{2\pi }y}{\mathrm{e}}^{-\frac{1}{2}{\left( \ln y\right) }^{2}}, & y > 0 \\  0, & y \leq  0 \end{matrix}\right.$

或

${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\left\{  {{\mathrm{e}}^{X} \leq  y}\right\}   = P\{ X \leq  \ln y\}  = {\int }_{-\infty }^{\ln y}f\left( x\right) \mathrm{d}x = {\int }_{-\infty }^{\ln y}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x$

从而 ${f}_{Y}\left( y\right)  = {F}_{Y}{}^{\prime }\left( y\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{\left( \ln y\right) }^{2}}{2}} \cdot  \frac{1}{y},\;\left( {y > 0}\right)$.

(2) 由 $Y = 2{X}^{2} + 1$ 知 $Y \geq  1$,故当 $y < 1$ 时, $\{ Y \leq  y\}$ 是不可能事件,所以 ${F}_{Y}\left( y\right)  = P\{ Y \leq$ $y\}  = 0$,从而 ${f}_{Y}\left( y\right)  = 0$.

当 $y \geq  1$ 时,

$$
{F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\left\{  {2{X}^{2} + 1 \leq  y}\right\}   = P\left\{  {-\sqrt{\frac{y - 1}{2}} \leq  X \leq  \sqrt{\frac{y - 1}{2}}}\right\}
$$

$$
= {\int }_{-\sqrt{\frac{y - 1}{2}}}^{\sqrt{\frac{y - 1}{2}}}f\left( x\right) \mathrm{d}x = {\int }_{-\sqrt{\frac{y - 1}{2}}}^{\sqrt{\frac{y - 1}{2}}}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x
$$

$$
{f}_{Y}\left( y\right)  = {F}_{Y}^{\prime }\left( y\right)  = \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{1}{2} \cdot  \frac{y - 1}{2}} \times  {\left( \sqrt{\frac{y - 1}{2}}\right) }^{\prime } - \frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{1}{2} \cdot  \frac{y - 1}{2}} \times  {\left( -\sqrt{\frac{y - 1}{2}}\right) }^{\prime }
$$

$$
= \frac{1}{2\sqrt{\pi \left( {y - 1}\right) }}{\mathrm{e}}^{-\frac{y - 1}{4}}
$$

即 ${f}_{Y}\left( y\right)  = \left\{  \begin{matrix} \frac{1}{2\sqrt{\pi \left( {y - 1}\right) }}{\mathrm{e}}^{-\frac{y - 1}{4}}, & y > 1 \\  0, & y \leq  1 \end{matrix}\right.$

(3) 由 $Y = \left| X\right|$ 知 $Y \geq  0$,所以当 $y < 0$ 时, $\{ Y \leq  y\}$ 为不可能事件, ${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  =$ 0,故 ${f}_{Y}\left( y\right)  = 0$.

$$
{F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\{ \left| X\right|  \leq  y\}  = P\{  - y \leq  X \leq  y\}
$$

$$
= {\int }_{-y}^{y}f\left( x\right) \mathrm{d}x = {\int }_{-y}^{y}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x = 2{\int }_{0}^{y}\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{x}^{2}}{2}}\mathrm{\;d}x
$$

$$
{f}_{Y}\left( y\right)  = {F}_{Y}{}^{\prime }\left( y\right)  = 2\frac{1}{\sqrt{2\pi }}{\mathrm{e}}^{-\frac{{y}^{2}}{2}}
$$

所以 ${f}_{Y}\left( y\right)  = \left\{  \begin{matrix} \sqrt{\frac{2}{\pi }}{\mathrm{e}}^{-\frac{{y}^{2}}{2}}, & y > 0 \\  0, & y \leq  0 \end{matrix}\right.$

点评 本题 (1) 既可用分布函数法,也可用公式法; (2)、(3) 中 $y = g\left( x\right)$ 不是单调函数,故只能用分布函数法.

## $§5$. 综合提高题型

#### 题型 1: 关于随机变量的判断及选择

【5.1】设离散型随机变量 $X$ 的分布律为: $P\{ X = k\}  = b{\lambda }^{k},\left( {k = 1,2,3,\cdots }\right)$ 且 $b > 0$, 则 $\lambda$ 为 (   ).

(A) $\lambda  > 0$ 的任意实数 (B) $\lambda  = b + 1$ (C) $\lambda  = \frac{1}{1 + b}$ (D) $\lambda  = \frac{1}{b - 1}$

解 因为 $\mathop{\sum }\limits_{{k = 1}}^{\infty }P\{ X = k\}  = \mathop{\sum }\limits_{{k = 1}}^{\infty }b{\lambda }^{k} = 1,\;{S}_{n} = \mathop{\sum }\limits_{{k = 1}}^{n}b{\lambda }^{k} = b \cdot  \frac{\left( {1 - {\lambda }^{n}}\right) \lambda }{1 - \lambda }$ 即

$$
\mathop{\lim }\limits_{{n \rightarrow  \infty }}{S}_{n} = \mathop{\lim }\limits_{{n \rightarrow  \infty }}b \cdot  \lambda \frac{\left( 1 - {\lambda }^{n}\right) }{1 - \lambda } = 1
$$

于是可知,当 $\left| \lambda \right|  < 1$ 时, $b \cdot  \frac{\lambda }{1 - \lambda } = 1$,所以

$$
\lambda  = \frac{1}{1 + b} < 1,\;\left( {\text{ 因 }b > 0}\right)
$$

故应选(C)

【5.2】设 ${F}_{1}\left( x\right)$ 与 ${F}_{2}\left( x\right)$ 为两个分布函数,其相应的概率密度 ${f}_{1}\left( x\right)$ 与 ${f}_{2}\left( x\right)$ 是连续函数,则必为概率密度的是 (   )

(A) ${f}_{1}\left( x\right) {f}_{2}\left( x\right)$. (B) $2{f}_{2}\left( x\right) {F}_{1}\left( x\right)$.

(C) ${f}_{1}\left( x\right) {F}_{2}\left( x\right)$. (D) ${f}_{1}\left( x\right) {F}_{2}\left( x\right)  + {f}_{2}\left( x\right) {F}_{1}\left( x\right)$.

解 因为 ${f}_{1}\left( x\right) {F}_{2}\left( x\right)  + {f}_{2}\left( x\right) {F}_{1}\left( x\right)  \geq  0$,且

${\int }_{-\infty }^{+\infty }\left\lbrack  {{f}_{1}\left( x\right) {F}_{2}\left( x\right)  + {f}_{2}\left( x\right) {F}_{1}\left( x\right) }\right\rbrack  \mathrm{d}x$

$= {\int }_{-\infty }^{+\infty }\left\lbrack  {{F}^{\prime }{}_{1}\left( x\right) {F}_{2}\left( x\right)  + {F}^{\prime }{}_{2}\left( x\right) {F}_{1}\left( x\right) }\right\rbrack  \mathrm{d}x$

$= {F}_{1}\left( x\right) {F}_{2}\left( x\right) {\left. \right| }_{-\infty }^{+\infty } = 1.$

则 ${f}_{1}\left( x\right) {F}_{2}\left( x\right)  + {f}_{2}\left( x\right) {F}_{1}\left( x\right)$ 满足概率密度的两条性质,故应选(D).

点评 本题考查了多个基本知识点, 综合性较强:

① 概率密度的性质: $f\left( x\right)  \geq  0;{\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = 1$;

② 分布函数的性质: $F\left( {-\infty }\right)  = 0;F\left( {+\infty }\right)  = 1$;

③ 分布函数与概率密度的关系: ${F}^{\prime }\left( x\right)  = f\left( x\right)$.

【5.3】设 $X \sim  B\left( {n, p}\right)$,若 $\left( {n + 1}\right) p$ 不是整数,则(   )时 $P\{ X = k\}$ 最大.

(A) $k = \left( {n + 1}\right) p$ (B) $k = \left( {n + 1}\right) p - 1$ (C) $k = {np}$ (D) $k = \left\lbrack  {\left( {n + 1}\right) p}\right\rbrack$

解 由二项分布的性质知, 应选 (D).

点评 设 $X \sim  B\left( {n, p}\right)$,则使 $P\{ X = k\}$ 达到最大的 $k$,称为二项分布的最可能值,记为 ${k}_{0}$ 且

$$
{k}_{0} = \left\{  \begin{array}{ll} \left( {n + 1}\right) p\text{ 和 }\left( {n + 1}\right) p - 1, & \text{ 当 }\left( {n + 1}\right) p\text{ 是整数时 } \\  \left\lbrack  {\left( {n + 1}\right) p}\right\rbrack , & \text{ 其他 } \end{array}\right.
$$

【5.4】设随机变量 $X$ 在区间 $\left( {2,5}\right)$ 上服从均匀分布,现对 $X$ 进行三次独立观测,则至少有两次观测值大于 3 的概率为(   ).

(A) $\frac{20}{27}$ (B) $\frac{27}{30}$ (C) $\frac{2}{5}$ (D) $\frac{2}{3}$

解 由题意“对 $X$ 进行三次独立观测” 即是在相同条件下进行三次独立重复试验,因此所求概率属于伯努利概型的概率计算问题.

以 $A$ 表示事件“对 $X$ 的观测值大于 ${3}^{\prime \prime }$,即 $A = \{ X > 3\}$,由题设知 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{3}, & 2 < x < 5 \\  0, & \text{ 其他 } \end{array}\right.
$$

因此 $P\left( A\right)  = P\{ X > 3\}  = {\int }_{3}^{5}\frac{1}{3}\mathrm{\;d}x = \frac{2}{3}$.

以 $Y$ 表示三次独立观测中观测值大于 3 的次数,则 $Y$ 的可能值为0,1,2,3,且据伯努利概型的计算公式, $Y$ 取各可能值的概率为

$$
P\{ Y = k\}  = {C}_{3}^{k}{p}^{k}{q}^{3 - k} = {C}_{3}^{k}{\left( \frac{2}{3}\right) }^{k}{\left( \frac{1}{3}\right) }^{3 - k}\;\left( {k = 0,1,2,3}\right)
$$

即 $Y \sim  B\left( {3,\frac{2}{3}}\right)$. 从而,所求概率为

$$
P\{ Y \geq  2\}  = {C}_{3}^{2}{\left( \frac{2}{3}\right) }^{2}\left( \frac{1}{3}\right)  + {C}_{3}^{3}{\left( \frac{2}{3}\right) }^{3} = \frac{20}{27}
$$

故应选 (A).

【5.5】当随机变量的可能值充满区间(   ),则 $\varphi \left( x\right)  = \cos x$ 可以成为随机变量 $X$ 的分布

密度.

(A) $\left\lbrack  {0,\frac{\pi }{2}}\right\rbrack$ (B) $\left\lbrack  {\frac{\pi }{2},\pi }\right\rbrack$ (C) $\left\lbrack  {0,\pi }\right\rbrack$ (D) $\left\lbrack  {\frac{3}{2}\pi,\frac{7}{4}\pi }\right\rbrack$

解 由随机变量 $X$ 的分布密度函数 $\varphi \left( x\right)$ 的非负性可知 (B)、(C) 不该入选.

又 ${\int }_{-\infty }^{+\infty }\varphi \left( x\right) \mathrm{d}x = 1$. 验证

(A) ${\int }_{-\infty }^{+\infty }\varphi \left( x\right) \mathrm{d}x = {\int }_{0}^{\frac{\pi }{2}}\cos x\mathrm{\;d}x = {\left. \sin x\right| }_{0}^{\frac{\pi }{2}} = 1$

(D) ${\int }_{-\infty }^{+\infty }\varphi \left( x\right) \mathrm{d}x = {\int }_{\frac{3}{2}\pi }^{\frac{7}{4}\pi }\cos x\mathrm{\;d}x = {\left. \sin x\right| }_{\begin{matrix} {\frac{3}{2}\pi } \\  {\frac{3}{2}\pi } \end{matrix}}^{\frac{7}{4}\pi } = \frac{\sqrt{2}}{2} + 1$

故应选(A).

【5.6】设 $X$ 为随机变量,若矩阵 $A = \left\lbrack  \begin{matrix} 2 & 3 & 2 \\  0 &  - 2 &  - X \\  0 & 1 & 0 \end{matrix}\right\rbrack$ 的特征值全为实数的概率为 0.5,

则(   ).

(A) $X$ 服从区间 $\left\lbrack  {0,2}\right\rbrack$ 的均匀分布 (B) $X$ 服从二项分布 $B\left( {2,{0.5}}\right)$

(C) $X$ 服从参数为 1 的指数分布 (D) $X$ 服从正态分布 $N\left( {0,1}\right)$

解 由 $\left| {{\lambda E} - A}\right|  = \left\lbrack  \begin{matrix} \lambda  - 2 &  - 3 &  - 2 \\  0 & \lambda  + 2 & X \\  0 &  - 1 & \lambda  \end{matrix}\right\rbrack   = \left( {\lambda  - 2}\right) \left( {{\lambda }^{2} + {2\lambda } + X}\right)$,而其特征值全为实数的概率 $P\left\{  {{2}^{2} - {4X} \geq  0}\right\}   = P\{ X \leq  1\}  = {0.5}$,可见当 $X$ 服从 $\left\lbrack  {0,2}\right\rbrack$ 上均匀分布时成立.

故应选(A).

【5.7】设随机变量 $X$ 的密度函数为 ${f}_{X}\left( x\right)$,则 $Y = 3 - {2X}$ 的密度函数为 (   ).

(A) $- \frac{1}{2}{f}_{X}\left( {-\frac{y - 3}{2}}\right)$ (B) $\frac{1}{2}{f}_{X}\left( {-\frac{y - 3}{2}}\right)$

(C) $- \frac{1}{2}{f}_{X}\left( {-\frac{y + 3}{2}}\right)$ (D) $\frac{1}{2}{f}_{X}\left( {-\frac{y + 3}{2}}\right)$

解 本题是求连续型随机变量函数的概率密度,因为 $Y = g\left( X\right)$ 是单调函数,由公式法可知 (B) 正确.

【5.8】设随机变量 $X$ 具有对称的概率密度,即 $f\left( {-x}\right)  = f\left( x\right)$,则对任意 $a > 0, P\{ \left| X\right|  >$ $a\}$ 是 (   ).

(A) $1 - {2F}\left( a\right)$ (B) ${2F}\left( a\right)  - 1$ (C) $2 - F\left( a\right)$ (D) $2\left\lbrack  {1 - F\left( a\right) }\right\rbrack$

解 因为 $f\left( {-x}\right)  = f\left( x\right)$,所以


$$
F\left( {-a}\right)  = {\int }_{-\infty }^{-a}f\left( x\right) \mathrm{d}x = {\int }_{a}^{+\infty }f\left( x\right) \mathrm{d}x
$$

所以

$$
F\left( a\right)  + F\left( {-a}\right)  = {\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = 1 \Rightarrow  F\left( {-a}\right)  = 1 - F\left( a\right)
$$

$$
\Rightarrow  P\{ \left| X\right|  > a\}  = 1 - P\{ \left| X\right|  < a\}  = 1 - P\{  - a < X < a\}
$$

$$
= 1 - \left\lbrack  {F\left( a\right)  - F\left( {-a}\right) }\right\rbrack   = 1 - \left\lbrack  {F\left( a\right)  - \left( {1 - F\left( a\right) }\right) }\right\rbrack   = 2\left\lbrack  {1 - F\left( a\right) }\right\rbrack .
$$

故应选(D).

【5.9】设随机变量 $X$ 服从正态分布 $N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right)$,随机变量 $Y$ 服从正态分布 $N\left( {{\mu }_{2},{\sigma }_{2}^{2}}\right)$,且

$P\left\{  {\left| {X - {\mu }_{1}}\right|  < 1}\right\}   > P\left\{  {\left| {Y - {\mu }_{2}}\right|  < 1}\right\}$,则必有 (   ).

(A) ${\sigma }_{1} < {\sigma }_{2}$ (B) ${\sigma }_{1} > {\sigma }_{2}$ (C) ${\mu }_{1} < {\mu }_{2}$ (D) ${\mu }_{1} > {\mu }_{2}$

解 $P\left\{  {\left| {X - {\mu }_{1}}\right|  < 1}\right\}   > P\left\{  {\left| {Y - {\mu }_{2}}\right|  < 1}\right\}$,即

$$
P\left\{  {\frac{-1}{{\sigma }_{1}} < \frac{X - {\mu }_{1}}{{\sigma }_{1}} < \frac{1}{{\sigma }_{1}}}\right\}   > P\left\{  {\frac{-1}{{\sigma }_{2}} < \frac{Y - {\mu }_{2}}{{\sigma }_{2}} < \frac{1}{{\sigma }_{2}}}\right\} ,
$$

从而 ${2\Phi }\left( \frac{1}{{\sigma }_{1}}\right)  - 1 > {2\Phi }\left( \frac{1}{{\sigma }_{2}}\right)  - 1$,故

$$
\Phi \left( \frac{1}{{\sigma }_{1}}\right)  > \Phi \left( \frac{1}{{\sigma }_{2}}\right),\;\frac{1}{{\sigma }_{1}} > \frac{1}{{\sigma }_{2}},\;\text{得}{\sigma }_{2} > {\sigma }_{1}
$$

故应选 (A).

【5.10】设随机变量 $X$ 的分布函数 $F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0 \\  \frac{1}{2}, & 0 \leq  x < 1, \\  1 - {\mathrm{e}}^{-x}, & x \geq  1 \end{array}\right.$ 则 $P\{ X = 1\}  =$ (   )

(A) 0 (B) $\frac{1}{2}$ (C) $\frac{1}{2} - {\mathrm{e}}^{-1}$ (D) $1 - {\mathrm{e}}^{-1}$

解 $P\{ X = 1\}  = P\{ X \leq  1\}  - P\{ X < 1\}  = F\left( 1\right)  - F\left( {1 - 0}\right)  = \left( {1 - {\mathrm{e}}^{-1}}\right)  - \frac{1}{2} = \frac{1}{2} - {\mathrm{e}}^{-1}$.

故应选(C)

#### 题型 2: 利用随机变量的分布求概率

【5.11】设随机变量 $X$ 的分布函数为 ${F}_{X}\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 1 \\  \ln x, & 1 \leq  x < \mathrm{e} \\  1, & x \geq  \mathrm{e} \end{array}\right.$

(1) 求 $P\{ X < 2\},\;P\{ 0 < X \leq  3\},\;P\left\{  {2 < X < \frac{5}{2}}\right\}$;

(2)求概率密度函数 ${f}_{X}\left( x\right)$.

解 (1) $P\{ X < 2\}  = {F}_{X}\left( 2\right)  = \ln 2$

$P\{ 0 < X \leq  3\}  = {F}_{X}\left( 3\right)  - {F}_{X}\left( 0\right)  = 1 - 0 = 1$

$P\left\{  {2 < X < \frac{5}{2}}\right\}   = {F}_{X}\left( \frac{5}{2}\right)  - {F}_{X}\left( 2\right)  = \ln \frac{5}{2} - \ln 2 = \ln \frac{5}{4}$

(2) ${f}_{X}\left( x\right)  = {F}_{X}{}^{\prime }\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{x}, & 1 < x < \mathrm{e} \\  0, & \text{ 其他 } \end{array}\right.$ 概率论与数理统计习题精选精解

【5.12】某公共汽车从上午 $7 : {00}$ 起每隔 15 分钟有一趟班车经过某车站,即 $7 : {00},7 : {15},7 :$ ${30},\cdots$ 时刻有班车到达此车站,如果某乘客是在 7:00 至 7:30 等可能地到达此车站候车,问他等候不超过 5 分钟便乘上汽车的概率.

解 设乘客于 7 点过 $X$ 分钟到达车站,则 $X \sim  U\left\lbrack  {0,{30}}\right\rbrack$,即其概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{30}, & 0 \leq  x \leq  {30} \\  0, & \text{ 其他 } \end{array}\right.
$$

于是该乘客等候不超过 5 分钟便能乘上汽车的概率为

$$
P\{ {10} \leq  X \leq  {15}\text{ 或 }{25} \leq  X \leq  {30}\}  = P\{ {10} \leq  X \leq  {15}\}  + P\{ {25} \leq  X \leq  {30}\}
$$

$$
= {\int }_{10}^{15}\frac{1}{30}\mathrm{\;d}x + {\int }_{25}^{30}\frac{1}{30}\mathrm{\;d}x = \frac{5}{30} + \frac{5}{30} = \frac{1}{3}
$$

【5.13】设 $X$ 是在 $\left\lbrack  {0,1}\right\rbrack$ 上取值的连续型随机变量,且 $P\{ X \leq  {0.29}\}  = {0.75}$. 如果 $Y = 1 -$ $X$,则 $k =$ _____时, $P\{ Y \leq  k\}  = {0.25}$.

解 $P\{ Y \leq  k\}  = P\{ 1 - X \leq  k\}  = P\{ X \geq  1 - k\}  = 1 - P\{ X < 1 - k\}  = {0.25}$

所以 $P\{ X < 1 - k\}  = {0.75}$,则 $1 - k = {0.29}$.

即 $k = {0.71}$.

【5.14】设 $X \sim  \left\lbrack  \begin{matrix} 0 & 1 \\  \frac{1}{4} & \frac{3}{4} \end{matrix}\right\rbrack , P\left\{  {Y =  - \frac{1}{2}}\right\}   = 1$,又 $n$ 维向量 ${\alpha }_{1}$ 、 ${\alpha }_{2}$ 、 ${\alpha }_{3}$ 线性无关,则 ${\alpha }_{1} + {\alpha }_{2}$, ${\alpha }_{2} + 2{\alpha }_{3}, X{\alpha }_{3} + Y{\alpha }_{1}$ 线性相关的概率为(   ).

(A) $\frac{3}{4}$ (B) $\frac{1}{4}$ (C) 1 (D) $\frac{1}{2}$

解 ${\alpha }_{1} + {\alpha }_{2},{\alpha }_{2} + 2{\alpha }_{3}, X{\alpha }_{3} + Y{\alpha }_{1}$ 线性相关 $\Leftrightarrow  \left| \begin{matrix} 1 & 1 & 0 \\  0 & 1 & 2 \\  Y & 0 & X \end{matrix}\right|  = X + {2Y} = 0$

$$
P\{ X + {2Y} = 0\}  = P\left\{  {X + {2Y} = 0, Y =  - \frac{1}{2}}\right\}   = P\left\{  {X = 1, Y =  - \frac{1}{2}}\right\}
$$

$$
= P\{ X = 1\}  = \frac{3}{4}
$$

故应选(A).

【5.15】连续型随机变量 $X$ 的密度函数为

$$
p\left( x\right)  = \left\{  \begin{matrix} \frac{A}{\sqrt{1 - {x}^{2}}}, & \left| x\right|  < 1 \\  0, & \text{ 其他 } \end{matrix}\right.
$$

求: (1) 系数 $A$;

(2) $X$ 落在区间 $\left( {-\frac{1}{2},\frac{1}{2}}\right)$ 内的概率；

(3) $X$ 的分布函数.

解 (1) 因为 ${\int }_{-\infty }^{+\infty }p\left( x\right) \mathrm{d}x = 1$,故

$$
{\int }_{-\infty }^{+\infty }p\left( x\right) \mathrm{d}x = {\int }_{-1}^{1}\frac{A}{\sqrt{1 - {x}^{2}}}\mathrm{\;d}x = {\left. A\arcsin x\right| }_{-1}^{1} = A\left( {\frac{\pi }{2} + \frac{\pi }{2}}\right)  = 1
$$

由此得 $A = \frac{1}{\pi }$

(2) $P\left\{  {-\frac{1}{2} < X < \frac{1}{2}}\right\}   = {\int }_{-\frac{1}{2}}^{\frac{1}{2}}\frac{1}{\pi }\frac{1}{\sqrt{1 - {x}^{2}}}\mathrm{\;d}x = {\left. \frac{1}{\pi }\arcsin x\right| }_{-\frac{1}{2}}^{\frac{1}{2}} = \frac{1}{3}$

(3)设 $X$ 的分布函数为 $F\left( x\right)$,当 $x \leq   - 1$ 时

$$
F\left( x\right)  = P\{ X \leq  x\}  = {\int }_{-\infty }^{x}p\left( t\right) \mathrm{d}t = {\int }_{-\infty }^{x}0\mathrm{\;d}t = 0
$$

当 $- 1 < x \leq  1$ 时,

$$
F\left( x\right)  = P\{ X \leq  x\}  = P\{ X \leq   - 1\}  + P\{  - 1 < X \leq  x\}
$$

$$
= {\int }_{-\infty }^{-1}0\mathrm{\;d}t + {\int }_{-1}^{x}\frac{1}{\pi \sqrt{1 - {t}^{2}}}\mathrm{\;d}t = \frac{1}{2} + \frac{1}{\pi }\arcsin x
$$

当 $x > 1$ 时,

$$
F\left( x\right)  = P\{ X \leq  x\}  = P\{ X \leq   - 1\}  + P\{  - 1 < X \leq  1\}  + P\{ 1 < X \leq  x\}
$$

$$
= {\int }_{-\infty }^{-1}0\mathrm{\;d}t + {\int }_{-1}^{1}\frac{1}{\pi \sqrt{1 - {t}^{2}}}\mathrm{\;d}t + {\int }_{1}^{x}0\mathrm{\;d}t = 1
$$

综合起来, 得

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x \leq   - 1 \\  \frac{1}{2} + \frac{1}{\pi }\arcsin x, &  - 1 < x \leq  1 \\  1, & x > 1 \end{array}\right.
$$

【5.16】设随机变量 $X$ 的密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} {cx}, & 0 \leq  x \leq  1 \\  0, & \text{ 其他 } \end{array}\right.
$$

求 (1) 常数 $c$;

(2) $P\{ {0.3} < X < {0.7}\}$;

(3) 常数 $a$,使 $P\{ X > a\}  = P\{ X < a\}$;

(4) $X$ 的分布函数 $F\left( x\right)$.

解 (1) 由性质 ${\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = {\int }_{0}^{1}{cx}\mathrm{\;d}x = \frac{c}{2} = 1$,可得 $c = 2$.

(2) $P\{ {0.3} < X < {0.7}\}  = {\int }_{0.3}^{0.7}f\left( x\right) \mathrm{d}x = {\int }_{0.3}^{0.7}{2x}\mathrm{\;d}x = {\left. {x}^{2}\right| }_{0.3}^{0.7} = {0.4}$.

(3) 因为 $P\{ X > a\}  + P\{ X < a\}  = 1\;\left( {P\{ X = a\}  = 0}\right)$,

而 $P\{ X > a\}  = P\{ X < a\}$,

故 $P\{ X > a\}  = P\{ X < a\}  = \frac{1}{2}$,

即 ${\int }_{-\infty }^{a}f\left( x\right) \mathrm{d}x = {\int }_{0}^{a}{2x}\mathrm{\;d}x = {a}^{2} = \frac{1}{2}$,得 $a = \frac{1}{\sqrt{2}}$.

(4) $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t$

$$
= \left\{  \begin{array}{ll} 0, & x < 0 \\  {\int }_{0}^{x}{2t}\mathrm{\;d}t, & 0 \leq  x < 1 \\  1, & x \geq  1 \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} 0, & x < 0 \\  {x}^{2}, & 0 \leq  x < 1 \\  1, & x \geq  1 \end{array}\right.
$$

【5.17】进行某种试验,成功的概率为 $\frac{3}{4}$,失败的概率为 $\frac{1}{4}$. 以 $X$ 表示直到试验首次成功时所需试验的次数,写出 $X$ 的概率分布并求 $X$ 取偶数的概率.

解 由题意可知, $X \sim  G\left( \frac{3}{4}\right)$,故 $X$ 的分布律为

$$
P\{ X = k\}  = \frac{3}{4}{\left( \frac{1}{4}\right) }^{k - 1}, k = 1,2,\cdots.
$$

$$
P\{ X = \text{ 偶数 }\}  = \frac{3}{4} \cdot  \frac{1}{4} + \frac{3}{4}{\left( \frac{1}{4}\right) }^{3} + \frac{3}{4}{\left( \frac{1}{4}\right) }^{5} + \cdots  = \frac{3}{4} \cdot  \frac{\frac{1}{4}}{1 - \frac{1}{16}} = \frac{1}{5}
$$

#### 题型3: 求随机变量或随机变量函数的分布

【5.18】假设随机变量 $X$ 的绝对值不大于 $1;P\{ X =  - 1\}  = \frac{1}{8}, P\{ X = 1\}  = \frac{1}{4}$; 在事件 $\{  - 1 < X < 1\}$ 出现的条件下, $X$ 在 $\left( {-1,1}\right)$ 内任一子区间上取值的条件概率与该子区间长度成正比. 试求 $X$ 的分布函数 $F\left( x\right)  = P\{ X \leq  x\}$.

分析 本题是求随机变量的分布函数问题, 熟练掌握事件概率与分布函数的关系是关键, 首先要求出随机变量在 $\left( {-1,1}\right)$ 上的条件概率.

解 由已知条件,当 $x <  - 1$ 时, $F\left( x\right)  = 0$; 且有 $F\left( {-1}\right)  = \frac{1}{8}$.

在 $x \geq  1$ 时, $F\left( x\right)  = 1$,且有

$$
P\{  - 1 < X < 1\}  = 1 - P\{ X =  - 1\}  - P\{ X = 1\}  = 1 - \frac{1}{4} - \frac{1}{8} = \frac{5}{8}
$$

在 $- 1 < x < 1$ 时, $F\left( x\right)  = P\{ X \leq  x\}  = P\{ X \leq   - 1\}  + P\{  - 1 < X \leq  x\}$,因为,

$$
P\{  - 1 < X \leq  x\}  = P\{  - 1 < X \leq  x, - 1 < X < 1\},
$$

由条件概率运算得

$$
P\{  - 1 < X \leq  x\}  = P\{  - 1 < X < 1\} P\{  - 1 < X \leq  x \mid   - 1 < X < 1\}
$$

$$
= \frac{5}{8} \cdot  \frac{x + 1}{2} = \frac{{5x} + 5}{16}
$$

故 $F\left( x\right)  = F\left( {-1}\right)  + P\{  - 1 < X \leq  x\}  = \frac{{5x} + 7}{16}$

从而得 $X$ 的分布函数 $F\left( x\right)  = \left\{  \begin{matrix} 0, & x <  - 1 \\  \frac{{5x} + 7}{16}, &  - 1 \leq  x < 1 \\  1, & x \geq  1 \end{matrix}\right.$ 电 66

【5.19】测量一圆形物体的半径, 其分布列为

<table><tr><td>$R$</td><td>10</td><td>11</td><td>12</td><td>13</td></tr><tr><td>$P$</td><td>0.1</td><td>0.4</td><td>0.3</td><td>0.2</td></tr></table>

求圆周长 $X$ 和圆面积 $Y$ 的分布列.

解 显然周长 $X = {2\pi R}$ 和面积 $Y = \pi {R}^{2}$ 均为随机变量 $R$ 的函数,且易看出 $X, Y$ 的取值分别全不相等,因而其分布列分别为:

<table><tr><td>$X$</td><td>20π</td><td>22π</td><td>${24\pi }$</td><td>${26\pi }$</td></tr><tr><td>$P$</td><td>0.1</td><td>0.4</td><td>0.3</td><td>0.2</td></tr><tr><td>$Y$</td><td>${100\pi }$</td><td>121π</td><td>${144\pi }$</td><td>169π</td></tr><tr><td>$P$</td><td>0.1</td><td>0.4</td><td>0.3</td><td>0.2</td></tr></table>

【5.20】假设随机变量 $X$ 的概率密度为 $f\left( x\right)  = \left\{  \begin{array}{ll} {2x}, & \text{ 若 }0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right.$,现在对 $X$ 进行 $n$ 次独立重复观测,以 ${V}_{n}$ 表示观测值不大于 0.1 的次数. 试求随机变量 ${V}_{n}$ 的概率分布.

解 事件“观测值不大于 0.1”,即事件 $\{ X \leq  {0.1}\}$ 的概率为

$$
p = P\{ X \leq  {0.1}\}  = {\int }_{-\infty }^{0.1}f\left( x\right) \mathrm{d}x = 2{\int }_{0}^{0.1}x\mathrm{\;d}x = {0.01}
$$

每次观测所得观测值不大于 0.1 为成功,则 ${V}_{n}$ 作为 $n$ 次独立重复试验成功的次数,服从参数为 $\left( {n,{0.01}}\right)$ 的二项分布

$$
P\left\{  {{V}_{n} = m}\right\}   = {C}_{n}^{m}{\left( {0.01}\right) }^{m}{\left( {0.99}\right) }^{n - m}\;\left( {m = 0,1,2,\cdots, n}\right)
$$

【5.21】已知随机变量 $X$ 的分布律如下:

<table><tr><td>$X$</td><td>-2</td><td>-1</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>$P$</td><td>${4a}$</td><td>$\frac{1}{12}$</td><td>${3a}$</td><td>$a$</td><td>10a</td><td>${4a}$</td></tr></table>

$Y = {X}^{2}$,则 $Y$ 的分布律为_____.

解 $Y$ 的分布律可表示为

<table><tr><td>Y</td><td>0</td><td>1</td><td>4</td><td>9</td></tr><tr><td>$P$</td><td>${3a}$</td><td>$\frac{1}{12} + a$</td><td>14a</td><td>${4a}$</td></tr></table>

由性质确定 $a = \frac{1}{24}$

则 $Y$ 的分布律为

<table><tr><td>Y</td><td>0</td><td>1</td><td>4</td><td>9</td></tr><tr><td>$P$</td><td>$\frac{1}{8}$</td><td>$\frac{1}{8}$</td><td>$\frac{7}{12}$</td><td>$\frac{1}{6}$</td></tr></table>

【5.22】设有随机变量 $X \sim  \left\lbrack  \begin{matrix}  - 1 & 0 & 1 \\  \frac{1}{3} & \frac{1}{6} & \frac{1}{2} \end{matrix}\right\rbrack$,则 $X$ 的分布函数为_____.

解 当 $x <  - 1$ 时, $F\left( x\right)  = P\{ X \leq  x\}  = 0$

当 $- 1 \leq  x < 0$ 时, $F\left( x\right)  = P\{ X \leq  x\}  = \frac{1}{3}$

当 $0 \leq  x < 1$ 时, $F\left( x\right)  = P\{ X \leq  x\}  = \frac{1}{3} + \frac{1}{6} = \frac{1}{2}$

当 $x \geq  1$ 时, $F\left( x\right)  = P\{ X \leq  x\}  = \frac{1}{3} + \frac{1}{6} + \frac{1}{2} = 1$

故 $F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x <  - 1 \\  \frac{1}{3}, &  - 1 \leq  x < 0 \\  \frac{1}{2}, & 0 \leq  x < 1 \\  1, & x > 1 \end{array}\right.$

【5.23】一房间有 3 扇同样大小的窗子,其中只有一扇是打开的. 有一只鸟自开着的窗子飞入了房间,它只能从开着的窗子飞出去. 鸟在房子里飞来飞去,试图飞出房间. 假定鸟是没有记忆的, 鸟飞向各扇窗子是随机的.

(1)以 $X$ 表示鸟为了飞出房间试飞的次数,求 $X$ 的分布律.

(2)户主声称,他养的一只鸟是有记忆的,它飞向任一窗子的尝试不多于一次. 以 $Y$ 表示这只聪明的鸟为了飞出房间试飞的次数,如户主所说是确定的,试求 $Y$ 的分布律.

解 (1) $X$ 的可能取值为 $1,2,3,\cdots, X$ 服从几何分布,故 $X$ 的分布律为

$$
P\{ X = k\}  = {\left( \frac{2}{3}\right) }^{k - 1} \cdot  \frac{1}{3},\;k = 1,2,\cdots
$$

或者

<table><tr><td>$X$</td><td>1</td><td>2</td><td>3</td><td>...</td></tr><tr><td>$P$</td><td>$\frac{1}{3}$</td><td>$\frac{2}{3} \times  \frac{1}{3}$</td><td>$\left( \frac{2}{3}\right)$$\times  \frac{1}{3}$</td><td>...</td></tr></table>

(2) $Y$ 的可能取值为1,2,3.

则由题意有 $Y$ 的分布律为

<table><tr><td>Y1</td><td>2</td><td>3</td></tr><tr><td>$P$$\frac{1}{3}$</td><td>$\frac{1}{3}$</td><td>$\frac{1}{3}$</td></tr></table>

【5.24】设随机变量 $X$ 的概率分布为 $P\{ X = 1\}  = P\{ X = 2\}  = \frac{1}{2}$. 在给定 $X = i$ 的条件下,随机变量 $Y$ 服从均匀分布 $U\left( {0, i}\right) \left( {i = 1,2}\right)$. 求 $Y$ 的分布函数 ${F}_{Y}\left( y\right)$ 和概率密度 ${f}_{Y}\left( y\right)$.

解 ${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}$

$$
= P\{ X = 1\} P\{ Y \leq  y \mid  X = 1\}  + P\{ X = 2\} P\{ Y \leq  y \mid  X = 2\}
$$

$= \frac{1}{2}P\{ Y \leq  y \mid  X = 1\}  + \frac{1}{2}P\{ Y \leq  y \mid  X = 2\}.$

当 $y < 0$ 时, ${F}_{Y}\left( y\right)  = 0$;

当 $0 \leq  y < 1$ 时, ${F}_{Y}\left( y\right)  = \frac{3y}{4}$;

当 $1 \leq  y < 2$ 时, ${F}_{Y}\left( y\right)  = \frac{1}{2} + \frac{y}{4}$;

当 $y \geq  2$ 时, ${F}_{Y}\left( y\right)  = 1$.

所以 $Y$ 的分布函数为

$$
{F}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} 0, & y < 0, \\  \frac{3y}{4}, & 0 \leq  y < 1, \\  \frac{1}{2} + \frac{y}{4}, & 1 \leq  y < 2, \\  1, & y \geq  2. \end{array}\right.
$$

随机变量 $Y$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{3}{4}, & 0 < y < 1, \\  \frac{1}{4}, & 1 \leq  y < 2, \\  0, & \text{ 其他 } \end{array}\right.
$$

点评 本题方法不难但过程复杂,求 ${F}_{Y}\left( y\right)$ 的关键在于全概率公式的使用,另外各种情形的讨论力求全面细致, 利用均匀分布求概率时要注意范围.

【5.25】设随机变量 $X$ 的概率密度为

( 1 ) $f\left( x\right)  = \left\{  \begin{array}{ll} 2\left( {1 - \frac{1}{{x}^{2}}}\right), & 1 \leq  x \leq  2 \\  0, & \text{ 其他 } \end{array}\right.$ (2) $f\left( x\right)  = \left\{  \begin{array}{ll} x, & 0 \leq  x < 1 \\  2 - x, & 1 \leq  x < 2 \\  0, & \text{ 其他 } \end{array}\right.$

求 $X$ 的分布函数 $F\left( x\right)$.

解 (1) 当 $x < 1$ 时, $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t = 0$

当 $1 \leq  x < 2$ 时, $F\left( x\right)  = {\int }_{1}^{x}2\left( {1 - \frac{1}{{t}^{2}}}\right) \mathrm{d}t = {2x} + \frac{2}{x} - 4$

当 $x \geq  2$ 时, $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t = {\int }_{1}^{2}2\left( {1 - \frac{1}{{x}^{2}}}\right) \mathrm{d}x = 1$

故 $X$ 的分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 1 \\  {2x} + \frac{2}{x} - 4, & 1 \leq  x < 2 \\  1, & x \geq  2 \end{array}\right.
$$

(2)当 $x < 0$ 时, $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t = 0$

当 $0 \leq  x < 1$ 时, $F\left( x\right)  = {\int }_{0}^{x}t\mathrm{\;d}t = \frac{{x}^{2}}{2}$

当 $1 \leq  x < 2$ 时, $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t = {\int }_{0}^{1}t\mathrm{\;d}t - {\int }_{1}^{x}\left( {2 - t}\right) \mathrm{d}t =  - \frac{{x}^{2}}{2} + {2x} - 1$

当 $x \geq  2$ 时, $F\left( x\right)  = {\int }_{-\infty }^{x}f\left( t\right) \mathrm{d}t = {\int }_{0}^{1}x\mathrm{\;d}x + {\int }_{1}^{2}\left( {2 - x}\right) \mathrm{d}x = 1$

故得 $X$ 的分布函数为

$$
F\left( x\right)  = \left\{  \begin{array}{ll} 0, & x < 0 \\  \frac{{x}^{2}}{2}, & 0 \leq  x < 1 \\   - \frac{{x}^{2}}{2} + {2x} - 1, & 1 \leq  x < 2 \\  1, & x \geq  2 \end{array}\right.
$$

【5.26】设随机变量 $\xi$ 的分布函数为 $F\left( x\right)  = A + B\arctan x\;\left( {-\infty  < x < \infty }\right)$. 试求:

(1)系数 $A$ 与 $B$;(2) $\xi$ 落在 $\left( {-1,1}\right)$ 内的概率；(3) $\xi$ 的分布密度.

解 (1) 由于 $F\left( {-\infty }\right)  = 0, F\left( {+\infty }\right)  = 1$,可知

$$
\left\{  {\begin{array}{l} A + B\left( {-\frac{\pi }{2}}\right)  = 0 \\  A + B\left( \frac{\pi }{2}\right)  = 1 \end{array} \Rightarrow  A = \frac{1}{2}, B = \frac{1}{\pi }}\right.
$$

于是 $F\left( x\right)  = \frac{1}{2} + \frac{1}{\pi }\arctan x.\;\left( {-\infty  < x <  + \infty }\right)$

(2) $P\{  - 1 < \xi  < 1\}  = F\left( 1\right)  - F\left( {-1}\right)  = \left( {\frac{1}{2} + \frac{1}{\pi }\arctan 1}\right)  - \left( {\frac{1}{2} + \frac{1}{\pi }\arctan \left( {-1}\right) }\right)$

$$
= \frac{1}{2} + \frac{1}{\pi } \times  \frac{\pi }{4} - \frac{1}{2} - \frac{1}{\pi }\left( {-\frac{\pi }{4}}\right)  = \frac{1}{2}
$$

(3) $\varphi \left( x\right)  = {F}^{\prime }\left( x\right)  = {\left( \frac{1}{2} + \frac{1}{\pi }\arctan x\right) }^{\prime } = \frac{1}{\pi \left( {1 + {x}^{2}}\right) }.\;\left( {-\infty  < x <  + \infty }\right)$

【5.27】设随机变量 $X$ 在 $\left( {0,1}\right)$ 服从均匀分布.

(1)求 $Y = {\mathrm{e}}^{X}$ 的概率密度； (2)求 $Y =  - 2\ln X$ 的概率密度.

解 由题设知, $X$ 的概率密度为 ${f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} 1, & 0 < x < 1 \\  0, & \text{ 其他 } \end{array}\right.$

(1) ${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = P\left\{  {{\mathrm{e}}^{X} \leq  y}\right\}   = P\{ X \leq  \ln y\}  = {\int }_{0}^{\ln y}{f}_{X}\left( x\right) \mathrm{d}x = {\int }_{0}^{\ln y}\mathrm{\;d}x$

故 ${f}_{Y}\left( y\right)  = {F}_{Y}{}^{\prime }\left( y\right)  = \frac{1}{y},0 < \ln y < 1$,所以 ${f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{y}, & 1 < y < \mathrm{e} \\  0, & \text{ 其他 } \end{array}\right.$

( 2 )由 $y =  - 2\ln x$ 得 $x = h\left( y\right)  = {\mathrm{e}}^{-\frac{y}{2}},{h}^{\prime }\left( y\right)  =  - \frac{1}{2}{\mathrm{e}}^{-\frac{y}{2}}$,由定理得 $Y =  - 2\ln X$ 的概率密度为

$$
{f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{2}{\mathrm{e}}^{-\frac{y}{2}}, & y > 0 \\  0, & y \leq  0 \end{array}\right.
$$

或由 $Y =  - 2\ln X$ 知, $Y$ 的取值必为非负,故当 $y \leq  0$ 时, $\{ Y \leq  y\}$ 是不可能事件,所以

$$
{F}_{Y}\left( y\right)  = P\{ Y \leq  y\}  = 0,\;{f}_{Y}\left( y\right)  = 0
$$

当 $y > 0$ 时,

$$
{F}_{Y}\left( x\right)  = P\{ Y \leq  y\}  = P\{  - 2\ln X \leq  y\}  = P\left\{  {\ln X \geq   - \frac{y}{2}}\right\}   = P\left\{  {X \geq  {\mathrm{e}}^{-\frac{y}{2}}}\right\}
$$

$$
= {\int }_{{\mathrm{e}}^{-\frac{y}{2}}}^{1}{f}_{X}\left( x\right) \mathrm{d}x = {\int }_{{\mathrm{e}}^{-\frac{y}{2}}}^{1}\mathrm{\;d}x =  - {\int }_{1}^{{\mathrm{e}}^{-\frac{y}{2}}}\mathrm{\;d}x
$$

从而 ${f}_{Y}\left( y\right)  = {F}_{Y}{}^{\prime }\left( y\right)  = \frac{1}{2}{\mathrm{e}}^{-\frac{y}{2}}$

故 ${f}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} \frac{1}{2}{\mathrm{e}}^{-\frac{y}{2}}, & y > 0 \\  0, & y \leq  0 \end{array}\right.$

【5.28】设随机变量 $X$ 的概率密度为

$$
f\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{9}{x}^{2}, & 0 < x < 3, \\  0, & \text{ 其他. } \end{array}\right.
$$

令随机变量 $Y = \left\{  \begin{array}{ll} 2, & X \leq  1, \\  X, & 1 < X < 2, \\  1, & X \geq  2. \end{array}\right.$

(1)求 $Y$ 的分布函数；

(2)求概率 $P\{ X \leq  Y\}$.

解 (1) 因为 $1 \leq  Y \leq  2$,故

${F}_{Y}\left( y\right)  = P\{ Y \leq  y\}$

当 $y < 1$ 时, ${F}_{Y}\left( y\right)  = 0$,

当 $y \geq  2$ 时, ${F}_{Y}\left( y\right)  = 1$,

当 $1 \leq  y < 2$ 时,

${F}_{Y}\left( y\right)  = P\{ Y = 1\}  + P\{ 1 < Y \leq  y\}  = P\{ X \geq  2\}  + P\{ 1 < X \leq  y\}$

$= {\int }_{2}^{3}\frac{1}{9}{x}^{2}\mathrm{\;d}x + {\int }_{1}^{y}\frac{1}{9}{x}^{2}\mathrm{\;d}x$

$= \frac{{y}^{3} + {18}}{27}$.

所以 ${F}_{Y}\left( y\right)  = \left\{  \begin{array}{ll} 0, & y < 1, \\  \frac{{y}^{3} + {18}}{27}, & 1 \leq  y < 2, \\  1, & y \geq  2. \end{array}\right.$

(2) $P\{ X \leq  Y\}  = P\{ X < 2\}  = {\int }_{0}^{2}\frac{1}{9}{x}^{2}\mathrm{\;d}x = \frac{8}{27}$.

【5.29】设随机变量 $X$ 的概率密度为 $f\left( x\right)  = \left\{  \begin{matrix} \frac{1}{3\sqrt[3]{{x}^{2}}}, & \text{ 若 }x \in  \left\lbrack  {1,8}\right\rbrack  \\  0, & \text{ 其他 } \end{matrix}\right.$, $F\left( x\right)$ 是 $X$ 的分布函数. 求随机变量 $Y = F\left( X\right)$ 的分布函数.

分析 随机变量函数 $Y = F\left( X\right)$ 隐含的条件是: 因为 $F\left( x\right)$ 是 $X$ 的分布函数的表达式,故 $Y$ 的值域为 $\left\lbrack  {0,1}\right\rbrack$.

解 当 $x < 1$ 时, $F\left( x\right)  = 0$; 当 $x > 8$ 时,有 $F\left( x\right)  = 1$; 当 $x \in  \left\lbrack  {1,8}\right\rbrack$ 时,

$$
F\left( x\right)  = {\int }_{1}^{x}\frac{1}{3\sqrt[3]{{t}^{2}}}\mathrm{\;d}t = \sqrt[3]{x} - 1.
$$

令 $G\left( y\right)$ 为 $Y = F\left( X\right)$ 的分布函数.

当 $y \leq  0$ 时, $G\left( y\right)  = 0$; 当 $y \geq  1$ 时, $G\left( y\right)  = 1$; 当 $y \in  \left( {0,1}\right)$ 时,

$$
G\left( y\right)  = P\{ Y \leq  y\}  = P\{ F\left( X\right)  \leq  y\}  = P\{ \sqrt[3]{X} - 1 \leq  y\}
$$

$$
= P\left\{  {X \leq  {\left( y + 1\right) }^{3}}\right\}   = F\left( {\left( y + 1\right) }^{3}\right)  = y.
$$

因此 $Y = F\left( X\right)$ 的分布函数为 $G\left( y\right)  = \left\{  \begin{array}{ll} 0, & y < 0 \\  y, & 0 \leq  y < 1 \\  1, & y \geq  1 \end{array}\right.$

点评 本题也可以不求 $F\left( x\right)$ 的具体表达式.

因为 $Y = F\left( X\right)$ 的分布函数为 $G\left( y\right)  = P\{ Y \leq  y\}  = P\{ F\left( X\right)  \leq  y\}$,注意到 $F\left( x\right)$ 为分布函数,于是 $0 \leq  F\left( x\right)  \leq  1$,因此当 $y < 0$ 时, $G\left( y\right)  = 0$; 当 $y \geq  1$ 时, $G\left( y\right)  = 1$;

当 $0 \leq  y < 1$ 时,因为 $F\left( x\right)$ 为单调增加函数,故

$$
G\left( y\right)  = P\{ Y \leq  y\}  = P\{ F\left( X\right)  \leq  y\}  = P\left\{  {X \leq  {F}^{-1}\left( y\right) }\right\}   = F\left\lbrack  {{F}^{-1}\left( y\right) }\right\rbrack   = y.
$$

则

$$
G\left( y\right)  = \left\{  \begin{array}{ll} 0, & y < 0 \\  y, & 0 \leq  y < 1 \\  1, & y \geq  1 \end{array}\right.
$$

实际上, $Y = F\left( X\right)$ 的分布与 $X$ 服从什么分布无关.

结论: 若连续型随机变量 $X$ 的分布函数是 $F\left( x\right)$,则 $Y = F\left( X\right)$ 服从 $\left( {0,1}\right)$ 上的均匀分布.

【5.30】设随机变量 $X$ 服从参数为 2 的指数分布,证明 $Y = 1 - {\mathrm{e}}^{-{2X}}$ 在区间 $\left( {0,1}\right)$ 上服从均匀分布.

证 $X$ 的分布函数 $F\left( x\right)  = \left\{  {\begin{array}{ll} 1 - {\mathrm{e}}^{-{2x}}, & x > 0 \\  0, & x \leq  0 \end{array}, y = 1 - {\mathrm{e}}^{-{2x}}}\right.$ 是单调增函数,其反函数为 $x =  - \frac{\ln \left( {1 - y}\right) }{2}$

设 $G\left( y\right)$ 是 $Y$ 的分布函数,则

$$
G\left( y\right)  = P\{ Y \leq  y\}  = P\left\{  {1 - {\mathrm{e}}^{-{2X}} \leq  y}\right\}   = \left\{  \begin{array}{ll} 0, & y \leq  0 \\  P\left\{  {X \leq   - \frac{1}{2}\ln \left( {1 - y}\right) }\right\} , & 0 < y < 1 \\  1, & y \geq  1 \end{array}\right.
$$

$$
= \left\{  \begin{array}{ll} 0, & y \leq  0 \\  y, & 0 < y < 1 \\  1, & y \geq  1 \end{array}\right.
$$


于是, $Y$ 在 $\left( {0,1}\right)$ 服从均匀分布.

#### 题型 4 : 关于重要分布

【5.31】设事件 $A$ 在每一次试验中发生的概率为 0.3,当 $A$ 发生不少于 3 次时,指示灯发出信号. (1)进行了 5 次独立试验,求指示灯发出信号的概率； (2)进行了 7 次独立试验,求指示灯发出信号的概率. 解 记 $A$ 发生的次数为 $X$,则 $X \sim  B\left( {n,{0.3}}\right), n = 5,7$. 记 $B$ 为指示灯发出信号. (1) $P\left( B\right)  = P\{ X \geq  3\}  = \mathop{\sum }\limits_{{k = 3}}^{5}{C}_{5}^{k}{\left( {0.3}\right) }^{k}{\left( {0.7}\right) }^{5 - k} \approx  {0.163}$,或

$$
P\left( B\right)  = 1 - \mathop{\sum }\limits_{{k = 0}}^{2}P\{ X = k\}
$$

$$
= 1 - {\left( {0.7}\right) }^{5} - {C}_{5}^{1}\left( {0.3}\right) {\left( {0.7}\right) }^{4} - {C}_{5}^{2}{\left( {0.3}\right) }^{2}{\left( {0.7}\right) }^{3} \approx  {0.163}
$$

(2) $P\left( B\right)  = \mathop{\sum }\limits_{{k = 3}}^{7}P\{ X = k\}  = \mathop{\sum }\limits_{{k = 3}}^{7}{C}_{7}^{k}{\left( {0.3}\right) }^{k}{\left( {0.7}\right) }^{7 - k} \approx  {0.353}$,或

$$
P\left( B\right)  = 1 - \mathop{\sum }\limits_{{k = 0}}^{2}P\{ X = k\}  = 1 - {\left( {0.7}\right) }^{7} - {C}_{7}^{1}\left( {0.3}\right) {\left( {0.7}\right) }^{6} - {C}_{7}^{2}{\left( {0.3}\right) }^{2}{\left( {0.7}\right) }^{5} \approx  {0.353}
$$

【5.32】某批零件的次品率为 0.1, 从这批零件中任取 20 件,求:

(1)恰有 3 件次品的概率;

(2)至少有 3 件次品的概率；

(3)次品数的最可能值.

解 设次品数为 $X$,则 $X \sim  B\left( {{20},{0.1}}\right)$,由二项分布的分布律可知:

(1) $P\{ X = 3\}  = {C}_{20}^{3} \cdot  {0.1}^{3} \cdot  {0.9}^{17} = {0.19}$.

(2) $P\{ X \geq  3\}  = 1 - P\{ X = 0\}  - P\{ X = 1\}  - P\{ X = 2\}$

$$
= 1 - {0.9}^{20} - {C}_{20}^{1} \cdot  {0.1}^{1} \cdot  {0.9}^{19} - {C}_{20}^{2} \cdot  {0.1}^{2} \cdot  {0.9}^{18}
$$

$$
= {0.3231}\text{.}
$$

(3)次品数的最可能值为 $\left\lbrack  {\left( {n + 1}\right) p}\right\rbrack   = 2$.

【5.33】设随机变量 $X$ 服从几何分布,证明

$$
P\{ X = n + k \mid  X > n\}  = P\{ X = k\},\;\left( {n \geq  1, k = 1,2,\cdots }\right)
$$

证 $P\{ X = k\}  = p{q}^{k - 1}.\left( {k = 1,2,\cdots;q = 1 - p}\right)$

$$
P\{ X = n + k \mid  X > n\}  = \frac{P\{ X = n + k\} }{P\{ X > n\} } = \frac{p{q}^{n + k - 1}}{\mathop{\sum }\limits_{{k = n + 1}}^{\infty }p{q}^{k - 1}} = p{q}^{k - 1}.
$$

故得证.

【5.34】一本 500 页的书, 共有 500 个错字, 每个错字等可能地出现在每一页上(每一页的印刷符号超过 500 个), 试求在给定的一页上至少有三个错字的概率.

解 500 个错字中的每一个在该页上的概率为 $p = \frac{1}{500}$. 设该页上的错字数为 $X$,则

$$
P\{ X = i\}  = {C}_{500}^{i}{p}^{i}{\left( 1 - p\right) }^{{500} - i},\;i = 0,1,2,\cdots,{500}
$$

概率论与数理统计习题精选精解

因 $n = {500}$ 较大,而 $p = \frac{1}{500}$ 较小,由泊松定理

$$
P\{ X = i\}  \approx  \frac{{\left( np\right) }^{i}}{i!}{\mathrm{e}}^{-{np}} = \frac{{\mathrm{e}}^{-1}}{i!},\;i = 1,2,\cdots
$$

$P\{$ 该页至少有三个错字 $\}  = 1 - P\{$ 该页上至多有三个错字 $\}$

$$
= 1 - \left\lbrack  {P\{ X = 0\}  + P\{ X = 1\}  + P\{ X = 2\} }\right\rbrack
$$

$$
\approx  1 - \left( {{\mathrm{e}}^{-1} + {\mathrm{e}}^{-1} + \frac{1}{2!}{\mathrm{e}}^{-1}}\right)  = 1 - \frac{5}{2}{\mathrm{e}}^{-1}.
$$

【5.35】现有 500 人检查身体,初步发现有 50 人患有某种病,从中任找出 10 人,求下列事件的概率:

(1)恰有 1 人患此病；

(2)最多有 1 人患此病；

(3)至少有 1 人患此病.

解 设任找的 10 人中患此病的人数为 $X$,据题意知 $X$ 服从超几何分布,有

$$
P\{ X = k\}  = \frac{{C}_{50}^{k}{C}_{450}^{{10} - k}}{{C}_{500}^{10}},\;k = 0,1,\cdots,{10}
$$

因为总数 $N$ 很大,而抽取个数 $n$ 相对较小,故可用二项分布近似代替超几何分布.

$$
P\{ X = k\}  \approx  {C}_{10}^{k}{\left( \frac{50}{500}\right) }^{k}{\left( \frac{450}{500}\right) }^{{10} - k} = {C}_{10}^{k} \cdot  {0.1}^{k} \cdot  {0.9}^{{10} - k}.
$$

(1) $P\{ X = 1\}  \approx  {10} \times  {0.1} \times  {0.9}^{9} \approx  {0.3874}$

(2) $P\{ X \leq  1\}  = P\{ X = 0\}  + P\{ X = 1\}  \approx  {0.9}^{10} + {0.3874} \approx  {0.7361}$

(3) $P\{ X \geq  1\}  = 1 - P\{ X < 1\}  = 1 - P\{ X = 0\}  = 1 - {0.9}^{10} \approx  {0.6513}$

【5.36】某地区一个月内发生交通事故的次数 $X$ 服从参数 $\lambda$ 的泊松分布,即 $X \sim  P\left( \lambda \right)$. 据统计资料知,一个月内发生 8 次交通事故的概率是发生 10 次事故概率的 2.5 倍.

(1)求 1 个月内发生 8 次、 10 次交通事故的概率；

(2)求 1 个月内至少发生 1 次交通事故的概率.

解 这是泊松分布的应用问题, $X \sim  P\left( \lambda \right), P\{ X = k\}  = \frac{{\lambda }^{k}{\mathrm{e}}^{-\lambda }}{k!}, k = 0,1,2,\cdots$ 这里 $\lambda$ 是未知的,关键是求出 $\lambda$.

根据题意有 $P\{ X = 8\}  = {2.5P}\{ X = {10}\}$,即 $\frac{{\lambda }^{8}{\mathrm{e}}^{-\lambda }}{8!} = {2.5} \times  \frac{{\lambda }^{10}{\mathrm{e}}^{-\lambda }}{{10}!}$

解出 ${\lambda }^{2} = {36},\lambda  = 6$

(1) $P\{ X = 8\}  = \frac{{6}^{8}{\mathrm{e}}^{-6}}{8!} \approx  {0.1033},\;P\{ X = {10}\}  = \frac{{6}^{10}{\mathrm{e}}^{-6}}{{10}!} \approx  {0.0413}$

(2) $P\{ X = 0\}  = {\mathrm{e}}^{-6} \approx  {0.00248},\;P\{ X \geq  1\}  = 1 - P\{ X = 0\}  \approx  1 - {0.00248} \approx  {0.9975}$.

【5.37】某单位招聘 155 人,按考试成绩录用,共有 526 人报名,假设报名者的考试成绩 $X \sim$ $N\left( {\mu,{\sigma }^{2}}\right)$. 已知 90 分以上的 12 人,60 分以下的 83 人,若从高分到低分依次录取,某人成绩为 78 分, 问此人能否被录取?

解 本题中只知成绩 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,但不知 $\mu,\sigma$ 的值是多少,所以必须首先想法求出 $\mu$ 和 $\sigma$. 根据已知条件有

$$
P\{ X > {90}\}  = \frac{12}{526} \approx  {0.0228},
$$

$$
P\{ X \leq  {90}\}  = 1 - P\{ X > {90}\}  \approx  1 - {0.0228} = {0.9772},
$$

又因为

$$
P\{ X \leq  {90}\} \overset{\text{ 标准化 }}{ = }P\left\{  {\frac{X - \mu }{\sigma } \leq  \frac{{90} - \mu }{\sigma }}\right\}   = \Phi \left( \frac{{90} - \mu }{\sigma }\right),
$$

所以

$$
\Phi \left( \frac{{90} - \mu }{\sigma }\right)  = {0.9772}.
$$

反查标准正态分布表得

$$
\frac{{90} - \mu }{\sigma } \approx  {2.0}
$$

①

又

$$
P\{ X < {60}\}  = \frac{83}{526} \approx  {0.1588},
$$

$$
P\{ X < {60}\} \overset{\text{ 标准化 }}{ = }P\left\{  {\frac{X - \mu }{\sigma } < \frac{{60} - \mu }{\sigma }}\right\}   = \Phi \left( \frac{{60} - \mu }{\sigma }\right),
$$

所以

$$
\Phi \left( \frac{{60} - \mu }{\sigma }\right)  \approx  {0.1588},\;\Phi \left( \frac{\mu  - {60}}{\sigma }\right)  \approx  1 - {0.1588} = {0.8412}.
$$

反查标准正态分布表得

$$
\frac{\mu  - {60}}{\sigma } \approx  {1.0},
$$

②

由 ①,② 联立解出 $\sigma  = {10},\mu  = {70}$. 所以

$$
X \sim  N\left( {{70},{10}^{2}}\right) \text{.}
$$

某人成绩 78 分,能否被录取,关键在于录取率. 已知录取率为 $\frac{155}{526} \approx  {0.2947}$. 看是否能被录取, 解法有二.

方法 1: 看 $P\{ X > {78}\}  =$ ?

$$
P\{ X > {78}\}  = 1 - P\{ X \leq  {78}\}  = 1 - P\left\{  {\frac{X - {70}}{10} \leq  \frac{{78} - {70}}{10}}\right\}   = 1 - P\left\{  {{X}^{ * } \leq  {0.8}}\right\}
$$

$$
= 1 - \Phi \left( {0.8}\right)  \approx  1 - {0.7881} = {0.2119}
$$

因为 ${0.2119} < {0.2947}$ (录取率),所以此人能被录取.

方法 2: 看录取分数限. 设被录用者的最低分为 ${x}_{0}$,则 $P\left\{  {X \geq  {x}_{0}}\right\}   = {0.2947}$ (录取率),

$$
P\left\{  {X \leq  {x}_{0}}\right\}   = 1 - P\left\{  {X > {x}_{0}}\right\}   \approx  1 - {0.2947} = {0.7053},
$$

而

$$
P\left\{  {X \leq  {x}_{0}}\right\}   = P\left\{  {\frac{X - {70}}{10} \leq  \frac{{x}_{0} - {70}}{10}}\right\}   = P\left\{  {{X}^{ * } \leq  \frac{{x}_{0} - {70}}{10}}\right\}   = \Phi \left( \frac{{x}_{0} - {70}}{10}\right),
$$

所以

$$
\Phi \left( \frac{{x}_{0} - {70}}{10}\right)  = {0.7053}.
$$

反查标准正态分布表得

$$
\frac{{x}_{0} - {70}}{10} \approx  {0.54}
$$

解出 ${x}_{0} = {75}$,某人成绩 78 分,在 75 分以上,所以能被录取.

【5.38】设随机变量 $X$ 服从正态分布 $N\left( {0,1}\right)$,对给定的 $\alpha \left( {0 < \alpha  < 1}\right)$,数 ${u}_{\alpha }$ 满足 $P\{ X >$ $\left. {u}_{\alpha }\right\}   = \alpha$. 若 $P\{ \left| X\right|  < x\}  = \alpha$,则 $x$ 等于 (   ).

(A) ${u}_{\frac{\alpha }{2}}$ (B) ${u}_{1 - \frac{\alpha }{2}}$ (C) $u\frac{1 - \alpha }{2}$ (D) ${u}_{1 - \alpha }$

解 由标准正态分布密度函数的对称性知

$1 - \alpha  = 1 - P\{ \left| X\right|  < x\}  = P\{ \left| X\right|  \geq  x\}  = P\{ X \geq  x\}  + P\{ X \leq   - x\}  = {2P}\{ X \geq  x\}.$ 即有 $P\{ X \geq  x\}  = \frac{1 - \alpha }{2}$,则 $x = u\frac{1 - \alpha }{2}$.

故应选(C).

点评 本题 ${u}_{a}$ 相当于上侧分位数,如图 2-5.38 所示.

![0195317d-ba2a-736d-8e6e-9afc1cf09b00_75_472_690_711_212_0.jpg](images/0195317d-ba2a-736d-8e6e-9afc1cf09b00_75_472_690_711_212_0.jpg)

图 2-5.38

【5.39】设随机变量 $X$ 与 $Y$ 均服从正态分布, $X \sim  N\left( {\mu,{4}^{2}}\right), Y \sim  N\left( {\mu,{5}^{2}}\right)$; 记 ${p}_{1} =$ $P\{ X \leq  \mu  - 4\},{p}_{2} = P\{ Y \geq  \mu  + 5\}$,则 (   ).

(A) 对任何实数 $\mu$,都有 ${p}_{1} = {p}_{2}$ (B) 对任何实数 $\mu$,都有 ${p}_{1} < {p}_{2}$

(C) 只对 $\mu$ 的个别值,才有 ${p}_{1} = {p}_{2}$ (D) 对任何实数 $\mu$,都有 ${p}_{1} > {p}_{2}$

解 由于 $\frac{X - \mu }{4} \sim  N\left( {0.1}\right),\frac{Y - \mu }{5} \sim  N\left( {0.1}\right)$,

所以

$$
{p}_{1} = P\left\{  {\frac{X - \mu }{4} \leq   - 1}\right\}   = \Phi \left( {-1}\right)  = 1 - \Phi \left( 1\right)
$$

$$
{p}_{2} = P\left\{  {\frac{Y - \mu }{5} \geq  1}\right\}   = 1 - \Phi \left( 1\right)
$$

故 ${p}_{1} = {p}_{2}$,而且与 $\mu$ 的取值无关.

故应选 (A).

【5.40】设 ${f}_{1}\left( x\right)$ 为标准正态分布的概率密度, ${f}_{2}\left( x\right)$ 为 $\left\lbrack  {-1,3}\right\rbrack$ 上均匀分布的概率密度,若

$$
f\left( x\right)  = \left\{  {\begin{array}{ll} a{f}_{1}\left( x\right), & x \leq  0, \\  b{f}_{2}\left( x\right), & x > 0 \end{array}\;\left( {a > 0, b > 0}\right) }\right.
$$

为概率密度,则 $a, b$ 应满足

(A) ${2a} + {3b} = 4$ (B) ${3a} + {2b} = 4$ (C) $a + b = 1$ (D) $a + b = 2$

解 由概率密度的性质: ${\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = 1$,而电 76

$$
{\int }_{-\infty }^{+\infty }f\left( x\right) \mathrm{d}x = a{\int }_{-\infty }^{0}{f}_{1}\left( x\right) \mathrm{d}x + b{\int }_{0}^{+\infty }{f}_{2}\left( x\right) \mathrm{d}x
$$

其中

$$
{\int }_{-\infty }^{0}{f}_{1}\left( x\right) \mathrm{d}x = \frac{1}{2}{\int }_{-\infty }^{+\infty }{f}_{1}\left( x\right) \mathrm{d}x = \frac{1}{2}\;\left( {{f}_{1}\left( x\right) }\right. \text{偶函数})
$$

$$
{\int }_{0}^{+\infty }{f}_{2}\left( x\right) \mathrm{d}x = {\int }_{0}^{3}\frac{1}{4}\mathrm{\;d}x = \frac{3}{4}\;\left( {{f}_{2}\left( x\right)  = \left\{  \begin{array}{ll} \frac{1}{4}, & x \in  \left\lbrack  {-1,3}\right\rbrack  \\  0, & \text{ 其他 } \end{array}\right) }\right.
$$

故 $\frac{a}{2} + \frac{3b}{4} = 1$ 即 ${2a} + {3b} = 4$.

故应选(A).

【5.41】设随机变量 $X$ 服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right) \left( {\sigma  > 0}\right)$,且二次方程 ${y}^{2} + {4y} + X = 0$ 无实根的概率为 $\frac{1}{2}$,则 $\mu  =$ _____.

解 二次方程 ${y}^{2} + {4y} + X = 0$ 无实根,则

$$
\Delta  = {4}^{2} - {4X} < 0,\;\text{ 即 }4 < X
$$

因为 $P\{ 4 < X\}  = \frac{1}{2}$

故 $\mu  = 4$

【5.42】设随机变量 $Y$ 服从参数为 1 的指数分布, $a$ 为常数且大于零,则 $P\{ Y \leq  a + 1 \mid  Y >$ $a\}  =$ _____.

解 因为 $Y$ 服从参数为 1 的指数分布,所以 $Y$ 的分布函数为:

$$
F\left( y\right)  = \left\{  {\begin{array}{ll} 1 - {\mathrm{e}}^{-y}, & y > 0 \\  0, & y \leq  0 \end{array},}\right.
$$

则

$$
P\{ Y \leq  a + 1 \mid  Y > a\}  = \frac{P\{ a < Y \leq  a + 1\} }{P\{ Y > a\} }
$$

$$
= \frac{P\{ a < Y \leq  a + 1\} }{1 - P\{ Y \leq  a\} } = \frac{F\left( {a + 1}\right)  - F\left( a\right) }{1 - F\left( a\right) }
$$

$$
= \frac{1 - {\mathrm{e}}^{-a - 1} - \left( {1 - {\mathrm{e}}^{-a}}\right) }{1 - \left( {1 - {\mathrm{e}}^{-a}}\right) } = 1 - {\mathrm{e}}^{-1}.
$$

点评 本题为条件概率, 先使用条件概率公式, 再利用指数分布的分布函数或概率密度求出相应的概率, 此为常规解法.

除此之外,本题也可以利用指数分布的性质一“无记忆性”:设 $Y \sim  E\left( \lambda \right)$,则

$P\{ Y > a + t \mid  Y > a\}  = P\{ Y > t\}.$

故 $P\{ Y \leq  a + 1 \mid  Y > a\}  = 1 - P\{ Y > a + 1 \mid  Y > a\}  = 1 - P\{ Y > 1\}  = P\{ Y \leq  1\}$ $= 1 - {\mathrm{e}}^{-1}$.

【5.43】设打一次电话所用时间 $X$ (分钟) 服从参数 $\lambda  = {0.1}$ 的指数分布. 如某人刚好在你前面走进电话间, 求你等待的时间:

(1)超过 10 分钟的概率；

(2)在 10 分钟到 20 分钟之间的概率.

解 因为 $X \sim  E\left( {0.1}\right)$,则 $f\left( x\right)  = \left\{  {\begin{matrix} \frac{1}{10}{\mathrm{e}}^{-\frac{x}{10}}, & x > 0 \\  0, & x \leq  0 \end{matrix}, F\left( x\right)  = \left\{  \begin{matrix} 1 - {\mathrm{e}}^{-\frac{x}{10}}, & x > 0 \\  0, & x \leq  0 \end{matrix}\right. }\right.$,故

(1) $P\{ X > {10}\}  = 1 - F\left( {10}\right) \;\left( {\text{或}{\int }_{10}^{+\infty }f\left( x\right) \mathrm{d}x}\right)  = {\mathrm{e}}^{-1}$;

(2) $P\{ {10} < X < {20}\}  = F\left( {20}\right)  - F\left( {10}\right) \;\left( {\text{或}{\int }_{10}^{20}f\left( x\right) \mathrm{d}x}\right)  = {\mathrm{e}}^{-1} - {\mathrm{e}}^{-2}$.

#### 题型 5 : 综合应用题

【5.44】设一大型设备在任何长为 $t$ 的时间内发生故障的次数 $N\left( t\right)$ 服从参数为 ${\lambda t}$ 的泊松分布.

(1)求在相继两次故障之间时间间隔 $T$ 的概率分布；

(2)求在设备已经无故障工作 8 小时的情况下,再无故障运行 8 小时的概率 $Q$.

解 (1) 由于 $T$ 是非负随机变量,可见

当 $t < 0$ 时, $F\left( t\right)  = P\{ T \leq  t\}  = 0$

设 $t \geq  0$ 时,则事件 $\{ T > t\}$ 与 $\{ N\left( t\right)  = 0\}$ 等价. 因此,当 $t \geq  0$ 时,有

$$
F\left( t\right)  = P\{ T \leq  t\}  = 1 - P\{ T > t\}  = 1 - P\{ N\left( t\right)  = 0\}  = 1 - {\mathrm{e}}^{-{\lambda t}}
$$

于是, $T$ 服从参数为 $\lambda$ 的指数分布.

$$
\text{(2)}Q = P\{ T \geq  {16} \mid  T \geq  8\}  = \frac{P\{ T \geq  {16}, T \geq  8\} }{P\{ T \geq  8\} } = \frac{P\{ T \geq  {16}\} }{P\{ T \geq  8\} } = \frac{{\mathrm{e}}^{-{16\lambda }}}{{\mathrm{e}}^{-{8\lambda }}} = {\mathrm{e}}^{-{8\lambda }}
$$

点评 本题第二问也可以利用指数分布的“无记忆性” 直接求 $Q$. 设 $X$ 服从指数分布,则 $P\{ X > s + t \mid  X > s\}  = P\{ X > t\}$,由此 $Q = P\{ T \geq  8\}  = {\mathrm{e}}^{-{8\lambda }}$.

-【5.45】假设测量的随机误差 $X \sim  N\left( {0,{10}^{2}}\right)$,试求在 100 次独立重复测量中,至少有三次测量误差的绝对值大于 19.6 的概率 $\alpha$,并利用泊松分布求出 $\alpha$ 的近似值(要求小数点后取两位有效数字).

解 设在 100 次测量中,有 $Y$ 次的测量误差的绝对值大于 19.6,则 $Y \sim  B\left( {{100}, p}\right)$. 其中

$$
p = P\{ \left| X\right|  > {19.6}\}  = 1 - P\{  - {19.6} \leq  X \leq  {19.6}\}
$$

$$
= 1 - \left\lbrack  {\Phi \left( {1.96}\right)  - \Phi \left( {-{1.96}}\right) }\right\rbrack   = 2 - {2\Phi }\left( {1.96}\right)  = 2 - 2 \times  {0.975} = {0.05}\text{.}
$$

故

$$
\alpha  = P\{ Y \geq  3\}  = \mathop{\sum }\limits_{{k = 3}}^{{100}}{C}_{100}^{k} \times  {0.05}^{k} \times  {0.95}^{{100} - k}
$$

若用泊松近似,则 $\lambda  = {100} \times  {0.05} = 5$,即 $Y \sim  B\left( {{100},{0.05}}\right)$ 近似于 $P\left( 5\right)$,故 $\alpha  \approx  {0.88}$.

【5.46】有一大批产品,其验收方案如下. 先作第一次检验:从中取 10 件,经检验无次品接受这批产品,次品数大于 2 拒收；否则作第二次检验,其做法是从中再任取 5 件,仅当 5 件中无次品时接受这批产品. 若产品的次品率为 10%, 求

(1)这批产品经第一次检验就能接受的概率；

(2)需作第二次检验的概率；

(3)这批产品按第二次检验的标准接受的概率；

(4)这批产品在第一次检验未能做决定且第二次检验时被通过的概率； 量 78

(5)这批产品被接受的概率.

解 第一次检验相当于 10 重伯努利试验. 设 $X$ 为第一次检验中次品数,则 $X \sim  B({10}$, 10%),第二次检验为 5 重伯努利试验. 设 $Y$ 为第二次检验中次品数,则 $Y \sim  B\left( {5,{10}\% }\right)$.

(1) $P\{ X = 0\}  = {C}_{10}^{0}{\left( {0.1}\right) }^{0} \times  {\left( {0.9}\right) }^{10} = {\left( {0.9}\right) }^{10} \approx  {0.349}$

(2) $P\{ 0 < X \leq  2\}  = P\{ X = 1\}  + P\{ X = 2\}  = {10} \times  {0.1} \times  {\left( {0.9}\right) }^{9} + \frac{{10} \times  9}{2} \times  {0.1}^{2} \times  {\left( {0.9}\right) }^{8}$

$$
\approx  {0.387} + {0.194} = {0.581}
$$

(3) $P\{ Y = 0\}  = {C}_{5}^{0}{\left( {0.1}\right) }^{0}{\left( {0.9}\right) }^{5} = {\left( {0.9}\right) }^{5} \approx  {0.590}$

(4) $P\{ 0 < X \leq  2, Y = 0\}  = P\{ 0 < X \leq  2\}  \cdot  P\{ Y = 0\}  \approx  {0.581} \times  {0.590} \approx  {0.343}$

(5) $P\{ X = 0\}  + P\{ 0 < X \leq  2, Y = 0\}  = {0.349} + {0.343} = {0.692}$.

【5.47】若每只母鸡产 $k$ 个蛋的概率服从参数为 $\lambda$ 的泊松分布,而每个蛋能孵化成小鸡的概率为 $p$. 试证: 每只母鸡有 $n$ 只小鸡的概率服从参数为 ${\lambda p}$ 的泊松分布.

证 设 $X = \{$ 蛋数 $\}, Y = \{$ 鸡数 $\}$. 由全概率公式,

$P\{ Y = n\}  = P\{ X = n\} P\{ Y = n \mid  X = n\}  + P\{ X = n + 1\} P\{ Y = n \mid  X = n + 1\}  + \cdots \cdots$

$$
= \frac{{\lambda }^{n}}{n!}{\mathrm{e}}^{-\lambda }{p}^{n} + \frac{{\lambda }^{n + 1}}{\left( {n + 1}\right) !}{\mathrm{e}}^{-\lambda }{C}_{n + 1}^{n}{p}^{n}q + \cdots \cdots
$$

$$
= \frac{{\left( \lambda p\right) }^{n}}{n!}{\mathrm{e}}^{-\lambda \left( {1 - q}\right) } = \frac{{\left( \lambda p\right) }^{n}}{n!}{\mathrm{e}}^{-{\lambda p}}
$$

所以 $Y \sim  P\left( {\lambda p}\right)$.

【5.48】设电源电压 $U \sim  N\left( {{220},{25}^{2}}\right)$ (单位: $\mathrm{V}$ ). 通常有 3 种状态:① 不超过 ${200}\mathrm{\;V}$; ② 在 ${200}\mathrm{\;V} \sim  {240}\mathrm{\;V}$ 之间; ③ 超过 ${240}\mathrm{\;V}$. 在上述三种状态下,某电子元件损坏的概率分别为 0.1, 0.001, 0.2.

(1)求电子元件损坏的概率 $\alpha$;

(2)在电子元件已损坏的情况下,试分析电压所处的状态.

解 (1) 设事件 ${A}_{1},{A}_{2},{A}_{3}$ 分别顺序表示题中所述电压的 3 种状态, $B$ 表示电子元件损坏, 则 $\alpha  = P\left( B\right)$. 根据全概率公式有

$$
P\left( B\right)  = \mathop{\sum }\limits_{{i = 1}}^{3}P\left( {A}_{i}\right) P\left( {B \mid  {A}_{i}}\right)
$$

据题意知, $P\left( {B \mid  {A}_{1}}\right)  = {0.1}, P\left( {B \mid  {A}_{2}}\right)  = {0.001}, P\left( {B \mid  {A}_{3}}\right)  = {0.2}$,下面求 $P\left( {A}_{i}\right) (i = 1$, $2,3)$,已知 $U \sim  N\left( {{220},{25}^{2}}\right)$,

$$
P\left( {A}_{1}\right)  = P\{ U \leq  {200}\} \text{ 标准化 }P\left\{  {\frac{U - {220}}{25} \leq  \frac{{200} - {220}}{25}}\right\}   = P\left\{  {{U}^{ * } \leq   - {0.8}}\right\}
$$

(其中 ${U}^{ * } \sim  N\left( {0.1}\right)$ )

$$
= \Phi \left( {-{0.8}}\right)  = 1 - \Phi \left( {0.8}\right) \text{(查表)} \approx  1 - {0.7881} = {0.2119}\text{.}
$$

考虑到正态分布的对称性, 有

$$
P\left( {A}_{3}\right)  = P\left( {A}_{1}\right)  \approx  {0.2119}
$$

由于 $\left( {{A}_{1},{A}_{2},{A}_{3}}\right)$ 是一个完备事件组,所以

$$
P\left( {A}_{1}\right)  + P\left( {A}_{2}\right)  + P\left( {A}_{3}\right)  = 1,
$$

$$
P\left( {A}_{2}\right)  = 1 - P\left( {A}_{1}\right)  - P\left( {A}_{3}\right)  = 1 - {2P}\left( {A}_{1}\right)  = 1 - 2 \times  {0.2119} = {0.5762}.
$$

故

$$
\alpha  = P\left( B\right)  = {0.2119} \times  {0.1} + {0.5762} \times  {0.001} + {0.2119} \times  {0.2} \approx  {0.0642}.
$$

(2) 考虑 $P\left( {{A}_{i} \mid  B}\right), i = 1,2,3$.

由贝叶斯公式 $P\left( {{A}_{i} \mid  B}\right)  = \frac{P\left( {A}_{i}\right) P\left( {B \mid  {A}_{i}}\right) }{P\left( B\right) }$,所以

$$
P\left( {{A}_{1} \mid  B}\right)  = \frac{P\left( {A}_{1}\right) P\left( {B \mid  {A}_{1}}\right) }{P\left( B\right) } \approx  \frac{{0.2119} \times  {0.1}}{0.0642} \approx  {0.330};
$$

$$
P\left( {{A}_{2} \mid  B}\right)  = \frac{P\left( {A}_{2}\right) P\left( {B \mid  {A}_{2}}\right) }{P\left( B\right) } \approx  \frac{{0.5762} \times  {0.001}}{0.0642} \approx  {0.009};
$$

$$
P\left( {{A}_{3} \mid  B}\right)  = \frac{P\left( {A}_{3}\right) P\left( {B \mid  {A}_{3}}\right) }{P\left( B\right) } \approx  \frac{{0.2119} \times  {0.2}}{0.0642} \approx  {0.660}.
$$

从上面的几个概率值看出, $P\left( {{A}_{3} \mid  B}\right)  \approx  {0.660}$ 是三者中的最大者,说明当电器损坏时,电压处在高压状态下的可能性最大; 而 $P\left( {{A}_{2} \mid  B}\right)  \approx  {0.009}$ 很小,说明当电器损坏时,电压处在中压 (200V 之间) 状态的可能性很小,几乎是不会的. 这符合实际.

【5.49】设某城市成年男子的身高 $X \sim  N\left( {{170},{6}^{2}}\right)$ (单位厘米).

(1)问应如何设计公共汽车车门的高度,使成年男子与车门顶碰头的机会小于 0.01？

(2)若车门设计高度为 182 厘米,求 10 个成年男子中与车门顶碰头的人数不多于 1 人的概率.

解 (1)设车门高度为 $l$ 厘米,按设计要求应有 $P\{ X > l\}  < {0.01}$. 由题设知 $X \sim  N({170}$, ${6}^{2}$ ),将其标准化后有

$$
\frac{X - {170}}{6} \sim  N\left( {0,1}\right),
$$

因此, 按设计要求有

$$
P\{ X > l\}  = 1 - P\{ X \leq  l\}  = 1 - P\left\{  {\frac{X - {170}}{6} \leq  \frac{l - {170}}{6}}\right\}   = 1 - \Phi \left( \frac{l - {170}}{6}\right)  < 0.
$$

01,

即 $\Phi \left( \frac{l - {170}}{6}\right)  > {0.99}$,查表得 $\frac{l - {170}}{6} > {2.33}$,故

$$
l > {183.98}\text{(厘米).}
$$

(2)因为任一男子其身高可能超过 182 厘米,也可能低于 182 厘米,一般来说,只有身高超过 182 厘米的才能与车门顶相碰, 因此, 我们将任一男子是否与车门顶碰头看成一个伯努利试验, 故问题转化为一个 10 重伯努利试验中的概率计算问题. 为此, 先求任一男子身高超过 182 厘米的概率 $p$,显然

$$
p = P\{ X > {182}\}  = P\left\{  {\frac{X - {170}}{6} > \frac{{182} - {170}}{6}}\right\}   = 1 - \Phi \left( 2\right)  = {0.0228}.
$$

设 $Y$ 为 10 个成年男子中身高超过 182 厘米的人数,故由以上分析知, $Y \sim  B\left( {{10},{0.0228}}\right)$,即

$$
P\{ Y = k\}  = {C}_{10}^{k}{\left( {0.0228}\right) }^{k}{\left( {0.9772}\right) }^{{10} - k},\;k = 0,1,\cdots,{10},
$$

故所求概率为

$$
P\{ Y \leq  1\}  = P\{ Y = 0\}  + P\{ Y = 1\}
$$

$$
= {\left( {0.9772}\right) }^{10} + {C}_{10}^{1}\left( {0.0228}\right) {\left( {0.9772}\right) }^{9}
$$

$$
\approx  {0.9793}\text{.}
$$

甲 80