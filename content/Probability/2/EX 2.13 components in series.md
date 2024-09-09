
Consider a system of five identical components connected in series, as illustrated in Figure 2.3.

![[01913607-292d-7d0a-a250-4b01870485a1_10_680627.jpg]]
Figure 2.3 A system of five components connected in a series

Denote 
- a component that fails by $F$
- one that doesn't fail by $S$ (for success).
---
Let $A$ be the event that the system fails.
For $A$ to occur, at least one of the individual components must fail.

Outcomes in $A$ include $SSFSS$ ( 1, 2, 4, and 5 all work,but 3 does not), $FFSSS$, and so on.
There are in fact 31 different outcomes in $A$.
However, $A\prime$, the event that the system works, consists of the single outcome $SSSSS$.
We will see in Section 2.5 that if $90\\%$ of all such components do not fail and different components fail independently of one another, then $P \left( A\prime \right) = P \left( SSSSS \right) = {.9}^{5} = .59$.
Thus $P\left( A \right) = 1 - .59 = .41$; so among a large number of such systems, roughly $41 \%$ will fail.

---