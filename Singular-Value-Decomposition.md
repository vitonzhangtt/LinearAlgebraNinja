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
of $`A`$ is $`VD^{−1}U^{T}`$, as the reader can verify. <sup>[1]</sup>

## Applications

### Find low rank matrix $`B`$ which is close to data matrix $`A`$

The data matrix $`A`$ is close to a matrix of low rank and it is useful to find a low [rank]() matrix <br>
which is a good approximation to the data matrix. <sup>[1]</sup>

### 

## First Singular Vector <sup>[1]</sup>

With this in mind, define the **first singular vector**, $`v_{1}`%, of $`A`$, which is a **column vector**, <br> 
as the best fit line through the origin for the $`n`$ points in **d-space** that are the rows of $`A`$. <br>
The matrix $`A`$ is like the following:

$`A = \begin{bmatrix}
   a_{1,1} & a_{1,2} & \cdots & a_{1,d} \\
   a_{2,1} & a_{2,2} & \cdots & a_{2,d} \\
   \vdots  & \vdots  & \ddots & \vdots  \\
   a_{n,1} & a_{n,2} & \cdots & a_{n,d} 
\end{bmatrix}`$ 

Thus 

$`\mathbf{v_{1}} = \underset{|v|=1}{argmax |A\mathbf{v}|}`$

The value $`\sigma_{1} (A) = |Av_{1}|`$ is called the **first singular value** of $`A`$. <br> 
Note that $`\sigma_{1}^2`$ is the sum of the squares of the projections of the points to <br>
the line determined by $`v_{1}`$.

### Argmax <sup>Google AI Overview</sup>
**Argmax** (or arg max) stands for "argument of the maximum". It is a mathematical operation <br>
that finds the **input value** from a function's domain that produces the function's greatest <br>
output value. This is distinct from the **max** function, which simply returns the maximum <br>
output value itself. The **argmax** operation can apply to *functions, sets, or arrays*. 

#### Argmax for a function 

For a function $`f(x)`$, the expression $`\mathrm{argmax}f(x)`$ returns the value of $`x`$ for <br> 
which $`f(x)`$ is at its maximum. 

#### Argmax for an array
In programming and data science, **argmax** is often used with arrays to find the index of the maximum value. 

## Second Singular Vector <sup>[1]</sup>

For every 2-dimensional subspace containing $`v_{1}`$, the sum of squared lengths of the projections <br>
onto the subspace equals the sum of squared projections onto $`v_{1}`$ plus the sum of squared <br>
projections along a vector *perpendicular to* $`v_{1}`$ in the subspace. 

Using the same greedy strategy to find the best three and higher dimensional **subspaces**, defines <br>
$`v_{3}`$, $`v_{4}`$, . . . in a similar manner.

The **second singular vector**, $`v_{2}`$, is defined by the best fit line perpendicular to $`v_{1}`$ <br>

$`v_{2} = \underset{,|v|=1}{argmax|Av|}`$















## Reference
1. [Singular Value Decomposition (SVD)](https://www.cs.cmu.edu/~venkatg/teaching/CStheory-infoage/book-chapter-4.pdf) from cmu
2. [What Is Argmax in Machine Learning?](https://machinelearningmastery.com/argmax-in-machine-learning/)
3. [15 Singular Value Decomposition](https://users.cs.utah.edu/~jeffp/teaching/cs5140-S15/cs5140/L15-SVD.pdf) from utah [To Read]
4. [7.4 Singular Value Decompositions](https://understandinglinearalgebra.org/sec-svd-intro.html) [To Read]
5. [Singular Value Decomposition (SVD), Demystified](https://towardsdatascience.com/singular-value-decomposition-svd-demystified-57fc44b802a0/)
