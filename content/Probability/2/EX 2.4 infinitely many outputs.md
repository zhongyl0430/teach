A reasonably large percentage of C++ programs written at a particular company compile on the first run, but some do not (a compiler is a program that translates source code, in this case C++ programs, into machine language so programs can be executed).

Suppose an experiment consists of selecting and compiling C++ programs at this location one by one until encountering a program that compiles on the first run.

---
Denote

-   a program that compiles on the first run by $S$ (for success)
-   one that doesn't do so by $F$ (for failure).

Although it may not be very likely, a possible outcome of this experiment is that the first 5 (or 10 or 20 or ...) are $F$'s and the next one is an $S$ .
That is, for any positive integer $n$ , we may have to examine $n$ programs before seeing the first $S$ .

---
The sample space is $\mathcal{S} = \{ S,{FS},{FFS},{FFFS},\ldots \}$ , which contains an infinite number of possible outcomes.

The same abbreviated form of the sample space is appropriate for an experiment in which, starting at a specified time, the gender of each newborn infant is recorded until the birth of a male is observed.
