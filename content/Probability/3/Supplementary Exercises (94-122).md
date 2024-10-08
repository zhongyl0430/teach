# 94
Consider a deck consisting of seven cards, marked 1, 2,\..., 7.
Three of these cards are selected at random. Define an rv $W$ by $W =$ the sum of the resulting numbers, and compute the pmf of $W$ . Then compute $\mu$ and ${\sigma }^{2}$ . 
Hint: Consider outcomes as unordered, so that $\left( {1,3,7}\right)$ and $(3$ , 1, 7) are not different outcomes. Then there are 35 outcomes, and they can be listed. (This type of rv actually arises in connection with a statistical procedure called Wilcoxon's rank-sum test, in which there is an $x$ sample and a $y$ sample and $W$ is the sum of the ranks of the $x$ 's in the combined sample; see Section 15.2.)
# 95
After shuffling a deck of 52 cards, a dealer deals out 5 . Let $X =$ the number of suits represented in the five-card hand.

a\. Show that the pmf of $X$ is

| $x$ | 1 | 2 | 3 | 4 |
| :--- | :---: | :---: | :---: | :---: |
| $p(x)$ | .002 | .146 | .588 | .264 |

Hint: $p\left( 1\right) = {4P}$ (all are spades), $p\left( 2\right) = {6P}$ (only spades and hearts with at least one of each suit), and $p\left( 4\right)$ $= {4P}$ (2 spades $\cap$ one of each other suit). 

b\. Compute $\mu ,{\sigma }^{2}$ , and $\sigma$ .
# 96
The negative binomial rv $X$ was defined as the number of $F$'s preceding the $r$ th $S$ . Let $Y =$ the number of trials necessary to obtain the $r$ th $S$ . In the same manner in which the pmf of $X$ was derived, derive the pmf of $Y$ .
# 97
Of all customers purchasing automatic garage-door openers, ${75}\%$ purchase a chain-driven model. Let $X =$ the number among the next 15 purchasers who select the chain-driven model.

a\. What is the pmf of $X$ ?

b\. Compute $P\left( {X > {10}}\right)$ .

c\. Compute $P\left( {6 \leq X \leq {10}}\right)$ .

d\. Compute $\mu$ and ${\sigma }^{2}$ .

e\. If the store currently has in stock 10 chain-driven models and 8 shaft-driven models, what is the probability that the requests of these 15 customers can all be met from existing stock?
# 98
In some applications the distribution of a discrete rv $X$ resembles the Poisson distribution except that zero is not a possible value of $X$ . For example, let $X =$ the number of tattoos that an individual wants removed when she or he arrives at a tattoo-removal facility. Suppose the pmf of $X$ is
$$p\left( x\right) = k\frac{{e}^{-\theta }{\theta }^{x}}{x}\;x = 1,2,3,\ldots$$

a\. Determine the value of $k$ . 
Hint: The sum of all probabilities in the Poisson pmf is 1 , and this pmf must also sum to 1 .

b\. If the mean value of $X$ is 2.313035, what is the probability that an individual wants at most 5 tattoos removed?

c\. Determine the standard deviation of $X$ when the mean value is as given in (b).

Note: The article \"An Exploratory Investigation of Identity Negotiation and Tattoo Removal\" (Academy of Marketing Science Review, vol. 12, no. 6, 2008) gave a sample of 22 observations on the number of tattoos people wanted removed; estimates of $\mu$ and $\sigma$ calculated from the data were 2.318182 and 1.249242, respectively.
# 99
A k-out-of-n system is one that will function if and only if at least $k$ of the $n$ individual components in the system function. If individual components function  independently of one another, each with probability .9 , what is the probability that a 3-out-of-5 system functions?
# 100
A manufacturer of integrated circuit chips wishes to control the quality of its product by rejecting any batch in which the proportion of defective chips is too high. To this end, out of each batch (10,000 chips), 25 will be selected and tested. If at least 5 of these 25 are defective, the entire batch will be rejected.

a\. What is the probability that a batch will be rejected if $5\%$ of the chips in the batch are in fact defective?

b\. Answer the question posed in (a) if the percentage of defective chips in the batch is ${10}\%$ .

c\. Answer the question posed in (a) if the percentage of defective chips in the batch is ${20}\%$ .

d\. What happens to the probabilities in (a)-(c) if the critical rejection number is increased from 5 to 6 ?
# 101
Of the people passing through an airport metal detector, ${.5}\%$ activate it; let $X =$ the number among a randomly selected group of 500 who activate the detector.

a\. What is the (approximate) pmf of $X$ ?

b\. Compute $P\left( {X = 5}\right)$ .

c\. Compute $P\left( {5 \leq X}\right)$ .
# 102
An educational consulting firm is trying to decide whether high school students who have never before used a hand-held calculator can solve a certain type of problem more easily with a calculator that uses reverse Polish logic or one that does not use this logic. A sample of 25 students is selected and allowed to practice on both calculators. Then each student is asked to work one problem on the reverse Polish
calculator and a similar problem on the other. Let $p = P\left( S\right)$ , where $S$ indicates that a student worked the problem more quickly using reverse Polish logic than without, and let $X =$ number of $S$ 's.

a\. If $p = {.5}$ , what is $P\left( {7 \leq X \leq {18}}\right)$ ?

b\. If $p = {.8}$ , what is $P\left( {7 \leq X \leq {18}}\right)$ ?

c\. If the claim that $p = {.5}$ is to be rejected when either $x \leq 7$ or $x \geq {18}$ , what is the probability of rejecting the claim when it is actually correct?

d\. If the decision to reject the claim $p = {.5}$ is made as in part (c), what is the probability that the claim is not rejected when $p = {.6}$ ? When $p = {.8}$ ?

e\. What decision rule would you choose for rejecting the claim $p = {.5}$ if you wanted the probability in part (c) to be at most .01 ?
# 103
Consider a disease whose presence can be identified by carrying out a blood test. Let $p$ denote the probability that a randomly selected individual has the disease. Suppose $n$ individuals are independently selected for testing. One way to proceed is to carry out a separate test on each of the $n$ blood samples. A potentially more economical approach, group testing, was introduced during World War II to identify syphilitic men among army inductees. First, take a part of each blood sample, combine these specimens, and carry out a single test. If no one has the disease, the result will be negative, and only the one test is required. If at least one individual is diseased, the test on the combined sample will yield a positive result, in which case the $n$ individual tests are then carried out. If $p = {.1}$ and $n = 3$ , what is the expected number of tests using this procedure? What is the expected number when $n = 5$ ? 
The article \"Random Multiple-Access Communication and Group Testing\" (IEEE Trans. on Commun., 1984: 769-774) applied these ideas to a communication system in which the dichotomy was active/ idle user rather than diseased/nondiseased.
# 104
Let ${p}_{1}$ denote the probability that any particular code symbol is erroneously transmitted through a communication system. Assume that on different symbols, errors occur independently of one another.
Suppose also that with probability ${p}_{2}$ an erroneous symbol is corrected upon receipt. Let $X$ denote the number of correct symbols in a message block consisting of $n$ symbols (after the correction process has ended). What is the probability distribution of $X$ ?
# 105
The purchaser of a power-generating unit requires $c$ consecutive successful start-ups before the unit will be accepted. Assume that the outcomes of individual startups are independent of one another. Let $p$ denote the probability that any particular start-up is successful. The random variable of interest is $X =$ the number of startups that must be made prior to acceptance. Give the pmf of $X$ for the case $c = 2$ . If $p = {.9}$ , what is $P\left( {X \leq 8}\right)$ ? 
Hint: For $x \geq 5$ , express $p\left( x\right)$ \"recursively\" in terms of the pmfevaluated at the smaller values $x - 3,x - 4,\ldots ,2$ .
(This problem was suggested by the article \"Evaluation of a Start-Up Demonstration Test,\" J. Quality Technology, 1983: 103-106.)
# 106
A plan for an executive travelers' club has been developed by an airline on the premise that ${10}\%$ of its current customers would qualify for membership.

a\. Assuming the validity of this premise, among 25 randomly selected current customers, what is the probability that between 2 and 6 (inclusive) qualify for membership?

b\. Again assuming the validity of the premise, what are the expected number of customers who qualify and the standard deviation of the number who qualify in a random sample of 100 current customers?

c\. Let $X$ denote the number in a random sample of 25 current customers who qualify for membership. Consider rejecting the company's premise in favor of the claim that $p > {.10}$ if $x \geq 7$ . What is the probability that the company's premise is rejected when it is actually valid?

d\. Refer to the decision rule introduced in part (c). What is the probability that the company's premise is not rejected even though $p = {.20}$ (i.e., ${20}\%$ qualify)?
# 107
Forty percent of seeds from maize (modern-day corn) ears carry single spikelets, and the other ${60}\%$ carry paired spikelets. A seed with single spikelets will produce an ear with single spikelets ${29}\%$ of the time, whereas a seed with paired spikelets will produce an ear with single spikelets ${26}\%$ of the time. Consider randomly selecting ten seeds.

a\. What is the probability that exactly five of these seeds carry a single spikelet and produce an ear with a single spikelet?

b\. What is the probability that exactly five of the ears produced by these seeds have single spikelets? What is the probability that at most five ears have single spikelets?
# 108
A trial has just resulted in a hung jury because eight members of the jury were in favor of a guilty verdict and the other four were for acquittal. If the jurors leave the jury room in random order and each of the first four leaving the room is accosted by a reporter in quest of an interview, what is the pmf of $X =$ the number of jurors favoring acquittal among those interviewed? 
How many of those favoring acquittal do you expect to be interviewed?
# 109
A reservation service employs five information operators who receive requests for information independently of one another, each according to a Poisson process with rate $\alpha = 2$ per minute.

a\. What is the probability that during a given 1-min period, the first operator receives no requests?

b\. What is the probability that during a given 1-min period, exactly four of the five operators receive no requests?

c\. Write an expression for the probability that during a given 1-min period, all of the operators receive exactly the same number of requests.
# 110
Grasshoppers are distributed at random in a large field according to a Poisson process with parameter $\alpha = 2$ per square yard. How large should the radius $R$ of a circular sampling region be taken so that the probability of finding at least one in the region equals .99 ?
# 111
A newsstand has ordered five copies of a certain issue of a photography magazine. Let $X =$ the number of individuals who come in to purchase this magazine. If $X$ has a Poisson distribution with parameter $\mu = 4$ , what is the expected number of copies that are sold?
# 112
Individuals A and B begin to play a sequence of chess games. Let $S = \{ \mathrm{\;A}$ wins a game $\}$ , and suppose that outcomes of successive games are independent with $P\left( S\right) =$ $p$ and $P\left( F\right) = 1 - p$ (they never draw). They will play until one of them wins ten games. Let $X =$ the number of games played (with possible values ${10},{11},\ldots ,{19}$ ).

a\. For $x = {10},{11},\ldots ,{19}$ , obtain an expression for $p\left( x\right) = P\left( {X = x}\right) .$

b\. If a draw is possible, with $p = P\left( S\right) ,q = P\left( F\right)$ , $1 - p - q = P$ (draw), what are the possible values of $X$ ? What is $P\left( {{20} \leq X}\right)$ ? 
Hint: $P\left( {{20} \leq X}\right) =$ $1 - P\left( {X < {20}}\right)$ .
# 113
A test for the presence of a certain disease has probability .20 of giving a false-positive reading (indicating that an individual has the disease when this is not the case) and probability . 10 of giving a false-negative result. Suppose that ten individuals are tested, five of whom have the disease and five of whom do not. Let $X =$ the number of positive readings that result.

a\. Does $X$ have a binomial distribution? Explain your reasoning.

b\. What is the probability that exactly three of the ten test results are positive?
# 114
The generalized negative binomial pmf is given by
$${nb}\left( {x;r,p}\right) = k\left( {r,x}\right) \cdot {p}^{r}{\left( 1 - p\right) }^{x}$$
for $x = 0,1,2,\ldots$

Let $X$ , the number of plants of a certain species found in a particular region, have this distribution with $p = {.3}$ and $r = {2.5}$ . What is $P\left( {X = 4}\right)$ ? What is the probability that at least one plant is found?
# 115
There are two Certified Public Accountants in a particular office who prepare tax returns for clients. Suppose that for a particular type of complex form, the number of errors made by the first preparer has a Poisson distribution with mean value ${\mu }_{1}$ , the number of errors made by the second preparer has a Poisson distribution with mean value ${\mu }_{2}$ , and that each CPA prepares the same number of forms of this type. Then if a form of this type is randomly selected, the function
$$p\left( {x;{\mu }_{1},{\mu }_{2}}\right) = {.5}\frac{{e}^{-{\mu }_{1}}{\mu }_{1}^{x}}{x!} + {.5}\frac{{e}^{-{\mu }_{2}}{\mu }_{2}^{x}}{x!}\;x = 0,1,2,\ldots$$
gives the pmf of $X =$ the number of errors on the selected form.

a\. Verify that $p\left( {x;{\mu }_{1},{\mu }_{2}}\right)$ is in fact a legitimate pmf $\left( { \geq 0\text{and sums to 1}}\right)$ .

b\. What is the expected number of errors on the selected form?

c\. What is the variance of the number of errors on the selected form?

d\. How does the pmf change if the first CPA prepares ${60}\%$ of all such forms and the second prepares ${40}\%$ ?
# 116
The mode of a discrete random variable $X$ with $\operatorname{pmf}p\left( x\right)$ is that value ${x}^{ * }$ for which $p\left( x\right)$ is largest (the most probable $x$ value).

a\. Let $X \sim \operatorname{Bin}\left( {n,p}\right)$ . By considering the ratio $b\left( {x + 1;n,p}\right) /b\left( {x;n,p}\right)$ , show that $b\left( {x;n,p}\right)$ increases with $x$ as long as $x < {np} - \left( {1 - p}\right)$ . Conclude that the mode ${x}^{ * }$ is the integer satisfying $\left( {n + 1}\right) p - 1 \leq {x}^{ * } \leq \left( {n + 1}\right) p.$

b\. Show that if $X$ has a Poisson distribution with parameter $\mu$ , the mode is the largest integer less than $\mu$ . If $\mu$ is an integer, show that both $\mu - 1$ and $\mu$ are modes.
# 117
A computer disk storage device has ten concentric tracks, numbered $1,2,\ldots ,{10}$ from outermost to innermost, and a single access arm.
Let ${p}_{i} =$ the probability that any particular request for data will take the arm to track $i\left( {i = 1,\ldots ,{10}}\right)$ .
Assume that the tracks accessed in successive seeks are independent. Let $X =$ the number of tracks over which the access arm passes during two successive requests (excluding the track that the arm has just left, so possible $X$ values are $x = 0,1,\ldots ,9)$ . Compute the pmf of $X$ . 
Hint: $P$ (the arm is now on track $i$ and $X = j$ ) = $P\left( {X = j \mid \operatorname{arm}\text{ nowon }i}\right) \cdot {p}_{i}$. After the conditional probability is written in terms of ${p}_{1},\ldots ,{p}_{10}$ , by the law of total probability, the desired probability is obtained by summing over $i$ .
# 118
If $X$ is a hypergeometric rv, show directly from the definition that $E\left( X\right) = {nM}/N$ (consider only the case $n < M$ ).
Hint: Factor ${nM}/N$ out of the sum for $E\left( X\right)$ , and show that the terms inside the sum are of the form $h\left( {y;n - 1,M - 1,N - 1}\right)$ , where $y = x - 1$ .
# 119
Use the fact that
$$\mathop{\sum }\limits_{{\text{all }x}}{\left( x - \mu \right) }^{2}p\left( x\right) \geq \mathop{\sum }\limits_{{x : \left| {x - \mu }\right| \geq {k\sigma }}}{\left( x - \mu \right) }^{2}p\left( x\right)$$
to prove Chebyshev's inequality given in Exercise 44.
# 120
The simple Poisson process of Section 3.6 is characterized by a constant rate $\alpha$ at which events occur per unit time. A generalization of this is to suppose that the probability of exactly one event occurring in the interval
$\left\lbrack {t,t + {\Delta t}}\right\rbrack$ is $\alpha \left( t\right) \cdot {\Delta t} + o\left( {\Delta t}\right)$ .
It can then be shown that the number of events occurring during an interval $\left\lbrack {{t}_{1},{t}_{2}}\right\rbrack$ has a Poisson distribution with parameter
$$\mu = {\int }_{{t}_{2}}^{{t}_{1}}\alpha \left( t\right) {dt}$$

The occurrence of events over time in this situation is called a nonhomogeneous Poisson process. The article \"Inference Based on Retrospective Ascertainment,\" (J. Amer. Stat. Assoc., 1989: 360-372), considers the intensity function
$$\alpha \left( t\right) = {e}^{a + {bt}}$$
as appropriate for events involving transmission of HIV (the AIDS virus) via blood transfusions. Suppose that $a = 2$ and $b = {.6}$ (close to values suggested in the paper), with time in years.

a\. What is the expected number of events in the interval $\left\lbrack {0,4}\right\rbrack$ ? In $\left\lbrack {2,6}\right\rbrack$ ?

b\. What is the probability that at most 15 events occur in the interval $\left\lbrack {0,{.9907}}\right\rbrack$ ?
# 121
Consider a collection ${A}_{1},\ldots ,{A}_{k}$ of mutually exclusive and exhaustive events, and a random variable $X$ whose distribution depends on which of the ${A}_{i}$ 's occurs (e.g., a commuter might select one of three possible routes from home to work, with $X$ representing the commute time). Let $E\left( {X \mid {A}_{i}}\right)$ denote the expected value of $X$ given that the event ${A}_{i}$ occurs. Then it can be shown that $E\left( X\right) = {\sum E}\left( {X \mid {A}_{i}}\right) \cdot P\left( {A}_{i}\right)$, the weighted average of the individual \"conditional expectations\" where the weights are the probabilities of the partitioning events.

a\. The expected duration of a voice call to a particular telephone number is 3 minutes, whereas the expected duration of a data call to that same number is 1 minute. If ${75}\%$ of all calls are voice calls, what is the expected duration of the next call?

b\. A deli sells three different types of chocolate chip cookies. The number of chocolate chips in a type $i$ cookie has a Poisson distribution with parameter ${\mu }_{i} = i + 1\;\left( {i = 1,2,3}\right)$ . If ${20}\%$ of all customers purchasing a chocolate chip cookie select the first type, ${50}\%$ choose the second type, and the remaining ${30}\%$ opt for the third type, what is the expected number of chips in a cookie purchased by the next customer?
# 122
Consider a communication source that transmits packets containing digitized speech. After each transmission, the receiver sends a message indicating whether the transmission was successful or unsuccessful. If a transmission is unsuccessful, the packet is re-sent. Suppose a voice packet can be transmitted a maximum of 10 times. Assuming that the results of successive transmissions are independent of one another and that the probability of any particular transmission being successful is $p$ , determine the probability mass function of the rv $X =$ the number of times a packet is transmitted. Then obtain an expression for the expected number of times a packet is transmitted.