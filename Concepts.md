# Concepts

## Order
TODO:

## Rank

### What's rank of a matrix?

The rank of a matrix is equal to the number of linearly independent rows (or columns) in it. <sup>[1]</sup> <br>
The rank of a matrix is the **order** of the highest ordered non-zero **minor**. <sup>[1]</sup>

In fact the rows and columns always agree on the rank (amazing but true!). <sup>[2]</sup>

The rank is how many of the rows are "unique": not made of other rows. (Same for columns.) <sup>[2]</sup>

### How to Find the Rank of a Matrix?


### Reference
1. [Rank of a Matrix](https://www.cuemath.com/algebra/rank-of-a-matrix/) [To Read]
2. [Matrix Rank](https://www.mathsisfun.com/algebra/matrix-rank.html)
3. [Rank of a matrix](https://byjus.com/jee/rank-of-a-matrix-and-special-matrices/)

## Determinant

### Definition
The determinant of an $`n × n`$ matrix $`A`$, denoted $`det(A)`$ or $`|A|`$, is a number given by the following: <br>
1. if $`A`$ is a 1×1 matrix $`A=[a]`$, then $`det(A)=a`$.
2. if $`A`$ is a 2×2 matrix <br>
$`
A =  \begin{pmatrix}
      a & b \\
      c & d \\
      \end{pmatrix} 
`$
then $`det(A) = ad − bc`$.
3. if $`A`$ is an n×n matrix, where $`n ≥ 2`$, then det(A) is the number found by taking <br>
the [cofactor expansion](#co-factor-expansion-ref3) along the first row of A. That is, <br>
$`det(A) = a_{1,1}C_{1,1} + a_{1,2}C_{1,2} + · · · + a_{1,n}C_{1,n}`$.

### Reference
1. [Section 3.3 'The Determinant' in Ref[3]](https://github.com/vitonzhangtt/LinearAlgebraNinja/edit/main/Reference.md#reference-list)


## Inverse

### Reference

## Moore–Penrose inverse

### Reference
1. [Moore–Penrose inverse](https://en.wikipedia.org/wiki/Moore%E2%80%93Penrose_inverse)

## Column space

## Nullspace
$`A`$ is a matrix with $`m \times n`$, as $`A_{m,n}`$.
The nullspace $`N(A)`$ consists of all solutions to $`A\mathbf{x}=0`$. These vectors $`\mathbf{x}`$ are in $`R^n`$. 

### Reference
Ref[1]: Section 3.2 

## Cross Product
The cross product $`× : R^3 × R^3 → R^3`$ is an operation that takes two vectors $`u`$ and $`v`$ <br>
in space and determines another vector $`u×v`$ in space. (Cross products  <br>
are sometimes called **outer products**, sometimes called **vector products**.) 

The definition<sup>Ref[2]</sup> of $`{\text{\color{red}{Cross Product}}}`$ of two vectors $`\vec{A}`$ and $`\vec{B}`$ is:  <br>
$`\vec{A} \times \vec{B} = |\vec{A}||\vec{B}|\sin{(\theta)}\hat{n}`$ <br>

| Symbols | Meaning |
| --- | --- |
| $`\theta`$ | the angle which is formed between $`\vec{A}`$ and $`\vec{B}`$. |
| $`\hat{n}`$ | the **unit vector** perpendicular to the plane containing both $`\vec{A}`$ and $`\vec{B}`$. |


### Reference
1. [Cross products](http://aleph0.clarku.edu/~ma130/crossproducts.pdf)
2. [Cross Product of Two Vectors](https://www.cuemath.com/geometry/cross-product/)
3. [wiki: Cross_product (AAAA+)](https://en.wikipedia.org/wiki/Cross_product)

## Dot Product

### Reference 
[Dot Product](https://www.cuemath.com/algebra/dot-product/)

## Triple Cross Product (Vector Triple Product)
$`A \times {(B \times C)}`$

### Reference

## Minor of a specific element
The **minor** of an element in a matrix is defined as the **determinant** <br>
obtained by deleting the row and column in which that element lies. <sup>[2]</sup>

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
M_{12} =  \begin{vmatrix}
            a_{21} & a_{23}\\
            a_{31} & a_{33}\\
      \end{vmatrix} 
`$

Minor of matrix for a particular element in the matrix is defined as **the matrix** <br>
obtained after deleting the row and column of the matrix in which that particular element lies. <sup>[1]</sup>

1.2 Definition: For any $`n×n`$ matrix $`T`$, the $`(n − 1)×(n − 1)`$ matrix formed by <br>
deleting row $`i`$ and column $`j`$ of $`T`$ is the **i,j minor of T**. <sup>[3]</sup>

## Minor of matrix
We can take the minors of the matrix and form a **minor matrix M** of the given matrix A as: <br>
$`
M =  \begin{pmatrix}
      M_{11} & M_{12} & M_{13}\\
      M_{21} & M_{22} & M_{23}\\
      M_{31} & M_{32} & M_{33}\\
      \end{pmatrix} 
`$

$`M_{ij}`$ is the minor of $`a_{ij}`$ element in matrix A. 

### Reference
1. ~~[Minor of matrix](https://www.cuemath.com/algebra/minor-of-matrix/)~~
2. [What Are Minors?](https://byjus.com/jee/minors-and-cofactors/)
3. Book: Linear Algebra 4th


## Co-factor Matrix

### Co-factor of a specific element
Cofactor of an element $`a_{ij}`$ is related to its minor as 
$`
C_{ij} = (-1)^{(i+j)}M_{ij}
`$
<br>
where $`i`$ denotes the **ith** row and $`j`$ denotes the **jth** column to <br>
which the element $`a_{ij}`$ belongs. <sup>Ref[2]</sup>


### Co-factor Matrix
Co-factor matrix is a matrix having the co-factors as the elements of the matrix. <sup>Ref[1]</sup> <br>
Let matrix C is cofactor matrix of matrix A, $`C_{ij} = (-1)^{(i+j)}M_{ij}`$: <br>

$`
C =  \begin{pmatrix}
      (-1)^{1+1}M_{11} & (-1)^{1+2}M_{12} & (-1)^{1+3}M_{13}\\
      (-1)^{2+1}M_{21} & (-1)^{2+2}M_{22} & (-1)^{2+3}M_{23}\\
      (-1)^{3+1}M_{31} & (-1)^{3+2}M_{32} & (-1)^{3+3}M_{33}\\
      \end{pmatrix} 
      =  
      \begin{pmatrix}
      M_{11} & -M_{12} & M_{13}\\
      -M_{21} & M_{22} & -M_{23}\\
      M_{31} & -M_{32} & M_{33}\\
      \end{pmatrix} 
      =
      \begin{pmatrix}
      C_{11} & C_{12} & C_{13}\\
      C_{21} & C_{22} & C_{23}\\
      C_{31} & C_{32} & C_{33}\\
      \end{pmatrix} 
`$

### Co-factor Expansion <sup>Ref[3]<sup>
Let $`A`$ be an $`n × n`$ matrix.
The **cofactor expansion** of $`A`$ along the **ith** row is the sum <br>
$`a_{i,1}C_{i,1} + a_{i,2}C_{i,2} + · · · + a_{i,n}C_{i,n}`$.

The **cofactor expansion** of $`A`$ down the **jth** column is the sum <br>
$`a_{1,j}C_{1,j} + a_{2,j}C_{2,j} + · · · + a_{n,j}C_{n,j}`$.

### Applications of Co-factor Matrix <sup>Ref[1]<sup>

### Reference
1. [Cofactor Matrix](https://www.cuemath.com/algebra/cofactor-matrix/)
2. [Minors and cofactors](https://byjus.com/jee/minors-and-cofactors/)
3. [Section 3.3 'The Determinant' in Ref[3]](https://github.com/vitonzhangtt/LinearAlgebraNinja/edit/main/Reference.md#reference-list)


## Adjoint of a Matrix <sup>Ref[1]<sup>
The **adjoint of a matrix** $`B`$ is the transpose of the [cofactor matrix](#co-factor-matrix-1) of $`B`$.  <br>
The adjoint of a square matrix $`B`$ is denoted by $`adj(B)`$. 

### Properties 
1. If $`0`$ is a **null matrix** and $`I`$ is an identity matrix then, $`adj(0) = 0`$ and $`adj(I) = I`$ 
2. $`adj(B^T) = adj(B)^T`$, here $`B^T`$ is a transpose of a matrix $`B`$
3. The **determinant** of a matrix $`B`$ can be defined as the product of $`B`$ with its adjoint <br>
yielding a diagonal matrix whose diagonal entries are the determinant $`det(B)`$. <br>
$`B adj(B) = adj(B) B = det(B) I`$, where $`I`$ is an **identity matrix**.
4. Suppose C is another square matrix then, $`adj(BC) = adj(C) adj(B)`$
5. For any **non-negative integer** $`k`$, $`adj(Bk) = adj(B)k`$.
6. The adjoint of a diagonal matrix is a diagonal matrix again.

### Applications

### Reference
1. [Adjoint of a Matrix](https://www.cuemath.com/algebra/adjoint-of-a-matrix/)

## Diagonal Matrix

A matrix $`A = [a_{ij}]`$ is said to be **diagonal** if
$`A`$ is a square matrix and $`a_{ij}=0 \text{ when }i \neq j.`$

### Examples
The following matrics are diagonal.

$`
A = \begin{pmatrix}
      1 & 0 & 0 \\
      0 & 5 & 0 \\
      0 & 0 & 6 \\
    \end{pmatrix} 
`$

$`
R = \begin{pmatrix}
      2 & 0 \\
      0 & 5 \\
    \end{pmatrix} 
`$

$`
B = \begin{pmatrix}
      4 & 0 & 0 \\
      0 & 0 & 0 \\
      0 & 0 & 7 \\
    \end{pmatrix} 
`$

Note: The diagonal elements of a diagonal matrix can be either zeros or non-zeros.

### Properties of a Diagonal Matrix

#### Property A: **Identity matrix**, **null matrix**, and **scalar matrix** are diagonal matrics.
   
#### Property B: The sum of two diagonal matrics (of the same order) is diagonal.
If $`n x n`$ matrics $`A`$ and $`B`$ are both diagonal matrics, then $`A+B`$ is also diagonal matrics.

#### Property C: The product of two diagonal matrices (of the same order) is a diagonal matrix.
$`A=[a_{ij}] \text{ and } B=[b_{ij}]`$ are diagonal matrics, matrix $`M`$ is $`M=A \times B`$. The entries <br>
of M matrix equals to $`m_{ij} = a_{ij} \times b_{ij}`$. <br>
For example,
let $`
A  = \begin{pmatrix}
      2 & 0 \\
      0 & 5 \\
      \end{pmatrix} 
`$

and $`
B = \begin{pmatrix}
      10 & 0 \\
      0 & -6 \\
      \end{pmatrix} 
`$
then $`
M = A \times B = \begin{pmatrix}
      20 & 0 \\
      0 & -30 \\
      \end{pmatrix}
`$

#### Property D: Diagonal matrices are **commutative** under both addition and multiplication.

#### Property E: Diagonal matrices are symmetric matrices(i.e. $`A=A^T`$). 

### Theorem

#### Theorem 1
For any square matrix $`A`$ with real number elements, $`A + A^T`$ is a **symmetric matrix**, and $`A - A^T`$ <br>
is a **skew-symmetric** matrix.

#### Theorem 2
Any square matrix $`A`$ can be expressed as the sum of a **symmetric matrix**, $`S`$ and <br>
a **skew symmetric matrix**, $`V`$, such that,
$`A = (1/2) × (A + A^T) + (1/2 ) × (A - A^T)`$. <br>
Here, $`A^T`$ is the transpose of the square matrix $`A`$.

1. If $`A + A^T`$ is a symmetric matrix, then $`(1/2) × (A + A^T)`$ is also a symmetric matrix.
2. If $`A - A^T`$ is a skew symmetric matrix, then $`(1/2 ) × (A - A^T)`$ is also a skew symmetric matrix.

### Reference
1. [Diagonal Matrix](https://www.cuemath.com/algebra/diagonal-matrix/)


## Order of matrix
The order of matrix gives the dimension of the matrix, and it informs  <br>
the number of rows and columns present in the matrix.  <br>
The order of matrix is general represented as $`A_{m \times n}`$, <br>
where $`m`$ is the number of rows, and $`n`$ is the number of columns in the given matrix. <br>

### Reference
[Order of matrix](https://www.cuemath.com/algebra/order-of-matrix/)

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


## Properties of Transpose
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


## Hermitian Matrix
A hermitian matrix is a square matrix, which is equal to its [conjugate transpose](#conjugate-transpose-matrix) <br>
matrix. The non-diagonal elements of a hermitian matrix are all complex numbers. <br> 
If $`A=A^{\mathrm {H}}`$, then A is hermitian matrix.

The complex numbers in a hermitian matrix are such that the element of the $`ith`$ row <br>
and $`jth`$ column is the complex conjugate of the element of the $`jth`$ row and $`ith`$ column. <br>
So for $`i \neq j`$, in the hermitian matrix $`a_{ij}=a_{ji}`$.

### Properties of Hermitian Matrix


### Reference
[Hermitian Matrix](https://www.cuemath.com/algebra/hermitian-matrix/)

## Skew-Hermitian matrix
A square matrix (with real/complex entries) $`A`$ is said to be a **skew Hermitian matrix** <br>
if and only if $`A^{\mathrm {H}} = -A`$, where $`A^{\mathrm {H}}`$ is the [conjugate transpose](#conjugate-transpose-matrix) of $`A`$.

### Properties

### Reference
[Skew Hermitian Matrix](https://www.cuemath.com/algebra/skew-hermitian-matrix/)

## Nilpotent Matrix

### Reference
[Nilpotent Matrix](https://www.cuemath.com/algebra/nilpotent-matrix/)

## Square Matrix
A **square matrix** is a matrix with an equal number of rows and columns.

### Reference
[Square Matrix](https://www.cuemath.com/algebra/square-matrix/)

## Orthogonal matrix
An **orthogonal matrix** is a **square matrix** A if and only its transpose is as same as <br>
its inverse. i.e., $`A^T = A^{-1}`$, where $`A^T`$ is the transpose of $`A`$ and $`A^{-1}`$ is the inverse of A. <br>
So for orthogonal matrix A, $`A{A^T}=I_{n}`$

### Reference
https://www.cuemath.com/algebra/orthogonal-matrix/

## Singular Matrix
A **singular matrix** is a square matrix if its **determinant** is 0, $`det(A)=0`$. <br>
A **singular matrix** is a square matrix if it's non-invertible, i.e. $`A^{-1}`$ is not defined.


### Reference
[Singular Matrix](https://www.cuemath.com/algebra/singular-matrix/)

## Symmetric matrix
A symmetric matrix is a square matrix that is equal to its transpose matrix. $`A=A^T`$

### Properties

### Reference
[Symmetric Matrix](https://www.cuemath.com/algebra/symmetric-matrix/)

## Skew-symmetric matrix
In mathematics, a skew symmetric matrix is defined as the square matrix that is equal <br>
to the negative of its transpose matrix. <br>
For any square matrix, $`A`$, the transpose matrix is given as $`A^T`$. <br>
A **skew-symmetric** or **antisymmetric** matrix $`A`$ can therefore be represented 
as, $`A = -A^T`$. <br>
For example,

$`A= \begin{pmatrix}
      0 & 4 & 3 \\
      -4 & 0 & -6 \\
      -3 & 6 & 0 \\
      \end{pmatrix} 
`$

### Property A: If $`A`$ and $`B`$ is Skew-symmetric, then $`(A+B)`$ is Skew-symmetric.

### Property B: If $`A`$ is Skew-symmetric, then $`tr(A) = 0`$. 

### Property C: The real eigenvalue of a real skew symmetric matrix $`A`$, $`λ`$ equal zero.

### Property D: If $`k`$ is scalar and $`B`$ is skew symmetric matrix, then $`(kB)^T = -kB`$.

### Reference
[Skew Symmetric Matrix](https://www.cuemath.com/algebra/skew-symmetric-matrix/)

## Conjugate matrix (Complex Conjugate of a Matrix)

### Complex Conjugate
A complex conjugate of a complex number is another complex number whose  <br>
real part is the same as the original complex number and the magnitude  <br>
of the imaginary part is the same with the opposite sign.  <br>

A complex number is of the form $`a + ib`$, where $`a, b`$ are real numbers, <br>
$`a`$ is called the real part, $`b`$ is called the imaginary part, <br>
and $`i`$ is an imaginary number equal to the root of negative 1.

The complex conjugate of complex number z is denoted by $`\bar{z}`$. <br>
If $`z=2+3i`$, then the conjugate of $`z`$ is $`\bar{z}=2-3i`$.

### Multiplication of Complex Conjugate
let $`z=a+ib`$, $`\bar{z}=a-ib`$, then $`z*\bar{z}=(a+ib)(a-ib)=a^2+b^2`$.

### Complex Conjugate Root Theorem
The complex conjugate root theorem states that if $`f(x)`$ is a polynomial with <br>
real coefficients and $`a + ib`$ is one of its roots, where $`a`$ and $`b`$ are real numbers, <br>
then the complex conjugate $`a - ib`$ is also a root of the polynomial $`f(x)`$. <br>

### Conjugate matrix
The **complex conjugate of a matrix** $`A`$ with complex entries is another matrix <br>
whose entries are the complex conjugates of the entries of matrix $`A`$. <br>
The complex conjugate of matrix $`A`$ is denoted by $`\bar{A}`$. <br> 

For example:
$`
A= \begin{pmatrix}
      3 & 3-i \\
      1+i & 2 \\
      \end{pmatrix} 
`$
then complex conjugate of $`A`$ is:
$`
\bar{A}= \begin{pmatrix}
      3 & 3+i \\
      1-i & 2 \\
      \end{pmatrix} 
`$

### Reference
[Complex Conjugate](https://www.cuemath.com/numbers/complex-conjugate/) 


## Conjugate transpose (matrix)
In mathematics, the **Conjugate transpose**, also known as the **Hermitian transpose**, of an <br>
$`m \times n`$ complex matrix $`{\boldsymbol {A}}`$ is an $`n\times m`$ matrix obtained <br>
by transposing $`{\boldsymbol {A}}`$ and applying complex conjugate on each entry. <br>
It is often denoted as $`{\displaystyle {\boldsymbol {A}}^{\mathrm {H} }}`$ or $`{\displaystyle {\boldsymbol {A}}^{*}}`$ or 
$`{\displaystyle {\boldsymbol {A}}'}`$, and very commonly in physics as 
$`{\displaystyle {\boldsymbol {A}}^{\dagger }}`$. <br>

For example, for matrix $`A`$: <br>
$`
A= \begin{pmatrix}
      1 & -2-i & 5 \\
      1+i & i & 4-2i \\
      \end{pmatrix} 
`$

$`
A^T= \begin{pmatrix}
      1 & 1+i       \\
      -2-i & i      \\
      5 & 4-2i      \\
      \end{pmatrix} 
`$

The conjugate transpose of $`A`$ is: 
$`
A^{\mathrm {H}}= 
      \begin{pmatrix}
      1 & 1-i       \\
      -2+i & -i      \\
      5 & 4+2i      \\
      \end{pmatrix} 
`$

### Notations: $`A^*`$,  $`A^H`$,  $`A^{\textdagger}`$,  $`A^+`$
Conjugate transpose can be denoted as $`A^*`$,  $`A^H`$,  $`A^{\textdagger}`$ and $`A^+`$.

| Notation | Description |
| --- | --- |
| $`A^*`$ | commonly used in linear algebra |
| $`A^H`$ |commonly used in linear algebra |
| $`A^{\dagger}`$ | (sometimes pronounced as A dagger), commonly used in quantum mechanics |
| $`A^+`$ | although this symbol is more commonly used for the Moore–Penrose pseudoinverse |

In some contexts, $`{A}^{*}`$ denotes the matrix with only complex conjugated entries and no transposition.

### Properties of the conjugate transpose

#### Property A: $`{\displaystyle ({\boldsymbol {A}}+{\boldsymbol {B}})^{\mathrm {H} }={\boldsymbol {A}}^{\mathrm {H} }+{\boldsymbol {B}}^{\mathrm {H} }}`$ If $`A`$ and $`B`$ have the same order.

#### Property B: $`{\displaystyle (z{\boldsymbol {A}})^{\mathrm {H} }={\overline {z}}{\boldsymbol {A}}^{\mathrm {H} }}`$ for any complex number z and any $`m \times n`$ matrix $`{\boldsymbol {A}}`$.

#### Property C:

#### Property D:

#### Property E:

### Reference
[Conjugate transpose](https://en.wikipedia.org/wiki/Conjugate_transpose)

## Unitary matrix (酉矩阵)
A unitary matrix is a square matrix of complex numbers, whose inverse is equal to <br>
its [conjugate transpose](#conjugate-transpose-matrix). If $`U^{\mathrm {H}}=U^{-1}`$, then U is unitary matrix.

### Reference
[Unitary Matrix](https://www.cuemath.com/algebra/unitary-matrix/)

## Null matrix (Zero matrix)
**Null matrix** is a matrix having zero as each of its elements. <br>
The null matrix is also called a **zero matrix**.

### Reference
[Null Matrix - Zero Matrix](https://www.cuemath.com/algebra/null-matrix/)

## Homogeneous Representation

### Reference
1. [Chapter 5 Homogeneous Representations of Points, Lines and Planes](https://www.ipb.uni-bonn.de/book-pcv/pdfs/PCV-A-sample-page.pdf)
2. [Homogeneous coordinates](https://en.wikipedia.org/wiki/Homogeneous_coordinates)

## Matrix exponential

### Reference

## Frobenius norm

The Frobenius norm is a way to measure the "size" of a matrix, defined as the square root <br>
of the sum of the squares of all its elements. 

It is calculated by summing the squares of every element, and then taking the square <br>
root of that sum. 

$`{\Vert A \Vert}_{F} = \sqrt{ \underset{j,k}{\sum {{a^2}_{jk}} }}`$

## 2-norm

The 2-norm of a matrix $`A`$ is the square root of the largest eigenvalue of $`A^{T}A`$. <br>
Alternatively, it is defined as the **maximum singular value** of the matrix.

$`{\Vert A \Vert}_{2} = \underset{|v|=1}{max|Av|}`$
