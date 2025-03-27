```python
import numpy as np
import matplotlib.pyplot as plt

# 均值向量和协方差矩阵
mu = np.array([0, 0])
sigma = np.array([[4, 2], [2, 4]])

# 生成二维正态分布样本
samples = np.random.multivariate_normal(mu, sigma, size=500)

# 绘制散点图
plt.scatter(samples[:, 0], samples[:, 1], alpha=0.5)
plt.title("multivariate_normal")
plt.xlabel("X1")
plt.ylabel("X2")
plt.axis('equal')
plt.show()
```

![[multivariate_normal.png]]

![[multivariate_normal_5000.png]]