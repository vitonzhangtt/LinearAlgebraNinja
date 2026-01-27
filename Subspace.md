# Subspace

## Definition of Subspace


### Definition from [1]
A subspace of a vector space $`V`$ is a subset $`U`$ of $`V`$ which

1. contains the zero vector $`0_{v}`$,
2. is closed under **addition**, meaning that for all $`v, w \in U`$ we have $`v + w \in U`$, and
3. is closed under **scalar multiplication**, meaning that for all scalars $`\lambda`$ <br>
 and all $`u \in U`$ we have $`\lambda u \in U`$.

We write $`U \leq V`$ to mean that $`U`$ is a subspace of $`V`$.

The idea this definition captures is that a subspace of $`V`$ is a nonempty subset which is <br>
itself a vector space under the same addition and scalar multiplication as $`V`$.

### Definition from [2]

Definition: A **subset** of $`R^{n}`$ is any collection of points of $`R^{n}`$.

For instance, the unit circle

$`C=\{(x,y) \text{ in } R^2 \vert x^2+y^2=1\}`$

is a subset of $`R^2`$.

A **subspace** of $`R^{n}`$ is a **subset** $`V`$ of $`R^{n}`$ satisfying:
* **Non-emptiness**: The zero vector is in $`V`$.
* **Closure under addition**: If $`u`$ and $`v`$ are in $`V`$, then $`u+v`$ is also in $`V`$.
* **Closure under scalar multiplication**: If $`v`$ is in $`V`$ and $`c`$ is in $`R`$, then $`cv`$ is also in $`V`$.


## Column Space <sup>[2]</sup>

Let $`A`$ be an $`m×n`$ matrix.

The **column space** of $`A`$ is the subspace of $`R^m`$ spanned by the columns of $`A`$. <br>
It is written **Col(A)**.

## Null Space <sup>[2]</sup>

Let $`A`$ be an $`m×n`$ matrix.

The **null space** of $`A`$ is the subspace of $`R^n`$ consisting of all solutions of the <br>
homogeneous equation $`Ax=0`$:

$`Nul(A)=\{x \text{ in } R^n | Ax=0 \}`$.


## Reference
1. [Subspaces](https://www.ucl.ac.uk/~ucahmto/0005_2021/Ch4.S4.html) [To Read]
2. [2.6 Subspaces](https://textbooks.math.gatech.edu/ila/subspaces.html) from `Interactive Linear Algebra`
