## 1. 引言

在概率论中，我们经常需要研究随机变量序列的收敛性。依概率收敛和以概率为一收敛是两种重要的收敛方式。本讲义将通过直观的例子，帮助大家理解这两种收敛方式的区别与联系。

## 2. 定义

设 $(X_n)_{n=1}^\infty$ 是定义在概率空间 $(\Omega, \mathcal{F}, P)$ 上的一列随机变量，$X$ 是定义在同一概率空间上的一个随机变量。

### 2.1 依概率收敛 (Convergence in Probability)

随机变量序列 $(X_n)$ 依概率收敛到 $X$，记为 $X_n \xrightarrow{P} X$，如果对于任意 $\epsilon > 0$，都有：
$$
\lim_{n \to \infty} P(|X_n - X| > \epsilon) = 0
$$

直观理解：当 $n$ 足够大时，$X_n$ 与 $X$ 的偏差超过任意给定的正数 $\epsilon$ 的概率趋近于零。也就是说，$X_n$ 很可能接近 $X$。

### 2.2 以概率为一收敛 (Convergence with Probability One / Almost Sure Convergence)

随机变量序列 $(X_n)$ 以概率为一收敛到 $X$，记为 $X_n \xrightarrow{a.s.} X$，如果：
$$
P(\{\omega \in \Omega : \lim_{n \to \infty} X_n(\omega) = X(\omega)\}) = 1
$$

这等价于：对于任意 $\epsilon > 0$，
$$
P(\bigcup_{m=n}^\infty \{|X_m - X| > \epsilon\} \text{ for some } n) = \lim_{n \to \infty} P(\bigcup_{m=n}^\infty \{|X_m - X| > \epsilon\}) = 0
$$

直观理解：以概率为一收敛意味着，除了一个概率为零的事件外，对于样本空间 $\Omega$ 中的每一个 $\omega$，随机变量序列 $X_n(\omega)$ 都收敛到 $X(\omega)$。也就是说，$X_n$ 最终会稳定在 $X$ 附近。

## 3. 直观例子比较

### 3.1 例子 1：硬币游戏

考虑一个无限次抛掷均匀硬币的实验。
设 $Z_i$ 是第 $i$ 次抛掷的结果，当正面朝上时 $Z_i = 1$，反面朝上时 $Z_i = 0$，$P(Z_i = 1) = P(Z_i = 0) = 1/2$，且每次抛掷相互独立。

定义随机变量序列 $X_n$ 如下：
$$
X_n = \begin{cases}
1 & \text{如果前 } n \text{ 次抛掷都是正面 (即 } Z_1 = Z_2 = \dots = Z_n = 1) \\
0 & \text{否则}
\end{cases}
$$

我们来分析 $X_n$ 的收敛性。

* **以概率为一收敛:**
    事件 $\{\omega : \lim_{n \to \infty} X_n(\omega) = 0\}$ 包含了所有不是无限次正面朝上的情况。无限次正面朝上的概率是 $\lim_{n \to \infty} (1/2)^n = 0$。因此，$P(\lim_{n \to \infty} X_n = 0) = 1$，所以 $X_n \xrightarrow{a.s.} 0$。

* **依概率收敛:**
    对于任意 $\epsilon > 0$ (不妨设 $0 < \epsilon \le 1$)，
    $$
    P(|X_n - 0| > \epsilon) = P(X_n = 1) = (1/2)^n
    $$
    因此，$\lim_{n \to \infty} P(|X_n - 0| > \epsilon) = \lim_{n \to \infty} (1/2)^n = 0$。所以 $X_n \xrightarrow{P} 0$。

在这个例子中，依概率收敛和以概率为一收敛都成立，且极限都是 0。

### 3.2 例子 2：闪烁的指示灯

考虑一个随机过程，在每个时刻 $n = 1, 2, \dots$，一个指示灯以概率 $1/n$ 亮起，以概率 $1 - 1/n$ 关闭。
设 $X_n$ 是指示灯在时刻 $n$ 的状态，
- $X_n = 1$ 表示亮起，
- $X_n = 0$ 表示关闭。

假设不同时刻的状态相互独立。
我们来分析 $Y_n := X_n$ 的收敛性到 $X = 0$。

* **依概率收敛:**
    对于任意 $\epsilon \in (0, 1]$，
    $$
    P(|X_n - 0| > \epsilon) = P(Y_n = 1) = \frac{1}{n}
    $$
    因此，$\lim_{n \to \infty} P(|X_n - 0| > \epsilon) = \lim_{n \to \infty} \frac{1}{n} = 0$。所以 $X_n \xrightarrow{P} 0$。

* **以概率为一收敛:**
    我们考虑事件 $\{\omega : \lim_{n \to \infty} X_n(\omega) = 0\}$。这等价于指示灯最终总是关闭。考虑指示灯无限次亮起的事件 $A = \bigcap_{n=1}^\infty \bigcup_{m=n}^\infty \{Y_m = 1\}$。
    $$
    P(\bigcup_{m=n}^\infty \{Y_m = 1\}) \le \sum_{m=n}^\infty P(Y_m = 1) = \sum_{m=n}^\infty \frac{1}{m}
    $$
    由于调和级数 $\sum_{m=1}^\infty \frac{1}{m}$ 发散，所以 $\lim_{n \to \infty} \sum_{m=n}^\infty \frac{1}{m} = \infty$。这个上界没有提供有用的信息。

    我们考虑不收敛到 0 的事件，即 $B = \{\omega : \limsup_{n \to \infty} Y_n(\omega) = 1\}$，表示指示灯无限次亮起。
    $$
    P(B) = P(\bigcap_{n=1}^\infty \bigcup_{m=n}^\infty \{Y_m = 1\})
    $$
    由于事件 $\{Y_m = 1\}$ 相互独立，且 $\sum_{m=1}^\infty P(Y_m = 1) = \sum_{m=1}^\infty \frac{1}{m} = \infty$，根据 [[Borel-Cantelli 引理]]，我们有 $P(B) = 1$。
    这意味着指示灯以概率 1 无限次亮起，所以 $P(\lim_{n \to \infty} Y_n = 0) = 0$。因此，$X_n$ 不以概率为一收敛到 0。

这个例子表明，依概率收敛不能保证以概率为一收敛。
即使 $X_n$ 在每个时刻都很有可能接近 0，但仍然有可能在无限长的时间内发生无穷多次偏离 0 的情况。

### 3.3 例子 3：区间上的随机点

设 $\Omega = [0, 1]$，概率测度为勒贝格测度。定义随机变量序列 $X_n$ 如下：

对于 $n = 1, 2, \dots$，设 $n = 2^k + j$，其中 $0 \le j < 2^k$。定义：
$$
X_n(\omega) = \begin{cases}
1 & \text{如果 } \omega \in [j/2^k, (j+1)/2^k) \\
0 & \text{否则}
\end{cases}
$$

这个序列依次覆盖区间 $[0, 1)$：
$[0, 1)$, $[0, 1/2)$, $[1/2, 1)$, $[0, 1/4)$, $[1/4, 2/4)$, $[2/4, 3/4)$, $[3/4, 1)$, $\dots$

* **依概率收敛:**
    对于任意 $\epsilon > 0$ (不妨设 $0 < \epsilon \le 1$)，
    $$
P(|X_n - 0| > \epsilon) = P(X_n = 1) = \text{区间 } [j/2^k, (j+1)/2^k) \text{ 的长度} = \frac{1}{2^k}
$$
    当 $n \to \infty$ 时，$k \to \infty$，所以 $\lim_{n \to \infty} P(|X_n - 0| > \epsilon) = 0$。因此，$X_n \xrightarrow{P} 0$。

* **以概率为一收敛:**
    对于任意 $\omega \in [0, 1)$，序列 $X_n(\omega)$ 会无限次地取值为 1 (当 $\omega$ 落在越来越小的区间内) 和 0 (当 $\omega$ 不在当前考虑的区间内)。因此，对于任何 $\omega \in [0, 1)$，$\lim_{n \to \infty} X_n(\omega)$ 不存在（或者说不等于 0）。
    所以，$P(\{\omega : \lim_{n \to \infty} X_n(\omega) = 0\}) = 0$。因此，$X_n$ 不以概率为一收敛到 0。

这个例子进一步说明了依概率收敛比以概率为一收敛弱。
序列可以依概率收敛到某个值，但对于每个具体的样本点，序列的极限可能并不存在或不等于该值。

## 4. 依概率为一收敛蕴含依概率收敛

如果 $X_n \xrightarrow{a.s.} X$，那么 $X_n \xrightarrow{P} X$。

### 证明思路
对于任意 $\epsilon > 0$，事件 $\{\lim_{n \to \infty} X_n = X\}$ 的补集是 
$$
\begin{align}
&\left\{\limsup_{n \to \infty} |X_n - X| > 0\right\} \\
&= \bigcup_{k=1}^\infty \bigcap_{n=1}^\infty \bigcup_{m=n}^\infty \left\{|X_m - X| > 1/k\right\}.
\end{align}
$$
由于 $X_n \xrightarrow{a.s.} X$，所以 $P(\{\lim_{n \to \infty} X_n = X\}) = 1$，因此 
$$P(\{\limsup_{n \to \infty} |X_n - X| > 0\}) = 0.$$
对于固定的 $\epsilon > 0$，
$$\bigcup_{m=n}^\infty \{|X_m - X| > \epsilon\} \subseteq \{\sup_{m \ge n} |X_m - X| > \epsilon\}.$$
$$
\begin{align}
\lim_{n \to \infty} P\left(\sup_{m \ge n} |X_m - X| > \epsilon\right) &= P\left(\bigcap_{n=1}^\infty \left\{\sup_{m \ge n} |X_m - X| > \epsilon\right\}\right) \\
&= P\left(\left\{\limsup_{n \to \infty} |X_n - X| > \epsilon\right\}\right) \\
&\le P\left(\left\{\limsup_{n \to \infty} |X_n - X| > 0\right\}\right) \\
&= 0
\end{align}
$$
所以 $\lim_{n \to \infty} P(\sup_{m \ge n} |X_n - X| > \epsilon) = 0$，进而 
$$\lim_{n \to \infty} P(|X_n - X| > \epsilon) = 0.$$

## 5. 总结

* **依概率收敛** 关注的是对于任意给定的偏差 $\epsilon$，当 $n$ 足够大时，$X_n$ 与 $X$ 的偏差超过 $\epsilon$ 的概率很小。允许在不同的样本点 $\omega$ 上，序列不收敛或收敛到不同的值，只要这些情况发生的概率趋于零。
* **以概率为一收敛** 要求对于几乎所有的样本点 $\omega$，序列 $X_n(\omega)$ 都收敛到 $X(\omega)$。这是一种更强的收敛方式，要求序列在样本空间的大部分地方都具有逐点收敛的性质。

以概率为一收敛蕴含依概率收敛，但反之不成立。例子 2 和例子 3 都说明了这一点。理解这两种收敛方式的区别对于深入学习概率论和随机过程至关重要。

## 6. 思考题

1.  你能否构造一个随机变量序列 $X_n$ 依概率收敛到 0，但 $E[X_n]$ 不收敛到 $E[0] = 0$ 吗？
2.  如果随机变量序列 $X_n$ 以概率为一收敛到常数 $c$，那么 $X_n$ 是否也依分布收敛到常数 $c$？反之成立吗？

希望本次讲义能够帮助大家更好地理解依概率收敛和以概率为一收敛的区别。