
> [!definition] probability
> Given an experiment and a sample space $\mathcal{S}$, the objective of probability is to assign to each event $A$ a number $P\left( A\right)$, called **the probability of the event $A$**, which will give a precise measure of the chance that $A$ will occur:

To ensure that the probability assignments will be consistent with our intuitive notions of probability, all assignments should satisfy the following axioms (basic properties) of probability.

## axioms of probability

> [!definition] (axioms of probability)
> 1.  For any event $A,P\left( A \right) \geq 0$.
> 2.  $P\left( \mathcal{S}\right) = 1$.
> 3.  If ${A}_{1},{A}_{2},{A}_{3},\ldots$ is an infinite collection of disjoint events, then
> $$P\left( {{A}_{1} \cup {A}_{2} \cup {A}_{3} \cup \cdots }\right) = \sum_{i = 1}^{\infty} P\left( {A}_{i}\right) .$$

### remark on 3rd axiom

You might wonder why the third axiom contains no reference to a finite collection of disjoint events. It is because the corresponding property for a finite collection can be derived from our three axioms. We want the axiom list to be as short as possible and not contain any property that can be derived from others on the list. 

> [!remark]
> 1. Axiom 1 reflects the intuitive notion that the chance of $A$ occurring should be nonnegative. 
> 2. The sample space is by definition the event that must occur when the experiment is performed $(\mathcal{S}$ contains all possible outcomes), so Axiom 2 says that the maximum possible probability of 1 is assigned to $\mathcal{S}$ . 
> 3. The third axiom formalizes the idea that if we wish the probability that at least one of a number of events will occur and no two of the events can occur simultaneously, then the chance of at least one occurring is the sum of the chances of the individual events.