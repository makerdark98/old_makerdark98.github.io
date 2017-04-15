---
layout: post
title: "Linear Algebra#2"
comments: true
description: "1st"
keywords: "math, linear_algebra"
tags : 
- linear_algebra
- math

---
## Matrix Transformations
### Another Way to View $$ A \vec x = b $$
- Matrix $$ A $$ is a way to produce a new vector $$ \vec b $$ from $$ \vec x $$ by multiplication.

### Definition
- A transformation $$ T $$ from $$ R^n $$ to $$ R^m $$ is a rul that assigns to each vector $$ \vec x $$ in $$ R^n $$ a vector $$ T(x) in R^m $$.
### Terminology

$$ R^n $$ : domatin of $$ T $$ , $$ R^m $$ : codomain of $$ T $$
- $$ T(x) $$ in $$ R^m $$ is the image of $$ x $$ under the transformation $$ T $$.
- Set of all images $$ T(x) $$ is the range of $$ T $$

# Linear Transformations
### Definition
- A transformation T is linear if :
  - $$ T(0) = 0 $$
  - $$ T(u + v)  = T(y) + T(v) $$ for all $$ u, $$ in the domain of $$T$$.
  - $$ T(cu) = cT(u) $$ for all $$ u $$ in the domain of $$ T $$ and all scalars $$ c $$.

## Identity Matrix
### Definition
- $$ I_n $$ is $$ m \times n $$ matrix with 1's on the main diagonal and 0's elsewhere. The $$ i^{th} $$ column of $$ I_n$$ is labeled $$ e_i $$.

## Linear Transformation
### Theorem
- Let $$ T : R^n -> R^m $$ be a linear transformation.
- Then there exists a unique matrix A such that
$$T(x) = Ax$$
- A is the $$ m \times n $$ matrix whoes $$ j^{th} $$ column is the vector $$ T(e_j) $$, where $$ e_j $$ is the $$ j^{th} $$ column of the identity matrix in $$ R^n $$
$$ A = [ T(e_1) $$ $$ T(e_2) $$ ... $$ T(e_n) $$ ]