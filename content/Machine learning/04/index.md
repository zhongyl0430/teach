
# Model Selection {#model-selection .unnumbered}

A key problem in the design of learning algorithms is the choice of the
hypothesis set $\mathcal{H}$ . This is known as the model selection
problem. How should the hypothesis set $\mathcal{H}$ be chosen? A rich
or complex enough hypothesis set could contain the ideal Bayes
classifier. On the other hand, learning with such a complex family
becomes a very difficult task. More generally, the choice of
$\mathcal{H}$ is subject to a trade-off that can be analyzed in terms of
the estimation and approximation errors.

Our discussion will focus on the particular case of binary
classification but much of what is discussed can be straightforwardly
extended to different tasks and loss functions.

# 4.1 Estimation and approximation errors {#estimation-and-approximation-errors .unnumbered}

Let $\mathcal{H}$ be a family of functions mapping $x$ to
$\{ - 1, + 1\}$ . The excess error of a hypothesis $h$ chosen from
$\mathcal{H}$ , that is the difference between its error
$R\left( h\right)$ and the Bayes error ${R}^{ * }$ , can be decomposed
as follows:

$$R\left( h\right) - {R}^{ * } = \underset{\text{estimation }}{\underbrace{\left( R\left( h\right) - \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right) \right) }} + \underset{\text{approximation }}{\underbrace{\left( \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right) - {R}^{ * }\right) }}. \tag{4.1}$$

The first term is called the estimation error, the second term the
approximation error. The estimation error depends on the hypothesis $h$
selected. It measures the error of $h$ with respect to the infimum of
the errors achieved by hypotheses in $\mathcal{H}$ , or that of the
best-in-class hypothesis ${h}^{ * }$ when that infimum is reached. Note
that the definition of agnostic PAC-learning is precisely based on the
estimation error.

The approximation error measures how well the Bayes error can be
approximated using $\mathcal{H}$ . It is a property of the hypothesis
set $\mathcal{H}$ , a measure of its richness. For a more complex or
richer hypothesis $\mathcal{H}$ , the approximation error tends to be
smaller at the price of a larger estimation error. This is illustrated
by Figure 4.1.

::: center
![image](images/019145d2-cc04-715a-aec7-5f9a00e87681_34_676100.jpg){width="30%"}
:::

Figure 4.1

Illustration of the estimation error (in green) and approximation error
(in orange). Here, it is assumed that there exists a best-in-class
hypothesis, that is ${h}^{ * }$ such that
$R\left( {h}^{ * }\right) = \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right)$
.

Model selection consists of choosing $\mathcal{H}$ with a favorable
trade-off between the approximation and estimation errors. Note,
however, that the approximation error is not accessible, since in
general the underlying distribution $\mathcal{D}$ needed to determine
${R}^{ * }$ is not known. Even with various noise assumptions,
estimating the approximation error is difficult. In contrast, the
estimation error of an algorithm $\mathcal{A}$ , that is, the estimation
error of the hypothesis ${h}_{S}$ returned after training on a sample
$S$ , can sometimes be bounded using generalization bounds as shown in
the next section.

# 4.2 Empirical risk minimization (ERM) {#empirical-risk-minimization-erm .unnumbered}

A standard algorithm for which the estimation error can be bounded is
Empirical Risk Minimization (ERM). ERM seeks to minimize the error on
the training sample: ${}^{4}$

$${h}_{S}^{\mathrm{{ERM}}} = \mathop{\operatorname{argmin}}\limits_{{h \in \mathcal{H}}}{\widehat{R}}_{S}\left( h\right) . \tag{4.2}$$

Proposition 4.1 For any sample $S$ , the following inequality holds for
the hypothesis returned by ERM:

$$\mathbb{P}\left\lbrack {R\left( {h}_{S}^{\mathrm{{ERM}}}\right) - \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right) > \epsilon }\right\rbrack \leq \mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{h \in \mathcal{H}}}\left| {R\left( h\right) - {\widehat{R}}_{S}\left( h\right) }\right| > \frac{\epsilon }{2}}\right\rbrack . \tag{4.3}$$

Proof: By definition of
$\mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right)$ , for any
$\epsilon > 0$ , there exists ${h}_{\epsilon }$ such that
$R\left( {h}_{\epsilon }\right) \leq \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right) + \epsilon$
. Thus, using
${\widehat{R}}_{S}\left( {h}_{S}^{\mathrm{{ERM}}}\right) \leq {\widehat{R}}_{S}\left( {h}_{\epsilon }\right)$
, which holds by the

::: center
![image](images/019145d2-cc04-715a-aec7-5f9a00e87681_35_270236.jpg){width="60%"}
:::

Figure 4.2

Illustration of the decomposition of a rich family
$\mathcal{H} = \mathop{\bigcup }\limits_{{\gamma \in \Gamma }}{\mathcal{H}}_{\gamma }$
.

definition of the algorithm, we can write

$$R\left( {h}_{S}^{\mathrm{{ERM}}}\right) - \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right) = R\left( {h}_{S}^{\mathrm{{ERM}}}\right) - R\left( {h}_{\epsilon }\right) + R\left( {h}_{\epsilon }\right) - \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right)$$

$$\leq R\left( {h}_{S}^{\mathrm{{ERM}}}\right) - R\left( {h}_{\epsilon }\right) + \epsilon$$

$$= R\left( {h}_{S}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{S}\left( {h}_{S}^{\mathrm{{ERM}}}\right) + {\widehat{R}}_{S}\left( {h}_{S}^{\mathrm{{ERM}}}\right) - R\left( {h}_{\epsilon }\right) + \epsilon$$

$$\leq R\left( {h}_{S}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{S}\left( {h}_{S}^{\mathrm{{ERM}}}\right) + {\widehat{R}}_{S}\left( {h}_{\epsilon }\right) - R\left( {h}_{\epsilon }\right) + \epsilon$$

$$\leq 2\mathop{\sup }\limits_{{h \in \mathcal{H}}}\left| {R\left( h\right) - {\widehat{R}}_{S}\left( h\right) }\right| + \epsilon$$

Since the inequality holds for all $\epsilon > 0$ , it implies the
following:

$$R\left( {h}_{S}^{\mathrm{{ERM}}}\right) - \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right) \leq 2\mathop{\sup }\limits_{{h \in \mathcal{H}}}\left| {R\left( h\right) - {\widehat{R}}_{S}\left( h\right) }\right| ,$$

which concludes the proof.

The right-hand side of (4.3) can be upper-bounded using the
generalization bounds presented in the previous chapter in terms of the
Rademacher complexity, the growth function, or the VC-dimension of
$\mathcal{H}$ . In particular, it can be bounded by
$2{e}^{-{2m}{\left\lbrack \epsilon - {\Re }_{m}\left( \mathcal{H}\right) \right\rbrack }^{2}}$
. Thus, when $\mathcal{H}$ admits a favorable Rademacher complexity, for
example a finite VC-dimension, for a sufficiently large sample, with
high probability, the estimation error is guaranteed to be small.
Nevertheless, the performance of ERM is typically very poor. This is
because the algorithm disregards the complexity of the hypothesis set
$\mathcal{H}$ : in practice, either $\mathcal{H}$ is not complex enough,
in which case the approximation error can be very large, or
$\mathcal{H}$ is very rich, in which case the bound on the estimation
error becomes very loose. Additionally, in many cases, determining the
ERM solution is computationally intractable. For example, finding a
linear hypothesis with the smallest error on the training sample is
NP-hard, as a function of the dimension of the space.

::: center
![image](images/019145d2-cc04-715a-aec7-5f9a00e87681_36_798890.jpg){width="50%"}
:::

Figure 4.3

Choice of ${\gamma }^{ * }$ with the most favorable trade-off between
estimation and approximation errors.

# 4.3 Structural risk minimization (SRM) {#structural-risk-minimization-srm .unnumbered}

In the previous section, we showed that the estimation error can be
sometimes bounded or estimated. But, since the approximation error
cannot be estimated, how should we choose $\mathcal{H}$ ? One way to
proceed is to choose a very complex family $\mathcal{H}$ with no
approximation error or a very small one. $\mathcal{H}$ may be too rich
for generalization bounds to hold for $\mathcal{H}$ , but suppose we can
decompose $\mathcal{H}$ as a union of increasingly complex hypothesis
sets ${\mathcal{H}}_{\gamma }$ , that is
$\mathcal{H} = \mathop{\bigcup }\limits_{{\gamma \in \Gamma }}{\mathcal{H}}_{\gamma }$
, with the complexity of ${\mathcal{H}}_{\gamma }$ increasing with
$\gamma$ , for some set $\Gamma$ . Figure 4.2 illustrates this
decomposition. The problem then consists of selecting the parameter
${\gamma }^{ * } \in \Gamma$ and thus the hypothesis set
${\mathcal{H}}_{{\gamma }^{ * }}$ with the most favorable trade-off
between estimation and approximation errors. Since these quantities are
not known, instead, as illustrated by Figure 4.3, a uniform upper bound
on their sum, the excess error (also called excess risk), can be used.

This is precisely the idea behind the Structural Risk Minimization (SRM)
method. For SRM, $\mathcal{H}$ is assumed to be decomposable into a
countable set, thus, we will write its decomposition as
$\mathcal{H} = \mathop{\bigcup }\limits_{{k \geq 1}}{\mathcal{H}}_{k}$ .
Additionally, the hypothesis sets ${\mathcal{H}}_{k}$ are assumed to be
nested: ${\mathcal{H}}_{k} \subset {\mathcal{H}}_{k + 1}$ for all
$k \geq 1$ . However, many of the results presented in this section also
hold for non-nested hypothesis sets. Thus, we will not make use of that
assumption, unless explicitly specified. SRM consists of choosing the
index ${k}^{ * } \geq 1$ and the ERM hypothesis $h$ in
${\mathcal{H}}_{{k}^{ * }}$ that minimize an upper bound on the excess
error.

::: center
![image](images/019145d2-cc04-715a-aec7-5f9a00e87681_37_857655.jpg){width="50%"}
:::

Figure 4.4

Illustration of structural risk minimization. The plots of three errors
are shown as a function of the index $k$ . Clearly, as $k$ , or
equivalently the complexity the hypothesis set ${\mathcal{H}}_{k}$ ,
increases, the training error decreases, while the penalty term
increases. SRM selects the hypothesis minimizing a bound on the
generalization error, which is a sum of the empirical error and the
penalty term.

As we shall see, the following learning bound holds for all
$h \in \mathcal{H}$ : for any $\delta > 0$ , with probability at least
$1 - \delta$ over the draw of a sample $S$ of size $m$ from
${\mathcal{D}}^{m}$ , for all $h \in {\mathcal{H}}_{k}$ and $k \geq 1$ ,

$$R\left( h\right) \leq {\widehat{R}}_{S}\left( h\right) + {\Re }_{m}\left( {\mathcal{H}}_{k\left( h\right) }\right) + \sqrt{\frac{\log k}{m}} + \sqrt{\frac{\log \frac{2}{\delta }}{2m}}.$$

Thus, to minimize the resulting bound on the excess error
$\left( {R\left( h\right) - {R}^{ * }}\right)$ , the index $k$ and the
hypothesis $h \in {\mathcal{H}}_{k}$ should be chosen to minimize the
following objective

function:

$${F}_{k}\left( h\right) = {\widehat{R}}_{S}\left( h\right) + {\Re }_{m}\left( {\mathcal{H}}_{k}\right) + \sqrt{\frac{\log k}{m}}.$$

This is precisely the definition of the SRM solution
${h}_{S}^{\mathrm{{SRM}}}$ :

$${h}_{S}^{\mathrm{{SRM}}} = \mathop{\operatorname{argmin}}\limits_{{k \geq 1,h \in {\mathcal{H}}_{k}}}{F}_{k}\left( h\right) = \mathop{\operatorname{argmin}}\limits_{{k \geq 1,h \in {\mathcal{H}}_{k}}}{\widehat{R}}_{S}\left( h\right) + {R}_{m}\left( {\mathcal{H}}_{k}\right) + \sqrt{\frac{\log k}{m}}. \tag{4.4}$$

Thus, SRM identifies an optimal index ${k}^{ * }$ and therefore
hypothesis set ${\mathcal{H}}_{{k}^{ * }}$ , and returns the ERM
solution based on that hypothesis set. Figure 4.4 further illustrates
the selection of the index ${k}^{ * }$ and hypothesis set
${\mathcal{H}}_{{k}^{ * }}$ by SRM by minimizing an upper bound on the
sum of the training error and the penalty term
${R}_{m}\left( {\mathcal{H}}_{k}\right) + \sqrt{\log k/m}$ . The
following theorem shows that the SRM solution benefits from a strong
learning guarantee. For any $h \in \mathcal{H}$ , we will denote by
${\mathcal{H}}_{k\left( h\right) }$ the least complex hypothesis set
among the ${\mathcal{H}}_{k}\mathrm{\;s}$ that contain $h$ .

Theorem 4.2 (SRM Learning guarantee) For any $\delta > 0$ , with
probability at least $1 - \delta$ over the draw of an i.i.d. sample $S$
of size $m$ from ${\mathcal{D}}^{m}$ , the generalization error of the
hypothesis ${h}_{S}^{\mathrm{{SRM}}}$ returned by the SRM method is
bounded as follows:

$$R\left( {h}_{S}^{\mathrm{{SRM}}}\right) \leq \mathop{\inf }\limits_{{h \in \mathcal{H}}}\left( {R\left( h\right) + 2{\Re }_{m}\left( {\mathcal{H}}_{k\left( h\right) }\right) + \sqrt{\frac{\log k\left( h\right) }{m}}}\right) + \sqrt{\frac{2\log \frac{3}{\delta }}{m}}.$$

Proof: Observe first that, by the union bound, the following general
inequality holds:

$$\mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{h \in \mathcal{H}}}R\left( h\right) - {F}_{k\left( h\right) }\left( h\right) > \epsilon }\right\rbrack$$

$$= \mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{k \geq 1}}\mathop{\sup }\limits_{{h \in {\mathcal{H}}_{k}}}R\left( h\right) - {F}_{k}\left( h\right) > \epsilon }\right\rbrack$$

$$\leq \mathop{\sum }\limits_{{k = 1}}^{\infty }\mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{h \in {\mathcal{H}}_{k}}}R\left( h\right) - {F}_{k}\left( h\right) > \epsilon }\right\rbrack$$

$$= \mathop{\sum }\limits_{{k = 1}}^{\infty }\mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{h \in {\mathcal{H}}_{k}}}R\left( h\right) - {\widehat{R}}_{S}\left( h\right) - {\Re }_{m}\left( {\mathcal{H}}_{k}\right) > \epsilon + \sqrt{\frac{\log k}{m}}}\right\rbrack$$

$$\leq \mathop{\sum }\limits_{{k = 1}}^{\infty }\exp \left( {-{2m}{\left\lbrack \epsilon + \sqrt{\frac{\log k}{m}}\right\rbrack }^{2}}\right) \tag{4.5}$$

$$\leq \mathop{\sum }\limits_{{k = 1}}^{\infty }{e}^{-{2m}{\epsilon }^{2}}{e}^{-2\log k}$$

$$= {e}^{-{2m}{\epsilon }^{2}}\mathop{\sum }\limits_{{k = 1}}^{\infty }\frac{1}{{k}^{2}} = \frac{{\pi }^{2}}{6}{e}^{-{2m}{\epsilon }^{2}} \leq 2{e}^{-{2m}{\epsilon }^{2}}.$$

Next, for any two random variables ${X}_{1}$ and ${X}_{2}$ , if
${X}_{1} + {X}_{2} > \epsilon$ , then either ${X}_{1}$ or ${X}_{2}$ must
be larger than $\epsilon /2$ . In view of that, by the union bound,
$\mathbb{P}\left\lbrack {{X}_{1} + {X}_{2} > \epsilon }\right\rbrack \leq$
$\mathbb{P}\left\lbrack {{X}_{1} > \frac{\epsilon }{2}}\right\rbrack + \mathbb{P}\left\lbrack {{X}_{2} > \frac{\epsilon }{2}}\right\rbrack$
. Using this inequality, inequality (4.5), and the inequality
${F}_{k\left( {h}_{S}^{\mathrm{{SRM}}}\right) }\left( {h}_{S}^{\mathrm{{SRM}}}\right) \leq {F}_{k\left( h\right) }\left( h\right)$
, which holds for all $h \in \mathcal{H}$ , by definition of
${h}_{S}^{\mathrm{{SRM}}}$ , we can write, for any $h \in \mathcal{H}$ ,

$$\mathbb{P}\left\lbrack {R\left( {h}_{S}^{\mathrm{{SRM}}}\right) - R\left( h\right) - 2{\Re }_{m}\left( {\mathcal{H}}_{k\left( h\right) }\right) - \sqrt{\frac{\log k\left( h\right) }{m}} > \epsilon }\right\rbrack$$

$$\leq \mathbb{P}\left\lbrack {R\left( {h}_{S}^{\mathrm{{SRM}}}\right) - {F}_{k\left( {h}_{S}^{\mathrm{{SRM}}}\right) }\left( {h}_{S}^{\mathrm{{SRM}}}\right) > \frac{\epsilon }{2}}\right\rbrack$$

$$+ \mathbb{P}\left\lbrack {{F}_{k\left( {h}_{S}^{\mathrm{{SRM}}}\right) }\left( {h}_{S}^{\mathrm{{SRM}}}\right) - R\left( h\right) - 2{\Re }_{m}\left( {\mathcal{H}}_{k\left( h\right) }\right) - \sqrt{\frac{\log k\left( h\right) }{m}} > \frac{\epsilon }{2}}\right\rbrack$$

$$\leq 2{e}^{-\frac{m{\epsilon }^{2}}{2}} + \mathbb{P}\left\lbrack {{F}_{k\left( h\right) }\left( h\right) - R\left( h\right) - 2{\Re }_{m}\left( {\mathcal{H}}_{k\left( h\right) }\right) - \sqrt{\frac{\log k\left( h\right) }{m}} > \frac{\epsilon }{2}}\right\rbrack$$

$$= 2{e}^{-\frac{m{\epsilon }^{2}}{2}} + \mathbb{P}\left\lbrack {{\widehat{R}}_{S}\left( h\right) - R\left( h\right) - {\Re }_{m}\left( {\mathcal{H}}_{k\left( h\right) }\right) > \frac{\epsilon }{2}}\right\rbrack$$

$$= 2{e}^{-\frac{m{\epsilon }^{2}}{2}} + {e}^{-\frac{m{\epsilon }^{2}}{2}} = 3{e}^{-\frac{m{\epsilon }^{2}}{2}}.$$

Setting the right-hand side to be equal to $\delta$ completes the proof.

The learning guarantee just proven for SRM is remarkable. To simplify
its discussion, let us assume that there exists ${h}^{ * }$ such that
$R\left( {h}^{ * }\right) = \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right)$
, that is, that there exists a best-in-class classifier
${h}^{ * } \in \mathcal{H}$ . Then, the theorem implies in particular
that, with probability at least $1 - \delta$ , the following inequality
holds for all $h \in \mathcal{H}$ :

$$R\left( {h}_{S}^{\mathrm{{SRM}}}\right) \leq R\left( {h}^{ * }\right) + 2{\Re }_{m}\left( {\mathcal{H}}_{k\left( {h}^{ * }\right) }\right) + \sqrt{\frac{\log k\left( {h}^{ * }\right) }{m}} + \sqrt{\frac{2\log \frac{3}{\delta }}{m}}. \tag{4.6}$$

Observe that, remarkably, this bound is similar to the estimation error
bound for ${\mathcal{H}}_{k\left( {h}^{ * }\right) }$ : it differs from
it only by the term $\sqrt{\log k\left( {h}^{ * }\right) /m}$ . Thus,
modulo that term, the guarantee for SRM is as favorable as the one we
would have obtained, had an oracle informed us of the index
$k\left( {h}^{ * }\right)$ of the best-in-class classifier's hypothesis
set.

Furthermore, observe that when $\mathcal{H}$ is rich enough that
$R\left( {h}^{ * }\right)$ is close to the Bayes error, the learning
bound (4.6) is approximately a bound on the excess error of the SRM
solution. Note that, if for some ${k}_{0}$ , the empirical error of the
ERM solution for ${\mathcal{H}}_{{k}_{0}}$ is zero, which holds in
particular if ${\mathcal{H}}_{{k}_{0}}$ contains the Bayes error, then,
we have
$\mathop{\min }\limits_{{h \in {\mathcal{H}}_{k}}}{F}_{{k}_{0}}\left( h\right) \leq \mathop{\min }\limits_{{h \in {\mathcal{H}}_{k}}}{F}_{k}\left( h\right)$
for all $k > {k}_{0}$ and only finitely many indices need to be
considered in SRM.

Assume more generally that if
$\mathop{\min }\limits_{{h \in {\mathcal{H}}_{k}}}{F}_{k}\left( h\right) \leq \mathop{\min }\limits_{{h \in {\mathcal{H}}_{k + 1}}}{F}_{k}\left( h\right)$
for some $k$ , then indices beyond $k + 1$ need not be inspected. This
property may hold for example if the empirical error cannot be further
improved after some index $k$ . In that case, the minimizing index
${k}^{ * }$ can be determined via a binary search in the interval
$\left\lbrack {1,{k}_{\max }}\right\rbrack$ , given some maximum value
${k}_{\max }.{k}_{\max }$ itself can be found by inspecting
$\mathop{\min }\limits_{{h \in {\mathcal{H}}_{{2}^{n}}}}{F}_{k}\left( h\right)$
for exponentially growing indices ${2}^{n},n \geq 1$ , and setting
${k}_{\max } = {2}^{n}$ for $n$ such that
$\mathop{\min }\limits_{{h \in {\mathcal{H}}_{{2}^{n}}}}{F}_{k}\left( h\right) \leq \mathop{\min }\limits_{{h \in {\mathcal{H}}_{{2}^{n + 1}}}}{F}_{k}\left( h\right)$
. The number of ERM computations needed to find ${k}_{\max }$ is in
$O\left( n\right) = O\left( {\log {k}_{\max }}\right)$ and similarly the
number of ERM computations due to the binary search is in
$O\left( {\log {k}_{\max }}\right)$ . Thus, if $n$ is the smallest
integer such that ${k}^{ * } < {2}^{n}$ , the overall number of ERM
computations is in $O\left( {\log {k}^{ * }}\right)$ .

While it benefits from a very favorable guarantee, SRM admits several
drawbacks. First, the decomposability of $\mathcal{H}$ into countably
many hypothesis sets, each with a converging Rademacher complexity,
remains a strong assumption. As an example, the family of all measurable
functions cannot be written as a union of countably many hypothesis sets
with finite VC-dimension. Thus, the choice of $\mathcal{H}$ or that of
the hypothesis sets ${\mathcal{H}}_{k}$ is a key component of SRM.
Second, and this is the main disadvantage of SRM, the method is
typically computationally intractable: for most hypothesis sets, finding
the solution of ERM is NP-hard and in general SRM requires determining
that solution for a large number of indices $k$ .

# 4.4 Cross-validation {#cross-validation .unnumbered}

An alternative method for model selection, cross-validation, consists of
using some fraction of the training sample as a validation set to select
a hypothesis set ${\mathcal{H}}_{k}$ . This is in contrast with the SRM
model which relies on a theoretical learning bound assigning a penalty
to each hypothesis set. In this section, we analyze the cross-validation
method and compare its performance to that of SRM.

As in the previous section, let
${\left( {\mathcal{H}}_{k}\right) }_{k \geq 1}$ be a countable sequence
of hypothesis sets with increasing complexities. The cross-validation
(CV) solution is obtained as follows. Let $S$ be an i.i.d. labeled
sample of size $m.S$ is divided into a sample ${S}_{1}$ of size
$\left( {1 - \alpha }\right) m$ and a sample ${S}_{2}$ of size
${\alpha m}$ , with $\alpha \in \left( {0,1}\right)$ typically chosen to
be relatively small. ${S}_{1}$ is reserved for training, ${S}_{2}$ for
validation. For any $k \in \mathbb{N}$ , let
${h}_{{S}_{1},k}^{\mathrm{{ERM}}}$ denote the solution of ERM run on
${S}_{1}$ using the hypothesis set ${\mathcal{H}}_{k}$ . The hypothesis
${h}_{S}^{\mathrm{{CV}}}$ returned by cross-validation is the ERM
solution ${h}_{{S}_{1},k}^{\mathrm{{ERM}}}$ with the best performance on
${S}_{2}$ :

$${h}_{S}^{\mathrm{{CV}}} = \mathop{\operatorname{argmin}}\limits_{{h \in \left\{ {{h}_{{S}_{1},k}^{\mathrm{{ENM}}} : k \geq 1}\right\} }}{\widehat{R}}_{{S}_{2}}\left( h\right) . \tag{4.7}$$

The following general result will help us derive learning guarantees for
cross-validation.

Proposition 4.3 For any $\alpha > 0$ and any sample size $m \geq 1$ ,
the following general inequality holds:

$$\mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{k \geq 1}}\left| {R\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{{S}_{2}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) }\right| > \epsilon + \sqrt{\frac{\log k}{\alpha m}}}\right\rbrack \leq 4{e}^{-{2\alpha m}{\epsilon }^{2}}.$$

Proof: By the union bound, we can write

$$\mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{k \geq 1}}\left| {R\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{{S}_{2}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) }\right| > \epsilon + \sqrt{\frac{\log k}{\alpha m}}}\right\rbrack$$

$$\leq \mathop{\sum }\limits_{{k = 1}}^{\infty }\mathbb{P}\left\lbrack {\left| {R\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{{S}_{2}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) }\right| > \epsilon + \sqrt{\frac{\log k}{\alpha m}}}\right\rbrack \tag{4.8}$$

$$= \mathop{\sum }\limits_{{k = 1}}^{\infty }\mathbb{E}\left\lbrack {\mathbb{P}\left\lbrack {\left| {R\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{{S}_{2}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) }\right| > \epsilon + \sqrt{\frac{\log k}{\alpha m}} \mid {S}_{1}}\right\rbrack }\right\rbrack .$$

The hypothesis ${h}_{{S}_{1},k}^{\mathrm{{ERM}}}$ is fixed conditioned
on ${S}_{1}$ . Furthermore, the sample ${S}_{2}$ is independent from
${S}_{1}$ . Therefore, by Hoeffding's inequality, we can bound the
conditional probability as follows:

$$\mathbb{P}\left\lbrack {\left| {R\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{{S}_{2}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) }\right| > \epsilon + \sqrt{\frac{\log k}{\alpha m}} \mid {S}_{1}}\right\rbrack \leq 2{e}^{-{2\alpha m}{\left( \epsilon + \sqrt{\frac{\log k}{\alpha m}}\right) }^{2}}.$$

$$\leq 2{e}^{-{2\alpha m}{\epsilon }^{2} - 2\log k}$$

$$= \frac{2}{{k}^{2}}{e}^{-{2\alpha m}{\epsilon }^{2}}.$$

Plugging in the right-hand side of this bound in (4.8) and summing over
$k$ yields

$$\mathbb{P}\left\lbrack {\mathop{\sup }\limits_{{k \geq 1}}\left| {R\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) - {\widehat{R}}_{{S}_{2}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) }\right| > \epsilon + \sqrt{\frac{\log k}{\alpha m}}}\right\rbrack \leq \frac{{\pi }^{2}}{3}{e}^{-{2\alpha m}{\epsilon }^{2}} < 4{e}^{-{2\alpha m}{\epsilon }^{2}},$$

which completes the proof.

Let $R\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right)$ be the
generalization error of the SRM solution using a sample ${S}_{1}$ of
size $\left( {1 - {\alpha m}}\right)$ and
$R\left( {{h}_{S}^{\mathrm{{CV}}},S}\right)$ the generalization error of
the cross-validation solution using a sample $S$ of size $m$ . Then,
using Proposition 4.3, the following learning guarantee can be derived
which compares the error of the CV method to that of SRM.

Theorem 4.4 (Cross-validation versus SRM) For any $\delta > 0$ , with
probability at least $1 - \delta$ , the following holds:

$$R\left( {h}_{S}^{\mathrm{{CV}}}\right) - R\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right) \leq 2\sqrt{\frac{\log \max \left( {k\left( {h}_{S}^{\mathrm{{CV}}}\right) ,k\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right) }\right) }{\alpha m}} + 2\sqrt{\frac{\log \frac{4}{\delta }}{2\alpha m}},$$

where, for any $h,k\left( h\right)$ denotes the smallest index of a
hypothesis set containing $h$ . Proof: By Proposition 4.3 and Theorem
4.2, using the property of ${h}_{S}^{\mathrm{{CV}}}$ as a minimizer, for
any $\delta > 0$ , with probability at least $1 - \delta$ , the
following inequalities

hold:

$$R\left( {h}_{S}^{\mathrm{{CV}}}\right) \leq {\widehat{R}}_{{S}_{2}}\left( {h}_{S}^{\mathrm{{CV}}}\right) + \sqrt{\frac{\log \left( {k\left( {h}_{S}^{\mathrm{{CV}}}\right) }\right) }{\alpha m}} + \sqrt{\frac{\log \frac{4}{\delta }}{2\alpha m}}$$

$$\leq {\widehat{R}}_{{S}_{2}}\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right) + \sqrt{\frac{\log \left( {k\left( {h}_{S}^{\mathrm{{CV}}}\right) }\right) }{\alpha m}} + \sqrt{\frac{\log \frac{4}{\delta }}{2\alpha m}}$$

$$\leq R\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right) + \sqrt{\frac{\log \left( {k\left( {h}_{S}^{\mathrm{{CV}}}\right) }\right) }{\alpha m}} + \sqrt{\frac{\log \left( {k\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right) }\right) }{\alpha m}} + 2\sqrt{\frac{\log \frac{4}{\delta }}{2\alpha m}}$$

$$\leq R\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right) + 2\sqrt{\frac{\log \left( {\max \left( {k\left( {h}_{S}^{\mathrm{{CV}}}\right) ,k\left( {h}_{{S}_{1}}^{\mathrm{{SRM}}}\right) }\right) }\right) }{\alpha m}} + 2\sqrt{\frac{\log \frac{4}{\delta }}{2\alpha m}},$$

which completes the proof.

The learning guarantee just proven shows that, with high probability,
the generalization error of the CV solution for a sample of size $m$ is
close to that of the SRM solution for a sample of size
$\left( {1 - \alpha }\right) m$ . For $\alpha$ relatively small, this
suggests a guarantee similar to that of SRM, which, as previously
discussed, is very favorable. However, in some unfavorable regimes, an
algorithm (here SRM) trained on $\left( {1 - \alpha }\right) m$ points
may have a significantly worse performance than when trained on $m$
points (avoiding this phase transition issue is one of the main
motivations behind the use of the $n$ -fold cross-validation method in
practice, see section 4.5). Thus, the bound suggests in fact a
trade-off: $\alpha$ should be chosen sufficiently small to avoid the
unfavorable regimes just mentioned and yet sufficiently large for the
right-hand side of the bound to be small and thus informative.

The learning bound for CV can be made more explicit in some cases in
practice. Assume for example that the hypothesis sets
${\mathcal{H}}_{k}$ are nested and that the empirical errors of the ERM
solutions ${h}_{{S}_{1},k}^{\mathrm{{ERM}}}$ are decreasing before
reaching zero: for any $k$ ,
${\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},k + 1}^{\mathrm{{ERM}}}\right) < {\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right)$
for all $k$ such that
${\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) > 0$
and
${\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},k + 1}^{\mathrm{{ERM}}}\right) \leq$
${\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right)$
otherwise. Observe that
${\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) > 0$
implies at least one error for ${h}_{{S}_{1},k}^{\mathrm{{ERM}}}$ ,
therefore
${\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},k}^{\mathrm{{ERM}}}\right) > \frac{1}{m}$
. In view of that, we must then have
${\widehat{R}}_{{S}_{1}}\left( {h}_{{S}_{1},n}^{\mathrm{{ERM}}}\right) =$
0 for all $n \geq m + 1$ . Thus, we have
${h}_{{S}_{1},n}^{\mathrm{{ERM}}} = {h}_{{S}_{1},m + 1}^{\mathrm{{ERM}}}$
for all $n \geq m + 1$ and we can assume that
$k\left( {f}_{CV}\right) \leq m + 1$ . Since the complexity of
${\mathcal{H}}_{k}$ increases with $k$ we also have
$k\left( {f}_{SRM}\right) \leq m + 1$ . In view of that, we obtain the
following more explicit learning bound for cross-validation:

$$R\left( {{f}_{CV},S}\right) - R\left( {{f}_{SRM},{S}_{1}}\right) \leq 2\sqrt{\frac{\log \left( \frac{4}{\delta }\right) }{2\alpha m}} + 2\sqrt{\frac{\log \left( {m + 1}\right) }{\alpha m}}.$$

# 4.5 $n$ -Fold cross-validation {#n--fold-cross-validation .unnumbered}

In practice, the amount of labeled data available is often too small to
set aside a validation sample since that would leave an insufficient
amount of training data. Instead, a widely adopted method known as
n-fold cross-validation is used to exploit the labeled data both for
model selection and for training.

Let $\mathbf{\theta }$ denote the vector of free parameters of the
algorithm. For a fixed value of $\mathbf{\theta }$ , the method consists
of first randomly partitioning a given sample $S$ of $m$ labeled
examples into $n$ subsamples, or folds. The $i$ th fold is thus a
labeled sample
$\left( {\left( {{x}_{i1},{y}_{i1}}\right) ,\ldots ,\left( {{x}_{i{m}_{i}},{y}_{i{m}_{i}}}\right) }\right)$
of size ${m}_{i}$ . Then, for any $i \in \left\lbrack n\right\rbrack$ ,
the learning algorithm is trained on all but the $i$ th fold to generate
a hypothesis ${h}_{i}$ , and the performance of ${h}_{i}$ is tested on
the $i$ th fold, as illustrated in figure 4.5a. The parameter value
$\mathbf{\theta }$ is evaluated based on the average error of the
hypotheses ${h}_{i}$ , which is called the cross-validation error. This
quantity is denoted by
${\widehat{R}}_{\mathrm{{CV}}}\left( \mathbf{\theta }\right)$ and
defined by

$${\widehat{R}}_{\mathrm{{CV}}}\left( \mathbf{\theta }\right) = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\underset{\text{error of }{h}_{i}\text{ on the }i\text{ th fold }}{\underbrace{\frac{1}{{m}_{i}}\mathop{\sum }\limits_{{j = 1}}^{{m}_{i}}L\left( {{h}_{i}\left( {x}_{ij}\right) ,{y}_{ij}}\right) }}.$$

The folds are generally chosen to have equal size, that is
${m}_{i} = m/n$ for all $i \in \left\lbrack n\right\rbrack$ . How should
$n$ be chosen? The appropriate choice is subject to a trade-off. For a
large $n$ , each training sample used in $n$ -fold cross-validation has
size $m - m/n =$ $m\left( {1 - 1/n}\right)$ (illustrated by the right
vertical red line in figure 4.5b), which is close to $m$ , the size of
the full sample, and also implies all training samples are quite
similar. At the same time, the $i$ th fold used to measure the error is
relatively small and thus the cross-validation error tends to have a
small bias but a large variance. In contrast, smaller values of $n$ lead
to more diverse training samples but their size (shown by the left
vertical red line in figure 4.5b) is significantly less than $m$ . In
this regime, the ith fold is relatively large and thus the
cross-validation error tends to have a smaller variance but a larger
bias.

In applications, $n$ is typically chosen to be 5 or 10. $n$ -fold
cross-validation is used as follows in model selection. The full labeled
data is first split into a training and a test sample. The training
sample of size $m$ is then used to compute the $n$ - fold
cross-validation error
${\widehat{R}}_{\mathrm{{CV}}}\left( \mathbf{\theta }\right)$ for a
small number of possible values of $\mathbf{\theta }$ . The free
parameter $\mathbf{\theta }$ is next set to the value
${\mathbf{\theta }}_{0}$ for which
${\widehat{R}}_{\mathrm{{CV}}}\left( \mathbf{\theta }\right)$ is
smallest and the algorithm is trained with the parameter setting
${\mathbf{\theta }}_{0}$ over the full training sample of size $m$ . Its
performance is evaluated on the test sample as already described in the
previous section.

The special case of $n$ -fold cross-validation where $n = m$ is called
leave-one-out cross-validation, since at each iteration exactly one
instance is left out of the training sample. As shown in chapter 5, the
average leave-one-out error is an approximately unbiased estimate of the
average error of an algorithm and can be used to derive simple
guarantees for some algorithms. In general, the leave-one-out error is
very costly to compute, since it requires training $m$ times on samples
of size $m - 1$ , but for some algorithms it admits a very efficient
computation (see exercise 11.9).

::: center
![image](images/019145d2-cc04-715a-aec7-5f9a00e87681_44_344163.jpg){width="60%"}
:::

Figure 4.5

$n$ -fold cross-validation. (a) Illustration of the partitioning of the
training data into 5 folds. (b) Typical plot of a classifier's
prediction error as a function of the size of the training sample $m$ :
the error decreases as a function of the number of training points. The
red line on the left side marks the region for small values of $n$ ,
while the red line on the right side marks the region for large values
of $n$ .

In addition to model selection, $n$ -fold cross-validation is also
commonly used for performance evaluation. In that case, for a fixed
parameter setting $\mathbf{\theta }$ , the full labeled sample is
divided into $n$ random folds with no distinction between training and
test samples. The performance reported is the $n$ -fold cross-validation
error on the full sample as well as the standard deviation of the errors
measured on each fold.

# 4.6 Regularization-based algorithms {#regularization-based-algorithms .unnumbered}

A broad family of algorithms inspired by the SRM method is that of
regularization-based algorithm. This consists of selecting a very
complex family $\mathcal{H}$ that is an uncountable union of nested
hypothesis sets
${\mathcal{H}}_{\gamma } : \mathcal{H} = \mathop{\bigcup }\limits_{{\gamma > 0}}{\mathcal{H}}_{\gamma }$
. $\mathcal{H}$ is often chosen to be dense in the space of continuous
functions over $x$ . For example, $\mathcal{H}$ may be chosen to be the
set of all linear functions in some high-dimensional space and
${\mathcal{H}}_{\gamma }$ the subset of those functions whose norm is
bounded by $\gamma : {\mathcal{H}}_{\gamma } = \{ x \mapsto$
$\mathbf{w} \cdot \mathbf{\Phi }\left( x\right) : \parallel \mathbf{w}\parallel \leq \gamma \}$
. For some choices of $\mathbf{\Phi }$ and the high-dimensional space,
it can be shown that $\mathcal{H}$ is indeed dense in the space of
continuous functions over $x$ .

Given a labeled sample $S$ , the extension of the SRM method to an
uncountable union would then suggest selecting $h$ based on the
following optimization problem:

$$\mathop{\operatorname{argmin}}\limits_{{\gamma > 0,h \in {H}_{\gamma }}}{\widehat{R}}_{S}\left( h\right) + {\Re }_{m}\left( {\mathcal{H}}_{\gamma }\right) + \sqrt{\frac{\log \gamma }{m}}$$

where other penalty terms pen $\left( {\gamma ,m}\right)$ can be chosen
in lieu of the specific choice
$\operatorname{pen}\left( {\gamma ,m}\right) = {\mathfrak{R}}_{m}\left( {\mathcal{H}}_{\gamma }\right) + \sqrt{\frac{\log \gamma }{m}}$
. Often, there exists a function
$\mathcal{R} : \mathcal{H} \rightarrow \mathbb{R}$ such that, for any
$\gamma > 0$ , the constrained optimization problem
${\operatorname{argmin}}_{\gamma > 0,h \in {H}_{\gamma }}{\widehat{R}}_{S}\left( h\right) +$
$\operatorname{pen}\left( {\gamma ,m}\right)$ can be equivalently
written as the unconstrained optimization problem

$$\mathop{\operatorname{argmin}}\limits_{{h \in \mathcal{H}}}{\widehat{R}}_{S}\left( h\right) + \lambda \mathcal{R}\left( h\right)$$

for some $\lambda > 0.\mathcal{R}\left( h\right)$ is called a
regularization term and $\lambda > 0$ is treated as a hyperparameter
since its optimal value is often not known. For most algorithms, the
regularization term $\mathcal{R}\left( h\right)$ is chosen to be an
increasing function of $\parallel h\parallel$ for some choice of the
norm $\parallel \cdot \parallel$ , when $\mathcal{H}$ is the subset of a
Hilbert space. The variable $\lambda$ is often called a regularization
parameter. Larger values of $\lambda$ further penalize more complex
hypotheses, while, for $\lambda$ close or equal to zero, the
regularization term has no effect and the algorithm coincides with ERM.
In practice, $\lambda$ is typically selected via cross-validation or
using $n$ -fold cross-validation.

When the regularization term is chosen to be
$\parallel h{\parallel }_{p}$ for some choice of the norm and $p \geq 1$
, then it is a convex function of $h$ , since any norm is convex.
However, for the zero-one loss, the first term of the objective function
is non-convex, thereby making the optimization problem computationally
hard. In practice, most regularization-based algorithms instead use a
convex upper bound on the zero-one loss and replace the empirical
zero-one term with the empirical value of that convex surrogate. The
resulting optimization problem is then convex and therefore admits more
efficient solutions than SRM. The next section studies the properties of
such convex surrogate losses.

# 4.7 Convex surrogate losses {#convex-surrogate-losses .unnumbered}

The guarantees for the estimation error that we presented in previous
sections hold either for ERM or for SRM, which itself is defined in
terms of ERM. However, as already mentioned, for many choices of the
hypothesis set $\mathcal{H}$ , including that of linear functions,
solving the ERM optimization problem is NP-hard mainly because the
zero-one loss function is not convex. One common method for addressing
this problem consists of using a convex surrogate loss function that
upper bounds the zero-one loss. This section analyzes learning
guarantees for such surrogate losses in terms of the original loss.

The hypotheses we consider are real-valued functions
$h : X \rightarrow \mathbb{R}$ . The sign of $h$ defines a binary
classifier ${f}_{h} : \mathcal{X} \rightarrow \{ - 1, + 1\}$ defined for
all $x \in \mathcal{X}$ by

$${f}_{h}\left( x\right) = \left\{ \begin{array}{ll} + 1 & \text{ if }h\left( x\right) \geq 0 \\ - 1 & \text{ if }h\left( x\right) < 0 \end{array}\right.$$

The loss or error of $h$ at point
$\left( {x,y}\right) \in \mathfrak{X} \times \{ - 1, + 1\}$ is defined
as the binary classification error of ${f}_{h}$ :

$${1}_{{f}_{h}\left( x\right) \neq y} = {1}_{{yh}\left( x\right) < 0} + {1}_{h\left( x\right) = 0 \land y = - 1} \leq {1}_{{yh}\left( x\right) \leq 0}.$$

We will denote by $R\left( h\right)$ the expected error of
$h : R\left( h\right) = {\mathbb{E}}_{\left( {x,y}\right) \sim \mathcal{D}}\left\lbrack {1}_{{f}_{h}\left( x\right) \neq y}\right\rbrack$
. For any $x \in X$ , let $\eta \left( x\right)$ denote
$\eta \left( x\right) = \mathbb{P}\left\lbrack {y = + 1 \mid x}\right\rbrack$
and let ${\mathcal{D}}_{X}$ denote the marginal distribution over $X$ .
Then, for any $h$ , we can write

$$R\left( h\right) = \underset{\left( {x,y}\right) \sim \mathcal{D}}{\mathbb{E}}\left\lbrack {1}_{{f}_{h}\left( x\right) \neq y}\right\rbrack$$

$$= \underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {\eta \left( x\right) {1}_{h\left( x\right) < 0} + \left( {1 - \eta \left( x\right) }\right) {1}_{h\left( x\right) > 0} + \left( {1 - \eta \left( x\right) }\right) {1}_{h\left( x\right) = 0}}\right\rbrack$$

$$= \underset{x \sim {\mathcal{D}}_{X}}{\mathbb{E}}\left\lbrack {\eta \left( x\right) {1}_{h\left( x\right) < 0} + \left( {1 - \eta \left( x\right) }\right) {1}_{h\left( x\right) \geq 0}}\right\rbrack .$$

In view of that, the Bayes classifier can be defined as assigning label
+1 to $x$ when $\eta \left( x\right) \geq \frac{1}{2}, - 1$ otherwise.
It can therefore be induced by the function ${h}^{ * }$ defined by

$${h}^{ * }\left( x\right) = \eta \left( x\right) - \frac{1}{2}. \tag{4.9}$$

We will refer to ${h}^{ * } : X \rightarrow \mathbb{R}$ as the Bayes
scoring function and will denote by ${R}^{ * }$ the error of the Bayes
classifier or Bayes scoring function:
${R}^{ * } = R\left( {h}^{ * }\right)$ .

Lemma 4.5 The excess error of any hypothesis
$h : X \rightarrow \mathbb{R}$ can be expressed as follows in terms of
$\eta$ and the Bayes scoring function ${h}^{ * }$ :

$$R\left( h\right) - {R}^{ * } = 2\underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {\left| {{h}^{ * }\left( x\right) }\right| {1}_{h\left( x\right) {h}^{ * }\left( x\right) \leq 0}}\right\rbrack .$$

Proof: For any $h$ , we can write

$$R\left( h\right) = \underset{x \sim {\mathcal{D}}_{X}}{\mathbb{E}}\left\lbrack {\eta \left( x\right) {1}_{h\left( x\right) < 0} + \left( {1 - \eta \left( x\right) }\right) {1}_{h\left( x\right) \geq 0}}\right\rbrack$$

$$= \underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {\eta \left( x\right) {1}_{h\left( x\right) < 0} + \left( {1 - \eta \left( x\right) }\right) \left( {1 - {1}_{h\left( x\right) < 0}}\right) }\right\rbrack$$

$$= \underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {\left\lbrack {{2\eta }\left( x\right) - 1}\right\rbrack {1}_{h\left( x\right) < 0} + \left( {1 - \eta \left( x\right) }\right) }\right\rbrack$$

$$= \underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {2{h}^{ * }\left( x\right) {1}_{h\left( x\right) < 0} + \left( {1 - \eta \left( x\right) }\right) }\right\rbrack ,$$

where we used for the last step equation (4.9). In view of that, for any
$h$ , the following holds:

$$R\left( h\right) - R\left( {h}^{ * }\right) = \underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {2\left\lbrack {{h}^{ * }\left( x\right) }\right\rbrack \left( {{1}_{h\left( x\right) \leq 0} - {1}_{{h}^{ * }\left( x\right) \leq 0}}\right) }\right\rbrack$$

$$= \underset{x \sim {\mathcal{D}}_{X}}{\mathbb{E}}\left\lbrack {2\left\lbrack {{h}^{ * }\left( x\right) }\right\rbrack \operatorname{sgn}\left( {{h}^{ * }\left( x\right) }\right) {1}_{\left( {h\left( x\right) {h}^{ * }\left( x\right) \leq 0}\right) \land \left( {\left( {h\left( x\right) ,{h}^{ * }\left( x\right) }\right) \neq \left( {0,0}\right) }\right) }}\right\rbrack$$

$$= 2\underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {\left| {{h}^{ * }\left( x\right) }\right| {1}_{h\left( x\right) {h}^{ * }\left( x\right) \leq 0}}\right\rbrack ,$$

which completes the proof, since $R\left( {h}^{ * }\right) = {R}^{ * }$
.

Let $\Phi : \mathbb{R} \rightarrow \mathbb{R}$ be a convex and
non-decreasing function so that for any $u \in \mathbb{R}$ ,
${1}_{u \leq 0} \leq \Phi \left( {-u}\right)$ . The $\Phi$ -loss of a
function $h : X \rightarrow \mathbb{R}$ at point
$\left( {x,y}\right) \in X \times \{ - 1, + 1\}$ is defined as
$\Phi \left( {-{yh}\left( x\right) }\right)$ and its expected loss given
by

$${\mathcal{L}}_{\Phi }\left( h\right) = \underset{\left( {x,y}\right) \sim \mathcal{D}}{\mathbb{E}}\left\lbrack {\Phi \left( {-{yh}\left( x\right) }\right) }\right\rbrack$$

$$= \underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}\left\lbrack {\eta \left( x\right) \Phi \left( {-h\left( x\right) }\right) + \left( {1 - \eta \left( x\right) }\right) \Phi \left( {h\left( x\right) }\right) }\right\rbrack . \tag{4.10}$$

Notice that since
${1}_{{yh}\left( x\right) \leq 0} \leq \Phi \left( {-{yh}\left( x\right) }\right)$
, we have $R\left( h\right) \leq {\mathcal{L}}_{\Phi }\left( h\right)$ .
For any $x \in X$ , let $u \mapsto {L}_{\Phi }\left( {x,u}\right)$ be
the function defined for all $u \in \mathbb{R}$ by

$${L}_{\Phi }\left( {x,u}\right) = \eta \left( x\right) \Phi \left( {-u}\right) + \left( {1 - \eta \left( x\right) }\right) \Phi \left( u\right) .$$

Then,
${\mathcal{L}}_{\Phi }\left( h\right) = {\mathbb{E}}_{x \sim {\mathcal{D}}_{X}}\left\lbrack {{L}_{\Phi }\left( {x,h\left( x\right) }\right) }\right\rbrack$
. Since $\Phi$ is convex, $u \mapsto {L}_{\Phi }\left( {x,u}\right)$ is
convex as a sum of two convex functions. Define
${h}_{\Phi }^{ * } : X \rightarrow \left\lbrack {-\infty , + \infty }\right\rbrack$
as the Bayes solution for the loss function ${L}_{\Phi }$ . That is, for
any $x,{h}_{\Phi }^{ * }\left( x\right)$ is a solution of the following
convex optimization problem:

$${h}_{\Phi }^{ * }\left( x\right) = \mathop{\operatorname{argmin}}\limits_{{u \in \left\lbrack {-\infty , + \infty }\right\rbrack }}{L}_{\Phi }\left( {x,u}\right)$$

$$= \mathop{\operatorname{argmin}}\limits_{{u \in \left\lbrack {-\infty , + \infty }\right\rbrack }}\eta \left( x\right) \Phi \left( {-u}\right) + \left( {1 - \eta \left( x\right) }\right) \Phi \left( u\right) .$$

The solution of this optimization is in general not unique. When
$\eta \left( x\right) = 0,{h}_{\Phi }^{ * }\left( x\right)$ is a
minimizer of $u \mapsto \Phi \left( u\right)$ and since $\Phi$ is
non-decreasing, we can choose
${h}_{\Phi }^{ * }\left( x\right) = - \infty$ in that case. Similarly,
when $\eta \left( x\right) = 1$ , we can choose
${h}_{\Phi }^{ * }\left( x\right) = + \infty$ . When
$\eta \left( x\right) = \frac{1}{2}$ ,
${L}_{\Phi }\left( {x,u}\right) = \frac{1}{2}\left\lbrack {\Phi \left( {-u}\right) + \Phi \left( u\right) }\right\rbrack$
, thus, by convexity,
${L}_{\Phi }\left( {x,u}\right) \geq \Phi \left( {-\frac{u}{2} + \frac{u}{2}}\right) = \Phi \left( 0\right)$
. Thus, we can choose ${h}_{\Phi }^{ * }\left( x\right) = 0$ in that
case. For all other values of $\eta \left( x\right)$ , in case of
non-uniqueness, an arbitrary minimizer is chosen in this definition. We
will denote by ${\mathcal{L}}_{\Phi }^{ * }$ the $\Phi$ -loss of
${h}_{\Phi }^{ * } : {\mathcal{L}}_{\Phi }^{ * } = {\mathbb{E}}_{\left( {x,y}\right) \sim \mathcal{D}}\left\lbrack {\Phi \left( {-y{h}_{\Phi }^{ * }\left( x\right) }\right) }\right\rbrack$
.

Proposition 4.6 Let $\Phi$ be a convex and non-decreasing function that
is differentiable at 0 with ${\Phi }^{\prime }\left( 0\right) > 0$ .
Then, the minimizer of $\Phi$ defines the Bayes classifier: for any
$x \in X,{h}_{\Phi }^{ * }\left( x\right) > 0$ iff
${h}^{ * }\left( x\right) > 0$ and ${h}^{ * }\left( x\right) = 0$ iff
${h}_{\Phi }^{ * }\left( x\right) = 0$ , which implies
${\mathcal{L}}_{\Phi }^{ * } = {R}^{ * }$ . Proof: Fix $x \in X$ . If
$\eta \left( x\right) = 0$ , then
${h}^{ * }\left( x\right) = - \frac{1}{2}$ and
${h}_{\Phi }^{ * }\left( x\right) = - \infty$ , thus
${h}^{ * }\left( x\right)$ and ${h}_{\Phi }^{ * }\left( x\right)$ admit
the same sign. Similarly, if $\eta \left( x\right) = 1$ , then
${h}^{ * }\left( x\right) = + \frac{1}{2}$ and
${h}_{\Phi }^{ * }\left( x\right) = + \infty$ , and
${h}^{ * }\left( x\right)$ and ${h}_{\Phi }^{ * }\left( x\right)$ admit
the same sign.

Let ${u}^{ * }$ denote the minimizer defining
${h}_{\Phi }^{ * }\left( x\right) .{u}^{ * }$ is a minimizer of
$u \mapsto {L}_{\Phi }\left( {x,u}\right)$ iff the subdifferential of
that function at ${u}^{ * }$ contains 0, that is, since
$\partial {L}_{\Phi }\left( {x,{u}^{ * }}\right) =$
$- \eta \left( x\right) \partial \Phi \left( {-{u}^{ * }}\right) + \left( {1 - \eta \left( x\right) }\right) \partial \Phi \left( {u}^{ * }\right)$
, iff there exist ${v}_{1} \in \partial \Phi \left( {-{u}^{ * }}\right)$
and ${v}_{2} \in \partial \Phi \left( {u}^{ * }\right)$ such that

$$\eta \left( x\right) {v}_{1} = \left( {1 - \eta \left( x\right) }\right) {v}_{2} \tag{4.11}$$

If ${u}^{ * } = 0$ , by the differentiability of $\Phi$ at 0 we have
${v}_{1} = {v}_{2} = {\Phi }^{\prime }\left( 0\right) > 0$ and thus
$\eta \left( x\right) = \frac{1}{2}$ , that is
${h}^{ * }\left( x\right) = 0$ . Conversely, If
${h}^{ * }\left( x\right) = 0$ , that is
$\eta \left( x\right) = \frac{1}{2}$ , then, by definition, we have
${h}_{\Phi }^{ * }\left( x\right) = 0$ . Thus,
${h}^{ * }\left( x\right) = 0$ iff
${h}_{\Phi }^{ * }\left( x\right) = 0$ iff
$\eta \left( x\right) = \frac{1}{2}$ .

We can assume now that $\eta \left( x\right)$ is not in
$\left\{ {0,1,\frac{1}{2}}\right\}$ . We first show that for any
${u}_{1},{u}_{2} \in \mathbb{R}$ with ${u}_{1} < {u}_{2}$ , and any two
choices of the subgradients at ${u}_{1}$ and ${u}_{2}$ ,
${v}_{1} \in \partial \Phi \left( {u}_{1}\right)$ and
${v}_{2} \in \partial \Phi \left( {u}_{2}\right)$ , we have
${v}_{1} \leq {v}_{2}$ . By definition of the subgradients at ${u}_{1}$
and ${u}_{2}$ , the following inequalities hold:

$$\Phi \left( {u}_{2}\right) - \Phi \left( {u}_{1}\right) \geq {v}_{1}\left( {{u}_{2} - {u}_{1}}\right) \;\Phi \left( {u}_{1}\right) - \Phi \left( {u}_{2}\right) \geq {v}_{2}\left( {{u}_{1} - {u}_{2}}\right) .$$

Summing up these inequalities yields
${v}_{2}\left( {{u}_{2} - {u}_{1}}\right) \geq {v}_{1}\left( {{u}_{2} - {u}_{1}}\right)$
and thus ${v}_{2} \geq {v}_{1}$ , since ${u}_{1} < {u}_{2}$ .

Now, if ${u}^{ * } > 0$ , then we have $- {u}^{ * } < {u}^{ * }$ . By
the property shown above, this implies ${v}_{1} \leq {v}_{2}$ . We
cannot have ${v}_{1} = {v}_{2} \neq 0$ since (4.11) would then imply
$\eta \left( x\right) = \frac{1}{2}$ . We also cannot have
${v}_{1} = {v}_{2} = 0$ since by the property shown above, we must have
${\Phi }^{\prime }\left( 0\right) \leq {v}_{2}$ and thus ${v}_{2} > 0$ .
Thus, we must have ${v}_{1} < {v}_{2}$ with ${v}_{2} > 0$ , which, by
(4.11), implies $\eta \left( x\right) > 1 - \eta \left( x\right)$ , that
is ${h}^{ * }\left( x\right) > 0$ .

Conversely, if ${h}^{ * }\left( x\right) > 0$ then
$\eta \left( x\right) > 1 - \eta \left( x\right)$ . We cannot have
${v}_{1} = {v}_{2} = 0$ or ${v}_{1} = {v}_{2} \neq 0$ as already shown.
Thus, since $\eta \left( x\right) \neq 1$ , by (4.11), this implies
${v}_{1} < {v}_{2}$ . We cannot have ${u}^{ * } < - {u}^{ * }$ since, by
the property shown above, this would imply ${v}_{2} \leq {v}_{1}$ .
Thus, we must have $- {u}^{ * } \leq {u}^{ * }$ , that is
${u}^{ * } \geq 0$ , and more specifically ${u}^{ * } > 0$ since, as
already shown above, ${u}^{ * } = 0$ implies
${h}^{ * }\left( x\right) = 0$ .

Theorem 4.7 Let $\Phi$ be a convex and non-decreasing function. Assume
that there exists $s \geq 1$ and $c > 0$ such that the following holds
for all $x \in X$ :

$${\left| {h}^{ * }\left( x\right) \right| }^{s} = {\left| \eta \left( x\right) - \frac{1}{2}\right| }^{s} \leq {c}^{s}\left\lbrack {{L}_{\Phi }\left( {x,0}\right) - {L}_{\Phi }\left( {x,{h}_{\Phi }^{ * }\left( x\right) }\right) }\right\rbrack .$$

Then, for any hypothesis $h$ , the excess error of $h$ is bounded as
follows:

$$R\left( h\right) - {R}^{ * } \leq {2c}{\left\lbrack {\mathcal{L}}_{\Phi }\left( h\right) - {\mathcal{L}}_{\Phi }^{ * }\right\rbrack }^{\frac{1}{s}}$$

Proof: We will use the following inequality which holds by the convexity
of $\Phi$ :

$$\Phi \left( {-2{h}^{ * }\left( x\right) h\left( x\right) }\right) = \Phi \left( {\left( {1 - {2\eta }\left( x\right) }\right) h\left( x\right) }\right)$$

$$= \Phi \left( {\eta \left( x\right) \left( {-h\left( x\right) }\right) + \left( {1 - \eta \left( x\right) }\right) h\left( x\right) }\right)$$

$$\leq \eta \left( x\right) \Phi \left( \left( {-h\left( x\right) }\right) \right) + \left( {1 - \eta \left( x\right) }\right) \Phi \left( {h\left( x\right) }\right) = {L}_{\Phi }\left( {x,h\left( x\right) }\right) . \tag{4.12}$$

By Lemma 4.5, Jensen's inequality, and
${h}^{ * }\left( x\right) = \eta \left( x\right) - \frac{1}{2}$ , we can
write

$$R\left( h\right) - R\left( {h}^{ * }\right)$$

$$= \underset{x \sim {\mathcal{D}}_{X}}{\mathbb{E}}\left\lbrack {\left| {{2\eta }\left( x\right) - 1}\right| {1}_{h\left( x\right) {h}^{ * }\left( x\right) \leq 0}}\right\rbrack$$

$$\leq \underset{x \sim {\mathcal{D}}_{X}}{\mathbb{E}}{\left\lbrack {\left| 2\eta \left( x\right) - 1\right| }^{s}{1}_{h\left( x\right) {h}^{ * }\left( x\right) \leq 0}\right\rbrack }^{\frac{1}{s}} \tag{Jensen's ineq.}$$

$$\leq {2c}\underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}{\left\lbrack \left\lbrack \Phi \left( 0\right) - {L}_{\Phi }\left( x,{h}_{\Phi }^{ * }\left( x\right) \right) \right\rbrack {1}_{h\left( x\right) {h}^{ * }\left( x\right) \leq 0}\right\rbrack }^{\frac{1}{s}} \tag{assumption}$$

$$\leq {2c}\underset{x \sim {\mathcal{D}}_{X}}{\mathbb{E}}{\left\lbrack \left\lbrack \Phi \left( -2{h}^{ * }\left( x\right) h\left( x\right) \right) - {L}_{\Phi }\left( x,{h}_{\Phi }^{ * }\left( x\right) \right) \right\rbrack {1}_{h\left( x\right) {h}^{ * }\left( x\right) \leq 0}\right\rbrack }^{\frac{1}{s}}\;\text{ (}\Phi \text{ non-decreasing) }$$

$$\leq {2c}\underset{x \sim {\mathcal{D}}_{X}}{\mathbb{E}}{\left\lbrack \left\lbrack {L}_{\Phi }\left( x,h\left( x\right) \right) - {L}_{\Phi }\left( x,{h}_{\Phi }^{ * }\left( x\right) \right) \right\rbrack {1}_{h\left( x\right) {h}^{ * }\left( x\right) \leq 0}\right\rbrack }^{\frac{1}{s}}\;\text{ (convexity ineq. (4.12)) }$$

$$\leq {2c}\underset{x \sim {\mathcal{D}}_{x}}{\mathbb{E}}{\left\lbrack {L}_{\Phi }\left( x,h\left( x\right) \right) - {L}_{\Phi }\left( x,{h}_{\Phi }^{ * }\left( x\right) \right) \right\rbrack }^{\frac{1}{s}},$$

which completes the proof, since
${\mathbb{E}}_{x \sim {\mathcal{D}}_{x}}\left\lbrack {{L}_{\Phi }\left( {x,{h}_{\Phi }^{ * }\left( x\right) }\right) }\right\rbrack = {L}_{\Phi }^{ * }$
.

The theorem shows that, when the assumption holds, the excess error of
$h$ can be upper bounded in terms of the excess $\Phi$ -loss. The
assumption of the theorem holds in particular for the following convex
loss functions:

-   Hinge loss, where
    $\Phi \left( u\right) = \max \left( {0,1 + u}\right)$ , with $s = 1$
    and $c = \frac{1}{2}$ .

<!-- -->

-   Exponential loss, where
    $\Phi \left( u\right) = \exp \left( u\right)$ , with $s = 2$ and
    $c = \frac{1}{\sqrt{2}}$ .

<!-- -->

-   Logistic loss, where
    $\Phi \left( u\right) = {\log }_{2}\left( {1 + {e}^{u}}\right)$ ,
    with $s = 2$ and $c = \frac{1}{\sqrt{2}}$ .

They also hold for the square loss and the squared Hinge loss (see
Exercises 4.2 and 4.3).

# 4.8 Chapter notes {#chapter-notes-1 .unnumbered}

The structural risk minimization (SRM) technique is due to Vapnik
\[1998\]. The original penalty term used by Vapnik \[1998\] is based on
the VC-dimension of the hypothesis set. The version of SRM with
Rademacher complexity-based penalties that we present here leads to
finer data-dependent learning guarantees. Penalties based on alternative
complexity measures can be used similarly leading to learning bounds in
terms of the corresponding complexity measure \[Bartlett et al.,
2002a\].

An alternative model selection theory of Voted Risk Minimization (VRM)
has been recently developed by Cortes, Mohri, and Syed \[2014\] and
other related publications \[Kuznetsov et al., 2014, DeSalvo et al.,
2015, Cortes et al., 2015\].

Theorem 4.7 is due to Zhang \[2003a\]. The proof given here is somewhat
different and simpler.

# 4.9 Exercises {#exercises-1 .unnumbered}

4.1 For any hypothesis set $\mathcal{H}$ , show that the following
inequalities hold:

$$\underset{S \sim {\mathcal{D}}^{m}}{\mathbb{E}}\left\lbrack {{\widehat{R}}_{S}\left( {h}_{S}^{\mathrm{{ERM}}}\right) }\right\rbrack \leq \mathop{\inf }\limits_{{h \in \mathcal{H}}}R\left( h\right) \leq \underset{S \sim {\mathcal{D}}^{m}}{\mathbb{E}}\left\lbrack {R\left( {h}_{S}^{\mathrm{{ERM}}}\right) }\right\rbrack . \tag{4.13}$$

4.2 Show that for the squared loss,
$\Phi \left( u\right) = {\left( 1 + u\right) }^{2}$ , the statement of
Theorem 4.7 holds with $s = 2$ and $c = \frac{1}{2}$ and therefore that
the excess error can be upper bounded as follows:

$$R\left( h\right) - {R}^{ * } \leq {\left\lbrack {\mathcal{L}}_{\Phi }\left( h\right) - {\mathcal{L}}_{\Phi }^{ * }\right\rbrack }^{\frac{1}{2}}.$$

4.3 Show that for the squared Hinge loss,
$\Phi \left( u\right) = \max {\left( 0,1 + u\right) }^{2}$ , the
statement of Theorem 4.7 holds with $s = 2$ and $c = \frac{1}{2}$ and
therefore that the excess error can be upper bounded as follows:

$$R\left( h\right) - {R}^{ * } \leq {\left\lbrack {\mathcal{L}}_{\Phi }\left( h\right) - {\mathcal{L}}_{\Phi }^{ * }\right\rbrack }^{\frac{1}{2}}.$$

4.4 In this problem, the loss of $h : X \rightarrow \mathbb{R}$ at point
$\left( {x,y}\right) \in X \times \{ - 1, + 1\}$ is defined to be
${1}_{{yh}\left( x\right) \leq 0}$ .

\(a\) Define the Bayes classifier and a Bayes scoring function
${h}^{ * }$ for this loss.

\(b\) Express the excess error of $h$ in terms of ${h}^{ * }$
(counterpart of Lemma 4.5, for loss considered here).

\(c\) Give a counterpart of the result of Theorem 4.7 for this loss.

4.5 Same questions as in Exercise 4.5 with the loss of
$h : X \rightarrow \mathbb{R}$ at point $\left( {x,y}\right) \in$
$X \times \{ - 1, + 1\}$ defined instead to be
${1}_{{yh}\left( x\right) < 0}$ .
