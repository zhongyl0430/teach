
Only 1 in 1000 adults is afflicted with a rare disease for which a diagnostic test has been developed. The test is such that when an individual actually has the disease, a positive result will occur ${99}\%$ of the time, whereas an individual without the disease will show a positive test result only $2\%$ of the time (the sensitivity of this test is ${99}\%$ and the specificity is ${98}\%$ ; in contrast, the Sept. 22, 2012 issue of The Lancet reports that the first at-home HIV test has a sensitivity of only ${92}\%$ and a specificity of ${99.98}\%$ ). If a randomly selected individual is tested and the result is positive, what is the probability that the individual has the disease?

示例2.31 罕见疾病的发病率。在1000名成年人中只有1人患有已开发出诊断测试的罕见疾病。该测试的特点是，当个体实际上患有该疾病时，阳性结果将发生 ${99}\%$ 的时间，而一个没有疾病的个体只会显示出阳性测试结果 $2\%$ 的时间（该测试的敏感性为 ${99}\%$ ，特异性为 ${98}\%$ ；相比之下，《柳叶刀》杂志2012年9月22日那一期报道的家庭HIV检测的敏感性仅为 ${92}\%$ ，特异性为 ${99.98}\%$ ）。如果一个随机选择的个体进行了测试并且结果为阳性，那么这个个体患有疾病的概率是多少？

To use Bayes' theorem, let ${A}_{1} =$ individual has the disease, ${A}_{2} =$ individual does not have the disease, and $B =$ positive test result. Then $P\left( {A}_{1}\right) = {.001}$ , $P\left( {A}_{2}\right) = {.999},P\left( {B \mid {A}_{1}}\right) = {.99}$ , and $P\left( {B \mid {A}_{2}}\right) = {.02}$ . The tree diagram for this problem is in Figure 2.12.

要使用贝叶斯定理，设 ${A}_{1} =$ 个体患有疾病， ${A}_{2} =$ 个体没有疾病， $B =$ 阳性测试结果。那么 $P\left( {A}_{1}\right) = {.001}$ ， $P\left( {A}_{2}\right) = {.999},P\left( {B \mid {A}_{1}}\right) = {.99}$ ，和 $P\left( {B \mid {A}_{2}}\right) = {.02}$ 。这个问题对应的树状图在图2.12中。

Figure 2.12 Tree diagram for the rare-disease problem
![](01913607-292d-7d0a-a250-4b01870485a1_31_864460.jpg)
图2.12 罕见疾病问题的树状图

Next to each branch corresponding to a positive test result, the multiplication rule yields the recorded probabilities. Therefore, $P\left( B\right) = {.00099} + {.01998} = {.02097}$ , from which we have

在每个对应阳性测试结果的分支旁边，乘法规则得出了记录的概率。因此， $P\left( B\right) = {.00099} + {.01998} = {.02097}$ ，由此我们有

$$
P\left( {{A}_{1} \mid B}\right) = \frac{P\left( {{A}_{1} \cap B}\right) }{P\left( B\right) } = \frac{.00099}{.02097} = {.047}
$$

This result seems counterintuitive; the diagnostic test appears so accurate that we expect someone with a positive test result to be highly likely to have the disease, whereas the computed conditional probability is only .047 . However, the rarity of the disease implies that most positive test results arise from errors rather than from diseased individuals. The probability of having the disease has increased by a multiplicative factor of 47 (from prior .001 to posterior .047); but to get a further increase in the posterior probability, a diagnostic test with much smaller error rates is needed.

这个结果看起来违反直觉；诊断测试看起来非常准确，以至于我们期望阳性测试结果的人很可能患有这种病，然而计算出的条件概率仅为0.047。然而，疾病的罕见性意味着大多数阳性测试结果来源于错误，而不是来自患病个体。患病的概率增加了一个乘数因子47（从先验的0.001增加到后验的0.047）；但要进一步增加后验概率，需要一个错误率更小的诊断测试。
