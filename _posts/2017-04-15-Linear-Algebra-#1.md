---
layout: post
title: "Linear Algebra#1"
comments: true
description: "1st"
keywords: "math, linear_algebra"
tags : 
- linear_algebra
- math

---

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
  
## Span
### Definition 
- span { $$\vec v_1, ... , \vec v_2 $$ } is the set of all vectors that can be written as<br>
                             $$ c_1 \vec v_1 + c_2 \vec v_2 + ... + c_k \vec v_k $$
for some scalas $$ c_1, c_2, ... , c_k $$

## Existence of solutions
### Theorem
- The following statements are equivalent.
  - The matrix equation $$ A \vec v = \vec b $$ has a solution
  - The vector equation $$ x_1 \vec a_1 + ... x_n \vec a_n = \vec b $$ has a solution
  - $$ \vec b $$ is a linear comination of $$ \vec a_1 , \vec a_2 , ... , \vec a_n $$
  - $$ \vec b $$ is in Span{$$\vec a_1 , \vec a_2 , ... , \vec a_n $$}
  - The Linear System with augmented matrix \{ $$ a_1 , a_2 , ... , a_n $$ \| $$ \vec b_n $$ \} = { $$ A $$\| $$ \vec b$$ } has a solution

## Homogeneous System
### Definition
- A Linear System is homogeneous if it can be written in the form $$A \vec x = \vec b$$
- A homogeneous system always has the solution $$ \vec x = 0 $$, called the trivial solution
- A nontrivial solution is a solution $$ \vec x \ne \vec 0 $$

### Theorem
- THe homogeneous equation $$A \vec x = \vec 0 $$ has a nontrivial solution iff it has at least one free variable.

## Nonhomogeneous System
### Theorem
- If $$ A \vec x = \vec b $$, the solution set of nonhomogeneous sytem is the set of all vectors of the form<br>
$$\vec w = \vec p + \vec v_h $$
where $$\vec v_h$$ is any solution of the corresponding homogeneous system $$ A \vec x = \vec 0 $$

### Notation 
- In the above , $$ \vec p $$ is called a particular solution

## Vector Equation of a Line
### Procedure
- To find the vector equation of a line
  - Find a vector $$\vec v$$ parallel to the line
  - Find a point $$\vec p$$ on the line
  - The vector equation is then.
 $$\vec p + t \vec v, t \in R $$
 
## Linear Dependence
### Definition
- Consider a list of vectors $$ \vec v_1, ... , \vec v_n$$ in $$ R^n $$ and the equation
  $$x_1\vec v_1 + x_2\vec v_2 + ... + x_p\vec v_p = \vec 0 $$
  - If this equation has only the trivial solution, the list of vectors is linearly independent.
  - If this equation has a nontrivial solution, the list of vectors is linearly dependent.
- The list of vectors is linearly dependent if there exist some scalas $$ c_1, ... , c_p $$ not all zero, such that

$$c_1\vec v_1 + c_2\vec v_2 + ... + c_p\vec v_p = \vec 0 $$
- This is called a linear dependence relation.


## Solving problems about linear dependence/independence
- So if you're given a list of vectors
$$ \vec v_1, \vec v_2, ... , \vec v_p $$

and you want to know if they're linearly dependent or independent,
  - Form the matrix $$ A  = $$ [ $$ \vec v_1 $$ $$ \vec v_2 $$ ... $$\vec v_p $$ ] 
  - Row reduce [ $$ A $$ | $$ \vec 0 $$ ] 
    - If there are free variables, -> nontrivial sol. -> the vectors ar dependent
    - If there are no free variables, -> trivial sol. -> the vectors are independent.

### Linear independence of a two vector set
$$ x_1 \vec v_1 + x_2 \vec v_2 = \vec 0 $$
- Two vectors is linearly dependent iff at liseas one of the vectors is a multiple of the other.

## Characterization of linearly independent sets
### Theorem
- A list $$ \vec v_1, \vec v_2, ... \vec v_p $$ of two or more vectors is linearly dependent iff at least one of the vectors in the list is a linear combination of the others.

## Theorem : $$ p > n $$
- If $$ \vec v_1, \vec v_2, ... , \vec v_p $$ is a liest of vectors in $$ R^n $$, and $$ p > n $$ then the set is linearly dependent.

## Zero Vector
### Theorem
- If a list of vectors contains the zero vector, the vectors are linearly dependent.