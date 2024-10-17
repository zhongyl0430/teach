---
title: 7 线性空间与线性变换
---
在前面的章节中,我们已经学习了任意一个数域 $F$ 上 $n$ 维向量空间 ${F}^{n}$ 及其性质,特别涉及 ${\mathbb{R}}^{n}$ 和 ${\mathbb{C}}^{n}$ . 在本章中,我们将此推广到更一般的情形,介绍抽象线性空间的定义和简单的性质, 并讨论联系线性空间之间关系的映射: 线性变换及其矩阵表示.

## §7.1 线性空间与线性子空间

## 1. 线性空间的定义

线性空间的定义和基本性质比较抽象, 初学者可能会不同程度地感到困难, 建议读者积极思考, 反复地考察各种例子, 并把抽象的理论和具体的例子相对照, 克服这些困难.

线性空间总定义在一个数域上. 第二章已给出了数域的定义, 这里总是假设 $F$ 是一个数域.

第四章已经定义了数域 $F$ 上的 $n$ 维向量空间 ${F}^{n}$ . 我们先回顾一下这个概念.

设 $\mathbf{\alpha } = \left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right) \in {F}^{n},\mathbf{\beta } = \left( {{b}_{1},{b}_{2},\cdots ,{b}_{n}}\right) \in {F}^{n}$ . 定义加法:

$$
\mathbf{\alpha } + \mathbf{\beta } = \left( {{a}_{1} + {b}_{1},{a}_{2} + {b}_{2},\cdots ,{a}_{n} + {b}_{n}}\right) .
$$

显然, $\mathbf{\alpha } + \mathbf{\beta } \in {F}^{n}$ . 对于任意 $k \in F$ ,定义数乘:

$$
k\mathbf{\alpha } = \left( {k{a}_{1}, k{a}_{2},\cdots , k{a}_{n}}\right)
$$

显然, $k\mathbf{\alpha } \in {F}^{n}$ . 因此, ${F}^{n}$ 对向量的加法和数乘运算是封闭的,并且满足以下 8 条基本运算规律:

(1) $\alpha + \beta = \beta + \alpha$ ;

(2) $\left( {\mathbf{\alpha } + \mathbf{\beta }}\right) + \mathbf{\gamma } = \mathbf{\alpha } + \left( {\mathbf{\beta } + \mathbf{\gamma }}\right)$ ;

(3) $\alpha + 0 = \alpha$ ;

(4) $\mathbf{\alpha } + \left( {-\mathbf{\alpha }}\right) = \mathbf{0}$ ;

(5) ${1\alpha } = \alpha$ ;

(6) $k\left( {\ell \mathbf{\alpha }}\right) = \left( {k\ell }\right) \mathbf{\alpha }$ ,

(7) $k\left( {\mathbf{\alpha } + \mathbf{\beta }}\right) = k\mathbf{\alpha } + k\mathbf{\beta }$ ;

(8) $\left( {k + \ell }\right) \alpha = {k\alpha } + \ell \alpha$

这里 $\mathbf{\alpha },\mathbf{\beta },\mathbf{\gamma } \in {F}^{n}, k,\ell \in F$ .

第三章讨论过平面上的向量和空间中的向量. 对于空间中以一个固定点 $O$ 为起点的全体向量, 我们有向量的加法 (平行四边形法则) 和数乘, 这两种运算也满足上述 8 条规律. 只是在那里参与数乘运算的数 $k$ 是实数. 若在平面上或空间内以固定点 $O$ 为原点建立直角坐标系,则每个从原点出发的向量就可以用它的终点坐标 $\left( {{a}_{1},{a}_{2}}\right)$ 或 $\left( {{a}_{1},{a}_{2},{a}_{3}}\right)$ 来表示,其中 ${a}_{i}$ 也均为实数. 此时向量 $\left( {{a}_{1},{a}_{2}}\right)$ 与 $\left( {{b}_{1},{b}_{2}}\right)$ 之和正好是 $\left( {{a}_{1} + {b}_{1},{a}_{2} + {b}_{2}}\right) ,\left( {{a}_{1},{a}_{2},{a}_{3}}\right)$ 与 $\left( {{b}_{1},{b}_{2},{b}_{3}}\right)$ 之和正好是 $\left( {{a}_{1} + {b}_{1},{a}_{2} + {b}_{2},{a}_{3} + {b}_{3}}\right)$ ,而实数 $k$ 与向量的数乘为 $\left( {k{a}_{1}, k{a}_{2}}\right)$ 或 $\left( {k{a}_{1}, k{a}_{2}, k{a}_{3}}\right)$ . 这样一来,可将平面上 (从原点出发的) 全体向量组成的集合看成实数域 $\mathbb{R}$ 上的二维向量空间 ${\mathbb{R}}^{2}$ ,将空间中的全体向量组成的集合看成三维向量空间 ${\mathbb{R}}^{3}$ . 于是我们前面定义过的 $F$ 上的向量空间 ${F}^{n}$ 只不过是 ${\mathbb{R}}^{2},{\mathbb{R}}^{3}$ 的推广而已: 分量个数从 2,3 推广到 $n$ ,数域从 $\mathbb{R}$ 推广到一般的 $F$ . 这也就说明了我们把 ${F}^{n}$ 中的元素称为向量的原因.

除去 ${F}^{n}$ 及平面上和空间中的向量以外,在其他的一些集合上也可以定义加法和数乘.

例题 1.1. 用 $F\left\lbrack {0,1}\right\rbrack$ 表示闭区间 $\left\lbrack {0,1}\right\rbrack$ 上的全体实函数构成的集合. 若 $f\left( x\right)$ , $g\left( x\right) \in F\left\lbrack {0,1}\right\rbrack$ ,把函数 $h\left( x\right)$ 称为 $f\left( x\right) , g\left( x\right)$ 的和,即

$$
h\left( x\right) = f\left( x\right) + g\left( x\right)
$$

若 $c$ 是实数,规定 $\ell \left( x\right) = {cf}\left( x\right)$ 为 $c$ 与 $f\left( x\right)$ 的数乘. 那么上述 8 条基本运算规律也成立.

例题 1.2. 用 ${\mathbb{R}}^{\infty }$ 表示无限实数序列 $\left( {a}_{n}\right) = \left( {{a}_{1},{a}_{2},\cdots }\right)$ 的全体. 规定加法

$$
\left( {a}_{n}\right) + \left( {b}_{n}\right) = \left( {{a}_{n} + {b}_{n}}\right)
$$

和数乘

$$
k\left( {a}_{n}\right) = \left( {k{a}_{n}}\right) .
$$

那么 8 条基本运算规律也成立.

我们把 ${F}^{n}$ ,例题 1.1 中的 $F\left\lbrack {0,1}\right\rbrack$ 和例题 1.2 中的 ${\mathbb{R}}^{\infty }$ 等抽象成如下的概念.

定义 1.1. 设 $F$ 为一个数域, $V$ 为一个非空集合. 设在 $V$ 中定义了加法和数乘两种运算 (即对 $V$ 中任意的排好次序的两个元素 $\mathbf{\alpha },\mathbf{\beta }$ ,有 $V$ 中唯一的一个元素 $\gamma$ 与之对应, $\gamma$ 称为 $\mathbf{\alpha },\mathbf{\beta }$ 之和,记为 $\gamma = \mathbf{\alpha } + \mathbf{\beta }$ ; 同时对数域 $F$ 中任意数 $k$ 与 $V$ 中任意元素 $\mathbf{\alpha }$ ,有 $V$ 中唯一的元素 $\mathbf{\delta }$ 与之对应, $\mathbf{\delta }$ 称为 $k$ 与 $\mathbf{\alpha }$ 的数乘,记为 $\delta = {k\alpha }$ ),并且满足以下八个条件:

(1) 加法交换律: 对一切 $\mathbf{\alpha },\mathbf{\beta } \in V,\mathbf{\alpha } + \mathbf{\beta } = \mathbf{\beta } + \mathbf{\alpha }$ ;

(2) 加法结合律: 对一切 $\mathbf{\alpha },\mathbf{\beta },\mathbf{\gamma } \in V,\left( {\mathbf{\alpha } + \mathbf{\beta }}\right) + \mathbf{\gamma } = \mathbf{\alpha } + \left( {\mathbf{\beta } + \mathbf{\gamma }}\right)$ ;

(3) 在 $V$ 中有一个向量 0,它对每个 $\mathbf{\alpha } \in V$ 均有 $\mathbf{\alpha } + \mathbf{0} = \mathbf{\alpha }$ ;

(4) 若 $\mathbf{\alpha } \in V$ ,则存在 $\mathbf{\beta } \in V$ ,使 $\mathbf{\alpha } + \mathbf{\beta } = \mathbf{0}$ ;

(5) 数域 $F$ 中元素 1 与每个 $\alpha \in V$ 的数乘都是 $\alpha$ 本身: ${1\alpha } = \alpha$ ;

(6) 若 $k,\ell \in F$ ,而 $\mathbf{\alpha } \in V$ ,则 $k\left( {\ell \mathbf{\alpha }}\right) = \left( {k\ell }\right) \mathbf{\alpha }$ ;

(7) 若 $k,\ell \in F$ ,而 $\mathbf{\alpha } \in V$ ,则 $\left( {k + \ell }\right) \mathbf{\alpha } = k\mathbf{\alpha } + \ell \mathbf{\alpha }$ ;

(8) 若 $k \in F$ ,而 $\mathbf{\alpha },\mathbf{\beta } \in V$ ,则 $k\left( {\mathbf{\alpha } + \mathbf{\beta }}\right) = k\mathbf{\alpha } + k\mathbf{\beta }$ ,

则 $V$ 称为 $F$ 上的线性空间, $V$ 中元素称为向量,(3) 中的 0 称为零向量,而 (4) 中的 $\beta$ 称为 $\alpha$ 的负向量.

今后总用大写拉丁文字母如 $U, V,\cdots$ 表示线性空间,用小写希腊字母如 $\mathbf{\alpha }$ , $\beta ,\cdots$ 表示向量.

这个定义高度抽象,定义未具体规定 $V$ 由何种元素组成,也未规定 $V$ 中的两种运算如何进行, 定义要求的只是运算满足规律 (1)-(8). 这种抽象性使我们可以把不同的数学对象统一到线性空间这一概念之下. 读者不难验证, 按上边的定义,向量空间 ${F}^{n}$ 、例题 1.1 中的 $F\left\lbrack {0,1}\right\rbrack$ 、例题 1.2 中的 ${\mathbb{R}}^{\infty }$ 都是线性空间. 由定义可知,线性空间的概念涉及四个要素: 数域 $F$ ,非空集合 $V$ ,加法和数乘. 所以如果要具体给出一个线性空间,必须指明数域 $F$ ,指明 $V$ 由何种数学对象组成, 并说明两种运算如何施行. 当然只有 (1)-(8) 都成立时才能称它是一个线性空间.

下面举例说明.

例题 1.3. 全体 $m \times n$ 的实矩阵,关于矩阵的加法和数乘两种运算构成实数域 $\mathbb{R}$ 上的线性空间,记为 ${M}_{mn}\left( \mathbb{R}\right)$ .

例题 1.4. 用 ${\mathbb{R}}_{n}\left\lbrack x\right\rbrack$ 表示 $x$ 的以 $\mathbb{R}$ 中元素为系数的次数小于 $n$ 的多项式以及零多项式组成的集合. 在 ${\mathbb{R}}_{n}\left\lbrack x\right\rbrack$ 中把多项式的加法作为我们的加法. 设

$$
f\left( x\right) = {a}_{0} + {a}_{1}x + \cdots + {a}_{n - 1}{x}^{n - 1},
$$

而 $k \in \mathbb{R}$ ,则数乘规定为

$$
{kf}\left( x\right) = k{a}_{0} + k{a}_{1}x + \cdots + k{a}_{n - 1}{x}^{n - 1}.
$$

容易验证 (1)-(8) 成立,所以 ${\mathbb{R}}_{n}\left\lbrack x\right\rbrack$ 在上述运算下是一个线性空间.

例题 1.5. 把全体复数 $\mathbb{C}$ 看成向量集合,向量加法规定为复数加法. 取 $F =$ $\mathbb{R}$ . 若 $k \in \mathbb{R},\alpha \in \mathbb{C}$ ,规定 ${k\alpha }$ 即通常复数乘法的积,那么 $\mathbb{C}$ 就成为实数域上的线性空间. 类似地, 复数域也可以看成自身上的线性空间.

例题 1.6. 令 $\mathbb{R}$ 表示实数域,令 $V = {\mathbb{R}}^{ + }$ ,即 $V$ 是由全体正实数组成的集合. 在 $V$ 中规定加法 $\oplus$ 和数乘 $\odot$ 为

$$
x \oplus y = {xy}, x, y \in V
$$

$$
k \odot x = {x}^{k}, k \in \mathbb{R}, x \in V.
$$

即 $x, y$ 在运算 $\oplus$ 下的 “和” 为 $x, y$ 在通常实数乘法下的积 (例如 $3 \oplus 5 = {15}$ ),而 $k \in \mathbb{R}$ 与 $x \in V$ 经数乘 $\odot$ 的结果是 $x$ 的 $k$ 次方 (如 $3 \odot 5 = {125}$ ). 由实数乘法的交换律和结合律知 $\left( 1\right) ,\left( 2\right)$ 成立. 实数 1 对任何 $x \in {\mathbb{R}}^{ + }$ 都满足 $1 \oplus x = x$ ,故 1 可充当 (3) 中的零向量. 同样 ${x}^{-1}$ 可充当 $x$ 的负向量. 由指数函数的性质可推出 (5)-(8) 成立. 故 $V$ 在运算 $\oplus , \odot$ 下成为实数域上的线性空间.

## 2. 线性空间的性质

下面列出线性空间的一些简单性质. 注意, 证明中我们只能使用定义 1.1 的 (1)一(8) 作为依据. 设 $V$ 为数域 $F$ 上的线性空间.

性质 1.1. 零向量是唯一的.

证明 设 $\mathbf{0},{\mathbf{0}}^{\prime }$ 都是线性空间 $V$ 中的零向量. 因 $\mathbf{0}$ 为零向量,故由 (3) 知故 $\mathbf{0} + \mathbf{0} = {\mathbf{0}}^{\prime }$ . 又 ${\mathbf{0}}^{\prime }$ 也为零向量,故由 (3) 又知 $\mathbf{0} + {\mathbf{0}}^{\prime } = \mathbf{0}$ . 因为 $\left( 1\right) ,\mathbf{0} + {\mathbf{0}}^{\prime } = {\mathbf{0}}^{\prime } + \mathbf{0}$ ,

性质 1.2. 负向量是唯一的. 以后把 $\alpha$ 的负向量记作 $- \alpha$ .

证明 设 $\mathbf{\beta },\mathbf{\gamma }$ 都是 $\mathbf{\alpha }$ 的负向量. 我们有

$$
\beta = \beta + 0 = \beta + \left( {\alpha + \gamma }\right) = \left( {\beta + \alpha }\right) + \gamma = \left( {\alpha + \beta }\right) + \gamma = 0 + \gamma = \gamma + 0 = \gamma .
$$

这里各等号成立的依据依次为定义 1.1 的 $\left( 3\right) ,\left( 4\right) ,\left( 2\right) ,\left( 1\right) ,\left( 4\right) ,\left( 1\right)$ 和 (3)

性质 1.3. 加法消去律成立,即若 $\alpha + \gamma = \beta + \gamma$ ,则 $\alpha = \beta$ .

证明 记 $\delta = - \gamma$ ,则

$$
\alpha = \alpha + 0 = \alpha + \left( {\gamma + \delta }\right) = \left( {\alpha + \gamma }\right) + \delta = \left( {\beta + \gamma }\right) + \delta = \beta + \left( {\gamma + \delta }\right) = \beta + 0 = \beta .
$$

性质 1.4. (1) $0\mathbf{\alpha } = \mathbf{0}$ ; (2) $k\mathbf{0} = \mathbf{0}$ ; (3) $\left( {-1}\right) \mathbf{\alpha } = - \mathbf{\alpha }$ .

证明 (1) 0 为 $F$ 的零元素,若 $\mathbf{\alpha } \in V$ ,则

$$
\mathbf{\alpha } + 0\mathbf{\alpha } = 1\mathbf{\alpha } + 0\mathbf{\alpha } = \left( {1 + 0}\right) \mathbf{\alpha } = 1\mathbf{\alpha } = \mathbf{\alpha } + \mathbf{0}.
$$

故由性质 1.3 知 $0\mathbf{\alpha } = \mathbf{0}$ .

(2) 任取 $k \in F$ . 若 $k = 0$ ,则由 $\left( 1\right) , k\mathbf{0} = \mathbf{0}$ . 今设 $k \neq 0$ . 则 $k - 1$ 存在,于具对任意 $\alpha \in V$ ，

$$
\mathbf{\alpha } + k\mathbf{0} = k\left( {{k}^{-1}\mathbf{\alpha }}\right) + k\mathbf{0} = k\left( {{k}^{-1}\mathbf{\alpha } + \mathbf{0}}\right) = k\left( {{k}^{-1}\mathbf{\alpha }}\right) = \left( {k{k}^{-1}}\right) \mathbf{\alpha } = 1\mathbf{\alpha } = \mathbf{\alpha }.
$$

故由消去律知 $k\mathbf{0} = \mathbf{0}$ .

(3) $\alpha + \left( {-1}\right) \alpha = {1\alpha } + \left( {-1}\right) \alpha = \left( {1 + \left( {-1}\right) }\right) \alpha = {0\alpha } = 0$ . 由负向量的唯一性

知, $\left( {-1}\right) \mathbf{\alpha } = - \mathbf{\alpha }$ .

性质 1.5. 若 $k \in F,\alpha \in V$ 使 ${k\alpha } = 0$ ,则要么 $k = 0$ ,要么 $\alpha = 0$

证明 即要证当 ${k\alpha } = 0$ 时, ${}^{u}k = 0$ ” 与 “ $\alpha = 0$ ” 二者之中至少有一个成立

今设 $k \neq 0$ ,那么 ${k}^{-1}$ 存在. 于是 $\mathbf{\alpha } = 1\mathbf{\alpha } = \left( {{k}^{-1}k}\right) \mathbf{\alpha } = {k}^{-1}\left( {k\mathbf{\alpha }}\right) = {k}^{-1}\mathbf{0} = \mathbf{0}$ .

## 3. 线性子空间

本节总假设 $V$ 是数域 $F$ 上的线性空间.

定义 1.2. 设 $W$ 为 $V$ 的一个非空子集合,若 $W$ 关于 $V$ 的加法和数乘也成为线性空间,则称 $W$ 为 $V$ 的一个线性子空间.

例题 1.7. $V$ 的零元素构成的子集 $\{ 0\}$ 是 $V$ 的子空间,称为 $V$ 的零子空间; $V$ 本身是 $V$ 的子空间. 这两个子空间称为 $V$ 的平凡子空间, $V$ 的其他子空间称为 $V$ 的非平凡子空间.

例题 1.8. 在 ${F}^{n}$ 中取集合

$$
W = \left\{ {\left( {0,{a}_{2},{a}_{3},\cdots ,{a}_{n}}\right) \mid {a}_{i} \in F}\right\}
$$

则 $W$ 为 ${F}^{n}$ 的子空间.

由于

$$
\left( {0,{a}_{2},{a}_{3},\cdots ,{a}_{n}}\right) + \left( {0,{b}_{2},{b}_{3},\cdots ,{b}_{n}}\right) = \left( {0,{a}_{2} + {b}_{2},{a}_{3} + {b}_{3},\cdots ,{a}_{n} + {b}_{n}}\right) ,
$$

所以 $W$ 中两个向量在 $V$ 的加法运算下之和还在 $W$ 中. 同样,

$$
k\left( {0,{a}_{2},{a}_{3},\cdots ,{a}_{n}}\right) = \left( {0, k{a}_{2}, k{a}_{3},\cdots , k{a}_{n}}\right) \in W.
$$

易知此时定义 1.1 的 $\left( 1\right) - \left( 8\right)$ 均成立. 其中 $\left( {0,0,\cdots ,0}\right)$ 为 $W$ 的零向量, $\left( {0, - {a}_{2}}\right.$ , $\left. {-{a}_{3},\cdots , - {a}_{n}}\right)$ 为 $\left( {0,{a}_{2},{a}_{3},\cdots ,{a}_{n}}\right)$ 的负向量. 于是 $W$ 为 ${F}^{n}$ 的一个子空间.

设在 $V$ 中已给了一个非空子集合 $W, W$ 要满足什么条件才成为 $V$ 的子空间呢? 首先, $W$ 作为 $V$ 的子集, $V$ 中的运算对 $W$ 中的元素来说,线性空间的定义 1.1 中的 $\left( 1\right) ,\left( 2\right) ,\left( 5\right) - \left( 8\right)$ 显然满足. 因此,只要 $W$ 关于 $V$ 的两种运算封闭且满足 (3) 和 (4),则 $W$ 就可构成一个线性空间. 这里,“ $W$ 关于 $V$ 的两种运算封闭” 是指: 若 $\mathbf{\alpha },\mathbf{\beta } \in W$ ,则 $\mathbf{\alpha } + \mathbf{\beta } \in W$ ; 若 $k \in F,\mathbf{\alpha } \in W$ ,则 $k\mathbf{\alpha } \in W$ . 但是, 若 $W$ 关于 $V$ 的两种运算封闭,则对 $\mathbf{\alpha } \in W$ ,分别取 $k = 0,1$ ,就有 $\mathbf{0} = 0\mathbf{\alpha } \in W$ , $- \mathbf{\alpha } = \left( {-1}\right) \mathbf{\alpha } \in W$ ,即定义 1.1 中的 (3) 和 (4) 自然也满足.

由此引入定理 1.1.

定理 1.1. 设 $V$ 为数域 $F$ 上的线性空间, $W$ 为 $V$ 的非空子集合. $W$ 是 $V$ 的子空间的充要条件是: $W$ 对 $V$ 中的加法和数乘封闭,即对于任意 $\alpha ,\beta \in W$ , $k \in F$ ,必有 $\mathbf{\alpha } + \mathbf{\beta } \in W, k\mathbf{\alpha } \in W$ .

证明 由上面的分析知, 条件是必要的.

今设 $W$ 对加法和数乘封闭. 此时 $V$ 的加法和数乘就是 $W$ 的运算. 因为 $W$ 非空,设 $\alpha \in W$ ,于是 $\mathbf{0} = 0\mathbf{\alpha } \in W$ . 当 $\mathbf{\beta }$ 为 $W$ 中任意向量时,由数乘的封闭性知, $- \mathbf{\beta } = \left( {-1}\right) \mathbf{\beta } \in W$ ,故在 $W$ 中定义 1.1 的 (3),(4) 成立. 由上面的分析知, $\left( 1\right) ,\left( 2\right) ,\left( 5\right) - \left( 8\right)$ 在 $W$ 中自然成立,故 $W$ 为 $V$ 的子空间.

例题 1.9. $n$ 元实系数齐次线性方程组 $\mathbf{A}\mathbf{X} = \mathbf{0}$ 的解 $\left( {{c}_{1},{c}_{2},\cdots ,{c}_{n}}\right)$ 可视为 ${\mathbb{R}}^{n}$ 的向量. 其全部解构成 ${\mathbb{R}}^{n}$ 的一个子集合 $W$ . 由于 $\left( {0,0\cdots ,0}\right)$ 为解,故 $W$ 非空. 两个解的和以及数乘还是解. 于是我们得到了一个重要结论: 一个 $n$ 元实系数齐次线性方程组的解的集合对 ${\mathbb{R}}^{n}$ 中的加法和数乘封闭,它构成 ${\mathbb{R}}^{n}$ 的子空间, 我们称之为齐次线性方程组的解空间.

$n$ 元实系数非齐次线性方程组 $\mathbf{A}\mathbf{X} = \mathbf{b}\left( {\mathbf{b} \neq \mathbf{0}}\right)$ 解的集合不构成 ${\mathbb{R}}^{n}$ 的子空间.

例题 1.10. $n$ 阶上三角形实矩阵的全体关于矩阵的加法和数乘运算是封闭的,因此它是 ${M}_{nn}\left( \mathbb{R}\right)$ 的子空间; 所有 $n$ 阶下三角形实矩阵集合也是 ${M}_{nn}\left( \mathbb{R}\right)$ 的子空间.

例题 1.11. 设 $V$ 为数域 $F$ 上的线性空间, ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2} \in V$ ,它们所有可能的线性组合的全体集合

$$
W = \left\{ {\mathbf{\beta } \mid \mathbf{\beta } = {k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2},{k}_{1},{k}_{2} \in F}\right\}
$$

关于 $V$ 的加法和数乘运算构成 $V$ 的线性子空间.

事实上, $W$ 非空,且对两种运算封闭,即若 ${\mathbf{\beta }}_{1} = {k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2},{\mathbf{\beta }}_{2} = {\ell }_{1}{\mathbf{\alpha }}_{1} +$ ${\ell }_{2}{\mathbf{\alpha }}_{2}$ ,则

$$
{\mathbf{\beta }}_{1} + {\mathbf{\beta }}_{2} = \left( {{k}_{1} + {\ell }_{1}}\right) {\mathbf{\alpha }}_{1} + \left( {{k}_{2} + {\ell }_{2}}\right) {\mathbf{\alpha }}_{2} \in W
$$

$$
k{\mathbf{\beta }}_{1} = k{k}_{1}{\mathbf{\alpha }}_{1} + k{k}_{2}{\mathbf{\alpha }}_{2} \in W.
$$

因此, $W$ 是 $V$ 的子空间,称为由元素 (向量) ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2}$ 生成的子空间,记为 $W =$ $L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2}}\right)$ ,而 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2}$ 称为 $W$ 的生成元.

一般而言,由 $V$ 的向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 所生成的子空间为

$$
L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}}\right) = \left\{ {\mathbf{\beta } \mid \mathbf{\beta } = {k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{s}{\mathbf{\alpha }}_{s},{k}_{1},{k}_{2},\cdots ,{k}_{s} \in F}\right\} .
$$

由子空间的定义知若 $V$ 的一个子空间 $U$ 包含 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ ,则 $U$ 一定包含 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 的一切线性组合,从而它必包含 $L\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}}\right)$ 作为子空间.

## $§{7.2}$ 维数、基与坐标

## 1. 向量的线性表示

在第四章讨论 $n$ 维向量空间 ${F}^{n}$ 时,我们定义了线性组合、线性相关、线性无关、向量组等价、极大线性无关组和向量组秩的概念, 以及有关的性质. 这些概念和结果都可以直接推广到抽象的线性空间.

定义 2.1. 设 $V$ 是数域 $F$ 上的线性空间, $\mathbf{\alpha },{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 是 $V$ 中的 $s + 1\left( {s \geq 1}\right)$ 个向量,若存在一组数 ${k}_{1},{k}_{2},\cdots ,{k}_{s} \in F$ ,使

$$
\mathbf{\alpha } = {k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{s}{\mathbf{\alpha }}_{s}
$$

成立,则称 $\mathbf{\alpha }$ 是向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 的线性组合,或者说 $\mathbf{\alpha }$ 可由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots$ , ${\alpha }_{s}$ 线性表示 (线性表出).

定义 2.2. 若向量组 (I): ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 和向量组 (II): ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{t}$ 是 $V$ 中的两个向量组, 且向量组 (I) 的每个向量都可以由向量组 (II) 中的向量线性表出, 则称向量组 (I) 可以由向量组 (II) 线性表出. 若向量组 (I) 和向量组 (II) 可以互相线性表出, 则称它们等价.

定义 2.3. 设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 为线性空间 $V$ 中的向量,若 $F$ 中存在 $s$ 个不全为零的元素 ${k}_{1},{k}_{2},\cdots ,{k}_{s}$ ,使

$$
{k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{s}{\mathbf{\alpha }}_{s} = \mathbf{0}
$$

成立,则称向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 线性相关. 否则,称 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s}$ 线性无关.

这些定义与第四章中的一样,只不过那里是在 ${F}^{n}$ 这个特殊的线性空间中来定义的,其元素或向量是 $F$ 上的 $n$ 元有序数组,而这里是在一般的线性空间上来给出定义的,这里 $V$ 的元素或向量是抽象的,其具体形式没有给出. 同样,在 ${F}^{n}$ 中讨论的向量组的性质也可以照搬到一般的线性空间上来,这里列出几个常用的结果:

(1) 单个向量 $\mathbf{\alpha }$ 是线性相关当且仅当 $\mathbf{\alpha } = \mathbf{0}$ . 两个以上的向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots$ , ${\alpha }_{m}$ 线性相关的充要条件是其中至少有一个向量可由其余向量线性表出.

(2) 若向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,且可以被向量组 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{s}$ 线性表出,则 $r \leq s$ .

由此易得, 两个等价的线性无关向量组含有相同个数的向量.

(3) 若向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,而向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r},\mathbf{\beta }$ 线性相关,则 $\mathbf{\beta }$ 可由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表出,且表示方法唯一.

我们给出 (3) 的证明. 由向量组 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r},\mathbf{\beta }$ 线性相关知,存在不全为零的数 ${k}_{1},{k}_{2},\cdots ,{k}_{r}, k \in F$ ,使得

$$
{k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{r}{\mathbf{\alpha }}_{r} + k\mathbf{\beta } = \mathbf{0}
$$

则必有 $k \neq 0$ . 这是因为若 $k = 0$ ,则 ${k}_{1},{k}_{2},\cdots ,{k}_{r}$ 不全为零,且上式变为 ${k}_{1}{\alpha }_{1} +$ ${k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{r}{\mathbf{\alpha }}_{r} = \mathbf{0}$ ,这样 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性相关,与已知矛盾. 故 $k \neq 0$ ,从而有

$$
\mathbf{\beta } = - \frac{{k}_{1}}{k}{\mathbf{\alpha }}_{1} - \frac{{k}_{2}}{k}{\mathbf{\alpha }}_{2} - \cdots - \frac{{k}_{r}}{k}{\mathbf{\alpha }}_{r}
$$

即 $\mathbf{\beta }$ 可由 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性表出.

若有 $\mathbf{\beta } = {k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{r}{\mathbf{\alpha }}_{r},\mathbf{\beta } = {k}_{1}^{\prime }{\mathbf{\alpha }}_{1} + {k}_{2}^{\prime }{\mathbf{\alpha }}_{2} + \cdots + {k}_{r}^{\prime }{\mathbf{\alpha }}_{r}$ . 两式相减得

$$
\left( {{k}_{1} - {k}_{1}^{\prime }}\right) {\mathbf{\alpha }}_{1} + \left( {{k}_{2} - {k}_{2}^{\prime }}\right) {\mathbf{\alpha }}_{2} + \cdots + \left( {{k}_{r} - {k}_{r}^{\prime }}\right) {\mathbf{\alpha }}_{r} = \mathbf{0}.
$$

而 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{r}$ 线性无关,故 ${k}_{1} = {k}_{1}^{\prime },\cdots ,{k}_{r} = {k}_{r}^{\prime }$ ,表示方法唯一.

## 2. 维数、基与坐标

在 ${\mathbb{R}}^{3}$ 中,线性无关的向量最多有 3 个,而任意 4 个向量一定共面,即线性相关; 在 ${F}^{n}$ 中,有 $n$ 个线性无关的向量,比如 $n$ 维单位向量 ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ ,而任意 $n + 1$ 个向量一定是线性相关的. 我们自然想到,在一个数域 $F$ 上的线性空间 $V$ 中线性无关的向量有几个. 为此,我们给出定义.

定义 2.4. 在线性空间 $V$ 中,若有 $n$ 个向量 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ ,满足

(1) ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 线性无关;

(2) $V$ 中任意一个向量 $\mathbf{\alpha }$ 都可以被 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 线性表出,

则称 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 是线性空间 $V$ 的一组基, $V$ 就称为是 $n$ 维的线性空间或 $V$ 的维数是 $n$ ,记为 $\dim \left( V\right) = n$ . 如果在 $V$ 中可以找到任意多个线性无关的向量, 那么 $V$ 就称为是无限维的线性空间. 规定零空间的维数是 0 .

由定义知, $\dim \left( {\mathbb{R}}^{3}\right) = 3,\dim \left( {F}^{n}\right) = n$ . 实数域 $\mathbb{R}$ 上的一元多项式的全体构成的实线性空间是无限维的,因为对于任意的 $n$ ,都可以找到 $n$ 个线性无关的向量 $1, x,{x}^{2},\cdots ,{x}^{n - 1}$ . 又比如 $n$ 元齐次线性方程组 $\mathbf{A}\mathbf{X} = \mathbf{0}$ 的解空间的维数为 $n - r\left( \mathbf{A}\right)$ ,解空间的基为该齐次线性方程组的任意一个基础解系.

今设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 为 $n$ 维线性空间 $V$ 的一组基, $\mathbf{\alpha }$ 为 $V$ 中的一个向量, 则 $\alpha$ 可表示成 ${\alpha }_{1},{\alpha }_{2},\cdots ,{\alpha }_{n}$ 的线性组合,即

$$
\mathbf{\alpha } = {x}_{1}{\mathbf{\alpha }}_{1} + {x}_{2}{\mathbf{\alpha }}_{2} + \cdots + {x}_{n}{\mathbf{\alpha }}_{n} \tag{2.1}
$$

且表示唯一,即 ${x}_{i}$ 由 $\mathbf{\alpha }$ 和基 ${\mathbf{\alpha }}_{i}$ 唯一确定. 此时我们把 ${F}^{n}$ 中的向量 $\left( {{x}_{1},{x}_{2},\cdots }\right.$ , $\left. {x}_{n}\right)$ 称为 $\mathbf{\alpha }$ 在基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 下的坐标.

式子 (2.1) 可以形式地表示为

$$
\mathbf{\alpha } = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) \left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right)
$$

若此时向量 $\mathbf{\beta }$ 在基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 下有坐标 $\left( {{y}_{1},{y}_{2},\cdots ,{y}_{n}}\right)$ ,那么易知 $\mathbf{\alpha } + \mathbf{\beta }$ 在此基下的坐标为

$$
\left( {{x}_{1} + {y}_{1},{x}_{2} + {y}_{2},\cdots ,{x}_{n} + {y}_{n}}\right)
$$

${k\alpha }$ 的坐标为

$$
\left( {k{x}_{1}, k{x}_{2},\cdots , k{x}_{n}}\right) \text{.}
$$

于是, 利用基和坐标可把线性空间的运算变得更具体.

例题 2.1. 在 ${\mathbb{R}}^{n}$ 中,我们已经知道

$$
{\varepsilon }_{1} = \left( {1,0,\cdots ,0}\right)
$$

$$
{\varepsilon }_{2} = \left( {0,1,\cdots ,0}\right)
$$

...

$$
{\varepsilon }_{n} = \left( {0,0,\cdots ,1}\right)
$$

线性无关,且任意一个向量 $\mathbf{\alpha } = \left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right)$ 都有

$$
\alpha = {a}_{1}{\varepsilon }_{1} + {a}_{2}{\varepsilon }_{2} + \cdots + {a}_{n}{\varepsilon }_{n}
$$

所以, ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ 是一组基,且 $\left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right)$ 就是 $\mathbf{\alpha }$ 在这组基下的坐标.

再比如, 若取

$$
{\eta }_{1} = \left( {1,1,\cdots ,1}\right)
$$

$$
{\eta }_{2} = \left( {0,1,\cdots ,1}\right)
$$

$$
\ldots
$$

$$
{\eta }_{n} = \left( {0,0,\cdots ,1}\right)
$$

易证它们线性无关,对任意向量 $\mathbf{\alpha } = \left( {{a}_{1},{a}_{2},\cdots ,{a}_{n}}\right)$ 有

$$
\mathbf{\alpha } = {a}_{1}{\mathbf{\eta }}_{1} + \left( {{a}_{2} - {a}_{1}}\right) {\mathbf{\eta }}_{2} + \cdots + \left( {{a}_{n} - {a}_{n - 1}}\right) {\mathbf{\eta }}_{n}.
$$

所以 ${\eta }_{1},{\eta }_{2},\cdots ,{\eta }_{n}$ 是一组基,且 $\left( {{a}_{1},{a}_{2} - {a}_{1},\cdots ,{a}_{n} - {a}_{n - 1}}\right)$ 就是 $\mathbf{\alpha }$ 在基 ${\eta }_{1}$ , ${\eta }_{2},\cdots ,{\eta }_{n}$ 下的坐标.

例题 2.2. 考虑实数域上的所有 $2 \times 2$ 矩阵的全体关于矩阵的加法和数乘构成的线性空间 ${M}_{22}\left( \mathbb{R}\right)$ .

解 设

$$
{\mathbf{E}}_{11} = \left( \begin{array}{ll} 1 & 0 \\ 0 & 0 \end{array}\right) ,{\mathbf{E}}_{12} = \left( \begin{array}{ll} 0 & 1 \\ 0 & 0 \end{array}\right) ,{\mathbf{E}}_{21} = \left( \begin{array}{ll} 0 & 0 \\ 1 & 0 \end{array}\right) ,{\mathbf{E}}_{22} = \left( \begin{array}{ll} 0 & 0 \\ 0 & 1 \end{array}\right) .
$$

首先我们证明 ${\mathbf{E}}_{11},{\mathbf{E}}_{12},{\mathbf{E}}_{21},{\mathbf{E}}_{22}$ 线性无关. 若 ${k}_{1}{\mathbf{E}}_{11} + {k}_{2}{\mathbf{E}}_{12} + {k}_{3}{\mathbf{E}}_{21} +$ ${k}_{4}{\mathbf{E}}_{22} = 0$ ,即有 $\left( \begin{array}{ll} {k}_{1} & {k}_{2} \\ {k}_{3} & {k}_{4} \end{array}\right) = \left( \begin{array}{ll} 0 & 0 \\ 0 & 0 \end{array}\right)$ ,故得 ${k}_{1} = {k}_{2} = {k}_{3} = {k}_{4} = 0$ . 又对任意 $2 \times 2$ 矩阵 $\mathbf{A} = \left( \begin{array}{ll} a & b \\ c & d \end{array}\right)$ 有

$$
\mathbf{A} = a{\mathbf{E}}_{11} + b{\mathbf{E}}_{12} + c{\mathbf{E}}_{21} + d{\mathbf{E}}_{22}
$$

所以 ${\mathbf{E}}_{ij}\left( {i, j = 1,2}\right)$ 是 ${M}_{22}\left( \mathbb{R}\right)$ 的一组基, $\dim \left( {{M}_{22}\left( \mathbb{R}\right) }\right) = 4$ 且 $\mathbf{A}$ 在基 ${\mathbf{E}}_{11},{\mathbf{E}}_{12}$ , ${\mathbf{E}}_{21},{\mathbf{E}}_{22}$ 下的坐标为 $\left( {a, b, c, d}\right)$ .

此例题的结果不难推广到一般的空间 ${M}_{mn}\left( \mathbb{R}\right)$ .

## 3. 基变换和坐标变换公式

由例题 2.1 可知, 一个线性空间有不同的基. 一般而言, 线性空间的同一个向量在不同基下有不同的坐标, 这里我们讨论坐标之间的关系.

设 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 和 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ 都是 $V$ 的基, $\mathbf{\alpha }$ 为 $V$ 的一个向量,设 $\mathbf{\alpha }$ 在 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 下的坐标为 $\left( {{x}_{1},{x}_{2},\cdots ,{x}_{n}}\right)$ ,在 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ 下的坐标为$\left( {{y}_{1},{y}_{2},\cdots ,{y}_{n}}\right)$

坐标之间的关系显然由两组基之间的关系决定. 由于 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 为基, 故每个 ${\mathbf{\beta }}_{j}$ 可以表示为 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 的线性组合. 设

$$
\left\{ \begin{matrix} {\mathbf{\beta }}_{1} = {c}_{11}{\mathbf{\alpha }}_{1} + {c}_{21}{\mathbf{\alpha }}_{2} + \cdots + {c}_{n1}{\mathbf{\alpha }}_{n}, \\ {\mathbf{\beta }}_{2} = {c}_{12}{\mathbf{\alpha }}_{1} + {c}_{22}{\mathbf{\alpha }}_{2} + \cdots + {c}_{n2}{\mathbf{\alpha }}_{n}, \\ \cdots \cdots \cdots \cdots \\ {\mathbf{\beta }}_{n} = {c}_{1n}{\mathbf{\alpha }}_{1} + {c}_{2n}{\mathbf{\alpha }}_{2} + \cdots + {c}_{nn}{\mathbf{\alpha }}_{n}, \end{matrix}\right. \tag{\left {2.2}\right}
$$

我们把矩阵

$$
\mathbf{C} = \left( \begin{matrix} {c}_{11} & {c}_{12} & \cdots & {c}_{1n} \\ {c}_{21} & {c}_{22} & \cdots & {c}_{2n} \\ \vdots & \vdots & & \vdots \\ {c}_{n1} & {c}_{n2} & \cdots & {c}_{nn} \end{matrix}\right) \tag{2.3}
$$

称为由基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 到基 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ 的过渡矩阵. 利用矩阵的乘法,两组基的关系可形式地表示为

$$
\left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right) = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) \mathbf{C},
$$

称为基变换公式. 另一方面,我们也可用矩阵写法表示 $\alpha$ 在两组基下的坐标,即

$$
\mathbf{\alpha } = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) \mathbf{X} = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right) \mathbf{Y},
$$

这里

$$
\mathbf{X} = \left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right) ,\mathbf{Y} = \left( \begin{matrix} {y}_{1} \\ {y}_{2} \\ \vdots \\ {y}_{n} \end{matrix}\right)
$$

因此

$$
\mathbf{\alpha } = \left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right) \mathbf{Y} = \left( {\left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) \mathbf{C}}\right) \mathbf{Y} = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) \left( \mathbf{{CY}}\right) .
$$

但 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 是基,因而线性无关. 由坐标的唯一性,得到 $\mathbf{X} = \mathbf{{CY}}$ ,即

$$
\left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right) = \mathbf{C}\left( \begin{matrix} {y}_{1} \\ {y}_{2} \\ \vdots \\ {y}_{n} \end{matrix}\right) \tag{2.4}
$$

亦即

$$
\left\{ \begin{matrix} {x}_{1} = {c}_{11}{y}_{1} + {c}_{12}{y}_{2} + \cdots + {c}_{1n}{y}_{n} \\ {x}_{2} = {c}_{21}{y}_{1} + {c}_{22}{y}_{2} + \cdots + {c}_{2n}{y}_{n} \\ \cdots \cdots \cdots \cdots \\ {x}_{n} = {c}_{n1}{y}_{1} + {c}_{n2}{y}_{2} + \cdots + {c}_{nn}{y}_{n} \end{matrix}\right. \tag{2.5}
$$

式 (2.4) 或 (2.5) 称为坐标变换公式.

最后,我们断言由基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 到基 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ 的过渡矩阵 $\mathbf{C}$ 是可逆矩阵.

理由如下: 考虑 $n$ 元齐次线性方程组 $\mathbf{C}\mathbf{X} = \mathbf{0}$ ,若能证明它只有零解,则 $r\left( \mathbf{C}\right) = n$ ,从而 $\mathbf{C}$ 可逆. 设

$$
{\mathbf{X}}_{0} = \left( \begin{matrix} {k}_{1} \\ {k}_{2} \\ \vdots \\ {k}_{n} \end{matrix}\right)
$$

是 ${CX} = 0$ 的解,则

$$
\left( {{\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}}\right) {\mathbf{X}}_{0} = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) \left( {\mathbf{C}{\mathbf{X}}_{0}}\right) = \left( {{\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}}\right) \left( \begin{matrix} 0 \\ 0 \\ \vdots \\ 0 \end{matrix}\right) = \mathbf{0}.
$$

即 ${k}_{1}{\mathbf{\beta }}_{1} + {k}_{2}{\mathbf{\beta }}_{2} + \cdots + {k}_{n}{\mathbf{\beta }}_{n} = \mathbf{0}$ 成立,而 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ 是线性空间 $V$ 的一组基,它们线性无关,故 ${k}_{1} = {k}_{2} = \cdots = {k}_{n} = 0$ . 故 $r\left( \mathbf{C}\right) = n$ ,从而 $\mathbf{C}$ 可逆.

综上, 有下述定理.

定理 2.1. 设 $n$ 维线性空间 $V$ 的基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{n}$ 到基 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},\cdots ,{\mathbf{\beta }}_{n}$ 的过渡矩阵为 $C$ ,则 $C$ 是可逆矩阵. 若向量 $\alpha \in V$ 在这两组基下的坐标分别是

$\left( {{x}_{1},{x}_{2},\cdots ,{x}_{n}}\right) ,\left( {{y}_{1},{y}_{2},\cdots ,{y}_{n}}\right)$ ,令 $\mathbf{X} = {\left( {x}_{1},{x}_{2},\cdots ,{x}_{n}\right) }^{\mathrm{T}}$ 和 $\mathbf{Y} = {\left( {y}_{1},{y}_{2},\cdots ,{y}_{n}\right) }^{\mathrm{T}}$ ,

则

$$
X = {CY}\text{ 或 }Y = {C}^{-1}X.
$$

## §7.3 线性变换

## 1. 线性变换的定义

定义 3.1. 设 $V$ 是数域 $F$ 上的线性空间, $\sigma$ 是 $V$ 到 $V$ 自身的一个映射. 如果 $\sigma$ 满足

(1) 对任意的 $\mathbf{\alpha },\mathbf{\beta } \in V$ ,都有 $\sigma \left( {\mathbf{\alpha } + \mathbf{\beta }}\right) = \sigma \left( \mathbf{\alpha }\right) + \sigma \left( \mathbf{\beta }\right)$ ;

(2) 对任意的 $\mathbf{\alpha } \in V, k \in F$ ,都有 $\sigma \left( {k\mathbf{\alpha }}\right) = {k\sigma }\left( \mathbf{\alpha }\right)$ ,

则称 $\sigma$ 为线性空间 $V$ 的一个线性变换.

在定义中,(1) 要求对 $V$ 中的向量 $\mathbf{\alpha },\mathbf{\beta }$ 而言,它们的和在 $\sigma$ 下的像等于它们像的和. 这一事实称为 $\sigma$ 保持加法; (2) 要求向量 $\mathbf{\alpha }$ 与 $k$ 的数乘的像等于 $\mathbf{\alpha }$ 的像与 $k$ 的数乘. 这一事实称 $\sigma$ 保持数乘.

例题 3.1. 设在空间中建立了直角坐标系, 全体从原点出发的向量组成了三维线性空间 $V$ ,令

$$
\sigma : \;\left( {x, y, z}\right) \rightarrow \left( {x, y,0}\right)
$$

则 $\sigma$ 是 $V$ 的线性变换,常称为投影变换,它的几何意义是把向量 $\mathbf{\alpha }$ 投影到 ${xOy}$ 平面上.

例题 3.2. 设 $V$ 为 $F$ 上的 $n$ 维线性空间. $\forall \mathbf{\alpha } \in V, k \in F$ ,定义 $\sigma \left( \mathbf{\alpha }\right) = k\mathbf{\alpha }$ , 则易验证 $\sigma$ 是 $V$ 的一个线性变换,称为由数 $k$ 决定的数乘变换.

特别地,取 $k = 0$ ,即 $\forall \mathbf{\alpha } \in V$ ,定义 $\sigma \left( \mathbf{\alpha }\right) = \mathbf{0}$ ,即把 $V$ 中每个向量都映射成 $V$ 的零向量,此时变换称为零变换,记为 $\mathcal{O}$ . 若定义 $\sigma \left( \mathbf{\alpha }\right) = \mathbf{\alpha }$ (即取 $k = 1$ ),常称为恒等变换或单位变换,记为 $\mathcal{E}$ .

例题 3.3. 设 $V = {\mathbb{R}}_{n}\left\lbrack x\right\rbrack$ 为次数小于 $n$ 的实系数多项式以及零多项式组成的线性空间, 则求导数运算

$$
\mathcal{D} : \;f\left( x\right) \rightarrow {f}^{\prime }\left( x\right)
$$

是 $V$ 的线性变换,称为微分变换.

证明 对任意的 $f\left( x\right) , g\left( x\right) \in V, k \in \mathbb{R}$ 有

$$
\mathcal{D}\left( {f\left( x\right) + g\left( x\right) }\right) = {\left( f\left( x\right) + g\left( x\right) \right) }^{\prime } = {f}^{\prime }\left( x\right) + {g}^{\prime }\left( x\right) = \mathcal{D}\left( {f\left( x\right) }\right) + \mathcal{D}\left( {g\left( x\right) }\right) .
$$

$$
\mathcal{D}\left( {{kf}\left( x\right) }\right) = {\left( kf\left( x\right) \right) }^{\prime } = k{f}^{\prime }\left( x\right) = k\mathcal{D}\left( {f\left( x\right) }\right) .
$$

故它是 ${\mathbb{R}}_{n}\left\lbrack x\right\rbrack$ 的线性变换.

2. 线性变换的简单性质

线性空间 $V$ 的线性变换 $\sigma$ 有下列初等性质:

(1) $\sigma \left( \mathbf{0}\right) = \mathbf{0},\sigma \left( {-\mathbf{\alpha }}\right) = - \sigma \left( \mathbf{\alpha }\right)$ .

实际上,

$$
\sigma \left( \mathbf{0}\right) = \sigma \left( {0\mathbf{\alpha }}\right) = {0\sigma }\left( \mathbf{\alpha }\right) = \mathbf{0},
$$

$$
\sigma \left( {-\mathbf{\alpha }}\right) = \sigma \left( {\left( {-1}\right) \mathbf{\alpha }}\right) = \left( {-1}\right) \sigma \left( \mathbf{\alpha }\right) = - \sigma \left( \mathbf{\alpha }\right) .
$$

(2) 线性变换保持线性组合与线性关系式不变, 即

$$
\sigma \left( {{k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{s}{\mathbf{\alpha }}_{s}}\right) = {k}_{1}\sigma \left( {\mathbf{\alpha }}_{1}\right) + {k}_{2}\sigma \left( {\mathbf{\alpha }}_{2}\right) + \cdots + {k}_{s}\sigma \left( {\mathbf{\alpha }}_{s}\right) .
$$

反复使用定义中的 $\left( 1\right) ,\left( 2\right)$ 即得.

(3) 若 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},\cdots ,{\mathbf{\alpha }}_{s} \in V$ 线性相关,则 $\sigma \left( {\mathbf{\alpha }}_{1}\right) ,\sigma \left( {\mathbf{\alpha }}_{2}\right) \cdots ,\sigma \left( {\mathbf{\alpha }}_{s}\right)$ 也线性相关.

设有不全为 0 的数 ${k}_{1},{k}_{2},\cdots ,{k}_{s}$ ,使 ${k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{s}{\mathbf{\alpha }}_{s} = \mathbf{0}$ ,则

$$
\sigma \left( {{k}_{1}{\mathbf{\alpha }}_{1} + {k}_{2}{\mathbf{\alpha }}_{2} + \cdots + {k}_{s}{\mathbf{\alpha }}_{s}}\right) = \sigma \left( \mathbf{0}\right) = \mathbf{0},
$$

即

$$
{k}_{1}\sigma \left( {\mathbf{\alpha }}_{1}\right) + {k}_{2}\sigma \left( {\mathbf{\alpha }}_{2}\right) + \cdots + {k}_{s}\sigma \left( {\mathbf{\alpha }}_{s}\right) = \mathbf{0},
$$

这说明 $\sigma \left( {\mathbf{\alpha }}_{1}\right) ,\sigma \left( {\mathbf{\alpha }}_{2}\right) ,\cdots ,\sigma \left( {\mathbf{\alpha }}_{s}\right)$ 线性相关.

注意, 性质 (3) 的逆命题不成立, 线性变换可能把线性无关的向量组变成线

性相关的向量组, 比如零变换.

(4) 设 $\sigma$ 为 $n$ 维线性空间 $V$ 的线性变换, $\sigma$ 的像集

$$
\sigma \left( V\right) = \{ \mathbf{\beta } \mid \mathbf{\beta } = \sigma \left( \mathbf{\alpha }\right) ,\mathbf{\alpha } \in V\}
$$

它是 $V$ 的一个线性子空间,称为 $\sigma$ 的值域或像空间.

显然 $\mathbf{0} \in \sigma \left( V\right)$ ,故 $\sigma \left( V\right)$ 为 $V$ 的非空子集. 任取 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2} \in \sigma \left( V\right)$ ,则存在 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2} \in V$ ,使得 $\sigma \left( {\mathbf{\alpha }}_{1}\right) = {\mathbf{\beta }}_{1},\sigma \left( {\mathbf{\alpha }}_{2}\right) = {\mathbf{\beta }}_{2}$ ,则

$$
{\mathbf{\beta }}_{1} + {\mathbf{\beta }}_{2} = \sigma \left( {\mathbf{\alpha }}_{1}\right) + \sigma \left( {\mathbf{\alpha }}_{2}\right) = \sigma \left( {{\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2}}\right) \in \sigma \left( V\right) ,
$$

$$
k{\mathbf{\beta }}_{1} = {k\sigma }\left( {\mathbf{\alpha }}_{1}\right) = \sigma \left( {k{\mathbf{\alpha }}_{1}}\right) \in \sigma \left( V\right) .
$$

因此, $\sigma \left( V\right)$ 为 $V$ 的一个子空间.

(5) 设 $\sigma$ 为 $n$ 维线性空间 $V$ 的线性变换,集合

$$
\operatorname{Ker}\left( \sigma \right) = \{ \alpha \in V \mid \sigma \left( \alpha \right) = 0\}
$$

称为线性变换 $\sigma$ 的核. 容易证明 $\operatorname{Ker}\left( \sigma \right)$ 也是 $V$ 的一个子空间,称为 $\sigma$ 的核空间.

关于 $n$ 维线性空间 $V$ 的线性变换的值域和核,我们不加证明地给出以下结果:

$$
\dim \left( {\sigma \left( V\right) }\right) + \dim \left( {\operatorname{Ker}\left( \sigma \right) }\right) = n.
$$

## 3. 线性变换的矩阵

定义 3.2. 设 $V$ 为 $F$ 上的 $n$ 维线性空间, $\sigma$ 为 $V$ 的线性变换. 设 ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ 为 $V$ 中的一组基,则基向量在 $\sigma$ 下的像可以被基 ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ 线性表出,如果设

$$
\left\{ \begin{matrix} \sigma \left( {\varepsilon }_{1}\right) = {a}_{11}{\varepsilon }_{1} + {a}_{21}{\varepsilon }_{2} + \cdots + {a}_{n1}{\varepsilon }_{n}, \\ \sigma \left( {\varepsilon }_{2}\right) = {a}_{12}{\varepsilon }_{1} + {a}_{22}{\varepsilon }_{2} + \cdots + {a}_{n2}{\varepsilon }_{n}, \\ \cdots \cdots \cdots \cdots \\ \sigma \left( {\varepsilon }_{n}\right) = {a}_{1n}{\varepsilon }_{1} + {a}_{2n}{\varepsilon }_{2} + \cdots + {a}_{nn}{\varepsilon }_{n}, \end{matrix}\right. \tag{3.1}
$$

则 $n$ 阶方阵

$$
\mathbf{A} = \left( \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{n1} & {a}_{n2} & \cdots & {a}_{nn} \end{matrix}\right)
$$

称为线性变换 $\sigma$ 在基 ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ 下的矩阵. 其中 $\mathbf{A}$ 的第 $j$ 列就是基向量 ${\varepsilon }_{j}$ 的像 $\sigma \left( {\varepsilon }_{j}\right)$ 在这组基下的坐标.

记 $\sigma \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) = \left( {\sigma \left( {\varepsilon }_{1}\right) ,\sigma \left( {\varepsilon }_{2}\right) ,\cdots ,\sigma \left( {\varepsilon }_{n}\right) }\right)$ ,则上式可用矩阵表示为

$$
\sigma \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) = \left( {\sigma \left( {\varepsilon }_{1}\right) ,\sigma \left( {\varepsilon }_{2}\right) ,\cdots ,\sigma \left( {\varepsilon }_{n}\right) }\right) = \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) A.
$$

这样,取定 $F$ 上的 $n$ 维线性空间 $V$ 的一组基之后,对于 $V$ 的每一个线性变换, $F$ 上有唯一确定的 $n \times n$ 矩阵和它对应. 反过来,任给一个数域 $F$ 上的 $n$ 阶方阵,按照 (3.1) 式可以唯一地定义一个线性变换 $\sigma$ (其证明我们不作要求). 这表明, $V$ 的线性变换与 $n$ 阶方阵之间一一对应. 当然这种对应关系以给定 $V$ 的一组基为前提条件, 若基改变, 线性变换对应的矩阵一般也要改变, 这一点后面还会谈到.

由定义知,把一切向量都映射成零向量的线性变换 $\mathcal{O}$ 在任意基下的矩阵为 $n$ 阶零矩阵 0,而恒等变换 $\mathcal{E}$ 在任意基下的矩阵是单位矩阵 ${\mathbf{E}}_{n}$ .

例题 3.4. 在 ${\mathbb{R}}^{3}$ 中,取基 ${\varepsilon }_{1} = \left( {1,0,0}\right) ,{\varepsilon }_{2} = \left( {0,1,0}\right) ,{\varepsilon }_{3} = \left( {0,0,1}\right)$ ,对于例题 3.1 中的投影变换 $\sigma$ ,求 $\sigma$ 在 ${\varepsilon }_{1},{\varepsilon }_{2},{\varepsilon }_{3}$ 下的矩阵.

实际上,对投影变换 $\sigma$ 有

$$
\sigma \left( {\varepsilon }_{1}\right) = \left( {1,0,0}\right) = {\varepsilon }_{1},\sigma \left( {\varepsilon }_{2}\right) = \left( {0,1,0}\right) = {\varepsilon }_{2},\sigma \left( {\varepsilon }_{3}\right) = \left( {0,0,0}\right) = \mathbf{0},
$$

故 $\sigma$ 在这组基下的矩阵为 $\mathbf{A} = \left( \begin{array}{lll} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 0 \end{array}\right)$ .

例题 3.5. 在实线性空间 ${\mathbb{R}}_{n}\left\lbrack x\right\rbrack$ 中,取基 $1, x,{x}^{2},\cdots ,{x}^{n - 1}$ ,求微商变换 $\mathcal{D}$ 在这组基下的矩阵.

解 我们有

$$
\mathcal{D}\left( 1\right) = 0 = 0 \cdot 1 + {0x} + 0{x}^{2} + \cdots + 0{x}^{n - 1},
$$

$$
\mathcal{D}\left( x\right) = 1 = 1 \cdot 1 + {0x} + 0{x}^{2} + \cdots + 0{x}^{n - 1},
$$

$$
\mathcal{D}\left( {x}^{2}\right) = {2x} = 0 \cdot 1 + {2x} + 0{x}^{2} + \cdots + 0{x}^{n - 1},
$$

$\ldots$

$$
\mathcal{D}\left( {x}^{n - 1}\right) = \left( {n - 1}\right) {x}^{n - 2} = 0 \cdot 1 + {0x} + \cdots + \left( {n - 1}\right) {x}^{n - 2} + 0{x}^{n - 1}.
$$

所以, $\mathcal{D}$ 在这组基下的矩阵是

$$
\mathbf{A} = \left( \begin{matrix} 0 & 1 & & & \\ & 0 & 2 & & \\ & & 0 & \ddots & \\ & & & \ddots & n - 1 \\ & & & & 0 \end{matrix}\right) .
$$

定理 3.1. 设线性变换 $\sigma$ 在基 ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ 下的矩阵为 $A$ ,向量 $\alpha$ 在这组基下的坐标是 $\left( {{x}_{1},{x}_{2},\cdots ,{x}_{n}}\right)$ ,则 $\sigma \left( \mathbf{\alpha }\right)$ 在基 ${\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},\cdots ,{\mathbf{\varepsilon }}_{n}$ 下的坐标 $\left( {{y}_{1},{y}_{2},\cdots }\right.$ , $\left. {y}_{n}\right)$ 可以按下列公式

$$
\left( \begin{matrix} {y}_{1} \\ {y}_{2} \\ \vdots \\ {y}_{n} \end{matrix}\right) = \mathbf{A}\left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right)
$$

计算.

证明 由条件知,

$$
\mathbf{\alpha } = \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) \left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right)
$$

$$
\sigma \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) = \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) A
$$

所以

$$
\sigma \left( \mathbf{\alpha }\right) = \left( {\sigma \left( {\mathbf{\varepsilon }}_{1}\right) ,\sigma \left( {\mathbf{\varepsilon }}_{2}\right) ,\cdots ,\sigma \left( {\mathbf{\varepsilon }}_{n}\right) }\right) \left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right) = \left( {{\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},\cdots ,{\mathbf{\varepsilon }}_{n}}\right) \mathbf{A}\left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right) .
$$

另一方面, 由假设知

$$
\sigma \left( \mathbf{\alpha }\right) = \left( {{\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},\cdots ,{\mathbf{\varepsilon }}_{n}}\right) \left( \begin{matrix} {y}_{1} \\ {y}_{2} \\ \vdots \\ {y}_{n} \end{matrix}\right) .
$$

由于 ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ 线性无关,所以

$$
\left( \begin{matrix} {y}_{1} \\ {y}_{2} \\ \vdots \\ {y}_{n} \end{matrix}\right) = \mathbf{A}\left( \begin{matrix} {x}_{1} \\ {x}_{2} \\ \vdots \\ {x}_{n} \end{matrix}\right)
$$

例题 3.6. 设 $\mathcal{D}$ 是实线性空间 ${\mathbb{R}}_{n}\left\lbrack x\right\rbrack$ 的微商变换. 取基 $1, x,{x}^{2},\cdots ,{x}^{n - 1}$ , 则 $\mathcal{D}$ 在这组基下的矩阵 (参见例题 3.5) 为

$$
\mathbf{A} = \left( \begin{array}{lllll} 0 & 1 & & & \\ & 0 & 2 & & \\ & & 0 & \ddots & \\ & & & \ddots & n - 1 \\ & & & & 0 \end{array}\right) .
$$

取多项式 $f\left( x\right) = 1 + x + {x}^{2} + {x}^{3} + \cdots + {x}^{n - 1}$ ,则 $\mathcal{D}\left( {f\left( x\right) }\right)$ 在这组基下的坐标为

$$
\left( \begin{matrix} 0 & 1 & & & \\ & 0 & 2 & & \\ & & 0 & \ddots & \\ & & & \ddots & n - 1 \\ & & & & 0 \end{matrix}\right) \left( \begin{matrix} 1 \\ 1 \\ \vdots \\ 1 \\ 1 \end{matrix}\right) = \left( \begin{matrix} 1 \\ 2 \\ \vdots \\ n - 1 \\ 0 \end{matrix}\right) .
$$

因此, $\mathcal{D}\left( {f\left( x\right) }\right) = 1 + {2x} + 3{x}^{2} + \cdots + \left( {n - 1}\right) {x}^{n - 2}$ . 这显然与直接求微商的结果一致.

下面的定理给出了同一个线性变换在不同基下的矩阵间的联系.

定理 3.2. 设 $F$ 上的 $n$ 维线性空间的线性变换 $\sigma$ 在基 ${\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}$ 下的矩阵为 $\mathbf{A}$ ,在基 ${\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}$ 下的矩阵为 $\mathbf{B}$ ,且由基 ${\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},\cdots ,{\mathbf{\varepsilon }}_{n}$ 到基 ${\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}$ 的过渡矩阵为 $\mathbf{P}$ ,那么

$$
B = {P}^{-1}{AP}\text{.}
$$

证明 由条件知道,

$$
\sigma \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) = \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) A,
$$

$$
\sigma \left( {{\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}}\right) = \left( {{\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}}\right) \mathbf{B},
$$

$$
\left( {{\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}}\right) = \left( {{\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},\cdots ,{\mathbf{\varepsilon }}_{n}}\right) \mathbf{P},
$$

于是

$$
\sigma \left( {{\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}}\right) = \sigma \left\lbrack {\left( {{\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},\cdots ,{\mathbf{\varepsilon }}_{n}}\right) \mathbf{P}}\right\rbrack = \left\lbrack {\sigma \left( {{\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},\cdots ,{\mathbf{\varepsilon }}_{n}}\right) }\right\rbrack \mathbf{P}
$$

$$
= \left( {{\varepsilon }_{1},{\varepsilon }_{2},\cdots ,{\varepsilon }_{n}}\right) \mathbf{{AP}} = \left( {{\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}}\right) {\mathbf{P}}^{-1}\mathbf{{AP}}.
$$

因为线性变换 $\sigma$ 在基 ${\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},\cdots ,{\mathbf{\eta }}_{n}$ 下的矩阵唯一确定,所以 $\mathbf{B} = {\mathbf{P}}^{-1}\mathbf{A}\mathbf{P}$ .

定理表明, $n$ 维线性空间的同一个线性变换在不同基下的矩阵是相似的.

例题 3.7. 设 $V$ 为实数域上的三维线性空间, ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 和 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 都是 $V$ 的基,并且

$$
{\mathbf{\beta }}_{1} = {\mathbf{\alpha }}_{1} + {\mathbf{\alpha }}_{2} + {\mathbf{\alpha }}_{3}
$$

$$
{\beta }_{2} = \frac{1}{5}{\alpha }_{1} + \frac{1}{5}{\alpha }_{2}
$$

$$
{\beta }_{3} = {\alpha }_{2} + {\alpha }_{3}
$$

今设 $\sigma$ 是 $V$ 的一个线性变换. 设 $\sigma$ 在基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 下的矩阵为

$$
\mathbf{A} = \left( \begin{array}{rrr} 1 & - 2 & 2 \\ 2 & 2 & - 3 \\ 2 & 3 & - 4 \end{array}\right)
$$

求 $\sigma$ 在基 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 下的矩阵.

解 设 $\sigma$ 在基 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 下的矩阵为 $\mathbf{B}$ . 基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3}$ 到基 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3}$ 的过

渡矩阵为

$$
\mathbf{P} = \left( \begin{array}{lll} 1 & \frac{1}{5} & 0 \\ 1 & \frac{1}{5} & 1 \\ 1 & 0 & 1 \end{array}\right)
$$

于是

$$
\mathbf{B} = {\mathbf{P}}^{-1}\mathbf{A}\mathbf{P} = \left( \begin{array}{rrr} 1 & 0 & 0 \\ 0 & - 1 & 0 \\ 0 & 1 & - 1 \end{array}\right)
$$

由此可知, $\sigma \left( {\mathbf{\beta }}_{1}\right) = {\mathbf{\beta }}_{1},\sigma \left( {\mathbf{\beta }}_{2}\right) = - {\mathbf{\beta }}_{2} + {\mathbf{\beta }}_{3},\sigma \left( {\mathbf{\beta }}_{3}\right) = - {\mathbf{\beta }}_{3}$ .

## 习 题 七

1. 讨论下列集合对于所给的线性运算是否构成线性空间:

(1) 实数域上的全体 $n$ 阶对称 (反称,上三角形) 矩阵,对于矩阵的加法和数乘;

(2) 实数域上的全体 $n$ 维向量,关于通常的向量加法和如下定义的数乘:

$$
k \cdot \alpha = \alpha
$$

(3) $V = \left\{ {\left( {{x}_{1},{x}_{2}}\right) \mid {x}_{1},{x}_{2} \in \mathbb{R}}\right\}$ ,关于下述定义的加法和数乘:

$$
\left( {{x}_{1},{x}_{2}}\right) \oplus \left( {{y}_{1},{y}_{2}}\right) = \left( {{x}_{1} + {y}_{1},{x}_{2} + {y}_{2}}\right)
$$

$$
k \odot \left( {{x}_{1},{x}_{2}}\right) = \left( {k{x}_{1}, k{x}_{2} + \frac{k\left( {k - 1}\right) }{2}{x}_{1}^{2}}\right) .
$$

2. 在 ${\mathbb{R}}^{4}$ 中,求向量 $\mathbf{\beta }$ 在基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 下的坐标,其中

(1) $\begin{cases} {\mathbf{\alpha }}_{1} & = \left( {1,1,1,1}\right) , \\ {\mathbf{\alpha }}_{2} & = \left( {1,1, - 1, - 1}\right) , \\ {\mathbf{\alpha }}_{3} & = \left( {1, - 1,1, - 1}\right) , \\ {\mathbf{\alpha }}_{4} & = \left( {1, - 1, - 1,1}\right) , \\ \mathbf{\beta } & = \left( {1,2,1,1}\right) ; \end{cases}$ (2) $\begin{cases} {\mathbf{\alpha }}_{1} & = \left( {1,1,0,1}\right) , \\ {\mathbf{\alpha }}_{2} & = \left( {2,1,3,1}\right) , \\ {\mathbf{\alpha }}_{3} & = \left( {1,1,0,0}\right) , \\ {\mathbf{\alpha }}_{4} & = \left( {0,1, - 1, - 1}\right) , \\ \mathbf{\beta } & = \left( {0,0,0,1}\right) . \end{cases}$

3. 在 ${\mathbb{R}}^{4}$ 中,求下列基 ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 到基 ${\mathbf{\beta }}_{1},{\mathbf{\beta }}_{2},{\mathbf{\beta }}_{3},{\mathbf{\beta }}_{4}$ 的过渡矩阵:

(1) ${\mathbf{\alpha }}_{1},{\mathbf{\alpha }}_{2},{\mathbf{\alpha }}_{3},{\mathbf{\alpha }}_{4}$ 为标准单位向量, $\left\{ \begin{array}{l} {\mathbf{\beta }}_{1} = \left( {2,1, - 1,1}\right) , \\ {\mathbf{\beta }}_{2} = \left( {0,3,1,0}\right) , \\ {\mathbf{\beta }}_{3} = \left( {5,3,2,1}\right) , \\ {\mathbf{\beta }}_{4} = \left( {6,6,1,3}\right) ; \end{array}\right.$

(2) $\left\{ {\begin{array}{l} {\mathbf{\alpha }}_{1} = \left( {1,2, - 1,0}\right) , \\ {\mathbf{\alpha }}_{2} = \left( {1, - 1,1,1}\right) , \\ {\mathbf{\alpha }}_{3} = \left( {-1,2,1,1}\right) , \\ {\mathbf{\alpha }}_{4} = \left( {-1, - 1,0,1}\right) . \end{array}\;\left\{ \begin{array}{l} {\mathbf{\beta }}_{1} = \left( {2,1,0,1}\right) , \\ {\mathbf{\beta }}_{2} = \left( {0,1,2,2}\right) , \\ {\mathbf{\beta }}_{3} = \left( {-2,1,1,2}\right) , \\ {\mathbf{\beta }}_{4} = \left( {1,3,1,2}\right) . \end{array}\right. }\right.$

4. 设 $V = {M}_{nn}\left( F\right)$ 表示由 $F$ 上全部 $n \times n$ 矩阵所组成的线性空间, $\mathbf{A}$ 为一个 $n \times n$ 矩阵.

(1) 变换 $\sigma \left( \mathbf{X}\right) = \mathbf{A}\mathbf{X},\mathbf{X} \in V$ 是不是 $V$ 的线性变换?

(2) 设又有 $n \times n$ 矩阵 $\mathbf{B}$ . 变换 $\tau \left( \mathbf{X}\right) = \mathbf{A}\mathbf{X}\mathbf{B},\mathbf{X} \in V$ 是不是 $V$ 的线性变换?

5. 设 $V,\mathbf{A}$ 和 $\sigma$ 的定义由上题给出,但 $n = 2$ . 令

$$
\mathbf{A} = \left( \begin{array}{ll} {a}_{11} & {a}_{12} \\ {a}_{21} & {a}_{22} \end{array}\right)
$$

求线性变换 $\sigma$ 在基 ${\mathbf{E}}_{11},{\mathbf{E}}_{12},{\mathbf{E}}_{21},{\mathbf{E}}_{22}$ 下的矩阵,其中

$$
{\mathbf{E}}_{11} = \left( \begin{array}{ll} 1 & 0 \\ 0 & 0 \end{array}\right) ,{\mathbf{E}}_{12} = \left( \begin{array}{ll} 0 & 1 \\ 0 & 0 \end{array}\right) ,{\mathbf{E}}_{21} = \left( \begin{array}{ll} 0 & 0 \\ 1 & 0 \end{array}\right) ,{\mathbf{E}}_{22} = \left( \begin{array}{ll} 0 & 0 \\ 0 & 1 \end{array}\right) .
$$

6. 已知三维空间 $V$ 的线性变换 $\sigma$ 在基 ${\varepsilon }_{1},{\varepsilon }_{2},{\varepsilon }_{3}$ 下的矩阵为

$$
A = \left( \begin{array}{lll} {a}_{11} & {a}_{12} & {a}_{13} \\ {a}_{21} & {a}_{22} & {a}_{23} \\ {a}_{31} & {a}_{32} & {a}_{33} \end{array}\right)
$$

(1) 求 $\sigma$ 在基 ${\varepsilon }_{3},{\varepsilon }_{1},{\varepsilon }_{2}$ 下的矩阵;

(2) 求 $\sigma$ 在基 ${\varepsilon }_{1},5{\varepsilon }_{2}, - 6{\varepsilon }_{3}$ 下的矩阵;

(3) 求 $\sigma$ 在基 ${\varepsilon }_{1} + {\varepsilon }_{2},{\varepsilon }_{2},{\varepsilon }_{3}$ 下的矩阵.

7. 设 $V = {F}_{n}\left\lbrack x\right\rbrack$ 表示数域 $F$ 上的由次数小于 $n$ 的多项式及零多项式组成的线性空间, 在 $V$ 内取基

$$
1, x,\frac{1}{2}{x}^{2},\cdots ,\frac{1}{n - 1}{x}^{n - 1}
$$

求微分变换 $\mathcal{D}$ 在此基下的矩阵.

8. 在三维线性空间 $V$ 中给定了线性变换 $\sigma$ 在基 ${\varepsilon }_{1},{\varepsilon }_{2},{\varepsilon }_{3}$ 下的矩阵为

$$
A = \left( \begin{array}{rrr} - 5 & 9 & 4 \\ - 6 & {11} & 5 \\ 7 & - {13} & - 6 \end{array}\right)
$$

另一组基 ${\eta }_{1},{\eta }_{2},{\eta }_{3}$ 与 ${\varepsilon }_{1},{\varepsilon }_{2},{\varepsilon }_{3}$ 的关系为

$$
\left\{ \begin{array}{l} {\eta }_{1} = 9{\varepsilon }_{1} + 3{\varepsilon }_{2} + 4{\varepsilon }_{3} \\ {\eta }_{2} = 2{\varepsilon }_{1} + {\varepsilon }_{2} \\ {\eta }_{3} = {\varepsilon }_{1} + {\varepsilon }_{2} - {\varepsilon }_{3} \end{array}\right.
$$

(1) 求 $\sigma$ 在基 ${\eta }_{1},{\eta }_{2},{\eta }_{3}$ 下的矩阵;

(2) 又设 $\mathbf{\alpha }$ 在基 ${\mathbf{\varepsilon }}_{1},{\mathbf{\varepsilon }}_{2},{\mathbf{\varepsilon }}_{3}$ 下的坐标为 $\left( {1,1,1}\right)$ ,求向量 $\mathbf{\alpha }$ 在基 ${\mathbf{\eta }}_{1},{\mathbf{\eta }}_{2},{\mathbf{\eta }}_{3}$ 下的坐标.

9. 设 $\sigma$ 为 ${\mathbb{R}}^{3}$ 的一个线性变换,已知 $\sigma$ 在标准单位向量 ${\varepsilon }_{1},{\varepsilon }_{2},{\varepsilon }_{3}$ 下的矩阵为

$$
A = \left( \begin{array}{rrr} 0 & 2 & 6 \\ - 1 & 0 & 3 \\ 1 & - 1 & 2 \end{array}\right)
$$

求 $\sigma$ 在基 ${\mathbf{\alpha }}_{1} = {\mathbf{\varepsilon }}_{1},{\mathbf{\alpha }}_{2} = {\mathbf{\varepsilon }}_{1} + {\mathbf{\varepsilon }}_{2},{\mathbf{\alpha }}_{3} = {\mathbf{\varepsilon }}_{1} + {\mathbf{\varepsilon }}_{2} + {\mathbf{\varepsilon }}_{3}$ 下的矩阵.

10. 设 $\sigma$ 是 $n$ 维线性空间 $V$ 的线性变换, $\alpha \in V$ ,若 $\alpha ,\sigma \left( \alpha \right) ,{\sigma }^{2}\left( \alpha \right) ,\cdots ,{\sigma }^{k - 1}\left( \alpha \right)$ 都不是零向量,但 ${\sigma }^{k}\left( \mathbf{\alpha }\right) = \mathbf{0}$ . 证明: $\mathbf{\alpha },\sigma \left( \mathbf{\alpha }\right) ,{\sigma }^{2}\left( \mathbf{\alpha }\right) ,\cdots ,{\sigma }^{k - 1}\left( \mathbf{\alpha }\right) \left( {k \geq 1}\right)$ 线性无关.