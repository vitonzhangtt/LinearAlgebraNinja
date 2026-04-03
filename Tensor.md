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

#### Example










### Covectors





## TODO

1. google "What Are Tensors Exactly"



# Reference
1. [Tensor basic definition](https://rodolphe-vaillant.fr/entry/139/tensor-basic-definition)
2. Book: [An Introduction to Tensor Calculus](https://grinfeld.org/books/An-Introduction-To-Tensor-Calculus/)
3. [Dual spaces, dual vectors and dual basis](https://ekamperi.github.io/mathematics/2019/11/17/dual-spaces-and-dual-vectors.html)



