若 $X \sim  N\left( {0,1}\right)$, 则
$$
{X}^{2} \sim  \Gamma \left( {\frac{1}{2},\frac{1}{2}}\right). \tag{6.3.3}
$$
一般地,若 $X$ 的分布密度为
$$
{f}_{X}\left( x\right)  = \left\{  \begin{array}{ll} \frac{{\lambda }^{\alpha }}{\Gamma \left( \alpha \right) }{x}^{\alpha  - 1}{\mathrm{e}}^{-{\lambda x}}, & x > 0, \\  0, & \text{ 其他. } \end{array}\right.  \tag{6.3.4}
$$
则称 $X$ 服从参数为 $\alpha  > 0$ 和 $\lambda  > 0$ 的 $\Gamma$ 分布, 记为 $X \sim  \Gamma \left( {\alpha,\lambda }\right)$, R 软件中的分布名为 gamma. 
此时
$$
E\left\lbrack  X\right\rbrack   = \frac{\alpha }{\lambda },\;\operatorname{Var}\left\lbrack  X\right\rbrack   = \frac{\alpha }{{\lambda }^{2}}. \tag{6.3.5}
$$

[[Gamma分布期望与方差的计算过程]]