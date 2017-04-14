---
layout: post
title: "Linear Algebra#1"
comments: true
description: "1st"
keywords: "math, linear_algebra"


---

<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
## Linear Equation
### Definition
A linear equation is an equation that can be written in the form 
$$a_1 x_1 + a_2x_2+ ... + a_nx_n= b$$

- $$x_1, ... x_n$$ are called the variables.
- $$a_a, ... a_n$$ are called the coefficient.
- $$b$$ is the right hand side constant.
- $$n$$ can be any positive integer.

## Solution Set
- we have 3 differents types of solution sets
- A system of linear equations has either
  - No solution -> System is Inconsistent
  - Exactely on solution -> System is Consistent
  - Infinitely many solution -> System is Consistent
  
  
## Elementary Row Operations
- When solving linear system, we will use these Elementary Row Operations
  - Replacement : Replace one row by the swan of itself and a multiple of another row
  - Interchange : Interchange two rows.
  - Scale : Multiply all entries in a row by a nonzero constant

## Echelon form
- A matrix is in echelon form if it satisfies the following 3 conditions
  1. All nonzero rows are above all zero rows.
  2. The leading entry of nonzero rows is to the right of the leading entry of any row above it.
  3. All entries in a column below a leading entry are zeros.
 
## Reduced Row Echelon form
- A matrix is in reduced row echelon form if it satisfies the 3 echelon form conditions are 2 more conditions
  4. All leading entries are 1
  5. Each leading 1 is the only nonzero entry in its column

## Pivot Positions and Columns
### Definition
- A pivot position is a location that corresponds to a leading entry in an EF
- A pivot column is a column that contains a pivot position.

## Basic and Free Variables
- Base variable : The Variables corresponding to leading entries position in RREF
- Free variables : Other variables

## Row reduction algorithm

Step 1 : Begin with the leftmost nonzero column. The pivot position is at the top.<br>
Step 2 : If necessary, interchange rows to move a nonzero entry into the pivot position.<br>
Step 3 : Create zeros in all positions below the pivot.<br>
Step 4 : Apply step 1-3 to the remaining submatrix.<br>
Step 5 : Beginning with the rightmost pivot and working up/left, make each pivot and create zero above each pivot.<br>

## Linear Combination
### Definition
- The vector $$\vec u$$ <br>
  $$\vec u = c_1 \vec v_1+ c_2 \vec v_2 + ... + c_n \vec v_n $$ <br>
  is called a linear combination fo $$\vec v_1, \vec v_2, ... , \vec v_k $$ is coefficients $$c_1,c_2,...,c_k$$