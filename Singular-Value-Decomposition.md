# Singular Value Decomposition (奇异值分解)

The singular value decomposition of a matrix $`A`$ is the factorization of $`A`$ into the <br>
product of three matrices $`A = UDV^{T}`$ where the columns of $`U`$ and $`V`$ are orthonormal and <br>
the matrix $`D`$ is diagonal with positive real entries. <sup>[1]</sup>

Singular value decomposition is defined for all matrices (**rectangular or square**) <br>
unlike the more commonly used *spectral decomposition* in Linear Algebra. <sup>[1]</sup>

In contrast, the columns of $`V`$ in the singular value decomposition, called the **right singular** <br>
**vectors** of $`A`$, always form an orthogonal set with no assumptions on $`A`$. The columns <br>
of $`U`$ are called the **left singular vectors** and they also form an orthogonal set. A simple <br>
consequence of the **orthogonality** is that for a **square and invertible matrix** $`A`$, the inverse <br>
of A is $`VD_{−1}U_{T}`$, as the reader can verify. <sup>[1]</sup>

## Applications

### Find low rank matrix $`B`$ which is close to data matrix $`A`$

The data matrix $`A`$ is close to a matrix of low rank and it is useful to find a low [rank]() matrix <br>
which is a good approximation to the data matrix. <sup>[1]</sup>

### 



## Reference
1. [Singular Value Decomposition (SVD)](https://www.cs.cmu.edu/~venkatg/teaching/CStheory-infoage/book-chapter-4.pdf) from cmu
