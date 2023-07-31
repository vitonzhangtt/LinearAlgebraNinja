# Matrix Exponentials ($`e^A`$)

## Exponential Function <sup>Ref[2] Ref[3]</sup>
The exponential function is a type of mathematical function which are helpful <br>
in finding the growth or decay of population, money, price, etc that are <br> 
growing or decay exponentially. 

Exponential function has a constant as its base and a variable as its exponent. <br>
The $`f`$ is an exponential function with parameter $`c`$ and $`b`$. <br>
$`f(x)=cb^x`$ <br>
When $`c=1, b=e`$, we get the following: <br>
$`f(x)=e^x`$

### Power function <sup>Ref[2]</sup>
Power function is a function which has a variable as the base and a constant as the exponent, 
$`f(x)=x^a`$.

### Power Series Expansion <sup>Ref[6]</sup>
$`e^x=\displaystyle\sum_{n=0}^{\infty} \frac{x^n}{n!}`$

## Why we need matrix exponential?



## Matrix Exponential <sup>Ref[8]</sup>
The exponential of a square matrix A is defined by the power series: <br>
$`e^A=I+A+\frac{A^2}{2!}+\frac{A^3}{3!}+\dots`$ <br>

Let $`A^0=I`$, then
$`e^A=\displaystyle\sum_{n=0}^{\infty} \frac{A^n}{n!}`$  

### Definition as limit

### Theorem 1 <sup>Ref[1]</sup>
If $`AB = BA`$, then $`e^{A}e^{B} = e^{A+B}`$.

#### Corollary 1 
Let $`A`$ be an $`n × n`$ matrix.
1. For any **real numbers** $`t`$ and $`s`$, we have $`e^{tA}e^{sA} = e^{(t+s)A}`$.
2. The matrix $`e^{A}`$ is **invertible**, and $`(e^A)^{−1} = e^{−A}`$.

##### Proof
For first, $`tA`$ and $`sA`$ are commute(i.e. $`tA \times sA = sA \times tA`$), so $`e^{tA}e^{sA} = e^{(t+s)A}`$ hold. 

For second, $`A`$ and $`-A`$ are commute, $`e^{A}e^{-A} = e^{A+(-A)}=e^{0_{n \times n}}= I_{n}`$, so $`(e^A)^{−1} = e^{−A}`$ hold.

### Theorem 2<sup>Ref[1]</sup>: $`(e^A)^T=e^{A^T} \text{ for any } n \times n \text{ matrix } A`$
$`A^T`$ is transpose of matrix $`A`$.

#### Proof
Accroding to properties of transpose <sup>Ref[10]</sup>, we have $`(A^n)^T = (A^T)^n`$ and $`(A+B)^T=A^T+B^T`$ then <br>
$`e^{A^T}=\displaystyle\sum_{n=0}^{\infty} \frac{{(A^T)}^n}{n!}=\displaystyle\sum_{n=0}^{\infty} \frac{{(A^n)}^T}{n!}=(\displaystyle{\sum_{n=0}^{\infty} \frac{(A^n)}{n!}})^T=(e^A)^T`$

### Property B: The Matrix Exponential of a [Diagonal Matrix](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Concepts.md#diagonal-matrix) 

Let $`M`$ is a **diagnoal matrix** with $`n = 3`$ as the following, <br>
$`
M =   
      \begin{pmatrix}
        m_{11} & 0 & 0 \\
        0 & m_{22} & 0 \\
        0 & 0 & m_{33} \\
      \end{pmatrix} 
`$

then $`M^0`$, $`M^2`$, $`M^k`$ are:
$` 
M^0 =   
      \begin{pmatrix}
        1 & 0 & 0 \\
        0 & 1 & 0 \\
        0 & 0 & 1 \\
      \end{pmatrix} 
`$ 

$` 
M^2 =   
      \begin{pmatrix}
        {m_{11}}^2 & 0 & 0 \\
        0 & {m_{22}}^2 & 0 \\
        0 & 0 & {m_{33}}^2 \\
      \end{pmatrix} 
`$ 

$` 
M^k =   
      \begin{pmatrix}
        {m_{11}}^k & 0 & 0 \\
        0 & {m_{22}}^k & 0 \\
        0 & 0 & {m_{33}}^k \\
      \end{pmatrix} 
`$ 

The matrix exponential of $`M`$ is $`e^M`$ which is as the following. <br>
$`
e^M= 
      \begin{pmatrix}
        e^{m_{11}} & 0 & 0 \\
        0 & e^{m_{22}} & 0 \\
        0 & 0 & e^{m_{33}} \\
      \end{pmatrix} 
`$ 

#### Proof <sup>Ref[11]</sup>

### Theorem 3 <sup>Ref[1]</sup>
Let $`A`$ be an $`n \times n`$ matrix. Then
1. If $`λ`$ is an eigenvalue for $`A`$, then $`e^λ`$ is an eigenvalue for $`e^A`$.
2. More precisely, if $`\vec{v}`$ is an eigenvector for $`A`$ with eigenvalue $`λ`$, then $`\vec{v}`$ is an <br>
eigenvector for $`e^A`$ with eigenvalue $`e^λ`$.

## Rotations as matrix exponentials <sup>Ref[1]</sup>

Using matrix exponentials represent rotation. <br>
An $`{n × n}`$ matrix is called **[skew-symmetric](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Concepts.md#skew-symmetric-matrix)** if $`A^T = −A`$.

### Theorem 1
If $`A`$ is a **skew-symmetric** $`n \times n`$ matrix, then $`e^A`$ is orthogonal. Additionally, $`det(e^A) = 1`$, <br>
so $`e^A`$ is a **rotation matrix**.

#### Exmaple (when $`n=2`$)
For a $`2×2`$ matrix 
$`
A =  \begin{pmatrix}
      a & b \\
      c & d \\
      \end{pmatrix}
`$,
we see $`A`$ is **skew-symmetric** if and only if $`A^T = −A`$: <br>
$`
A^T = \begin{pmatrix}
      a & c \\
      b & d \\
\end{pmatrix} = \begin{pmatrix} 
-a & -b \\
-c & -d \\
\end{pmatrix} = -A
`$

Hence a 2 × 2 skew-symmetric matrix has the form
$`\begin{pmatrix}
0 & −b \\
b & 0 \\
\end{pmatrix}
`$. This is precisely <br>
the family of matrices we took the exponential of when we computed

$`e^A=exp(\begin{bmatrix} 0 & −t \\ t & 0 \\ \end{bmatrix}) = \begin{bmatrix} \cos{t} & −\sin{t} \\ \sin{t} & \cos{t} \\ \end{bmatrix}`$


### Theorem 2: Skew matrics and Rotation Matrics
If $`A`$ is a **skew-symmetric** $`n \times n`$ matrix, then $`e^{tA}`$ is a rotation matrix <br>
for each **real number** $`t`$.


### Theorem 3: Rotation axis and angle
Let $`\vec{v} = [x, y, z]^T`$ be a unit vector and let $`A = \begin{bmatrix} 0 & −z & y \\ z & 0 & -x \\ -y & x & 0 \\ \end{bmatrix}`$. <br>
Then rotation about the line through the origin in the direction of $`\vec{v}`$ by $`θ`$ radians <br>
is given by the matrix $`e^{θA}`$.

#### Example: calculate the rotation matrics

If we want to rotate about the axis determined by $`\vec{v} = [3, 2, -6]^T`$ by 27 degrees. <br>
The angle is $`θ = \frac{2\pi}{360} \times 27=\frac{3\pi}{20}`$ radians.

**Unit vector**: <br>

$`\vec{u}=\frac{1}{\lVert \vec{v} \rVert} \times \vec{v}=\frac{1}{\sqrt{9+4+36}} \times [3, 2, -6]^T = [\frac{3}{7}, \frac{2}{7}, \frac{-6}{7}]^T`$

So, $`x=\frac{3}{7}, y=\frac{2}{7}, z=\frac{-6}{7}`$ and $`A=\begin{bmatrix} 
            0 & \frac{6}{7} & \frac{2}{7} \\ 
            \frac{-6}{7} & 0 & \frac{-3}{7} \\ 
            \frac{-2}{7} & \frac{3}{7} & 0 \\ 
      \end{bmatrix}`$

**Rotation matrix**: <br>
$`
e^{θA} = exp(\frac{3\pi}{20} \times 
      \begin{bmatrix} 
            0 & \frac{6}{7} & \frac{2}{7} \\ 
            \frac{-6}{7} & 0 & \frac{-3}{7} \\ 
            \frac{-2}{7} & \frac{3}{7} & 0 \\ 
      \end{bmatrix})
`$

Note: **expm** command in MATLAB.


## Reference
1. [Exponentials and Rotations (AAAA+)](https://www.math.umd.edu/~immortal/MATH401/book/ch_exponentials_and_rotations.pdf)
2. [Exponential Function](https://www.cuemath.com/calculus/exponential-functions/)
3. [The exponential function](https://mathinsight.org/exponential_function)
4. [The Matrix Exponential](https://nesinkoyleri.org/wp-content/uploads/2021/07/Exponential.pdf)
5. [wiki: Matrix_exponential](https://en.wikipedia.org/wiki/Matrix_exponential)
6. [Power Series Expansion for Exponential Function](https://proofwiki.org/wiki/Power_Series_Expansion_for_Exponential_Function)
7. [7.8 Matrix exponentials](https://web.uvic.ca/~tbazett/diffyqs/sec_matexp.html)
8. [What Is the Matrix Exponential?](https://nhigham.com/2020/05/28/what-is-the-matrix-exponential/)
9. [The Matrix exponential, Dynamic Systems and Control](https://www2.imm.dtu.dk/pubdb/edoc/imm3059.pdf)
10. [Transpose properties](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Concepts.md#properties-of-transpose)
11. [The Matrix Exponential of a Diagonal Matrix](https://yutsumura.com/the-matrix-exponential-of-a-diagonal-matrix/)
12. [The Matrix Exponential e^{tA}.](https://www.youtube.com/watch?v=WSt9R66U6Po)
13. [How (and why) to raise e to the power of a matrix | DE6](https://www.youtube.com/watch?v=O85OWBJ2ayo)

