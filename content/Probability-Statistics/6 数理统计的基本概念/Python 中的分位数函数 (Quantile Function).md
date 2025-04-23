## 常见的分位数类型

根据 $p$ 的取值，分位数有一些常见的名称：

* **中位数 (Median)**: $p=0.5$ 时的分位数，$Q(0.5)$。它将数据分为数量相等的两部分。
* **四分位数 (Quartiles)**:
    * 第一四分位数 (Lower Quartile, Q1): $p=0.25$ 时的分位数，$Q(0.25)$。
    * 第三四分位数 (Upper Quartile, Q3): $p=0.75$ 时的分位数，$Q(0.75)$。
    * 四分位数将数据分为数量相等的四部分。Q1, Median (Q2), Q3 是分割点。
* **百分位数 (Percentiles)**: 将 $p$ 乘以 100 得到百分比。例如，第 90 百分位数是 $p=0.90$ 时的分位数，$Q(0.90)$。
* **十分位数 (Deciles)**: 将数据分为十等份的分位数，$Q(0.1), Q(0.2), \dots, Q(0.9)$。

## 样本分位数的计算

在实际应用中，我们通常处理的是一组有限的**样本数据** $x_1, x_2, \dots, x_n$，而不是理论上的概率分布。计算样本分位数需要先对数据进行排序，得到有序样本 $x_{(1)} \le x_{(2)} \le \dots \le x_{(n)}$。

计算样本分位数并没有一个绝对统一的标准，不同的统计软件或库可能采用不同的**插值方法 (Interpolation Methods)**，尤其是在 $p(n-1)$ 不是整数时。

一种最常见的方法是**线性插值 (Linear Interpolation)**，这也是 NumPy 和 Pandas 库的默认方法。其计算步骤如下 (使用 0-based 索引，即 $x_{(0)}, x_{(1)}, \dots, x_{(n-1)}$)：

1.  计算索引值：$k = p \times (n - 1)$。
2.  将 $k$ 分解为整数部分 $i = \lfloor k \rfloor$ 和小数部分 $f = k - i$。
3.  如果 $f=0$ (即 $k$ 是整数)，则 $p$-分位数就是 $x_{(i)}$。
4.  如果 $f>0$，则 $p$-分位数通过 $x_{(i)}$ 和 $x_{(i+1)}$ 进行线性插值得到：
    $$ q_p = x_{(i)} + f \times (x_{(i+1)} - x_{(i)}) $$
    也可以写成：
    $$ q_p = (1 - f) x_{(i)} + f x_{(i+1)} $$

除了线性插值，还有其他方法，如：

* `lower`: $x_{(i)}$
* `higher`: $x_{(i+1)}$
* `nearest`: $x_{(i)}$ 或 $x_{(i+1)}$ 中离 $k$ 更近的索引对应的点。
* `midpoint`: $(x_{(i)} + x_{(i+1)}) / 2$

选择哪种方法取决于具体的应用场景和约定。

## Python 实现

Python 中计算分位数主要使用 NumPy 和 Pandas 库。

### NumPy

NumPy 提供了 `numpy.quantile()` 和 `numpy.percentile()` 函数。`percentile` 的计算方式与 `quantile` 相同，只是输入参数为 0-100 的百分数而不是 0-1 的概率。

```python
import numpy as np

# 示例数据
data = np.array([1, 3, 2, 5, 4, 7, 6, 9, 8, 10])

# 计算中位数 (p=0.5)
median = np.quantile(data, 0.5)
print(f"Median (p=0.5): {median}") # 输出: Median (p=0.5): 5.5

# 计算第一和第三四分位数 (Q1: p=0.25, Q3: p=0.75)
q1 = np.quantile(data, 0.25)
q3 = np.quantile(data, 0.75)
print(f"Q1 (p=0.25): {q1}")   # 输出: Q1 (p=0.25): 3.25
print(f"Q3 (p=0.75): {q3}")   # 输出: Q3 (p=0.75): 7.75

# 同时计算多个分位数
quantiles = np.quantile(data, [0.1, 0.5, 0.9])
print(f"Quantiles (p=0.1, 0.5, 0.9): {quantiles}") # 输出: Quantiles (p=0.1, 0.5, 0.9): [1.9 5.5 9.1]

# 使用不同的插值方法
# 'lower' 插值计算 Q1
q1_lower = np.quantile(data, 0.25, method='lower') # NumPy 1.22 之后使用 'method'，之前使用 'interpolation'
print(f"Q1 (p=0.25, method='lower'): {q1_lower}") # 输出: Q1 (p=0.25, method='lower'): 3

# 解释 Q1 (p=0.25, method='linear') 的计算:
# 排序后数据: [ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10] (n=10)
# 索引 (0-based): 0,  1,  2,  3,  4,  5,  6,  7,  8,  9
# k = p * (n - 1) = 0.25 * (10 - 1) = 0.25 * 9 = 2.25
# i = floor(k) = 2
# f = k - i = 0.25
# q_p = x_(i) + f * (x_(i+1) - x_(i))
# q_0.25 = data[2] + 0.25 * (data[3] - data[2])
# q_0.25 = 3 + 0.25 * (4 - 3) = 3 + 0.25 * 1 = 3.25

# 'lower' 插值: q_p = x_(i) = data[2] = 3
````

**`numpy.quantile()` 主要参数：**

- `a`: 输入数组。
- `q`: 需要计算的分位数，介于 0 和 1 之间（可以是一个数值或列表/数组）。
- `axis`: 计算分位数的轴。默认是在扁平化后的数组上计算。
- `method` (NumPy >= 1.22) 或 `interpolation` (NumPy < 1.22): 插值方法，默认为 `'linear'`。可选值包括 `'lower'`, `'higher'`, `'midpoint'`, `'nearest'`。

### Pandas

Pandas 的 Series 和 DataFrame 对象也有 `quantile()` 方法，用法与 NumPy 类似。

Python

```
import pandas as pd

# 使用 Pandas Series
data_series = pd.Series([1, 3, 2, 5, 4, 7, 6, 9, 8, 10])

# 计算中位数
median_pd = data_series.quantile(0.5)
print(f"Pandas Series Median: {median_pd}") # 输出: Pandas Series Median: 5.5

# 计算 Q1 和 Q3
q1_pd = data_series.quantile(0.25)
q3_pd = data_series.quantile(0.75)
print(f"Pandas Series Q1: {q1_pd}") # 输出: Pandas Series Q1: 3.25
print(f"Pandas Series Q3: {q3_pd}") # 输出: Pandas Series Q3: 7.75

# 使用不同的插值方法
q1_lower_pd = data_series.quantile(0.25, interpolation='lower')
print(f"Pandas Series Q1 (interpolation='lower'): {q1_lower_pd}") # 输出: Pandas Series Q1 (interpolation='lower'): 3

# 使用 Pandas DataFrame
df = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [10, 20, 5, 15, 25]})
print("\nDataFrame:")
print(df)

# 计算每列的 0.5 分位数 (中位数)
median_df = df.quantile(0.5) # 默认 axis=0 (按列计算)
print("\nDataFrame Median (axis=0):")
print(median_df)
# 输出:
# DataFrame Median (axis=0):
# A     3.0
# B    15.0
# Name: 0.5, dtype: float64

# 计算每行的 0.5 分位数 (中位数)
median_df_rows = df.quantile(0.5, axis=1)
print("\nDataFrame Median (axis=1):")
print(median_df_rows)
# 输出:
# DataFrame Median (axis=1):
# 0     5.5
# 1    11.0
# 2     4.0
# 3     9.5
# 4    15.0
# Name: 0.5, dtype: float64
```

**`pandas.Series.quantile()` / `pandas.DataFrame.quantile()` 主要参数：**

- `q`: 需要计算的分位数，介于 0 和 1 之间（可以是一个数值或列表）。
- `interpolation`: 插值方法，默认为 `'linear'`。可选值与 NumPy 类似。
- `axis` (仅 DataFrame): 计算分位数的轴，`0` 或 `'index'`（列），`1` 或 `'columns'`（行）。

## 总结

分位数和分位数函数是理解数据分布特征的重要工具。它们告诉我们数据在特定概率点上的取值。Python 的 NumPy 和 Pandas 库提供了强大而灵活的函数来计算样本分位数，允许我们通过指定不同的插值方法来处理样本数据。掌握分位数的概念和计算方法对于进行有效的数据分析至关重要。