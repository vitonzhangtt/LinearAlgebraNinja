# Concepts

## Column space

## Nullspace
$`A`$ is a matrix with $`m \times n`$, as $`A_{m,n}`$.
The nullspace $`N(A)`$ consists of all solutions to $`A\mathbf{x}=0`$. These vectors $`\mathbf{x}`$ are in $`R^n`$. 

### Reference
Ref[1]: Section 3.2 

## Minor of matrix (for a specific element)
**Minor** of matrix for a particular element in the matrix is defined as <br>
the matrix obtained after deleting the row and column of the matrix  <br>
in which that particular element lies.

Here the minor of the element $`a_{ij}`$ is denoted as $`M_{ij}`$. <br>
For example, the minor for the $`a_{12}`$ entry is $`M_{12}`$ in $`A`$ matrix. <br>

$`
A =  \begin{pmatrix}
      a_{11} & a_{12} & a_{13}\\
      a_{21} & a_{22} & a_{23}\\
      a_{31} & a_{32} & a_{33}\\
      \end{pmatrix} 
`$

$`
M_{12} =  \begin{pmatrix}
            a_{21} & a_{23}\\
            a_{31} & a_{33}\\
      \end{pmatrix} 
`$


## Minor matrix

### Reference
[Minor of matrix](https://www.cuemath.com/algebra/minor-of-matrix/)

## Transpose
The **transpose** of matrix $`A`$ is $`A^T`$ . The columns of $`A^T`$ are the rows of $`A`$. <br>

For example, $`A`$ and $`A^T`$ are as the following:

$`
A = \begin{pmatrix}
      1 & 2 & 3 \\
      4 & 5 & 6 \\
    \end{pmatrix} 
`$

$`
A^T = \begin{pmatrix}
      1 & 4 \\
      2 & 5 \\
      3 & 6 \\
      \end{pmatrix} 
`$

### Reference
Ref[1]: Section 2.7 


## Properties
For $`A_{m, n}`$ and $`B_{m, n}`$ matrix, there are the following properties of transpose. <br>

1. $`(A^T)^T=A`$ <br>
2. $`(A+B)^T=A^T+B^T`$ <br>
3. $`(AB)^T=B^TA^T`$  (Here $`A_{m,n}, B_{n,m}`$) <br> 
4. $`(A^{-1})^T=(A^T)^{-1} \implies (A^{-1}A)^T=A^T(A^{-1})^T=I^T=I=A^T(A^T)^{-1}`$ ($`A`$ is square matrix)  <br>
5. $`(A^n)^T = (A^T)^n`$

### Proof: $`(A^n)^T = (A^T)^n`$
For property 3, when $`A=B`$ we have the following: <br>
$`(A^2)^T=A^TA^T=(A^T)^2`$ <br>
$`(A^3)^T=A^TA^TA^T=(A^T)^3 \implies (A^n)^T=(A^T)^n `$


## Cofactor Matrix


### Reference
[Cofactor Matrix](https://www.cuemath.com/algebra/cofactor-matrix/)

## Square Matrix
A **square matrix** is a matrix with an equal number of rows and columns.

### Reference
[Square Matrix](https://www.cuemath.com/algebra/square-matrix/)

## Symmetric matrix
A symmetric matrix is a square matrix that is equal to its transpose matrix. $`A=A^T`$

### Properties


### Reference
[Symmetric Matrix](https://www.cuemath.com/algebra/symmetric-matrix/)

## Singular Matrix
A **singular matrix** is a square matrix if its **determinant** is 0.

### Reference
[Singular Matrix](https://www.cuemath.com/algebra/singular-matrix/)


## Skew-symmetric matrix
In mathematics, a skew symmetric matrix is defined as the square matrix that is equal 
to the negative of its transpose matrix. <br>
For any square matrix, $`A`$, the transpose matrix is given as $`A^T`$. <br>
A **skew-symmetric** or **antisymmetric** matrix $`A`$ can therefore be represented 
as, $`A = -A^T`$. For example,

$`A= \begin{pmatrix}
      0 & 4 & 3 \\
      -4 & 0 & -6 \\
      -3 & 6 & 0 \\
      \end{pmatrix} `$

### Reference
[Skew Symmetric Matrix](https://www.cuemath.com/algebra/skew-symmetric-matrix/)


## Matrix exponential



### Reference



