## 1.1 What is Linear Algebra (and why you need it)

**Linear algebra** is a _branch of mathematics focused on the study of vectors, matrices, and linear transformations._ **Vectors** are _quantities that have both magnitude and direction, and they are used to represent states or configurations in many physical systems._ **Matrices** are _rectangular arrays of numbers that can represent observables, operators, or changes in spacetime, depending on the context._

This subject forms the foundational language for many areas of modern physics, including quantum mechanics, relativity, string theory, and quantum field theory (QFT). In these fields, linear algebra provides the tools to describe and manipulate the mathematical objects that model physical phenomena. _For example, in quantum mechanics, vectors represent quantum states, while matrices (or more generally, operators) represent measurements and transformations of those states._ Understanding linear algebra is therefore essential for anyone studying advanced physics or related mathematical disciplines.

### In short:
* Linear algebra is the study of **vectors**, **matrices**, and **linear transformations**.
* It’s the language of **quantum mechanics**, **relativity**, **string theory**, and **QFT**.
* Vectors represent states, matrices represent observables, operators, or spacetime changes.

## 1.2 Vectors

### What is a vector?

* A **vector** is a _mathematical object that represents a quantity with both direction and magnitude._ In practice, a **vector** is _often written as a list of numbers, with each number corresponding to a component, along a particular axis._ For example, _a 3D vector can be written as a column of three numbers, each representing the vector’s projection along the x, y, and z axes._

- **On components**, a component refers to the _value of a vector along a specific axis or direction._ For example, in three-dimensional space, **a vector has three components**: _one for the x-axis, one for the y-axis, and one for the z-axis._ Each component tells you how much the vector points in that particular direction. So, the components are simply the individual numbers in the list that make up the vector.

- **Vectors** can be manipulated using several basic operations. 

- **Addition** is **performed component-wise**, meaning you _add corresponding components from each vector to get a new vector._ For example, you add the x-component of one vector to the x-component of another, and so on. To avoid any confusion, you can only add corresponding components (numbers) from two vectors of the same dimension. You cannot add extra dimensions, functionals, or other types of mathematical objects - just the matching numbers from each vector. The result is always another vector of the same dimension.

![](https://quicklatex.com/cache3/c0/ql_2ca4fbbdcdee16595f4d1cb29b89dac0_l3.png)

- **Scalar multiplication** involves _taking a vector and multiplying every component (number) in that vector by the same single number, called a scalar._ This operation _changes the length (magnitude)_ of the vector but _keeps its direction the same - unless the scalar is negative, in which case the vector points in the opposite direction._ For example, multiplying a vector by 2 doubles its length, while multiplying by -1 flips its direction. If the original vector pointed right, multiplying by -1 makes it point left. If it pointed up, it now points down, and so on.g

![](https://quicklatex.com/cache3/6b/ql_473f99423a9552588f01a4d81c35746b_l3.png)

In scalar multiplication, (c) is the scalar (a single number), and (\vec{a}) is the vector. When you multiply a vector by a scalar, you multiply each component of the vector by that scalar. So, (c a_1) means you multiply the first component (a_1) by (c), (c a_2) means you multiply the second component (a_2) by (c), and so on.

For example, if ![](https://quicklatex.com/cache3/57/ql_96f8267b905d56cd1efc2003efee6e57_l3.png) and (c = 4):

![](https://quicklatex.com/cache3/a2/ql_0ba8cdeb333a079b2b94101e758b63a2_l3.png)

So, (c a_1) just means "multiply the scalar (c) by the component (a_1)."

- **dot product** _takes two vectors and produces a single number (a scalar). This scalar tells you how much the two vectors point in the same direction._ _If the vectors are pointing in exactly the same direction, the dot product is large and positive; if they are perpendicular, the dot product is zero; if they point in opposite directions, the dot product is negative._

The result of a dot product is called a scalar because it is just a regular number, not a vector. However, the process is different from scalar multiplication:

- Scalar multiplication means multiplying a vector by a number, resulting in another vector. 
- A single number (scalar) is produced by the dot product by multiplying the corresponding components of two vectors and then adding up all those products.
For example, if you have two 3D vectors:

![](https://quicklatex.com/cache3/9e/ql_3495498474ca4607fbc6db0c069c3a9e_l3.png), ![](https://quicklatex.com/cache3/04/ql_d43510977afdaf7f434ab5621885a704_l3.png)

The dot product is:

![](https://quicklatex.com/cache3/fd/ql_11b885a7639530d0b0f3953a74552cfd_l3.png)

This sum is a single number (not a vector). The same process works for any dimension: multiply matching components, then add them all together.

- Dot product means combining two vectors to get a single number (scalar).
- So, while the result of a dot product is a scalar, the operation itself is fundamentally about comparing two vectors, not just multiplying by a number.

**Note that:** When you take the dot product of two vectors, you combine them to produce a single number (a scalar). The original vectors themselves do not change - they remain the same. The dot product just tells you how much the two vectors point in the same direction, but it does not alter the vectors themselves.


Finally, 

- the **norm (or magnitude)** of a vector is _a way to measure how long the vector is._ For a vector written as a list of numbers (components), you calculate the norm by squaring each component, adding them all together, and then taking the square root of that sum.

For example, for a 3D vector 

![](https://quicklatex.com/cache3/ba/ql_fe70a2197191a0aa057944acd193c9ba_l3.png), 

the norm is:

![](https://quicklatex.com/cache3/0c/ql_90159b2fad32bb96f01a2964eefcbc0c_l3.png)


This gives you a single number that tells you the "length" of the vector, just like the length of an arrow in space. This concept is fundamental in physics and mathematics for describing distances, speeds, and many other quantities.

## 1.3 Matrices

### What is a matrix?

* A matrix is a rectangular array of numbers.
* Think of it as a transformation tool for vectors, because they can act on vectors - meaning they can transform vectors by changing their direction, length, or both.
* For example a 2×2 matrix has 2 rows and 2 columns and looks like this::

  * <img src="https://quicklatex.com/cache3/f1/ql_f54a65eeb9e330b1b691b19d29a55ff1_l3.png">

### Matrix operations:

* ### Addition: 
Matrix addition is a basic operation where you combine two matrices by adding their corresponding elements. For this to work, both matrices must have the same dimensions - that is, the same number of rows and columns. You cannot add matrices of different sizes because there would be elements in one matrix that do not have a counterpart in the other.

To perform matrix addition, simply add each entry in the first matrix to the entry in the same position in the second matrix. For example, the element in the first row and first column of the result is the sum of the elements in the first row and first column of each matrix. This process is repeated for every position in the matrices.

The result is a new matrix of the same size, where each entry is the sum of the corresponding entries from the original matrices. This operation is always performed entry-by-entry, and is only defined when the matrices have matching dimensions.

Example:

![](https://quicklatex.com/cache3/03/ql_5cd0d7dc14b16150f70f1df72cc48b03_l3.png)   

and

 ![](https://quicklatex.com/cache3/61/ql_3e52ac679a0d27517b99c94e63efe361_l3.png)  

To add     

![](https://quicklatex.com/cache3/4b/ql_ecbab37cfe73c3f7ac215ef9945f324b_l3.png)

Explanation:

- The $(1,1)$ entry is $1+5=6$

- The $(1,2)$ entry is $2+6=8$

- The $(2,1)$ entry is $3+7=10$

- The $(2,2)$ entry is $4+8=12$

Matrix addition is always done entry-by-entry, and only works if both matrices have the same number of rows and columns.


* ### Scalar multiplication: Multiply each element by a number.

* A **scalar** is just a regular number — like 2, 3, or -1.  
* Scalar multiplication means **you multiply every number** inside the matrix by that same scalar. This process changes the scale of the matrix, making every value larger, smaller, or flipping its sign if the scalar is negative. 
  It’s like applying the same filter to every value.
  
  Let’s say we have a matrix:

![](https://quicklatex.com/cache3/03/ql_5cd0d7dc14b16150f70f1df72cc48b03_l3.png)

and a scalar:

![](https://quicklatex.com/cache3/45/ql_d6125dca23d24a09a5141fd27fc3f445_l3.png)

To do scalar multiplication, multiply **every entry** in the matrix by the scalar:

![](https://quicklatex.com/cache3/d3/ql_9cd9be15813890e4d1babd5d35c231d3_l3.png)

This means:

- The (1,1) entry: **3 × 1 = 3**
- The (1,2) entry: **3 × 2 = 6**
- The (2,1) entry: **3 × 3 = 9**
- The (2,2) entry: **3 × 4 = 12**

So the new matrix becomes:

![](https://quicklatex.com/cache3/9a/ql_c327f2dd1e6531738e033a7169f8129a_l3.png)

---

### What does this mean?

When you multiply a matrix by a scalar, you are scaling every entry in the matrix by that number. This means that the matrix’s effect - such as stretching or shrinking vectors - also gets scaled. If the scalar is positive, all the values in the matrix grow or shrink but keep their original direction. If the scalar is negative, not only do the values change in size, but their direction is also reversed (flipped).

### Matrix-vector multiplication:
is an operation where a _matrix acts on a vector to produce a new vector._ This is a fundamental way that matrices transform vectors, changing their direction, length, or both.

Suppose you have a matrix (A) and a vector (\vec{x}):

![](https://quicklatex.com/cache3/f6/ql_5eb4cf2f52e0a5d1df4b603e8799b2f6_l3.png)

The matrix-vector multiplication (A\vec{x}) is calculated as:

![](https://quicklatex.com/cache3/b2/ql_03a4f763d73d8f954c0cfb88f6c753b2_l3.png)

Explanation:

Each entry in the resulting vector is a sum of products: you multiply each entry in a row of the matrix by the corresponding entry in the vector, then add them up. The result is a new vector, which is generally in a different direction and may have a different length than the original vector.

So, matrix-vector multiplication transforms the vector according to the rules encoded in the matrix.

### Matrix-matrix Multiplication (row x column)
**Matrix-matrix multiplication** is _an operation where you multiply two matrices to produce a new matrix. This is only possible when the number of columns in the first matrix matches the number of rows in the second matrix._

_For each entry in the resulting matrix, you take the dot product of a row from the first matrix and a column from the second matrix._ This means you multiply corresponding elements and add them up.

---

Suppose:

![](https://quicklatex.com/cache3/76/ql_76656ff4ff57bce54fd54f75bd1e2876_l3.png) ![](https://quicklatex.com/cache3/bc/ql_8750494045fe32cf17a1e8d76fd5fbbc_l3.png)

Then the product ( AB ) is:

![](https://quicklatex.com/cache3/38/ql_5e33097aca9fcf6560c309f7e9f52c38_l3.png)

---

Explanation:

Each entry in the new matrix is found by multiplying the elements of a row from the first matrix by the corresponding elements of a column from the second matrix, then adding the results.
For example, the entry in the first row and first column is ![](https://quicklatex.com/cache3/f1/ql_9e11162461279d5e7ef9dd96805dfdf1_l3.png).
Example with numbers:

![](https://quicklatex.com/cache3/4f/ql_4318236c2dac0c470bcc109ae44b3b4f_l3.png)

![](https://quicklatex.com/cache3/74/ql_9429d57c7982065b519987465f268874_l3.png)

So, matrix-matrix multiplication combines the transformations of both matrices into a single new matrix.

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
