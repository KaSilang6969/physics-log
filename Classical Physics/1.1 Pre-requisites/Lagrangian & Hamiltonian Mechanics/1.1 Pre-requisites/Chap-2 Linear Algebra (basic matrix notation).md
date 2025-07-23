## 1.1 What is Linear Algebra (and why you need it)

* Linear algebra is the study of **vectors**, **matrices**, and **linear transformations**.
* It’s the language of **quantum mechanics**, **relativity**, **string theory**, and **QFT**.
* Vectors represent states, matrices represent observables, operators, or spacetime changes.

## 1.2 Vectors

### What is a vector?

* A vector is a list of numbers that represents a quantity with direction and magnitude.
* You can write a 3D vector like:

  * ![](https://quicklatex.com/cache3/86/ql_827de02c6f1fc9d6a49692bcee2d7686_l3.png)
  * This is a column vector.

### Vector operations:

* **Addition** (component-wise):

  * ![](https://quicklatex.com/cache3/76/ql_0ba33e6534a58f4b1abd8f72efb7f276_l3.png)
* **Scalar multiplication**:

  * ![](https://quicklatex.com/cache3/ef/ql_f25ff6a0b2a898909df2e3150452d8ef_l3.png)
* **Dot product** (produces a number):

  * ![](https://quicklatex.com/cache3/9b/ql_b579fab278048794e941aec8e6c7b39b_l3.png)
* **Norm (magnitude)**:

  * ![](https://quicklatex.com/cache3/2f/ql_c42a9ccbf23162891bb25514294c542f_l3.png)

## 1.3 Matrices

### What is a matrix?

* A matrix is a rectangular array of numbers.
* Think of it as a transformation tool for vectors.
* Example 2×2 matrix:

  * ![](https://quicklatex.com/cache3/f1/ql_f54a65eeb9e330b1b691b19d29a55ff1_l3.png)

### Matrix operations:

* **Addition**: Add component-wise (same size only).
* **Scalar multiplication**: Multiply each element by a number.
* **Matrix-vector multiplication**:

  * ![](https://quicklatex.com/cache3/bd/ql_1745f229171977e6b6773fab622cc1bd_l3.png)

1.4 Special Matrices and 
* **Matrix-matrix multiplication** (row × column):

  * ![](https://quicklatex.com/cache3/f1/ql_f54a65eeb9e330b1b691b19d29a55ff1_l3.png)

## 1.4 Special Matrices and Types

* **Identity matrix (I)**:

  * Leaves a vector unchanged: 
* **Zero matrix**: all entries are 0
* **Diagonal matrix**: only diagonal entries are non-zero
* **Symmetric**: ![](https://quicklatex.com/latex3.f/ql_56aa47b74a9d8f1c11932c50c8ce49e6_l3.png)
* **Orthogonal**: ![](https://quicklatex.com/cache3/10/ql_90cc55392ca1b5c9c4b4450c793bec10_l3.png)
* **Hermitian**: ![](https://quicklatex.com/cache3/31/ql_a002f92824e04d66c76dface905a2831_l3.png)
* **Unitary**: ![](https://quicklatex.com/cache3/33/ql_8ca961d77346267f5862c0616af8ae33_l3.png)

## 1.5 Transpose, Conjugate, Adjoint

* **Transpose (A^T)**: Flip rows and columns
* **Conjugate (A^\*)**: Replace each entry with its complex conjugate
* **Adjoint (A^\dagger)**: Take the conjugate transpose

## 1.6 Determinant and Inverse

* **Determinant**: Scalar that tells if matrix is invertible

  * 2x2 case: ![](https://quicklatex.com/cache3/3f/ql_be8bade7dd41981e91877ab0574f813f_l3.png)
* **Inverse (A^{-1})**: matrix that undoes transformation

  * Only exists if ![](\det(A) \neq 0)
  * ![](https://quicklatex.com/cache3/97/ql_8966a6474c24b399aa61dd0c69a17497_l3.png)
## 1.7 Eigenvalues and Eigenvectors

* **Eigenvector**: a direction that stays unchanged under transformation (just gets scaled)
* **Eigenvalue**: the scale factor
* Formula:

  * ![](https://quicklatex.com/cache3/9d/ql_e21fa5f8c6afb722072256325d2ab19d_l3.png)

* To find them, solve:

  * ![](https://quicklatex.com/cache3/bd/ql_157bd5179fbb3baffada0e6526e477bd_l3.png)

## 1.8 Basis and Change of Basis

* A **basis** is a set of vectors that can build any vector in the space.
* **Standard basis**: x̂, ŷ, ẑ
* You can switch between bases using a **change of basis matrix**.

## 1.9 Vector Spaces and Subspaces

* A **vector space** is any set where vector addition and scalar multiplication work.
* A **subspace** is a smaller space inside that also follows the rules.
* Important in quantum, where states live in **Hilbert spaces** (infinite-dimensional vector spaces).

## 1.10 Linear Independence and Span

* **Span**: all combinations of some vectors
* **Linearly independent**: no vector in the set can be built from the others
* These ideas define dimensionality

## 1.11 Projection and Orthogonality

* **Projection**: dropping a vector onto another
* **Orthogonal**: dot product is zero
* Useful for breaking motion into components, decomposing quantum states

## 1.12 Inner Products

* Generalization of dot product
* Denoted: ![](https://quicklatex.com/cache3/6e/ql_f8e63b5920d0a086056c93d96adbba6e_l3.png)
* Used to define lengths and angles in abstract spaces
* In quantum, it's how you compute probabilities

## 1.13 Dirac Notation (Bra-Ket)

* Compact notation to represent quantum states

* A ket is a state vector: 

* A bra is its conjugate transpose: 

* Inner product between two states: 

* Outer product (builds operators): 

* Expectation value: 

## 1.14 Tensor Algebra (Intro Only)

* Tensors are generalizations of scalars, vectors, and matrices

* They describe relationships between vectors and coordinate systems

* Einstein summation convention: repeated indices imply summation

* A tensor equation:

![](https://quicklatex.com/cache3/8b/ql_048859ffead5c7e89714214e7aec4b8b_l3.png)

* Used in relativity to describe curvature, gravity, and transformations

## 1.15 Hilbert Space Formalism

* A Hilbert space is a complete inner product space

* States are vectors: ![](https://quicklatex.com/cache3/de/ql_63fa88b81aacf2b8032bd2fa88f20dde_l3.png)

* Observables are Hermitian operators: ![](https://quicklatex.com/cache3/61/ql_bc9227850827e04d886296ee890e7961_l3.png)

* Measurement results are eigenvalues of operators

* Time evolution (Schrödinger eq.):

* ![](https://quicklatex.com/cache3/09/ql_fc3c03b4b39cfeeb384d00b2d122f709_l3.png)

* Key in quantum mechanics, QFT, and quantum computing
