# Matrix Exponentials

## Exponential Function <sup>Ref[^2] Ref[3]</sup>
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

## Matrix Exponential <sup>Ref[8]</sup>
The exponential of a square matrix A is defined by the power series: <br>
$`e^A=I+A+\frac{A^2}{2!}+\frac{A^3}{3!}+\dots`$ <br>

Let $`A^0=I`$, then
$`e^A=\displaystyle\sum_{n=0}^{\infty} \frac{A^n}{n!}`$  

### Definition as limit

## Theorem 1 <sup>Ref[1]</sup>
If $`AB = BA`$, then $`e^{A}e^{B} = e^{A+B}`$.

## Property A: $`(e^A)^T=e^{A^T}`$
$`A^T`$ is transpose of matrix $`A`$.

### Proof
Accroding to properties of transpose <sup>Ref[10]</sup>, we have $`(A^n)^T = (A^T)^n`$ and $`(A+B)^T=A^T+B^T`$ then <br>
$`e^{A^T}=\displaystyle\sum_{n=0}^{\infty} \frac{{(A^T)}^n}{n!}=\displaystyle\sum_{n=0}^{\infty} \frac{{(A^n)}^T}{n!}=(\displaystyle{\sum_{n=0}^{\infty} \frac{(A^n)}{n!}})^T=(e^A)^T`$

## Property B: The Matrix Exponential of a [Diagonal Matrix](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Concepts.md#diagonal-matrix) 

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

### Proof <sup>Ref[11]</sup>





## TODO [^3] [^4] [^12]

[^1]: [Exponentials and Rotations (AAAA+)](https://www.math.umd.edu/~immortal/MATH401/book/ch_exponentials_and_rotations.pdf)
[^2]: [Exponential Function](https://www.cuemath.com/calculus/exponential-functions/)
[^3]: [The exponential function](https://mathinsight.org/exponential_function)
[^4]: [The Matrix Exponential](https://nesinkoyleri.org/wp-content/uploads/2021/07/Exponential.pdf)
[^5]: [wiki: Matrix_exponential](https://en.wikipedia.org/wiki/Matrix_exponential)
[^6]: [Power Series Expansion for Exponential Function](https://proofwiki.org/wiki/Power_Series_Expansion_for_Exponential_Function)
[^7]: [7.8 Matrix exponentials](https://web.uvic.ca/~tbazett/diffyqs/sec_matexp.html)
[^8]: [What Is the Matrix Exponential?](https://nhigham.com/2020/05/28/what-is-the-matrix-exponential/)
[^9]: [The Matrix exponential, Dynamic
Systems and Control](https://www2.imm.dtu.dk/pubdb/edoc/imm3059.pdf)
[^10]: [Transpose properties](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Concepts.md#properties-of-transpose)
[^11]: [The Matrix Exponential e^{tA}.](https://www.youtube.com/watch?v=WSt9R66U6Po)
[^12]: [How (and why) to raise e to the power of a matrix | DE6](https://www.youtube.com/watch?v=O85OWBJ2ayo)

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

