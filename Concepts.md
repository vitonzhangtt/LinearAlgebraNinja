# Concepts

## Column space

## Nullspace
$`A`$ is a matrix with $`m \times n`$, as $`A_{m,n}`$.
The nullspace $`N(A)`$ consists of all solutions to $`A\mathbf{x}=0`$. These vectors $`\mathbf{x}`$ are in $`R^n`$. 

### Reference
Ref[1]: Section 3.2 

## Minor of a specific element
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


## Minor of matrix

### Reference
[Minor of matrix](https://www.cuemath.com/algebra/minor-of-matrix/)

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


## Cofactor Matrix

### Reference
[Cofactor Matrix](https://www.cuemath.com/algebra/cofactor-matrix/)


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
A **singular matrix** is a square matrix if its **determinant** is 0, $`det(A)=0`$.

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
In mathematics, the **conjugate transpose**, also known as the **Hermitian transpose**, of an <br>
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


### Reference
[Conjugate transpose](https://en.wikipedia.org/wiki/Conjugate_transpose)

## Unitary matrix
A unitary matrix is a square matrix of complex numbers, whose inverse is equal to <br>
its [conjugate transpose](#conjugate-transpose-matrix). If $`U^{\mathrm {H}}=U^{-1}`$, then U is unitary matrix.

### Reference
[Unitary Matrix](https://www.cuemath.com/algebra/unitary-matrix/)

## Null matrix (Zero matrix)
**Null matrix** is a matrix having zero as each of its elements. <br>
The null matrix is also called a **zero matrix**.

### Reference
[Null Matrix - Zero Matrix](https://www.cuemath.com/algebra/null-matrix/)

## Matrix exponential



### Reference



