# Bounding the Sizes of Binary Matroids with Respect to Rank

## Authors
Kyle Booker,
Rachael Lobay,
Cory Langille,
and Sean McGuinness

## Introduction

A good understanding of matroid theory is required to fully utilize these scripts.

This project looks at the problem of bounding the size (i.e. number of elements ) of a binary matroid as a function of its rank, given that one is excluding certain matroid minors.   

We aim to look at this problem in the context of binary matroids where we exclude certain small matroids as minors.  For example, it has been conjectured that for a (simple) binary matroid M, the maximum number of elements
of M is at most  9/2 r(M), where r(M) denotes the rank of M.  In this project, we follow the methods of Kung et al by first looking at the cases where r(M) is small with the help of a computer, and then using this to set up
an inductive proof to establish good bounds.

## Note

These methods have not been modularized nor are they fully functional on other computers without modification. These methods were not meant to be used outside of research purposes.

## Methods

The matroids are stored in a large dictionary of lists using keys of the form (r, k) where r = rank and k = n – r, where n = number of elements (columns) of the matroid. If you wanted access to all matroids of rank 4 and 9 elements, you would use “dictionary_name[(4, 5)]”.

### all_matroids(field, maxsize, maxrank):
Calculates the total number of matroids not containing a K5 minor of a particular rank, size and field. For binary matroids input a field size of "GF(2)"; K5 can be replaced with other minors. Saves the output to the file "test.sobj". Located in All_matroids.sobj.

### Circumference(matroids)
Calculates and prints the circumference (Defined to be the largest circuit in a matroid) over all matroids of a particular rank. Located in Circumference.sobj.

### triangle_number(matroids)
Calculates and prints the triangle numbers of all matroids to the console. Located in triangle_number.sobj.

## Instructions

Open and run the script of your choice in Sage. It is not reccomended to use the Sage Data Cloud, as the computations could take very long for certain matroids. To change input values, users will need to modify the source directly.

