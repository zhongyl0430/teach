An individual has 3 different email accounts. Most of her messages, in fact 70%, come into account #1, whereas ${20}\%$ come into account #2 and the remaining ${10}\%$ into account #3. Of the messages into account #1, only 1% are spam, whereas the corresponding percentages for accounts #2 and #3 are $2\%$ and $5\%$ , respectively. What is the probability that a randomly selected message is spam?

示例 2.30 一个个体有 3 个不同的电子邮件账户。她的大部分信息，实际上 70%，都进入了账户 1，而 ${20}\%$ 进入账户 2，剩下的 ${10}\%$ 进入账户 3。在账户 1 中的信息，只有 1% 是垃圾邮件，而账户 #2 和 #3 对应的百分比分别是 $2\%$ 和 $5\%$ 。随机选取一条信息是垃圾邮件的概率是多少？

To answer this question, let's first establish some notation:

为了回答这个问题，让我们首先建立一些记号：

${A}_{i} = \{$ message is from account $\# i\}$ for $i = 1,2,3,\;B = \{$ message is spam $\}$

${A}_{i} = \{$ 信息来自账户 $\# i\}$ 对于 $i = 1,2,3,\;B = \{$ 信息是垃圾邮件 $\}$

Then the given percentages imply that

那么给出的百分比意味着

$$
P\left( {A}_{1}\right) = {.70},P\left( {A}_{2}\right) = {.20},P\left( {A}_{3}\right) = {.10}
$$

$$
P\left( {B \mid {A}_{1}}\right) = {.01},P\left( {B \mid {A}_{2}}\right) = {.02},P\left( {B \mid {A}_{3}}\right) = {.05}
$$

Now it is simply a matter of substituting into the equation for the law of total probability:

现在只需将值代入总概率定律的方程中：

$$
P\left( B\right) = \left( {.01}\right) \left( {.70}\right) + \left( {.02}\right) \left( {.20}\right) + \left( {.05}\right) \left( {.10}\right) = {.016}
$$

In the long run, ${1.6}\%$ of this individual's messages will be spam.

从长远来看， ${1.6}\%$ 的这个个体的信息将是垃圾邮件。