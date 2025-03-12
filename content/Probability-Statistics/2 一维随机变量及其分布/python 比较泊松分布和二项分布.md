```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.stats import binom, poisson

# 设定二项分布参数，使得 np = λ 恒定
n = 100  # 试验次数
p = 0.1  # 成功概率
lambda_ = n * p  # 泊松分布参数

# 定义 x 轴范围（取到 3σ 范围）
x = np.arange(0, int(lambda_ + 3 * np.sqrt(lambda_)) + 1)

# 计算二项分布和泊松分布的 PMF
pmf_binom = binom.pmf(x, n, p)
pmf_poisson = poisson.pmf(x, lambda_)

# 绘图
plt.figure(figsize=(8, 5))
plt.bar(x, pmf_binom, alpha=0.6, color='blue', label="Binomial PMF (n=100, p=0.1)")
plt.plot(x, pmf_poisson, 'ro-', markersize=5, label="Poisson PMF (λ=10)")

plt.xlabel("k")
plt.ylabel("Probability")
plt.title("Binomial Distribution Approximating Poisson Distribution")
plt.legend()
plt.grid()

# 显示图像
plt.show()
```

![[Poisson_vs_binormal_n=100.png]]

![[Poisson_vs_binormal_n=1000.png]]