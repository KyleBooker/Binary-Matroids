# Binary-Matroids

This project looks at the problem of bounding the size (i.e. number of elements ) of a binary matroid as a function of its rank, given that one is excluding certain matroid minors.   

We aim to look at this problem in the context of binary matroids where which exclude certain small matroids as minors.  For example, it has been conjectured that for a (simple) binary matroid M, the maximum number of elements
of M is at most  9/2 r(M), where r(M) denote the rank of M.  In this project, we follow the methods of Kung et al by first looking at the cases where r(M) is small with the help of a computer, and then using this to set up
and inductive proof to establish good bounds.

There are several main methods included in this repository:

K5_minor: Counts the number of binary matroids without a K5 minor of a certain rank.

Circumference: Calculates the circumference of a binary matroid.

