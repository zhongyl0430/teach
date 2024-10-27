
Frequently the nature of an experiment suggests that two events $A$ and $B$ should be assumed independent. This is the case, for example, if a manufacturer receives a circuit board from each of two different suppliers, each board is tested on arrival, and $A = \{$ first is defective $\}$ and $B = \{$ second is defective $\}$ . If $P\left( A\right) = {.1}$ , it should also be the case that $P\left( {A \mid B}\right) = {.1}$ ; knowing the condition of the second board shouldn&rsquo;t provide information about the condition of the first. The probability that both events will occur is easily calculated from the individual event probabilities when the events are independent.

通常实验的性质暗示两个事件 $A$ 和 $B$ 应该被假定为独立的。例如，如果一个制造商从两个不同的供应商那里各接收一块电路板，每块板在到达时都进行测试，且 $A = \{$ 第一块是次品 $\}$ 和 $B = \{$ 第二块是次品 $\}$ 。如果 $P\left( A\right) = {.1}$ ，那么 $P\left( {A \mid B}\right) = {.1}$ 也应该是这样的情况；了解第二块板的情况不应当提供关于第一块板情况的信息。当事件独立时，两个事件同时发生的概率可以很容易地从各自事件的概率计算得出。

> [!proposition] independence
> $A$ and $B$ are independent if and only if (iff)
> 
> 命题 $A$ 和 $B$ 是独立的当且仅当（iff）
> 
> $$
> P\left( {A \cap B}\right) = P\left( A\right) \cdot P\left( B\right) \tag{2.8}
> $$

The verification of this multiplication rule is as follows:

本乘法规则的验证如下：

$$
P\left( {A \cap B}\right) = P\left( {A \mid B}\right) \cdot P\left( B\right) = P\left( A\right) \cdot P\left( B\right) \tag{2.9}
$$

where the second equality in Equation (2.9) is valid iff $A$ and $B$ are independent. Equivalence of independence and Equation (2.8) imply that the latter can be used as a definition of independence.其中方程（2.9）中的第二个等式在 $A$ 和 $B$ 独立时有效。独立性与方程（2.8）的等价性意味着后者可以作为独立性的定义使用。

[[EX 2.34 washer vs dryer]]

[[EX 2.35 batch pass inspection]]