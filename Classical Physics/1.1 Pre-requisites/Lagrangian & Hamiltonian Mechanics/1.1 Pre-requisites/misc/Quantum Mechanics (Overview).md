## 1.1 What is Quantum Mechanics (Overview for Theoretical Physics)

* Quantum mechanics is the theory that describes **particles and waves** at the smallest scales.
* It replaces classical mechanics when dealing with:

  * Atoms, subatomic particles
  * Quantum fields
  * Photons, electrons, quarks, etc.
* Core principle: **Physical systems are described by wavefunctions**, and **observables** come from operators.

---

## 1.2 Key Concepts

* **Wavefunction**: ![](https://quicklatex.com/cache3/6f/ql_1f7b28115d06036e8c9d066d1fa39f6f_l3.png) contains all info about a system. Squared magnitude ![](https://quicklatex.com/cache3/3d/ql_8e396936e520d367c66fc4bc4c09fd3d_l3.png) gives probability density.
* **Hilbert space**: the space of all possible wavefunctions.
* **Operators**: mathematical objects that correspond to physical observables.

  * Example: position ![](https://quicklatex.com/cache3/b6/ql_f7341b8e290df2a6c81d24076abf36b6_l3.png), momentum ![](https://quicklatex.com/cache3/21/ql_8c987a50804c83863fb78f8bd9eae221_l3.png)
* **Eigenvalues**: measurement outcomes; if ![](https://quicklatex.com/cache3/8c/ql_4273a87f8ab0e538d823a9d057d7458c_l3.png), then `a` is the value you can observe.

---

## 1.3 Postulates of Quantum Mechanics

1. **State**: The state of a system is a vector ![](https://quicklatex.com/cache3/e0/ql_ea350f937a5a48c4978db3b4c1526be0_l3.png) in Hilbert space.
2. **Observables**: Every measurable quantity is represented by a Hermitian operator.
3. **Measurement**: Measuring `A` gives eigenvalue `a` with probability ![](https://quicklatex.com/cache3/0f/ql_90ce5936d1eface077ed701d393cce0f_l3.png)
4. **Time evolution**: Governed by the Schrödinger equation:

   * ![](https://quicklatex.com/cache3/60/ql_6cdca726100bf28a5ac6695852fbdf60_l3.png)

---

## 1.4 Schrödinger Equation

* **Time-dependent**:

  * ![](https://quicklatex.com/cache3/a7/ql_af2339cba0a1d2fe0992a4db359745a7_l3.png)

* **Time-independent** (stationary states):

  * ![](https://quicklatex.com/cache3/41/ql_f3d03dd52c1dca3b7ed6029381a90d41_l3.png)

* ![](https://quicklatex.com/cache3/ca/ql_810117c1d9bf98bd22b6115c8d6428ca_l3.png) is the **Hamiltonian**, which gives total energy:

  * For one particle: ![](https://quicklatex.com/cache3/84/ql_92372e8a9db03783d738aa89e82de884_l3.png)

---

## 1.5 Commutators and the Uncertainty Principle

* The commutator of two operators is:

  * ![](https://quicklatex.com/cache3/b7/ql_f6b776fb66300af11966c91033e63db7_l3.png)

### Canonical Commutation Relation

* ![](https://quicklatex.com/cache3/f6/ql_4fddb75e4fabca930a1296638a24bef6_l3.png)

### Uncertainty Principle

* ![](https://quicklatex.com/cache3/83/ql_d51049e152af25ab9c2f52d3f6556983_l3.png)
* The more precisely you know position, the less you know momentum.

---

## 1.6 Dirac Notation

* ![](https://quicklatex.com/cache3/e0/ql_ea350f937a5a48c4978db3b4c1526be0_l3.png): state vector ("ket")
* ![](https://quicklatex.com/cache3/68/ql_c4cd68b8884ea7f52848b99eb6a24268_l3.png): dual vector ("bra")
* ![](https://quicklatex.com/cache3/e3/ql_efa66dba015a997b3ecf9203926053e3_l3.png): inner product
* ![](https://quicklatex.com/cache3/11/ql_fa8322b6ac2a73893c63ff52f14f9a11_l3.png): applying operator A to state

---

## 1.7 Basis and Representations

* States can be expressed in different bases:

  * **Position basis**: ![](https://quicklatex.com/cache3/5c/ql_0303daa638af0c4cf1fc0f1b8f09fa5c_l3.png)
  * **Momentum basis**: ![](https://quicklatex.com/cache3/88/ql_06001f88d4e794bcdfb709c534ed3b88_l3.png)
* **Fourier transform** connects position and momentum representations.

---

## 1.8 Superposition and Linearity

* If ![](https://quicklatex.com/cache3/b0/ql_bc69e5e481a76a61c42f7ef502192eb0_l3.png) and ![](https://quicklatex.com/cache3/b2/ql_b259d692a774538ec583133f3bb3cdb2_l3.png) are valid states, then so is:

  * ![](https://quicklatex.com/cache3/57/ql_53901715feeced8be8a7a88d21c68357_l3.png)
* This leads to interference and wave behavior.

---

## 1.9 Entanglement

* When two systems share a state that can't be factored:

  * ![](https://quicklatex.com/cache3/6d/ql_4d0007d6bec2639075d83d0813781d6d_l3.png)
* Measurement on one system affects the other — even at a distance.

---

## 1.10 Measurement and Collapse

* When you measure a system, the wavefunction **collapses** to an eigenstate:

  * Before: ![](https://quicklatex.com/cache3/ab/ql_5188e5fb70d41e1ea89efed8200fa4ab_l3.png)
  * After: ![](https://quicklatex.com/cache3/9f/ql_a87211717347ecbb9be45fd880c1519f_l3.png) or ![](https://quicklatex.com/cache3/dc/ql_fd7d6a4ed63612f4d4d1efe9570a58dc_l3.png) with probabilities ![](https://quicklatex.com/cache3/73/ql_1a16cf02be086990dc0cecc6da081a73_l3.png) and ![](https://quicklatex.com/cache3/5e/ql_38bfab667b3e4bd6259333289f4a4b5e_l3.png)

---

## 1.11 Applications in Theoretical Physics

* **Quantum field theory (QFT)**: quantum mechanics + special relativity
* **Quantum computing**: qubits use superposition and entanglement
* **Black hole physics**: Hawking radiation is quantum mechanical
* **String theory**: quantum mechanics on vibrating strings

