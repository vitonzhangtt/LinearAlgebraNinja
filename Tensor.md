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

## Definition

Tensors are used in many fields, such as, Neural Networks, Continuum Mechanics or even General Relativity; <br>
and while tensors are a quite general concept, depending on which field you apply them, you may come across <br>
very different definitions. This is often the cause of a great deal of confusion. <sup>[1]</sup>

### Strict mathematical definition <sup>[1]</sup>

A type $`(p,q)`$ tensor $`T`$ is defined as a **multi-linear map**

<img width="397" height="69" alt="" src="https://github.com/user-attachments/assets/416c44d1-bc39-44ae-bc7d-6e11dc14adb0" />

Where V is a **vector space** (also called **linear space**) over a **field** F, and $`V^*`$ is its corresponding <br>
**dual space**. (Note that while $`F`$ is oftentimes the set of real numbers $`R`$, it could well be the rationals <br>
$`Q`$ or complex numbers $`C`$)

The literal way of saying the above is:
Tensor is a collection of **vectors** and **covectors** combined together using the tensor product.



### Multilinear Map (多重线性映射)


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



