> [!property] F分布的性质
> 若 $Z \sim  F\left( {m, n}\right)$, 则 
> $$\frac{1}{Z} \sim  F\left( {n, m}\right) .$$

^statement

### **证明步骤**

**1. F分布的定义**
根据 $F$-分布的定义，若 $X \sim \chi^2(m)$ 和 $Y \sim \chi^2(n)$ 是独立的卡方分布变量，则随机变量：
$$
Z = \frac{X/m}{Y/n}
$$
服从自由度为 $(m, n)$ 的 $F$-分布，即 $Z \sim F(m, n)$ [^1][^3][^7]。

**2. 计算 $1/Z$ 的表达式**
对 $Z$ 取倒数：
$$
\frac{1}{Z} = \frac{Y/n}{X/m} = \frac{Y/m}{X/n}.
$$

此时，分子 $Y/m$ 是自由度为 $n$ 的卡方变量除以自由度 $m$，分母 $X/n$ 是自由度为 $m$ 的卡方变量除以自由度 $n$。

**3. 应用F分布的定义**
根据 $F$-分布的定义，若将分子和分母的卡方变量交换自由度，则：
$$
\frac{Y/m}{X/n} \sim F(n, m).
$$

因此，$\frac{1}{Z} \sim F(n, m)$。

### **数学推导验证**

设 $Z \sim F(m, n)$，则其概率密度函数（PDF）为：
$$
f_Z(z) = \frac{\Gamma\left(\frac{m+n}{2}\right)}{\Gamma\left(\frac{m}{2}\right)\Gamma\left(\frac{n}{2}\right)} \left(\frac{m}{n}\right)^{m/2} \frac{z^{(m/2)-1}}{\left(1 + \frac{m}{n}z\right)^{(m+n)/2}} \quad (z \geq 0).
$$

令 $W = \frac{1}{Z}$，则 $ W $ 的累积分布函数（CDF）为：
$$
P(W \leq w) = P\left(\frac{1}{Z} \leq w\right) = P\left(Z \geq \frac{1}{w}\right) = 1 - P\left(Z \leq \frac{1}{w}\right).
$$

对 $W$ 求导得到其 PDF：
$$
f_W(w) = \frac{d}{dw} \left[1 - F_Z\left(\frac{1}{w}\right)\right] = f_Z\left(\frac{1}{w}\right) \cdot \frac{1}{w^2}.
$$

将 $f_Z\left(\frac{1}{w}\right)$ 代入并化简，可得：
$$
f_W(w) = \frac{\Gamma\left(\frac{m+n}{2}\right)}{\Gamma\left(\frac{n}{2}\right)\Gamma\left(\frac{m}{2}\right)} \left(\frac{n}{m}\right)^{n/2} \frac{w^{(n/2)-1}}{\left(1 + \frac{n}{m}w\right)^{(m+n)/2}} \quad (w \geq 0),
$$

这正是自由度为 $(n, m)$ 的 $F$-分布的 PDF[^4][^6]。

### **结论**

通过定义和概率密度函数的推导，证明了若 $Z \sim F(m, n)$，则 $\frac{1}{Z} \sim F(n, m)$。这一性质在统计推断中常用于计算双侧检验的临界值或构造置信区间[^2][^5]。

[^1]: https://www.almabetter.com/bytes/tutorials/applied-statistics/f-distribution

[^2]: https://www.reddit.com/r/statistics/comments/wlv3av/question_reasonproof_for_inverse_rule_in/

[^3]: https://www.randomservices.org/random/special/Fisher.html

[^4]: https://stattrek.com/probability-distributions/f-distribution

[^5]: https://math.stackexchange.com/questions/2371494/show-prove-that-f-alpha-n-m-1-f-1-alpha-m-n

[^6]: https://proofwiki.org/wiki/Reciprocal_of_Random_Variable_with_Snedecor's_F-Distribution_has_Snedecor's_F-Distribution

[^7]: https://statproofbook.github.io/P/f-pdf.html

[^8]: https://math.stackexchange.com/questions/695165/help-for-u-t2-has-an-f-distribution-with-1-numerator-and-v-denominator

[^9]: https://stats.stackexchange.com/questions/35204/what-are-the-connections-between-the-normal-the-chi2-the-f-distributions

[^10]: https://people.richland.edu/james/lecture/m113/f_test.html

[^11]: https://www.reddit.com/r/AskStatistics/comments/md5nfs/whats_the_difference_between_a_z_distribution_t/

[^12]: https://online.stat.psu.edu/stat415/lesson/4/4.2

[^13]: https://www.math.wm.edu/~leemis/chart/UDR/PDFs/FI.pdf

[^14]: https://ecampusontario.pressbooks.pub/sccstatistics/chapter/facts-about-the-f-distribution/

[^15]: https://www.youtube.com/watch?v=gd-mebhr8l8

[^16]: https://courses.lumenlearning.com/introstats1/chapter/facts-about-the-f-distribution/

[^17]: https://www.acsu.buffalo.edu/~adamcunn/probability/f.html

[^18]: https://analystprep.com/cfa-level-1-exam/quantitative-methods/chi-square-distribution-and-f-distribution/

[^19]: https://stats.libretexts.org/Bookshelves/Probability_Theory/Probability_Mathematical_Statistics_and_Stochastic_Processes_(Siegrist)/05:_Special_Distributions/5.11:_The_F_Distribution

[^20]: https://www.youtube.com/watch?v=AmHiOKYmHkI

[^21]: https://www.youtube.com/watch?v=rU3LwSdOyWk

[^22]: https://math.stackexchange.com/questions/2371494/show-prove-that-f-alpha-n-m-1-f-1-alpha-m-n

[^23]: https://statproofbook.github.io/P/ugkv-ztest1.html

[^24]: https://www.reddit.com/r/askmath/comments/1dlgmq7/how_to_solve_fmn1_fm_fn/

[^25]: https://www.statlect.com/probability-distributions/F-distribution

[^26]: http://www.milefoot.com/math/stat/pdfc-fdist.htm

[^27]: https://www.math.ucsd.edu/~jmckerna/Teaching/16-17/Spring/109/l_9.pdf

[^28]: https://en.wikipedia.org/wiki/F-distribution

[^29]: https://www3.nd.edu/~dgalvin1/40210/40210_S12/40210H9_sols.pdf

[^30]: https://stats.stackexchange.com/questions/312337/easy-proof-of-sum-i-1n-leftz-i-barz-right2-sim-chi2-n-1

[^31]: https://en.wikipedia.org/wiki/Reciprocal_distribution

[^32]: https://math.stackexchange.com/questions/1532650/finding-density-of-1-z-when-z-is-a-standard-random-normal-variable

[^33]: https://math.stackexchange.com/questions/2494973/how-find-the-fm1-fm-textconstant-forall-m-in-bbbn/2507069

[^34]: https://www.ucl.ac.uk/~rmjbale/Stat/Lecture_2.pdf

[^35]: https://math.stackexchange.com/questions/743823/if-fmnfmn-1-fmfnhow-find-fn

