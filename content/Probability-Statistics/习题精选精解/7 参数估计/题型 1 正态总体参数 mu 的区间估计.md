## 3.1
设由来自正态总体 $X \sim  N\left( {\mu,{0.9}^{2}}\right)$ 容量为 9 的简单随机样本,得样本均值 $\bar{X} = 5$,则未知参数 $\mu$ 的置信度为 0.95 的置信区间是_____.

### 分析
本题是一个正态总体在方差已知的情况下求期望值 $\mu$ 的置信区间的问题,由公式
$$
\left\lbrack  {\bar{X} - \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}},\bar{X} + \frac{\sigma }{\sqrt{n}}{u}_{\frac{\alpha }{2}}}\right\rbrack
$$

求解该置信区间.

### 解
由置信度 $1 - \alpha  = {0.95}$ 可得 $\alpha  = {0.05}$.

查 $N\left( {0,1}\right)$ 分布表得到 ${u}_{0.025} = {1.96}$.

代入 $\bar{X} = 5, n = 9,\sigma  = {0.9}$ 得
$$
\left\lbrack  {5 - \frac{0.9}{\sqrt{9}} \times  {1.96},\;5 + \frac{0.9}{\sqrt{9}} \times  {1.96}}\right\rbrack,
$$

因此参数 $\mu$ 置信度 0.95 的置信区间为 $\left\lbrack  {{4.412},{5.588}}\right\rbrack$.

## 3.2
设一批零件的长度服从正态分布 $N\left( {\mu,{\sigma }^{2}}\right)$,其中 $\mu,{\sigma }^{2}$ 均未知,现从中随机抽取 16 个零件,测得样本均值 $\bar{x} = {20}\left( \mathrm{\;{cm}}\right)$,样本标准差 $s = 1\left( \mathrm{\;{cm}}\right)$. 则 $\mu$ 的置信度为 0.90 的置信区间是 (   ).

(A) $\left( {{20} - \frac{1}{4}{t}_{0.05}\left( {16}\right),{20} + \frac{1}{4}{t}_{0.05}\left( {16}\right) }\right)$

(B) $\left( {{20} - \frac{1}{4}{t}_{0.1}\left( {16}\right),{20} + \frac{1}{4}{t}_{0.1}\left( {16}\right) }\right)$

(C) $\left( {{20} - \frac{1}{4}{t}_{0.05}\left( {15}\right),{20} + \frac{1}{4}{t}_{0.05}\left( {15}\right) }\right)$

(D) $\left( {{20} - \frac{1}{4}{t}_{0.1}\left( {15}\right),{20} + \frac{1}{4}{t}_{0.1}\left( {15}\right) }\right)$

### 解
经过分析本题属于在方差未知情况下求一个正态总体期望的置信区间, 其公式为
$$
\left( {\bar{X} - \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right),\;\bar{X} + \frac{S}{\sqrt{n}}{t}_{\frac{\alpha }{2}}\left( {n - 1}\right) }\right).
$$

根据题意 $\bar{x} = {20}, s = 1, n = {16},\frac{\alpha }{2} = {0.05}$,代入公式.

可知应选(C).

## 3.3
设总体 $X \sim  N\left( {\mu,{\sigma }^{2}}\right)$,已知 ${\sigma }^{2}$. 则样本容量 $n$ 至少为_____时,才能保证 $\mu$ 的置信度 $1 - \alpha$ 的置信区间长度不大于 $d$.

### 解
因为 $\mu$ 的置信区间为
$$
\left\lbrack  {\bar{X} - {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}},\bar{X} + {u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}}\right\rbrack
$$

所以区间长度为 $2{u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}}$,
则 $2{u}_{\frac{\alpha }{2}}\frac{\sigma }{\sqrt{n}} \leq  d$,
故 $n \geq  {\left( \frac{2{u}_{\frac{\alpha }{2}}\sigma }{d}\right) }^{2}$.

## 3.4
从总体 ${X}_{1} \sim  N\left( {{\mu }_{1},{25}}\right)$ 中取出一容量为 ${n}_{1} = {10}$ 的样本,其样本均值 ${\bar{X}}_{1} = {19.8}$; 从总体 ${X}_{2} \sim  N\left( {{\mu }_{2},{36}}\right)$ 中取出容量为 ${n}_{2} = {12}$ 的样本,其样本均值 ${\bar{X}}_{2} = {24.0}$,已知两个样本之间相互独立,求 ${\mu }_{1} - {\mu }_{2}$ 的 0.90 置信区间.

### 解
这是 ${\sigma }_{1}^{2},{\sigma }_{2}^{2}$ 都为已知时,求均值差的区间估计问题.

由于 $1 - \alpha  = {0.90}$,故 $\frac{\alpha }{2} = {0.05},{u}_{\frac{\alpha }{2}} = {1.645}$,

又因为 ${n}_{1} = {10},{n}_{2} = {12},{\sigma }_{1}^{2} = {25},{\sigma }_{2}^{2} = {36}$,所以
$$
\sqrt{\frac{{\sigma }_{1}^{2}}{{n}_{1}} + \frac{{\sigma }_{2}^{2}}{{n}_{2}}} = \sqrt{\frac{25}{10} + \frac{36}{12}} = \sqrt{5.5} = {2.345},
$$
$$
\begin{align}
\bar{X}_{1} - \bar{X}_{2} - u_{\frac{\alpha}{2}} \sqrt{\frac{\sigma_{1}^{2}}{n_{1}} + \frac{\sigma_{2}^{2}}{n_{2}}} & = 19.8 - 24.0 - 1.645 \times 2.345 \\
& = -4.2 - 3.858 \\
& = -8.06 \text{.}
\end{align}
$$$$
{\bar{X}}_{1} - {\bar{X}}_{2} + {u}_{\frac{\alpha }{2}}\sqrt{\frac{{\sigma }_{1}^{2}}{{n}_{1}} + \frac{{\sigma }_{2}^{2}}{{n}_{2}}} =  - {4.2} + {3.858} =  - {0.34}.
$$

因此,所求的 ${\mu }_{1} - {\mu }_{2}$ 的 0.90 置信区间为 $\left\lbrack  {-{8.06}, - {0.34}}\right\rbrack$.

## 3.5
设有甲、乙两种安眠药,随机变量 $X, Y$ 分别表示患者服用甲、乙药后睡眠时间的延长数,并假设 $X \sim  N\left( {{\mu }_{1},{\sigma }^{2}}\right), Y \sim  N\left( {{\mu }_{2},{\sigma }^{2}}\right)$. 为比较两种药品的疗效,随机地从服用甲药的患者中选取 10 人,从服用乙药的患者中选取 10 人,分别测得睡眠延长时间的均值与方差: $\overline{X} = {2.33},{S}_{1}^{2}$ $= {\left( {1.9}\right) }^{2};\bar{Y} = {0.75},{S}_{2}^{2} = {\left( {28.9}\right) }^{2}$. 试求方差未知情况下 ${\mu }_{1} - {\mu }_{2}$ 的 ${95}\%$ 置信区间.

### 解
两正态总体的方差未知但相等,小样本,取
$$
T = \frac{\left( {\bar{X} - \bar{Y}}\right)  - \left( {{\mu }_{1} - {\mu }_{2}}\right) }{{S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}}} \sim  t\left( {{n}_{1} + {n}_{2} - 2}\right) \;\text{(这里}{n}_{1} = {n}_{2} = {10}\text{),}
$$
$$
P\left\{  {\left| T\right|  < {t}_{\frac{\alpha }{2}}\left( {18}\right) }\right\}   = 1 - \alpha \;\left( {\alpha  = {0.05}}\right),
$$

查得 ${t}_{0.025}\left( {18}\right)  = {2.101}$. 于是算得置信下限、上限分别为
$$
\begin{align}
&\left( \bar{x} - \bar{y} \right) - t_{0.025}(18) \cdot S_{w} \sqrt{\frac{1}{n_{1}} + \frac{1}{n_{2}}} \\
& = \left( 2.33 - 0.75 \right) - 2.101 \times \sqrt{\frac{36.1 + 28.9}{18}} \times \sqrt{\frac{2}{10}} \\
& = 1.58 - 1.78 \\
& = -0.20 \text{.}
\end{align}
$$$$
\left( {\bar{x} - \bar{y}}\right)  + {t}_{0.025}\left( {18}\right)  \cdot  {S}_{w}\sqrt{\frac{1}{{n}_{1}} + \frac{1}{{n}_{2}}} = {1.58} + {1.78} = {3.36}.
$$
从而得 ${\mu }_{1} - {\mu }_{2}$ 的 ${95}\%$ 置信区间为 $\left( {-{0.20},{3.36}}\right)$.

## 3.6
为研究正常成年男、女血液红细胞的平均数的差别, 检查某地正常成年男子 156 名, 正常成年女子 74 名,计算得男性红细胞平均数为 465.13 万 $/{\mathrm{{mm}}}^{3}$,样本标准差为 54.80 万 $/{\mathrm{{mm}}}^{3}$; 女子红细胞平均数为 422.16 万 $/{\mathrm{{mm}}}^{3}$,样本标准差为 49.20 万 $/{\mathrm{{mm}}}^{3}$. 试问能否以 95% 的把握判定男子血红细胞均值高于女子血红细胞均值?

### 解
设正常成年男女血红细胞数构成的两个总体为 $X, Y$,则 $X \sim  N\left( {{\mu }_{1},{\sigma }_{1}^{2}}\right), Y \sim  N\left( {\mu }_{2}\right.$, $\left. {\sigma }_{2}^{2}\right)$, $X$ 与 $Y$ 独立,由 $1 - \alpha  = {0.95}$,得 $\alpha  = {0.05}$, ${u}_{\frac{\alpha }{2}} = {1.96}$,又 ${n}_{1} = {156},{n}_{2} = {74}$, $\bar{x} = {465.13}$, $\bar{y} = {422.16},{s}_{1} = {54.80},{s}_{2} = {49.20}$. 虽然 ${\sigma }_{1}^{2},{\sigma }_{2}^{2}$ 未知,但因为两组样本都属于大样本,故 ${\sigma }_{1}^{2} \approx  {s}_{1}^{2}$, ${\sigma }_{2}^{2} \approx  {s}_{2}^{2}$. 则 ${\mu }_{1} - {\mu }_{2}$ 的置信限为: $\left( {\bar{X} - \bar{Y}}\right)  \pm  {u}_{\frac{\alpha }{2}}\sqrt{\frac{{S}_{1}^{2}}{{n}_{1}} + \frac{{S}_{2}^{2}}{{n}_{2}}}$.

代入数值:
$$
\begin{align}
\left( \bar{x} - \bar{y} \right) - u_{\frac{\alpha}{2}} \sqrt{\frac{s_{1}^{2}}{n_{1}} + \frac{s_{2}^{2}}{n_{2}}} & \approx 28.04, \\
\left( \bar{x} - \bar{y} \right) + u_{\frac{\alpha}{2}} \sqrt{\frac{s_{1}^{2}}{n_{1}} + \frac{s_{2}^{2}}{n_{2}}} & \approx 57.1 \text{.}
\end{align}
$$
因此, ${\mu }_{1} - {\mu }_{2}$ 的 95 % 置信区间为 $\left\lbrack  {{28.04},{57.1}}\right\rbrack$.

因置信下限 28.04>0,从而 ${\mu }_{1} > {\mu }_{2}$,所以有 95% 的把握判定男性血红细胞均值高于女性血红细胞均值.