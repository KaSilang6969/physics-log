## 1.1 What is Thermodynamics

* Thermodynamics is the study of **heat, work, energy**, and how they relate.
* In physics, it's crucial for understanding:

  * Statistical mechanics
  * Black hole entropy and Hawking radiation
  * Quantum field theory at finite temperature

---

## 1.2 Thermodynamic Variables

### Types

* **Extensive**: depends on amount of substance (energy, volume, entropy, mass)
* **Intensive**: independent of amount (temperature, pressure, chemical potential)

### Common Symbols

* `U`: internal energy
* `T`: temperature
* `S`: entropy
* `P`: pressure
* `V`: volume
* `μ`: chemical potential
* `F`: Helmholtz free energy
* `G`: Gibbs free energy

---

## 1.3 The Four Laws of Thermodynamics

### Zeroth Law

* If A = B and B = C in thermal equilibrium, then A = C.
* This defines **temperature** as a consistent concept.

### First Law (Energy Conservation)

* Energy is conserved:

  * `dU = δQ - δW`
  * `dU = TdS - PdV` (for reversible processes)

### Second Law

* **Entropy** always increases in a closed system:

  * `ΔS ≥ 0`
* Heat flows naturally from hot to cold.

### Third Law

* As `T → 0`, `S → constant` (often 0)
* Perfect crystals have minimum entropy at 0 K

---

## 1.4 Thermodynamic Potentials

* These are used depending on what's held constant:

### Internal Energy `U`

* Fundamental potential: `U(S, V)`

### Helmholtz Free Energy `F`

* `F = U - TS`
* Use when `T, V` are constant

### Gibbs Free Energy `G`

* `G = U - TS + PV = F + PV`
* Use when `T, P` are constant

### Enthalpy `H`

* `H = U + PV`
* Use when `S, P` are constant

---

## 1.5 Maxwell Relations

* These come from taking second derivatives of thermodynamic potentials.
* Very useful for relating quantities you can't directly measure.

### Example

* From `dF = -S dT - P dV`, derive:

  * ![](https://quicklatex.com/cache3/01/ql_11ee9b6616253a40001e2df303e30f01_l3.png)

---

## 1.6 Equations of State

* These relate state variables (like `P`, `V`, `T`) to each other.
* Ideal Gas Law:

  * `PV = nRT`
* van der Waals equation (real gas):

  * ![](https://quicklatex.com/cache3/e2/ql_8a6558b5a234b07aa67de615c78afae2_l3.png)

---

## 1.7 Heat Capacity

* Measures how much energy is needed to change temperature.
* Two types:

  * At constant volume: ![](https://quicklatex.com/cache3/44/ql_522d3a449dbee295a0bdcc85c9e87c44_l3.png)
  * At constant pressure: ![](https://quicklatex.com/cache3/03/ql_c28b4d72ca615315216b912a85cbcd03_l3.png)

---

## 1.8 Useful Derivatives in Thermo

* ![](https://quicklatex.com/cache3/ba/ql_1914870d7056fed2f945cea0158e5aba_l3.png)
* ![](https://quicklatex.com/cache3/3e/ql_b0b1964a3b89a7f50286a7cecfae883e_l3.png)
* ![](https://quicklatex.com/cache3/ae/ql_6bb7084c98576242d55e1e2495ac78ae_l3.png)

---

## 1.9 Applications in Theoretical Physics

* **Black holes**: Bekenstein–Hawking entropy, temperature, area law
* **AdS/CFT**: Thermodynamics maps to boundary QFT thermodynamics
* **Statistical mechanics**: Thermodynamics is recovered from ensemble averages
* **Cosmology**: Thermodynamic expansion laws, entropy of universe
