# Norms

## Why norms? 

Norms are fundamental in linear algebra to quantify the "size" or "length" of vectors, <br>
which is used to **measure distances between vectors**, **determine the error in predictions**, <br>
**define convergence of sequences**, and **separate a vector's magnitude from its direction**. <br>
They are essential for applications like *machine learning*, *numerical analysis*, and *physics*, <br>
where we often need to measure how "far apart" two vectors are or how well a model approximates <br>
a solution. <sup>Google AI Overview</sup>

### Key uses of norms <sup>Google AI Overview</sup>

* **Measuring distance**: Norms define a distance metric between vectors, allowing us to quantify <br>
  how "close" two vectors are to each other. For example, the difference between a vector <br>
  and its projection can be evaluated using its norm.
* **Quantifying error**: In machine learning, a norm is used to **measure the error** between a model's <br>
  prediction (a vector) and the actual value (another vector). The goal of training is often <br>
  to minimize this error.
* **Defining convergence**: Norms are used to define the convergence of a sequence of vectors. <br>
  If the norm of the difference between vectors in a sequence gets smaller and smaller, <br>
  the sequence is said to converge.
* **Simplifying operations**: A norm provides a way to get a **single scalar value** (the magnitude) <br>
  from a vector, separating it from its direction. This simplifies many calculations, such as <br>
  when using the method of **least squares**.
* **Providing different perspectives**: Different norms provide different ways of measuring length. <br>
  For example, the **L1** or **"Manhattan"** norm sums the absolute values of the vector's components, <br>
  while the **L2** or **"Euclidean"** norm is the standard "straight-line" distance. <br>
  The choice of norm can be crucial depending on the problem (e.g., a "taxi cab" metric in <br>
  city navigation vs. a direct distance). 

## Vector Norms

TODO: [8]

## Matrix Norms

### Frobenius norm

Definition 4.6. <sup>[1]</sup> The Frobenius norm $`\Vert \Vert_{F}`$ is defined so <br>
that for every **square** $`n × n`$ matrix $`A \in M_{n}(\mathbb{C})`$

$`\Vert A \Vert_{F} = (\sum_{i,j=1}^{n}|a_{ij}|^2)^{\frac{1}{2}} = \sqrt{tr(AA^*)} = \sqrt{tr(A^*A)}`$

**NOTE**: $`A^*`$ is the [conjugate transpose](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Concepts.md#conjugate-transpose-matrix) of $`A`$.







## Reference
1. [Chapter 4: Vector Norms and Matrix Norms](https://www.cis.upenn.edu/~cis5150/cis515-11-sl4.pdf)
2. Video: [Linear Algebra: Norm](https://www.youtube.com/watch?v=3i3klTnGZZM) [To Read]
3. Video: [Norms | Linear Algebra prerequisites](https://www.youtube.com/watch?v=_xfOIp55VD4&t=3) [To Read]
4. [Linear Algebra: Norm of a Vector, L1 and L2 Norm](https://medium.com/@praggrt/linear-algebra-norm-of-a-vector-l1-and-l2-norm-7cdf061b9888)
5. [Norms](https://www.cfm.brown.edu/people/dobrush/cs52/Mathematica/Part5/norm.html) from 	Brown University
6. [Machine Learning Basics - The Norms: Learn linear algebra through code and visualization.](https://www.datacamp.com/tutorial/tutorial-machine-learning-basics-norms) [To Read]
7. [Lecture 26: Norms and inner products.](https://people.tamu.edu/~yvorobets/MATH304-2011C/Lect3-04web.pdf)
8. [Norms in Linear Algebra](https://blog.langformers.com/norms-linear-algebra/)
