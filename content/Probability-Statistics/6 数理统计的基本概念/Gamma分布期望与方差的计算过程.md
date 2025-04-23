Gamma分布的概率密度函数（PDF）为：
$$f(x) = \frac{\beta^\alpha}{\Gamma(\alpha)} x^{\alpha-1} e^{-\beta x} \quad (x \geq 0)$$
其中：

- $\alpha > 0$ 为**形状参数**
- $\beta > 0$ 为**速率参数**
- $\Gamma(\alpha)$ 是Gamma函数

### 一、期望（均值）的计算

$$\mathbb{E}[X] = \int_0^\infty x \cdot f(x) \, dx$$

**详细步骤：**

1. 代入PDF：
$$
\mathbb{E}[X] = \frac{\beta^\alpha}{\Gamma(\alpha)} \int_0^\infty x^{\alpha} e^{-\beta x} \, dx
$$
2. 变量替换 $t = \beta x$，则 $x = t/\beta$，$dx = dt/\beta$：
$$
\int_0^\infty \left(\frac{t}{\beta}\right)^\alpha e^{-t} \cdot \frac{dt}{\beta} = \frac{1}{\beta^{\alpha+1}} \int_0^\infty t^\alpha e^{-t} dt
$$
3. 利用Gamma函数定义 $\Gamma(n) = \int_0^\infty t^{n-1} e^{-t} dt$：
$$
\int_0^\infty t^\alpha e^{-t} dt = \Gamma(\alpha+1)
$$
4. 化简得：
$$
\mathbb{E}[X] = \frac{\beta^\alpha}{\Gamma(\alpha)} \cdot \frac{\Gamma(\alpha+1)}{\beta^{\alpha+1}} = \frac{\alpha}{\beta}
$$

**结论：**
$$\mathbb{E}[X] = \frac{\alpha}{\beta}$$

### 二、方差的计算

$\text{Var}[X] = \mathbb{E}[X^2] - (\mathbb{E}[X])^2$

**步骤1：计算 $\mathbb{E}[X^2]$**
$$
\mathbb{E}[X^2] = \frac{\beta^\alpha}{\Gamma(\alpha)} \int_0^\infty x^{\alpha+1} e^{-\beta x} dx
$$

1. 变量替换 $t = \beta x$，类似期望计算：
$$
\mathbb{E}[X^2] = \frac{\beta^\alpha}{\Gamma(\alpha)} \cdot \frac{\Gamma(\alpha+2)}{\beta^{\alpha+2}} = \frac{\Gamma(\alpha+2)}{\Gamma(\alpha) \beta^2}
$$
2. 利用Gamma函数性质 $\Gamma(\alpha+2) = (\alpha+1)\alpha \Gamma(\alpha)$：
$$
\mathbb{E}[X^2] = \frac{(\alpha+1)\alpha}{\beta^2}
$$

**步骤2：计算方差**
$$
\text{Var}[X] = \frac{(\alpha+1)\alpha}{\beta^2} - \left(\frac{\alpha}{\beta}\right)^2 = \frac{\alpha}{\beta^2}
$$

**结论：**
$$\text{Var}[X] = \frac{\alpha}{\beta^2}$$

### 三、关键公式总结

| 参数化方式                  | 期望                     | 方差                       |
| :--------------------- | :--------------------- | :----------------------- |
| 形状 $\alpha$，速率 $\beta$ | $\frac{\alpha}{\beta}$ | $\frac{\alpha}{\beta^2}$ |
| 形状 $k$，尺度 $\theta$     | $k\theta$              | $k\theta^2$              |

Gamma函数性质：$\Gamma(\alpha+1) = \alpha \Gamma(\alpha)$
变量替换技巧：积分时通过 $t = \beta x$ 标准化积分区间。