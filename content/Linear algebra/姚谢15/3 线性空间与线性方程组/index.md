---
title: 3 线性空间与线性方程组
---
## § 3.1 基本概念

## 3.1.1 向量与向量空间

## 1. 定义

设 $\mathbb{F}$ 是一个数域, $\mathbb{F}$ 中 $n$ 个元素 ${a}_{1},{a}_{2},\cdots ,{a}_{n}$ 组成的有序组 $\mathbf{\alpha } = \left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right)$ 称为数域 $\mathbb{F}$ 上的一个 $n$ 维行向量. 若将这 $n$ 个元素排成一列:

$$
{\mathbf{\alpha }}^{\prime } = \left( \begin{matrix} {a}_{1} \\ {a}_{2} \\ \vdots \\ {a}_{n} \end{matrix}\right)
$$

则称之为 $n$ 维列向量.

## 2. 向量的运算

若 $\mathbf{\alpha } = \left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right) ,\mathbf{\beta } = \left( {{b}_{1},{b}_{2},\cdots ,{b}_{n}}\right)$ ,定义向量加法:

$$
\mathbf{\alpha } + \mathbf{\beta } = \left( {{a}_{1} + {b}_{1},{a}_{2} + {b}_{2},\cdots ,{a}_{n} + {b}_{n}}\right) .
$$

又若 $k \in \mathbb{F}$ ,定义 $k$ 与 $\mathbf{\alpha }$ 的数乘:

$$
k\mathbf{\alpha } = \left( {k{a}_{1}, k{a}_{2},\cdots, k{a}_{n}}\right) .
$$

3. 向量运算适合的规则

(1) 加法交换律: $\mathbf{\alpha } + \mathbf{\beta } = \mathbf{\beta } + \mathbf{\alpha }$ ;

(2) 加法结合律: $\left( {\mathbf{\alpha } + \mathbf{\beta }}\right) + \mathbf{\gamma } = \mathbf{\alpha } + \left( {\mathbf{\beta } + \mathbf{\gamma }}\right)$ ;

(3) $\mathbf{\alpha } + \mathbf{0} = \mathbf{\alpha }$ ;

(4) $\mathbf{\alpha } + \left( {-\mathbf{\alpha }}\right) = \mathbf{0}$ ;

(5) $1 \cdot \alpha = \alpha$ ;

(6) $k\left( {\mathbf{\alpha } + \mathbf{\beta }}\right) = k\mathbf{\alpha } + k\mathbf{\beta }$ ;

(7) $\left( {k + l}\right) \mathbf{\alpha } = k\mathbf{\alpha } + k\mathbf{\beta }$ ;

(8) $k\left( {l\alpha }\right) = \left( {kl}\right) \alpha$ .

## 4. 定义

设 $V$ 是一个集合, $\mathbb{F}$ 是数域,若在 $V$ 上定义了元素的加法 “+” 和 $\mathbb{F}$ 中的数对 $V$ 中元素的数乘,且这两种运算适合上面的 8 条运算规则,则称 $V$ 是数域 $\mathbb{F}$ 上的线性空间或向量空间.

## 3.1.2 向量的线性关系

## 1. 定义

设 $V$ 是数域 $\mathbb{F}$ 上的向量空间, ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 是 $V$ 中的向量,若存在 $\mathbb{F}$ 中 $m$ 个不全为零的数 ${a}_{1},{a}_{2},\cdots ,{a}_{m}$ ,使

$$
{a}_{1}{\mathbf{\alpha }}_{1} + {a}_{2}{\mathbf{\alpha }}_{2} + \cdots + {a}_{m}{\mathbf{\alpha }}_{m} = \mathbf{0},
$$

则称向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关. 反之,若不存在这样的数使上式成立,则称 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关.

## 2. 定义

设 $V$ 是数域 $\mathbb{F}$ 上的向量空间, $\mathbf{\beta },{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 是 $V$ 中向量,若存在 $\mathbf{F}$ 中 $m$ 个数 ${a}_{1},{a}_{2},\cdots ,{a}_{m}$ ,使

$$
\mathbf{\beta } = {a}_{1}{\mathbf{\alpha }}_{1} + {a}_{2}{\mathbf{\alpha }}_{2} + \cdots + {a}_{m}{\mathbf{\alpha }}_{m},
$$

则称向量 $\mathbf{\beta }$ 是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的线性组合,或称向量 $\mathbf{\beta }$ 可用向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 来线性表示 (或线性表出).

## 3. 定理

设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m},\mathbf{\beta }$ 是线性空间 $V$ 中的向量.

(1) 若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关,则任意一组包含这组向量的向量组必线性相关. 若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关,则从这组向量中任意取出一组向量必线性无关.

(2) 向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关的充要条件是其中至少有一个向量可以表示为其余向量的线性组合.

(3) 若 $\mathbf{\beta }$ 可表示为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的线性组合,即

$$
\mathbf{\beta } = {k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{m}{\mathbf{\alpha }}_{m},
$$

则表示唯一的充要条件是向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关.

## 4. 定理

设向量组 $A = \left\{ {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}}\right\}, B = \left\{ {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right\}$ 和 $C = \left\{ {{\mathbf{\gamma }}_{1},{\mathbf{\gamma }}_{2},\cdots ,{\mathbf{\gamma }}_{p}}\right\}$ 满足: $A$ 中任一向量都是 $B$ 中向量的线性组合, $B$ 中任一向量都是 $C$ 中向量的线性组合,则 $A$ 中任一向量都是 $C$ 中向量的线性组合.

## 3.1.3 基 与 维 数

## 1. 定义

设线性空间 $V$ 中有一族向量 $S$ ,如果在 $S$ 中存在一组向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ ,适合如下条件:

(1) ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关;

(2) $S$ 中任一向量都可以用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表示,

则称向量组 $\left\{ {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}}\right\}$ 是向量族 $S$ 的极大无关组. 一族向量的极大无关组可能有许多, 但由下面的定理可得: 每个极大无关组所含的向量的个数都相同. 这个数称为向量族的秩.

## 2. 定理

设 $A, B$ 是两组向量, $A$ 含有 $r$ 个向量, $B$ 含有 $s$ 个向量. 若 $A$ 中向量线性无关且 $A$ 中每个向量均可用 $B$ 中向量线性表示,则 $r \leq s$ .

## 3. 定义

数域 $\mathbb{F}$ 上的向量空间 $V$ 的一个极大无关组称为 $V$ 的一组基. 若 $V$ 的基含 $n$ 个向量,则称 $V$ 是 $n$ 维向量空间.

在向量空间 $V$ 中引进一组基 $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\}$ 以后, $V$ 中任意一个向量 $\mathbf{\alpha }$ 有且只有一种方法表示为基向量的线性组合. 设 $\mathbf{\alpha } = {a}_{1}{\mathbf{e}}_{1} + {a}_{2}{\mathbf{e}}_{2} + \cdots + {a}_{n}{\mathbf{e}}_{n}$ ,则称 $n$ 维列向量 ${\left( {a}_{1},{a}_{2},\cdots ,{a}_{n}\right) }^{\prime }$ 为向量 $\mathbf{\alpha }$ 在基 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 下的坐标向量. 映射 $\varphi : V \rightarrow {\mathbb{F}}^{n},\varphi \left( \mathbf{\alpha }\right) = {\left( {a}_{1},{a}_{2},\cdots ,{a}_{n}\right) }^{\prime }$ ,是一个一一对应.

## 4. 定义

设 $V$ 和 $U$ 都是数域 $\mathbb{F}$ 上的线性空间,若存在 $V$ 到 $U$ 的映射 $\varphi$ 适合条件:

(1) $\varphi \left( {\mathbf{\alpha } + \mathbf{\beta }}\right) = \varphi \left( \mathbf{\alpha }\right) + \varphi \left( \mathbf{\beta }\right)$ 对任意的 $\mathbf{\alpha },\mathbf{\beta } \in V$ 成立;

(2) $\varphi \left( {k\mathbf{\alpha }}\right) = {k\varphi }\left( \mathbf{\alpha }\right)$ 对任意的 $\mathbf{\alpha } \in V, k \in \mathbb{F}$ 成立;

(3) $\varphi$ 是一一对应的,

则称 $\varphi$ 是 $V$ 到 $U$ 的线性同构.

将任一向量映射为它在给定基下的坐标向量的映射 $\varphi : V \rightarrow {\mathbb{F}}^{n}$ 是线性同构.

## 5. 定理

(1) 同构关系是一种等价关系;

(2) 线性同构不仅将线性相关的向量组映射为线性相关的向量组, 而且将线性无关的向量映射为线性无关的向量组;

(3) 同一个数域 $\mathbb{F}$ 上的线性空间同构的充要条件是它们具有相同的维数.

## 3.1.4 基变换与过渡矩阵

## 1. 过渡矩阵

设 $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\}$ 和 $\left\{ {{f}_{1},{f}_{2},\cdots ,{f}_{n}}\right\}$ 是 $n$ 维线性空间 $V$ 的两组基,若

$$
\left\{ \begin{matrix} {\mathbf{f}}_{1} = {a}_{11}{\mathbf{e}}_{1} + {a}_{21}{\mathbf{e}}_{2} + \cdots + {a}_{n1}{\mathbf{e}}_{n}, \\ {\mathbf{f}}_{2} = {a}_{12}{\mathbf{e}}_{1} + {a}_{22}{\mathbf{e}}_{2} + \cdots + {a}_{n2}{\mathbf{e}}_{n}, \\ \cdots \cdots \cdots \cdots \\ {\mathbf{f}}_{n} = {a}_{1n}{\mathbf{e}}_{1} + {a}_{2n}{\mathbf{e}}_{2} + \cdots + {a}_{nn}{\mathbf{e}}_{n}, \end{matrix}\right.
$$

则矩阵

$$
\mathbf{A} = \left( \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{n1} & {a}_{n2} & \cdots & {a}_{nn} \end{matrix}\right)
$$

称为从基 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 到基 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots ,{\mathbf{f}}_{n}}\right\}$ 的过渡矩阵.

## 2. 同一向量在不同基下坐标向量的关系

设 $V$ 是数域 $\mathbb{F}$ 上 $n$ 维线性空间,从基 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 到 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots ,{\mathbf{f}}_{n}}\right\}$ 的过渡矩阵为 $\mathbf{A} = \left( {a}_{ij}\right)$ . 若 $V$ 中向量 $\mathbf{\alpha }$ 在基 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 下的坐标向量是 ${\left( {x}_{1},{x}_{2},\cdots ,{x}_{n}\right) }^{\prime }$ ,在基 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots ,{\mathbf{f}}_{n}}\right\}$ 下的坐标向量是 ${\left( {y}_{1},{y}_{2},\cdots ,{y}_{n}\right) }^{\prime }$ ,则

$$
\left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right) = \left( \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{n1} & {a}_{n2} & \cdots & {a}_{nn} \end{matrix}\right) \left( \begin{matrix} {y}_{1} \\ {y}_{2} \\ \vdots \\ {y}_{n} \end{matrix}\right) .
$$

## 3. 定理

矩阵 $\mathbf{A}$ 是 $n$ 维线性空间 $V$ 的基 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 到基 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots ,{\mathbf{f}}_{n}}\right\}$ 的过渡矩阵,则 $\mathbf{A}$ 是可逆矩阵且从基 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots ,{\mathbf{f}}_{n}}\right\}$ 到基 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 的过渡矩阵为 ${\mathbf{A}}^{-1}$ . 又若 $\mathbf{B}$ 是从基 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots ,{\mathbf{f}}_{n}}\right\}$ 到基 $\left\{ {{\mathbf{g}}_{1},{\mathbf{g}}_{2},\cdots ,{\mathbf{g}}_{n}}\right\}$ 的过渡矩阵,则从基 $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\}$ 到基 $\left\{ {{g}_{1},{g}_{2},\cdots ,{g}_{n}}\right\}$ 的过渡矩阵为 $\mathbf{{AB}}$ .

## 3.1.5 子 空 间

## 1. 定义

设 $V$ 是数域 $\mathbb{F}$ 上的线性空间, $U$ 是 $V$ 的非空子集,若 $U$ 在 $V$ 的向量加法与数乘下也成为线性空间,则称 $U$ 是 $V$ 的子空间.

要验证线性空间 $V$ 的非空子集 $U$ 是子空间,只要验证 $U$ 中元素在向量加法与数乘下封闭就可以了.

## 2. 子空间的运算

设 ${V}_{1},{V}_{2}$ 是线性空间 $V$ 的子空间,定义 ${V}_{1} + {V}_{2} = \left\{ {{v}_{1} + {v}_{2} \mid {v}_{1} \in {V}_{1},{v}_{2} \in {V}_{2}}\right\}$ , 则 ${V}_{1} + {V}_{2}$ 是 $V$ 的子空间,称为 ${V}_{1}$ 与 ${V}_{2}$ 的和空间. 又 ${V}_{1} \cap {V}_{2}$ 也是 $V$ 的子空间,称为 ${V}_{1}$ 与 ${V}_{2}$ 的交空间.

## 3. 生成

设 $S$ 是线性空间 $V$ 的子集, $V$ 中所有包含 $S$ 的子空间的交称为由子集 $S$ 生成的子空间,记为 $L\left( S\right) .L\left( S\right)$ 是 $V$ 中包含集合 $S$ 的最小子空间,它由 $S$ 中向量所有可能的线性组合组成. 4. 直和

${V}_{1},{V}_{2},\cdots ,{V}_{k}$ 是线性空间 $V$ 的子空间,若对任意的 $i\left( {i = 1,2,\cdots, k}\right)$ ,均有

$$
{V}_{i} \cap \left( {{V}_{1} + \cdots + {V}_{i - 1} + {V}_{i + 1} + \cdots + {V}_{k}}\right) = 0,
$$

则称和 ${V}_{1} + {V}_{2} + \cdots + {V}_{k}$ 是直接和,简称直和,记为

$$
{V}_{1} \oplus {V}_{2} \oplus \cdots \oplus {V}_{k}
$$

## 5. 定理

设 ${V}_{1},{V}_{2},\cdots ,{V}_{k}$ 是线性空间 $V$ 的子空间, ${V}_{0} = {V}_{1} + {V}_{2} + \cdots + {V}_{k}$ ,则下列命题等价:

(1) ${V}_{0} = {V}_{1} \oplus {V}_{2} \oplus \cdots \oplus {V}_{k}$ 是直和;

(2) 对任意的 $2 \leq i \leq k$ ,有

$$
{V}_{i} \cap \left( {{V}_{1} + {V}_{2} + \cdots + {V}_{i - 1}}\right) = 0
$$

(3) $\dim \left( {{V}_{1} + {V}_{2} + \cdots + {V}_{k}}\right) = \dim {V}_{1} + \dim {V}_{2} + \cdots + \dim {V}_{k}$ ;

(4) ${V}_{1},{V}_{2},\cdots ,{V}_{k}$ 的一组基可以拼成 ${V}_{0}$ 的一组基;

(5) ${V}_{0}$ 中的向量表示为 ${V}_{1},{V}_{2},\cdots ,{V}_{k}$ 中的向量之和时其表示唯一.

## 6. 定理 (维数公式)

设 ${V}_{1},{V}_{2}$ 是线性空间 $V$ 的两个子空间,则

$$
\dim \left( {{V}_{1} + {V}_{2}}\right) = \dim {V}_{1} + \dim {V}_{2} - \dim \left( {{V}_{1} \cap {V}_{2}}\right)
$$

## 3.1.6 矩 阵 的 秩

## 1. 定义

设 $\mathbf{A}$ 是 $m \times n$ 矩阵, $\mathbf{A}$ 的行向量 (或列向量) 组的秩定义为 $\mathbf{A}$ 的秩.

## 2. 定理

矩阵的秩在矩阵的初等变换下不变.

## 3. 推论

(1) 对任意一个秩为 $r$ 的 $m \times n$ 矩阵 $\mathbf{A}$ ,总存在 $m$ 阶非异阵 $\mathbf{P}$ 和 $n$ 阶非异阵 $\mathbf{Q}$ ,使得

$$
{PAQ} = \left( \begin{array}{ll} {I}_{r} & O \\ O & O \end{array}\right)
$$

(2) 任一矩阵与一非异阵相乘, 其秩不变.

(3) $n$ 阶方阵是可逆矩阵的充要条件是它是满秩阵,即它的秩等于 $n$ .

(4) 两个 $m \times n$ 矩阵等价的充要条件是它们具有相同的秩.

## 4. 定理

矩阵 $\mathbf{A}$ 的秩等于 $r$ 的充要条件是 $\mathbf{A}$ 有一个 $r$ 阶子式不等于零,而 $\mathbf{A}$ 的所有 $r + 1$ 阶子式都等于零.

## 3.1.7 线性方程组的解

## 1. 定理

设有 $n$ 个未知数 $m$ 个方程式组成的线性方程组

$$
\left\{ \begin{matrix} {a}_{11}{x}_{1} + {a}_{12}{x}_{2} + \cdots + {a}_{1n}{x}_{n} = {b}_{1}, \\ {a}_{21}{x}_{1} + {a}_{22}{x}_{2} + \cdots + {a}_{2n}{x}_{n} = {b}_{2}, \\ \cdots \cdots \cdots \cdots \\ {a}_{m1}{x}_{1} + {a}_{m2}{x}_{2} + \cdots + {a}_{mn}{x}_{n} = {b}_{m}. \end{matrix}\right.
$$

它的系数矩阵记为 $\mathbf{A}$ ,增广矩阵记为 $\widetilde{\mathbf{A}}$ ,则

(1) 若 $\widetilde{\mathbf{A}}$ 和 $\mathbf{A}$ 的秩都等于 $n$ ,则方程组有且只有一组解.

(2) 若 $\widetilde{\mathbf{A}}$ 和 $\mathbf{A}$ 的秩相等但小于 $n$ ,则方程组有无穷多组解.

(3) 若 $\widetilde{\mathbf{A}}$ 和 $\mathbf{A}$ 的秩不相等,则方程组无解.

## 2. 定义

设 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 是 $n$ 个变元 $m$ 个方程式的齐次线性方程组. 假定 ${\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{k}$ 是它的一组解向量, 若这组解向量线性无关且方程组的任意一个解向量均可表示为它们的线性组合,则 ${\eta }_{1},{\eta }_{2},\cdots ,{\eta }_{k}$ 称为齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的一个基础解系.

## 3. 定理

设 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 是 $n$ 个变元 $m$ 个方程式的齐次线性方程组. 假定系数矩阵 $\mathbf{A}$ 的秩等于 $r < n$ ,则方程组有非零解且每个基础解系均由 $n - r$ 个向量组成.

## 4. 定理

设 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 是 $n$ 个变元 $m$ 个方程式的非齐次线性方程组. 假定 $\mathbf{A}$ 的秩等于增广矩阵 $\widetilde{\mathbf{A}}$ 的秩,又假定该方程组的相伴齐次线性方程组 (或称导出组) $\mathbf{{Ax}} = \mathbf{0}$ 的基础解系为 ${\eta }_{1},{\eta }_{2},\cdots ,{\eta }_{n - r}$ ,向量 $\gamma$ 是 ${Ax} = \beta$ 的一个解 (也称为特解),则非齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 的所有解均可表示为下列形状:

$$
{a}_{1}{\mathbf{\eta }}_{1} + {a}_{2}{\mathbf{\eta }}_{2} + \cdots + {a}_{n - r}{\mathbf{\eta }}_{n - r} + \mathbf{\gamma }
$$

其中 ${a}_{1},{a}_{2},\cdots ,{a}_{n - r}$ 可取任意数.

## § 3.2 例题解析

## 3.2.1 向量的线性关系

对线性空间 $V$ 中的一组向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ ,判定它们是线性相关还是线性无关, 这是线性空间理论中的一个基本问题. 处理这类问题通常有两种方法, 一种是代数方法, 即矩阵的初等变换以及秩的理论; 另一种是几何方法, 即向量线性关系的定义以及发展起来的线性空间理论. 在这一节中, 我们首先阐述代数方法的相关原理, 然后再分主题进行例题的讨论和分析.

矩阵 $\mathbf{A}$ 的第 $i$ 行从左至右第一个非零元素称为第 $i$ 行的阶梯点. 若矩阵 $\mathbf{A}$ 的阶梯点的列指标随着行数严格递增, 则称这样的矩阵为阶梯形矩阵. 利用数学归纳法容易证明: 对任一矩阵 $\mathbf{A}$ ,经过若干次初等行变换之后,均可以化为阶梯形矩阵.

例 3.1 设 $\mathbf{A}$ 是 $m \times n$ 阶梯形矩阵,则 $\mathbf{A}$ 的秩等于其非零行的个数,且阶梯点所在的列向量是 $\mathbf{A}$ 的列向量的极大无关组.

证明 设

$$
\mathbf{A} = \left( \begin{matrix} 0 & \cdots & {a}_{1{k}_{1}} & \cdots & \cdots & \cdots & \cdots & \cdots \\ 0 & \cdots & 0 & \cdots & {a}_{2{k}_{2}} & \cdots & \cdots & \cdots \\ \vdots & \cdot & \vdots & & \vdots & & \vdots & \vdots \\ 0 & \cdots & 0 & \cdots & 0 & \cdots & {a}_{r{k}_{r}} & \cdots \\ & & & & 0 & & & \end{matrix}\right) ,
$$

其中 ${a}_{1{k}_{1}},{a}_{2{k}_{2}},\cdots ,{a}_{r{k}_{r}}$ 是 $\mathbf{A}$ 的阶梯点. 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 是 $\mathbf{A}$ 的前 $r$ 行,我们先证明它们线性无关. 设

$$
{c}_{1}{\mathbf{\alpha }}_{1} + {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{r}{\mathbf{\alpha }}_{r} = \mathbf{0},
$$

其中 ${c}_{1},{c}_{2},\cdots ,{c}_{r}$ 是常数. 上式是关于 $n$ 维行向量的等式,先考察行向量的第 ${k}_{1}$ 分量可得 ${c}_{1}{a}_{1{k}_{1}} = 0$ ,因为 ${a}_{1{k}_{1}} \neq 0$ ,故 ${c}_{1} = 0$ ; 再依次考察行向量的第 ${k}_{2},\cdots ,{k}_{r}$ 分量,最后可得 ${c}_{1} = {c}_{2} = \cdots = {c}_{r} = 0$ . 因此 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,从而 $\mathbf{A}$ 的秩等于 $r$ ,即其非零行的个数.

再将 $r$ 个阶梯点所在的列向量取出,拼成一个新的矩阵:

$$
\mathbf{B} = \left( \begin{matrix} {a}_{1{k}_{1}} & \cdots & \cdots & \cdots \\ 0 & {a}_{2{k}_{2}} & \cdots & \cdots \\ \vdots & \vdots & & \vdots \\ 0 & 0 & \cdots & {a}_{r{k}_{r}} \\ & & & \end{matrix}\right) .
$$

采用相同的方法可证明矩阵 $\mathbf{B}$ 的前 $r$ 行线性无关,因此 $\mathrm{r}\left( \mathbf{B}\right) = r$ ,从而阶梯点所在的列向量组的秩也等于 $r$ ,又因为 $\mathrm{r}\left( \mathbf{A}\right) = r$ ,故它们是 $\mathbf{A}$ 的列向量的极大无关组. [

例 3.2 设 $\mathbf{A} = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right)$ 是一个 $m \times n$ 矩阵, ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 是列向量. $\mathbf{P}$ 是一个 $m$ 阶可逆矩阵, $\mathbf{B} = \mathbf{P}\mathbf{A} = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right)$ ,其中 ${\mathbf{\beta }}_{j} = \mathbf{P}{\mathbf{\alpha }}_{j}(j =$ $1,2,\cdots, n)$ . 若 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{k}}$ 是 $\mathbf{A}$ 的列向量的极大无关组,则 ${\mathbf{\beta }}_{{i}_{1}},{\mathbf{\beta }}_{{i}_{2}},\cdots ,{\mathbf{\beta }}_{{i}_{k}}$ 是 $\mathbf{B}$ 的列向量的极大无关组.

证明 先证明向量组 ${\mathbf{\beta }}_{{i}_{1}},{\mathbf{\beta }}_{{i}_{2}},\cdots ,{\mathbf{\beta }}_{{i}_{k}}$ 线性无关. 设

$$
{c}_{1}{\mathbf{\beta }}_{{i}_{1}} + {c}_{2}{\mathbf{\beta }}_{{i}_{2}} + \cdots + {c}_{k}{\mathbf{\beta }}_{{i}_{k}} = \mathbf{0},
$$

即

$$
{c}_{1}\mathbf{P}{\mathbf{\alpha }}_{{i}_{1}} + {c}_{2}\mathbf{P}{\mathbf{\alpha }}_{{i}_{2}} + \cdots + {c}_{k}\mathbf{P}{\mathbf{\alpha }}_{{i}_{k}} = \mathbf{0}.
$$

已知 $\mathbf{P}$ 是可逆矩阵,因此

$$
{c}_{1}{\mathbf{\alpha }}_{{i}_{1}} + {c}_{2}{\mathbf{\alpha }}_{{i}_{2}} + \cdots + {c}_{k}{\mathbf{\alpha }}_{{i}_{k}} = \mathbf{0}.
$$

而向量组 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{k}}$ 线性无关,故 ${c}_{1} = {c}_{2} = \cdots = {c}_{k} = 0$ . 这证明了向量组 ${\mathbf{\beta }}_{{i}_{1}},{\mathbf{\beta }}_{{i}_{2}},\cdots ,{\mathbf{\beta }}_{{i}_{k}}$ 线性无关. 要证这是 $\mathbf{B}$ 列向量的极大无关组,只需证明 $\mathbf{B}$ 的任意一个列向量都是这些向量的线性组合即可. 设 ${\mathbf{\beta }}_{j}$ 是 $\mathbf{B}$ 的任意一个列向量,则 ${\mathbf{\beta }}_{j} = \mathbf{P}{\mathbf{\alpha }}_{j}$ . 因为 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{k}}$ 是 $\mathbf{A}$ 的列向量的极大无关组,故 ${\mathbf{\alpha }}_{j}$ 可用 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{k}}$ 线性表示,不妨设

$$
{\mathbf{\alpha }}_{j} = {b}_{1}{\mathbf{\alpha }}_{{i}_{1}} + {b}_{2}{\mathbf{\alpha }}_{{i}_{2}} + \cdots + {b}_{k}{\mathbf{\alpha }}_{{i}_{k}},
$$

则

$$
\mathbf{P}{\mathbf{\alpha }}_{j} = {b}_{1}\mathbf{P}{\mathbf{\alpha }}_{{i}_{1}} + {b}_{2}\mathbf{P}{\mathbf{\alpha }}_{{i}_{2}} + \cdots + {b}_{k}\mathbf{P}{\mathbf{\alpha }}_{{i}_{k}},
$$

即

$$
{\mathbf{\beta }}_{j} = {b}_{1}{\mathbf{\beta }}_{{i}_{1}} + {b}_{2}{\mathbf{\beta }}_{{i}_{2}} + \cdots + {b}_{k}{\mathbf{\beta }}_{{i}_{k}}
$$

注 (1) 因为矩阵的秩在初等变换下不变, 由例 3.1 我们得到求一个矩阵秩的方法: 用初等行变换将一个矩阵 $\mathbf{A}$ 化为阶梯形矩阵 $\mathbf{B}$ ,则矩阵 $\mathbf{B}$ 的非零行的个数就是矩阵 $\mathbf{A}$ 的秩.

(2) 对矩阵求秩的方法也可以用来求行 (列) 向量组的秩, 方法是将行 (列) 向量组拼成一个矩阵, 用初等变换求出矩阵的秩, 由于矩阵的秩就是其行 (列) 向量组的秩, 从而就得到了向量组的秩.

(3) 知道向量组的秩之后, 我们就可以判定向量组是否线性相关了. 若向量组的秩等于向量的个数, 则向量组线性无关; 若向量组的秩小于向量的个数, 则向量组线性相关.

(4) 进一步还可以求行 (列) 向量组的极大无关组, 注意此时应将行 (列) 向量组按列分块的方式拼成矩阵 $\mathbf{A}$ ,并用初等行变换将矩阵变为阶梯形矩阵 $\mathbf{B}$ . 由例 3.1 知 $\mathbf{B}$ 的阶梯点所在的列向量是 $\mathbf{B}$ 的列向量的极大无关组,再由例 3.2 知初等行变换保持 $\mathbf{A},\mathbf{B}$ 列向量的极大无关组的列指标,从而可得 $\mathbf{A}$ 的列向量的极大无关组.

## 1. 具体计算问题

遇到具体的行 (列) 向量组, 要判定线性相关还是线性无关, 或者要求出它的秩和极大无关组, 我们通常都是利用上面的代数方法去做.

例 3.3 判定下列两组向量是线性相关还是线性无关:

(1) $\left( {-1,3,1}\right) ,\left( {2,1,0}\right) ,\left( {1,4,1}\right)$ ;

(2) $\left( {2,3,0}\right) ,\left( {-1,4,0}\right) ,\left( {0,0,2}\right)$ .

解 (1) 将向量拼成矩阵, 并用初等行变换化为阶梯形矩阵:

$$
\left( \begin{matrix} - 1 & 3 & 1 \\ 2 & 1 & 0 \\ 1 & 4 & 1 \end{matrix}\right) \rightarrow \left( \begin{matrix} - 1 & 3 & 1 \\ 0 & 7 & 2 \\ 0 & 7 & 2 \end{matrix}\right) \rightarrow \left( \begin{matrix} - 1 & 3 & 1 \\ 0 & 7 & 2 \\ 0 & 0 & 0 \end{matrix}\right)
$$

上述矩阵的秩等于 2 , 故向量组线性相关.

(2) 将向量拼成矩阵, 并用初等行变换化为阶梯形矩阵:

$$
\left( \begin{matrix} 2 & 3 & 0 \\ - 1 & 4 & 0 \\ 0 & 0 & 2 \end{matrix}\right) \rightarrow \left( \begin{matrix} - 1 & 4 & 0 \\ 2 & 3 & 0 \\ 0 & 0 & 2 \end{matrix}\right) \rightarrow \left( \begin{matrix} - 1 & 4 & 0 \\ 0 & {11} & 0 \\ 0 & 0 & 2 \end{matrix}\right)
$$

上述矩阵秩等于 3 , 故向量组线性无关.

要判定一个向量 $\mathbf{\beta }$ 是向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的线性组合,也可以用矩阵方法. 先求出向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的秩,再求出向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m},\mathbf{\beta }$ 的秩,如果两者相等,则 $\mathbf{\beta }$ 可以用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表示,否则 $\mathbf{\beta }$ 不能用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表示. 这种方法实际上和解非齐次线性方程组是一回事, 即判断是否存在 ${x}_{1},{x}_{2},\cdots ,{x}_{m}$ ,使 $\mathbf{\beta } = {x}_{1}{\mathbf{\alpha }}_{1} + {x}_{2}{\mathbf{\alpha }}_{2} + \cdots + {x}_{m}{\mathbf{\alpha }}_{m}$ . 求出 ${x}_{i}$ 就可以得到具体的表达式, 同时还可以判断表示是否唯一.

例 3.4 判定下列向量 $\mathbf{\beta }$ 能否用向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性表示:

(1) $\mathbf{\beta } = \left( {5,4, - 2,4}\right) ;{\mathbf{\alpha }}_{1} = \left( {1,0, - 1,3}\right) ,{\mathbf{\alpha }}_{2} = \left( {2,1,0,1}\right) ,{\mathbf{\alpha }}_{3} = \left( {0, - 2,1,1}\right)$ ;

(2) $\mathbf{\beta } = \left( {1,1,1,1}\right) ;{\mathbf{\alpha }}_{1} = \left( {-1,2, - 1,1}\right) ,{\mathbf{\alpha }}_{2} = \left( {4,0,1, - 1}\right) ,{\mathbf{\alpha }}_{3} = \left( {3,2,0,0}\right)$ .

解 (1) 将向量按列分块方式拼成矩阵, 并用初等行变换化为阶梯形矩阵:

$$
\left( \begin{matrix} 1 & 2 & 0 & \vdots & 5 \\ 0 & 1 & - 2 & \vdots & 4 \\ - 1 & 0 & 1 & \vdots & - 2 \\ 3 & 1 & 1 & \vdots & 4 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 2 & 0 & \vdots & 5 \\ 0 & 1 & - 2 & \vdots & 4 \\ 0 & 2 & 1 & \vdots & 3 \\ 0 & 1 & 4 & \vdots & - 2 \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 2 & 0 & \vdots & 5 \\ 0 & 1 & - 2 & \vdots & 4 \\ 0 & 0 & 5 & \vdots & - 5 \\ 0 & 0 & 5 & \vdots & - 5 \\ 0 & 0 & 0 & \vdots & 0 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 2 & 0 & \vdots & 5 \\ 0 & 1 & - 2 & \vdots & 4 \\ 0 & 0 & 5 & \vdots & - 5 \\ 0 & 0 & 0 & \vdots & 0 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & 0 & 1 & \\ 0 & 1 & 0 & \vdots & 2 \\ 0 & 0 & 1 & - 1 & \\ 0 & 0 & 0 & \vdots & 0 \end{matrix}\right) ,
$$

故 $\mathbf{\beta }$ 能用向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性表示. 由线性方程组解的理论可知上述表示是唯一的, 且

$$
\mathbf{\beta } = {\mathbf{\alpha }}_{1} + 2{\mathbf{\alpha }}_{2} - {\mathbf{\alpha }}_{3}
$$

(2) 将向量按列分块方式拼成矩阵, 并用初等行变换化为阶梯形矩阵:

$$
\left( \begin{matrix} - 1 & 4 & 3 & 1 \\ 2 & 0 & 2 & 1 \\ - 1 & 1 & 0 & 1 \\ 1 & - 1 & 0 & 1 \end{matrix}\right) \rightarrow \left( \begin{matrix} - 1 & 4 & 3 & 1 \\ 0 & 8 & 8 & 3 \\ 0 & - 3 & - 3 & 0 \\ 0 & 0 & 0 & 2 \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} - 1 & 4 & 3 & 1 \\ 0 & 0 & 0 & 1 \\ 0 & - 3 & - 3 & 0 \\ 0 & 0 & 0 & 1 \end{matrix}\right) \rightarrow \left( \begin{matrix} - 1 & 4 & 3 & 1 \\ 0 & - 3 & - 3 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & 0 \end{matrix}\right)
$$

故 $\mathbf{\beta }$ 不能用向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性表示.

例 3.5 求下列向量组的秩:

$$
\left( {1,0, - 1,3, - 2}\right) ,\left( {2,1,0, - 1,0}\right) ,\left( {3,1, - 1,2, - 2}\right) \text{.}
$$

解 将向量拼成矩阵, 并用初等行变换化为阶梯形矩阵:

$$
\left( \begin{matrix} 1 & 0 & - 1 & 3 & - 2 \\ 2 & 1 & 0 & - 1 & 0 \\ 3 & 1 & - 1 & 2 & - 2 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & - 1 & 3 & - 2 \\ 0 & 1 & 2 & - 7 & 4 \\ 0 & 0 & 0 & 0 & 0 \end{matrix}\right)
$$

故矩阵的秩为 2 , 因此向量组的秩也为 2 .

例 3.6 求下列向量组的一个极大无关组:

$$
{\mathbf{\alpha }}_{1} = \left( {1,1,2,2,1}\right) ,{\mathbf{\alpha }}_{2} = \left( {0,2,1,5, - 1}\right) ,{\mathbf{\alpha }}_{3} = \left( {2,0,3, - 1,3}\right) ,{\mathbf{\alpha }}_{4} = \left( {1,1,0,4, - 1}\right) \text{.}
$$

解 将向量按列分块方式拼成矩阵, 并用初等行变换化为阶梯形矩阵:

$$
\left( \begin{matrix} 1 & 0 & 2 & 1 \\ 1 & 2 & 0 & 1 \\ 2 & 1 & 3 & 0 \\ 2 & 5 & - 1 & 4 \\ 1 & - 1 & 3 & - 1 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & 2 & 1 \\ 0 & 1 & - 1 & - 2 \\ 0 & 0 & 0 & 4 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{matrix}\right) .
$$

注意到右边阶梯形矩阵中阶梯点所在的列指标为 $1,2,4$ ,所以 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{4}$ 是向量组的一个极大无关组. 注意到极大无关组一般并不唯一,在本题中,除了 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{4}$ 之外, ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 和 ${\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 也都是极大无关组,但 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 不是极大无关组.

## 2. 理论证明问题

遇到向量线性关系的证明题, 通常我们从线性关系的定义出发, 利用发展起来的线性空间的理论加以证明. 下面我们将给出一些典型的例题.

例 3.7 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 是线性空间 $V$ 中一组线性无关的向量, $\mathbf{\beta }$ 是 $V$ 中的向量. 求证: 或者 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m},\mathbf{\beta }$ 线性无关,或者 $\mathbf{\beta }$ 是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的线性组合.

证明 若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m},\mathbf{\beta }$ 线性无关,则结论得证. 若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m},\mathbf{\beta }$ 线性相关,则存在不全为零的数 ${c}_{1},{c}_{2},\cdots ,{c}_{m}, d$ ,使得

$$
{c}_{1}{\mathbf{\alpha }}_{1} + {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{m}{\mathbf{\alpha }}_{m} + d\mathbf{\beta } = \mathbf{0}.
$$

若 $d = 0$ ,则 ${c}_{1},{c}_{2},\cdots ,{c}_{m}$ 不全为零且 ${c}_{1}{\mathbf{\alpha }}_{1} + {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{m}{\mathbf{\alpha }}_{m} = \mathbf{0}$ ,这与 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots$ , ${\mathbf{\alpha }}_{m}$ 线性无关矛盾. 因此 $d \neq 0$ ,从而

$$
\mathbf{\beta } = - \frac{{c}_{1}}{d}{\mathbf{\alpha }}_{1} - \frac{{c}_{2}}{d}{\mathbf{\alpha }}_{2} - \cdots - \frac{{c}_{m}}{d}{\mathbf{\alpha }}_{m}
$$

即 $\mathbf{\beta }$ 是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的线性组合.

注 上述结论等价于: 若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关且 $\mathbf{\beta } \notin L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}}\right)$ , 则 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m},\mathbf{\beta }$ 线性无关. 虽然这个等价命题很简单,但后面经常会用到.

例 3.8 设向量 $\mathbf{\beta }$ 可由向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表示,但不能由其中任何一个个数少于 $m$ 的部分向量线性表示,求证: 这 $m$ 个向量线性无关.

证明 用反证法,设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关,则至少有一个向量是其余向量的线性组合. 不妨设 ${\mathbf{\alpha }}_{m}$ 是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m - 1}$ 的线性组合,则由线性组合的传递性可知 $\mathbf{\beta }$ 也是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m - 1}$ 的线性组合,这与假设矛盾.

例 3.9 设线性空间 $V$ 中向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,已知有序向量组 $\left\{ {\mathbf{\beta },{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}}\right\}$ 线性相关,求证: 最多只有一个 ${\mathbf{\alpha }}_{i}$ 可以表示为前面向量的线性组合.

证明 用反证法,设存在 $1 \leq i < j \leq r$ ,使得

$$
{\mathbf{\alpha }}_{i} = b\mathbf{\beta } + {a}_{1}{\mathbf{\alpha }}_{1} + {a}_{2}{\mathbf{\alpha }}_{2} + \cdots + {a}_{i - 1}{\mathbf{\alpha }}_{i - 1},
$$

$$
{\mathbf{\alpha }}_{j} = d\mathbf{\beta } + {c}_{1}{\mathbf{\alpha }}_{1} + {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{j - 1}{\mathbf{\alpha }}_{j - 1}.
$$

由于 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,故 $b \neq 0$ . 将第一个等式乘以 $- \frac{d}{b}$ 后加到第二个等式上,可得 ${\mathbf{\alpha }}_{j}$ 是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{j - 1}$ 的线性组合,这与 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关矛盾. $\square$

例 3.10 设 $n$ 维列向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关, $\mathbf{A}$ 为 $n$ 阶可逆矩阵,求证: $\mathbf{A}{\mathbf{\alpha }}_{1},\mathbf{A}{\mathbf{\alpha }}_{2},\cdots ,\mathbf{A}{\mathbf{\alpha }}_{m}$ 线性无关.

证明 由例 3.2 即得.

例 3.11 设 $\mathbf{A}$ 是 $n \times m$ 矩阵, $\mathbf{B}$ 是 $m \times n$ 矩阵. 若 $\mathbf{A}\mathbf{B} = {\mathbf{I}}_{n}$ ,求证: $\mathbf{B}$ 的 $n$ 个列向量线性无关.

证明 设 $\mathbf{B} = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right)$ 为列分块,则 $\mathbf{A}\mathbf{B} = \left( {\mathbf{A}{\mathbf{\beta }}_{1},\mathbf{A}{\mathbf{\beta }}_{2},\cdots ,\mathbf{A}{\mathbf{\beta }}_{n}}\right)$ . 由 $\mathbf{A}\mathbf{B} = {\mathbf{I}}_{n}$ 可得 $\mathbf{A}{\mathbf{\beta }}_{i} = {\mathbf{e}}_{i}\left( {1 \leq i \leq n}\right)$ ,其中 ${\mathbf{e}}_{i}$ 是 $n$ 维标准单位列向量. 设

$$
{c}_{1}{\mathbf{\beta }}_{1} + {c}_{2}{\mathbf{\beta }}_{2} + \cdots + {c}_{n}{\mathbf{\beta }}_{n} = \mathbf{0}.
$$

上式两边同时左乘 $\mathbf{A}$ ,可得

$$
\mathbf{0} = {c}_{1}\mathbf{A}{\mathbf{\beta }}_{1} + {c}_{2}\mathbf{A}{\mathbf{\beta }}_{2} + \cdots + {c}_{n}\mathbf{A}{\mathbf{\beta }}_{n} = {c}_{1}{\mathbf{e}}_{1} + {c}_{2}{\mathbf{e}}_{2} + \cdots + {c}_{n}{\mathbf{e}}_{n} = {\left( {c}_{1},{c}_{2},\cdots ,{c}_{n}\right) }^{\prime },
$$

因此 ${c}_{1} = {c}_{2} = \cdots = {c}_{n} = 0$ ,即 $\mathbf{B}$ 的 $n$ 个列向量 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ 线性无关.

例 3.12 设 $\left\{ {{\mathbf{\alpha }}_{i} = \left( {{a}_{i1},{a}_{i2},\cdots ,{a}_{in}}\right) ,1 \leq i \leq m}\right\}$ 是一组 $n$ 维行向量, $1 \leq {j}_{1} <$ ${j}_{2} < \cdots < {j}_{t} \leq n$ 是给定的 $t\left( {t < n}\right)$ 个指标. 定义 ${\widetilde{\mathbf{\alpha }}}_{i} = \left( {{a}_{i{j}_{1}},{a}_{i{j}_{2}},\cdots ,{a}_{i{j}_{t}}}\right)$ ,称 ${\widetilde{\mathbf{\alpha }}}_{i}$ 为 ${\mathbf{\alpha }}_{i}$ 的 $t$ 维缩短向量. 求证: 如果 ${\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{m}$ 线性无关,则 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 也线性无关.

证明 我们来证明它的逆否命题,即若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关,则 ${\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots$ , ${\widetilde{\mathbf{\alpha }}}_{m}$ 也线性相关. 由假设存在不全为零的数 ${c}_{1},{c}_{2},\cdots ,{c}_{m}$ ,使得

$$
\mathbf{0} = {c}_{1}{\mathbf{\alpha }}_{1} + {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{m}{\mathbf{\alpha }}_{m} = \left( {\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}{a}_{i1},\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}{a}_{i2},\cdots ,\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}{a}_{in}}\right) .
$$

等式两边同时取 $t$ 维缩短向量,可得

$$
\mathbf{0} = \left( {\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}{a}_{i{j}_{1}},\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}{a}_{i{j}_{2}},\cdots ,\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{i}{a}_{i{j}_{t}}}\right) = {c}_{1}{\widetilde{\mathbf{\alpha }}}_{1} + {c}_{2}{\widetilde{\mathbf{\alpha }}}_{2} + \cdots + {c}_{m}{\widetilde{\mathbf{\alpha }}}_{m},
$$

从而结论得证.

例 3.13 设 $V$ 是实数域上连续函数全体构成的实线性空间,求证下列函数线性无关:

(1) $\sin x,\sin {2x},\cdots ,\sin {nx}$ ; (2) $1,\cos x,\cos {2x},\cdots ,\cos {nx}$ ;

(3) $1,\sin x,\cos x,\sin {2x},\cos {2x},\cdots ,\sin {nx},\cos {nx}$ .

证法 1 根据向量线性无关的基本性质,我们只要证明 (3) 即可. 对 $n$ 进行归纳. 当 $n = 0$ 时,显然 1 作为一个函数线性无关. 假设命题对小于 $n$ 的自然数成立, 现证明等于 $n$ 的情形. 设

$$
a + {b}_{1}\sin x + {c}_{1}\cos x + {b}_{2}\sin {2x} + {c}_{2}\cos {2x} + \cdots + {b}_{n}\sin {nx} + {c}_{n}\cos {nx} = 0,
$$

其中 $a,{b}_{i},{c}_{i}$ 都是实数. 对上式两次求导,可得

$$
- {b}_{1}\sin x - {c}_{1}\cos x - 4{b}_{2}\sin {2x} - 4{c}_{2}\cos {2x} - \cdots - {n}^{2}{b}_{n}\sin {nx} - {n}^{2}{c}_{n}\cos {nx} = 0,
$$

再将第一个式子乘以 ${n}^{2}$ 加到第二个式子上,可得

$$
a{n}^{2} + \mathop{\sum }\limits_{{i = 1}}^{{n - 1}}{b}_{i}\left( {{n}^{2} - {i}^{2}}\right) \sin {ix} + \mathop{\sum }\limits_{{i = 1}}^{{n - 1}}{c}_{i}\left( {{n}^{2} - {i}^{2}}\right) \cos {ix} = 0,
$$

由归纳假设即得 $a = {b}_{1} = {c}_{1} = \cdots = {b}_{n - 1} = {c}_{n - 1} = 0$ . 将此结论代入第一个式子可得 ${b}_{n}\sin {nx} + {c}_{n}\cos {nx} = 0$ . 若 ${b}_{n} \neq 0\left( {{c}_{n} \neq 0}\right)$ ,则 $\tan {nx} = - {c}_{n}/{b}_{n}$ $\left( {\cot {nx} = - {b}_{n}/{c}_{n}}\right)$ 为常数,矛盾. 因此 ${b}_{n} = {c}_{n} = 0$ .

证法 2 设

$$
f\left( x\right) = a + {b}_{1}\sin x + {c}_{1}\cos x + {b}_{2}\sin {2x} + {c}_{2}\cos {2x} + \cdots + {b}_{n}\sin {nx} + {c}_{n}\cos {nx} = 0,
$$

其中 $a,{b}_{i},{c}_{i}$ 都是实数. 依次设 $g\left( x\right) = 1,\sin x,\cos x,\sin {2x},\cos {2x},\cdots ,\sin {nx},\cos {nx}$ , 并分别计算定积分 ${\int }_{0}^{2\pi }f\left( x\right) g\left( x\right) \mathrm{d}x$ 可得 $a = {b}_{1} = {c}_{1} = \cdots = {b}_{n} = {c}_{n} = 0$ . [

例 3.14 设向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,又

$$
\left\{ \begin{matrix} {\mathbf{\beta }}_{1} = {a}_{11}{\mathbf{\alpha }}_{1} + {a}_{12}{\mathbf{\alpha }}_{2} + \cdots + {a}_{1r}{\mathbf{\alpha }}_{r}, \\ {\mathbf{\beta }}_{2} = {a}_{21}{\mathbf{\alpha }}_{1} + {a}_{22}{\mathbf{\alpha }}_{2} + \cdots + {a}_{2r}{\mathbf{\alpha }}_{r}, \\ \cdots \cdots \cdots \cdots \\ {\mathbf{\beta }}_{r} = {a}_{r1}{\mathbf{\alpha }}_{1} + {a}_{r2}{\mathbf{\alpha }}_{2} + \cdots + {a}_{rr}{\mathbf{\alpha }}_{r}. \end{matrix}\right.
$$

求证: ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 线性相关的充要条件是系数矩阵 $\mathbf{A} = {\left( {a}_{ij}\right) }_{r \times r}$ 的行列式为零.

证明 记 $\mathbf{A}$ 的行向量为 ${\gamma }_{1},{\gamma }_{2},\cdots ,{\gamma }_{r}$ . 若 $\left| \mathbf{A}\right| = 0$ ,则 $\mathbf{A}$ 的行向量线性相关, 即存在不全为零的 $r$ 个数 ${c}_{1},{c}_{2},\cdots ,{c}_{r}$ ,使

$$
{c}_{1}{\gamma }_{1} + {c}_{2}{\gamma }_{2} + \cdots + {c}_{r}{\gamma }_{r} = \mathbf{0}.
$$

经简单计算可得

$$
{c}_{1}{\mathbf{\beta }}_{1} + {c}_{2}{\mathbf{\beta }}_{2} + \cdots + {c}_{r}{\mathbf{\beta }}_{r} = \mathbf{0},
$$

从而 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 线性相关.

反之,若 $\mathbf{A}$ 可逆,如有 ${k}_{1},{k}_{2},\cdots ,{k}_{r}$ ,使

$$
{k}_{1}{\mathbf{\beta }}_{1} + {k}_{2}{\mathbf{\beta }}_{2} + \cdots + {k}_{r}{\mathbf{\beta }}_{r} = \mathbf{0},
$$

将 ${\mathbf{\beta }}_{i}$ 代入,可得以 ${k}_{i}$ 为未知数的线性方程组:

$$
\left\{ \begin{matrix} {a}_{11}{k}_{1} + {a}_{21}{k}_{2} + \cdots + {a}_{r1}{k}_{r} = 0, \\ {a}_{12}{k}_{1} + {a}_{22}{k}_{2} + \cdots + {a}_{r2}{k}_{r} = 0, \\ \cdots \cdots \cdots \cdots \\ {a}_{1r}{k}_{1} + {a}_{2r}{k}_{2} + \cdots + {a}_{rr}{k}_{r} = 0. \end{matrix}\right.
$$

因为 $\mathbf{A}$ 可逆,所以该方程组只有零解,故 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 线性无关.

我们可以得到例 3.14 在计算方面的应用.

例 3.15 设向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性无关,向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 可由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性表示:

$$
\left\{ \begin{array}{l} {\mathbf{\beta }}_{1} = {\mathbf{\alpha }}_{1} + 2{\mathbf{\alpha }}_{2} + 3{\mathbf{\alpha }}_{3}, \\ {\mathbf{\beta }}_{2} = 3{\mathbf{\alpha }}_{1} - {\mathbf{\alpha }}_{2} + 4{\mathbf{\alpha }}_{3}, \\ {\mathbf{\beta }}_{3} = {\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3}. \end{array}\right.
$$

问 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 是否线性无关?

解 通过计算知矩阵

$$
\left( \begin{matrix} 1 & 2 & 3 \\ 3 & - 1 & 4 \\ 0 & 1 & 1 \end{matrix}\right)
$$

的秩等于 3,因此向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 线性无关.

例 3.16 设向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 是齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的一个基础解系,问向量组

$$
{\mathbf{\alpha }}_{1} + 2{\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3},2{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + 2{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3}
$$

是否也是齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的一个基础解系?

解 矩阵

$$
\left( \begin{array}{lll} 1 & 2 & 1 \\ 2 & 1 & 2 \\ 1 & 1 & 1 \end{array}\right)
$$

的秩等于 2 , 不是可逆矩阵, 因此所要判定的向量组线性相关, 不可能是方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的基础解系.

我们还可以将例 3.14 进一步推广为如下有用的命题, 它将文字向量组秩的判定也归结为矩阵秩的计算.

例 3.17 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 是一组线性无关的向量,若向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 可用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表示如下:

$$
\left\{ \begin{matrix} {\mathbf{\beta }}_{1} = {a}_{11}{\mathbf{\alpha }}_{1} + {a}_{12}{\mathbf{\alpha }}_{2} + \cdots + {a}_{1m}{\mathbf{\alpha }}_{m}, \\ {\mathbf{\beta }}_{2} = {a}_{21}{\mathbf{\alpha }}_{1} + {a}_{22}{\mathbf{\alpha }}_{2} + \cdots + {a}_{2m}{\mathbf{\alpha }}_{m}, \\ \cdots \cdots \cdots \cdots \\ {\mathbf{\beta }}_{k} = {a}_{k1}{\mathbf{\alpha }}_{1} + {a}_{k2}{\mathbf{\alpha }}_{2} + \cdots + {a}_{km}{\mathbf{\alpha }}_{m}. \end{matrix}\right.
$$

记表示矩阵 $\mathbf{A} = {\left( {a}_{ij}\right) }_{k \times m}$ . 求证: 向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 的秩等于 $\mathrm{r}\left( \mathbf{A}\right)$ .

证明 设 $\mathrm{r}\left( \mathbf{A}\right) = r$ . 记 $\mathbf{A}$ 的 $k$ 个行向量为 ${\gamma }_{1},{\gamma }_{2},\cdots ,{\gamma }_{k}$ . 不失一般性,可假定 $\mathbf{A}$ 的前 $r$ 个行向量线性无关,其余行向量均可用前 $r$ 个行向量线性表示. 若

$$
{\gamma }_{i} = {c}_{1}{\gamma }_{1} + {c}_{2}{\gamma }_{2} + \cdots + {c}_{r}{\gamma }_{r}
$$

则经过简单计算可得

$$
{c}_{1}{\mathbf{\beta }}_{1} + {c}_{2}{\mathbf{\beta }}_{2} + \cdots + {c}_{r}{\mathbf{\beta }}_{r} = {\mathbf{\beta }}_{i}.
$$

另一方面, 若

$$
{c}_{1}{\mathbf{\beta }}_{1} + {c}_{2}{\mathbf{\beta }}_{2} + \cdots + {c}_{r}{\mathbf{\beta }}_{r} = \mathbf{0},
$$

则

$$
{c}_{1}\left( {{a}_{11}{\mathbf{\alpha }}_{1} + \cdots + {a}_{1m}{\mathbf{\alpha }}_{m}}\right) + \cdots + {c}_{r}\left( {{a}_{r1}{\mathbf{\alpha }}_{1} + \cdots + {a}_{rm}{\mathbf{\alpha }}_{m}}\right) = \mathbf{0},
$$

即

$$
\left( {{c}_{1}{a}_{11} + \cdots + {c}_{r}{a}_{r1}}\right) {\mathbf{\alpha }}_{1} + \cdots + \left( {{c}_{1}{a}_{1m} + \cdots + {c}_{r}{a}_{rm}}\right) {\mathbf{\alpha }}_{m} = \mathbf{0}.
$$

因为 ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关,得

$$
\left\{ \begin{matrix} {a}_{11}{c}_{1} + {a}_{21}{c}_{2} + \cdots + {a}_{r1}{c}_{r} = 0, \\ {a}_{12}{c}_{1} + {a}_{22}{c}_{2} + \cdots + {a}_{r2}{c}_{r} = 0, \\ \cdots \cdots \cdots \cdots \\ {a}_{1m}{c}_{1} + {a}_{2m}{c}_{2} + \cdots + {a}_{rm}{c}_{r} = 0. \end{matrix}\right.
$$

将上述方程组看成是未知数 ${c}_{i}$ 的齐次线性方程组,其系数矩阵的秩为 $r$ ,未知数个数也是 $r$ ,因此只有唯一组解,即零解. 这表明 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 是向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 的极大无关组,因此向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 的秩等于 $r$ . [

下列命题对判断向量组秩的大小是很有用的.

例 3.18 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 是向量空间 $V$ 中一组向量,向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 可用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表出,求证: 向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 的秩小于等于向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的秩.

证明 不失一般性,可设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 是向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的极大无关组, ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}$ 是向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 的极大无关组. 因为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 可用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表出,所以 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}$ 也可用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表出, 故 $s \leq r$ ,结论成立.

注 如果我们将向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 称为原向量组,将向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 称为表出向量组, 则命题可表为: “表出向量组的秩不超过原向量组的秩”. 从几何上看,这是一个自然的结果. 因为每个 ${\mathbf{\beta }}_{i}$ 都属于由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 生成的子空间,故它们的秩不会超过该子空间的维数.

如果我们已知向量组的秩, 那么判定其极大无关组有如下简洁的方法.

例 3.19 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 是向量空间 $V$ 中一组向量且其秩等于 $r,{\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}}$ , $\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是其中 $r$ 个向量. 假定下列条件之一成立:

(1) ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 线性无关;

(2) 任一 ${\mathbf{\alpha }}_{i}$ 均可由 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 线性表示.

求证: ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是向量组的极大无关组.

证明 (1) 设 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 线性无关,又设 ${\mathbf{\alpha }}_{{j}_{1}},{\mathbf{\alpha }}_{{j}_{2}},\cdots ,{\mathbf{\alpha }}_{{j}_{r}}$ 是向量组的极大无关组. 对任意的 $1 \leq i \leq m,{\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}},{\mathbf{\alpha }}_{i}$ 均可由 ${\mathbf{\alpha }}_{{j}_{1}},{\mathbf{\alpha }}_{{j}_{2}},\cdots ,{\mathbf{\alpha }}_{{j}_{r}}$ 线性表示,根据 $§{3.1.3}$ 定理 2 的逆否命题可知 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}},{\mathbf{\alpha }}_{i}$ 必线性相关,再由例 3.7 可知 ${\mathbf{\alpha }}_{i}$ 可由 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 线性表示,从而 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 也是向量组的极大无关组.

(2) 设任一 ${\mathbf{\alpha }}_{i}$ 均可由 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 线性表示. 不失一般性,可设 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}}$ , $\cdots ,{\mathbf{\alpha }}_{{i}_{s}}$ 是向量组 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 的极大无关组. 因此 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{s}}$ 线性无关,再由线性组合的传递性可知,任一 ${\mathbf{\alpha }}_{i}$ 均可由 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{s}}$ 线性表示, 故 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{s}}$ 是原向量组的极大无关组,从而 $s = r$ ,即 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是原向量组的极大无关组.

两组向量称为等价, 若它们可以互相线性表示. 注意向量组的等价与矩阵的等价不是一回事. 两个矩阵 $\mathbf{A}$ 和 $\mathbf{B}$ 等价是指通过初等变换可将 $\mathbf{A}$ 变成 $\mathbf{B}$ . 两个矩阵等价的充要条件是它们具有相同的秩. 但是两个向量组如果只具有相同的秩还不能保证它们等价. 比如 $A = \{ \left( {1,0}\right) \}, B = \{ \left( {0,1}\right) \}$ . 它们的秩都等于 1,但它们不等价. 下面的例题给出了两个向量组等价的充要条件.

例 3.20 设有两个向量组 $A = \left\{ {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}}\right\}$ 和 $B = \left\{ {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right\}$ . 求证: 它们等价的充要条件是它们的秩相等且其中一组向量可以用另外一组向量线性表示.

证明 根据向量组等价的定义可知,只需证明充分性. 假设向量组 $A$ 可用向量组 $B$ 线性表示,现证明向量组 $B$ 也可用向量组 $A$ 线性表示. 不失一般性, 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 是向量组 $A$ 的极大无关组, ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 是向量组 $B$ 的极大无关组. 考虑向量组 $C = \left\{ {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r};{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}}\right\}$ . 因为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 可用 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 线性表出,故 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 是向量组 $C$ 的极大无关组,从而向量组 $C$ 的秩等于 $r$ . 注意到 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,故由例 3.19 可知, ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 也是向量组 $C$ 的极大无关组,从而 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{r}$ 可用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表示. 因此向量组 $B$ 也可用向量组 $A$ 线性表示,故 $A$ 和 $B$ 等价.

例 3.21 设向量 $\mathbf{\beta }$ 可由向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表示,但不能由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots$ , ${\mathbf{\alpha }}_{r - 1}$ 线性表示,问向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 和向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r - 1},\mathbf{\beta }$ 是否等价?

答 等价. 由定义只需证明向量 ${\mathbf{\alpha }}_{r}$ 可由向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r - 1},\mathbf{\beta }$ 线性表示即可. 由已知条件可设

$$
\mathbf{\beta } = {c}_{1}{\mathbf{\alpha }}_{1} + {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{r - 1}{\mathbf{\alpha }}_{r - 1} + {c}_{r}{\mathbf{\alpha }}_{r},
$$

且 ${c}_{r} \neq 0$ (否则向量 $\mathbf{\beta }$ 将可以用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r - 1}$ 线性表示,与已知矛盾). 因此,向量 ${\mathbf{\alpha }}_{r}$ 可由向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r - 1},\mathbf{\beta }$ 线性表示.

## 3.2.2 线性空间及其基

线性空间理论是整个高等代数的核心内容. 因此判断某个集合是否成为线性空间, 如是线性空间, 如何计算其维数或确定其一组基, 这些都是线性空间理论的基石. 在本节中我们将给出这方面的典型例题.

例 3.22 通常的教科书 (如 [1]) 都会提及以下线性空间的典型例子:

(1) 数域 $\mathbb{K}$ 上 $n$ 维行 (列) 向量集合 ${\mathbb{K}}_{n}\left( {\mathbb{K}}^{n}\right)$ 在行 (列) 向量的加法和数乘下成为 $\mathbb{K}$ 上的线性空间,称为数域 $\mathbb{K}$ 上的 $n$ 维行 (列) 向量空间.

(2) 数域 $\mathbb{K}$ 上的一元多项式全体 $\mathbb{K}\left\lbrack x\right\rbrack$ 在多项式的加法和数乘下成为 $\mathbb{K}$ 上的线性空间. 在 $\mathbb{K}\left\lbrack x\right\rbrack$ 中,取次数小于等于 $n$ 的多项式全体,记这个集合为 ${\mathbb{K}}_{n}\left\lbrack x\right\rbrack$ ,则 ${\mathbb{K}}_{n}\left\lbrack x\right\rbrack$ 也是 $\mathbb{K}$ 上的线性空间.

(3) 数域 $\mathbb{K}$ 上 $m \times n$ 矩阵全体 ${M}_{m \times n}\left( \mathbb{K}\right)$ 在矩阵的加法与数乘下成为 $\mathbb{K}$ 上的线性空间.

(4) 若两个数域 ${\mathbb{K}}_{1} \subseteq {\mathbb{K}}_{2}$ ,则 ${\mathbb{K}}_{2}$ 可以看成是 ${\mathbb{K}}_{1}$ 上的线性空间. 向量就是 ${\mathbb{K}}_{2}$ 中的数,向量的加法就是数的加法,数乘就是 ${\mathbb{K}}_{1}$ 中的数乘以 ${\mathbb{K}}_{2}$ 中的数. 特别地,数域 $\mathbb{K}$ 也可以看成是 $\mathbb{K}$ 自身上的线性空间.

(5) 实数域 $\mathbb{R}$ 上的连续函数全体记为 $C\left( \mathbb{R}\right)$ ,函数的加法及数乘分别定义为 $\left( {f + g}\right) \left( x\right) = f\left( x\right) + g\left( x\right) ,\left( {kf}\right) \left( x\right) = {kf}\left( x\right)$ ,则 $C\left( \mathbb{R}\right)$ 是 $\mathbb{R}$ 上的线性空间.

在上面的例子中, 列举的线性空间及其运算 (加法和数乘) 在某种意义下都是标准的. 然而下面的例题却告诉我们, 某些特殊的集合或者常见线性空间上还可以定义一些特殊的加法或数乘, 它们或者是或者不是线性空间. 这足以反映线性空间这一概念的广泛包容性.

例 3.23 判断下列集合是否构成实数域 $\mathbb{R}$ 上的线性空间:

(1) $V$ 为次数等于 $n\left( {n \geq 1}\right)$ 的实系数多项式全体,加法和数乘就是多项式的加法和数乘.

(2) $V = {M}_{n}\left( \mathbb{R}\right)$ ,数乘就是矩阵的数乘,加法 $\oplus$ 定义为 $\mathbf{A} \oplus \mathbf{B} = \mathbf{A}\mathbf{B} - \mathbf{B}\mathbf{A}$ ,其中等式右边是矩阵的乘法和减法.

(3) $V = {M}_{n}\left( \mathbb{R}\right)$ ,数乘就是矩阵的数乘,加法 $\oplus$ 定义为 $\mathbf{A} \oplus \mathbf{B} = \mathbf{A}\mathbf{B} + \mathbf{B}\mathbf{A}$ ,其中等式右边是矩阵的乘法和加法.

(4) $V$ 是以 0 为极限的实数数列全体,即 $V = \left\{ {\left\{ {a}_{n}\right\} \mid \mathop{\lim }\limits_{{n \rightarrow \infty }}{a}_{n} = 0}\right\}$ ,定义两个数列的加法 $\oplus$ 及数乘 $\circ$ 为: $\left\{ {a}_{n}\right\} \oplus \left\{ {b}_{n}\right\} = \left\{ {{a}_{n} + {b}_{n}}\right\}, k \circ \left\{ {a}_{n}\right\} = \left\{ {k{a}_{n}}\right\}$ ,其中等式右边分别是数的加法和乘法.

(5) $V$ 是正实数全体 ${\mathbb{R}}^{ + }$ ,加法 $\oplus$ 定义为 $a \oplus b = {ab}$ ,数乘 $\circ$ 定义为 $k \circ a = {a}^{k}$ , 其中等式右边分别是数的乘法和乘方.

(6) $V$ 为实数对全体 $\{ \left( {a, b}\right) \mid a, b \in \mathbb{R}\}$ ,加法 $\oplus$ 定义为 $\left( {{a}_{1},{b}_{1}}\right) \oplus \left( {{a}_{2},{b}_{2}}\right) =$ $\left( {{a}_{1} + {a}_{2},{b}_{1} + {b}_{2} + {a}_{1}{a}_{2}}\right)$ ,数乘 $\circ$ 定义为 $k \circ \left( {a, b}\right) = \left( {{ka},{kb} + \frac{k\left( {k - 1}\right) }{2}{a}^{2}}\right)$ .

解 (1) $V$ 不是线性空间,因为加法不封闭.

(2) $V$ 不是线性空间,因为加法不满足交换律,即 $\mathbf{A} \oplus \mathbf{B} \neq \mathbf{B} \oplus \mathbf{A}$ .

(3) $V$ 不是线性空间,因为加法不满足结合律,即 $\left( {\mathbf{A} \oplus \mathbf{B}}\right) \oplus \mathbf{C} \neq \mathbf{A}\left( {\oplus \mathbf{B} \oplus \mathbf{C}}\right)$ .

(4)、(5)、(6) $V$ 都是线性空间,特别是 (5) 和 (6),其加法和数乘的定义都不是线性的, 但它们竟然都是线性空间! 请读者自己验证线性空间的 8 条性质的确成立, 在下一节我们会从线性同构的角度来说明它们成为线性空间的深层次理由.

如果考虑的向量族是整个线性空间 $V$ ,那么其极大无关组就称为线性空间 $V$ 的一组基. 因此要验证 $V$ 中若干个向量是否组成 $V$ 的一组基必须验证两点: 一是它们线性无关,二是 $V$ 中任意一个向量均可以表示为这些向量的线性组合. 但是如果已经知道 $V$ 的维数为 $n$ ,而所要验证的向量恰为 $n$ 个,则我们可以用下面的命题.

例 3.24 设 $V$ 是 $n$ 维线性空间, ${e}_{1},{e}_{2},\cdots ,{e}_{n}$ 是 $V$ 中的 $n$ 个向量. 若它们适合下列条件之一,则 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 是 $V$ 的一组基.

(1) ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 线性无关;

(2) $V$ 中的向量均可由 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 线性表示.

证明 完全类似于例 3.19 的证明.

下面的命题通常称为基扩张定理, 它在后面会经常用到.

例 3.25 设 $V$ 是 $n$ 维线性空间, ${v}_{1},{v}_{2},\cdots ,{v}_{m}$ 是一组线性无关的向量 (是 $V$ 的子空间 $U$ 的一组基),又 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 是 $V$ 的基,则必可在 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 中选出 $n - m$ 个向量,使之和 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{m}$ 一起组成 $V$ 的一组基.

证明 将 ${\mathbf{e}}_{i}\left( {i = 1,\cdots, n}\right)$ 依次放入向量组 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{m}$ ,则必有一个 ${\mathbf{e}}_{i}$ , 使 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{m},{\mathbf{e}}_{i}$ 线性无关. 这是因为若任意一个 ${\mathbf{e}}_{i}$ 加入 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{m}$ 后线性相关,则每个 ${\mathbf{e}}_{i}$ 都可用 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{m}$ 线性表示,将和例 3.18 的结论矛盾. 现不妨设 $i = m + 1$ . 若 $m + 1 < n$ ,又可从 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 中找到一个向量,加入进去以后仍线性无关. 不断这样做下去,便可将 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{m}$ 扩张成为 $V$ 的一组基. [

容易验证 $n$ 维标准单位行 (列) 向量是数域 $\mathbb{K}$ 上的 $n$ 维行 (列) 向量空间的一组基. 下面我们接着给出一些常见线性空间的基向量的例子.

例 3.26 设 $V$ 是数域 $\mathbb{K}$ 上次数不超过 $n$ 的多项式全体构成的线性空间,求证: $\left\{ {1, x,{x}^{2},\cdots ,{x}^{n}}\right\}$ 是 $V$ 的一组基,并且 $\left\{ {1, x + 1,{\left( x + 1\right) }^{2},\cdots ,{\left( x + 1\right) }^{n}}\right\}$ 也是 $V$ 的一组基.

证明 根据多项式的定义容易验证 $\left\{ {1, x,{x}^{2},\cdots ,{x}^{n}}\right\}$ 是 $V$ 的一组基,特别地, $\dim V = n + 1$ . 对任意的 $f\left( x\right) \in V$ ,设 $y = x + 1$ ,则

$$
f\left( x\right) = f\left( {y - 1}\right) = {b}_{n}{y}^{n} + \cdots + {b}_{1}y + {b}_{0} = {b}_{n}{\left( x + 1\right) }^{n} + \cdots + {b}_{1}\left( {x + 1}\right) + {b}_{0},
$$

其中 ${b}_{n},\cdots ,{b}_{1},{b}_{0}$ 是 $\mathbb{K}$ 中的数. 因此 $V$ 中任一多项式 $f\left( x\right)$ 均可由 $1, x + 1,(x +$ $1{)}^{2},\cdots ,{\left( x + 1\right) }^{n}$ 线性表示,由例 3.24 知, $\left\{ {1, x + 1,{\left( x + 1\right) }^{2},\cdots ,{\left( x + 1\right) }^{n}}\right\}$ 是 $V$ 的一组基.

例 3.27 设 $V$ 是由数域 $\mathbb{K}$ 上次数小于 $n$ 的多项式全体构成的线性空间, ${a}_{i}\left( {i = 1,2,\cdots, n}\right)$ 是 $\mathbb{K}$ 中互不相同的 $n$ 个数, $f\left( x\right) = \left( {x - {a}_{1}}\right) \left( {x - {a}_{2}}\right) \cdots \left( {x - {a}_{n}}\right)$ , ${f}_{i}\left( x\right) = f\left( x\right) /\left( {x - {a}_{i}}\right)$ ,求证: $\left\{ {{f}_{i}\left( x\right) \left( {i = 1,2,\cdots, n}\right) }\right\}$ 组成 $V$ 的一组基.

证明 因为 $V$ 是 $n$ 维线性空间,故由例 3.24 只需证明 $n$ 个向量 ${f}_{i}\left( x\right) (i =$ $1,2,\cdots, n)$ 线性无关即可. 设

$$
{k}_{1}{f}_{1}\left( x\right) + {k}_{2}{f}_{2}\left( x\right) + \cdots + {k}_{n}{f}_{n}\left( x\right) = 0,
$$

依次令 $x = {a}_{1},{a}_{2},\cdots ,{a}_{n}$ ,即可求出 ${k}_{1} = {k}_{2} = \cdots = {k}_{n} = 0$ .

例 3.28 设 $V$ 是数域 $\mathbb{K}$ 上 $m \times n$ 矩阵组成的线性空间,令 ${\mathbf{E}}_{ij}(i = 1,2,\cdots, m$ ; $j = 1,2,\cdots, n)$ 是第 $\left( {i, j}\right)$ 元素为 1 、其余元素为 0 的 $m \times n$ 矩阵,求证: 全体 ${\mathbf{E}}_{ij}$ 组成了 $V$ 的一组基,因而 $V$ 是 ${mn}$ 维线性空间.

证明 一方面,对任意的 $\mathbf{A} = \left( {a}_{ij}\right) \in V$ ,容易验证 $\mathbf{A} = \mathop{\sum }\limits_{{i = 1}}^{m}\mathop{\sum }\limits_{{j = 1}}^{n}{a}_{ij}{\mathbf{E}}_{ij}$ . 另一方面,设 ${mn}$ 个数 ${c}_{ij}\left( {1 \leq i \leq m,1 \leq j \leq n}\right)$ 满足 $\mathop{\sum }\limits_{{i = 1}}^{m}\mathop{\sum }\limits_{{j = 1}}^{n}{c}_{ij}{\mathbf{E}}_{ij} = \mathbf{O}$ ,则由矩阵相等的定义可得所有的 ${c}_{ij} = 0$ . 因此全体 ${\mathbf{E}}_{ij}$ 组成了 $V$ 的一组基,特别地, $\dim V = {mn}$ .

例 3.29 求下列线性空间 $V$ 的维数:

(1) $V$ 是数域 $\mathbb{K}$ 上 $n$ 阶上三角矩阵全体组成的线性空间;

(2) $V$ 是数域 $\mathbb{K}$ 上 $n$ 阶对称矩阵全体组成的线性空间;

(3) $V$ 是数域 $\mathbb{K}$ 上 $n$ 阶反对称矩阵全体组成的线性空间.

解 (1) 容易验证 $\left\{ {{\mathbf{E}}_{ij}\left( {1 \leq i \leq j \leq n}\right) }\right\}$ 是 $V$ 的一组基,因此 $\dim V =$ $\frac{n\left( {n + 1}\right) }{2}$ .

(2) 容易验证 $\left\{ {{\mathbf{E}}_{ii}\left( {1 \leq i \leq n}\right) ;{\mathbf{E}}_{ij} + {\mathbf{E}}_{ji}\left( {1 \leq i < j \leq n}\right) }\right\}$ 是 $V$ 的一组基,因此 $\dim V = \frac{n\left( {n + 1}\right) }{2}$ .

(3) 容易验证 $\left\{ {{\mathbf{E}}_{ij} - {\mathbf{E}}_{ji}\left( {1 \leq i < j \leq n}\right) }\right\}$ 是 $V$ 的一组基,因此 $\dim V =$ $\frac{n\left( {n - 1}\right) }{2}$ . $\square$

例 3.30 设 ${V}_{1} = \left\{ {\mathbf{A} \in {M}_{n}\left( \mathbb{C}\right) \mid {\overline{\mathbf{A}}}^{\prime } = \mathbf{A}}\right\}$ 为 $n$ 阶 Hermite 矩阵全体, ${V}_{2} =$ $\left\{ {\mathbf{A} \in {M}_{n}\left( \mathbb{C}\right) \mid {\overline{\mathbf{A}}}^{\prime } = - \mathbf{A}}\right\}$ 为 $n$ 阶斜 Hermite 矩阵全体,求证: 在矩阵加法和实数关于矩阵的数乘下, ${V}_{1},{V}_{2}$ 成为实数域 $\mathbb{R}$ 上的线性空间,并且具有相同的维数.

证明 首先,容易证明对任意的 $\mathbf{A},\mathbf{B} \in {V}_{i}, c \in \mathbb{R}$ ,我们有 $\mathbf{A} + \mathbf{B} \in {V}_{i}, c\mathbf{A} \in {V}_{i}$ , 这就验证了上述加法和数乘是定义好的运算. 其次, 容易验证线性空间的 8 条性质成立,因此 ${V}_{1},{V}_{2}$ 是实线性空间 (注意虽然向量都是复矩阵,但它们绝不是复线性空间). 最后,容易验证 $\left\{ {{\mathbf{E}}_{ii}\left( {1 \leq i \leq n}\right) ;{\mathbf{E}}_{ij} + {\mathbf{E}}_{ji}\left( {1 \leq i < j \leq n}\right) ;\mathrm{i}{\mathbf{E}}_{ij} - \mathrm{i}{\mathbf{E}}_{ji}(1 \leq i < j \leq }\right.$ $\left. n\right\}$ 是 ${V}_{1}$ 的一组基, $\left\{ {\mathrm{i}{\mathbf{E}}_{ii}\left( {1 \leq i \leq n}\right) ;{\mathbf{E}}_{ij} - {\mathbf{E}}_{ji}\left( {1 \leq i < j \leq n}\right) ;\mathrm{i}{\mathbf{E}}_{ij} + \mathrm{i}{\mathbf{E}}_{ji}(1 \leq }\right.$ $i < j \leq n)\}$ 是 ${V}_{2}$ 的一组基,因此 ${\dim }_{\mathbb{R}}{V}_{1} = {\dim }_{\mathbb{R}}{V}_{2} = {n}^{2}$ .

例 3.31 设 $\mathbb{Q}\left( \sqrt[3]{2}\right) = \{ a + b\sqrt[3]{2} + c\sqrt[3]{4}\}$ ,其中 $a, b, c$ 均是有理数,证明 $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 是有理数域上的线性空间并求其维数.

证明 事实上,我们可以证明 $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 是一个数域. 加法、减法和乘法的封闭性都是显然的, 我们只要证明除法封闭, 或等价地证明非零数的倒数封闭即可. 为此首先需要找出一个数非零的充要条件. 我们断言以下 3 个结论等价:

(1) $a + b\sqrt[3]{2} + c\sqrt[3]{4} = 0$ ; (2) ${a}^{3} + 2{b}^{3} + 4{c}^{3} - {6abc} = 0$ ; (3) $a = b = c = 0$ .

由公式 $\left( {x + y + z}\right) \left( {{x}^{2} + {y}^{2} + {z}^{2} - {xy} - {yz} - {zx}}\right) = {x}^{3} + {y}^{3} + {z}^{3} - {3xyz}$ 很容易从 (1) 推出 (2). 假设 (2) 对不全为零的有理数 $a, b, c$ 成立,将 (2) 式两边同时乘以 $a, b, c$ 公分母的立方,可将 $a, b, c$ 化为整数; 又可将整数 $a, b, c$ 的最大公因数从 (2) 式提出,因此不妨假设满足 (2) 式的 $a, b, c$ 是互素的整数. 由 (2) 式可得 $a$ 是偶数, 可设 $a = 2{a}_{1}$ ,代入 (2) 式可得 $\left( {2}^{\prime }\right) 4{a}_{1}^{3} + {b}^{3} + 2{c}^{3} - 6{a}_{1}{bc} = 0$ ; 由 $\left( {2}^{\prime }\right)$ 式可得 $b$ 是偶数,可设 $b = 2{b}_{1}$ ,代入 $\left( {2}^{\prime }\right)$ 式可得 $\left( {2}^{\prime \prime }\right) 2{a}_{1}^{3} + 4{b}_{1}^{3} + {c}^{3} - 6{a}_{1}{b}_{1}c = 0$ ; 由 $\left( {2}^{\prime \prime }\right)$ 式可得 $c$ 是偶数,可设 $c = 2{c}_{1}$ ,这样 $a, b, c$ 就有了公因子 2,这与它们互素矛盾. 因此从 (2) 可以推出 (3). 从 (3) 推出 (1) 是显然的.

任取 $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 中的非零数 $a + b\sqrt[3]{2} + c\sqrt[3]{4}$ ,由上述充要条件以及公式可得

$$
\left( {a + b\sqrt[3]{2} + c\sqrt[3]{4}}\right) \left\lbrack {\left( {{a}^{2} - {2bc}}\right) + \left( {2{c}^{2} - {ab}}\right) \sqrt[3]{2} + \left( {{b}^{2} - {ac}}\right) \sqrt[3]{4}}\right\rbrack = {a}^{3} + 2{b}^{3} + 4{c}^{3} - {6abc} \neq 0,
$$

从而 $\left( {{a}^{2} - {2bc}}\right) + \left( {2{c}^{2} - {ab}}\right) \sqrt[3]{2} + \left( {{b}^{2} - {ac}}\right) \sqrt[3]{4} \neq 0$ . 将倒数 $\frac{1}{\left( a + b\sqrt[3]{2} + c\sqrt[3]{4}\right) }$ 的分子分母同时乘以非零数 $\left( {{a}^{2} - {2bc}}\right) + \left( {2{c}^{2} - {ab}}\right) \sqrt[3]{2} + \left( {{b}^{2} - {ac}}\right) \sqrt[3]{4}$ 进行化简,可得

$$
\frac{1}{a + b\sqrt[3]{2} + c\sqrt[3]{4}} = \frac{\left( {{a}^{2} - {2bc}}\right) + \left( {2{c}^{2} - {ab}}\right) \sqrt[3]{2} + \left( {{b}^{2} - {ac}}\right) \sqrt[3]{4}}{{a}^{3} + 2{b}^{3} + 4{c}^{3} - {6abc}} \in \mathbb{Q}\left( \sqrt[3]{2}\right) .
$$

这就证明了 $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 是一个数域. 因为 $\mathbb{Q} \subseteq \mathbb{Q}\left( \sqrt[3]{2}\right)$ ,故由例 3.22 可知 $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 是有理数域上的线性空间.

由 $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 的定义可知, $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 中每个数都是 $1,\sqrt[3]{2},\sqrt[3]{4}$ 的 $\mathbb{Q}$ -线性组合; 又由上述充要条件可知, $1,\sqrt[3]{2},\sqrt[3]{4}$ 是 $\mathbb{Q}$ -线性无关的. 因此 $\{ 1,\sqrt[3]{2},\sqrt[3]{4}\}$ 是 $\mathbb{Q}\left( \sqrt[3]{2}\right)$ 的一组基,特别地, ${\dim }_{\mathbb{Q}}\mathbb{Q}\left( \sqrt[3]{2}\right) = 3$ .

* 例 3.32 设 ${\mathbb{K}}_{1},{\mathbb{K}}_{2},{\mathbb{K}}_{3}$ 是数域且 ${\mathbb{K}}_{1} \subseteq {\mathbb{K}}_{2} \subseteq {\mathbb{K}}_{3}$ ,若将 ${\mathbb{K}}_{2}$ 看成是 ${\mathbb{K}}_{1}$ 上的线性空间,其维数为 $m$ ,又将 ${\mathbb{K}}_{3}$ 看成是 ${\mathbb{K}}_{2}$ 上的线性空间,其维数为 $n$ ,求证: 如将 ${\mathbb{K}}_{3}$ 看成是 ${\mathbb{K}}_{1}$ 上的线性空间,则其维数为 ${mn}$ .

证明 ${\mathbb{K}}_{2}$ 作为 ${\mathbb{K}}_{1}$ 上的线性空间,取其一组基为 $\left\{ {{\alpha }_{1},{\alpha }_{2},\cdots ,{\alpha }_{m}}\right\} ;{\mathbb{K}}_{3}$ 作为 ${\mathbb{K}}_{2}$ 上的线性空间,取其一组基为 $\left\{ {{\beta }_{1},{\beta }_{2},\cdots ,{\beta }_{n}}\right\}$ . 注意到 ${\alpha }_{i},{\beta }_{j}$ 都是数,现在我们断言: ${\mathbb{K}}_{3}$ 作为 ${\mathbb{K}}_{1}$ 上的线性空间, $\left\{ {{\alpha }_{i}{\beta }_{j} \mid 1 \leq i \leq m,1 \leq j \leq n}\right\}$ 恰为其一组基.

一方面,对 ${\mathbb{K}}_{3}$ 中任一数 $a$ ,存在 ${\mathbb{K}}_{2}$ 中的数 ${b}_{1},{b}_{2},\cdots ,{b}_{n}$ ,使得

$$
a = {b}_{1}{\beta }_{1} + {b}_{2}{\beta }_{2} + \cdots + {b}_{n}{\beta }_{n}
$$

又对 ${b}_{j} \in {\mathbb{K}}_{2}$ ,存在 ${\mathbb{K}}_{1}$ 中的数 ${c}_{1j},{c}_{2j},\cdots ,{c}_{mj}$ ,使得

$$
{b}_{j} = {c}_{1j}{\alpha }_{1} + {c}_{2j}{\alpha }_{2} + \cdots + {c}_{mj}{\alpha }_{m}, j = 1,2,\cdots, n.
$$

将上述两式进行整理, 可得

$$
a = \mathop{\sum }\limits_{{j = 1}}^{n}{b}_{j}{\beta }_{j} = \mathop{\sum }\limits_{{j = 1}}^{n}\left( {\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{ij}{\alpha }_{i}}\right) {\beta }_{j} = \mathop{\sum }\limits_{{j = 1}}^{n}\mathop{\sum }\limits_{{i = 1}}^{m}{c}_{ij}{\alpha }_{i}{\beta }_{j},
$$

即 ${\mathbb{K}}_{3}$ 中任一数均可由 $\left\{ {{\alpha }_{i}{\beta }_{j} \mid 1 \leq i \leq m,1 \leq j \leq n}\right\}$ 线性表示.

另一方面,设有 ${\mathbb{K}}_{1}$ 中的数 ${k}_{ij}\left( {1 \leq i \leq m,1 \leq j \leq n}\right)$ ,使得

$$
\mathop{\sum }\limits_{{j = 1}}^{n}\mathop{\sum }\limits_{{i = 1}}^{m}{k}_{ij}{\alpha }_{i}{\beta }_{j} = 0
$$

则经过变形可得

$$
\mathop{\sum }\limits_{{j = 1}}^{n}\left( {\mathop{\sum }\limits_{{i = 1}}^{m}{k}_{ij}{\alpha }_{i}}\right) {\beta }_{j} = 0
$$

注意到 $\mathop{\sum }\limits_{{i = 1}}^{m}{k}_{ij}{\alpha }_{i} \in {\mathbb{K}}_{2}$ 且 ${\beta }_{1},{\beta }_{2},\cdots ,{\beta }_{n}$ 是 ${\mathbb{K}}_{3}/{\mathbb{K}}_{2}$ 的一组基,故有 $\mathop{\sum }\limits_{{i = 1}}^{m}{k}_{ij}{\alpha }_{i} = 0(1 \leq$ $j \leq n)$ . 又因为 $\left\{ {{\alpha }_{1},{\alpha }_{2},\cdots ,{\alpha }_{m}}\right\}$ 是 ${\mathbb{K}}_{2}/{\mathbb{K}}_{1}$ 的一组基,故有 ${k}_{ij} = 0(1 \leq i \leq m,1 \leq$ $j \leq n)$ ,即 $\left\{ {{\alpha }_{i}{\beta }_{j} \mid 1 \leq i \leq m,1 \leq j \leq n}\right\}$ 是 ${\mathbb{K}}_{1}$ -线性无关的.

综上所述, $\left\{ {{\alpha }_{i}{\beta }_{j} \mid 1 \leq i \leq m,1 \leq j \leq n}\right\}$ 是 ${\mathbb{K}}_{3}/{\mathbb{K}}_{1}$ 的一组基,特别地, ${\dim }_{{\mathbb{K}}_{1}}{\mathbb{K}}_{3} = {mn} = {\dim }_{{\mathbb{K}}_{1}}{\mathbb{K}}_{2} \cdot {\dim }_{{\mathbb{K}}_{2}}{\mathbb{K}}_{3}.$

例 3.33 证明下列线性空间是实数域上的无限维线性空间:

(1) 实数域 $\mathbb{R}$ 上的连续函数全体构成的线性空间 $C\left( \mathbb{R}\right)$ (见例 3.22 (5));

(2) 以 0 为极限的实数数列全体构成的线性空间 $V = \left\{ {\left\{ {a}_{n}\right\} \mid \mathop{\lim }\limits_{{n \rightarrow \infty }}{a}_{n} = 0}\right\}$ (见例 ${3.23}\left( 4\right) )$ .

证明 我们用反证法来证明.

(1) 若 $C\left( \mathbb{R}\right)$ 是有限维线性空间,则可取到正整数 $k > \dim C\left( \mathbb{R}\right)$ . 然而由例 3.13 可知 $\sin x,\sin {2x},\cdots ,\sin {kx}$ 是 $\mathbb{R}$ -线性无关的,矛盾.

(2) 若 $V$ 是有限维线性空间,则可取到正整数 $k > \dim V$ . 构造 $V$ 中 $k$ 个数列:

$$
\left\{ {{a}_{n}^{\left( 1\right) } = \frac{1}{n}}\right\} ,\left\{ {{a}_{n}^{\left( 2\right) } = \frac{1}{{n}^{2}}}\right\} ,\cdots ,\left\{ {{a}_{n}^{\left( k\right) } = \frac{1}{{n}^{k}}}\right\} .
$$

设有实数 ${c}_{1},{c}_{2},\cdots ,{c}_{k}$ ,使得

$$
{c}_{1}\left\{ {a}_{n}^{\left( 1\right) }\right\} + {c}_{2}\left\{ {a}_{n}^{\left( 2\right) }\right\} + \cdots + {c}_{k}\left\{ {a}_{n}^{\left( k\right) }\right\} = \{ 0\}
$$

则对于任意的正整数 $n$ ,成立

$$
\frac{{c}_{1}}{n} + \frac{{c}_{2}}{{n}^{2}} + \cdots + \frac{{c}_{k}}{{n}^{k}} = 0.
$$

任取 $k$ 个不同的正整数代入上式,并利用 Vander Monde 行列式即得 ${c}_{1} = {c}_{2} =$ $\cdots = {c}_{k} = 0$ ,从而上述 $k$ 个数列线性无关,矛盾.

事实上, 对于无限维线性空间也可以定义基的概念. 首先需要适当地修改线性无关和线性表示的定义, 然后就可以利用选择公理或 Zorn 引理来证明任意线性空间中基向量的存在性了. 由于高等代数主要研究有限维线性空间理论, 故我们不对上述内容做进一步的展开, 有兴趣的读者可以参考相关的教材. 虽然如此, 但在本书中, 我们还是会适当地强调有限维线性空间和无限维线性空间在某些性质上的巨大差异, 这些讨论将为我们学习后续课程提供几何上的想象和例证.

## 3.2.3 线性同构和几何问题代数化

同一个数域 $\mathbb{K}$ 上的两个线性空间 $V, U$ 是线性同构的,即存在一个一一对应 $\varphi : V \rightarrow U$ ,使得 $\varphi$ 保持前后两个线性空间的代数运算 (加法和数乘). 因此线性同构的两个线性空间实际上具有相同的代数结构 (即线性结构),从而 $\varphi$ 保持对应向量组的线性关系和秩,特别地, $V$ 和 $U$ 具有相同的维数 (参考 $§{3.1.3}$ 定理 5).

我们先来看几个线性同构的例子.

例 3.34 验证下列映射是线性同构:

(1) 一维实行向量空间 $\mathbb{R}$ ,例 3.23 (5) 中的实线性空间 ${\mathbb{R}}^{ + }$ ,映射 $\varphi : \mathbb{R} \rightarrow {\mathbb{R}}^{ + }$ 定义为 $\varphi \left( x\right) = {\mathrm{e}}^{x}$ ;

(2) 二维实行向量空间 ${\mathbb{R}}_{2}$ ,例 3.23 (6) 中的实线性空间 $V$ ,映射 $\varphi : {\mathbb{R}}_{2} \rightarrow V$ 定义为 $\varphi \left( {a, b}\right) = \left( {a, b + \frac{1}{2}{a}^{2}}\right)$ .

解 (1) $\varphi$ 的逆映射是 $\psi : {\mathbb{R}}^{ + } \rightarrow \mathbb{R},\psi \left( y\right) = \ln y$ ,故 $\varphi$ 是一一对应. 根据加法和数乘的定义可得

$$
\varphi \left( {x + y}\right) = {\mathrm{e}}^{x + y} = {\mathrm{e}}^{x}{\mathrm{e}}^{y} = \varphi \left( x\right) \oplus \varphi \left( y\right) ,\varphi \left( {kx}\right) = {\mathrm{e}}^{kx} = {\left( {\mathrm{e}}^{x}\right) }^{k} = k \circ \varphi \left( x\right) ,
$$

因此 $\varphi : \mathbb{R} \rightarrow {\mathbb{R}}^{ + }$ 是线性同构.

(2) $\varphi$ 的逆映射是 $\psi : V \rightarrow {\mathbb{R}}_{2},\psi \left( {x, y}\right) = \left( {x, y - \frac{{x}^{2}}{2}}\right)$ ,故 $\varphi$ 是一一对应. 根据具体的计算可得

$$
\varphi \left( {{a}_{1} + {a}_{2},{b}_{1} + {b}_{2}}\right) = \varphi \left( {{a}_{1},{b}_{1}}\right) \oplus \varphi \left( {{a}_{2},{b}_{2}}\right) ,\varphi \left( {{ka},{kb}}\right) = k \circ \varphi \left( {a, b}\right) ,
$$

因此 $\varphi : {\mathbb{R}}_{2} \rightarrow V$ 是线性同构.

注 从上例可以看出, 例 3.23 (5) 和 (6) 中的对象和常见的线性空间之间存在着线性同构, 所以即使它们的加法和数乘定义得极其不自然 (并非线性定义), 但仍可使它们成为线性空间.

例 3.35 构造下列线性空间之间的线性同构:

(1) $V$ 是数域 $\mathbb{K}$ 上的 $n$ 阶上三角矩阵构成的线性空间, $U$ 是数域 $\mathbb{K}$ 上的 $n$ 阶对称矩阵构成的线性空间 (参考例 3.29);

(2) $V$ 是 $n$ 阶 Hermite 矩阵构成的实线性空间, $U$ 是 $n$ 阶斜 Hermite 矩阵构成的实线性空间 (参考例 3.30).

解 (1) $\varphi : V \rightarrow U$ 定义为: 对任意的 $\mathbf{A} = \left( {a}_{ij}\right) \in V$ ,当 $i \leq j$ 时,矩阵 $\varphi \left( \mathbf{A}\right)$ 的第 $\left( {i, j}\right)$ 元素为 ${a}_{ij}$ ; 当 $i > j$ 时,矩阵 $\varphi \left( \mathbf{A}\right)$ 的第 $\left( {i, j}\right)$ 元素为 ${a}_{ji}$ . 容易验证 $\varphi : V \rightarrow U$ 是定义好的映射,并且是数域 $\mathbb{K}$ 上的线性同构.

(2) $\varphi : V \rightarrow U$ 定义为: 对任意的 $\mathbf{A} = \left( {a}_{ij}\right) \in V,\varphi \left( \mathbf{A}\right) = \mathrm{i}\mathbf{A}$ . 容易验证 $\varphi : V \rightarrow U$ 是定义好的映射,并且是实数域上的线性同构. 注意到 $\varphi$ 的逆映射 $\psi : U \rightarrow V$ 为: $\psi \left( \mathbf{B}\right) = - \mathrm{i}\mathbf{B}$ .

我们还有一类特别重要的线性同构. 设 $V$ 是数域 $\mathbb{K}$ 上的 $n$ 维线性空间, $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\}$ 是 $V$ 的一组基并固定次序. 对任一向量 $\mathbf{\alpha } \in V$ ,设 $\mathbf{\alpha } = {\lambda }_{1}{\mathbf{e}}_{1} +$ ${\lambda }_{2}{\mathbf{e}}_{2} + \cdots {\lambda }_{n}{\mathbf{e}}_{n}$ ,则映射 $\mathbf{\eta } : V \rightarrow {\mathbb{K}}^{n}$ 定义为: $\mathbf{\eta }\left( \mathbf{\alpha }\right) = {\left( {\lambda }_{1},{\lambda }_{2},\cdots ,{\lambda }_{n}\right) }^{\prime }$ ,即 $\mathbf{\eta }$ 将 $V$ 中向量映射到它在给定基下的坐标向量. 容易验证 $\eta : V \rightarrow {\mathbb{K}}^{n}$ 是一个线性同构. 因此通过这个线性同构,我们可将抽象的线性空间 $V$ 和具体的列向量空间 ${\mathbb{K}}^{n}$ 等同起来. 进一步,将 $§{3.1.3}$ 定理 5 运用到线性同构 $\eta$ 上,我们可以得到如下重要的定理.

定理 假设和记号同上,设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m},\mathbf{\beta }$ 是 $V$ 中向量,它们在给定基下的坐标向量记为 ${\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{m},\widetilde{\mathbf{\beta }}$ ,则

(1) ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关的充要条件是 ${\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{m}$ 线性无关.

(2) $\mathbf{\beta }$ 可以用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表示的充要条件是 $\widetilde{\mathbf{\beta }}$ 可以用 ${\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{m}$ 线性表示.

(3) ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的极大无关组的充要条件是 ${\widetilde{\mathbf{\alpha }}}_{{i}_{1}}$ , ${\widetilde{\mathbf{\alpha }}}_{{i}_{2}},\cdots ,{\widetilde{\mathbf{\alpha }}}_{{i}_{r}}$ 是向量组 ${\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{m}$ 的极大无关组. 特别地,我们有

$$
\mathrm{r}\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}}\right) = \mathrm{r}\left( {{\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{m}}\right) .
$$

由上述定理,我们可以将抽象线性空间 $V$ 中向量组线性关系的判定和秩的计算转化为具体列向量空间 ${\mathbb{K}}^{n}$ 中由它们的坐标向量构成的列向量组线性关系的判定和秩的计算. 由于后者通常可以通过矩阵的方法来处理, 故上述过程被称为 “几何问题代数化”. 接下来我们将给出几个典型例题, 体会一下 “几何问题代数化” 这一技巧.

例 3.17 的证法 2 令 $V$ 是由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 生成的向量空间. 因为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots$ , ${\mathbf{\alpha }}_{m}$ 线性无关,故它们组成 $V$ 的一组基, $V$ 的维数等于 $m$ . 注意到 ${\mathbf{\beta }}_{i}$ 在这组基

下的坐标向量为 ${\left( {a}_{i1},{a}_{i2},\cdots ,{a}_{im}\right) }^{\prime }$ ,故这些列向量组成的矩阵就是 ${\mathbf{A}}^{\prime }$ ,从而向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{k}$ 的秩等于 $\mathrm{r}\left( {\mathbf{A}}^{\prime }\right) = \mathrm{r}\left( \mathbf{A}\right)$ .

例 3.36 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{k},{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{m}$ 是向量空间 $V$ 中的向量且

$$
\left\{ \begin{matrix} {\mathbf{\beta }}_{1} = {c}_{11}{\mathbf{\alpha }}_{1} + {c}_{12}{\mathbf{\alpha }}_{2} + \cdots + {c}_{1k}{\mathbf{\alpha }}_{k}, \\ {\mathbf{\beta }}_{2} = {c}_{21}{\mathbf{\alpha }}_{1} + {c}_{22}{\mathbf{\alpha }}_{2} + \cdots + {c}_{2k}{\mathbf{\alpha }}_{k}, \\ \cdots \cdots \cdots \cdots \\ {\mathbf{\beta }}_{m} = {c}_{m1}{\mathbf{\alpha }}_{1} + {c}_{m2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{mk}{\mathbf{\alpha }}_{k}. \end{matrix}\right.
$$

记上述表示式中的系数矩阵为 $\mathbf{C} = {\left( {c}_{ij}\right) }_{m \times k}$ ,求证:

(1) 若 $\mathrm{r}\left( \mathbf{C}\right) = k$ ,则这两组向量等价.

(2) 若 $\mathrm{r}\left( \mathbf{C}\right) = r$ ,则向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{m}$ 的秩不超过 $r$ .

证明 (1) 在 $V$ 中取定一组基 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ ,假定在这组基下 ${\mathbf{\alpha }}_{i}$ 的坐标向量是 ${\widetilde{\mathbf{\alpha }}}_{i}\left( {i = 1,\cdots, k}\right) ,{\mathbf{\beta }}_{j}$ 的坐标向量是 ${\widetilde{\mathbf{\beta }}}_{j}\left( {j = 1,\cdots, m}\right)$ ,则

$$
\left\{ \begin{matrix} {\widetilde{\mathbf{\beta }}}_{1} = {c}_{11}{\widetilde{\mathbf{\alpha }}}_{1} + {c}_{12}{\widetilde{\mathbf{\alpha }}}_{2} + \cdots + {c}_{1k}{\widetilde{\mathbf{\alpha }}}_{k}, \\ {\widetilde{\mathbf{\beta }}}_{2} = {c}_{21}{\widetilde{\mathbf{\alpha }}}_{1} + {c}_{22}{\widetilde{\mathbf{\alpha }}}_{2} + \cdots + {c}_{2k}{\widetilde{\mathbf{\alpha }}}_{k}, \\ \cdots \cdots \cdots \cdots \\ {\widetilde{\mathbf{\beta }}}_{m} = {c}_{m1}{\widetilde{\mathbf{\alpha }}}_{1} + {c}_{m2}{\widetilde{\mathbf{\alpha }}}_{2} + \cdots + {c}_{mk}{\widetilde{\mathbf{\alpha }}}_{k}, \end{matrix}\right.
$$

写成矩阵形式为

$$
\left( {{\widetilde{\mathbf{\beta }}}_{1},{\widetilde{\mathbf{\beta }}}_{2},\cdots ,{\widetilde{\widetilde{\mathbf{\beta }}}}_{m}}\right) = \left( {{\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{k}}\right) {\mathbf{C}}^{\prime }.
$$

因为 ${\mathbf{C}}^{\prime }$ 是一个行满秩 $k \times m$ 矩阵,根据后面的例 3.86,存在 $m \times k$ 矩阵 $\mathbf{T}$ , 使 ${\mathbf{C}}^{\prime }\mathbf{T} = {\mathbf{I}}_{k}$ ,于是

$$
\left( {{\widetilde{\mathbf{\beta }}}_{1},{\widetilde{\mathbf{\beta }}}_{2},\cdots ,{\widetilde{\mathbf{\beta }}}_{m}}\right) \mathbf{T} = \left( {{\widetilde{\mathbf{\alpha }}}_{1},{\widetilde{\mathbf{\alpha }}}_{2},\cdots ,{\widetilde{\mathbf{\alpha }}}_{k}}\right) .
$$

这表明 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{k}$ 可以用 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{m}$ 来线性表示. 于是这两组向量等价.

(2) 类似于 (1) 的讨论, 可以用两个矩阵积的秩不超过每个矩阵的秩得到.

例 3.37 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 是数域 $\mathbb{F}$ 上 $n$ 维线性空间 $V$ 中选定的 $m$ 个向量且已知它们的秩等于 $r$ . 求证: 全体适合 ${x}_{1}{\mathbf{\alpha }}_{1} + {x}_{2}{\mathbf{\alpha }}_{2} + \cdots + {x}_{m}{\mathbf{\alpha }}_{m} = \mathbf{0}$ 的列向量 ${\left( {x}_{1},{x}_{2},\cdots ,{x}_{m}\right) }^{\prime }\left( {{x}_{i} \in \mathbb{F}}\right)$ 构成数域 $\mathbb{F}$ 上 $m$ 维列向量空间 ${\mathbb{F}}^{m}$ 的 $m - r$ 维子空间.

证明 在 $V$ 中引进基以后,记 ${\widetilde{\mathbf{\alpha }}}_{i}$ 是 ${\mathbf{\alpha }}_{i}$ 的坐标向量,则 ${x}_{1}{\mathbf{\alpha }}_{1} + {x}_{2}{\mathbf{\alpha }}_{2} + \cdots +$ ${x}_{m}{\mathbf{\alpha }}_{m} = \mathbf{0}$ 等价于 ${x}_{1}{\widetilde{\mathbf{\alpha }}}_{1} + {x}_{2}{\widetilde{\mathbf{\alpha }}}_{2} + \cdots + {x}_{m}{\widetilde{\mathbf{\alpha }}}_{m} = \mathbf{0}$ . 而后者是一个齐次线性方程组, 其系数矩阵的秩等于 $r$ (将 ${x}_{i}$ 视为未知数),因此其解构成 ${\mathbb{F}}^{m}$ 的 $m - r$ 维子空间.

例 3.38 设 $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\}$ 是线性空间 $V$ 的一组基,问: $\left\{ {{e}_{1},{e}_{1} + {e}_{2},\cdots ,{e}_{1} + }\right.$ $\left. {{\mathbf{e}}_{2} + \cdots + {\mathbf{e}}_{n}}\right\}$ 是否也是 $V$ 的基?

答 将 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{1} + {\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{1} + {\mathbf{e}}_{2} + \cdots + {\mathbf{e}}_{n}}\right\}$ 对应的坐标向量拼成如下矩阵:

$$
\mathbf{A} = \left( \begin{matrix} 1 & 1 & \cdots & 1 \\ 0 & 1 & \cdots & 1 \\ \vdots & \vdots & & \vdots \\ 0 & 0 & \cdots & 1 \end{matrix}\right)
$$

显然 $\left| \mathbf{A}\right| = 1$ ,从而 $\mathbf{A}$ 是满秩阵,于是 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{1} + {\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{1} + {\mathbf{e}}_{2} + \cdots + {\mathbf{e}}_{n}}\right\}$ 也是 $V$ 的一组基.

例 3.39 已知向量组 $\left\{ {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}}\right\} \left( {s > 1}\right)$ 是线性空间 $V$ 的一组基, 设 ${\mathbf{\beta }}_{1} = {\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2},{\mathbf{\beta }}_{2} = {\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3},\cdots ,{\mathbf{\beta }}_{s} = {\mathbf{\alpha }}_{s} + {\mathbf{\alpha }}_{1}$ . 讨论向量 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}$ 的线性相关性.

解 将 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}$ 对应的坐标向量拼成如下矩阵:

$$
\mathbf{A} = \left( \begin{matrix} 1 & 0 & \cdots & 1 \\ 1 & 1 & \cdots & 0 \\ 0 & 1 & \cdots & 0 \\ \vdots & \vdots & & \vdots \\ 0 & 0 & \cdots & 1 \end{matrix}\right)
$$

经计算可得 $\left| \mathbf{A}\right| = 1 + {\left( -1\right) }^{s + 1}$ . 因此当 $s$ 为偶数时, $\left| \mathbf{A}\right| = 0$ ,从而向量 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}$ 线性相关; 当 $s$ 为奇数时, $\left| \mathbf{A}\right| = 2$ ,从而向量 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}$ 线性无关.

例 3.40 设 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},{\mathbf{e}}_{3},{\mathbf{e}}_{4}}\right\}$ 是线性空间 $V$ 的一组基,已知

$$
\left\{ \begin{array}{l} {\mathbf{\alpha }}_{1} = {\mathbf{e}}_{1} + {\mathbf{e}}_{2} + {\mathbf{e}}_{3} + 3{\mathbf{e}}_{4}, \\ {\mathbf{\alpha }}_{2} = - {\mathbf{e}}_{1} - 3{\mathbf{e}}_{2} + 5{\mathbf{e}}_{3} + {\mathbf{e}}_{4}, \\ {\mathbf{\alpha }}_{3} = 3{\mathbf{e}}_{1} + 2{\mathbf{e}}_{2} - {\mathbf{e}}_{3} + 4{\mathbf{e}}_{4}, \\ {\mathbf{\alpha }}_{4} = - 2{\mathbf{e}}_{1} - 6{\mathbf{e}}_{2} + {10}{\mathbf{e}}_{3} + 2{\mathbf{e}}_{4}, \end{array}\right.
$$

求 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 的一个极大无关组.

解 将 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 对应的坐标向量拼成如下矩阵,并用初等行变换将其化为阶梯形矩阵:

$$
\mathbf{A} = \left( \begin{matrix} 1 & - 1 & 3 & - 2 \\ 1 & - 3 & 2 & - 6 \\ 1 & 5 & - 1 & {10} \\ 3 & 1 & 4 & 2 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & - 1 & 3 & - 2 \\ 0 & - 2 & - 1 & - 4 \\ 0 & 0 & - 7 & 0 \\ 0 & 0 & 0 & 0 \end{matrix}\right)
$$

因此矩阵 $\mathbf{A}$ 的第一列、第二列和第三列是坐标向量组的极大无关组,从而 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 的一个极大无关组.

例 3.41 设 ${a}_{i}\left( {i = 1,2,\cdots, n}\right)$ 是 $n$ 个不同的数, $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\}$ 是线性空间 $V$ 的一组基,已知

$$
\left\{ \begin{matrix} {\mathbf{\alpha }}_{1} = {\mathbf{e}}_{1} + {a}_{1}{\mathbf{e}}_{2} + \cdots + {a}_{1}^{n - 1}{\mathbf{e}}_{n}, \\ {\mathbf{\alpha }}_{2} = {\mathbf{e}}_{1} + {a}_{2}{\mathbf{e}}_{2} + \cdots + {a}_{2}^{n - 1}{\mathbf{e}}_{n}, \\ \cdots \cdots \cdots \cdots \\ {\mathbf{\alpha }}_{n} = {\mathbf{e}}_{1} + {a}_{n}{\mathbf{e}}_{2} + \cdots + {a}_{n}^{n - 1}{\mathbf{e}}_{n}, \end{matrix}\right.
$$

求证: $\left\{ {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right\}$ 也是 $V$ 的一组基.

证明 将 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 对应的坐标向量拼成如下矩阵:

$$
\mathbf{A} = \left( \begin{matrix} 1 & 1 & \cdots & 1 \\ {a}_{1} & {a}_{2} & \cdots & {a}_{n} \\ \vdots & \vdots & & \vdots \\ {a}_{1}^{n - 1} & {a}_{2}^{n - 1} & \cdots & {a}_{n}^{n - 1} \end{matrix}\right)
$$

显然 $\left| \mathbf{A}\right| = \mathop{\prod }\limits_{{1 \leq i < j \leq n}}\left( {{a}_{j} - {a}_{i}}\right) \neq 0$ ,故 $\mathbf{A}$ 是满秩阵,从而 $\left\{ {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right\}$ 也是 $V$ 的一组基.

## 3.2.4 基变换与过渡矩阵

例 3.42 设 $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\} ,\left\{ {{u}_{1},{u}_{2},\cdots ,{u}_{n}}\right\} ,\left\{ {{v}_{1},{v}_{2},\cdots ,{v}_{n}}\right\}$ 是向量空间 $V$ 的 3 组基. 若从 ${\mathbf{u}}_{1},{\mathbf{u}}_{2},\cdots ,{\mathbf{u}}_{n}$ 到 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 的过渡矩阵是 $\mathbf{A}$ ,从 ${\mathbf{u}}_{1},{\mathbf{u}}_{2},\cdots ,{\mathbf{u}}_{n}$ 到 ${v}_{1},{v}_{2},\cdots ,{v}_{n}$ 的过渡矩阵是 $\mathbf{B}$ ,求从 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 到 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{n}$ 的过渡矩阵.

解 从 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 到 ${\mathbf{u}}_{1},{\mathbf{u}}_{2},\cdots ,{\mathbf{u}}_{n}$ 的过渡矩阵为 ${\mathbf{A}}^{-1}$ ,故从 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 到 ${\mathbf{v}}_{1},{\mathbf{v}}_{2},\cdots ,{\mathbf{v}}_{n}$ 的过渡矩阵为 ${\mathbf{A}}^{-1}\mathbf{B}$ .

例 3.43 在四维行向量空间中求从基 ${e}_{1},{e}_{2},\cdots ,{e}_{n}$ 到 ${f}_{1},{f}_{2},\cdots ,{f}_{n}$ 的过渡矩阵, 其中

$$
{\mathbf{e}}_{1} = \left( {1,1,0,1}\right) ,{\mathbf{e}}_{2} = \left( {2,1,3,0}\right) ,{\mathbf{e}}_{3} = \left( {1,1,0,0}\right) ,{\mathbf{e}}_{4} = \left( {0,1, - 1, - 1}\right) ,
$$

$$
{\mathbf{f}}_{1} = \left( {1,0,0,1}\right) ,{\mathbf{f}}_{2} = \left( {0,0,1, - 1}\right) ,{\mathbf{f}}_{3} = \left( {2,1,0,3}\right) ,{\mathbf{f}}_{4} = \left( {-1,0,1,2}\right) .
$$

解 这类题如用解线性方程组的方法比较繁, 可采用下列方法.

设该向量空间的标准基为

$$
{\mathbf{u}}_{1} = \left( {1,0,0,0}\right) ,{\mathbf{u}}_{2} = \left( {0,1,0,0}\right) ,{\mathbf{u}}_{3} = \left( {0,0,1,0}\right) ,{\mathbf{u}}_{4} = \left( {0,0,0,1}\right) ,
$$

则从 ${\mathbf{u}}_{1},{\mathbf{u}}_{2},{\mathbf{u}}_{3},{\mathbf{u}}_{4}$ 到 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},{\mathbf{e}}_{3},{\mathbf{e}}_{4}$ 的过渡矩阵为

$$
\mathbf{A} = \left( \begin{matrix} 1 & 2 & 1 & 0 \\ 1 & 1 & 1 & 1 \\ 0 & 3 & 0 & - 1 \\ 1 & 0 & 0 & - 1 \end{matrix}\right)
$$

从 ${\mathbf{u}}_{1},{\mathbf{u}}_{2},{\mathbf{u}}_{3},{\mathbf{u}}_{4}$ 到 ${\mathbf{f}}_{1},{\mathbf{f}}_{2},{\mathbf{f}}_{3},{\mathbf{f}}_{4}$ 的过渡矩阵为

$$
\mathbf{B} = \left( \begin{matrix} 1 & 0 & 2 & - 1 \\ 0 & 0 & 1 & 0 \\ 0 & 1 & 0 & 1 \\ 1 & - 1 & 3 & 2 \end{matrix}\right)
$$

根据上例,从基 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},{\mathbf{e}}_{3},{\mathbf{e}}_{4}$ 到 ${\mathbf{f}}_{1},{\mathbf{f}}_{2},{\mathbf{f}}_{3},{\mathbf{f}}_{4}$ 的过渡矩阵为 ${\mathbf{A}}^{-1}\mathbf{B}$ . 它可以用初等变换和求逆矩阵类似的方法直接求得 (对矩阵 $\left( {\mathbf{A};\mathbf{B}}\right)$ 进行初等行变换,将 $\mathbf{A}$ 化为单位矩阵,则右边一块就化为了 ${\mathbf{A}}^{-1}\mathbf{B}$ ):

$$
\left( {\mathbf{A};\mathbf{B}}\right) = \left( \begin{matrix} 1 & 2 & 1 & 0 & 1 & 0 & 2 & - 1 \\ 1 & 1 & 1 & 1 & 0 & 0 & 1 & 0 \\ 0 & 3 & 0 & - 1 & 0 & 1 & 0 & 1 \\ 1 & 0 & 0 & - 1 & 1 & - 1 & 3 & 2 \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 2 & 1 & 0 & 1 & 1 & 0 & 2 & - 1 \\ 0 & - 1 & 0 & 1 & 1 & - 1 & 0 & - 1 & 1 \\ 0 & 3 & 0 & - 1 & 0 & 1 & 0 & 1 & \\ 0 & - 2 & - 1 & - 1 & 0 & - 1 & 1 & 3 & \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 2 & 1 & 0 & 1 & 1 & 0 & 2 & - 1 \\ 0 & - 1 & 0 & 1 & 1 & - 1 & 0 & - 1 & 1 \\ 0 & 0 & - 1 & - 3 & 1 & 2 & - 1 & 3 & 1 \\ 0 & 0 & 0 & 2 & 1 & - 3 & 1 & - 3 & 4 \end{matrix}\right)
$$

$$
\left( \begin{matrix} 1 & 2 & 1 & 0 & 1 & 1 & 0 & 2 & - 1 \\ 0 & 1 & 0 & - 1 & 1 & 0 & 1 & - 1 & \\ 0 & 0 & 1 & 3 & - 2 & 1 & - 3 & - 1 & \\ 0 & 0 & 0 & 2 & - 3 & 1 & - 3 & 4 & \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 2 & 1 & 0 & 1 & 1 & 0 & 2 & - 1 \\ 0 & 1 & 0 & 0 & 1 & - \frac{1}{2} & \frac{1}{2} & - \frac{1}{2} & 1 \\ 0 & 0 & 1 & 0 & 1 & \frac{5}{2} & - \frac{1}{2} & \frac{3}{2} & - 7 \\ 0 & 0 & 0 & 2 & 1 & 2 & 1 & - 3 & 4 \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 2 & 0 & 0 & \frac{1}{1} & \frac{3}{2} & \frac{1}{2} & \frac{1}{2} & 6 \\ 0 & 1 & 0 & 0 & - \frac{1}{2} & \frac{1}{2} & - \frac{1}{2} & 1 & \\ 0 & 0 & 1 & 0 & \frac{1}{2} & - \frac{1}{2} & \frac{3}{2} & - 7 & \\ 0 & 0 & 0 & 1 & - \frac{3}{2} & - \frac{1}{2} & - \frac{3}{2} & - 7 & \\ 0 & 0 & 0 & 1 & - \frac{3}{2} & \frac{1}{2} & - \frac{3}{2} & 2 & \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 0 & 0 & 0 & \frac{1}{1} - \frac{1}{2} & - \frac{1}{2} & \frac{3}{2} & 4 & \\ 0 & 1 & 0 & 0 & \frac{1}{1} - \frac{1}{2} & \frac{1}{2} & - \frac{1}{2} & 1 & \\ 0 & 0 & 1 & 0 & \frac{1}{1} & \frac{5}{2} & - \frac{1}{2} & \frac{3}{2} & - 7 \\ 0 & 0 & 0 & 1 & \frac{1}{1} & - \frac{3}{2} & \frac{1}{2} & - 7 & \\ 0 & 0 & 0 & 1 & - \frac{3}{2} & \frac{1}{2} & - \frac{3}{2} & 2 & \end{matrix}\right) .
$$

因此, 所求之过渡矩阵为

$$
\left( \begin{matrix} - \frac{1}{2} & - \frac{1}{2} & \frac{3}{2} & 4 \\ - \frac{1}{2} & \frac{1}{2} & - \frac{1}{2} & 1 \\ \frac{5}{2} & - \frac{1}{2} & \frac{3}{2} & - 7 \\ - \frac{3}{2} & \frac{1}{2} & - \frac{3}{2} & 2 \end{matrix}\right) .\square
$$

例 3.44 设 $a$ 为常数,求向量 $\mathbf{\alpha } = \left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right)$ 在基

$$
\left\{ {{\mathbf{f}}_{1} = \left( {{a}^{n - 1},{a}^{n - 2},\cdots, a,1}\right) ,{\mathbf{f}}_{2} = \left( {{a}^{n - 2},{a}^{n - 3},\cdots ,1,0}\right) ,\cdots ,{\mathbf{f}}_{n} = \left( {1,0,\cdots ,0,0}\right) }\right\}
$$

下的坐标.

解 设 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ 是标准单位行向量,则从 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 到 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots }\right.$ , $\left. {f}_{n}\right\}$ 的过渡矩阵是

$$
\mathbf{A} = \left( \begin{matrix} {a}^{n - 1} & {a}^{n - 2} & \cdots & 1 \\ {a}^{n - 2} & {a}^{n - 3} & \cdots & 0 \\ \vdots & \vdots & & \vdots \\ a & 1 & \cdots & 0 \\ 1 & 0 & \cdots & 0 \end{matrix}\right) .
$$

设 $\mathbf{\alpha }$ 在 $\left\{ {{\mathbf{f}}_{1},{\mathbf{f}}_{2},\cdots ,{\mathbf{f}}_{n}}\right\}$ 下的坐标向量为 $\mathbf{x} = \left( {{x}_{1},{x}_{2},\cdots ,{x}_{n}}\right)$ ,则有 $\mathbf{A}{\mathbf{x}}^{\prime } = {\mathbf{\alpha }}^{\prime }$ . 这是一个非齐次线性方程组, 可由初等行变换求出方程组的解:

$$
\left( \begin{matrix} {a}^{n - 1} & {a}^{n - 2} & \cdots & 1 & {a}_{1} \\ {a}^{n - 2} & {a}^{n - 3} & \cdots & 0 & {a}_{1} \\ \vdots & \vdots & & \vdots & \vdots \\ a & 1 & \cdots & 0 & {a}_{n} \\ 1 & 0 & \cdots & 0 & {a}_{n} \end{matrix}\right) \rightarrow \left( \begin{matrix} 0 & {a}^{n - 2} & \cdots & 1 & {a}_{1} - {a}^{n - 1}{a}_{n} \\ 0 & {a}^{n - 3} & \cdots & 0 & {a}_{2} - {a}^{n - 2}{a}_{n} \\ \vdots & \vdots & & \vdots & \vdots \\ 0 & 1 & \cdots & 0 & {a}_{n - 1} - a{a}_{n} \\ 1 & 0 & \cdots & 0 & {a}_{n} \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 0 & 0 & \cdots & 1 & {a}_{1} - a{a}_{2} \\ 0 & 0 & \cdots & 0 & {a}_{2} - a{a}_{3} \\ \vdots & \vdots & & \vdots & \vdots \\ 0 & 1 & \cdots & 0 & {a}_{n - 1} - a{a}_{n} \\ 1 & 0 & \cdots & 0 & {a}_{n} \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & \cdots & 0 & {a}_{n} \\ 0 & 1 & \cdots & 0 & {a}_{n - 1} - a{a}_{n} \\ \vdots & \vdots & & \vdots & \vdots \\ 0 & 0 & \cdots & 0 & {a}_{2} - a{a}_{3} \\ 0 & 0 & \cdots & 1 & {a}_{1} - a{a}_{2} \end{matrix}\right) ,
$$

因此 $\mathbf{x} = \left( {{a}_{n},{a}_{n - 1} - a{a}_{n},\cdots ,{a}_{2} - a{a}_{3},{a}_{1} - a{a}_{2}}\right)$ .

例 3.45 设 $V$ 是次数不超过 $n$ 的实系数多项式全体组成的线性空间,求从基 $\left\{ {1, x,{x}^{2},\cdots ,{x}^{n}}\right\}$ 到基 $\left\{ {1, x - a,{\left( x - a\right) }^{2},\cdots ,{\left( x - a\right) }^{n}}\right\}$ 的过渡矩阵并以此证明多项式的 Taylor 公式:

$$
f\left( x\right) = f\left( a\right) + \frac{{f}^{\prime }\left( a\right) }{1!}\left( {x - a}\right) + \frac{{f}^{\prime \prime }\left( a\right) }{2!}{\left( x - a\right) }^{2} + \cdots + \frac{{f}^{\left( n\right) }\left( a\right) }{n!}{\left( x - a\right) }^{n},
$$

其中 ${f}^{\left( n\right) }\left( x\right)$ 表示 $f\left( x\right)$ 的 $n$ 次导数.

解 过渡矩阵 $\left( {n + 1\text{阶}}\right)$ 容易求出为

$$
\mathbf{P} = \left( \begin{matrix} 1 & - a & {a}^{2} & \cdots & {\left( -1\right) }^{n}{a}^{n} \\ 0 & 1 & - {2a} & \cdots & {\left( -1\right) }^{n - 1}n{a}^{n - 1} \\ 0 & 0 & 1 & \cdots & {\left( -1\right) }^{n - 2}\frac{n\left( {n - 1}\right) }{2!}{a}^{n - 2} \\ \vdots & \vdots & \vdots & & \vdots \\ 0 & 0 & 0 & \cdots & 1 \end{matrix}\right) .
$$

注意 $\mathbf{P}$ 的逆矩阵 ${\mathbf{P}}^{-1}$ 可通过变换 $x \rightarrow \left( {x + a}\right)$ 马上得到 (不必用初等变换法求逆矩阵):

$$
{\mathbf{P}}^{-1} = \left( \begin{matrix} 1 & a & {a}^{2} & \cdots & {a}^{n} \\ 0 & 1 & {2a} & \cdots & n{a}^{n - 1} \\ 0 & 0 & 1 & \cdots & \frac{n\left( {n - 1}\right) }{2!}{a}^{n - 2} \\ \vdots & \vdots & \vdots & & \vdots \\ 0 & 0 & 0 & \cdots & 1 \end{matrix}\right)
$$

设 $f\left( x\right) = {a}_{0} + {a}_{1}x + {a}_{2}{x}^{2} + \cdots + {a}_{n}{x}^{n}$ ,则 $f\left( x\right)$ 在基 $\left\{ {1, x - a,{\left( x - a\right) }^{2},\cdots ,{\left( x - a\right) }^{n}}\right\}$ 下的坐标向量为

$$
{\mathbf{P}}^{-1}\left( \begin{matrix} {a}_{0} \\ {a}_{1} \\ {a}_{2} \\ \vdots \\ {a}_{n} \end{matrix}\right) = \left( \begin{matrix} 1 & a & {a}^{2} & \cdots & {a}^{n} \\ 0 & 1 & {2a} & \cdots & n{a}^{n - 1} \\ 0 & 0 & 1 & \cdots & \frac{n\left( {n - 1}\right) }{2!}{a}^{n - 2} \\ \vdots & \vdots & \vdots & & \vdots \\ 0 & 0 & 0 & \cdots & 1 \end{matrix}\right) \left( \begin{matrix} {a}_{0} \\ {a}_{1} \\ {a}_{2} \\ \vdots \\ {a}_{n} \end{matrix}\right) = \left( \begin{matrix} f\left( a\right) \\ \frac{{f}^{\prime }\left( a\right) }{1!} \\ \vdots \\ \frac{{f}^{\left( n\right) }\left( a\right) }{n!} \end{matrix}\right) ,
$$

由此即得结论.

## 3.2.5 子 空 间

例 3.46 设 $V = {M}_{n}\left( \mathbb{K}\right)$ 是数域 $\mathbb{K}$ 上的 $n$ 阶矩阵全体组成的线性空间, $\mathbf{A} \in V$ , 求证: 与 $\mathbf{A}$ 乘法可交换的矩阵全体 $C\left( \mathbf{A}\right)$ 组成 $V$ 的子空间. 又若 $T$ 是 $V$ 的非空子集,求证: 与 $T$ 中任一矩阵乘法可交换的矩阵全体 $C\left( T\right)$ 也构成 $V$ 的子空间且其维数不为零.

证明 任取 $\mathbf{B},\mathbf{C} \in C\left( \mathbf{A}\right), k \in \mathbb{K}$ ,容易验证 $\mathbf{B} + \mathbf{C} \in C\left( \mathbf{A}\right), k\mathbf{B} \in C\left( \mathbf{A}\right)$ , 故 $C\left( \mathbf{A}\right)$ 是 ${M}_{n}\left( \mathbb{K}\right)$ 的子空间. 因为 ${\mathbf{I}}_{n} \in C\left( \mathbf{A}\right)$ ,所以 $C\left( \mathbf{A}\right)$ 的维数不为零. $C\left( T\right)$ 的结论同理可证.

下面的例 3.47 给出了求子空间和及交的矩阵方法. 对一般的抽象线性空间, 可将它等同于行 (列) 向量空间, 然后用矩阵方法来解, 这样做往往比较简便.

例 3.47 设 ${\mathbf{\alpha }}_{1} = \left( {1,0, - 1,0}\right) ,{\mathbf{\alpha }}_{2} = \left( {0,1,2,1}\right) ,{\mathbf{\alpha }}_{3} = \left( {2,1,0,1}\right)$ 是四维实行向量空间 $V$ 中的向量,它们生成的子空间为 ${V}_{1}$ ,又向量 ${\mathbf{\beta }}_{1} = \left( {-1,1,1,1}\right) ,{\mathbf{\beta }}_{2} =$ $\left( {1, - 1, - 3, - 1}\right) ,{\mathbf{\beta }}_{3} = \left( {-1,1, - 1,1}\right)$ 生成的子空间为 ${V}_{2}$ ,求子空间 ${V}_{1} + {V}_{2}$ 和 ${V}_{1} \cap {V}_{2}$ 的基.

解法 $1{V}_{1} + {V}_{2}$ 是由 ${\mathbf{\alpha }}_{i}$ 和 ${\mathbf{\beta }}_{i}$ 生成的,因此只要求出这 6 个向量的极大无关组即可. 将这 6 个向量按列分块方式拼成矩阵, 并用初等行变换将其化为阶梯形矩阵:

$$
\left( \begin{matrix} 1 & 0 & 2 & - 1 & 1 & - 1 \\ 0 & 1 & 1 & 1 & - 1 & 1 \\ - 1 & 2 & 0 & 1 & - 3 & - 1 \\ 0 & 1 & 1 & 1 & - 1 & 1 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & 2 & - 1 & 1 & - 1 \\ 0 & 1 & 1 & 1 & - 1 & 1 \\ 0 & 2 & 2 & 0 & - 2 & - 2 \\ 0 & 0 & 0 & 0 & 0 & 0 \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 0 & 2 & - 1 & 1 & - 1 \\ 0 & 1 & 1 & 1 & - 1 & 1 \\ 0 & 0 & 0 & - 2 & 0 & - 4 \\ 0 & 0 & 0 & 0 & 0 & 0 \end{matrix}\right)
$$

故可取 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\beta }}_{1}$ 为 ${V}_{1} + {V}_{2}$ 的基 (不唯一).

再来求 ${V}_{1} \cap {V}_{2}$ 的基. 首先注意到 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2}$ 是 ${V}_{1}$ 的基 (从上面的矩阵即可看出),又不难验证 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2}$ 是 ${V}_{2}$ 的基, ${V}_{2}$ 中的向量可以表示为 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2}$ 的线性组合. 假定 ${t}_{1}{\mathbf{\beta }}_{1} + {t}_{2}{\mathbf{\beta }}_{2}$ 属于 ${V}_{1}$ ,则向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{t}_{1}{\mathbf{\beta }}_{1} + {t}_{2}{\mathbf{\beta }}_{2}$ 和向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2}$ 的秩相等 (因为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2}$ 是 ${V}_{1}$ 的基). 所以我们也可以用矩阵方法来求出参数 ${t}_{1},{t}_{2}$ .

$$
\left( \begin{matrix} 1 & 0 & - {t}_{1} + {t}_{2} \\ 0 & 1 & {t}_{1} - {t}_{2} \\ - 1 & 2 & {t}_{1} - 3{t}_{2} \\ 0 & 1 & {t}_{1} - {t}_{2} \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & - {t}_{1} + {t}_{2} \\ 0 & 1 & {t}_{1} - {t}_{2} \\ 0 & 2 & - 2{t}_{2} \\ 0 & 0 & 0 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & - {t}_{1} + {t}_{2} \\ 0 & 1 & {t}_{1} - {t}_{2} \\ 0 & 0 & - 2{t}_{1} \\ 0 & 0 & 0 \end{matrix}\right) ,
$$

得到 ${t}_{1} = 0$ ,所以 ${V}_{1} \cap {V}_{2}$ 的基可取为 ${\mathbf{\beta }}_{2}$ .

解法 2 求 ${V}_{1} + {V}_{2}$ 的基同解法 1,现用解线性方程组的方法来求 ${V}_{1} \cap {V}_{2}$ 的基. 因为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2}$ 是 ${V}_{1}$ 的基, ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2}$ 是 ${V}_{2}$ 的基,故对任一向量 $\gamma \in {V}_{1} \cap {V}_{2}$ , $\gamma = {x}_{1}{\alpha }_{1} + {x}_{2}{\alpha }_{2} = \left( {-{x}_{3}}\right) {\beta }_{1} + \left( {-{x}_{4}}\right) {\beta }_{2}$ . 因此,求向量 $\gamma$ 等价于求解线性方程组

$$
{x}_{1}{\mathbf{\alpha }}_{1} + {x}_{2}{\mathbf{\alpha }}_{2} + {x}_{3}{\mathbf{\beta }}_{1} + {x}_{4}{\mathbf{\beta }}_{2} = \mathbf{0}.
$$

通过初等行变换将其系数矩阵 $\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2}}\right)$ 进行化简:

$$
\left( \begin{matrix} 1 & 0 & - 1 & 1 \\ 0 & 1 & 1 & - 1 \\ 0 & 0 & - 2 & 0 \\ 0 & 0 & 0 & 0 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & 0 & 1 \\ 0 & 1 & 0 & - 1 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 \end{matrix}\right)
$$

故上述线性方程组的通解为 $\left( {{x}_{1},{x}_{2},{x}_{3},{x}_{4}}\right) = k\left( {-1,1,0,1}\right)$ ,从而 $\gamma = - k\left( {{\alpha }_{1} - {\alpha }_{2}}\right) =$ $- k{\mathbf{\beta }}_{2}\left( {k \in \mathbb{R}}\right)$ ,于是 ${\mathbf{\beta }}_{2}$ 是 ${V}_{1} \cap {V}_{2}$ 的基.

要证明向量空间 $V$ 是其子空间 ${V}_{1},{V}_{2}$ 的直和,只需证明两件事: 一是证明 $V$ 中任一向量均可表示为 ${V}_{1}$ 与 ${V}_{2}$ 中向量之和,即 $V = {V}_{1} + {V}_{2}$ ; 二是证明 ${V}_{1}$ 与 ${V}_{2}$ 的交等于零. 下面是两个典型的例子.

例 3.48 设 $V$ 是数域 $\mathbb{F}$ 上 $n$ 阶矩阵组成的向量空间, ${V}_{1}$ 和 ${V}_{2}$ 分别是 $\mathbb{F}$ 上对称矩阵和反对称矩阵组成的子集. 求证: ${V}_{1}$ 和 ${V}_{2}$ 都是 $V$ 的子空间且 $V = {V}_{1} \oplus {V}_{2}$ .

证明 由于对称矩阵之和仍是对称矩阵, 一个数乘以对称矩阵仍是对称矩阵, 因此 ${V}_{1}$ 是 $V$ 的子空间. 同理 ${V}_{2}$ 也是 $V$ 的子空间. 又由例 2.8 可知,任一 $n$ 阶矩阵都可以表示成为一个对称矩阵和一个反对称矩阵之和,故 $V = {V}_{1} + {V}_{2}$ . 若一个矩阵既是对称矩阵又是反对称矩阵,则它一定是零矩阵. 这就是说 ${V}_{1} \cap {V}_{2} = 0$ . 于是 $V = {V}_{1} \oplus {V}_{2}$ .

例 3.49 设 ${V}_{1},{V}_{2}$ 分别是数域 $\mathbb{F}$ 上的齐次线性方程组 ${x}_{1} = {x}_{2} = \cdots = {x}_{n}$ 与 ${x}_{1} + {x}_{2} + \cdots + {x}_{n} = 0$ 的解空间,求证: ${\mathbb{F}}^{n} = {V}_{1} \oplus {V}_{2}$ .

证明 由线性方程组解的定理知, ${V}_{1}$ 的维数是 $1,{V}_{2}$ 的维数是 $n - 1$ . 若列向量 $\mathbf{\alpha } \in {V}_{1} \cap {V}_{2}$ ,则 $\mathbf{\alpha }$ 既是第一个线性方程组的解,也是第二个线性方程组的解,不难看出 $\mathbf{\alpha }$ 只能等于零向量,因此 ${V}_{1} \cap {V}_{2} = 0$ . 又因为

$$
\dim \left( {{V}_{1} \oplus {V}_{2}}\right) = \dim {V}_{1} + \dim {V}_{2} = 1 + \left( {n - 1}\right) = n = \dim {\mathbb{F}}^{n},
$$

故 ${\mathbb{F}}^{n} = {V}_{1} \oplus {V}_{2}$ .

例 3.50 设 $U, V$ 是数域 $\mathbb{K}$ 上的两个线性空间, $W = U \times V$ 是 $U$ 和 $V$ 的积集合,即 $W = \{ \left( {\mathbf{u},\mathbf{v}}\right) \mid \mathbf{u} \in U,\mathbf{v} \in V\}$ . 现在 $W$ 上定义加法和数乘:

$$
\left( {{\mathbf{u}}_{1},{\mathbf{v}}_{1}}\right) + \left( {{\mathbf{u}}_{2},{\mathbf{v}}_{2}}\right) = \left( {{\mathbf{u}}_{1} + {\mathbf{u}}_{2},{\mathbf{v}}_{1} + {\mathbf{v}}_{2}}\right), k\left( {\mathbf{u},\mathbf{v}}\right) = \left( {k\mathbf{u}, k\mathbf{v}}\right) .
$$

验证: $W$ 是 $\mathbb{K}$ 上的线性空间 (这个线性空间称为 $U$ 和 $V$ 的外直和).

又若设 ${U}^{\prime } = \{ \left( {\mathbf{u},\mathbf{0}}\right) \mid \mathbf{u} \in U\} ,{V}^{\prime } = \{ \left( {\mathbf{0},\mathbf{v}}\right) \mid \mathbf{v} \in V\}$ ,则 ${U}^{\prime },{V}^{\prime }$ 是 $W$ 的子空间且 ${U}^{\prime }$ 和 $U$ 同构, ${V}^{\prime }$ 和 $V$ 同构且 $W = {U}^{\prime } \oplus {V}^{\prime }$ .

证明 容易验证 $W$ 在上述加法和数乘下满足线性空间的 8 条性质,从而是 $\mathbb{K}$ 上的线性空间. 任取 $\left( {{\mathbf{u}}_{1},\mathbf{0}}\right) ,\left( {{\mathbf{u}}_{2},\mathbf{0}}\right) \in {U}^{\prime }, k \in \mathbb{K}$ ,则 $\left( {{\mathbf{u}}_{1},\mathbf{0}}\right) + \left( {{\mathbf{u}}_{2},\mathbf{0}}\right) = \left( {{\mathbf{u}}_{1} + {\mathbf{u}}_{2},\mathbf{0}}\right) \in$ ${U}^{\prime }, k\left( {{\mathbf{u}}_{1},\mathbf{0}}\right) = \left( {k{\mathbf{u}}_{1},\mathbf{0}}\right) \in {U}^{\prime }$ ,因此 ${U}^{\prime }$ 是 $W$ 的子空间. 同理可证 ${V}^{\prime }$ 是 $W$ 的子空间. 构造映射 $\varphi : U \rightarrow {U}^{\prime },\varphi \left( \mathbf{u}\right) = \left( {\mathbf{u},\mathbf{0}}\right)$ ,容易验证 $\varphi$ 是一一对应并且保持加法和数乘运算,所以 $\varphi : U \rightarrow {U}^{\prime }$ 是一个线性同构. 构造映射 $\psi : V \rightarrow {V}^{\prime },\psi \left( v\right) = \left( {\mathbf{0},\mathbf{v}}\right)$ ,同理可证 $\mathbf{\psi } : V \rightarrow {V}^{\prime }$ 是一个线性同构. 显然 ${U}^{\prime } \cap {V}^{\prime } = 0$ ,又对 $W$ 中任一向量 $\left( {\mathbf{u},\mathbf{v}}\right)$ , 有 $\left( {\mathbf{u},\mathbf{v}}\right) = \left( {\mathbf{u},\mathbf{0}}\right) + \left( {\mathbf{0},\mathbf{v}}\right) \in {U}^{\prime } + {V}^{\prime }$ ,因此 $W = {U}^{\prime } \oplus {V}^{\prime }$ . [

例 3.51 设 $U$ 是 $V$ 的子空间,求证: 存在 $V$ 的子空间 $W$ ,使得 $V = U \oplus W$ . 这样的子空间 $W$ 称为子空间 $U$ 在 $V$ 中的补空间.

证明 取子空间 $U$ 的一组基 $\left\{ {{\mathbf{e}}_{1},\cdots ,{\mathbf{e}}_{m}}\right\}$ ,由基扩张定理可将其扩张为 $V$ 的一组基 $\left\{ {{\mathbf{e}}_{1},\cdots ,{\mathbf{e}}_{m},{\mathbf{e}}_{m + 1},\cdots ,{\mathbf{e}}_{n}}\right\}$ . 令 $W = L\left( {{\mathbf{e}}_{m + 1},\cdots ,{\mathbf{e}}_{n}}\right)$ ,则 $V = U + W$ . 事实上, $\left\{ {{e}_{m + 1},\cdots ,{e}_{n}}\right\}$ 是 $W$ 的一组基,故 $\dim V = \dim U + \dim W$ ,从而 $V = U \oplus W$ .

和两个子空间的情形不同,要判定子空间 ${V}_{1},{V}_{2},\cdots ,{V}_{m}\left( {m \geq 3}\right)$ 的和是否为直和,只验证 ${V}_{i} \cap {V}_{j} = 0\left( {1 \leq i < j \leq m}\right)$ 是远远不够的. 例如 ${\mathbb{R}}_{2}$ 的 3 个子空间: ${V}_{1} = \{ \left( {a,0}\right) \mid a \in \mathbb{R}\} ,{V}_{2} = \{ \left( {0, b}\right) \mid b \in \mathbb{R}\} ,{V}_{3} = \{ \left( {a, a}\right) \mid a \in \mathbb{R}\}$ ,它们满足 ${V}_{i} \cap {V}_{j} = 0\left( {1 \leq i < j \leq 3}\right)$ ,但 ${V}_{1} + {V}_{2} + {V}_{3}$ 不是直和. 因此在子空间个数多于两个的情形下,我们通常需要利用 $§{3.1.5}$ 的定理 5 来进行直和判定.

例 3.52 若 $V = U \oplus W$ 且 $U = {U}_{1} \oplus {U}_{2}$ ,求证: $V = {U}_{1} \oplus {U}_{2} \oplus W$ .

证明 由 $U = {U}_{1} \oplus {U}_{2}$ 可得 ${U}_{1} \cap {U}_{2} = 0$ ; 由 $V = U \oplus W$ 可得 $\left( {{U}_{1} + {U}_{2}}\right) \cap$ $W = U \cap W = 0$ ,因此由 $§{3.1.5}$ 的定理 5 (2) 可得 ${U}_{1} + {U}_{2} + W$ 是直和,从而 $V = {U}_{1} + {U}_{2} + W = {U}_{1} \oplus {U}_{2} \oplus W$ .

例 3.53 求证: 每一个 $n$ 维线性空间均可表示为 $n$ 个一维子空间的直和.

证明 设 $V$ 是 $n$ 维线性空间,取其一组基为 $\left\{ {{e}_{1},{e}_{2},\cdots ,{e}_{n}}\right\}$ . 设 ${V}_{i} =$ $L\left( {\mathbf{e}}_{i}\right) \left( {1 \leq i \leq n}\right)$ ,则 ${V}_{i}$ 是 $V$ 的一维子空间且 $V = {V}_{1} + {V}_{2} + \cdots + {V}_{n}$ . 注意到 $\dim V = n = \dim {V}_{1} + \dim {V}_{2} + \cdots + \dim {V}_{n}$ ,故由 $§{3.1.5}$ 的定理 5 (3) 可知, $V = {V}_{1} \oplus {V}_{2} \oplus \cdots \oplus {V}_{n}$ . 注意到 ${V}_{i}$ 的基是 $\left\{ {\mathbf{e}}_{i}\right\}$ ,因此 ${V}_{i}\left( {1 \leq i \leq n}\right)$ 的基能拼成 $V$ 的基,故由 $§{3.1.5}$ 的定理 5 (4) 也可得到结论. 再注意到 $V$ 中任一向量写成基向量 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ 的线性组合时,其表示是唯一的. 这就是说, $V$ 中任一向量写成 ${V}_{i}$ 中的向量之和时,其表示是唯一的,故由 $§{3.1.5}$ 的定理 5 (5) 同样可得结论.

* 例 3.54 设 ${V}_{1},{V}_{2},\cdots ,{V}_{m}$ 是数域 $\mathbb{F}$ 上向量空间 $V$ 的 $m$ 个真子空间,证明: 在 $V$ 中必存在一个向量 $\mathbf{\alpha }$ ,它不属于任何一个 ${V}_{i}$ .

证明 对 $m$ 用归纳法. 当 $m = 1$ 时结论显然成立. 设 $m = k$ 时结论成立, 现要证明 $m = k + 1$ 时结论也成立. 由归纳假设,存在向量 $\mathbf{\alpha }$ ,它不属于任何一个 ${V}_{i}\left( {i = 1,\cdots, k}\right)$ . 若 $\mathbf{\alpha }$ 也不属于 ${V}_{k + 1}$ ,则结论已成立,因此可设 $\mathbf{\alpha } \in {V}_{k + 1}$ . 在 ${V}_{k + 1}$ 外选一个向量 $\mathbf{\beta }$ . 作集合 $M = \{ t\mathbf{\alpha } + \mathbf{\beta } \mid t \in \mathbb{F}\}$ . 事实上,我们可将 $M$ 看成是通过 $\mathbf{\beta }$ 的终点且平行于 $\mathbf{\alpha }$ 的一根 “直线”,现要证明它和每个 ${V}_{i}$ 最多只有一个交点. 首先, $M$ 和 ${V}_{k + 1}$ 无交点,因为若 $t\mathbf{\alpha } + \mathbf{\beta } \in {V}_{k + 1}$ ,则从 $t\mathbf{\alpha } \in {V}_{k + 1}$ 可推出 $\mathbf{\beta } \in {V}_{k + 1}$ , 与假设矛盾. 又若 ${t}_{1}\mathbf{\alpha } + \mathbf{\beta } \in {V}_{i},{t}_{2}\mathbf{\alpha } + \mathbf{\beta } \in {V}_{i}\left( {i < k + 1}\right)$ ,则 $\left( {{t}_{1} - {t}_{2}}\right) \mathbf{\alpha } \in {V}_{i}$ . 若 ${t}_{1} \neq {t}_{2}$ ,将导致 $\mathbf{\alpha } \in {V}_{i}$ ,与假设矛盾. 由此可以看到, $M$ 中只有有限个向量属于 ${V}_{i}$ 的并集,而 $t$ 有无穷多个选择,由此即得结论.

注 本结论证明中要用到任意一个数域都有无穷个元素这一事实, 因此, 对有限域 (读者以后可能会学到) 上的向量空间, 结论不一定成立.

* 例 3.55 设 ${V}_{1},{V}_{2},\cdots ,{V}_{m}$ 是数域 $\mathbb{F}$ 上向量空间 $V$ 的 $m$ 个真子空间,证明: $V$ 中必有一组基,使得其中每个基向量都不在诸 ${V}_{i}$ 的并中.

证明 由例 3.54 可知,存在非零向量 ${\mathbf{e}}_{1} \in V$ ,使得 ${\mathbf{e}}_{1} \notin \mathop{\bigcup }\limits_{{i = 1}}^{m}{V}_{i}$ . 定义 ${V}_{m + 1} =$ $L\left( {\mathbf{e}}_{1}\right)$ ,再由例 3.54 可知,存在向量 ${\mathbf{e}}_{2} \in V$ ,使得 ${\mathbf{e}}_{2} \notin \mathop{\bigcup }\limits_{{i = 1}}^{{m + 1}}{V}_{i}$ . 由例 3.7 可知, ${\mathbf{e}}_{2} \notin L\left( {\mathbf{e}}_{1}\right)$ 意味着 ${\mathbf{e}}_{1},{\mathbf{e}}_{2}$ 线性无关. 重新定义 ${V}_{m + 1} = L\left( {{\mathbf{e}}_{1},{\mathbf{e}}_{2}}\right)$ ,再由例 3.54 可知, 存在向量 ${\mathbf{e}}_{3} \in V$ ,使得 ${\mathbf{e}}_{3} \notin \mathop{\bigcup }\limits_{{i = 1}}^{{m + 1}}{V}_{i}$ . 再由例 3.7 可知, ${\mathbf{e}}_{3} \notin L\left( {{\mathbf{e}}_{1},{\mathbf{e}}_{2}}\right)$ 意味着 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},{\mathbf{e}}_{3}$ 线性无关. 不断重复上述讨论,即添加线性无关的向量重新定义 ${V}_{m + 1}$ ,并反复利用例 3.54 和例 3.7 的结论,最后可以得到 $n$ 个线性无关的向量 ${\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}$ ,它们构成 $V$ 的一组基,且满足 ${\mathbf{e}}_{j} \notin \mathop{\bigcup }\limits_{{i = 1}}^{m}{V}_{i}, j = 1,2,\cdots, n$ .

利用 “几何问题代数化” 这一技巧, 我们可以给出上述两道例题的一个统一解法.

例 3.54 和例 3.55 的证法 2 任取 $V$ 的一组基 $\left\{ {{\mathbf{e}}_{1},{\mathbf{e}}_{2},\cdots ,{\mathbf{e}}_{n}}\right\}$ . 对任意的正整数 $k$ ,构造 $V$ 中向量 ${\mathbf{\alpha }}_{k} = {\mathbf{e}}_{1} + k{\mathbf{e}}_{2} + \cdots + {k}^{n - 1}{\mathbf{e}}_{n}$ ,设向量族 $S = \left\{ {{\mathbf{\alpha }}_{k} \mid k = 1,2,\cdots }\right\}$ . 由例 3.41 可知, $S$ 中任意 $n$ 个不同的向量都构成 $V$ 的一组基. 因为 ${V}_{i}$ 都是 $V$ 的真子空间,所以每个 ${V}_{i}$ 至多包含 $S$ 中 $n - 1$ 个向量. 由于 $S$ 是无限集合,故存在某个向量 ${\mathbf{\alpha }}_{k}$ ,使得 ${\mathbf{\alpha }}_{k}$ 不属于任何一个 ${V}_{i}$ ,这就证明了例 3.54. 进一步,在 $S$ 中还存在 $n$ 个不同的向量 ${\mathbf{\alpha }}_{{k}_{1}},{\mathbf{\alpha }}_{{k}_{2}},\cdots ,{\mathbf{\alpha }}_{{k}_{n}}$ ,使得每个 ${\mathbf{\alpha }}_{{k}_{j}}$ 都不属于任何一个 ${V}_{i}$ ,此时 $\left\{ {{\mathbf{\alpha }}_{{k}_{1}},{\mathbf{\alpha }}_{{k}_{2}},\cdots ,{\mathbf{\alpha }}_{{k}_{n}}}\right\}$ 就构成了 $V$ 的一组基,这就证明了例 3.55.

## 3.2.6 矩阵的秩

矩阵秩的计算及估计在高等代数中有着诸多的应用,例如在 $§{3.2.1}$ 中,我们利用矩阵秩的计算可以判定向量组的线性关系等. 秩的等式 (不等式) 的证明是矩阵理论中的一个难点, 要证明它们通常需要一定的技巧, 而且我们还将发现, 随着矩阵的秩在高等代数中应用的深入, 相关的证明技巧将会更丰富, 也更具有难度. 在本节中我们将主要介绍 3 种方法, 分别是利用矩阵的初等变换、线性方程组的求解理论和线性空间理论来进行矩阵秩的等式 (不等式) 的证明.

## 1. 初等变换法

因为矩阵的秩在初等变换或分块初等变换下不变, 故初等变换法是处理矩阵秩的首要方法, 然后再配合利用如下矩阵秩的基本公式, 就可以证明一系列结论.

矩阵秩的基本公式 (将在下面的例题中依次证明):

(1) 若 $k \neq 0,\mathrm{r}\left( {k\mathbf{A}}\right) = \mathrm{r}\left( \mathbf{A}\right)$ ;

(2) $\mathrm{r}\left( \mathbf{{AB}}\right) \leq \min \{ \mathrm{r}\left( \mathbf{A}\right) ,\mathrm{r}\left( \mathbf{B}\right) \}$ ;

(3) $\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right) = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ ;

(4) $\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{C} \\ \mathbf{O} & \mathbf{B} \end{array}\right) \geq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) ,\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{D} & \mathbf{B} \end{array}\right) \geq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ ;

(5) $\mathrm{r}\left( {\mathbf{A};\mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) ,\mathrm{r}\left( \begin{array}{l} \mathbf{A} \\ \mathbf{B} \end{array}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ ;

(6) $\mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) ,\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ ;

(7) $\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) \geq \left| {\mathrm{r}\left( \mathbf{A}\right) - \mathrm{r}\left( \mathbf{B}\right) }\right|$ .

例 3.56 设 $\mathbf{A}$ 是 $m \times n$ 矩阵, $k \neq 0$ ,求证: $\mathrm{r}\left( {k\mathbf{A}}\right) = \mathrm{r}\left( \mathbf{A}\right)$ .

证明 由于 $k\mathbf{A} = {\mathbf{P}}_{1}\left( k\right) {\mathbf{P}}_{2}\left( k\right) \cdots {\mathbf{P}}_{m}\left( k\right) \mathbf{A}$ ,故 $\mathrm{r}\left( {k\mathbf{A}}\right) = \mathrm{r}\left( \mathbf{A}\right)$ .

例 3.57 设 $\mathbf{A} = \left( {a}_{ij}\right) ,\mathbf{B} = \left( {b}_{ij}\right)$ 是 $m \times n$ 矩阵,且 ${b}_{ij} = {\left( -1\right) }^{i + j}{a}_{ij}$ . 求证: $\mathrm{r}\left( \mathbf{A}\right) = \mathrm{r}\left( \mathbf{B}\right) .$

证明 将 $\mathbf{A}$ 的第 $i$ 行乘以 ${\left( -1\right) }^{i}$ ,又将 $\mathbf{A}$ 的第 $j$ 列乘以 ${\left( -1\right) }^{j}$ ,即得矩阵 $\mathbf{B}$ ,因此 $\mathbf{A}$ 和 $\mathbf{B}$ 相抵,故结论成立. $\square$

例 3.58 求证: $\mathrm{r}\left( \mathbf{{AB}}\right) \leq \min \{ \mathrm{r}\left( \mathbf{A}\right) ,\mathrm{r}\left( \mathbf{B}\right) \}$ .

证明 设 $\mathbf{A}$ 是 $m \times n$ 矩阵, $\mathbf{B}$ 是 $n \times s$ 矩阵. 将矩阵 $\mathbf{B}$ 按列分块, $\mathbf{B} =$ $\left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}}\right)$ ,则 $\mathbf{{AB}} = \left( {\mathbf{A}{\mathbf{\beta }}_{1},\mathbf{A}{\mathbf{\beta }}_{2},\cdots ,\mathbf{A}{\mathbf{\beta }}_{s}}\right)$ . 若 $\mathbf{B}$ 列向量的极大无关组为 $\left\{ {{\mathbf{\beta }}_{{j}_{1}},{\mathbf{\beta }}_{{j}_{2}},\cdots ,{\mathbf{\beta }}_{{j}_{r}}}\right\}$ ,则 $\mathbf{B}$ 的任一列向量 ${\mathbf{\beta }}_{j}$ 均可用 $\left\{ {{\mathbf{\beta }}_{{j}_{1}},{\mathbf{\beta }}_{{j}_{2}},\cdots ,{\mathbf{\beta }}_{{j}_{r}}}\right\}$ 线性表示. 于是任一 $\mathbf{A}{\mathbf{\beta }}_{j}$ 也可用 $\left\{ {\mathbf{A}{\mathbf{\beta }}_{{j}_{1}},\mathbf{A}{\mathbf{\beta }}_{{j}_{2}},\cdots ,\mathbf{A}{\mathbf{\beta }}_{{j}_{r}}}\right\}$ 来线性表示. 因此向量组 $\left\{ {\mathbf{A}{\mathbf{\beta }}_{1},\mathbf{A}{\mathbf{\beta }}_{2},\cdots ,\mathbf{A}{\mathbf{\beta }}_{s}}\right\}$ 的秩不超过 $r$ ,即 $\mathrm{r}\left( \mathbf{{AB}}\right) \leq \mathrm{r}\left( \mathbf{B}\right)$ . 同理,对矩阵 $\mathbf{A}$ 用行分块的方法可以证明 $\mathrm{r}\left( \mathbf{{AB}}\right) \leq \mathrm{r}\left( \mathbf{A}\right)$ .

注 上例即是说, 矩阵相乘之后秩相等或变小. 这是证明矩阵秩的不等式时一个重要的技巧, 关键是如何选取适当的矩阵 (可以是奇异矩阵) 以取得较好的效果.

例 3.59 求证: $\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right) = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ .

证明 设 $\mathbf{A},\mathbf{B}$ 的秩分别为 ${r}_{1},{r}_{2}$ ,则存在非异阵 ${\mathbf{P}}_{1},{\mathbf{Q}}_{1}$ 和非异阵 ${\mathbf{P}}_{2},{\mathbf{Q}}_{2}$ ,使

$$
{\mathbf{P}}_{1}\mathbf{A}{\mathbf{Q}}_{1} = \left( \begin{matrix} {\mathbf{I}}_{{r}_{1}} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{matrix}\right) ,{\mathbf{P}}_{2}\mathbf{B}{\mathbf{Q}}_{2} = \left( \begin{matrix} {\mathbf{I}}_{{r}_{2}} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{matrix}\right) .
$$

于是

$$
\left( \begin{matrix} {P}_{1} & O \\ O & {P}_{2} \end{matrix}\right) \left( \begin{matrix} A & O \\ O & B \end{matrix}\right) \left( \begin{matrix} {Q}_{1} & O \\ O & {Q}_{2} \end{matrix}\right) = \left( \begin{matrix} {P}_{1}A{Q}_{1} & O \\ O & {P}_{2}B{Q}_{2} \end{matrix}\right) = \left( \begin{matrix} {I}_{{r}_{1}} & O & O & O \\ O & O & O & O \\ O & O & {I}_{{r}_{2}} & O \\ O & O & O & O \end{matrix}\right) .
$$

因此 $\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right) = {r}_{1} + {r}_{2} = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ .

例 3.59 是关于矩阵秩的一个十分基本的公式, 它除了告诉我们分块对角矩阵的秩等于每个对角矩阵秩的和之外, 我们还可以反过来用这个公式, 即看到两个矩阵秩之和时, 可以把这两个矩阵拼成一个分块对角矩阵去考虑问题. 但如果考虑的是分块上 (下) 三角矩阵的秩时, 通常我们只能得到如下的不等式.

例 3.60 求证: $\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{C} \\ \mathbf{O} & \mathbf{B} \end{array}\right) \geq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) ,\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{D} & \mathbf{B} \end{array}\right) \geq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ .

证法 1 我们只证明第一个不等式, 第二个不等式同理可证. 采用与例 3.59 相同的证法和记号, 可得

$$
\left( \begin{matrix} {P}_{1} & O \\ O & {P}_{2} \end{matrix}\right) \left( \begin{matrix} A & C \\ O & B \end{matrix}\right) \left( \begin{matrix} {Q}_{1} & O \\ O & {Q}_{2} \end{matrix}\right) = \left( \begin{matrix} {P}_{1}A{Q}_{1} & {P}_{1}C{Q}_{2} \\ O & {P}_{2}B{Q}_{2} \end{matrix}\right) = \left( \begin{matrix} {I}_{{r}_{1}} & O & {C}_{11} & {C}_{12} \\ O & O & {C}_{21} & {C}_{22} \\ O & O & {I}_{{r}_{2}} & O \\ O & O & O & O \end{matrix}\right) .
$$

在上面的分块矩阵中实施第三类分块初等变换,用 ${\mathbf{I}}_{{r}_{1}}$ 消去同行的矩阵; 用 ${\mathbf{I}}_{{r}_{2}}$ 消去同列的矩阵,再将 ${\mathbf{C}}_{22}$ 对换到第 $\left( {2,2}\right)$ 位置:

$$
\left( \begin{matrix} {I}_{{r}_{1}} & O & {C}_{11} & {C}_{12} \\ O & O & {C}_{21} & {C}_{22} \\ O & O & {I}_{{r}_{2}} & O \\ O & O & O & O \end{matrix}\right) \rightarrow \left( \begin{matrix} {I}_{{r}_{1}} & O & O & O \\ O & O & O & {C}_{22} \\ O & O & {I}_{{r}_{2}} & O \\ O & O & O & O \end{matrix}\right) \rightarrow \left( \begin{matrix} {I}_{{r}_{1}} & O & O & O \\ O & {C}_{22} & O & O \\ O & O & {I}_{{r}_{2}} & O \\ O & O & O & O \end{matrix}\right) ,
$$

再由例 3.59 可得

$$
\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{C} \\ \mathbf{O} & \mathbf{B} \end{array}\right) = \mathrm{r}\left( {\mathbf{I}}_{{r}_{1}}\right) + \mathrm{r}\left( {\mathbf{C}}_{22}\right) + \mathrm{r}\left( {\mathbf{I}}_{{r}_{2}}\right) \geq {r}_{1} + {r}_{2} = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) .
$$

证法 2 我们也可用子式法来证明. 设 $\mathrm{r}\left( \begin{array}{ll} A & O \\ O & B \end{array}\right) = r$ ,则由 $§{3.1.6}$ 定理 4 可知, $\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right)$ 有一个 $r$ 阶子式不为零,不妨设为 $\left| \begin{matrix} {\mathbf{A}}_{1} & \mathbf{O} \\ \mathbf{O} & {\mathbf{B}}_{1} \end{matrix}\right|$ ,其中 ${\mathbf{A}}_{1},{\mathbf{B}}_{1}$ 分别是 $\mathbf{A},\mathbf{B}$ 的子阵. 注意 ${\mathbf{A}}_{1}$ 或 ${\mathbf{B}}_{1}$ 允许是零阶矩阵,这对应于该子式完全包含在 $\mathbf{B}$ 或 $\mathbf{A}$ 中,但若 ${\mathbf{A}}_{1},{\mathbf{B}}_{1}$ 的阶数都大于零,则通过该子式非零容易验证 ${\mathbf{A}}_{1},{\mathbf{B}}_{1}$ 都是方阵. 设在矩阵 $\left( \begin{array}{ll} A & C \\ O & B \end{array}\right)$ 中对应的 $r$ 阶子式是 $\left| \begin{array}{ll} {A}_{1} & {C}_{1} \\ O & {B}_{1} \end{array}\right|$ ,则由 Laplace 定理可

得 $\left| \begin{matrix} {\mathbf{A}}_{1} & {\mathbf{C}}_{1} \\ \mathbf{O} & {\mathbf{B}}_{1} \end{matrix}\right| = \left| {\mathbf{A}}_{1}\right| \left| {\mathbf{B}}_{1}\right| = \left| \begin{matrix} {\mathbf{A}}_{1} & \mathbf{O} \\ \mathbf{O} & {\mathbf{B}}_{1} \end{matrix}\right| \neq 0$ ,再次由 $§{3.1.6}$ 定理 4 可得

$$
\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{C} \\ \mathbf{O} & \mathbf{B} \end{array}\right) \geq r = \mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right) = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) .
$$

例 3.61 求证: $\mathrm{r}\left( {\mathbf{A};\mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) ,\mathrm{r}\left( \begin{array}{l} \mathbf{A} \\ \mathbf{B} \end{array}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ .

证明 注意到

$$
\left( {\mathbf{I};\mathbf{I}}\right) \left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right) = \left( {\mathbf{A};\mathbf{B}}\right) ,\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right) \left( \begin{array}{l} \mathbf{I} \\ \mathbf{I} \end{array}\right) = \left( \begin{array}{l} \mathbf{A} \\ \mathbf{B} \end{array}\right) ,
$$

故由例 3.58 和例 3.59 即得结论.

例 3.62 求证: $\mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) ,\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ .

证明 注意到

$$
\left( {\mathbf{A}!\mathbf{B}}\right) \left( \begin{array}{l} \mathbf{I} \\ \mathbf{I} \end{array}\right) = \mathbf{A} + \mathbf{B},\left( {\mathbf{A}!\mathbf{B}}\right) \left( \begin{matrix} \mathbf{I} \\ - \mathbf{I} \end{matrix}\right) = \mathbf{A} - \mathbf{B},
$$

故由例 3.58 和例 3.61 即得结论. [

例 3.63 求证: $\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) \geq \left| {\mathrm{r}\left( \mathbf{A}\right) - \mathrm{r}\left( \mathbf{B}\right) }\right|$ .

证明 由于 $\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) = \mathrm{r}\left( {\mathbf{B} - \mathbf{A}}\right)$ ,故不妨设 $\mathrm{r}\left( \mathbf{A}\right) \geq \mathrm{r}\left( \mathbf{B}\right)$ ,则由例 3.62 可得 $\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) + \mathrm{r}\left( \mathbf{B}\right) \geq \mathrm{r}\left( {\mathbf{A} - \mathbf{B} + \mathbf{B}}\right) = \mathrm{r}\left( \mathbf{A}\right)$ ,即 $\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) \geq \mathrm{r}\left( \mathbf{A}\right) - \mathrm{r}\left( \mathbf{B}\right)$ .

例 3.64 (Sylvester 不等式) 设 $\mathbf{A}$ 是 $m \times n$ 矩阵, $\mathbf{B}$ 是 $n \times t$ 矩阵,求证:

$$
\mathrm{r}\left( \mathbf{{AB}}\right) \geq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) - n.
$$

证明 考虑下列矩阵的分块初等变换:

$$
\left( \begin{matrix} {I}_{n} & O \\ O & {AB} \end{matrix}\right) \rightarrow \left( \begin{matrix} {I}_{n} & O \\ A & {AB} \end{matrix}\right) \rightarrow \left( \begin{matrix} {I}_{n} & - B \\ A & O \end{matrix}\right) \rightarrow \left( \begin{matrix} B & {I}_{n} \\ O & A \end{matrix}\right) ,
$$

由例 3.59 和例 3.60 可得

$$
\mathrm{r}\left( \mathbf{{AB}}\right) + n = \mathrm{r}\left( \begin{matrix} {\mathbf{I}}_{n} & \mathbf{O} \\ \mathbf{O} & \mathbf{{AB}} \end{matrix}\right) = \mathrm{r}\left( \begin{matrix} \mathbf{B} & {\mathbf{I}}_{n} \\ \mathbf{O} & \mathbf{A} \end{matrix}\right) \geq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) ,
$$

即 $\mathrm{r}\left( {\mathbf{A}\mathbf{B}}\right) \geq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) - n$ .

推论 若 $\mathbf{A}$ 是 $m \times n$ 矩阵, $\mathbf{B}$ 是 $n \times t$ 矩阵且 $\mathbf{A}\mathbf{B} = \mathbf{O}$ ,则 $\mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) \leq n$ .

例 3.65 设有 $m$ 个 $n$ 阶矩阵其积为零: ${\mathbf{A}}_{1}{\mathbf{A}}_{2}\cdots {\mathbf{A}}_{m} = \mathbf{O}$ ,求证:

$$
\mathrm{r}\left( {\mathbf{A}}_{1}\right) + \mathrm{r}\left( {\mathbf{A}}_{2}\right) + \cdots + \mathrm{r}\left( {\mathbf{A}}_{m}\right) \leq \left( {m - 1}\right) n.
$$

证明 用归纳法. 当 $m = 2$ 时,由上面的推论即得. 设 $m$ 时结论成立. 对 $m + 1$ ,令 ${\mathbf{A}}_{m}{\mathbf{A}}_{m + 1} = \mathbf{B}$ ,则 ${\mathbf{A}}_{1}{\mathbf{A}}_{2}\cdots \mathbf{B} = {\mathbf{A}}_{1}{\mathbf{A}}_{2}\cdots {\mathbf{A}}_{m}{\mathbf{A}}_{m + 1} = \mathbf{O}$ ,再由 $\mathrm{r}\left( \mathbf{B}\right) \geq$ $\mathrm{r}\left( {\mathbf{A}}_{m}\right) + \mathrm{r}\left( {\mathbf{A}}_{m + 1}\right) - n$ 及归纳假设,得

$$
\mathrm{r}\left( {\mathbf{A}}_{1}\right) + \mathrm{r}\left( {\mathbf{A}}_{2}\right) + \cdots + \mathrm{r}\left( {\mathbf{A}}_{m}\right) + \mathrm{r}\left( {\mathbf{A}}_{m + 1}\right) - n \leq \mathrm{r}\left( {\mathbf{A}}_{1}\right) + \mathrm{r}\left( {\mathbf{A}}_{2}\right) + \cdots + \mathrm{r}\left( \mathbf{B}\right) \leq \left( {m - 1}\right) n,
$$

从而

$$
\mathrm{r}\left( {\mathbf{A}}_{1}\right) + \mathrm{r}\left( {\mathbf{A}}_{2}\right) + \cdots + \mathrm{r}\left( {\mathbf{A}}_{m}\right) + \mathrm{r}\left( {\mathbf{A}}_{m + 1}\right) \leq {mn}.
$$

注 用同样的方法可以证明下列更一般的结论:

$$
\mathrm{r}\left( {\mathbf{A}}_{1}\right) + \mathrm{r}\left( {\mathbf{A}}_{2}\right) + \cdots + \mathrm{r}\left( {\mathbf{A}}_{m}\right) \leq \mathrm{r}\left( {{\mathbf{A}}_{1}{\mathbf{A}}_{2}\cdots {\mathbf{A}}_{m}}\right) + \left( {m - 1}\right) n.
$$

我们还可以将 Sylvester 不等式进行如下的推广.

例 3.66 (Frobenius 不等式) 证明: $\mathrm{r}\left( {\mathbf{A}\mathbf{B}\mathbf{C}}\right) \geq \mathrm{r}\left( {\mathbf{A}\mathbf{B}}\right) + \mathrm{r}\left( {\mathbf{B}\mathbf{C}}\right) - \mathrm{r}\left( \mathbf{B}\right)$ .

证明 考虑下列分块初等变换:

$$
\left( \begin{matrix} {ABC} & O \\ O & B \end{matrix}\right) \rightarrow \left( \begin{matrix} {ABC} & {AB} \\ O & B \end{matrix}\right) \rightarrow \left( \begin{matrix} O & {AB} \\ - {BC} & B \end{matrix}\right) \rightarrow \left( \begin{matrix} {AB} & O \\ B & {BC} \end{matrix}\right) .
$$

由例 3.59 和例 3.60 可得

$$
\mathrm{r}\left( {ABC}\right) + \mathrm{r}\left( B\right) = \mathrm{r}\left( \begin{matrix} {ABC} & O \\ O & B \end{matrix}\right) = \mathrm{r}\left( \begin{matrix} {AB} & O \\ B & {BC} \end{matrix}\right) \geq \mathrm{r}\left( {AB}\right) + \mathrm{r}\left( {BC}\right) ,
$$

由此便可得到所需不等式.

下面我们给出幂等矩阵和对合矩阵关于秩的判定准则.

例 3.67 求证: $n$ 阶矩阵 $\mathbf{A}$ 是幂等矩阵 (即 ${\mathbf{A}}^{2} = \mathbf{A}$ ) 的充要条件是:

$$
\mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( {{\mathbf{I}}_{n} - \mathbf{A}}\right) = n.
$$

证明 在下列矩阵的分块初等变换中矩阵的秩保持不变:

$$
\left( \begin{matrix} A & O \\ O & I - A \end{matrix}\right) \rightarrow \left( \begin{matrix} A & A \\ O & I - A \end{matrix}\right) \rightarrow \left( \begin{matrix} A & A \\ A & I \end{matrix}\right) \rightarrow \left( \begin{matrix} A - {A}^{2} & A \\ O & I \end{matrix}\right) \rightarrow \left( \begin{matrix} A - {A}^{2} & O \\ O & I \end{matrix}\right) .
$$

因此

$$
\mathrm{r}\left( \begin{matrix} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{I} - \mathbf{A} \end{matrix}\right) = \mathrm{r}\left( \begin{matrix} \mathbf{A} - {\mathbf{A}}^{2} & \mathbf{O} \\ \mathbf{O} & \mathbf{I} \end{matrix}\right)
$$

即 $\mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( {\mathbf{I} - \mathbf{A}}\right) = \mathrm{r}\left( {\mathbf{A} - {\mathbf{A}}^{2}}\right) + n$ . 由此即得结论.

例 3.68 求证: $n$ 阶矩阵 $\mathbf{A}$ 是对合矩阵 (即 $\left. {{\mathbf{A}}^{2} = {\mathbf{I}}_{n}}\right)$ 的充要条件是:

$$
\mathrm{r}\left( {{\mathbf{I}}_{n} + \mathbf{A}}\right) + \mathrm{r}\left( {{\mathbf{I}}_{n} - \mathbf{A}}\right) = n.
$$

证明 在下列矩阵的分块初等变换中矩阵的秩保持不变:

$$
\left( \begin{matrix} {{I}_{n} + A} & O \\ O & {{I}_{n} - A} \end{matrix}\right) \rightarrow \left( \begin{matrix} {{I}_{n} + A} & {{I}_{n} + A} \\ O & {{I}_{n} - A} \end{matrix}\right) \rightarrow \left( \begin{matrix} {{I}_{n} + A} & {{I}_{n} + A} \\ {{I}_{n} + A} & {2{I}_{n}} \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} \frac{1}{2}\left( {{\mathbf{I}}_{n} - {\mathbf{A}}^{2}}\right) & {\mathbf{I}}_{n} - \mathbf{A} \\ \mathbf{O} & 2{\mathbf{I}}_{n} \end{matrix}\right) \rightarrow \left( \begin{matrix} \frac{1}{2}\left( {{\mathbf{I}}_{n} - {\mathbf{A}}^{2}}\right) & \mathbf{O} \\ \mathbf{O} & 2{\mathbf{I}}_{n} \end{matrix}\right) .
$$

因此

$$
\mathrm{r}\left( \begin{matrix} {\mathbf{I}}_{n} + \mathbf{A} & \mathbf{O} \\ \mathbf{O} & {\mathbf{I}}_{n} - \mathbf{A} \end{matrix}\right) = \mathrm{r}\left( \begin{matrix} \frac{1}{2}\left( {{\mathbf{I}}_{n} - {\mathbf{A}}^{2}}\right) & \mathbf{O} \\ \mathbf{O} & 2{\mathbf{I}}_{n} \end{matrix}\right) ,
$$

即 $\mathrm{r}\left( {{\mathbf{I}}_{n} + \mathbf{A}}\right) + \mathrm{r}\left( {{\mathbf{I}}_{n} - \mathbf{A}}\right) = \mathrm{r}\left( {{\mathbf{I}}_{n} - {\mathbf{A}}^{2}}\right) + n$ . 由此即得结论.

例 3.69 设 $\mathbf{A}$ 是 $n$ 阶矩阵,求证: $\mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( {{\mathbf{I}}_{n} + \mathbf{A}}\right) \geq n$ .

证法 1 由下列初等变换即得

$$
\left( \begin{matrix} A & O \\ O & I + A \end{matrix}\right) \rightarrow \left( \begin{matrix} A & A \\ O & I + A \end{matrix}\right) \rightarrow \left( \begin{matrix} A & A \\ - A & I \end{matrix}\right) \rightarrow \left( \begin{matrix} A + {A}^{2} & O \\ - A & I \end{matrix}\right) \rightarrow \left( \begin{matrix} A + {A}^{2} & O \\ O & I \end{matrix}\right) .
$$

证法 $2\;\mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( {\mathbf{I} + \mathbf{A}}\right) = \mathrm{r}\left( {-\mathbf{A}}\right) + \mathrm{r}\left( {\mathbf{I} + \mathbf{A}}\right) \geq \mathrm{r}\left( {-\mathbf{A} + \mathbf{I} + \mathbf{A}}\right) = \mathrm{r}\left( \mathbf{I}\right) = n$ .

例 3.70 设有分块矩阵

$$
M = \left( \begin{array}{ll} A & B \\ C & D \end{array}\right)
$$

若 $\mathbf{A}$ 是非异阵,求证: $\mathrm{r}\left( \mathbf{M}\right) = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( {\mathbf{D} - \mathbf{C}{\mathbf{A}}^{-1}\mathbf{B}}\right)$ .

证明 用分块初等变换得:

$$
\left( \begin{array}{ll} A & B \\ C & D \end{array}\right) \rightarrow \left( \begin{matrix} A & B \\ O & D - C{A}^{-1}B \end{matrix}\right) \rightarrow \left( \begin{matrix} A & O \\ O & D - C{A}^{-1}B \end{matrix}\right) ,
$$

因此结论成立.

例 3.71 设 $A, B$ 都是数域 $\mathbb{K}$ 上的 $n$ 阶矩阵且 ${AB} = {BA}$ ,证明:

$$
\mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) - \mathrm{r}\left( \mathbf{{AB}}\right) .
$$

证明 考虑如下分块矩阵的乘法:

$$
\left( \begin{matrix} I & I \\ O & I \end{matrix}\right) \left( \begin{matrix} A & O \\ O & B \end{matrix}\right) \left( \begin{matrix} I & { - B} \\ I & A \end{matrix}\right) = \left( \begin{matrix} {A + B} & { - {AB} + {BA}} \\ B & {BA} \end{matrix}\right) = \left( \begin{matrix} {A + B} & O \\ B & {AB} \end{matrix}\right) .
$$

由例 3.58 和例 3.60 可得

$$
\mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) = \mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{O} \\ \mathbf{O} & \mathbf{B} \end{array}\right) \geq \mathrm{r}\left( \begin{matrix} \mathbf{A} + \mathbf{B} & \mathbf{O} \\ \mathbf{B} & \mathbf{B}\mathbf{A} \end{matrix}\right) \geq \mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) + \mathrm{r}\left( {\mathbf{A}\mathbf{B}}\right) ,
$$

由此即得结论.

## 2. 利用线性方程组的求解理论讨论矩阵的秩

设 $\mathbf{A}$ 是数域 $\mathbb{K}$ 上的 $m \times n$ 矩阵,则齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的解集 ${V}_{\mathbf{A}}$ 是 $n$ 维列向量空间 ${\mathbb{K}}^{n}$ 的子空间. 根据线性方程组的求解理论,我们有

$$
\dim {V}_{\mathbf{A}} + \mathrm{r}\left( \mathbf{A}\right) = n
$$

即齐次线性方程组解空间的维数与系数矩阵的秩之和等于未知数的个数. 根据上述公式, 由矩阵的秩可以讨论线性方程组解的性质; 反过来, 也可以由线性方程组解的性质讨论矩阵的秩. 下面的几个例子具有一定的典型性.

例 3.72 设 $\mathbf{A}$ 是 $m \times n$ 实矩阵,求证: $\mathrm{r}\left( {{\mathbf{A}}^{\prime }\mathbf{A}}\right) = \mathrm{r}\left( {\mathbf{A}{\mathbf{A}}^{\prime }}\right) = \mathrm{r}\left( \mathbf{A}\right)$ .

证明 首先证明 $\mathrm{r}\left( {{\mathbf{A}}^{\prime }\mathbf{A}}\right) = \mathrm{r}\left( \mathbf{A}\right)$ ,为此我们将证明齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 和 ${A}^{\prime }{Ax} = 0$ 同解. 显然 ${Ax} = 0$ 的解都是 ${A}^{\prime }{Ax} = 0$ 的解. 反之,若实向量 $\mathbf{\alpha }$ 是方程组 ${\mathbf{A}}^{\prime }\mathbf{A}\mathbf{x} = \mathbf{0}$ 的解,则 ${\mathbf{\alpha }}^{\prime }{\mathbf{A}}^{\prime }\mathbf{A}\mathbf{\alpha } = 0$ ,即 ${\left( \mathbf{A}\mathbf{\alpha }\right) }^{\prime }\left( {\mathbf{A}\mathbf{\alpha }}\right) = 0$ . 记 $\mathbf{A}\mathbf{\alpha } =$ ${\left( {b}_{1},{b}_{2},\cdots ,{b}_{m}\right) }^{\prime }$ ,则

$$
{b}_{1}^{2} + {b}_{2}^{2} + \cdots + {b}_{m}^{2} = 0.
$$

因为 ${b}_{i}$ 是实数,故每个 ${b}_{i} = 0$ ,即 $\mathbf{A}\mathbf{\alpha } = \mathbf{0}$ ,也就是说, $\mathbf{\alpha }$ 是 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的解. 这就证明了方程组 ${Ax} = 0$ 和 ${A}^{\prime }{Ax} = 0$ 同解,因此 $\mathrm{r}\left( {{A}^{\prime }A}\right) = \mathrm{r}\left( A\right)$ . 在上述等式中用 ${A}^{\prime }$ 替代 $\mathbf{A}$ 可得 $\mathrm{r}\left( {\mathbf{A}{\mathbf{A}}^{\prime }}\right) = \mathrm{r}\left( {\mathbf{A}}^{\prime }\right)$ ,又因为 $\mathrm{r}\left( \mathbf{A}\right) = \mathrm{r}\left( {\mathbf{A}}^{\prime }\right)$ ,故结论得证.

例 3.73 设 $\mathbf{A}$ 和 $\mathbf{B}$ 是数域 $\mathbb{K}$ 上的 $n$ 阶矩阵,若线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 和 $\mathbf{B}\mathbf{x} = \mathbf{0}$ 同解,且每个方程组的基础解系含 $m$ 个线性无关的向量,求证: $\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) \leq n - m$ .

证明 显然方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的每个解都是方程组 $\left( {\mathbf{A} - \mathbf{B}}\right) \mathbf{x} = \mathbf{0}$ 的解,因此 $\mathrm{r}\left( {\mathbf{A} - \mathbf{B}}\right) \leq n - m$ .

例 3.74 设 $\mathbf{A}$ 是 $m \times n$ 矩阵, $\mathbf{B}$ 是 $n \times k$ 矩阵,证明方程组 $\mathbf{A}\mathbf{B}\mathbf{x} = \mathbf{0}$ 和方程组 $\mathbf{B}\mathbf{x} = \mathbf{0}$ 同解的充要条件是 $\mathrm{r}\left( \mathbf{{AB}}\right) = \mathrm{r}\left( \mathbf{B}\right)$ .

证明 注意到方程组 ${Bx} = 0$ 的解都是方程组 ${ABx} = 0$ 的解,就是说 ${Bx} = 0$ 的解空间 ${V}_{B}$ 是 $\mathbf{A}\mathbf{B}\mathbf{x} = \mathbf{0}$ 的解空间 ${V}_{\mathbf{A}\mathbf{B}}$ 的子空间. 两个线性方程组同解等价于它们的解空间重合,即 ${V}_{B} = {V}_{AB}$ . 因为 ${V}_{B} \subseteq {V}_{AB}$ ,故 ${V}_{B} = {V}_{AB}$ 的充要条件是 $\dim {V}_{\mathbf{B}} = \dim {V}_{\mathbf{{AB}}}$ . 注意到 $\dim {V}_{\mathbf{B}} = k - \mathrm{r}\left( \mathbf{B}\right) ,\dim {V}_{\mathbf{{AB}}} = k - \mathrm{r}\left( \mathbf{{AB}}\right)$ ,因此上述两个方程组同解的充要条件是 $\mathrm{r}\left( \mathbf{{AB}}\right) = \mathrm{r}\left( \mathbf{B}\right)$ .

例 3.75 设 $\mathbf{A}$ 是 $m \times n$ 矩阵, $\mathbf{B}$ 是 $n \times k$ 矩阵. 若 $\mathbf{A}\mathbf{B}$ 和 $\mathbf{B}$ 有相同的秩,求证: 对任意的 $k \times l$ 矩阵 $\mathbf{C}$ ,矩阵 $\mathbf{{ABC}}$ 和矩阵 $\mathbf{{BC}}$ 也有相同的秩.

证法 1 由假设和例 3.74 可知,方程组 $\mathbf{A}\mathbf{B}\mathbf{x} = \mathbf{0}$ 和方程组 $\mathbf{B}\mathbf{x} = \mathbf{0}$ 同解. 要证明 $\mathrm{r}\left( {ABC}\right) = \mathrm{r}\left( {BC}\right)$ ,我们只要证明方程组 ${ABCx} = 0$ 和方程组 ${BCx} = 0$ 同解即可. 显然方程组 ${BCx} = 0$ 的解都是方程组 ${ABCx} = 0$ 的解. 反之,若列向量 $\mathbf{\alpha }$ 是方程组 ${ABCx} = 0$ 的解,则 $C\mathbf{\alpha }$ 是方程组 ${ABx} = 0$ 的解,因此 $C\mathbf{\alpha }$ 也是方程组 ${Bx} = 0$ 的解,即 ${BC\alpha } = 0$ ,于是 $\alpha$ 是方程组 ${BCx} = 0$ 的解. 这就证明了方程组 $\mathbf{{ABC}}\mathbf{x} = \mathbf{0}$ 和方程组 $\mathbf{{BC}}\mathbf{x} = \mathbf{0}$ 同解,从而结论得证.

证法 2 由 Frobenius 不等式可得

$$
\mathrm{r}\left( \mathbf{{ABC}}\right) \geq \mathrm{r}\left( \mathbf{{AB}}\right) + \mathrm{r}\left( \mathbf{{BC}}\right) - \mathrm{r}\left( \mathbf{B}\right) = \mathrm{r}\left( \mathbf{{BC}}\right) ,
$$

又因为 $\mathrm{r}\left( {\mathbf{A}\mathbf{B}\mathbf{C}}\right) \leq \mathrm{r}\left( {\mathbf{B}\mathbf{C}}\right)$ ,故结论得证.

例 3.71 的证法 2 设 ${V}_{A}$ 是方程组 ${Ax} = 0$ 的解空间, ${V}_{B},{V}_{AB},{V}_{A + B}$ 的意义同理. 若列向量 $\mathbf{\alpha } \in {V}_{\mathbf{A}} \cap {V}_{\mathbf{B}}$ ,即 $\mathbf{\alpha }$ 满足 $\mathbf{A}\mathbf{\alpha } = \mathbf{0}$ 且 $\mathbf{B}\mathbf{\alpha } = \mathbf{0}$ ,于是 $\left( {\mathbf{A} + \mathbf{B}}\right) \mathbf{\alpha } = \mathbf{0}$ , 即 $\alpha \in {V}_{A + B}$ ,从而 ${V}_{A} \cap {V}_{B} \subseteq {V}_{A + B}$ . 同理可证 ${V}_{A} \subseteq {V}_{BA},{V}_{B} \subseteq {V}_{AB}$ . 因为 $\mathbf{A}\mathbf{B} = \mathbf{B}\mathbf{A}$ ,所以 ${V}_{\mathbf{B}\mathbf{A}} = {V}_{\mathbf{A}\mathbf{B}}$ ,从而 ${V}_{\mathbf{A}} + {V}_{\mathbf{B}} \subseteq {V}_{\mathbf{A}\mathbf{B}}$ . 因此,我们有

$\dim \left( {{V}_{\mathbf{A}} \cap {V}_{\mathbf{B}}}\right) \leq \dim {V}_{\mathbf{A} + \mathbf{B}} = n - \mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) ,\dim \left( {{V}_{\mathbf{A}} + {V}_{\mathbf{B}}}\right) \leq \dim {V}_{\mathbf{{AB}}} = n - \mathrm{r}\left( \mathbf{{AB}}\right) .$ 上面两个不等式相加, 再由子空间的维数公式可得

$$
n - \mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) + n - \mathrm{r}\left( \mathbf{{AB}}\right) \geq \dim \left( {{V}_{\mathbf{A}} \cap {V}_{\mathbf{B}}}\right) + \dim \left( {{V}_{\mathbf{A}} + {V}_{\mathbf{B}}}\right)
$$

$$
= \dim {V}_{\mathbf{A}} + \dim {V}_{\mathbf{B}} = n - \mathrm{r}\left( \mathbf{A}\right) + n - \mathrm{r}\left( \mathbf{B}\right) ,
$$

因此 $\mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) + \mathrm{r}\left( {\mathbf{A}\mathbf{B}}\right) \leq \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ ,结论得证.

例 3.76 设齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 由 $n$ 个未知数及 $n$ 个方程式组成, 且 $\left| \mathbf{A}\right| = 0$ . 行列式 $\left| \mathbf{A}\right|$ 中某个元素 ${a}_{ij}$ 的代数余子式 ${A}_{ij} \neq 0$ . 求证: 该方程组的所有解都可写为下列形式:

$$
k\left( \begin{matrix} {A}_{i1} \\ {A}_{i2} \\ \vdots \\ {A}_{in} \end{matrix}\right) .
$$

证明 显然 $\mathbf{A}$ 的秩等于 $n - 1$ . 因此线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的基础解系只含一个向量. 注意到 $\left| \mathbf{A}\right| = 0$ ,故 $\mathbf{A}{\mathbf{A}}^{ * } = \left| \mathbf{A}\right| {\mathbf{I}}_{n} = \mathbf{O}$ ,这就是说 $\mathbf{A}$ 的伴随 ${\mathbf{A}}^{ * }$ 的任一列向量

都是 $\mathbf{{Ax}} = \mathbf{0}$ 的解. 而已知 ${A}_{ij} \neq 0$ ,从而列向量 $\left( \begin{matrix} {A}_{i1} \\ {A}_{i2} \\ \vdots \\ {A}_{in} \end{matrix}\right)$ 是 $\mathbf{{Ax}} = \mathbf{0}$ 的基础解系. [

例 3.77 设 $n$ 阶矩阵 $\mathbf{A} = \left( {a}_{ij}\right)$ 的行列式等于零,证明: ${\mathbf{A}}^{ * }$ 的秩不超过 1 .

证明 若 $\mathbf{A}$ 的秩小于 $n - 1$ ,则 $\mathbf{A}$ 的任意一个 $n - 1$ 阶子式等于零,故 ${\mathbf{A}}^{ * } = \mathbf{O}$ , ${\mathbf{A}}^{ * }$ 的秩为零. 若 $\mathbf{A}$ 的秩等于 $n - 1$ ,则由上题可知 ${\mathbf{A}}^{ * }$ 的 $n$ 个列向量都成比例且至少有一列不为零,故 ${\mathbf{A}}^{ * }$ 的秩等于 1 .

注 当 $n > 2$ 时,若 $\mathbf{A}$ 不是可逆矩阵,由上题知 ${\left( {\mathbf{A}}^{ * }\right) }^{ * } = \mathbf{O}$ ,这就给出了第 2 章例 2.27 的另外一个解法.

第 2 章解答题 14 的证法 2 由假设可知 $\mathbf{A}$ 是奇异矩阵. 若 $\mathbf{A}$ 的秩小于 $n - 1$ , 则 $\mathbf{A}$ 的任意一个代数余子式 ${A}_{ij}$ 都等于零,结论显然成立. 若 $\mathbf{A}$ 的秩等于 $n - 1$ ,则线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的基础解系只含一个向量. 又因为 $\mathbf{A}$ 的每一行元素之和都等于零,我们可以选取 $\mathbf{\alpha } = {\left( 1,1,\cdots ,1\right) }^{\prime }$ 作为 $\mathbf{{Ax}} = \mathbf{0}$ 的基础解系. 由例 3.76 的证明可知 ${A}^{ * }$ 的每一列都与 $\alpha$ 成比例,特别地, ${A}^{ * }$ 的每一行都相等. 对 ${A}^{\prime }$ 重复上面的讨论,注意到 ${\left( {\mathbf{A}}^{\prime }\right) }^{ * } = {\left( {\mathbf{A}}^{ * }\right) }^{\prime }$ ,从而 ${\mathbf{A}}^{ * }$ 的每一列都相等,于是 $\mathbf{A}$ 的所有代数余子式 ${A}_{ij}$ 都相等.

由公式 $\dim {V}_{\mathbf{A}} + \mathrm{r}\left( \mathbf{A}\right) = n$ 可以得到一个简单的推论,即线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 只有零解的充要条件是 $\mathbf{A}$ 为列满秩阵,特别地,若 $\mathbf{A}$ 是方阵,则充要条件是 $\mathbf{A}$ 为非异阵. 这一充要条件可以用来证明方阵的非异性, 我们在例 2.33 中应用过, 下面我们再来看几个典型例题.

例 3.78 设 $\mathbf{A}$ 是 $n$ 阶实反对称矩阵, $\mathbf{D} = \operatorname{diag}\left\{ {{d}_{1},{d}_{2},\cdots ,{d}_{n}}\right\}$ 是同阶对角矩阵且主对角线上元素全大于零,求证: $\left| {\mathbf{A} + \mathbf{D}}\right| > 0$ . 特别, ${\mathbf{I}}_{n} + \mathbf{A}$ 和 ${\mathbf{I}}_{n} - \mathbf{A}$ 都是非异阵.

证明 先证明 $\left| {\mathbf{A} + \mathbf{D}}\right| \neq 0$ ,即证明 $\left( {\mathbf{A} + \mathbf{D}}\right) \mathbf{x} = \mathbf{0}$ 只有零解. 因为 ${\mathbf{x}}^{\prime }\left( {\mathbf{A} + \mathbf{D}}\right) \mathbf{x} =$ 0,转置得 ${\mathbf{x}}^{\prime }\left( {-\mathbf{A} + \mathbf{D}}\right) \mathbf{x} = 0$ ,上述两式相加即得 ${\mathbf{x}}^{\prime }\mathbf{D}\mathbf{x} = 0$ . 由于 $\mathbf{D}$ 是对角矩阵且主对角线上元素全大于零,若设 $\mathbf{x} = {\left( {x}_{1},{x}_{2},\cdots ,{x}_{n}\right) }^{\prime }$ ,则 ${\mathbf{x}}^{\prime }\mathbf{D}\mathbf{x} = 0$ 表示 ${d}_{1}{x}_{1}^{2} + {d}_{2}{x}_{2}^{2} + \cdots + {d}_{n}{x}_{n}^{2} = 0$ . 考虑到 ${x}_{i}$ 都是实数,即有 $\mathbf{x} = \mathbf{0}$ .

再证明本题的结论. 设 $f\left( t\right) = \left| {t\mathbf{A} + \mathbf{D}}\right|$ ,则 $f\left( t\right)$ 是关于 $t$ 的多项式,从而是关于 $t$ 的连续函数. 注意到对任意的实数 $t, t\mathbf{A}$ 仍是实反对称矩阵,故由上面的讨论可得 $f\left( t\right) = \left| {t\mathbf{A} + \mathbf{D}}\right| \neq 0$ ,即 $f\left( t\right)$ 是 $\mathbb{R}$ 上处处不为零的连续函数. 又因为当 $t = 0$ 时, $f\left( 0\right) = \left| \mathbf{D}\right| > 0$ ,所以 $f\left( t\right)$ 只能是 $\mathbb{R}$ 上取值恒为正数的连续函数. 特别, $f\left( 1\right) = \left| {\mathbf{A} + \mathbf{D}}\right| > 0.$

* 例 3.79 如果 $n$ 阶方阵 $\mathbf{A} = \left( {a}_{ij}\right)$ 适合条件:

$$
\left| {a}_{ii}\right| > \mathop{\sum }\limits_{{j = 1, j \neq i}}^{n}\left| {a}_{ij}\right|, i = 1,2,\cdots, n,
$$

则称 $\mathbf{A}$ 是严格对角占优阵. 求证: 严格对角占优阵必是满秩阵. 若上述条件改为

$$
{a}_{ii} > \mathop{\sum }\limits_{{j = 1, j \neq i}}^{n}\left| {a}_{ij}\right|, i = 1,2,\cdots, n,
$$

求证: $\left| \mathbf{A}\right| > 0$ .

证明 对第一个结论,只需证明线性方程组 ${Ax} = 0$ 只有零解. 若有非零解,设为 $\left( {{c}_{1},{c}_{2},\cdots ,{c}_{n}}\right)$ ,假定 ${c}_{k}$ 是其中绝对值最大者. 将解代入该方程组的第 $k$ 个方程式, 得

$$
{a}_{k1}{c}_{1} + \cdots + {a}_{kk}{c}_{k} + \cdots + {a}_{kn}{c}_{n} = 0,
$$

即有

$$
- {a}_{kk}{c}_{k} = {a}_{k1}{c}_{1} + \cdots + {a}_{k, k - 1}{c}_{k - 1} + {a}_{k, k + 1}{c}_{k + 1} + \cdots + {a}_{kn}{c}_{n}.
$$

上式两边同取绝对值,由三角不等式以及 ${c}_{k}$ 是绝对值最大的假定可得

$$
\begin{aligned} \left| {a}_{kk}\right| \left| {c}_{k}\right| & \leq \left| {a}_{k1}\right| \left| {c}_{1}\right| + \cdots + \left| {a}_{k, k - 1}\right| \left| {c}_{k - 1}\right| + \left| {a}_{k, k + 1}\right| \left| {c}_{k + 1}\right| + \cdots + \left| {a}_{kn}\right| \left| {c}_{n}\right| \end{aligned}
$$

$$
\leq \left( {\mathop{\sum }\limits_{{j = 1, j \neq i}}^{n}\left| {a}_{ij}\right| }\right) \left| {c}_{k}\right|
$$

从而有

$$
\left| {a}_{kk}\right| \leq \mathop{\sum }\limits_{{j = 1, j \neq i}}^{n}\left| {a}_{ij}\right|
$$

得到矛盾. 因此方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 只有零解.

第二个结论的证明可借助连续函数性质. 考虑矩阵 $t{\mathbf{I}}_{n} + \mathbf{A}$ ,当 $t \geq 0$ 时这是一个严格对角占优矩阵,因此其行列式不为零. 而 $f\left( t\right) = \left| {t{\mathbf{I}}_{n} + \mathbf{A}}\right|$ 是关于 $t$ 的多项式且首项系数为 1,因此当 $t$ 充分大时, $f\left( t\right) > 0$ . 由于 $f\left( t\right)$ 连续,故当 $t = 0$ 时, $f\left( 0\right) = \left| \mathbf{A}\right| > 0.$

例 3.80 设 $\mathbf{A}$ 是 $n$ 阶实对称矩阵,求证: ${\mathbf{I}}_{n} + \mathrm{i}\mathbf{A}$ 和 ${\mathbf{I}}_{n} - \mathrm{i}\mathbf{A}$ 都是非异阵.

证明 只需证明 $\left( {{\mathbf{I}}_{n} + \mathrm{i}\mathbf{A}}\right) \mathbf{x} = \mathbf{0}$ 只有零解. 由 ${\overline{\mathbf{x}}}^{\prime }\left( {{\mathbf{I}}_{n} + \mathrm{i}\mathbf{A}}\right) \mathbf{x} = 0$ 共轭转置得 ${\overline{\mathbf{x}}}^{\prime }\left( {{\mathbf{I}}_{n} - \mathrm{i}\mathbf{A}}\right) \mathbf{x} = 0$ . 上述两式相加,得 ${\overline{\mathbf{x}}}^{\prime }{\mathbf{I}}_{n}\mathbf{x} = 0$ ,因此 $\mathbf{x} = \mathbf{0}$ . !

## 3. 利用线性空间理论讨论矩阵的秩

按照最初的定义, 矩阵秩的就是矩阵的行 (列) 向量组的秩, 所以通过发展起来的线性空间理论去讨论矩阵的秩是十分自然的事情. 下面我们列举一些典型的例题.

例 3.60 的证法 3 设 $\mathbf{A} = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right)$ 是 $\mathbf{A}$ 的列分块, ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是 $\mathbf{A}$ 的列向量的极大无关组; 设 $\mathbf{B} = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{l}}\right) ,\mathbf{C} = \left( {{\mathbf{\gamma }}_{1},{\mathbf{\gamma }}_{2},\cdots ,{\mathbf{\gamma }}_{l}}\right)$ 是 $\mathbf{B},\mathbf{C}$ 的列分块, ${\mathbf{\beta }}_{{j}_{1}},{\mathbf{\beta }}_{{j}_{2}},\cdots ,{\mathbf{\beta }}_{{j}_{s}}$ 是 $\mathbf{B}$ 的列向量的极大无关组,则 $\mathrm{r}\left( \mathbf{A}\right) = r$ 且 $\mathrm{r}\left( \mathbf{B}\right) = s$ .

我们接下来证明: 作为 $\left( \begin{array}{ll} A & C \\ O & B \end{array}\right)$ 的列向量, $\left( \begin{matrix} {\alpha }_{{i}_{1}} \\ 0 \end{matrix}\right) ,\cdots ,\left( \begin{matrix} {\alpha }_{{i}_{r}} \\ 0 \end{matrix}\right) ,\left( \begin{matrix} {\gamma }_{{j}_{1}} \\ {\beta }_{{j}_{1}} \end{matrix}\right) ,\cdots ,\left( \begin{matrix} {\gamma }_{{j}_{s}} \\ {\beta }_{{j}_{s}} \end{matrix}\right)$

线性无关. 设

$$
{c}_{1}\left( \begin{matrix} {\mathbf{\alpha }}_{{i}_{1}} \\ \mathbf{0} \end{matrix}\right) + \cdots + {c}_{r}\left( \begin{matrix} {\mathbf{\alpha }}_{{i}_{r}} \\ \mathbf{0} \end{matrix}\right) + {d}_{1}\left( \begin{matrix} {\mathbf{\gamma }}_{{j}_{1}} \\ {\mathbf{\beta }}_{{j}_{1}} \end{matrix}\right) + \cdots + {d}_{s}\left( \begin{matrix} {\mathbf{\gamma }}_{{j}_{s}} \\ {\mathbf{\beta }}_{{j}_{s}} \end{matrix}\right) = \mathbf{0},
$$

即

$$
{c}_{1}{\mathbf{\alpha }}_{{i}_{1}} + \cdots + {c}_{r}{\mathbf{\alpha }}_{{i}_{r}} + {d}_{1}{\mathbf{\gamma }}_{{j}_{1}} + \cdots + {d}_{s}{\mathbf{\gamma }}_{{j}_{s}} = \mathbf{0},{d}_{1}{\mathbf{\beta }}_{{j}_{1}} + \cdots + {d}_{s}{\mathbf{\beta }}_{{j}_{s}} = \mathbf{0}.
$$

由上面的假设即得 ${c}_{1} = \cdots = {c}_{r} = {d}_{1} = \cdots = {d}_{s} = 0$ ,于是上述结论得证. 因为 $\left( \begin{array}{ll} \mathbf{A} & \mathbf{C} \\ \mathbf{O} & \mathbf{B} \end{array}\right)$ 的列向量中有 $r + s$ 个线性无关,故 $\mathrm{r}\left( \begin{array}{ll} \mathbf{A} & \mathbf{C} \\ \mathbf{O} & \mathbf{B} \end{array}\right) \geq r + s = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ . $\square$

设 $\mathbf{A}$ 是矩阵, $\left| \mathbf{D}\right|$ 是 $\mathbf{A}$ 的 $r$ 阶子式, $\mathbf{A}$ 中所有包含 $\left| \mathbf{D}\right|$ 为 $r$ 阶子式的 $r + 1$ 子式称为 $\left| \mathbf{D}\right|$ 的 $r + 1$ 阶加边子式. 下面的例题给出了矩阵的秩关于加边子式的判定准则.

例 3.81 求证: 矩阵 $\mathbf{A}$ 的秩等于 $r$ 的充要条件是 $\mathbf{A}$ 存在一个 $r$ 阶子式 $\left| \mathbf{D}\right|$ 不等于零,而 $\left| \mathbf{D}\right|$ 的所有 $r + 1$ 阶加边子式全等于零.

证明 只需证明充分性. 不失一般性,我们可设 $\left| \mathbf{D}\right|$ 是由 $\mathbf{A}$ 的前 $r$ 行和前 $r$ 列构成的 $r$ 阶子式. 设

$$
\mathbf{A} = \left( \begin{matrix} {\mathbf{\alpha }}_{1} \\ {\mathbf{\alpha }}_{2} \\ \vdots \\ {\mathbf{\alpha }}_{m} \end{matrix}\right) = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right)
$$

为矩阵 $\mathbf{A}$ 的行分块和列分块,记 ${\tau }_{ \leq r}{\mathbf{\alpha }}_{i}$ 为行向量 ${\mathbf{\alpha }}_{i}$ 关于前 $r$ 列的缩短向量 (缩短向量的定义请参考例 3.12), ${\tau }_{ \leq r}{\mathbf{\beta }}_{j}$ 为列向量 ${\mathbf{\beta }}_{j}$ 关于前 $r$ 行的缩短向量. 由 $\left| \mathbf{D}\right| \neq 0$ 可得 ${\tau }_{ \leq r}{\mathbf{\alpha }}_{1},\cdots ,{\tau }_{ \leq r}{\mathbf{\alpha }}_{r}$ 线性无关,根据例 3.12 可知 ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关. 我们只要证明 ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{r}$ 是 $\mathbf{A}$ 的行向量的极大无关组即可得到 $\mathrm{r}\left( \mathbf{A}\right) = r$ . 用反证法证明,若它们不是极大无关组,则可以添加一个行向量,不妨设为 ${\mathbf{\alpha }}_{r + 1}$ ,使得 ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{r},{\mathbf{\alpha }}_{r + 1}$ 线性无关. 设 ${\mathbf{A}}_{1}$ 是 $\mathbf{A}$ 的前 $r + 1$ 行构成的矩阵,则 ${\mathbf{A}}_{1} =$ $\left( {{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{1},{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{2},\cdots ,{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{n}}\right)$ 且 $\mathrm{r}\left( {\mathbf{A}}_{1}\right) = r + 1$ . 由 $\left| \mathbf{D}\right| \neq 0$ 可得 ${\tau }_{ \leq r}{\mathbf{\beta }}_{1},\cdots ,{\tau }_{ \leq r}{\mathbf{\beta }}_{r}$ 线性无关,根据例 3.12 可知 ${\tau }_{ \leq r + 1}{\mathbf{\beta }}_{1},\cdots ,{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{r}$ 线性无关. 因为 $\mathrm{r}\left( {\mathbf{A}}_{1}\right) = r + 1$ ,故存在 ${\mathbf{A}}_{1}$ 的一个列向量,不妨设为 ${\tau }_{ \leq r + 1}{\mathbf{\beta }}_{r + 1}$ ,使得 ${\tau }_{ \leq r + 1}{\mathbf{\beta }}_{1},\cdots ,{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{r},{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{r + 1}$ 线性无关. 设 ${\mathbf{A}}_{2} = \left( {{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{1},\cdots ,{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{r},{\tau }_{ \leq r + 1}{\mathbf{\beta }}_{r + 1}}\right)$ ,即 ${\mathbf{A}}_{2}$ 是 $\mathbf{A}$ 的前 $r + 1$ 行和前 $r + 1$ 列构成的方阵,则 $\mathrm{r}\left( {\mathbf{A}}_{2}\right) = r + 1$ . 因此 $\left| {\mathbf{A}}_{2}\right| \neq 0$ 是包含 $\left| \mathbf{D}\right|$ 的加边子式,这与假设矛盾.

* 例 3.82 设 $m \times n$ 矩阵 $\mathbf{A}$ 的 $m$ 个行向量为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ ,其中 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}}$ , $\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是其极大无关组. 又设 $\mathbf{A}$ 的 $n$ 个列向量为 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ ,其中 ${\mathbf{\beta }}_{{j}_{1}},{\mathbf{\beta }}_{{j}_{2}}$ , $\cdots ,{\mathbf{\beta }}_{{j}_{r}}$ 是其极大无关组,则 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 和 ${\mathbf{\beta }}_{{j}_{1}},{\mathbf{\beta }}_{{j}_{2}},\cdots ,{\mathbf{\beta }}_{{j}_{r}}$ 交叉点上的元素组成的子矩阵 $\mathbf{D}$ 的行列式 $\left| \mathbf{D}\right| \neq 0$ .

我们要用到下列显然的引理.

引理 设 $\left\{ {{\mathbf{\alpha }}_{i} = \left( {{a}_{i1},{a}_{i2},\cdots ,{a}_{in}}\right) \left( {i = 1,2,\cdots, r}\right) }\right\}$ 是一组 $n$ 维行向量, $\mathbf{\alpha } =$ $\left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right)$ ,且

$$
\mathbf{\alpha } = {k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{r}{\mathbf{\alpha }}_{r}
$$

记 ${\widetilde{\mathbf{\alpha }}}_{i}$ 是 ${\mathbf{\alpha }}_{i}$ 的 $t$ 维缩短向量 ${\widetilde{\mathbf{\alpha }}}_{i} = \left( {{a}_{i{j}_{1}},{a}_{i{j}_{2}},\cdots ,{a}_{i{j}_{t}}}\right) ,\widetilde{\mathbf{\alpha }} = \left( {{a}_{{j}_{1}},{a}_{{j}_{2}},\cdots ,{a}_{{j}_{t}}}\right)$ ,则

$$
\widetilde{\mathbf{\alpha }} = {k}_{1}{\widetilde{\mathbf{\alpha }}}_{1} + {k}_{2}{\widetilde{\mathbf{\alpha }}}_{2} + \cdots + {k}_{r}{\widetilde{\mathbf{\alpha }}}_{r}.
$$

下面证明例 3.82.

证明 因为 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是极大无关组,故 $\mathbf{A}$ 的任一行向量 ${\mathbf{\alpha }}_{s}$ 均可表示为向量组 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 的线性组合. 记 ${\widetilde{\mathbf{\alpha }}}_{{i}_{1}},{\widetilde{\mathbf{\alpha }}}_{{i}_{2}},\cdots ,{\widetilde{\mathbf{\alpha }}}_{{i}_{r}},{\widetilde{\mathbf{\alpha }}}_{s}$ 分别是 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots$ , ${\mathbf{\alpha }}_{{i}_{r}},{\mathbf{\alpha }}_{s}$ 处在 ${j}_{1},{j}_{2},\cdots ,{j}_{r}$ 列的缩短向量,则由引理, ${\widetilde{\mathbf{\alpha }}}_{s}$ 可以表示为 ${\widetilde{\mathbf{\alpha }}}_{{i}_{1}},{\widetilde{\mathbf{\alpha }}}_{{i}_{2}},\cdots ,{\widetilde{\mathbf{\alpha }}}_{{i}_{r}}$ 的线性组合. 考虑由列向量 ${\mathbf{\beta }}_{{j}_{1}},{\mathbf{\beta }}_{{j}_{2}},\cdots ,{\mathbf{\beta }}_{{j}_{r}}$ 组成的矩阵 $\mathbf{B} = \left( {{\mathbf{\beta }}_{{j}_{1}},{\mathbf{\beta }}_{{j}_{2}},\cdots ,{\mathbf{\beta }}_{{j}_{r}}}\right)$ ,这是个 $m \times r$ 矩阵且秩等于 $r$ . 由于矩阵 $\mathbf{B}$ 的任一行向量都可用 ${\widetilde{\mathbf{\alpha }}}_{{i}_{1}},{\widetilde{\mathbf{\alpha }}}_{{i}_{2}},\cdots ,{\widetilde{\mathbf{\alpha }}}_{{i}_{r}}$ 线性表示,并且 $\mathbf{B}$ 的行秩等于 $r$ ,则由例 3.19 可知, ${\widetilde{\mathbf{\alpha }}}_{{i}_{1}},{\widetilde{\mathbf{\alpha }}}_{{i}_{2}},\cdots ,{\widetilde{\mathbf{\alpha }}}_{{i}_{r}}$ 是 $\mathbf{B}$ 的行向量的极大无关组,从而它们线性无关. 注意到 $r$ 阶方阵 $\mathbf{D}$ 的行向量恰好是 ${\widetilde{\mathbf{\alpha }}}_{{i}_{1}},{\widetilde{\mathbf{\alpha }}}_{{i}_{2}},\cdots ,{\widetilde{\mathbf{\alpha }}}_{{i}_{r}}$ , 因此 $\mathbf{D}$ 是满秩阵,从而 $\left| \mathbf{D}\right| \neq 0$ . [

例 3.83 设 $\mathbf{A}$ 是一个 $n$ 阶方阵, $\mathbf{A}$ 的第 ${i}_{1},\cdots ,{i}_{r}$ 行和第 ${i}_{1},\cdots ,{i}_{r}$ 列交点上的元素组成的子式称为 $\mathbf{A}$ 的一个主子式. 若 $\mathbf{A}$ 是对称矩阵或反对称矩阵且秩等于 $r$ : 求证: $\mathbf{A}$ 必有一个 $r$ 阶主子式不等于零.

证法 1 由对称性 (或反对称性),若 $\mathbf{A}$ 的第 ${i}_{1},\cdots ,{i}_{r}$ 行是 $\mathbf{A}$ 的行向量的极大无关组,则它的第 ${i}_{1},\cdots ,{i}_{r}$ 列也是 $\mathbf{A}$ 的列向量的极大无关组,因此由例 3.82 可知, 它们交点上的元素组成的 $r$ 阶主子式不等于零.

证法 2 同上假定 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 是 $\mathbf{A}$ 的行向量的极大无关组,用初等行变换可将这些行向量换到前 $r$ 行,再用对称的初等列变换可将列向量 ${\mathbf{\beta }}_{{i}_{1}},{\mathbf{\beta }}_{{i}_{2}},\cdots ,{\mathbf{\beta }}_{{i}_{r}}$ 换到前 $r$ 列,得到的矩阵记为 $\mathbf{B},\mathbf{B}$ 仍是对称矩阵 (或反对称矩阵),且 $\mathbf{A}$ 的第 ${i}_{1},{i}_{2},\cdots ,{i}_{r}$ 行和第 ${i}_{1},{i}_{2},\cdots ,{i}_{r}$ 列交叉点上的元素组成的行列式变成变换后矩阵 $\mathbf{B}$ 的处于左上方的 $r$ 阶主子式 $\left| \mathbf{D}\right|$ . 现要证明 $\left| \mathbf{D}\right| \neq 0.\mathbf{B}$ 的后 $n - r$ 个行向量中的每个都是前 $r$ 个行向量的线性组合,因此可用第三类初等行变换将它们消去. 接着进行对称的第三类初等列变换,得到的矩阵记为 $\mathbf{C}$ ,则 $\mathbf{C}$ 是对称矩阵 (或反对称矩阵). 由对称性 (反对称性), $\mathbf{C}$ 具有下列形式:

$$
C = \left( \begin{array}{ll} D & O \\ O & O \end{array}\right)
$$

因为 $\mathbf{C}$ 的秩等于 $\mathbf{A}$ 的秩,故 $\mathbf{D}$ 的秩等于 $r$ ,从而 $\left| \mathbf{D}\right| \neq 0$ . [

例 3.84 证明: 反对称矩阵的秩必为偶数.

证明 用反证法,设反对称矩阵 $\mathbf{A}$ 的秩等于 ${2r} + 1$ ,则由例 3.83 可知, $\mathbf{A}$ 有一个 ${2r} + 1$ 阶主子式 $\left| \mathbf{D}\right|$ 不等于零. 注意到反对称矩阵的主子式是反对称行列式,而奇数阶反对称行列式的值等于零,从而 $\left| \mathbf{D}\right| = 0$ ,矛盾.

例 3.71 的证法 3 设 $\mathbf{A} = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right)$ 为 $\mathbf{A}$ 的列分块, $\mathbf{B} = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots }\right.$ , $\left. {\mathbf{\beta }}_{n}\right)$ 为 $\mathbf{B}$ 的列分块. 记 ${U}_{\mathbf{A}} = L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right)$ 为 $\mathbf{A}$ 的列向量生成的 ${\mathbb{K}}^{n}$ 的子空间, ${U}_{B},{U}_{AB},{U}_{A + B}$ 的意义同理. 因为向量组 ${\alpha }_{1},{\alpha }_{2},\cdots ,{\alpha }_{n}$ 的极大无关组就是 $L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right)$ 的一组基,故 $\mathrm{r}\left( \mathbf{A}\right) = \dim {U}_{\mathbf{A}}$ ,关于 $\mathbf{B},\mathbf{A}\mathbf{B},\mathbf{A} + \mathbf{B}$ 的等式同理可得. 显然我们有 ${U}_{\mathbf{A} + \mathbf{B}} \subseteq {U}_{\mathbf{A}} + {U}_{\mathbf{B}}$ . 注意到 $\mathbf{{AB}} = \left( {\mathbf{A}{\mathbf{\beta }}_{1},\mathbf{A}{\mathbf{\beta }}_{2},\cdots ,\mathbf{A}{\mathbf{\beta }}_{n}}\right)$ ,若设 ${\mathbf{\beta }}_{j} = {\left( {b}_{1j},{b}_{2j},\cdots ,{b}_{nj}\right) }^{\prime }$ ,则 $\mathbf{{AB}}$ 的列向量 $\mathbf{A}{\mathbf{\beta }}_{j} = {b}_{1j}{\mathbf{\alpha }}_{1} + {b}_{2j}{\mathbf{\alpha }}_{2} + \cdots + {b}_{nj}{\mathbf{\alpha }}_{n} \in {U}_{\mathbf{A}}$ , 从而 ${U}_{AB} \subseteq {U}_{A}$ . 又因为 ${AB} = {BA}$ ,故 ${U}_{AB} \subseteq {U}_{A} \cap {U}_{B}$ . 最后,由上述包含关系以及子空间的维数公式可得

$$
\mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) + \mathrm{r}\left( {\mathbf{A}\mathbf{B}}\right) = \dim {U}_{\mathbf{A} + \mathbf{B}} + \dim {U}_{\mathbf{A}\mathbf{B}} \leq \dim \left( {{U}_{\mathbf{A}} + {U}_{\mathbf{B}}}\right) + \dim \left( {{U}_{\mathbf{A}} \cap {U}_{\mathbf{B}}}\right)
$$

$$
= \dim {U}_{\mathbf{A}} + \dim {U}_{\mathbf{B}} = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) .
$$

注 例 3.71 是一道矩阵秩的典型例题, 我们分别给出了它的 3 种证法, 而这恰好对应于本节中所阐述的 3 种一般的方法, 请读者好好加以体会. 从另一个角度来看, 第一种证法利用矩阵的初等变换, 从而是代数的方法; 后两种证法利用线性方程组解的理论和线性空间理论, 从而是几何的方法. 不过从本质上看, 后两种几何方法其实是一种方法, 因为它们正好对应于线性变换的核空间和像空间, 而这将是第 4 章要阐述的内容.

## 3.2.7 相抵标准型及其应用

相抵标准型是指任何一个 $m \times n$ 矩阵经初等变换均可化成如下标准型:

$$
\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right)
$$

其中 $r$ 为原矩阵的秩. 矩阵的秩 $r$ 是矩阵的相抵不变量,且两个同阶矩阵相抵的充要条件是它们的秩相等. 在 $§{2.2.5}$ 初等变换这一节,我们已经看到了相抵标准型的一些应用, 在引入了秩的概念后, 我们可以利用相抵标准型来解决更多的问题. 通常的方法是, 先对相抵标准型证明有关性质, 然后再对一般的矩阵证明同样的性质也成立. 我们来看下面几个典型的例题.

例 3.85 求证: 秩等于 $r$ 的矩阵可以表示为 $r$ 个秩等于 1 的矩阵之和,但不能表示为少于 $r$ 个秩为 1 的矩阵之和.

证明 将 $\mathbf{A}$ 化为相抵标准型,即存在非异矩阵 $\mathbf{P}$ 及 $\mathbf{Q}$ ,使

$$
\mathbf{A} = \mathbf{P}\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) \mathbf{Q}
$$

矩阵 $\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right)$ 显然可以化为 $r$ 个秩等于 1 的矩阵之和,记为 ${\mathbf{A}}_{1} + {\mathbf{A}}_{2} + \cdots + {\mathbf{A}}_{r}$ , 则 $\mathbf{A} = \mathbf{P}{\mathbf{A}}_{1}\mathbf{Q} + \mathbf{P}{\mathbf{A}}_{2}\mathbf{Q} + \cdots + \mathbf{P}{\mathbf{A}}_{r}\mathbf{Q}$ ,每个 $\mathbf{P}{\mathbf{A}}_{i}\mathbf{Q}$ 秩仍等于 1 .

若 $\mathbf{A} = {\mathbf{B}}_{1} + {\mathbf{B}}_{2} + \cdots + {\mathbf{B}}_{k}, k < r$ ,且每个 ${\mathbf{B}}_{i}$ 的秩等于 1,则由秩的不等式 $\mathrm{r}\left( {\mathbf{B} + \mathbf{C}}\right) \leq \mathrm{r}\left( \mathbf{B}\right) + \mathrm{r}\left( \mathbf{C}\right)$ 可知, $\mathbf{A}$ 的秩将不超过 $k$ ,这和 $\mathbf{A}$ 的秩等于 $r$ 矛盾,故不可能.

例 3.86 设 $\mathbf{A}$ 是 $m \times n$ 矩阵,求证:

(1) 若 $\mathrm{r}\left( \mathbf{A}\right) = n$ ,即 $\mathbf{A}$ 是列满秩阵,则必存在秩等于 $n$ 的 $n \times m$ 矩阵 $\mathbf{B}$ , 使 $\mathbf{B}\mathbf{A} = {\mathbf{I}}_{n}$ ;

(2) 若 $\mathrm{r}\left( \mathbf{A}\right) = m$ ,即 $\mathbf{A}$ 是行满秩阵,则必存在秩等于 $m$ 的 $n \times m$ 矩阵 $\mathbf{C}$ , 使 $\mathbf{{AC}} = {\mathbf{I}}_{m}$ .

证明 (1) 存在可逆矩阵 $\mathbf{P}$ 和 $\mathbf{Q}$ ,使

$$
{PAQ} = \left( \begin{matrix} {\mathbf{I}}_{n} \\ \mathbf{O} \end{matrix}\right)
$$

因此 $\left( {{I}_{n}, O}\right) {PAQ} = {I}_{n}$ ,即 $\left( {{I}_{n}, O}\right) {PA} = {Q}^{-1}$ ,也就是 $Q\left( {{I}_{n}, O}\right) {PA} = {I}_{n}$ . 令 $B =$ $\mathbf{Q}\left( {{\mathbf{I}}_{n},\mathbf{O}}\right) \mathbf{P}$ 即可.

(2) 同理可证,或者考虑 ${\mathbf{A}}^{\prime }$ 并利用 (1) 的结论.

推论 列满秩矩阵适合左消去律,即若 $\mathbf{A}$ 列满秩且 $\mathbf{{AD}} = \mathbf{{AE}}$ ,则 $\mathbf{D} = \mathbf{E}$ . 同理,行满秩矩阵适合右消去律,即若 $\mathbf{A}$ 行满秩且 $\mathbf{D}\mathbf{A} = \mathbf{E}\mathbf{A}$ ,则 $\mathbf{D} = \mathbf{E}$ .

例 3.87 设 $\mathbf{A},\mathbf{B}$ 分别是 $3 \times 2,2 \times 3$ 矩阵且满足

$$
\mathbf{{AB}} = \left( \begin{matrix} 8 & 2 & - 2 \\ 2 & 5 & 4 \\ - 2 & 4 & 5 \end{matrix}\right)
$$

试求 $\mathbf{{BA}}$ .

解 根据简单的计算可得 ${\left( AB\right) }^{2} = {9AB}$ ,经整理可得 $A\left( {{BA} - 9{I}_{2}}\right) B = O$ . 再通过简单的计算可得 $\mathrm{r}\left( \mathbf{{AB}}\right) = 2$ ,从而 $\mathrm{r}\left( \mathbf{A}\right) \geq 2,\mathrm{r}\left( \mathbf{B}\right) \geq 2$ . 又因为矩阵的秩不超过行数和列数的最小值,故 $\mathrm{r}\left( \mathbf{A}\right) = \mathrm{r}\left( \mathbf{B}\right) = 2$ ,即 $\mathbf{A}$ 是列满秩阵, $\mathbf{B}$ 是行满秩阵. 根据上述推论,可以在上式的左边消去 $\mathbf{A}$ ,右边消去 $\mathbf{B}$ ,从而可得 $\mathbf{B}\mathbf{A} = 9{\mathbf{I}}_{2}$ .

例 3.88 设 $\mathbf{A}$ 是秩为 $r$ 的 $m \times n$ 矩阵,则 $\mathbf{A} = \mathbf{B}\mathbf{C}$ ,其中 $\mathbf{B}$ 是 $m \times r$ 矩阵且 $\mathrm{r}\left( \mathbf{B}\right) = r,\mathbf{C}$ 是 $r \times n$ 矩阵且 $\mathrm{r}\left( \mathbf{C}\right) = r$ .

证明 类似例 3.86,存在可逆矩阵 $\mathbf{P}$ 和 $\mathbf{Q}$ ,使

$$
\mathbf{A} = \mathbf{P}\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) \mathbf{Q} = \mathbf{P}\left( \begin{array}{l} {\mathbf{I}}_{r} \\ \mathbf{O} \end{array}\right) \left( {{\mathbf{I}}_{r},\mathbf{O}}\right) \mathbf{Q}.
$$

令 $\mathbf{B} = \mathbf{P}\left( \begin{array}{l} {\mathbf{I}}_{r} \\ \mathbf{O} \end{array}\right) ,\mathbf{C} = \left( {{\mathbf{I}}_{r},\mathbf{O}}\right) \mathbf{Q}$ 即可. $\square$

例 3.89 设 $\mathbf{A}$ 是 $n$ 阶方阵且 $\mathrm{r}\left( \mathbf{A}\right) = r$ ,求证: ${\mathbf{A}}^{2} = \mathbf{A}$ 的充要条件是存在秩等于 $r$ 的 $n \times r$ 矩阵 $\mathbf{S}$ 和秩等于 $r$ 的 $r \times n$ 矩阵 $\mathbf{T}$ ,使 $\mathbf{A} = \mathbf{S}\mathbf{T},\mathbf{T}\mathbf{S} = {\mathbf{I}}_{r}$ .

证明 充分性显然,现证必要性. 同上题,存在可逆矩阵 $\mathbf{P}$ 和 $\mathbf{Q}$ ,使

$$
\mathbf{A} = \mathbf{P}\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) \mathbf{Q}
$$

代入 ${\mathbf{A}}^{2} = \mathbf{A}$ 消去两侧的可逆矩阵 $\mathbf{P}$ 和 $\mathbf{Q}$ ,得

$$
\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) = \left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) \mathbf{Q}\mathbf{P}\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right)
$$

只须令

$$
\mathbf{S} = \mathbf{P}\left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) \left( \begin{array}{l} {\mathbf{I}}_{r} \\ \mathbf{O} \end{array}\right) ,\mathbf{T} = \left( {{\mathbf{I}}_{r},\mathbf{O}}\right) \left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) \mathbf{Q},
$$

经简单计算即可得到结论.

注 如果读者已学过相似标准型, 用相似标准型来证明则更简单. 事实上, 由 ${\mathbf{A}}^{2} = \mathbf{A}$ 知,存在可逆矩阵 $\mathbf{P}$ ,使

$$
{\mathbf{P}}^{-1}\mathbf{{AP}} = \left( \begin{array}{ll} {\mathbf{I}}_{r} & \mathbf{O} \\ \mathbf{O} & \mathbf{O} \end{array}\right) = \left( \begin{array}{l} {\mathbf{I}}_{r} \\ \mathbf{O} \end{array}\right) \left( {{\mathbf{I}}_{r},\mathbf{O}}\right) ,
$$

所以

$$
\mathbf{A} = \mathbf{P}\left( \begin{array}{l} {\mathbf{I}}_{r} \\ \mathbf{O} \end{array}\right) \left( {{\mathbf{I}}_{r},\mathbf{O}}\right) {\mathbf{P}}^{-1}
$$

令

$$
\mathbf{S} = \mathbf{P}\left( \begin{array}{l} {\mathbf{I}}_{r} \\ \mathbf{O} \end{array}\right) ,\mathbf{T} = \left( {{\mathbf{I}}_{r},\mathbf{O}}\right) {\mathbf{P}}^{-1}
$$

即可.

## 3.2.8 线性方程组的解及其应用

如何求解线性方程组是高等代数中第一个重要的问题, 为了彻底地回答这个问题, 我们依次引入了行列式、矩阵和线性空间等概念, 并发展了它们的一整套理论, 然后才给出了这一问题的完满回答. 线性方程组的求解理论自身内容十分丰富, 包括解的判定定理和结构定理等; 其应用也十分广泛, 例如, 我们曾用线性方程组的求解理论判定某个向量能否由给定向量组线性表出, 求出交空间的基以及推导出矩阵秩的相关性质等. 在本节中, 我们将给出带参数线性方程组解的讨论以及解空间的相关性质、线性方程组公共解的讨论以及线性方程组的求解理论在解析几何上的应用等.

## 1. 线性方程组解及解的讨论

例 ${3.90\lambda }$ 为何值时,下列线性方程组有解?

$$
\left\{ \begin{array}{l} 2{x}_{1} - {x}_{2} + {x}_{3} + {x}_{4} = 1, \\ {x}_{1} + 2{x}_{2} - {x}_{3} + 4{x}_{4} = 2, \\ {x}_{1} + 7{x}_{2} - 4{x}_{3} + {11}{x}_{4} = \lambda . \end{array}\right.
$$

解 对增广矩阵进行初等变换:

$$
\left( \begin{matrix} 2 & - 1 & 1 & 1 & 1 \\ 1 & 2 & - 1 & 4 & 2 \\ 1 & 7 & - 4 & {11} & 1 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 2 & - 1 & 4 & 2 \\ 2 & - 1 & 1 & 1 & 1 \\ 1 & 7 & - 4 & {11} & 1 \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 2 & - 1 & 4 & 2 \\ 0 & - 5 & 3 & - 7 & - 3 \\ 0 & 5 & - 3 & 7 & \lambda - 2 \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 2 & - 1 & 4 & 2 \\ 0 & - 5 & 3 & - 7 & - 3 \\ 0 & 0 & 0 & 0 & 1 - 5 \end{matrix}\right) .
$$

因此,当 $\lambda = 5$ 时有无穷多组解,否则无解.

例 3.91 讨论下列线性方程组的解:

$$
\left\{ \begin{array}{l} \lambda {x}_{1} + {x}_{2} + {x}_{3} + {x}_{4} = 1, \\ {x}_{1} + \lambda {x}_{2} + {x}_{3} + {x}_{4} = \lambda , \\ {x}_{1} + {x}_{2} + \lambda {x}_{3} + {x}_{4} = {\lambda }^{2}, \\ {x}_{1} + {x}_{2} + {x}_{3} + \lambda {x}_{4} = {\lambda }^{3}. \end{array}\right.
$$

解 对增广矩阵进行初等变换 (将所有行加到第一行), 得:

$$
\left( \begin{matrix} \lambda + 3 & \lambda + 3 & \lambda + 3 & \lambda + 3 & 1 & b \\ 1 & \lambda & 1 & 1 & 1 & \lambda \\ 1 & 1 & \lambda & 1 & 1 & {\lambda }^{2} \\ 1 & 1 & 1 & \lambda & 1 & {\lambda }^{3} \end{matrix}\right)
$$

其中 $b = 1 + \lambda + {\lambda }^{2} + {\lambda }^{3}$ . 若 $\lambda = - 3$ ,则 $b = - {20}$ ,方程组无解.

现设 $\lambda \neq - 3$ . 令 $c = b/\left( {\lambda + 3}\right)$ . 上述矩阵经初等变换为

$$
\left( \begin{matrix} 1 & 1 & 1 & 1 & 1 & c \\ 1 & \lambda & 1 & 1 & 1 & \lambda \\ 1 & 1 & \lambda & 1 & 1 & \lambda \\ 1 & 1 & \lambda & 1 & 1 & \lambda \\ 1 & 1 & 1 & \lambda & 1 & \lambda \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 1 & 1 & 1 & 1 & c \\ 0 & \lambda - 1 & 0 & 0 & 1 & \lambda - c \\ 0 & 0 & \lambda - 1 & 0 & 1 & \lambda - c \\ 0 & 0 & 0 & \lambda - 1 & \lambda & 3 - c \end{matrix}\right) .
$$

当 $\lambda = 1$ 时, $c = 1$ . 因此原线性方程组有无穷多组解. 当 $\lambda \neq 1, - 3$ 时,原方程组有唯一解.

例 3.92 设 $\mathbf{A}$ 是一个 $m \times n$ 矩阵,记 ${\mathbf{\alpha }}_{i}$ 是 $\mathbf{A}$ 的第 $i$ 个行向量, $\mathbf{\beta } =$ $\left( {{b}_{1},{b}_{2},\cdots ,{b}_{n}}\right)$ . 求证: 若齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的解全是方程 ${b}_{1}{x}_{1} + {b}_{2}{x}_{2} +$ $\cdots + {b}_{n}{x}_{n} = 0$ 的解,则 $\mathbf{\beta }$ 是 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的线性组合.

证明 令 $\mathbf{B} = \left( \begin{array}{l} \mathbf{A} \\ \mathbf{\beta } \end{array}\right)$ ,由已知,方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 和方程组 $\mathbf{B}\mathbf{x} = \mathbf{0}$ 同解, 故 $\mathrm{r}\left( \mathbf{A}\right) = \mathrm{r}\left( \mathbf{B}\right)$ ,从而 $\mathbf{A}$ 的行向量的极大无关组也是 $\mathbf{B}$ 的行向量的极大无关组. 因此, $\mathbf{\beta }$ 可表示为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 的线性组合.

例 3.93 设 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 是 $m$ 个方程式 $n$ 个未知数的线性方程组,求证: 它有解的充要条件是方程组 ${\mathbf{A}}^{\prime }\mathbf{y} = \mathbf{0}$ 的任一解 $\mathbf{\alpha }$ 均适合等式 ${\mathbf{\alpha }}^{\prime }\mathbf{\beta } = 0$ .

证明 方程组 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 有解当且仅当 $\mathrm{r}\left( {\mathbf{A}!\mathbf{\beta }}\right) = \mathrm{r}\left( \mathbf{A}\right)$ ,当且仅当 $\mathrm{r}\left( \begin{array}{l} {\mathbf{A}}^{\prime } \\ {\mathbf{\beta }}^{\prime } \end{array}\right) =$ $\mathrm{r}\left( {\mathbf{A}}^{\prime }\right)$ ,当且仅当方程组 $\left( \begin{array}{l} {\mathbf{A}}^{\prime } \\ {\mathbf{\beta }}^{\prime } \end{array}\right) \mathbf{y} = \mathbf{0}$ 与 ${\mathbf{A}}^{\prime }\mathbf{y} = \mathbf{0}$ 同解,而这当且仅当 ${\mathbf{A}}^{\prime }\mathbf{y} = \mathbf{0}$ 的任一解 $\mathbf{\alpha }$ 均适合等式 ${\mathbf{\beta }}^{\prime }\mathbf{\alpha } = 0$ ,即 ${\mathbf{\alpha }}^{\prime }\mathbf{\beta } = 0$ .

例 3.94 设

$$
\mathbf{A} = \left( \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{m1} & {a}_{m2} & \cdots & {a}_{mn} \end{matrix}\right) \left( {m < n}\right) ,
$$

已知 $\mathbf{{Ax}} = \mathbf{0}$ 的基础解系为 ${\mathbf{\beta }}_{i} = {\left( {b}_{i1},{b}_{i2},\cdots ,{b}_{in}\right) }^{\prime }\left( {i = 1,2,\cdots, n - m}\right)$ ,试求齐次线性方程组

$$
\mathop{\sum }\limits_{{j = 1}}^{n}{b}_{ij}{y}_{j} = 0\left( {i = 1,2,\cdots, n - m}\right)
$$

的基础解系.

解 令 $\mathbf{B} = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n - m}}\right)$ ,则 $\mathbf{A}\mathbf{B} = \mathbf{O},{\mathbf{B}}^{\prime }{\mathbf{A}}^{\prime } = \mathbf{O}$ . 已知 $\mathbf{A}$ 的秩为 $m$ , 因此 ${\mathbf{B}}^{\prime }\mathbf{y} = \mathbf{0}$ 的基础解系为 ${\mathbf{A}}^{\prime }$ 的全部列向量,即 $\mathbf{A}$ 的所有行向量.

例 3.95 设有两个线性方程组:

$$
\left\{ \begin{matrix} {a}_{11}{x}_{1} + {a}_{12}{x}_{2} + \cdots + {a}_{1n}{x}_{n} = {b}_{1}, \\ {a}_{21}{x}_{1} + {a}_{22}{x}_{2} + \cdots + {a}_{2n}{x}_{n} = {b}_{2}, \\ \cdots \cdots \cdots \cdots \\ {a}_{m1}{x}_{1} + {a}_{m2}{x}_{2} + \cdots + {a}_{mn}{x}_{n} = {b}_{m}; \end{matrix}\right. \tag{3.1}
$$

$$
\left\{ \begin{matrix} {a}_{11}{x}_{1} + {a}_{21}{x}_{2} + \cdots + {a}_{m1}{x}_{m} = 0, \\ {a}_{12}{x}_{1} + {a}_{22}{x}_{2} + \cdots + {a}_{m2}{x}_{m} = 0, \\ \cdots \cdots \cdots \cdots \\ {a}_{1n}{x}_{1} + {a}_{2n}{x}_{2} + \cdots + {a}_{mn}{x}_{m} = 0, \\ {b}_{1}{x}_{1} + {b}_{2}{x}_{2} + \cdots + {b}_{m}{x}_{m} = 1. \end{matrix}\right. \tag{3.2}
$$

求证: 方程组 (3.1) 有解的充要条件是方程组 (3.2) 无解.

证明 设第一个线性方程组的系数矩阵为 $\mathbf{A}$ ,常数向量为 $\mathbf{\beta }$ ,则第二个线性方程组的系数矩阵和增广矩阵分别为

$$
\mathbf{B} = \left( \begin{array}{l} {\mathbf{A}}^{\prime } \\ {\mathbf{\beta }}^{\prime } \end{array}\right) ,\;\widetilde{\mathbf{B}} = \left( \begin{matrix} {\mathbf{A}}^{\prime } & \mathbf{O} \\ {\mathbf{\beta }}^{\prime } & 1 \end{matrix}\right) .
$$

显然我们有 $\mathrm{r}\left( \widetilde{\mathbf{B}}\right) = \mathrm{r}\left( {\mathbf{A}}^{\prime }\right) + 1 = \mathrm{r}\left( \mathbf{A}\right) + 1$ .

若方程组 (3.1) 有解,则 $\mathrm{r}\left( {\mathbf{A},\mathbf{\beta }}\right) = \mathrm{r}\left( \mathbf{A}\right)$ ,故 $\mathrm{r}\left( \mathbf{B}\right) = \mathrm{r}\left( {\mathbf{B}}^{\prime }\right) = \mathrm{r}\left( {\mathbf{A},\mathbf{\beta }}\right) = \mathrm{r}\left( \mathbf{A}\right) \neq$ $\mathrm{r}\left( \widetilde{\mathbf{B}}\right)$ . 因此方程组 (3.2) 无解.

反之,若方程组 (3.1) 无解,则 $\mathrm{r}\left( {\mathbf{A},\mathbf{\beta }}\right) = \mathrm{r}\left( \mathbf{A}\right) + 1$ ,故 $\mathrm{r}\left( \mathbf{B}\right) = \mathrm{r}\left( {\mathbf{B}}^{\prime }\right) = \mathrm{r}\left( {\mathbf{A},\mathbf{\beta }}\right) =$ $\mathrm{r}\left( \mathbf{A}\right) + 1 = \mathrm{r}\left( \widetilde{\mathbf{B}}\right)$ . 因此方程组 (3.2) 有解.

例 3.96 设 ${V}_{0}$ 是数域 $\mathbb{K}$ 上 $n$ 维列向量空间的真子空间,求证: 必存在矩阵 $\mathbf{A}$ , 使 ${V}_{0}$ 是 $n$ 元齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的解空间.

证明 设 ${\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{r}$ 是子空间 ${V}_{0}$ 的一组基. 令 $\mathbf{B} = \left( {{\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{r}}\right)$ ,这是一个 $n \times r$ 矩阵. 考虑齐次线性方程组 ${\mathbf{B}}^{\prime }\mathbf{x} = \mathbf{0}$ . 因为 $\mathbf{B}$ 的秩等于 $r$ ,故其基础解系含 $n - r$ 个向量,记为 ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{n - r}$ . 令 $\mathbf{A} = {\left( {\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{n - r}\right) }^{\prime }$ ,这是个 $\left( {n - r}\right) \times n$ 矩阵且秩为 $n - r$ . 显然齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的基础解系是 ${\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{r}$ ,故其解空间就是 ${V}_{0}$ .

例 3.97 设 $\mathbf{A}$ 是秩为 $r$ 的 $m \times n$ 矩阵,求证: 必存在秩为 $n - r$ 的 $n \times \left( {n - r}\right)$ 矩阵 $\mathbf{B}$ ,使 $\mathbf{A}\mathbf{B} = \mathbf{O}$ .

证明 考虑线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ ,它有 $n - r$ 个基础解系,不妨设为 ${\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{n - r}$ . 令 $\mathbf{B} = \left( {{\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{n - r}}\right)$ 即为所求.

例 3.98 设 $\mathbf{A}$ 是秩为 $r$ 的 $m \times n$ 矩阵, ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{n - r}$ 与 ${\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{n - r}$ 是齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的两个基础解系. 求证: 必存在 $n - r$ 阶可逆矩阵 $\mathbf{P}$ ,使

$$
\left( {{\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{n - r}}\right) = \left( {{\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{n - r}}\right) \mathbf{P}.
$$

证明 设 $U$ 是齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的解空间,则向量组 ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{n - r}$ 与 ${\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{n - r}$ 是 $U$ 的两组基. 令 $\mathbf{P}$ 是这两组基之间的过渡矩阵,则

$$
\left( {{\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{n - r}}\right) = \left( {{\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{n - r}}\right) \mathbf{P}.
$$

## 2. 线性方程组的公共解

若有两个含 $n$ 个未知数的齐次线性方程组 ${Ax} = 0$ 和 ${Bx} = 0$ ,要求它们的公共解只需将它们联立起来解就可以了. 如果只已知两个齐次方程组的基础解系而并不知道方程组本身, 我们只需求它们的基础解系生成的解空间的交就可以了. 而求两个子空间交的方法在 $§{3.2.5}$ 中已有交代. 对非齐次线性方程组,如果知道它们的解 (而不知道方程组本身), 要求它们的公共解, 我们可以这样做:

设 $\mathbf{A}\mathbf{x} = {\mathbf{\alpha }}_{1},\mathbf{B}\mathbf{x} = {\mathbf{\beta }}_{2}$ 是两个含 $n$ 个未知数的非齐次线性方程组. 方程组 $\mathbf{A}\mathbf{x} = {\mathbf{\beta }}_{1}$ 有特解 $\gamma$ 且 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 的基础解系为 ${\mathbf{\eta }}_{1},\cdots ,{\mathbf{\eta }}_{n - r}$ . 方程组 $\mathbf{B}\mathbf{x} = {\mathbf{\beta }}_{2}$ 有特解 $\delta$ 且 $\mathbf{B}\mathbf{x} = \mathbf{0}$ 的基础解系为 ${\mathbf{\xi }}_{1},\cdots ,{\mathbf{\xi }}_{n - s}$ .

方法 1 假设它们的公共解为 $\gamma + {t}_{1}{\eta }_{1} + \cdots + {t}_{n - r}{\eta }_{n - r}$ ,则 $\gamma + {t}_{1}{\eta }_{1} + \cdots +$ ${t}_{n - r}{\eta }_{n - r} - \delta$ 是 $\mathbf{B}\mathbf{x} = \mathbf{0}$ 的解,因此可以表示为 ${\mathbf{\xi }}_{1},\cdots ,{\mathbf{\xi }}_{n - s}$ 的线性组合. 于是矩阵 $\left( {{\mathbf{\xi }}_{1},\cdots ,{\mathbf{\xi }}_{n - s},\gamma + {t}_{1}{\mathbf{\eta }}_{1} + \cdots + {t}_{n - r}{\mathbf{\eta }}_{n - r} - \mathbf{\delta }}\right)$ 的秩等于 $n - s$ . 由此可以求出 ${t}_{1},\cdots ,{t}_{n - r}$ ,从而求出公共解.

方法 2 假设它们的公共解为 $\zeta$ ,则

$$
\zeta = \gamma + {t}_{1}{\eta }_{1} + \cdots + {t}_{n - r}{\eta }_{n - r} = \delta + \left( {-{u}_{1}}\right) {\xi }_{1} + \cdots + \left( {-{u}_{n - s}}\right) {\xi }_{n - s}.
$$

要求公共解 $\zeta$ 等价于求解下列关于未定元 ${t}_{1},\cdots ,{t}_{n - r};{u}_{1},\cdots ,{u}_{n - s}$ 的线性方程组:

$$
{t}_{1}{\eta }_{1} + \cdots + {t}_{n - r}{\eta }_{n - r} + {u}_{1}{\xi }_{1} + \cdots + {u}_{n - s}{\xi }_{n - s} = \delta - \gamma .
$$

下面是这类问题的一个典型例子.

例 3.99 设有两个非齐次线性方程组 (I), (II). 它们的通解分别为

$$
\mathbf{\gamma } + {t}_{1}{\mathbf{\eta }}_{1} + {t}_{2}{\mathbf{\eta }}_{2};\;\mathbf{\delta } + {k}_{1}{\mathbf{\xi }}_{1} + {k}_{2}{\mathbf{\xi }}_{2},
$$

其中 $\gamma = {\left( 5, - 3,0,0\right) }^{\prime },{\mathbf{\eta }}_{1} = {\left( -6,5,1,0\right) }^{\prime },{\mathbf{\eta }}_{2} = {\left( -5,4,0,1\right) }^{\prime };\mathbf{\delta } = {\left( -{11},3,0,0\right) }^{\prime }$ , ${\mathbf{\xi }}_{1} = {\left( 8, - 1,1,0\right) }^{\prime },{\mathbf{\xi }}_{2} = {\left( {10}, - 2,0,1\right) }^{\prime }$ . 求这两个方程组的公共解.

解法 1 设公共解为

$$
\mathbf{\gamma } + {t}_{1}{\mathbf{\eta }}_{1} + {t}_{2}{\mathbf{\eta }}_{2} = \left( \begin{matrix} 5 - 6{t}_{1} - 5{t}_{2} \\ - 3 + 5{t}_{1} + 4{t}_{2} \\ {t}_{1} \\ {t}_{2} \end{matrix}\right)
$$

矩阵 $\left( {{\xi }_{1},{\xi }_{2},\gamma - \delta + {t}_{1}{\eta }_{1} + {t}_{2}{\eta }_{2}}\right)$ 的秩等于 2 . 对此矩阵做初等行变换:

$$
\left( \begin{matrix} 8 & {10} & {16} - 6{t}_{1} - 5{t}_{2} \\ - 1 & - 2 & - 6 + 5{t}_{1} + 4{t}_{2} \\ 1 & 0 & {t}_{1} \\ 0 & 1 & {t}_{2} \end{matrix}\right) \rightarrow \left( \begin{matrix} 1 & 0 & {t}_{1} \\ 0 & 1 & {t}_{2} \\ 8 & {10} & {16} - 6{t}_{1} - 5{t}_{2} \\ - 1 & - 2 & - 6 + 5{t}_{1} + 4{t}_{2} \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} 1 & 0 & {t}_{1} \\ 0 & 1 & {t}_{2} \\ 0 & 0 & {16} - {14}{t}_{1} - {15}{t}_{2} \\ 0 & 0 & - 6 + 6{t}_{1} + 6{t}_{2} \end{matrix}\right)
$$

于是得到关于 ${t}_{1},{t}_{2}$ 的方程组

$$
\left\{ \begin{array}{l} {14}{t}_{1} + {15}{t}_{2} = {16} \\ 6{t}_{1} + 6{t}_{2} = 6 \end{array}\right.
$$

解得 ${t}_{1} = - 1,{t}_{2} = 2$ ,所以公共解为 (只有一个向量) $\gamma - {\eta }_{1} + 2{\eta }_{2} = {\left( 1,0, - 1,2\right) }^{\prime }$ .

解法 2 求公共解等价于求解下列线性方程组:

$$
{t}_{1}{\mathbf{\eta }}_{1} + {t}_{2}{\mathbf{\eta }}_{2} + {u}_{1}{\mathbf{\xi }}_{1} + {u}_{2}{\mathbf{\xi }}_{2} = \mathbf{\delta } - \mathbf{\gamma }.
$$

对其增广矩阵实施初等行变换, 可得

$$
\left( \begin{matrix} - 6 & - 5 & 8 & {10} & 1 & - {16} \\ 5 & 4 & - 1 & - 2 & 6 & 6 \\ 1 & 0 & 1 & 0 & 1 & 0 \\ 0 & 1 & 0 & 1 & 1 & 0 \end{matrix}\right) \rightarrow \left( \begin{array}{llllll} 1 & 0 & 0 & 0 & 1 & - 1 \\ 0 & 1 & 0 & 0 & 1 & 2 \\ 0 & 0 & 1 & 0 & 1 & 1 \\ 0 & 0 & 0 & 1 & - 2 & \end{array}\right)
$$

故 $\left( {{t}_{1},{t}_{2},{u}_{1},{u}_{2}}\right)$ 只有唯一解 $\left( {-1,2,1, - 2}\right)$ . 因此公共解为 $\gamma - {\eta }_{1} + 2{\eta }_{2} = \delta - {\xi }_{1} +$ $2{\xi }_{2} = {\left( 1,0, - 1,2\right) }^{\prime }.$

例 3.100 设有非齐次线性方程组 (I):

$$
\left\{ \begin{array}{l} 7{x}_{1} - 6{x}_{2} + 3{x}_{3} = b \\ 8{x}_{1} - 9{x}_{2} + a{x}_{4} = 7 \end{array}\right.
$$

又已知方程组 (II) 的通解为

$$
{\left( 1,1,0,0\right) }^{\prime } + {t}_{1}{\left( 1,0, - 1,0\right) }^{\prime } + {t}_{2}{\left( 2,3,0,1\right) }^{\prime }.
$$

若这两个方程组有无穷多组公共解,求出 $a, b$ 的值并求出公共解.

解 将 (II) 的通解写为 ${\left( 1 + {t}_{1} + 2{t}_{2},1 + 3{t}_{2}, - {t}_{1},{t}_{2}\right) }^{\prime }$ ,代入方程组 (I) 后化简得到

$$
\left\{ \begin{array}{l} 4{t}_{1} - 4{t}_{2} = b - 1 \\ 8{t}_{1} + \left( {a - {11}}\right) {t}_{2} = 8 \end{array}\right.
$$

要使这两个方程组有无穷多组公共解, ${t}_{1},{t}_{2}$ 必须有无穷多组解,因此上面方程组的系数矩阵和增广矩阵的秩都应该等于 1 . 于是 $a = 3, b = 5$ . 解出方程组得到 ${t}_{1} = {t}_{2} + 1$ . 所以方程组 (I), (II) 的公共解为

$$
{\left( 1 + {t}_{1} + 2{t}_{2},1 + 3{t}_{2}, - {t}_{1},{t}_{2}\right) }^{\prime } = {\left( 2,1, - 1,0\right) }^{\prime } + {t}_{2}{\left( 3,3, - 1,1\right) }^{\prime },
$$

其中 ${t}_{2}$ 为任意数.

## 3. 在解析几何上的应用

例 3.101 求平面上 $n$ 个点 $\left( {{x}_{1},{y}_{1}}\right) ,\left( {{x}_{2},{y}_{2}}\right) ,\cdots ,\left( {{x}_{n},{y}_{n}}\right)$ 位于一条直线上的充要条件.

解 充要条件为第一个点和其余点代表的向量之差属于一个一维子空间, 即 $\left( {{x}_{i} - {x}_{1},{y}_{i} - {y}_{1}}\right)$ 都成比例. 写成矩阵形式为

$$
\mathrm{r}\left( \begin{array}{llll} {x}_{2} - {x}_{1} & {x}_{3} - {x}_{1} & \cdots & {x}_{n} - {x}_{1} \\ {y}_{2} - {y}_{1} & {y}_{3} - {y}_{1} & \cdots & {y}_{n} - {y}_{1} \end{array}\right) \leq 1,
$$

或

$$
\mathrm{r}\left( \begin{matrix} {x}_{1} & {x}_{2} & {x}_{3} & \cdots & {x}_{n} \\ {y}_{1} & {y}_{2} & {y}_{3} & \cdots & {y}_{n} \\ 1 & 1 & 1 & \cdots & 1 \end{matrix}\right) \leq 2.\square
$$

例 3.102 求三维实空间中 4 点 $\left( {{x}_{i},{y}_{i},{z}_{i}}\right) \left( {1 \leq i \leq 4}\right)$ 共面的充要条件.

解 设 4 点的向量为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ ,则 4 点共面的充要条件是: 向量组 ${\mathbf{\alpha }}_{2} -$ ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{3} - {\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{4} - {\mathbf{\alpha }}_{1}$ 的秩不超过 2 . 不难将此写成矩阵形式:

$$
\mathrm{r}\left( \begin{array}{lll} {x}_{2} - {x}_{1} & {x}_{3} - {x}_{1} & {x}_{4} - {x}_{1} \\ {y}_{2} - {y}_{1} & {y}_{3} - {y}_{1} & {y}_{4} - {y}_{1} \\ {z}_{2} - {z}_{1} & {z}_{3} - {z}_{1} & {z}_{4} - {z}_{1} \end{array}\right) \leq 2,
$$

或

$$
\mathrm{r}\left( \begin{matrix} {x}_{1} & {x}_{2} & {x}_{3} & {x}_{4} \\ {y}_{1} & {y}_{2} & {y}_{3} & {y}_{4} \\ {z}_{1} & {z}_{2} & {z}_{3} & {z}_{4} \\ 1 & 1 & 1 & 1 \end{matrix}\right) \leq 3.\square
$$

例 3.103 证明: 通过平面内不在一条直线上的 3 点 $\left( {{x}_{1},{y}_{1}}\right) ,\left( {{x}_{2},{y}_{2}}\right) ,\left( {{x}_{3},{y}_{3}}\right)$ 的圆方程为

$$
\left| \begin{matrix} {x}^{2} + {y}^{2} & x & y & 1 \\ {x}_{1}^{2} + {y}_{1}^{2} & {x}_{1} & {y}_{1} & 1 \\ {x}_{2}^{2} + {y}_{2}^{2} & {x}_{2} & {y}_{2} & 1 \\ {x}_{3}^{2} + {y}_{3}^{2} & {x}_{3} & {y}_{3} & 1 \end{matrix}\right| = 0.
$$

证明 圆方程可设为

$$
{u}_{1}\left( {{x}^{2} + {y}^{2}}\right) + {u}_{2}x + {u}_{3}y + {u}_{4} = 0,
$$

于是得未知数 ${u}_{1},{u}_{2},{u}_{3},{u}_{4}$ 的方程组:

$$
\left\{ \begin{array}{l} \left( {{x}_{1}^{2} + {y}_{1}^{2}}\right) {u}_{1} + {x}_{1}{u}_{2} + {y}_{1}{u}_{3} + {u}_{4} = 0 \\ \left( {{x}_{2}^{2} + {y}_{2}^{2}}\right) {u}_{1} + {x}_{2}{u}_{2} + {y}_{2}{u}_{3} + {u}_{4} = 0 \\ \left( {{x}_{3}^{2} + {y}_{3}^{2}}\right) {u}_{1} + {x}_{3}{u}_{2} + {y}_{3}{u}_{3} + {u}_{4} = 0 \end{array}\right.
$$

上述方程组加上原方程组组成一个含 4 个未知数、 4 个方程式的齐次线性方程组. 它有非零解的充要条件是系数行列式等于零, 即

$$
\left| \begin{matrix} {x}^{2} + {y}^{2} & x & y & 1 \\ {x}_{1}^{2} + {y}_{1}^{2} & {x}_{1} & {y}_{1} & 1 \\ {x}_{2}^{2} + {y}_{2}^{2} & {x}_{2} & {y}_{2} & 1 \\ {x}_{3}^{2} + {y}_{3}^{2} & {x}_{3} & {y}_{3} & 1 \end{matrix}\right| = 0.
$$

注意到已知 3 点不在同一条直线上意味着

$$
\left| \begin{array}{lll} {x}_{1} & {y}_{1} & 1 \\ {x}_{2} & {y}_{2} & 1 \\ {x}_{3} & {y}_{3} & 1 \end{array}\right| \neq 0
$$

故圆方程不退化.

例 3.104 求平面上不在一条直线上的 4 个点 $\left( {{x}_{1},{y}_{1}}\right) ,\left( {{x}_{2},{y}_{2}}\right) ,\left( {{x}_{3},{y}_{3}}\right) ,\left( {{x}_{4},{y}_{4}}\right)$ 位于同一个圆上的充要条件.

解 利用上题得充要条件为

$$
\left| \begin{array}{llll} {x}_{1}^{2} + {y}_{1}^{2} & {x}_{1} & {y}_{1} & 1 \\ {x}_{2}^{2} + {y}_{2}^{2} & {x}_{2} & {y}_{2} & 1 \\ {x}_{3}^{2} + {y}_{3}^{2} & {x}_{3} & {y}_{3} & 1 \\ {x}_{4}^{2} + {y}_{4}^{2} & {x}_{4} & {y}_{4} & 1 \end{array}\right| = 0.\square
$$

例 3.105 已知平面上两条不同的二次曲线 ${a}_{i}{x}^{2} + {b}_{i}{xy} + {c}_{i}{y}^{2} + {d}_{i}x + {e}_{i}y + {f}_{i} =$ $0\left( {i = 1,2}\right)$ 交于 4 个不同的点 $\left( {{x}_{i},{y}_{i}}\right) \left( {i = 1,2,3,4}\right)$ . 求证: 过这 4 个点的二次曲线均可写为如下形状:

$$
{\lambda }_{1}\left( {{a}_{1}{x}^{2} + {b}_{1}{xy} + {c}_{1}{y}^{2} + {d}_{1}x + {e}_{1}y + {f}_{1}}\right) + {\lambda }_{2}\left( {{a}_{2}{x}^{2} + {b}_{2}{xy} + {c}_{2}{y}^{2} + {d}_{2}x + {e}_{2}y + {f}_{2}}\right) = 0.
$$

证明 显然上述曲线过 4 个交点. 现设 $a{x}^{2} + {bxy} + c{y}^{2} + {dx} + {ey} + f = 0$ 是过 4 个交点的二次曲线, 则有

$$
\left\{ \begin{array}{l} a{x}_{1}^{2} + b{x}_{1}{y}_{1} + c{y}_{1}^{2} + d{x}_{1} + e{y}_{1} + f = 0, \\ a{x}_{2}^{2} + b{x}_{2}{y}_{2} + c{y}_{2}^{2} + d{x}_{2} + e{y}_{2} + f = 0, \\ a{x}_{3}^{2} + b{x}_{3}{y}_{3} + c{y}_{3}^{2} + d{x}_{3} + e{y}_{3} + f = 0, \\ a{x}_{4}^{2} + b{x}_{4}{y}_{4} + c{y}_{4}^{2} + d{x}_{4} + e{y}_{4} + f = 0. \end{array}\right. \tag{3.3}
$$

视 $a, b, c, d, e, f$ 为未知数,则线性方程组 (3.3) 有线性无关解 ${\left( {a}_{1},{b}_{1},{c}_{1},{d}_{1},{e}_{1},{f}_{1}\right) }^{\prime }$ , ${\left( {a}_{2},{b}_{2},{c}_{2},{d}_{2},{e}_{2},{f}_{2}\right) }^{\prime }$ . 如果方程组 (3.3) 系数矩阵的秩等于 4,则这两个解就成了基础解系, 即可得到要求的结论.

现假定所求的二次曲线还经过另外第五点 $\left( {{x}_{5},{y}_{5}}\right)$ ,则该曲线方程可用行列式表示为

$$
\left| \begin{matrix} {x}^{2} & {xy} & {y}^{2} & x & y & 1 \\ {x}_{1}^{2} & {x}_{1}{y}_{1} & {y}_{1}^{2} & {x}_{1} & {y}_{1} & 1 \\ {x}_{2}^{2} & {x}_{2}{y}_{2} & {y}_{2}^{2} & {x}_{2} & {y}_{2} & 1 \\ {x}_{3}^{2} & {x}_{3}{y}_{3} & {y}_{3}^{2} & {x}_{3} & {y}_{3} & 1 \\ {x}_{4}^{2} & {x}_{4}{y}_{4} & {y}_{4}^{2} & {x}_{4} & {y}_{4} & 1 \\ {x}_{5}^{2} & {x}_{5}{y}_{5} & {y}_{5}^{2} & {x}_{5} & {y}_{5} & 1 \end{matrix}\right| = 0.
$$

这是个非退化的方程, 如果由行列式中第二、第三、第四和第五行组成矩阵的秩小于 4 , 则行列式恒等于零, 出现矛盾. 因此方程组 (3.3) 系数矩阵的秩只能等于 4 . [

## § 3.3 基础训练

## 3.3.1 训 练 题

## 一、单选题

1. 已知任一 $n$ 维向量均可由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 线性表示,则 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}\left( \;\right)$ .

(A) 线性相关 (B) 秩等于 $n$ (C) 秩小于 $n$ (D) 以上都不对

2. 设 $\mathbf{A}$ 为 $n$ 阶方阵且 $\left| \mathbf{A}\right| = 0$ ,则 ( ).

(A) $\mathbf{A}$ 中必有两行 (列) 元素对应成比例

(B) $\mathbf{A}$ 中至少有一行 (列) 元素全为零

(C) $\mathbf{A}$ 中至少有一行向量是其余各行向量的线性组合

(D) $\mathbf{A}$ 中每一行向量都是其余各行向量的线性组合

3. 一个向量组中的极大线性无关组 ( ).

(A) 个数唯一 (B) 个数不唯一

(C) 所含向量个数唯一 (D) 所含向量个数不唯一

4. 设向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}\left( {s > 1,{\mathbf{\alpha }}_{1} \neq \mathbf{0}}\right)$ 线性相关,则 $\left( \;\right)$ 由 ${\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{i - 1}$ 线性表示.

(A) 每个 ${\mathbf{\alpha }}_{i}\left( {i > 1}\right)$ 都能 (B) 每个 ${\mathbf{\alpha }}_{i}\left( {i > 1}\right)$ 都不能

(C) 有一个 ${\mathbf{\alpha }}_{i}\left( {i > 1}\right)$ 能 (D) 某一个 ${\mathbf{\alpha }}_{i}\left( {i > 1}\right)$ 不能

5. 设 $m \times n$ 矩阵 $\mathbf{A}$ 中 $n$ 个列向量线性无关,则 $\mathbf{A}$ 的秩 ( ).

(A) 大于 $m$ (B) 大于 $n$ (C) 等于 $m$ (D) 等于 $n$

6. 设矩阵 $\mathbf{A}$ 和 $\mathbf{B}$ 等价, $\mathbf{A}$ 有一个 $k$ 阶子式不等于零,则 $\mathbf{B}$ 的秩 $\left( \;\right) k$ .

(A) $<$ (B) $=$ (C) $\geq$ (D) $\leq$

7. 已知 $\mathbf{A} = \left( \begin{array}{lll} 1 & 2 & 3 \\ 2 & 4 & t \\ 3 & 6 & 9 \end{array}\right) ,\mathbf{B}$ 为三阶非零矩阵且 $\mathbf{B}\mathbf{A} = \mathbf{O}$ ,则 $\left( \;\right)$ .

(A) 当 $t = 6$ 时, $\mathbf{B}$ 的秩必为 1 (B) 当 $t = 6$ 时, $\mathbf{B}$ 的秩必为 2

(C) 当 $t \neq 6$ 时, $\mathbf{B}$ 的秩必为 1 (D) 当 $t \neq 6$ 时, $\mathbf{B}$ 的秩必为 2

8. 向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 的秩为 $r$ 的充要条件是 ( ).

(A) 向量组中不含零向量

(B) 向量组中没有两个向量的对应分量成比例

(C) 向量组中有一个向量不能由其余向量线性表示

(D) 向量组线性无关

9. $\mathbf{A}$ 是三阶方阵, ${\mathbf{A}}^{ * }$ 是其伴随, $\mathbf{A}$ 的所有二阶子式都等于零,则 $\left( \;\right)$ .

(A) $\mathrm{r}\left( \mathbf{A}\right) \leq 1,\mathrm{r}\left( {\mathbf{A}}^{ * }\right) = 0$ (B) $\mathrm{r}\left( \mathbf{A}\right) = 1,\mathrm{r}\left( {\mathbf{A}}^{ * }\right) = 0$

(C) $\mathrm{r}\left( \mathbf{A}\right) \leq 1,\mathrm{r}\left( {\mathbf{A}}^{ * }\right) = 1$ (D) $\mathrm{r}\left( \mathbf{A}\right) = 2,\mathrm{r}\left( {\mathbf{A}}^{ * }\right) = 1$

10. 要下列齐次线性方程组有非零解, 只需条件 ( ) 满足:

$$
\left\{ \begin{matrix} {a}_{11}{x}_{1} + {a}_{12}{x}_{2} + \cdots + {a}_{1n}{x}_{n} = 0, \\ \cdots \cdots \cdots \cdots \\ {a}_{m1}{x}_{1} + {a}_{m2}{x}_{2} + \cdots + {a}_{mn}{x}_{n} = 0. \end{matrix}\right.
$$

(A) $m \leq n$ (B) $m = n$ (C) $m > n$ (D) 系数矩阵的秩小于 $n$

11. 设 $\mathbf{A}$ 是 $m \times n$ 矩阵,若非齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 的解不唯一,则结论 ( ) 成立.

(A) $\mathbf{A}$ 的秩小于 $m$ (B) $m < n$ (C) $\mathbf{A}$ 是零矩阵 (D) $\mathbf{{Ax}} = \mathbf{0}$ 的解不唯一

12. 设 $\mathbf{A}$ 是 $m \times n$ 矩阵,若线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ 有非零解,则必有 ( ).

(A) $m < n$ (B) $\mathrm{r}\left( \mathbf{A}\right) < n$

(C) $\mathbf{A}$ 中有两列对应元素成比例 (D) $\mathbf{A}$ 的行向量组线性相关

13. 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 是齐次线性方程组 $\mathbf{{Ax}} = \mathbf{0}$ 的一个基础解系,则 $\left( \;\right)$ 也是该方程组的基础解系.

(A) ${\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} - {\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + 5{\mathbf{\alpha }}_{3},4{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} - 2{\mathbf{\alpha }}_{3}$

(B) ${\mathbf{\alpha }}_{1} + 2{\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3},2{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + 2{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3}$

(C) ${\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3}$

(D) ${\mathbf{\alpha }}_{1} - {\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{2} - {\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{3} - {\mathbf{\alpha }}_{1}$

14. 当 $t = \left( \;\right)$ 时,向量组 ${\mathbf{\alpha }}_{1} = \left( {2,1,0}\right) ,{\mathbf{\alpha }}_{2} = \left( {3,2,5}\right) ,{\mathbf{\alpha }}_{3} = \left( {5,4, t}\right)$ 线性相关.

(A) 5 (B) 10 (C) 15 (D) 20

15. 设 ${\mathbf{\alpha }}_{1} = \left( {1,4,1}\right) ,{\mathbf{\alpha }}_{2} = \left( {2,1, - 5}\right) ,{\mathbf{\alpha }}_{3} = \left( {6,2, - {16}}\right) ,\mathbf{\beta } = \left( {2, t,3}\right)$ ,当 $t = \left( \;\right)$ 时, $\mathbf{\beta }$ 可用 $\mathbf{\alpha },{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性表示.

(A) 1 (B) 3 (C) 6 (D) 9

## 二、慎空题

1. 设向量 ${\mathbf{\beta }}_{1} = {\mathbf{\alpha }}_{1} - {\mathbf{\alpha }}_{2},{\mathbf{\beta }}_{2} = {\mathbf{\alpha }}_{2} - {\mathbf{\alpha }}_{3},{\mathbf{\beta }}_{3} = {\mathbf{\alpha }}_{3} - {\mathbf{\alpha }}_{4},{\mathbf{\beta }}_{4} = {\mathbf{\alpha }}_{4} - {\mathbf{\alpha }}_{1}$ ,则向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3},{\mathbf{\beta }}_{4}$ 线性相关吗? ( )

2. 若向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性无关,则其中任意两个向量线性无关. 反之,若其中任意两个向量线性无关, 问该向量组是否线性无关? ( )

3. 若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性相关,则 ${\mathbf{\alpha }}_{1}$ 是否必可由 ${\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性表示? ( )

4. $n$ 维行向量集合中的任意 $n$ 个线性无关的行向量是否和向量组 ${\mathbf{e}}_{1} = \left( {1,0,\cdots ,0}\right) ,{\mathbf{e}}_{2} =$ $\left( {0,1,\cdots ,0}\right) ,\cdots ,{\mathbf{e}}_{n} = \left( {0,0,\cdots ,1}\right)$ 等价? $\left( \;\right)$

5. 设 $n$ 维列向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关, $\mathbf{A}$ 为可逆矩阵,问 $\mathbf{A}{\mathbf{\alpha }}_{1},\mathbf{A}{\mathbf{\alpha }}_{2},\cdots ,\mathbf{A}{\mathbf{\alpha }}_{m}$ 是否线性无关? ( )

6. 设向量 $\mathbf{\beta }$ 可由向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表示,但不能由其中任何一个个数少于 $m$ 的部分向量组线性表示, 问这个向量组是否线性无关? ( )

7. 设向量 $\mathbf{\beta }$ 可由向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性表示,且 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关,则 $\mathbf{\beta }$ 的表示是否唯一? ( )

8. 设向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性无关,问向量组

$$
{\mathbf{\beta }}_{1} = {\mathbf{\alpha }}_{1},{\mathbf{\beta }}_{2} = {\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\beta }}_{m} = {\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + \cdots + {\mathbf{\alpha }}_{m}
$$

是否线性无关? ( )

9. 设向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性无关,向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 可由向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 线性表示:

$$
\left\{ \begin{array}{l} {\mathbf{\beta }}_{1} = {\mathbf{\alpha }}_{1} + 4{\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3} \\ {\mathbf{\beta }}_{2} = 2{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} - {\mathbf{\alpha }}_{3} \\ {\mathbf{\beta }}_{3} = {\mathbf{\alpha }}_{1} - 3{\mathbf{\alpha }}_{3} \end{array}\right.
$$

问 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 是否线性无关? ( )

10. 若向量组 $A : {\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 中每个向量都可由它的一个部分向量组 $B : {\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ 唯一地线性表示,问向量组 $A$ 的秩是否等于 $r$ ? ( )

11. 设向量 $\mathbf{\beta }$ 可由向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表示,但不能由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r - 1}$ 线性表示, 问向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 和向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r - 1},\mathbf{\beta }$ 的秩是否相等? $\left( \;\right)$

12. 若线性方程组中方程式的个数多于未知数的个数, 此方程组是否必无解? ( )

13. 现有齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{0}$ ,其中 $\mathbf{A}$ 的秩为 $r$ ,未知数个数为 $n$ ,问: 是否任意 $n - r$ 个解向量都是它的一个基础解系? ( )

14. 非齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 的系数矩阵 $\mathbf{A}$ 是 $m \times n$ 阵,若 $\mathbf{A}$ 的行向量组线性无关,问该方程组是否一定有解? ( )

15. 设 ${\eta }_{1},{\eta }_{2},\cdots ,{\eta }_{r}$ 是非齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 的解向量,设 ${k}_{1},{k}_{2},\cdots ,{k}_{r}$ 是一组数,适合 ${k}_{1} + {k}_{2} + \cdots + {k}_{r} = 1$ ,问: ${k}_{1}{\eta }_{1} + {k}_{2}{\eta }_{2} + \cdots + {k}_{r}{\eta }_{r}$ 是否也是该方程组的解? $\left( \;\right)$

## 三、解答题

1. 设 ${\mathbf{\alpha }}_{1} = \left( {1,3,0,2}\right) ,{\mathbf{\alpha }}_{2} = \left( {-1,0,1,0}\right) ,{\mathbf{\alpha }}_{3} = \left( {5,9, - 2,6}\right)$ ,是否存在数 $\left\{ {{a}_{ij} \mid i, j = 1,2,3}\right\}$ , 使向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 线性无关? 其中

$$
{\mathbf{\beta }}_{1} = {a}_{11}{\mathbf{\alpha }}_{1} + {a}_{12}{\mathbf{\alpha }}_{2} + {a}_{13}{\mathbf{\alpha }}_{3}
$$

$$
{\mathbf{\beta }}_{2} = {a}_{21}{\mathbf{\alpha }}_{1} + {a}_{22}{\mathbf{\alpha }}_{2} + {a}_{23}{\mathbf{\alpha }}_{3}
$$

$$
{\mathbf{\beta }}_{3} = {a}_{31}{\mathbf{\alpha }}_{1} + {a}_{32}{\mathbf{\alpha }}_{2} + {a}_{33}{\mathbf{\alpha }}_{3}.
$$

2. 已知向量空间 $V$ 中 $m\left( {m > 1}\right)$ 个向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关. 求证: 可找到 $m$ 个不全为零的数 ${c}_{1},{c}_{2},\cdots ,{c}_{m}$ ,使对 $V$ 中任一向量 $\mathbf{\beta }$ ,向量组 $\mathbf{\beta },{\mathbf{\alpha }}_{1} + {c}_{1}\mathbf{\beta },\cdots ,{\mathbf{\alpha }}_{m} + {c}_{m}\mathbf{\beta }$ 都线性相关.

3. 设 $V$ 是实数域上连续函数空间, ${a}_{1},{a}_{2},\cdots ,{a}_{n}$ 是 $n$ 个不同的实数,求证: ${\mathrm{e}}^{{a}_{1}x},{\mathrm{e}}^{{a}_{2}x},\cdots$ , ${\mathrm{e}}^{{a}_{n}x}$ 线性无关.

4. 已知向量组 ${\mathbf{\alpha }}_{1} = \left( {1,2,1, - 2}\right) ,{\mathbf{\alpha }}_{2} = \left( {2,3,1,0}\right) ,{\mathbf{\alpha }}_{3} = \left( {1,2,2, - 3}\right) ,{\mathbf{\beta }}_{1} = \left( {1,1,1,1}\right) ,{\mathbf{\beta }}_{2} =$ $\left( {1,0,1, - 1}\right) ,{\mathbf{\beta }}_{3} = \left( {1,3,0, - 4}\right)$ ,设子空间 ${V}_{1} = L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}}\right) ,{V}_{2} = L\left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}}\right)$ . 求 ${V}_{1} + {V}_{2}$ 及 ${V}_{1} \cap {V}_{2}$ 的维数和基.

5. 设 $\mathbf{A}$ 是 $m \times n$ 矩阵, $\mathbf{B}$ 是 $m \times k$ 矩阵且 $\mathbf{A} = \left( {{\mathbf{\alpha }}_{1},\cdots ,{\mathbf{\alpha }}_{n}}\right) ,\mathbf{B} = \left( {{\mathbf{\beta }}_{1},\cdots ,{\mathbf{\beta }}_{k}}\right)$ 是它们的列向量分块. 假定对每个 ${\mathbf{\beta }}_{j}$ ,分块矩阵 $\left( {\mathbf{A}!{\mathbf{\beta }}_{j}}\right)$ 的秩都与 $\mathbf{A}$ 的秩相等,求证: 分块矩阵 $\left( {\mathbf{A}!\mathbf{B}}\right)$ 的秩等于 $\mathbf{A}$ 的秩.

6. 设 $\mathbf{A},\mathbf{B}$ 都是 $n$ 阶矩阵,求证: $\mathrm{r}\left( {\mathbf{A}\mathbf{B} - {\mathbf{I}}_{n}}\right) \leq \mathrm{r}\left( {\mathbf{A} - {\mathbf{I}}_{n}}\right) + \mathrm{r}\left( {\mathbf{B} - {\mathbf{I}}_{n}}\right)$ .

7. 已知矩阵 ${\mathbf{B}}_{i}\left( {i = 1,\cdots, k}\right)$ 是 $n$ 阶幂等矩阵,即 ${\mathbf{B}}_{i}^{2} = {\mathbf{B}}_{i}$ ,又 $\mathbf{A} = {\mathbf{B}}_{1}\cdots {\mathbf{B}}_{k}$ ,求证:

$$
\mathrm{r}\left( {{\mathbf{I}}_{n} - \mathbf{A}}\right) \leq k\left( {n - \mathrm{r}\left( \mathbf{A}\right) }\right) .
$$

8. 设 $n$ 阶实方阵 $\mathbf{A}$ 满足 $\mathbf{A}{\mathbf{A}}^{\prime } = {a}^{2}{\mathbf{I}}_{n}$ ,其中 $a$ 为实数,证明:

$$
\mathrm{r}\left( {a{\mathbf{I}}_{n} - \mathbf{A}}\right) = \mathrm{r}\left( {\left( a{\mathbf{I}}_{n} - \mathbf{A}\right) }^{2}\right) .
$$

9. 设 $n$ 阶方阵 $\mathbf{A},\mathbf{B}$ 满足: ${\left( \mathbf{A} + \mathbf{B}\right) }^{2} = \mathbf{A} + \mathbf{B},\mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right)$ ,证明:

$$
{A}^{2} = A,{B}^{2} = B,{AB} = {BA} = O.
$$

10. 设 $\mathbf{A}$ 是一个对称矩阵, $\mathbf{A}$ 有一个 $r$ 阶主子式 $\left| \mathbf{M}\right|$ 不等于零且 $\mathbf{A}$ 所有包含 $\left| \mathbf{M}\right|$ 的 $r + 1$ 及 $r + 2$ 阶加边主子式都等于零,求证: $\mathbf{A}$ 的秩等于 $r$ .

11. 设 $\mathbf{A}$ 是一个反对称矩阵, $\mathbf{A}$ 有一个 $r$ 阶主子式 $\left| \mathbf{M}\right|$ 不等于零且 $\mathbf{A}$ 所有包含 $\left| \mathbf{M}\right|$ 的 $r + 2$ 阶加边主子式都等于零,求证: $\mathbf{A}$ 的秩等于 $r$ .

12. 求解下列线性方程组,其中 $k$ 为参数:

$$
\left\{ \begin{array}{l} k{x}_{1} + {x}_{2} + {x}_{3} = - 2, \\ {x}_{1} + k{x}_{2} + {x}_{3} = - 2, \\ {x}_{1} + {x}_{2} + k{x}_{3} = - 2. \end{array}\right.
$$

13. 已知非齐次线性方程组 ${Ax} = \beta$ 的相伴齐次线性方程组 ${Ax} = 0$ 的基础解系为 $\left\{ {{\eta }_{1},\cdots ,{\eta }_{n - r}}\right\} ,{Ax} = \beta$ 的特解为 $\gamma$ ,求证: $\gamma ,\gamma + {\eta }_{1},\cdots ,\gamma + {\eta }_{n - r}$ 线性无关.

14. 已知非齐次线性方程组 $\mathbf{A}\mathbf{x} = \mathbf{\beta }$ 有解. 求证: 每个解向量中第 $k$ 个分量都等于零的充分必要条件是将增广矩阵 $\widetilde{\mathbf{A}}$ 的第 $k$ 列划去后得到的矩阵的秩比 $\widetilde{\mathbf{A}}$ 的秩小.

15. 设在实平面上有 3 条不同的直线:

$$
{L}_{1} : \;{ax} + {by} + c = 0,
$$

$$
{L}_{2} : {bx} + {cy} + a = 0,
$$

$$
{L}_{3} : \;{cx} + {ay} + b = 0,
$$

求证: 它们相交于一点的充要条件是 $a + b + c = 0$ .

## 3.3.2 训练题答案

## 一、单选题

1. 选择 (B).

2. 选择 (C). 当 $\left| \mathbf{A}\right| = 0$ 时,矩阵 $\mathbf{A}$ 的秩小于 $n$ ,因此行向量线性相关,于是至少有一个行向量是其余各行向量的线性组合.

3. 向量组的极大无关组含有相同的向量个数, 因此选择 (C).

4. 选择 (C).

5. 选择 (D).

6. 由矩阵秩的子式判定法可知, 选择 (C).

7. 当 $t = 6$ 时, $\mathbf{A}$ 的秩等于 1,于是 $\mathbf{B}$ 的秩可能是 1 或 2,故不应该选择 (A) 与 (B). 当 $t \neq 6$ 时, $\mathbf{A}$ 的秩等于 $2,\mathbf{B}$ 的秩不可能为 2 (因为方程组 ${\mathbf{A}}^{\prime }\mathbf{x} = \mathbf{0}$ 的基础解系只含一个向量). 故正确的选择是 (C).

8. 选择 (D).

9. 当 $\mathbf{A}$ 的二阶子式全为零时, $\mathbf{A}$ 的任意一个代数余子式都等于零,故 ${\mathbf{A}}^{ * } = \mathbf{O}$ . 这时 $\mathbf{A}$ 有可能是零矩阵, 因此选择 (A).

10. 根据线性方程组有解的判定定理可知, 选择 (D).

11. 由非齐次线性方程组的解与其相伴齐次方程组的解的关系可知, 正确的选择是 (D).

12. 选择 (B).

13. (C) 中只有两个向量, 不可能成为方程组的基础解系, 另外只有 (A) 中向量线性无关, 因此正确的选择是 (A).

14. 当 $t = {15}$ 时,向量组的秩小于 3,因此,应该选择 (C).

15. 要使 $\mathbf{\beta }$ 能表示为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 的线性组合,当且仅当向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},\mathbf{\beta }$ 的秩等于向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 的秩. 经计算可知 $t = 9$ ,因此选择 (D).

## 二、填空题

1. 因为 ${\mathbf{\beta }}_{1} + {\mathbf{\beta }}_{2} + {\mathbf{\beta }}_{3} + {\mathbf{\beta }}_{4} = \mathbf{0}$ ,向量组线性相关.

2. 不一定. 如 3 个二维行向量 $\left( {1,0}\right) ,\left( {0,1}\right) ,\left( {1,1}\right)$ 两两线性无关,但这 3 个向量线性相关.

3. 不一定. 如 $\left( {1,0}\right) ,\left( {0,0}\right) ,\left( {0,1}\right)$ .

4. 等价. $n$ 维向量空间中任意 $n$ 个线性无关的向量均可成为一组基,因此它们互相等价.

5. 线性无关. 参考例 3.10.

6. 线性无关. 假定向量组线性相关,则必有某个 ${\mathbf{\alpha }}_{i}$ 可以用组内其他向量线性表示,于是 $\mathbf{\beta }$ 也可用这些向量线性表示, 矛盾.

7. 不唯一. 参考 $§{3.1.2}$ 定理 3 (3).

8. 线性无关. 参考例 3.14 计算行列式, 或参考例 3.17 计算矩阵的秩, 或直接根据线性无关的定义验证即可.

9. 矩阵 $\left( \begin{matrix} 1 & 4 & 1 \\ 2 & 1 & - 1 \\ 1 & 0 & - 3 \end{matrix}\right)$ 的秩等于 3,故 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 线性无关.

10. 等于 $r$ . 因为这时表示唯一,故 ${\mathbf{\alpha }}_{{i}_{1}},{\mathbf{\alpha }}_{{i}_{2}},\cdots ,{\mathbf{\alpha }}_{{i}_{r}}$ . 线性无关 (参考 $§{3.1.2}$ 定理 3 (3)). 于是这 $r$ 个向量是原向量组的极大无关组.

11. 相等. 参考例 3.21.

12. 不一定.

13. 不一定. 只有当这 $n - r$ 个解向量线性无关时才构成基础解系.

14. 有解. 因为这时 $\mathbf{A}$ 的秩为 $m$ ,而其增广矩阵是 $m \times \left( {n + 1}\right)$ 矩阵,秩只能为 $m$ .

15. 将向量代入即知是解.

## 三、解答题

1. 不存在. 因为通过计算可知,向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 的秩小于 3,故表出向量组的秩也小于 3 (参见例题 3.18 的注).

2. 已知 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{m}$ 线性相关,故存在不全为零的数 ${k}_{1},{k}_{2},\cdots ,{k}_{m}$ ,使 ${k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots +$ ${k}_{m}{\mathbf{\alpha }}_{m} = \mathbf{0}$ . 因为 $m > 1$ 且 ${k}_{i}$ 不全为零,必存在数 ${c}_{1},{c}_{2},\cdots ,{c}_{m}$ ,使 ${k}_{1}{c}_{1} + {k}_{2}{c}_{2} + \cdots + {k}_{m}{c}_{m} = - 1$ . 于是对任意的 $\mathbf{\beta },\mathbf{\beta } + {k}_{1}\left( {{\mathbf{\alpha }}_{1} + {c}_{1}\mathbf{\beta }}\right) + {k}_{2}\left( {{\mathbf{\alpha }}_{2} + {c}_{2}\mathbf{\beta }}\right) + \cdots + {k}_{m}\left( {{\mathbf{\alpha }}_{m} + {c}_{m}\mathbf{\beta }}\right) = \mathbf{0}$ .

3. 设 ${k}_{1},{k}_{2},\cdots ,{k}_{n}$ 为 $n$ 个实数,使得 ${k}_{1}{\mathrm{e}}^{{a}_{1}x} + {k}_{2}{\mathrm{e}}^{{a}_{2}x} + \cdots + {k}_{n}{\mathrm{e}}^{{a}_{n}x} = 0$ . 对上式求导 $i$ 次并令 $x = 0$ ,可得 ${a}_{1}^{i}{k}_{1} + {a}_{2}^{i}{k}_{2} + \cdots + {a}_{n}^{i}{k}_{n} = 0\left( {i = 0,1,\cdots, n}\right)$ . 上述 $n$ 个方程构成了关于 ${k}_{1},{k}_{2},\cdots ,{k}_{n}$ 的线性方程组,其系数行列式是关于 ${a}_{1},{a}_{2},\cdots ,{a}_{n}$ 的 Vander Monde 行列式. 由于 ${a}_{1},{a}_{2},\cdots ,{a}_{n}$ 互不相同,故系数行列式不等于零,从而方程组只有零解 ${k}_{1} = {k}_{2} = \cdots = {k}_{n} = 0$ , 于是 ${\mathrm{e}}^{{a}_{1}x},{\mathrm{e}}^{{a}_{2}x},\cdots ,{\mathrm{e}}^{{a}_{n}x}$ 线性无关.

4. ${V}_{1} + {V}_{2} = L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}}\right)$ . 只需求出 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 的一个极大无关组就是 ${V}_{1} + {V}_{2}$ 的基,经计算求得为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\beta }}_{2}$ (答案不唯一),故 ${V}_{1} + {V}_{2}$ 的维数等于 4 (全空间). 又经计算可得 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 的秩为 $3,{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 的秩也为 3,故 ${V}_{1},{V}_{2}$ 的维数都是 3,因此由维数公式得 ${V}_{1} \cap {V}_{2}$ 的维数为 2. 求 ${V}_{1} \cap {V}_{2}$ 的基需要求下列齐次线性方程组的基础解系: ${x}_{1}{\alpha }_{1} + {x}_{2}{\alpha }_{2} + {x}_{3}{\alpha }_{3} + {x}_{4}{\beta }_{1} + {x}_{5}{\beta }_{2} + {x}_{6}{\beta }_{3} = 0$ (参考例 3.47 的解法 2). 经计算可知, ${\beta }_{1},{\beta }_{3}$ 就是 ${V}_{1} \cap {V}_{2}$ 的基 (答案不唯一).

5. 由 $\mathrm{r}\left( {\mathbf{A};{\mathbf{\beta }}_{j}}\right) = \mathrm{r}\left( \mathbf{A}\right)$ 可知,每个 ${\mathbf{\beta }}_{j}$ 都可以用 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 线性表示,因此 $\left( {\mathbf{A};\mathbf{B}}\right)$ 的秩不超过 $\mathbf{A}$ 的秩,从而等于 $\mathbf{A}$ 的秩.

6. 注意到 $\mathbf{A}\mathbf{B} - {\mathbf{I}}_{n} = \left( {\mathbf{A} - {\mathbf{I}}_{n}}\right) \mathbf{B} + \left( {\mathbf{B} - {\mathbf{I}}_{n}}\right)$ ,故 $\mathrm{r}\left( {\mathbf{A}\mathbf{B} - {\mathbf{I}}_{n}}\right) \leq \mathrm{r}\left( {\left( {\mathbf{A} - {\mathbf{I}}_{n}}\right) \mathbf{B}}\right) + \mathrm{r}\left( {\mathbf{B} - {\mathbf{I}}_{n}}\right) \leq$ $\mathrm{r}\left( {\mathbf{A} - {\mathbf{I}}_{n}}\right) + \mathrm{r}\left( {\mathbf{B} - {\mathbf{I}}_{n}}\right) .$

7. 由 $\mathbf{A} = {\mathbf{B}}_{1}\cdots {\mathbf{B}}_{k}$ 可得 $\mathrm{r}\left( \mathbf{A}\right) \leq \mathrm{r}\left( {\mathbf{B}}_{i}\right)$ . 因为 ${\mathbf{B}}_{i}$ 是幂等矩阵,故由例 3.67 可得 $\mathrm{r}\left( {{\mathbf{I}}_{n} - }\right.$ $\left. {\mathbf{B}}_{i}\right) = n - \mathrm{r}\left( {\mathbf{B}}_{i}\right)$ . 注意到 ${\mathbf{I}}_{n} - \mathbf{A} = \left( {{\mathbf{I}}_{n} - {\mathbf{B}}_{1}}\right) + {\mathbf{B}}_{1}\left( {{\mathbf{I}}_{n} - {\mathbf{B}}_{2}}\right) + \cdots + {\mathbf{B}}_{1}\cdots {\mathbf{B}}_{k - 1}\left( {{\mathbf{I}}_{n} - {\mathbf{B}}_{k}}\right)$ , 故 $\mathrm{r}\left( {{\mathbf{I}}_{n} - \mathbf{A}}\right) \leq \mathop{\sum }\limits_{{i = 1}}^{k}\mathrm{r}\left( {{\mathbf{I}}_{n} - {\mathbf{B}}_{i}}\right) = \mathop{\sum }\limits_{{i = 1}}^{k}\left( {n - \mathrm{r}\left( {\mathbf{B}}_{i}\right) }\right) \leq k\left( {n - \mathrm{r}\left( \mathbf{A}\right) }\right)$ .

8. 若 $a = 0$ ,则 $A{A}^{\prime } = O$ ,由例 2.42 可知 $A = O$ ,从而结论显然成立. 若 $a \neq 0$ ,注意到 ${\left( a{I}_{n} - A\right) }^{2} = \left( {\frac{1}{a}A{A}^{\prime } - A}\right) \left( {a{I}_{n} - A}\right) = - \frac{1}{a}A\left( {a{I}_{n} - {A}^{\prime }}\right) \left( {a{I}_{n} - A}\right) = - \frac{1}{a}A{\left( a{I}_{n} - A\right) }^{\prime }\left( {a{I}_{n} - A}\right)$ , 则由例 3.72 以及 $- \frac{1}{a}\mathbf{A}$ 的非异性可得 $\mathrm{r}\left( {\left( a{\mathbf{I}}_{n} - \mathbf{A}\right) }^{2}\right) = \mathrm{r}\left( {{\left( a{\mathbf{I}}_{n} - \mathbf{A}\right) }^{\prime }\left( {a{\mathbf{I}}_{n} - \mathbf{A}}\right) }\right) = \mathrm{r}\left( {a{\mathbf{I}}_{n} - \mathbf{A}}\right)$ .

9. 由例 3.67 可得 $n = \mathrm{r}\left( {\mathbf{A} + \mathbf{B}}\right) + \mathrm{r}\left( {{\mathbf{I}}_{n} - \mathbf{A} - \mathbf{B}}\right) = \mathrm{r}\left( \mathbf{A}\right) + \mathrm{r}\left( \mathbf{B}\right) + \mathrm{r}\left( {{\mathbf{I}}_{n} - \mathbf{A} - \mathbf{B}}\right)$ . 构造如下分块对角阵, 并对其实施分块初等变换, 可得

$$
\left( \begin{matrix} A & O & O \\ O & B & O \\ O & O & {I}_{n} - A - B \end{matrix}\right) \rightarrow \left( \begin{matrix} A & O & O \\ O & B & O \\ A & B & {I}_{n} - A - B \end{matrix}\right) \rightarrow \left( \begin{matrix} A & O & A \\ O & B & B \\ A & B & {I}_{n} \end{matrix}\right) \rightarrow
$$

$$
\left( \begin{matrix} A - {A}^{2} & - {AB} & O \\ - {BA} & B - {B}^{2} & O \\ A & B & {I}_{n} \end{matrix}\right) \rightarrow \left( \begin{matrix} A - {A}^{2} & - {AB} & O \\ - {BA} & B - {B}^{2} & O \\ O & O & {I}_{n} \end{matrix}\right) .
$$

注意到分块初等变换不改变矩阵的秩,故可得 $\mathrm{r}\left( \begin{matrix} A - {A}^{2} & - {AB} \\ - {BA} & B - {B}^{2} \end{matrix}\right) = 0$ ,从而 ${A}^{2} = A$ , ${B}^{2} = B,{AB} = {BA} = O.$

10. 对一个对称矩阵进行一次行对换, 再进行一次对称的列对换后得到的矩阵仍是对称矩阵. 因此不妨设 $\mathbf{M}$ 在 $\mathbf{A}$ 的左上角. 现考虑任意一个包含 $\mathbf{M}$ 的 $r + 2$ 阶主子阵 $\left( \begin{matrix} \mathbf{M} & \mathbf{\alpha } & \mathbf{\beta } \\ {\mathbf{\alpha }}^{\prime } & {a}_{ss} & {a}_{st} \\ {\mathbf{\beta }}^{\prime } & {a}_{ts} & {a}_{tt} \end{matrix}\right)$ , 注意由对称性 ${a}_{st} = {a}_{ts}$ . 因为 $\left| \mathbf{M}\right| \neq 0,\mathbf{M}$ 是可逆矩阵. 对上述矩阵作分块初等行变换分别消去 ${\alpha }^{\prime }$ 及 ${\beta }^{\prime }$ ,得:

$$
\left( \begin{matrix} M & \alpha & \beta \\ 0 & {a}_{ss} - {\alpha }^{\prime }{M}^{-1}\alpha & {a}_{st} - {\alpha }^{\prime }{M}^{-1}\beta \\ 0 & {a}_{ts} - {\beta }^{\prime }{M}^{-1}\alpha & {a}_{tt} - {\beta }^{\prime }{M}^{-1}\beta \end{matrix}\right)
$$

因为 $\left| \begin{matrix} \mathbf{M} & \mathbf{\alpha } \\ {\mathbf{\alpha }}^{\prime } & {a}_{ss} \end{matrix}\right| = 0$ ,有 ${a}_{ss} - {\mathbf{\alpha }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\alpha } = 0$ . 同理 ${a}_{tt} - {\mathbf{\beta }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\beta } = 0$ . 又, ${a}_{ts} - {\mathbf{\beta }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\alpha }$ 是一个数,把它看成 $1 \times 1$ 矩阵,转置后有 ${a}_{ts} - {\mathbf{\beta }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\alpha } = {a}_{st} - {\mathbf{\alpha }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\beta }$ . 再由已知,上述 $r + 2$ 阶子式等于零, 得

$$
\left| \begin{matrix} \mathbf{M} & \mathbf{\alpha } & \mathbf{\beta } \\ 0 & {a}_{ss} - {\mathbf{\alpha }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\alpha } & {a}_{st} - {\mathbf{\alpha }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\beta } \\ 0 & {a}_{ts} - {\mathbf{\beta }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\alpha } & {a}_{tt} - {\mathbf{\beta }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\beta } \end{matrix}\right| = 0,
$$

即有 ${a}_{ts} - {\mathbf{\beta }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\alpha } = {a}_{st} - {\mathbf{\alpha }}^{\prime }{\mathbf{M}}^{-1}\mathbf{\beta } = 0$ . 对任意的 $r$ 维向量 $\mathbf{\alpha },\mathbf{\beta }$ ,都有上式成立. 因此,若在 $\mathbf{A}$ 中用上述方法消去 ${\mathbf{\alpha }}^{\prime }$ 时,后面的项全部消去. 于是可消去除前 $r$ 行外的所有行. 这就证明了 $\mathbf{A}$ 的秩等于 $r$ .

11. 注意反对称矩阵的奇数阶主子式总等于零, 其余同上题证明.

12. 当 $k = - 2$ 时,方程组无解; 当 $k = 1$ 时,方程组的通解为 ${\left( -2,0,0\right) }^{\prime } + {c}_{1}{\left( -1,1,0\right) }^{\prime } +$ ${c}_{2}{\left( -1,0,1\right) }^{\prime }$ ,其中 ${c}_{1},{c}_{2}$ 为任意数; 当 $k \neq - 2,1$ 时,方程组有唯一解 ${\left( -\frac{2}{k + 2}, - \frac{2}{k + 2}, - \frac{2}{k + 2}\right) }^{\prime }$ .

13. 假定 ${a}_{0}\gamma + {a}_{1}\left( {\gamma + {\eta }_{1}}\right) + \cdots + {a}_{n - r}\left( {\gamma + {\eta }_{n - r}}\right) = \mathbf{0}$ ,得 $\left( {{a}_{0} + {a}_{1} + \cdots + {a}_{n - r}}\right) \gamma + {a}_{1}{\eta }_{1} +$ $\cdots + {a}_{n - r}{\mathbf{\eta }}_{n - r} = \mathbf{0}$ . 两边作用 $\mathbf{A}$ 得 $\left( {{a}_{0} + {a}_{1} + \cdots + {a}_{n - r}}\right) \mathbf{\beta } = \mathbf{0}$ ,故 ${a}_{0} + {a}_{1} + \cdots + {a}_{n - r} = 0$ . 于是 ${a}_{1}{\mathbf{\eta }}_{1} + \cdots + {a}_{n - r}{\mathbf{\eta }}_{n - r} = \mathbf{0}$ ,由于 ${\mathbf{\eta }}_{1},\cdots ,{\mathbf{\eta }}_{n - r}$ 是基础解系,故 ${a}_{i} = 0$ .

14. 不失一般性,令 $k = 1$ . 又假定 $\mathbf{A} = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right)$ 是其列向量分块. 将方程组写为 ${x}_{1}{\mathbf{\alpha }}_{1} + {x}_{2}{\mathbf{\alpha }}_{2} + \cdots + {x}_{n}{\mathbf{\alpha }}_{n} = \mathbf{\beta }$ . 若解向量中第一个分量总是零,则 $\mathbf{\beta } = {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{n}{\mathbf{\alpha }}_{n}$ , 其中 ${\left( 0,{c}_{2},\cdots ,{c}_{n}\right) }^{\prime }$ 是某个解向量. 于是 $\mathrm{r}\left( {{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) = \mathrm{r}\left( {{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n},\mathbf{\beta }}\right)$ . 假定 ${\mathbf{\alpha }}_{1} = {a}_{2}{\mathbf{\alpha }}_{2} +$ $\cdots + {a}_{n}{\mathbf{\alpha }}_{n}$ ,则 $\left( {-1}\right) {\mathbf{\alpha }}_{1} + \left( {{a}_{2} + {c}_{2}}\right) {\mathbf{\alpha }}_{2} + \cdots + \left( {{a}_{n} + {c}_{n}}\right) {\mathbf{\alpha }}_{n} = \mathbf{\beta }$ ,即 ${\left( -1,{a}_{2} + {c}_{2},\cdots ,{a}_{n} + {c}_{n}\right) }^{\prime }$ 也将是解,和解的第一个分量都是零矛盾. 因此 ${\alpha }_{1}$ 不能表示为其余 ${\alpha }_{i}$ 的线性组合. 注意到 $\beta$ 可表示为 ${\alpha }_{i}$ 的线性组合,因此 $\widetilde{\mathbf{A}}$ 第一列划去后得到的矩阵的秩比 $\widetilde{\mathbf{A}}$ 的秩小. 反过来,若某个解向量中第一分量不等于零,不妨假定有 ${c}_{1}{\mathbf{\alpha }}_{1} + {c}_{2}{\mathbf{\alpha }}_{2} + \cdots + {c}_{n}{\mathbf{\alpha }}_{n} = \mathbf{\beta },{c}_{1} \neq 0$ ,则 ${\mathbf{\alpha }}_{1}$ 可以表示为 ${\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n},\mathbf{\beta }$ 的线性组合. 因此 $\widetilde{\mathbf{A}}$ 划去第一列后的秩与 $\widetilde{\mathbf{A}}$ 的秩相同.

15. 3 条直线相交于一点的充要条件是方程组有唯一解,即 $\mathrm{r}\left( \begin{array}{ll} a & b \\ b & c \\ c & a \end{array}\right) = \mathrm{r}\left( \begin{array}{lll} a & b & c \\ b & c & a \\ c & a & b \end{array}\right) = 2$ .

3 条直线不同表明 $\mathrm{r}\left( \begin{array}{lll} a & b & c \\ b & c & a \end{array}\right) = 2$ ,故上述充要条件等价于矩阵 $\mathbf{A} = \left( \begin{array}{lll} a & b & c \\ b & c & a \\ c & a & b \end{array}\right)$ 的秩等于 2, 这也等价于 $\left| \mathbf{A}\right| = 0$ . 注意到 $\left| \mathbf{A}\right| = \left( {a + b + c}\right) \left( {{ab} + {bc} + {ca} - {a}^{2} - {b}^{2} - {c}^{2}}\right)$ ,并且由于 $a, b, c$ 不全相等,故 ${ab} + {bc} + {ca} - {a}^{2} - {b}^{2} - {c}^{2} = - \frac{1}{2}\left( {{\left( a - b\right) }^{2} + {\left( b - c\right) }^{2} + {\left( c - a\right) }^{2}}\right) < 0$ ,于是 $\left| \mathbf{A}\right| = 0$ 当且仅当 $a + b + c = 0$ .