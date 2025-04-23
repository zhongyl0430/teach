卡方分布、t分布和F分布是统计学中三大重要抽样分布，在假设检验和参数估计中具有核心作用。以下从定义、性质和应用角度进行系统比较：

### 三大分布对比表

| 特征         | 卡方分布 (χ²)                                             | t分布 (Student's t)                                                                              | F分布                                                                                                        |
| :--------- | :---------------------------------------------------- | :--------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| **定义**     | 独立标准正态变量平方和                                           | 正态变量与卡方变量根之比                                                                                   | 两个独立卡方变量自由度比                                                                                               |
| **概率密度函数** | $f(x) = \frac{x^{k/2-1}e^{-x/2}}{2^{k/2}\Gamma(k/2)}$ | $f(t) = \frac{\Gamma(\frac{ν+1}{2})}{\sqrt{νπ}\Gamma(\frac{ν}{2})}(1+\frac{t²}{ν})^{-(ν+1)/2}$ | $f(x) = \frac{\sqrt{\frac{(d_1x)^{d_1}d_2^{d_2}}{(d_1x+d_2)^{d_1+d_2}}}}{xB(\frac{d_1}{2},\frac{d_2}{2})}$ |
| **参数**     | 自由度$k$                                                | 自由度$ν$                                                                                         | 自由度$d_1$, $d_2$                                                                                            |
| **取值范围**   | $[0, +∞)$                                             | $(-∞, +∞)$                                                                                     | $[0, +∞)$                                                                                                  |
| **形态特征**   | 右偏态，随$k$增大趋近正态                                        | 对称钟型，尾部厚于正态                                                                                    | 右偏态，随自由度增加趋近正态                                                                                             |
| **均值**     | $k$                                                   | 0 (当$ν > 1$)                                                                                   | $\frac{d_2}{d_2-2}$($d_2 > 2$)                                                                             |
| **方差**     | $2k$                                                  | $\frac{ν}{ν-2}$($ν > 2$)                                                                       | $\frac{2d_2^2(d_1+d_2-2)}{d_1(d_2-2)^2(d_2-4)}$($d_2 > 4$)                                                 |
| **主要应用**   | 方差检验、拟合优度检验、独立性检验                                     | 均值差异检验、回归系数显著性检验                                                                               | 方差齐性检验、ANOVA、回归模型显著性检验                                                                                     |

### 核心联系

1. **衍生关系**
    - t分布可视为正态分布与卡方分布的组合：$T = \frac{Z}{\sqrt{\chi²_ν/ν}}$[^2][^5]
    - F分布本质是两个卡方分布的比值：$F = \frac{\chi²_{d_1}/d_1}{\chi²_{d_2}/d_2}$[^3][^4]
2. **渐进性质**
    - 当自由度$ν→∞$时，t分布收敛于标准正态分布
    - 当$d_1=1$时，F分布等价于t分布的平方
3. **检验方法关联**
    - 回归分析中，F检验整体模型显著性，t检验单个系数显著性
    - 方差分析(ANOVA)使用F分布，事后比较常采用t检验

**应用示例**：在药物疗效比较实验中，先用F检验判断不同剂量组的方差齐性，再用t检验比较各组均值差异，最后用卡方检验分析疗效与剂量的独立性。这种组合检验充分发挥了三大分布的特点[^3][^5][^6]。

[^1]: https://www.scribbr.com/statistics/chi-square-distributions/

[^2]: https://www.investopedia.com/terms/t/tdistribution.asp

[^3]: https://www.almabetter.com/bytes/tutorials/applied-statistics/f-distribution

[^4]: https://en.wikipedia.org/wiki/Chi-squared_distribution

[^5]: https://byjus.com/maths/t-distribution/

[^6]: https://www.ck12.org/flexi/algebra-ii/probability-distributions/what-are-the-characteristics-of-a-chi-square-distribution/

[^7]: https://stats.libretexts.org/Courses/Los_Angeles_City_College/Introductory_Statistics/11:_The_Chi-Square_Distribution/11.02:_Facts_About_the_Chi-Square_Distribution

[^8]: https://www.statlect.com/probability-distributions/F-distribution

[^9]: https://courses.lumenlearning.com/introstats1/chapter/facts-about-the-chi-square-distribution/

[^10]: https://stattrek.com/probability-distributions/t-distribution

[^11]: https://www.numberanalytics.com/blog/f-distribution-basics-concepts-tests-explained

[^12]: https://www.westga.edu/academics/research/vrc/assets/docs/ChiSquareTest_LectureNotes.pdf

[^13]: https://www.scribbr.com/statistics/t-distribution/

[^14]: https://courses.lumenlearning.com/introstats1/chapter/facts-about-the-f-distribution/

[^15]: https://www.scribbr.com/statistics/chi-square-tests/

[^16]: https://www.jmp.com/en_us/statistics-knowledge-portal/t-test/t-distribution.html

[^17]: https://online.stat.psu.edu/stat415/lesson/4/4.2

[^18]: https://www.me.psu.edu/casestudy/Statistics/t.htm

[^19]: https://soc.utah.edu/sociology3112/chi-square.php

[^20]: https://stattrek.com/probability-distributions/chi-square

