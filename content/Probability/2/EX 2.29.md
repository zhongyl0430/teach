- An electronics store sells three different brands of DVD players. 
- Of its DVD player sales, 
	- ${50}\%$ are brand 1 (the least expensive), 
	- ${30}\%$ are brand 2, 
	- ${20}\%$ are brand 3 . 
- Each manufacturer offers a 1-year warranty on parts and labor. 
- It is known that ${25}\%$ of brand 1's DVD players require warranty repair work, 
	- whereas the corresponding percentages for brands 2 and 3 are ${20}\%$ and ${10}\%$ , respectively.

示例 2.29 一家电子产品商店销售三种不同品牌的 DVD 播放器。在其 DVD 播放器的销售中， ${50}\%$ 是品牌 1（最便宜的）， ${30}\%$ 是品牌 2，而 ${20}\%$ 是品牌 3。每个制造商都为零部件和人工提供一年的保修。已知 ${25}\%$ 的品牌 1 的 DVD 播放器需要保修维修，而品牌 2 和品牌 3 的相应百分比分别为 ${20}\%$ 和 ${10}\%$ 。

1.  What is the probability that a randomly selected purchaser has bought a brand 1 DVD player that will need repair while under warranty?

2.  随机选择的购买者购买的品牌 1 DVD 播放器在保修期内需要维修的概率是多少？

3.  What is the probability that a randomly selected purchaser has a DVD player that will need repair while under warranty?

4.  随机选择的购买者购买的 DVD 播放器在保修期内需要维修的概率是多少？

5.  If a customer returns to the store with a DVD player that needs warranty repair work, what is the probability that it is a brand 1 DVD player? A brand 2 DVD player? A brand 3 DVD player?

如果客户带着需要保修维修的DVD播放器回到商店，它是品牌1的DVD播放器的概率是多少？品牌2的DVD播放器呢？品牌3的DVD播放器呢？

The first stage of the problem involves a customer selecting one of the three brands of DVD player. Let ${A}_{i} = \{$ brand $i$ is purchased $\}$ , for $i = 1,2$ , and 3 . Then $P\left( {A}_{1}\right) = {.50},P\left( {A}_{2}\right) = {.30}$ , and $P\left( {A}_{3}\right) = {.20}$ . Once a brand of DVD player is selected, the second stage involves observing whether the selected DVD player needs warranty repair. With $B = \{$ needs repair $\}$ and ${B}^{\prime } = \{$ doesn't need repair $\}$ , the given information implies that $P\left( {B \mid {A}_{1}}\right) = {.25},P\left( {B \mid {A}_{2}}\right) = {.20}$ , and $P\left( {B \mid {A}_{3}}\right) = {.10}$ .

问题的第一阶段涉及客户选择三种DVD播放器品牌之一。设 ${A}_{i} = \{$ 品牌为 $i$ 被购买 $\}$ ，对于 $i = 1,2$ ，和3。那么 $P\left( {A}_{1}\right) = {.50},P\left( {A}_{2}\right) = {.30}$ ，和 $P\left( {A}_{3}\right) = {.20}$ 。一旦选择了DVD播放器品牌，第二阶段就是观察所选的DVD播放器是否需要保修维修。已知 $B = \{$ 需要维修 $\}$ 和 ${B}^{\prime } = \{$ 不需要维修 $\}$ ，给定信息暗示 $P\left( {B \mid {A}_{1}}\right) = {.25},P\left( {B \mid {A}_{2}}\right) = {.20}$ ，和 $P\left( {B \mid {A}_{3}}\right) = {.10}$ 。

The tree diagram representing this experimental situation is shown in Figure 2.10. The initial branches correspond to different brands of DVD players; there are two second-generation branches emanating from the tip of each initial branch, one for "needs repair" and the other for "doesn't need repair." The probability $P\left( {A}_{i}\right)$ appears on the $i$ th initial branch, whereas the conditional probabilities $P\left( {B \mid {A}_{i}}\right)$ and $P\left( {{B}^{\prime } \mid {A}_{i}}\right)$ appear on the second-generation branches. To the right of each second-generation branch corresponding to the occurrence of $B$ , we display the product of probabilities on the branches leading out to that point. This is simply the multiplication rule in action. The answer to the question posed in 1 is thus $P\left( {{A}_{1} \cap B}\right) = P\left( {B \mid {A}_{1}}\right) \cdot P\left( {A}_{1}\right) = {.125}$ . The answer to question 2 is

表示这种实验情况的树状图如图2.10所示。初始分支对应不同的DVD播放器品牌；每个初始分支的尖端发出两个第二代分支，一个对应"需要维修"，另一个对应"不需要维修"。概率 $P\left( {A}_{i}\right)$ 出现在第 $i$ 个初始分支上，而条件概率 $P\left( {B \mid {A}_{i}}\right)$ 和 $P\left( {{B}^{\prime } \mid {A}_{i}}\right)$ 出现在第二代分支上。在每个对应 $B$ 发生的第二代分支右侧，我们展示了引导到该点的分支上概率的乘积。这就是乘法规则的运用。因此，问题1中提出的问题的答案是 $P\left( {{A}_{1} \cap B}\right) = P\left( {B \mid {A}_{1}}\right) \cdot P\left( {A}_{1}\right) = {.125}$ 。问题2的答案是

$$
P\left( B\right) = P\left\lbrack \text{(brand 1 and repair) or (brand 2 and repair) or (brand 3 and repair)}\right\rbrack
$$

$$
= P\left( {{A}_{1} \cap B}\right) + P\left( {{A}_{2} \cap B}\right) + P\left( {{A}_{3} \cap B}\right)
$$

$$
= {.125} + {.060} + {.020} = {.205}
$$

Figure 2.10 Tree diagram for Example 2.29
![](01913607-292d-7d0a-a250-4b01870485a1_28_663477.jpg)

图 2.10 示例 2.29 的树状图

Finally,

最后，

$$
P\left( {{A}_{1} \mid B}\right) = \frac{P\left( {{A}_{1} \cap B}\right) }{P\left( B\right) } = \frac{.125}{.205} = {.61}
$$

$$
P\left( {{A}_{2} \mid B}\right) = \frac{P\left( {{A}_{2} \cap B}\right) }{P\left( B\right) } = \frac{.060}{.205} = {.29}
$$

and

以及

$$
P\left( {{A}_{3} \mid B}\right) = 1 - P\left( {{A}_{1} \mid B}\right) - P\left( {{A}_{2} \mid B}\right) = {.10}
$$

The initial or prior probability of brand 1 is .50 . Once it is known that the selected DVD player needed repair, the posterior probability of brand 1 increases to .61. This is because brand 1 DVD players are more likely to need warranty repair than are the other brands. The posterior probability of brand 3 is $P\left( {{A}_{3} \mid B}\right) = {.10}$ , which is much less than the prior probability $P\left( {A}_{3}\right) = {.20}$ .

品牌 1 的初始或先验概率为 0.50。一旦知道选定的 DVD 播放器需要维修，品牌 1 的后验概率增加到 0.61。这是因为品牌 1 的 DVD 播放器比其他品牌更有可能需要保修维修。品牌 3 的后验概率是 $P\left( {{A}_{3} \mid B}\right) = {.10}$ ，这比先验概率 $P\left( {A}_{3}\right) = {.20}$ 小得多。