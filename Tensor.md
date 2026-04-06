# Tensor

## Google AI Overview

Tensors are primarily contained within **linear algebra** and **multilinear algebra**, which provide the <br>
foundational definitions and operations. Because tensors are essential for describing geometric shapes <br>
and spaces that vary, they are also central to **differential geometry**. 

### Here is a breakdown of the mathematical fields and their context:

* Multilinear Algebra: **This is the most formal field where tensors are defined**. Tensors are considered <br>
  elements of tensor products of vector spaces, extending the concept of vectors and matrices.
* Linear Algebra: As generalizations of vectors (rank-1 tensors) and matrices (rank-2 tensors), they are <br>
  a primary focus of advanced linear algebra.
* Differential Geometry & Differential Topology: Tensors (often called tensor fields) are used here to <br>
  describe geometric properties of manifolds, such as curvature in general relativity.
* Tensor Calculus (Tensor Analysis): This subfield focuses specifically on the manipulation of tensors, <br>
  particularly concerning coordinate transformations (covariant and contravariant).
* Abstract/Algebraic Algebra: Tensors are often used in the context of tensor products of modules, <br>
  extending the algebraic properties beyond finite-dimensional vector spaces. 

In physics and engineering, the field of **continuum mechanics** frequently uses tensors to represent **stress** <br> 
and **strain**.

## Multilinear Algebra (多重线性代数)

### Books for Multilinear Algebra

* Multilinear Algebra by Werner Greub (Springer): A classic, comprehensive text in the Universitext series, suitable as a companion to advanced linear algebra.
* Multilinear Algebra by Russell Merris (CRC Press): Covers tensor spaces, symmetry classes, and group representation theory.
* Multilinear Algebra by D.G. Northcott (Cambridge University Press): Provides a solid theoretical foundation.
* Tensors: Geometry and Applications by J.M. Landsberg (AMS): Useful for applications of multilinear algebra in geometry.
* Finite Dimensional Multilinear Algebra by Marvin Marcus: Available in two parts, covering foundational aspects

## Definition of Tensor

Tensors are used in many fields, such as, Neural Networks, Continuum Mechanics or even General Relativity; <br>
and while tensors are a quite general concept, depending on which field you apply them, you may come across <br>
very different definitions. This is often the cause of a great deal of confusion. <sup>[1]</sup>

### Strict mathematical definition <sup>[1]</sup>

A type $`(p,q)`$ tensor $`T`$ is defined as a **multi-linear map**

<img width="397" height="69" alt="" src="https://github.com/user-attachments/assets/416c44d1-bc39-44ae-bc7d-6e11dc14adb0" />

Where $`V`$ is a **vector space** (also called **linear space**) over a **field** F, and $`V^*`$ is its corresponding <br>
[**dual space**](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Tensor.md#dual-space-%E5%AF%B9%E5%81%B6%E7%A9%BA%E9%97%B4). (Note that while $`F`$ is oftentimes the set of real numbers $`R`$, it could well be the rationals <br>
$`Q`$ or complex numbers $`C`$)

where $`q`$ is called the **covariant** order and $`p`$ is called the **contravariant** order of $`T`$. <sup>11.1 DEFINITIONS@[7]</sup>

The literal way of saying the above is:
Tensor is a collection of **vectors** and **covectors** combined together using the tensor product.

### (p, q) Tensor

The $`(p, q)`$ classification of a tensor defines its type based on the number of **contravariant** (upper, $`p`$) <br>
and **covariant** (lower, $`q`$) indices it possesses. This classification, often referred to as the <br>
tensor's "type," "valence," or "rank" (specifically, type $`(p, q)`$ means a total rank of $`p + q`$), dictates <br>
how the tensor's components change under coordinate transformations. <sup>Google AI Overview</sup>

#### Understanding $`(p, q)`$ Classification

* $`p`$ (Contravariant Indices - Upper): These indices indicate how the tensor transforms like a vector <br>
  (e.g., coordinate differentials $`dx^{\mu}`$).
* $`q`$ (Covariant Indices - Lower): These indices indicate how the tensor transforms like a **dual vector** <br>
  or **covector** (e.g., gradient $`\partial_{\mu} f`$).
* Total Order/Rank: The total number of indices is $`n = p+q`$, often described as the dimension of the <br>
  multi-dimensional array representing the tensor.

#### Examples of $`(p, q)`$ Tensors

* Type (0,0) - Scalar: A rank 0 tensor, such as temperature, which is a single number and does not change <br>
  under coordinate transformation.
* Type (1,0) - Contravariant Vector: A rank 1 tensor, such as velocity, with one upper index ($`v^i`$).
* Type (0,1) - Covariant Vector (Covector): A rank 1 tensor, such as a **gradient**, with one lower index ($`\omega_i`$).
* Type (1,1) - Mixed Tensor: A rank 2 tensor, such as the **Kronecker delta** $`\delta_{j}^{j}`$  or a linear <br>
  operator, with one upper and one lower index.
* Type (0,2) - Covariant Tensor: A rank 2 tensor, such as the metric tensor $`g_{ij}`$


#### Key Concepts for Mastering $`(p,q)`$ Classification

* Transformation Law: A $`(p, q)`$ tensor transforms using the Jacobian matrix ($`p`$ times for components, <br>
$`q`$ times for coordinates).
* Raising and Lowering Indices: You can change the $`(p, q)`$ type of a tensor using the metric tensor $`g_{ij}`$ <br>
  (or its inverse $`g^{ij}`$) without changing the underlying geometric object.
* Tensor Product: The combination of a type $`(p, q)`$ tensor and a type $`(r, s)`$ tensor results in a type <br>
  $`(p+r, q+s)`$ tensor.
* Contracting Indices: Summing over one upper and one lower index ($`T_{ij}^{i} = V_j`$) reduces the tensor type <br>
  by (1,1), resulting in a type $`(p-1,q-1)`$ tensor.
* Physical Meaning: Tensors describe physical, coordinate-independent relationships. The $`(p, q)`$ labels help <br>
  ensure that the equations formulated are consistent in different coordinate systems (e.g., general relativity).


### Covariant and Contravariant

In general terms, **covariance**(协变性) describes things that change together in the same direction as a <br>
reference, while **contravariance**(逆变性) describes things that change in the opposite direction. The meaning <br>
of these terms shifts depending on whether you are looking at them through the lens of physics/mathematics <br>
or computer science.

In **linear algebra** and **differential geometry**, these terms describe **how the components of a vector** <br>
**change when you change your basis (coordinate system)**.

Transformation Law: If a coordinate system transforms via $`M`$, contravariant vectors transform by $`M^{-1}`$, <br>
and covariant vectors transform by $`M`$.


#### Contravariance (Upper Indices, e.g., $`V^i`$):

* Definition: Components that transform using **the inverse of the basis change matrix**.
* Analogy: If you shrink your ruler (the basis), the number of units you measure (the components) must <br>
  increase to keep the physical object the same length.
* Examples: Position, velocity, and displacement. These are often what people mean when they simply say "vector."

#### Covariance (Lower Indices, e.g., $`W_i`$):

* Definition: Components that transform using the same matrix as the basis change.
* Analogy: These vary "with" the basis. If the basis vectors get longer, the covariant components <br>
  also "scale up" accordingly.
* Examples: Gradients and "one-forms" (or covectors). A gradient $`\frac{\partial \phi}{\partial x^i}`$ naturally has its index downstairs.


### Multilinear Map (多重线性映射) <sup>[7]</sup>

A **multilinear map** is a **function** of several variables that is linear in each variable independently, <br>
generalizing linear and **bilinear maps**. It takes inputs from multiple vector spaces (e.g., $`V_1, V_2, ..., V_k`$) <br> 
and maps them to a final space ($`W`$). It is "linear in each coordinate," meaning if you fix all variables <br>
except one, the mapping is linear.

#### Definition

For a map $`f: V_1 \times ... \times V_k \rightarrow W`$, $`f`$ is multilinear if  

$`f(v_1, ..., \lambda v_i + \mu {v^{\prime}}_i, ..., v_k) = \lambda f(v_1, ..., v_i, ..., v_k) + \mu f(v_1, ..., {v^{\prime}}_i, ..., v_k)`$ for any $`i`$.

#### Key Aspects of Multilinear Maps
* Linearity vs. Multilinearity: If a function has only one input ($`k=1`$), it is a standard linear map.
* Tensors: A multilinear map can be viewed as a tensor, particularly when mapping into a field ($`W = F`$), <br>
  where it is termed an $`r`$-tensor or multilinear form.
* Determinant Example: The determinant of a matrix is a key example, acting as an alternating multilinear map
  on the rows (or columns) of the matrix.
* Applications: These maps are fundamental in **multilinear algebra**, **differential geometry (tensors)**, and
  **advanced cryptography**.

### Dual Space (对偶空间)

#### Definition <sup>[3]</sup>

Given a vector space $`V`$, we define its **dual space** $`V^*`$ to be **the set of all linear transformations** <br>
$`\varphi: V \rightarrow F`$. The $`\varphi`$ is called a **linear functional**. In other words, $`\varphi`$ is <br>
something that accepts a vector $`v \in V`$ as input and spits out an element of $`F`$ (lets just assume that <br>
$`F = R`$, meaning that it spits out a real number). If you take all the possible (linear) ways that a $`\varphi`$ <br>
can eat such vectors and produce real numbers, you get $`V^*`$.

#### Examples of dual spaces

Here is a list of examples of dual spaces:

##### Example 1

Let $`V = R^3`$ and $`\varphi: R^3 \rightarrow R`$, then $`\varphi(x,y,z) = 2x+3y+4z`$ is a member of $`V^*`$.

##### Example 2

Let $`V = P_n`$ (the set of polynomials with degreee $`n`$) and $`\varphi: P_n \rightarrow R`$, then $`\varphi(p) = p(1)`$ <br>
is a member of $`V^*`$. Concretely, $`\varphi(1+2x+3x^2) = 1+2 \cdot 1 + 3 \cdot 1^2 = 6`$.

##### Example 3

Let $`V = M_{n \times n}`$ (the set of matrices with dimensions $`n \times n`$) and $`\varphi: M_{n \times n} \rightarrow R`$, then $`\varphi(A) = Trace(A)`$ is a member of $`V^*`$. In specific,

<img width="347" height="93" alt="" src="https://github.com/user-attachments/assets/c338b533-d15c-46ab-aa89-06db7ac99c92" />

##### Example 4

Let $`V = C([0, 1])`$ (the set of all continuous function on the interval $`[0, 1]`$) and $`\varphi: C([0, 1] \rightarrow R`$, then $`\varphi(g) = \int_{0}{1} g(x) dx`$ is a member of $`V^*`$. <br>
For instance, $`\varphi(e^x) = \int_{0}{1} e^x dx = e^1 - 1 = e - 1`$.

As it turns out, the elements of $`V^*`$ satisfy the **axioms of a vector space** and therefore $`V^*`$ <br>
is indeed a vector space itself.

#### The dual basis <sup>[3]</sup>

If $`b = {v_1, v_2, \cdot\cdot\cdot, v_n }`$ is a basis of vector space $`V`$, then $`b^* = {\varphi_1, \varphi_2, \cdot\cdot\cdot,\varphi_n}`$ is a basis of $`V^*`$. <br>
If you define $`\varphi`$ via the following relations, then the basis you get is called the **dual basis**:

<img width="424" height="62" alt="" src="https://github.com/user-attachments/assets/00281376-6d34-4dd9-b579-700c9d779d96" />

It is as if the functional $`\varphi`$ acts on a vector $`v \in V`$ and returns the $`i`$-th component $`a_i`$. <br>
Another way to write the above relations is if you set $`\varphi_i(v_j) = \delta_{ij}`$.

Then any functional $`\varphi`$ can be written as a linear combination of the dual basis vectors, i.e.

<img width="410" height="46" alt="" src="https://github.com/user-attachments/assets/0216f166-27c3-4793-bd48-94bb73ba20f6" />

##### Example


#### The dual of a dual space <sup>[3]</sup>




### Covectors





## TODO

1. google "What Are Tensors Exactly"



# Reference
1. [Tensor basic definition](https://rodolphe-vaillant.fr/entry/139/tensor-basic-definition)
2. Book: [An Introduction to Tensor Calculus](https://grinfeld.org/books/An-Introduction-To-Tensor-Calculus/)
3. [Dual spaces, dual vectors and dual basis](https://ekamperi.github.io/mathematics/2019/11/17/dual-spaces-and-dual-vectors.html)
4. [Tensor](https://mathworld.wolfram.com/Tensor.html)
5. video: [Vector Calculus: Lecture 25/29 - Multilinear Maps, The Tensor Quotient Rule](https://www.youtube.com/watch?v=OuuvkdUGPtk)
6. video: [Vector Calculus Lectures](https://www.youtube.com/playlist?list=PLC0PGB2LK3Rhijc9H3Ijx2dGrAYB0F-lk)
7. [Multilinear Mappings and Tensors](https://cseweb.ucsd.edu/~gill/CILASite/Resources/15Chap11.pdf) [To Read]
8. [CHAPTER 1 MULTILINEAR ALGEBRA](https://math.mit.edu/classes/18.952/2015SP/docs/chapter1.pdf) [To Read]
9. video: [What is a Tensor? An Animated Introduction!](https://www.youtube.com/watch?v=W4oQ8LisNn4&t=430)
10. video: [Understand Tensors Like a Physicist! (The Easy Way)](https://www.youtube.com/watch?v=czrel_yqJYM)
11. [Covariant and Contravariant Tensors](https://rinterested.github.io/statistics/tensors2.html)
12. video: [Tensor Calculus](https://www.youtube.com/playlist?list=PLXPyU0M9IEAbIYz6O5v3IynmnNlY-uraS)



