# Trace


## Definition
The **trace** of a matrix is defined as *the sum of the diagonal elements* of a matrix. <sup>[1]</sup>

## Properties

### It equals the sum of its eigenvalues

### Invariant under a change of basis
Therefore Trace of a matrix remains same independent of the basis in which the matrix is represented in. <sup>[1]</sup>

#### Change of basis
A change of basis operation finds the new representation of the matrix in a new basis. <br> 
These operations are essential when transforming from standard basis to other basis (example- eigen basis). <br> 
A change of basis operation transforms the entire grid into a new grid (with the origin remaining intact) <br> 
and no grid line curving. <sup>[1]</sup>

## The Practical Significance of the trace <sup>Google AI Overview</sup>
The practical significance of the trace of a matrix stems from two key properties: <br>
**it equals the sum of its eigenvalues** and **it is invariant under a change of basis**. <br>
These properties allow the trace to condense complex spectral information into a single <br>
scalar value that has consistent physical or statistical meaning across various applications. <br> 
Key practical applications and interpretations include: 

### In Statistics and Data Analysis 

* **Total Variance/Risk**: In statistics and finance, the trace of the covariance matrix is <br> 
  the sum of the variances of all individual variables. This provides a single measure of <br> 
  the total individual risk or "spread" in a dataset or investment portfolio, before <br> 
  considering the effects of diversification (covariances).
* **Dimensionality/Rank Estimation**: The trace of an idempotent (projection) matrix equals <br> 
  its rank, which is the dimension of the subspace it projects onto. <br> 
  This is useful in applications like **Principal Component Analysis (PCA)** for understanding <br> 
  the effective dimensionality of data.
* **Optimization Problems**: The trace is a linear operator and is often used as an analytic <br> 
  tool in matrix optimization problems, such as maximum likelihood estimation for **covariance matrices** <br>
  or in the derivation of algorithms like the **Kalman Filter**.

### In Physics and Engineering 
* **Quantum Mechanics**(量子力学): In quantum mechanics, the trace operation is used to calculate <br>
  the expectation value of an observable (a physical quantity being measured, represented by an operator).
* **Elasticity Theory**(弹性理论): The trace of the infinitesimal strain tensor represents the <br>
  fractional volume change (dilation) in a material when it is deformed.
* **Fluid Dynamics**(流体动力学): A vector field is considered divergence-free if the trace of <br>
  its **Jacobian matrix** is zero, a concept extensively used in physics for modeling fluid flow <br>
  and other continuous systems.
* **System Dynamics**(系统动力学): The trace is used in the analysis of matrix-valued dynamical systems, <br>
  where it can help build Lyapunov functions for assessing system stability.

### In Mathematics and Computer Science 
* **Inner Products and Norms**: The trace generalizes the standard inner product for vectors to matrices, <br>
  defining the **Frobenius inner product** $`\langle X,Y\rangle =\text{tr}(X^{T}Y)`$ and <br>
  the **induced Frobenius norm**.
* **Graph Theory**: In network theory, the trace of powers of an adjacency matrix $`tr((A^{k})`$ can <br>
  be used to count the number of closed walks or cycles of length $`k`$ in a graph.
* Group Representation Theory: The trace is crucial in defining the characters of linear representations <br>
  of groups, which completely characterize the representation theory. 



## Reference
1. [Geometric meaning of a trace](https://saksham-malhotra2196.medium.com/geometric-meaning-of-a-trace-85ac170229f8) (AAAA+)
2. [Understanding the Trace of a Matrix: Key Properties and Their Proofs](https://www.youtube.com/watch?v=F6EImVmPbb8)
3. [Understanding the Trace of a Matrix in C: A Comprehensive Guide](https://30dayscoding.com/blog/trace-of-a-matrix-in-c)
