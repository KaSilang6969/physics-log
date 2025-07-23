## 1.1 What Are Partial Derivatives

* A **partial derivative** measures how a function with several variables changes when only **one variable changes**, holding the others fixed.
* This is useful when dealing with multivariable functions in physics.

### Notation

* If: ![](https://quicklatex.com/cache3/49/ql_a6f16d499ec3784b184d365d4553ab49_l3.png)
* Then:

 * ![](https://quicklatex.com/cache3/dc/ql_6c6e791d86de966325ada89d0afb43dc_l3.png) = derivative of f with respect to x, treating y as a constant

 * ![](https://quicklatex.com/cache3/7d/ql_7de31f7d6c86abc744abb5c2f0a7fa7d_l3.png) = derivative of f with respect to y, treating x as a constant

### Example

* Let: ![](https://quicklatex.com/cache3/d8/ql_8e59d48b215ab07445941c62189539d8_l3.png)
* Then:

  * ![](https://quicklatex.com/cache3/b5/ql_b2be3e1d1fd696f37e72e381265c20b5_l3.png)
  * ![](https://quicklatex.com/cache3/7f/ql_908cb0924d0bf647e9a3ea6114f4a57f_l3.png)

### Why It's Important

* Used in:

  * [Thermodynamics:](misc/Thermodynamics.md) ![](https://quicklatex.com/cache3/2b/ql_d98187207c95f779cfde2630ebe4da2b_l3.png),  ![](https://quicklatex.com/cache3/a6/ql_c0e03a8b60cdf06307e9ef98a5ee64a6_l3.png)
  * [Electromagnetism:](misc/Electromagenetism.md) fields like ![](https://quicklatex.com/cache3/86/ql_b7df271408505815c51c5a63ce680686_l3.png)
  * [Quantum Mechanics:](misc/Quantum%20Mechanics%20(Overview).md) ![](https://quicklatex.com/cache3/6f/ql_1f7b28115d06036e8c9d066d1fa39f6f_l3.png)
  * General relativity: tensor fields

---

## 1.2 Second-Order and Mixed Partials

* You can take the derivative of a derivative (second-order):

  * ![](https://quicklatex.com/cache3/42/ql_447fc1268bc59c667ca9dfef98045542_l3.png)
  * ![](https://quicklatex.com/cache3/30/ql_c4fbe787fb70ca2ca72d8569de80c730_l3.png)

### Clairaut’s Theorem (if smooth function)

* Mixed partials are equal:

  * ![](https://quicklatex.com/cache3/aa/ql_d4133f7d84de52f4d47e478623dbb3aa_l3.png)

---

## 1.3 Chain Rule (Multivariable)

### Case 1: Single Variable Dependence

* If: ![](https://quicklatex.com/cache3/6d/ql_742fb61625312283288eb6afe590066d_l3.png)
* Then:

  * ![](https://quicklatex.com/cache3/c4/ql_8ac06a74dadb9fca5fb085440ce3b4c4_l3.png)

### Case 2: General Case (Multiple Intermediates)

* If: 
![](https://quicklatex.com/cache3/68/ql_120f50d2b9174e8fa889d4c044ee8868_l3.png)


and each ![](https://quicklatex.com/cache3/00/ql_d00b4f9929d479cc7fdb592c7f7c2c00_l3.png)

* Then:

 * ![](https://quicklatex.com/cache3/a5/ql_8dfa0b72938acd84ce4a3d46e2bf8ba5_l3.png)

### Why It’s Used

* Lagrangian mechanics: ![](https://quicklatex.com/cache3/79/ql_e83524fef40c098820ef80d754c60579_l3.png)
* Thermodynamic identities
* Field theory and coordinate transformations

---

## 1.4 Gradient (\nabla f)

* The **gradient** is a vector pointing in the direction of steepest increase.
* Defined as:

  * ![](https://quicklatex.com/cache3/a9/ql_6f999913c4eecbd59a03ea3d608a14a9_l3.png)

### Example

* If: ![](https://quicklatex.com/cache3/82/ql_91db2f7975eec81df244a665b8f7f682_l3.png)
* Then: ![](https://quicklatex.com/cache3/c5/ql_00b29ead9fcff576666d0ebfc96fa5c5_l3.png)

### Why It's Useful

* Appears in:

  * Newtonian force fields: ![](https://quicklatex.com/cache3/e3/ql_9608f2e90a359afab406254366cadce3_l3.png)
  * Electromagnetic theory
  * Wave equations, fluid flow, heat equations


