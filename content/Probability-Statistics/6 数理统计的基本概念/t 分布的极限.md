## 证明：当 $n \to \infty$ 时，$t(n)$ 分布渐近于 $N(0,1)$

### 1. $t$ 分布的定义

自由度为 $n$ 的 $t$ 分布可以表示为
$$
T_n = \frac{Z}{\sqrt{Y/n}}
$$
其中 $Z \sim N(0,1)$，$Y \sim \chi^2(n)$，且 $Z$ 与 $Y$ 独立。[3][4]

### 2. 利用大数定律和Slutsky定理

- 由大数定律，$\frac{Y}{n} \xrightarrow{P} 1$，即当 $n \to \infty$ 时，$\chi^2(n)/n$ 以概率收敛到 $1$。[3][4]
- 因此，$\sqrt{Y/n} \xrightarrow{P} 1$。
- $Z \sim N(0,1)$，与 $Y$ 独立。

由 Slutsky 定理，若 $A_n \xrightarrow{d} A$，$B_n \xrightarrow{P} b$，则 $A_n/B_n \xrightarrow{d} A/b$。因此，
$$
T_n = \frac{Z}{\sqrt{Y/n}} \xrightarrow{d} N(0,1)
$$
即 $t$ 分布在自由度 $n \to \infty$ 时，趋于标准正态分布。[3][4]

### 3. 密度函数极限法（严格证明）

$t$ 分布的概率密度函数为
$$
f_n(x) = \frac{\Gamma\left(\frac{n+1}{2}\right)}{\sqrt{n\pi}\,\Gamma\left(\frac{n}{2}\right)}\left(1+\frac{x^2}{n}\right)^{-\frac{n+1}{2}}
$$

分析 $n \to \infty$ 时的极限：

- 利用
  $$
  \lim_{n\to\infty} \left(1+\frac{x^2}{n}\right)^{-n/2} = e^{-x^2/2}
  $$
- 斯特林公式可证
  $$
  \lim_{n\to\infty} \frac{\Gamma\left(\frac{n+1}{2}\right)}{\sqrt{n\pi}\,\Gamma\left(\frac{n}{2}\right)} = \frac{1}{\sqrt{2\pi}}
  $$

因此，
$$
\lim_{n\to\infty} f_n(x) = \frac{1}{\sqrt{2\pi}} e^{-x^2/2}
$$
即为标准正态分布的密度函数。[1][4]

### 4. 直观解释

$t$ 分布的“厚尾”随着自由度 $n$ 增大而变薄，最终与标准正态分布重合。这说明在样本量足够大时，$t$ 检验与正态检验结果一致。[3]

**结论：**
$$
t(n) \xrightarrow{d} N(0,1) \quad (n \to \infty)
$$
即自由度趋于无穷时，$t$ 分布收敛于标准正态分布。