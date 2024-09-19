## EX 2.36

The article "Reliability Evaluation of Solar Photovoltaic Arrays" (Solar Energy, 2002: 129-141) presents various configurations of solar photovoltaic arrays consisting of crystalline silicon solar cells. Consider first the system illustrated in Figure 2.14(a).

；文章《太阳能光伏阵列的可靠性评估》（太阳能，2002年：129-141页）介绍了由晶体硅太阳能电池组成的太阳能光伏阵列的各种配置。首先考虑图2.14(a)所示的系统。

Figure 2.14 System configurations for Example 2.36: (a) series-parallel; (b) total-cross-tied
![](01913607-292d-7d0a-a250-4b01870485a1_37_425535.jpg)

图2.14 示例2.36的系统配置：(a) 串联-并联；(b) 完全交叉连接

There are two subsystems connected in parallel, each one containing three cells. In order for the system to function, at least one of the two parallel subsystems must work. Within each subsystem, the three cells are connected in series, so a subsystem will work only if all cells in the subsystem work. Consider a particular lifetime value ${t}_{0}$ , and supose we want to determine the probability that the system lifetime exceeds ${t}_{0}$ . Let ${A}_{i}$ denote the event that the lifetime of cell $i$ exceeds ${t}_{0}\left( {i = 1,2,\ldots ,6}\right)$ . We assume that the ${A}_{i}^{\prime }s$ are independent events (whether any particular cell lasts more than ${t}_{0}$ hours has no bearing on whether or not any other cell does) and that $P\left( {A}_{i}\right) = {.9}$ for every $i$ since the cells are identical. Then

系统中有两个并联的子系统，每个子系统中包含三个电池。为了使系统正常工作，至少需要两个并联子系统中的一个能够工作。在每个子系统中，三个电池是串联连接的，因此只有当子系统中的所有电池都工作时，子系统才会工作。考虑一个特定的寿命值 ${t}_{0}$ ，假设我们想要确定系统寿命超过 ${t}_{0}$ 的概率。令 ${A}_{i}$ 表示电池 $i$ 的寿命超过 ${t}_{0}\left( {i = 1,2,\ldots ,6}\right)$ 的事件。我们假设 ${A}_{i}^{\prime }s$ 是独立事件（任何一个电池能否持续超过 ${t}_{0}$ 小时不会影响其他电池的情况），并且由于电池相同，对于每一个 $i$ 都有 $P\left( {A}_{i}\right) = {.9}$ 。那么

$$
P\left( {\text{system lifetime exceeds}{t}_{0}}\right) = P\left\lbrack {\left( {{A}_{1} \cap {A}_{2} \cap {A}_{3}}\right) \cup \left( {{A}_{4} \cap {A}_{5} \cap {A}_{6}}\right) }\right\rbrack
$$

$$
= P\left( {{A}_{1} \cap {A}_{2} \cap {A}_{3}}\right) + P\left( {{A}_{4} \cap {A}_{5} \cap {A}_{6}}\right)
$$

$$
-   P\left\lbrack {\left( {{A}_1 \cap {A}_2 \cap {A}_3}\right) \cap \left( {{A}_4 \cap {A}_5 \cap {A}_6}\right) }\right\rbrack
$$

$$
= \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) + \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) - \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) \left( {.9}\right) = {.927}
$$

Alternatively,

或者，

$P\left( {\text{system lifetime exceeds}{t}_{0}}\right) = 1 - P\left( {\text{both subsystem lives are} \leq {t}_{0}}\right)$

$$
= 1 - {\left\lbrack P\left( \text{ subsystem life is } \leq {t}_{0}\right) \right\rbrack }^{2}
$$

$$
= 1 - {\left\lbrack 1 - P\left( \text{ subsystem life is } > {t}_{0}\right) \right\rbrack }^{2}
$$

$$
= 1 - {\left\lbrack 1 - {\left( {.9}\right) }^{3}\right\rbrack }^{2} = {.927}
$$

Next consider the total-cross-tied system shown in Figure 2.14(b), obtained from the series-parallel array by connecting ties across each column of junctions. Now the

接下来考虑图2.14(b)所示的完全交叉连接系统，该系统通过在每一个交叉点列连接交叉带来获得串联-并联阵列。现在系统会在整个列一旦失效时失败，只有当每个列的寿命都超过 时，系统的寿命才会超过 。

system fails as soon as an entire column fails, and system lifetime exceeds ${t}_{0}$ only if the life of every column does so. For this configuration,

对于这种配置，系统一旦整列失效就会失败，只有当每个列的寿命都超过 ${t}_{0}$ 时，系统寿命才会超过 ${t}_{0}$ 。

$P\left( {\text{system lifetime is at least}{t}_{0}}\right) = {\left\lbrack P\left( \text{column lifetime exceeds}{t}_{0}\right) \right\rbrack }^{3}$

$$
= {\left\lbrack 1 - P\left( \text{ column lifetime is } \leq {t}_{0}\right) \right\rbrack }^{3}
$$

$= {\left\lbrack 1 - P\left( \text{ both cells in a column have lifetime } \leq {t}_{0}\right) \right\rbrack }^{3}$

$= {\left\lbrack 1 - {\left( 1 - {.9}\right) }^{2}\right\rbrack }^{3} = {.970}$


<a id="org09cfbcf"></a>