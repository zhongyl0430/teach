
> [!definition] 行列式的记号
> 我们用
> $$D = \left| \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{n1} & {a}_{n2} & \cdots & {a}_{nn} \end{matrix}\right|$$
> 表示一个 $n$ 阶行列式,其中元素 ${a}_{ij} \in \mathbb{C}$ $\left( {i,j = 1,2,\cdots ,n}\right)$ ,这里 $\mathbb{C}$ 为复数集. 
> 为了描述行列式中某个位置的元素, 我们将行列式的
> - 横排称为行 (row)
> - 竖排称为列 (column)
>这也是用行列式来命名上面式子的原因所在.
>那么,
>- ${a}_{ij}$ 表示此 $n$ 阶行列式的第 $i$ 行第 $j$ 列的元素, 
>- $i$ 称为行指标,
>- $j$ 称为列指标.

我们首先 [[分析2阶与3阶行列式的定义]]. 
从二阶和三阶行列式的展开式中得到启发,下面借助于 $n$ 阶排列的知识来定义 $n$ 阶行列式的值.

> [!definition] 定义 3.1. $n$ 阶行列式
> $n$ 阶行列式
> $$D = \left| \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{n1} & {a}_{n2} & \cdots & {a}_{nn} \end{matrix}\right|$$
> 等于所有来自不同行不同列的 $n$ 个元素乘积的代数和. 
> 
> 由于代数和的项数为 $n !$ 个,
> 为了表达方便, 我们可以将每项中的 $n$ 个元素按行指标由小及大的顺序排列, 
> 即写作 
> $${a}_{1{j}_{1}}{a}_{2{j}_{2}}\cdots {a}_{n{j}_{n}}$$
> 的形式,并规定
> - 当列指标 ${j}_{1}{j}_{2}\cdots {j}_{n}$ 是 *偶排列* 时,此项前面带正号; 
> - 当列指标 ${j}_{1}{j}_{2}\cdots {j}_{n}$ 是 *奇排列* 时,此项前面带负号. 
> 
> 这样, $n$ 阶行列式可以表示为
> $$
> \begin{align}
> D &= \left| \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{n1} & {a}_{n2} & \cdots & {a}_{nn} \end{matrix}\right| \\
> &= \mathop{\sum }\limits_{{{j}_{1}{j}_{2}\cdots {j}_{n}}}{\left( -1\right) }^{\tau \left( {{j}_{1}{j}_{2}\cdots {j}_{n}}\right) }{a}_{1{j}_{1}}{a}_{2{j}_{2}}\cdots {a}_{n{j}_{n}}. \tag{3.1}
> \end{align}
> $$
> 其中 $\mathop{\sum }\limits_{{{j}_{1}{j}_{2}\cdots {j}_{n}}}$ 表示对所有可能的 $n$ 阶排列求和. 
> (3.1) 称为行列式的 **展开式**.
> 
> 上述 $n$ 阶行列式通常记为 $D = \det \left( {a}_{ij}\right)$ 或者 ${\left| {a}_{ij}\right| }_{n}$.

> [!remark] 验证低阶行列式
> - 当 $n = 1$ 时, 规定 $\left| {a}_{11}\right| = {a}_{11}$ .
> - 当 $n = 2$ 时, 
> $$\left| \begin{array}{ll} {a}_{11} & {a}_{12} \\ {a}_{21} & {a}_{22} \end{array}\right| = \mathop{\sum }\limits_{{{j}_{1}{j}_{2}}}{\left( -1\right) }^{\tau \left( {{j}_{1}{j}_{2}}\right) }{a}_{1{j}_{1}}{a}_{2{j}_{2}},$$
> - 当 $n = 3$ 时, 
> $$\left| \begin{array}{lll} {a}_{11} & {a}_{12} & {a}_{13} \\ {a}_{21} & {a}_{22} & {a}_{23} \\ {a}_{31} & {a}_{32} & {a}_{33} \end{array}\right| = \mathop{\sum }\limits_{{{j}_{1}{j}_{2}{j}_{3}}}{\left( -1\right) }^{\tau \left( {{j}_{1}{j}_{2}{j}_{3}}\right) }{a}_{1{j}_{1}}{a}_{2{j}_{2}}{a}_{3{j}_{3}}.$$

> [!remark] 行列式按列展开
> - 上面定义行列式展开式中的项是按行指标的自然顺序排列的. 
> - 一个自然的问题是, 每一项能否按列指标的自然顺序排列呢? 
> 	- 答案是肯定的.
> 由于数的乘法满足交换律,不妨设某项为 ${a}_{1{j}_{1}}{a}_{2{j}_{2}}\cdots {a}_{n{j}_{n}}$ ,调整元素的顺序,设
> $${a}_{1{j}_{1}}{a}_{2{j}_{2}}\cdots {a}_{n{j}_{n}} = {a}_{{i}_{1}1}{a}_{{i}_{2}2}\cdots {a}_{{i}_{n}n}.$$
> - 我们知道此项的正负由 $\tau \left( {{j}_{1}{j}_{2}\cdots {j}_{n}}\right)$ 来决定. 
> - 将上述等式左侧化为右侧可以通过元素之间的对换来完成, 
> 	- 每作一次元素的对换, 由其元素的行指标和列指标构成的排列也都要作一次对换, 
> 	- 也就是说 ${i}_{1}{i}_{2}\cdots {i}_{n}$ 与 ${j}_{1}{j}_{2}\cdots {j}_{n}$ 同时改变奇偶性, 
> - 故由定理 2.2 知 ${\left( -1\right) }^{\tau \left( {{i}_{1}{i}_{2}\cdots {i}_{n}}\right) } = {\left( -1\right) }^{\tau \left( {{j}_{1}{j}_{2}\cdots {j}_{n}}\right) }$.
> - 于是, $n$ 阶行列式的另一个展开式为
> $$\left| \begin{matrix} {a}_{11} & {a}_{12} & \cdots & {a}_{1n} \\ {a}_{21} & {a}_{22} & \cdots & {a}_{2n} \\ \vdots & \vdots & & \vdots \\ {a}_{n1} & {a}_{n2} & \cdots & {a}_{nn} \end{matrix}\right| = \mathop{\sum }\limits_{{{i}_{1}{i}_{2}\cdots {i}_{n}}}{\left( -1\right) }^{\tau \left( {{i}_{1}{i}_{2}\cdots {i}_{n}}\right) }{a}_{{i}_{1}1}{a}_{{i}_{2}2}\cdots {a}_{{i}_{n}n}. \tag{3.2}$$

[[teach/Linear algebra/1/例题 3.1]]