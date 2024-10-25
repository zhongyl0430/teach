- Our first counting rule applies to any situation in which 
	- a set (event) consists of ordered pairs of objects and 
	- we wish to count the number of such pairs. 

> [!definition] ordered pair
> By an **ordered pair**, we mean that, 
> - if $O_{1}$ and $O_{2}$ are objects, 
> - then the pair $\left( O_{1}, O_{2} \right)$ is different from the pair $\left( O_{2}, O_{1} \right)$. 

> [!example]
> If an individual selects one airline for a trip 
> 1. from Los Angeles to Chicago and 
> 2. (after transacting business in Chicago) a second one for continuing on to New York, 
> 
> Possible selections: 
> - one possibility is (American, United), 
> - another is (United, American), and 
> - still another is (United, United).

> [!proposition] total number of ordered pairs
> If 
> - the first element or object of an ordered pair can be selected in ${n}_{1}$ ways, 
> - and for each of these ${n}_{1}$ ways the second element of the pair can be selected in ${n}_{2}$ ways, 
> 
> then the number of pairs is 
> $${n}_{1}{n}_{2} .$$

An alternative interpretation involves carrying out an operation that consists of *two stages*. 
If 
- the first stage can be performed in any one of ${n}_{1}$ ways, 
- and for each such way there are ${n}_{2}$ ways to perform the second stage, 
then ${n}_{1}{n}_{2}$ is the number of ways of carrying out the two stages in sequence.

> [!example] Example 2.17
> - A homeowner doing some remodeling requires the services of 
> 	- both a plumbing contractor 
> 	- and an electrical contractor. 
> - If there are 
> 	- 12 plumbing contractors and 
> 	- 9 electrical contractors available in the area, 
> - in how many ways can the contractors be chosen? 
> 
> - If we denote 
> 	- the plumbers by ${P}_{1},\ldots ,{P}_{12}$ and 
> 	- the electricians by ${Q}_{1},\ldots ,{Q}_{9}$ , 
> - then we wish the number of pairs of the form 
>   $$\left( {{P}_{i},{Q}_{i}}\right)$$
> - With ${n}_{1} = {12}$ and ${n}_{2} = 9$, the product rule yields 
>   $$N = \left( {12}\right) \left( 9\right) = {108}$$
>    possible ways of choosing the two types of contractors.

^ex-2-17

- In Example 2.17, the choice of the second element of the pair did not depend on which first element was chosen or occurred. 
- As long as 
	- there is the same number of choices of the second element for each first element, 
- the product rule is valid 
	- even when the set of possible second elements depends on the first element.

> [!example] Example 2.18
> - A family 
> 	- has just moved to a new city and 
> 	- requires the services of 
> 		- both an obstetrician 
> 		- and a pediatrician. 
> - There are two easily accessible medical clinics, each having 
> 	- two obstetricians and 
> 	- three pediatricians.
> - The family will obtain maximum health insurance benefits 
> 	- by joining a clinic and selecting both doctors from that clinic. 
> - In how many ways can this be done? 
> 
> Denote
> -   the obstetricians by ${O}_{1}$, ${O}_{2}$, ${O}_{3}$, and ${O}_{4}$
> -   the pediatricians by ${P}_{1},\ldots ,{P}_{6}$.
> 
> - Then we wish the number of pairs $\left( {{O}_{i},{P}_{j}}\right)$ 
> 	- for which ${O}_{i}$ and ${P}_{j}$ are associated with the same clinic.
> - Because 
> 	- there are four obstetricians, ${n}_{1} = 4$ , 
> 	- and for each there are three choices of pediatrician, so ${n}_{2} = 3$ . 
> - Applying the product rule gives 
>   $$N = {n}_{1}{n}_{2} = {12}$$
>    possible choices.

^ex-2-18

## tree diagram

- In many counting and probability problems, 
	- a configuration called a **tree diagram** can be used to represent pictorially all the possibilities. 
- The tree diagram associated with Example 2.18 appears in Figure 2.7. 

Figure 2.7 Tree diagram for Example 2.18
![](images/01913607-292d-7d0a-a250-4b01870485a1_17_162463.jpg)

- Starting from a point on the left side of the diagram, 
	- for each possible first element of a pair a straight-line segment emanates rightward. 
	- Each of these lines is referred to as a first-generation branch. 
- Now for any given first-generation branch 
	- we construct another line segment emanating from the tip of the branch for each possible choice of a second element of the pair. 
	- Each such line segment is a second-generation branch. 
- Because there are four obstetricians, there are four first-generation branches, 
- and three pediatricians for each obstetrician yields three second-generation branches emanating from each first-generation branch.

- Generalizing, suppose 
	- there are ${n}_{1}$ first-generation branches, 
	- and for each first-generation branch there are ${n}_{2}$ second-generation branches. 
- The total number of second-generation branches is then 
  $${n}_{1}{n}_{2}$$
- Since the end of each second-generation branch corresponds to exactly one possible pair 
	- choosing a first element and then a second puts us at the end of exactly one second-generation branch, 
- there are ${n}_{1}{n}_{2}$ pairs, verifying the product rule.

- The construction of a tree diagram does not depend on 
	- having the same number of second-generation branches emanating from each first-generation branch. 

> [!example]
> - If the second clinic had four pediatricians,
> - then there would be 
> 	- only three branches emanating from two of the first-generation branches 
> 	- and four emanating from each of the other two first-generation branches. 
> - A tree diagram can thus be used to represent pictorially experiments 
> 	- other than those to which the product rule applies.