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

## Matrix Multiplication (Row × Column)

### Given Matrices

Let:

![](https://quicklatex.com/cache3/6f/ql_4cc99f0ddaf00a4efb82ce871a0f5c6f_l3.png)

We want to compute:

![](https://quicklatex.com/cache3/60/ql_72d7b59f70ab4854e2f74621aa50d460_l3.png)

---

### How Matrix Multiplication Works

To compute each entry of ![](https://quicklatex.com/cache3/4f/ql_48b09a8b3db3326b126db38d6e6a1d4f_l3.png):

- Pick a **row** from matrix ![](https://quicklatex.com/cache3/82/ql_d6096c6b9d4cc326ee6ec961ed3e9082_l3.png)

- Pick a **column** from matrix ![](https://quicklatex.com/cache3/d2/ql_03abf73052575a8c077cb6c61b98c7d2_l3.png)
- Multiply corresponding entries and sum the results

---

###  Step-by-Step

#### 🔹 Entry (1, 1): Top-left

Row 1 of ![](https://quicklatex.com/cache3/82/ql_d6096c6b9d4cc326ee6ec961ed3e9082_l3.png): ![](https://quicklatex.com/cache3/e2/ql_8a6e3470c687f03d77e912b45141a1e2_l3.png)
Column 1 of ![](https://quicklatex.com/cache3/d2/ql_03abf73052575a8c077cb6c61b98c7d2_l3.png): ![](https://quicklatex.com/cache3/c2/ql_2d71af5a690712482f57dd9ae96c73c2_l3.png)

![](https://quicklatex.com/cache3/e6/ql_f10cca21d34da91cd744a417c3a7bbe6_l3.png)

---

#### 🔹 Entry (1, 2): Top-right

Row 1 of ![](https://quicklatex.com/cache3/af/ql_b56151d53e5350969502b4ed9051a3af_l3.png)
Column 2 of ![](https://quicklatex.com/cache3/23/ql_0144bd0709e1233b403348301e17d923_l3.png)

![](https://quicklatex.com/cache3/79/ql_5b0472a3c8b5e993492e0f79f02bdf79_l3.png)

---

#### 🔹 Entry (2, 1): Bottom-left

Row 2 of ![](https://quicklatex.com/cache3/36/ql_0043ff2dd9aa1ec2a521e0f4412ef236_l3.png)
Column 1 of ![](https://quicklatex.com/cache3/c7/ql_d062d4d6a961951e86a403bd8bf820c7_l3.png)

![](https://quicklatex.com/cache3/60/ql_3ae0833122766d2ca96e20ba11b41860_l3.png)

---

#### 🔹 Entry (2, 2): Bottom-right

Row 2 of ![](https://quicklatex.com/cache3/36/ql_0043ff2dd9aa1ec2a521e0f4412ef236_l3.png)
Column 2 of ![](https://quicklatex.com/cache3/23/ql_0144bd0709e1233b403348301e17d923_l3.png)

![](https://quicklatex.com/cache3/10/ql_69a80030ba328c5313c905c3915b7010_l3.png)

---

### Final Result:

![](https://quicklatex.com/cache3/bd/ql_1c08b9c944d04b3bd8b0ae278eb9ebbd_l3.png)

---

### Visualization Tip

Think of matrix multiplication like **sliding a row across a column**:

> Like scanning a barcode: one row (the scanner) slides over a column (the tag), combining values to produce one number.

Each entry is the **sum of pairwise products** of corresponding elements.

---

### Summary

| Step              | Action                                       |
|-------------------|----------------------------------------------|
| Pick row from A   | Left matrix (rows)                          |
| Pick column from B| Right matrix (columns)                      |
| Multiply + add    | Match 1st × 1st, 2nd × 2nd, then sum         |
| Repeat for all entries | Until the full product matrix is filled |



## 1.4 Special Matrices and Types

* **Identity matrix (I)**:

The identity matrix is a special square matrix with 1s on the diagonal and 0s everywhere else. When you multiply any vector or matrix by the identity matrix, it remains unchanged - just like multiplying a number by 1.

Example with a vector:

![](https://quicklatex.com/cache3/06/ql_b1ca51d7f06795b799d33d0f4c5dd306_l3.png)

Example with a matrix:

![](https://quicklatex.com/cache3/82/ql_61756f29146b6114242d1605210f5382_l3.png)

The identity matrix leaves any compatible vector or matrix unchanged when multiplied:

* **Zero matrix**:

The zero matrix is a special matrix where every entry is 0. It acts like the number 0 in matrix addition: when you add the zero matrix to any other matrix of the same size, the result is just the original matrix. The zero matrix is used to represent the absence of any effect or transformation.

Example (2×2 zero matrix):

![](https://quicklatex.com/cache3/b2/ql_e64edb68ba6b546d739116900e2e27b2_l3.png)

For any matrix (A) of the same size:

[ A + 0 = A ]

The zero matrix leaves other matrices unchanged when added.

* **Diagonal matrix**:

A diagonal matrix is a special type of square matrix where all the entries outside the main diagonal are zero. Only the diagonal entries (from top left to bottom right) can be non-zero. Diagonal matrices are important because they are easy to work with and often represent scaling transformations.

Example (2×2 diagonal matrix):

![](https://quicklatex.com/cache3/fb/ql_efcb915fb2007aca421a5d01db3b48fb_l3.png)

For a 3×3 diagonal matrix:

![](https://quicklatex.com/cache3/df/ql_70cf50088195c3b45d4cc70ceafb2cdf_l3.png)

When you multiply a vector by a diagonal matrix, each component of the vector is scaled by the corresponding diagonal entry.

### 🔸 Multiplying a Diagonal Matrix by a Vector

Let’s say:

![](https://quicklatex.com/cache3/d7/ql_1786cf5d7b76f534ee295170327bb8d7_l3.png)

Then:

![](https://quicklatex.com/cache3/4c/ql_2a6f32564716fd7f8a854d4cbefd8d4c_l3.png)

Yes, we still "use" the 0s in multiplication — they just wipe out everything off-diagonal.


* **Symmetric**:

A symmetric matrix is a square matrix that is equal to its transpose. This means the entries are mirrored across the main diagonal: the element in row (i), column (j) is the same as the element in row (j), column (i).

Mathematically:
![](https://quicklatex.com/cache3/da/ql_6abe67e801a21646d1157efcf7dbe5da_l3.png)

![](https://quicklatex.com/cache3/75/ql_dd891a84dcecfde252b8aa16c2343e75_l3.png)

Here, the off-diagonal elements are equal ((b)), so the matrix is symmetric. Symmetric matrices are important in physics and mathematics because they often represent real, observable quantities and have useful properties, such as real eigenvalues.


* **Orthogonal**:

An orthogonal matrix is a square matrix whose rows and columns are all orthonormal vectors. This means that the matrix multiplied by its transpose gives the identity matrix:

![](https://quicklatex.com/cache3/41/ql_ad92960e6c2575ee1582c564e3199341_l3.png)

Example (2×2 orthogonal matrix):

![](https://quicklatex.com/cache3/ee/ql_8ec69d79c5cd82d5a81cf03e01043cee_l3.png)

Orthogonal matrices represent rotations and reflections. They preserve the length and angles of vectors when applied as transformations, which is why they are important in physics and geometry.

* **Hermitian**: 

A Hermitian matrix is a square matrix that is equal to its own conjugate transpose. This means that each entry is the complex conjugate of its mirror image across the main diagonal. Hermitian matrices are important in quantum mechanics because they always have real eigenvalues and represent observable quantities.

Mathematically:

![](https://quicklatex.com/cache3/ba/ql_e8a9f04d642e61152921c357868795ba_l3.png)

is the conjugate transpose of (A).

Example (2×2 Hermitian matrix):

![](https://quicklatex.com/cache3/67/ql_a9841046acf60bcf63794b3873e5b567_l3.png)

 where (a, c) are real and (b) is complex.


* **Unitary**:

A unitary matrix is a square matrix whose conjugate transpose is also its inverse. This means that multiplying a unitary matrix by its conjugate transpose gives the identity matrix. Unitary matrices preserve the length of vectors and are fundamental in quantum mechanics for describing time evolution and symmetry operations.

Mathematically:
![](https://quicklatex.com/cache3/ea/ql_260aa34fbdf7ded376bb90afc5449aea_l3.png)

is the conjugate transpose of (U).

Example (2×2 unitary matrix): 

![](https://quicklatex.com/cache3/4b/ql_33c68598f94c376543df524613f3714b_l3.png)

Unitary matrices preserve inner products and probabilities in quantum systems.

---

## 1.5 Transpose, Conjugate, Adjoint

* **Transpose (A^T)**:

The transpose of a matrix is formed by flipping its rows and columns. The element in row (i), column (j) of the original matrix becomes the element in row (j), column (i) of the transposed matrix.

Example: 

![](https://quicklatex.com/cache3/8d/ql_e55c0659ee8bdee0104dea70defffc8d_l3.png)

---

**Conjugate!**[](https://quicklatex.com/cache3/50/ql_c3fe9ffc036b61486e9791b4fdc38250_l3.png)): 

The conjugate of a matrix replaces each entry with its complex conjugate. For a real matrix, this does nothing; for a complex matrix, it flips the sign of the imaginary part.

Example:

![](https://quicklatex.com/cache3/a0/ql_34c86b88e13361578f17dcb182076da0_l3.png)

---

**Adjoint** ![](https://quicklatex.com/cache3/86/ql_d5dd44e9fd39a748622d6c433b388e86_l3.png):

The adjoint (or Hermitian conjugate) of a matrix is the conjugate transpose: take the transpose, then take the complex conjugate of each entry.

Example: 

![](https://quicklatex.com/cache3/89/ql_2796b7ff1a928a600e659de35e988089_l3.png)

---

## 1.6 Determinant and Inverse

The determinant of a matrix is a scalar value that tells you important information about the matrix, such as whether it is invertible (can be "undone"). If the determinant is zero, the matrix is not invertible.

For a 2×2 matrix:

![](https://quicklatex.com/cache3/82/ql_65e46586fb212b28080a7aff12339682_l3.png)

The determinant is:

![](https://quicklatex.com/cache3/83/ql_95bd4820f9666c70517f1b78369a0e83_l3.png)

Inverse ![](https://quicklatex.com/cache3/5b/ql_19e45445a41540b9cdc8a62c9de6eb5b_l3.png)
The inverse of a matrix is another matrix that "undoes" the effect of the original matrix. Only matrices with a nonzero determinant have an inverse.

For a 2×2 matrix:

![](https://quicklatex.com/cache3/df/ql_a8ee27daecccce7671879e2f4e06c2df_l3.png)

Condition for invertibility:

![](https://quicklatex.com/cache3/be/ql_abc886bb8b76749d7e9a3dc382742ebe_l3.png)

Property:

![](https://quicklatex.com/cache3/87/ql_57431231a2c6ca49e0615973ce1c6287_l3.png)

where (I) is the identity matrix.

**Summary:**

- The determinant tells you if a matrix is invertible.
- The inverse matrix undoes the transformation of the original matrix.
- Only matrices with a nonzero determinant have an inverse.


## 1.7 Eigenvalues and Eigenvectors

- **Eigenvector:**
A direction that stays unchanged under a transformation (it only gets scaled).
- **Eigenvalue:**
The scale factor by which the eigenvector is stretched or shrunk.

## Eigenvalue

Formula: 

![](https://quicklatex.com/cache3/ee/ql_3cf8ae0cfac8b58f2205ef944cd641ee_l3.png)

- ![](https://quicklatex.com/cache3/82/ql_d6096c6b9d4cc326ee6ec961ed3e9082_l3.png): square matrix

- ![](https://quicklatex.com/cache3/bd/ql_5334e94e9e2b14e22fd604747d3498bd_l3.png): eigenvector (nonzero)

- ![](https://quicklatex.com/cache3/06/ql_0c2a4f5762d2437115c037c069d9d506_l3.png): eigenvalue (scalar)

---

##  Characteristic Equation

![](https://quicklatex.com/cache3/43/ql_a194379995babe0d971a2022a1baf943_l3.png)

To find eigenvalues:
1. Subtract ![](https://quicklatex.com/cache3/b1/ql_38dafcbb2bc40bb1a9c640d19a8e22b1_l3.png)
2. Take the determinant
3. Set it equal to zero and solve for ![](https://quicklatex.com/cache3/06/ql_0c2a4f5762d2437115c037c069d9d506_l3.png)

---

## Summary

- **Eigenvectors** point in directions that remain unchanged (only scaled) under the transformation ![](https://quicklatex.com/cache3/82/ql_d6096c6b9d4cc326ee6ec961ed3e9082_l3.png)
- **Eigenvalues** tell how much those vectors are stretched or shrunk
- To find them:
  1. Solve ![](https://quicklatex.com/cache3/25/ql_f98854549e27baa9366d0c95f4838a25_l3.png)
  2. For each ![](https://quicklatex.com/cache3/06/ql_0c2a4f5762d2437115c037c069d9d506_l3.png), find the corresponding ![](https://quicklatex.com/cache3/bd/ql_5334e94e9e2b14e22fd604747d3498bd_l3.png) such that ![](https://quicklatex.com/cache3/b7/ql_a7e60883d5048b9027168b80d31005b7_l3.png)

---

## Example (2×2 Matrix)

Given:

![](https://quicklatex.com/cache3/c2/ql_bf5f8b19998ff50cec181926ec31c2c2_l3.png)

Find eigenvalues by solving:

![](https://quicklatex.com/cache3/8f/ql_503fca5d14ca7acdc058d215a34f4a8f_l3.png)

![](https://quicklatex.com/cache3/fd/ql_3833163ec67a7172b3763428cc8638fd_l3.png)

Compute:

![](https://quicklatex.com/cache3/1e/ql_8f38ef63f32040be4ea6fd87c4cb1d1e_l3.png)

---

## Find Eigenvectors

For each eigenvalue ![](https://quicklatex.com/cache3/06/ql_0c2a4f5762d2437115c037c069d9d506_l3.png), solve:

![](https://quicklatex.com/cache3/b5/ql_4b0217a591e1a1eb5dc792f324eb1cb5_l3.png)

For example, for ![](https://quicklatex.com/cache3/be/ql_fbaf438331f6728a437003dc53674bbe_l3.png):

![](https://quicklatex.com/cache3/5c/ql_a8e853a3a90472cf47b276fb6715475c_l3.png)

Solution: ![](https://quicklatex.com/cache3/c6/ql_6f3a39b989f3fed06e1a4320af2ef5c6_l3.png)

Similarly for ![](https://quicklatex.com/cache3/16/ql_0f407fd359a9d6cbfe8e057e2da82816_l3.png):

![](https://quicklatex.com/cache3/ce/ql_9bc69f41e2320bd83151bae46768edce_l3.png)

---

## Final Answer

- Eigenvalues:

![](https://quicklatex.com/cache3/1a/ql_7dd87a9950362907376e1cf380df271a_l3.png)

- Corresponding eigenvectors:
  - ![](https://quicklatex.com/cache3/66/ql_3d403188452db091cbda6a42a4a23f66_l3.png)


  - ![](https://quicklatex.com/cache3/e4/ql_6da2a8699ddcbecc3059a3cda63388e4_l3.png)

---

## Use Cases

- Diagonalization
- Quantum mechanics
- Principal component analysis
- Differential equations

---

## 1.8 Basis and Change of Basis

### What Is a Basis?

A **basis** is a set of linearly independent vectors that can represent any vector in the space via linear combination.

- In ![](https://quicklatex.com/cache3/4d/ql_5707d877d3febd69dea9370cb8d0d04d_l3.png): a basis could be two non-parallel vectors  
- In ![](https://quicklatex.com/cache3/23/ql_dd8881b7831826c92d367f4ebd8be823_l3.png): the standard basis is:

![](https://quicklatex.com/cache3/02/ql_d6be7470d178d6af03bda013df15d302_l3.png)

Any vector ![](https://quicklatex.com/cache3/81/ql_eec433c672dffcdc37dca3c55a1b0081_l3.png) can be written as:

![](https://quicklatex.com/cache3/58/ql_e88a084c63f69c30dbdc8a923ccb5558_l3.png)

---

### Change of Basis

You can switch between two bases using a **change of basis matrix**.

Let:
- ![](https://quicklatex.com/cache3/36/ql_094f2f9e9e02f84d41e06e081f312836_l3.png) be the new basis
- ![](https://quicklatex.com/cache3/3b/ql_d181386fd2fe7ff03a3a7d56a5d1c13b_l3.png) be the **change of basis matrix** with columns = new basis vectors

Then:
![](https://quicklatex.com/cache3/ef/ql_5e617dc0930ba4f8df0484de7d1157ef_l3.png)

Where:
- ![](https://quicklatex.com/cache3/de/ql_fd8e6fd2cbed7ce17080ab801b66a8de_l3.png): coordinates of ![](https://quicklatex.com/cache3/bd/ql_5334e94e9e2b14e22fd604747d3498bd_l3.png) in the new basis
- ![](https://quicklatex.com/cache3/96/ql_fab8ede7f2548c162eb9f7d78d034896_l3.png): undoes the basis transformation

---

###  Summary

- Basis = coordinate system for vectors
- Standard basis = ![](https://quicklatex.com/cache3/70/ql_3c68f72bfd90be9231c851220143cd70_l3.png)
- Change of basis rewrites the same vector in a different coordinate system
- Use the matrix ![](https://quicklatex.com/cache3/3b/ql_d181386fd2fe7ff03a3a7d56a5d1c13b_l3.png) made from new basis vectors:

![](https://quicklatex.com/cache3/95/ql_7d2b891adfa7e99f22c5622b691ed595_l3.png)

---


## 1.9 Vector Spaces and Subspaces

###  What Is a Vector Space?

A **vector space** is a set of vectors that satisfies:

1. **Vector addition** is defined  
2. **Scalar multiplication** is defined  
3. The following 8 axioms hold:  
   - Closure under addition and scalar multiplication  
   - Associativity, commutativity, distributivity  
   - Identity and inverse elements

If these hold, then you can:
- Add vectors
- Scale vectors
- Build **linear combinations**

Examples:
- ![](https://quicklatex.com/cache3/9f/ql_95f7c085eff52024e786352907bf269f_l3.png)
- Function spaces: all continuous functions on [0, 1]
- Quantum state spaces (Hilbert spaces)

---

###  What Is a Subspace?

A **subspace** is a subset of a vector space that is also a vector space. It must:

1. Contain the **zero vector**
2. Be **closed under addition**:

![](https://quicklatex.com/cache3/05/ql_b3792d4da994913ac3404d212b618f05_l3.png)

3. Be **closed under scalar multiplication**:

![](https://quicklatex.com/cache3/d1/ql_73633c44b9aeeb81f6520023bfe29bd1_l3.png)

Examples:
- A line or plane through the origin in ![](https://quicklatex.com/cache3/23/ql_dd8881b7831826c92d367f4ebd8be823_l3.png)
- The span of one or more vectors
- The set of all solutions to a homogeneous equation ![](https://quicklatex.com/cache3/b5/ql_a8eca83d3d6feecca0675a2a4110dfb5_l3.png)

---

### In Quantum Mechanics

Quantum states live in **Hilbert spaces** - special infinite-dimensional vector spaces with:

- Inner product: ![](https://quicklatex.com/cache3/52/ql_837fc5acaf2dd1e0255979ac4426c952_l3.png)
- Norms and orthogonality
- Completeness (limits of sequences exist)

These are crucial for:
- Superposition
- Measurement
- Projection onto subspaces (like eigenstates)

---

### Summary

- A **vector space** is where linear combinations make sense
- A **subspace** is a smaller vector space inside a larger one
- Subspaces must include the zero vector and be closed under both operations
- In physics: Hilbert spaces are infinite-dimensional vector spaces used to describe quantum states


## 1.10 Linear Independence and Span

### 🔹 What Is the Span?

The **span** of a set of vectors is the set of all linear combinations of them.

Let ![](https://quicklatex.com/cache3/b9/ql_a24bf367ba906582f5f8c4fbf001dbb9_l3.png) be vectors in a vector space.

Then:

![](https://quicklatex.com/cache3/59/ql_4797b9f66e775024504058c84e22ca59_l3.png)

 Intuition:
- Span is the **space you can reach** by stretching and adding those vectors.
- If you're in ![](https://quicklatex.com/cache3/23/ql_dd8881b7831826c92d367f4ebd8be823_l3.png), and you span 2 vectors, you usually get a **plane**.

---

### 🔸 What Is Linear Independence?

A set of vectors is **linearly independent** if **no vector in the set can be written as a linear combination of the others**.

Formally:
- Vectors ![](https://quicklatex.com/cache3/b9/ql_a24bf367ba906582f5f8c4fbf001dbb9_l3.png) are linearly independent if:

![](https://quicklatex.com/cache3/62/ql_91874b5bb8410c4a4ef73890ddc50e62_l3.png)

- If any nonzero solution exists, the set is **linearly dependent**.

---

### 📌 Examples

- Vectors ![](https://quicklatex.com/cache3/e1/ql_6e4a6dd8e0cdfc7d822d83fe9f8d06e1_l3.png):

  ✔️ Linearly independent  
  ✔️ Their span is all of ![](https://quicklatex.com/cache3/4d/ql_5707d877d3febd69dea9370cb8d0d04d_l3.png)

- Vectors ![](https://quicklatex.com/cache3/7a/ql_045ec2ec46c6a6af8eae4bd73fa24a7a_l3.png):

  ❌ Linearly dependent  
  ✔️ Their span is just a line

---

### 🧠 In Physics

- In **quantum mechanics**, basis vectors for a Hilbert space must be **linearly independent**
- You can express any quantum state as a **linear combination (superposition)** of basis states
- Span helps define **subspaces**, **solutions to equations**, and **degrees of freedom**

---

### ✅ Summary

| Term                 | Meaning                                                                 |
|----------------------|-------------------------------------------------------------------------|
| **Span**             | All vectors you can build from linear combinations of a set             |
| **Linear Independence** | No vector in the set is a combo of the others                         |
| **Dependent set**    | At least one vector can be written using the others                     |
| **Span + independence** | Forms a **basis** - minimal set that still spans the space           |


## 1.11 Projection and Orthogonality

### 🔸 Projection

The **projection** of one vector onto another is like dropping a shadow.  
It gives the component of one vector in the direction of another.

Let ![](https://quicklatex.com/cache3/19/ql_bfcdb9717abffe24024ab09d07c12919_l3.png).
The projection of ![](https://quicklatex.com/cache3/11/ql_8008a865e486477667198464852fed11_l3.png) is:

![](https://quicklatex.com/cache3/0a/ql_8c512a206cd25480f4b10243f770260a_l3.png)

- This gives a new vector **along** ![](https://quicklatex.com/cache3/8f/ql_1c04f6e030b06f61bcb779e7cb0a1b8f_l3.png)
- It’s the best approximation of ![](https://quicklatex.com/cache3/e6/ql_2b77d20661cb33be39e222f9820316e6_l3.png) using only the direction of ![](https://quicklatex.com/cache3/8f/ql_1c04f6e030b06f61bcb779e7cb0a1b8f_l3.png)

🧠 Think: “How much of ![](https://quicklatex.com/cache3/e6/ql_2b77d20661cb33be39e222f9820316e6_l3.png) points in the direction of ![](https://quicklatex.com/cache3/8f/ql_1c04f6e030b06f61bcb779e7cb0a1b8f_l3.png)?”

---

### 🔹 Orthogonality

Two vectors ![](https://quicklatex.com/cache3/0e/ql_eb9c0b5f81ec80b4a6cc6f07a5b38d0e_l3.png) are **orthogonal** (perpendicular) if:

![](https://quicklatex.com/cache3/45/ql_afb646a497546e7950ad252361cd8b45_l3.png)

- Geometrically: angle between them is 90°
- Algebraically: no overlap or projection

If the dot product is zero → no component of one lies in the direction of the other.

---

### 📦 In Quantum Mechanics

- Quantum states are often **orthogonal** (e.g. ![](https://quicklatex.com/cache3/dc/ql_b861a043bedef250fa1804c0352bfadc_l3.png))
- You often **project** a state onto an eigenvector or measurement basis:
  
![](https://quicklatex.com/cache3/ed/ql_f3b6a28227ff08340cc03a12a6e1dded_l3.png)

- This is a projection of ![](https://quicklatex.com/cache3/c6/ql_d4cd717bf354d8bbd4d6e7a022d9ffc6_l3.png)

---

### ✅ Summary

| Concept        | Meaning |
|----------------|---------|
| **Projection** | Shadow or component of one vector along another |
| **Orthogonal** | Vectors at 90°, dot product = 0 |
| **![](https://quicklatex.com/cache3/c1/ql_d10ad744a26cd2d79fe15c0b4b244fc1_l3.png)** | ![](https://quicklatex.com/cache3/36/ql_a28db4fc43ef83714acb10940dbe7e36_l3.png) |

---

### 🧠 Bonus Insight

If ![](https://quicklatex.com/cache3/83/ql_158ddc4c3db70331c0f19286691b4e83_l3.png),
then ![](https://quicklatex.com/cache3/a0/ql_295136544d813536965640f8ce6fd7a0_l3.png),
where ![](https://quicklatex.com/cache3/21/ql_41ba87f34eb1c5e6300b1be0d12d4c21_l3.png) is **orthogonal** to ![](https://quicklatex.com/cache3/8f/ql_1c04f6e030b06f61bcb779e7cb0a1b8f_l3.png).

This is how you break any vector into:
- A part that aligns with ![](https://quicklatex.com/cache3/8f/ql_1c04f6e030b06f61bcb779e7cb0a1b8f_l3.png)
- A part that’s perpendicular to ![](https://quicklatex.com/cache3/8f/ql_1c04f6e030b06f61bcb779e7cb0a1b8f_l3.png)

## 1.12 Inner Products

### 🔸 What Is an Inner Product?

An **inner product** is a generalization of the dot product to abstract vector spaces.  
It lets you measure:

- Length (norm)
- Angle (orthogonality)
- Projections

Denoted:
![](https://quicklatex.com/cache3/ac/ql_b98854c54810206d92484ce85b1008ac_l3.png)

In ![](https://quicklatex.com/cache3/38/ql_92203bce76ddb7fe61c47dc300625638_l3.png), it's just the dot product:

![](https://quicklatex.com/cache3/26/ql_084e2c1b2fd1382d8e92cd6ad30d6426_l3.png)

In complex spaces (like quantum states):

![](https://quicklatex.com/cache3/de/ql_4b9a3aaec44494123cfbc9cdf2f74dde_l3.png)

This includes a **complex conjugate** to ensure positivity.

---

### 🔹 Properties of Inner Products

Let ![](https://quicklatex.com/cache3/3f/ql_39f13f603a85ce511a485d8e2a77933f_l3.png) be vectors and ![](https://quicklatex.com/cache3/e4/ql_75fb6f258738cd95e798c0d5bbcff6e4_l3.png). Then:

1. **Linearity in the second argument**:
  ![](https://quicklatex.com/cache3/69/ql_cc999a5049717720dedd7b7e2e5e0a69_l3.png)

2. **Conjugate symmetry**:
  ![](https://quicklatex.com/cache3/0f/ql_53f313dc5d4994823d9ff646992a820f_l3.png)

3. **Positive-definiteness**:
  ![](https://quicklatex.com/cache3/f4/ql_108083159a29f0bf595818a4f4a19af4_l3.png)

---

### 📦 In Physics (QM Context)

- States are written as ![](https://quicklatex.com/cache3/86/ql_75b558f834b0e3f77d4d5c2d19547186_l3.png)
- Inner product gives probability amplitude:
  ![](https://quicklatex.com/cache3/17/ql_6b68cf6daec5aacaaf8f1b405a4d0d17_l3.png)

- Squared magnitude gives probability:
  ![](https://quicklatex.com/cache3/c4/ql_6dae1da2014d1cdf8bae32b8c43c61c4_l3.png)

- Orthogonality: ![](https://quicklatex.com/cache3/57/ql_2c11a16a6af5f3f74a56d46e1cc7bb57_l3.png) states are distinguishable

---

### ✅ Summary

| Concept         | Meaning |
|-----------------|---------|
| **Inner product** | Generalized dot product |
| **Notation**     | ![](https://quicklatex.com/cache3/4b/ql_4e4d0e1456d3944813aeff5ef7d4464b_l3.png)
| **Use**          | Measures angle, length, orthogonality, projection |
| **QM role**      | Probabilities, measurement, basis decomposition |

---

### 🧠 Bonus: Norm from Inner Product

![](https://quicklatex.com/cache3/09/ql_4c685e4dcde2b8af399b73d84cdbde09_l3.png)

This lets you define **unit vectors**, **distance**, and **orthonormal bases**.


## 1.13 Dirac Notation (Bra-Ket)

### 🔸 What Is Dirac Notation?

Dirac notation (also called **bra-ket notation**) is a compact way to describe vectors and inner products in **quantum mechanics**.

- A **ket** represents a column vector (a state):
 ![](https://quicklatex.com/cache3/1e/ql_cc9af0f4deda3885c19f9e9a6872571e_l3.png)

- A **bra** represents a row vector (the conjugate transpose of a ket):
  ![](https://quicklatex.com/cache3/9e/ql_8e5dd6012e693d85b63fcf7e1c7dc99e_l3.png)

- The inner product (overlap) is written as:
  ![](https://quicklatex.com/cache3/38/ql_e4fc0b3177bfe0c8f8229ca1e1f9ca38_l3.png)

---

### 🔹 Summary of Symbols

| Symbol           | Meaning                        |
|------------------|---------------------------------|
| ![](https://quicklatex.com/cache3/86/ql_75b558f834b0e3f77d4d5c2d19547186_l3.png) | A vector (quantum state)       |
| ![](https://quicklatex.com/cache3/4a/ql_b0351b43d80c8149bc11cfadf6830a4a_l3.png) | Conjugate transpose of a state |
| ![](https://quicklatex.com/cache3/ca/ql_83d7fa43fa22ec1e07c73c2c1f69d6ca_l3.png) | Inner product (scalar) |
| ![](https://quicklatex.com/cache3/2c/ql_de10699fe3b2feb00b69d2e0f516f82c_l3.png) | Operator (outer product) |

---

### 🔹 Outer Product

This is a matrix formed from a ket and a bra:

![](https://quicklatex.com/cache3/5f/ql_1c25aa12bf5218dd091143c3325ddf5f_l3.png)

Used to:
- Project onto a state
- Build density matrices
- Define linear operators

---

### 📦 In Practice (QM)

- Quantum states: 
  ![](https://quicklatex.com/cache3/bc/ql_d85337020d5a307bcb06e9b69e14abbc_l3.png)

- Measurement probabilities:
  ![](https://quicklatex.com/cache3/96/ql_376645975118aa0d1d999538342b9996_l3.png)

- Operators act on kets:
  ![](https://quicklatex.com/cache3/61/ql_f2608834dbbde6ea65f24ac81f0d8661_l3.png)

---

### ✅ Summary

- **Ket** = vector = column = ![](https://quicklatex.com/cache3/86/ql_75b558f834b0e3f77d4d5c2d19547186_l3.png)

- **Bra** = conjugate row = ![](https://quicklatex.com/cache3/6f/ql_2821d9c298f0e74d4124e4ca5b3c376f_l3.png)

- Inner product = ![](https://quicklatex.com/cache3/ca/ql_83d7fa43fa22ec1e07c73c2c1f69d6ca_l3.png)

- Outer product = operator = ![](https://quicklatex.com/cache3/2c/ql_de10699fe3b2feb00b69d2e0f516f82c_l3.png)

---

### 🧠 Bonus: Matrix Form

If:

![](https://quicklatex.com/cache3/5c/ql_70f9a73e51ed85ca4eecbd831a32015c_l3.png)

Then:

![](https://quicklatex.com/cache3/2e/ql_4154c3f41a3a1361858d30bec0cf432e_l3.png)


## 1.14 Tensor Algebra (Intro Only)

### 🔸 What Is a Tensor?

A **tensor** is a mathematical object that generalizes:

- **Scalars** (single numbers)
- **Vectors** (1D arrays)
- **Matrices** (2D arrays)

Tensors can be thought of as **multidimensional arrays** that follow specific transformation rules under change of basis.

---

### 🔹 Rank / Order of a Tensor

| Tensor Type    | Components               | Rank (Order) |
|----------------|--------------------------|--------------|
| Scalar         | ![](https://quicklatex.com/cache3/64/ql_04c710828a62bedc6f61a8b2dd43de64_l3.png)                  | 0            |
| Vector         | ![](https://quicklatex.com/cache3/ab/ql_36cebea9ad63a5c519b3655426f790ab_l3.png)                | 1            |
| Matrix         | ![](https://quicklatex.com/cache3/92/ql_44c9fb4471b8c296cf610d1f58127d92_l3.png)              | 2            |
| 3-Tensor       | ![](https://quicklatex.com/cache3/2f/ql_a5e277d903df4bcf3265c3b50cdce02f_l3.png), etc. | 3            |

- The **rank** is the number of indices the tensor has.
- Each index tells you how it behaves under transformation.

---

### 📐 Notation

- **Upper indices** (like ![](https://quicklatex.com/cache3/bd/ql_9673ccb61b4dcd22442603c2aa2eadbd_l3.png)) are **contravariant**
- **Lower indices** (like ![](https://quicklatex.com/cache3/1e/ql_71a2ffc55b4c47ec5b49894b8253a51e_l3.png)) are **covariant**

Mixed-index tensors (like ![](https://quicklatex.com/cache3/c6/ql_1ea42d97484e72a8a249eed2b2c3dac6_l3.png)) can handle transformations of both kinds.

---

### 🔄 Change of Basis Rule

A key property of tensors:  
They **transform predictably** under a change of coordinates.

Example (vector transforms):

![](https://quicklatex.com/cache3/c1/ql_f0f7b2728f95e23b239c9bc8080126c1_l3.png)

Tensors follow similar rules with multiple indices — each index transforms depending on its type (up or down).

---

### 🧠 In Physics

Tensors are everywhere:

- **Scalars**: mass, charge
- **Vectors**: velocity, force
- **Tensors**:
  - **In classical mechanics**: inertia tensor
  - **In electromagnetism**: field strength tensor ![](https://quicklatex.com/cache3/63/ql_8cb3902f251cd7110a891ff29b8b1263_l3.png)
  - **In general relativity**: metric tensor ![](https://quicklatex.com/cache3/75/ql_d29e7aa684c8190ef0c43eb43f6a5975_l3.png), curvature tensors

---

### ✅ Summary

| Concept        | Meaning |
|----------------|---------|
| **Tensor**     | Multi-index object (generalizes vectors & matrices) |
| **Rank**       | Number of indices (0 = scalar, 1 = vector, 2 = matrix) |
| **Covariant**  | Lower indices (subscripts), transforms with basis |
| **Contravariant** | Upper indices (superscripts), transforms with inverse basis |
| **Transformation rule** | Tensors keep equations valid under coordinate change |

---

### ⚠️ Note

This is just the intro. Full tensor algebra includes:

- Tensor contraction
- Tensor product
- Raising/lowering indices with the metric
- Applications to differential geometry and physics (e.g., GR)


* Used in relativity to describe curvature, gravity, and transformations

## 1.15 Hilbert Space Formalism

### 🔸 What Is a Hilbert Space?

A **Hilbert space** is a special kind of vector space used in quantum mechanics.

It has:

1. **Infinite or finite dimensions**
2. An **inner product**:
   ![](https://quicklatex.com/cache3/17/ql_6b68cf6daec5aacaaf8f1b405a4d0d17_l3.png)

3. **Completeness**: every Cauchy sequence converges in the space
4. Often over **complex numbers** ![](https://quicklatex.com/cache3/96/ql_027c5376134ca2840feef48ea2465196_l3.png)

---

### 🧠 Why Is It Important?

In quantum mechanics:

- **States** are vectors in a Hilbert space: ![](https://quicklatex.com/cache3/86/ql_75b558f834b0e3f77d4d5c2d19547186_l3.png)
- **Observables** are operators on the space: ![](https://quicklatex.com/cache3/5b/ql_279801fc042829dd3131229d367b4e5b_l3.png)
- **Probabilities** come from inner products:
 
 ![](https://quicklatex.com/cache3/47/ql_3c508bcdf851eff4f9e79204b4bbb647_l3.png)
 
- Superposition, measurement, and time evolution all use this formalism

---

### 📐 Key Properties

| Property                | Meaning                                                   |
|-------------------------|-----------------------------------------------------------|
| **Vector space**        | Closed under addition and scalar multiplication           |
| **Inner product**       | ![](https://quicklatex.com/cache3/38/ql_37609655f7849f8676e363afc8f7b338_l3.png)         |
| **Norm**                | ![](https://quicklatex.com/cache3/e9/ql_f8c17835e4d48ebe3a8096aabd97bbe9_l3.png)   |
| **Completeness**        | Limits of sequences of vectors are still in the space     |
| **Orthonormal basis**   | ![](https://quicklatex.com/cache3/74/ql_73f191fa91b941fb02e653e383a78674_l3.png)          |

---

### 🔄 Orthonormal Basis

A Hilbert space can have an **orthonormal basis** ![](https://quicklatex.com/cache3/2f/ql_0e2d988f3a0faf46d784a516642ccb2f_l3.png) such that:

![](https://quicklatex.com/cache3/53/ql_804f4bb633912849bfbc6b30327c0a53_l3.png)

This is like a Fourier expansion — any state is a linear combination of basis states.

---

### 🧪 Example: Qubit Hilbert Space

For a single qubit (2D system):

![](https://quicklatex.com/cache3/c1/ql_89c1174db679b80f53e61c2ef80defc1_l3.png)

Any qubit state is:

![](https://quicklatex.com/cache3/e8/ql_d065c70b8b6d760bc2d734a5447c39e8_l3.png)

---

### ✅ Summary

| Concept              | Meaning |
|----------------------|---------|
| **Hilbert space**    | Vector space + inner product + completeness |
| **Quantum state**    | Vector in Hilbert space ![](https://quicklatex.com/cache3/86/ql_75b558f834b0e3f77d4d5c2d19547186_l3.png) |
| **Measurement**      | Projects onto a subspace, gives probability |
| **Operators**        | Act on states: ![](https://quicklatex.com/cache3/5b/ql_279801fc042829dd3131229d367b4e5b_l3.png) |
| **Basis states**     | Form complete orthonormal set: ![](https://quicklatex.com/cache3/74/ql_73f191fa91b941fb02e653e383a78674_l3.png) |
