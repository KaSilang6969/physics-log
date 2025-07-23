## 1.1 Calculus of Variation

The **calculus of variations** (or **variational calculus**) is a field of [mathematical analysis](https://en.wikipedia.org/wiki/Mathematical_analysis "Mathematical analysis") that uses variations, which are small changes in [functions](https://en.wikipedia.org/wiki/Function_$mathematics$ "Function (mathematics)") and [functionals](https://en.wikipedia.org/wiki/Functional_$mathematics$ "Functional (mathematics)"), to find maxima and minima of functionals: [mappings](https://en.wikipedia.org/wiki/Map_$mathematics$ "Map (mathematics)") from a set of [functions](https://en.wikipedia.org/wiki/Function_$mathematics$ "Function (mathematics)") to the [real numbers](https://en.wikipedia.org/wiki/Real_number "Real number").[[a]](https://en.wikipedia.org/wiki/Calculus_of_variations#cite_note-2) Functionals are often expressed as [definite integrals](https://en.wikipedia.org/wiki/Definite_integral "Definite integral") involving functions and their [derivatives](https://en.wikipedia.org/wiki/Derivative "Derivative"). Functions that maximize or minimize functionals may be found using the [Euler–Lagrange equation](https://en.wikipedia.org/wiki/Euler%E2%80%93Lagrange_equation "Euler–Lagrange equation") of the calculus of variations.

A simple example of such a problem is to find the curve of shortest length connecting two points. If there are no constraints, the solution is a [straight line](https://en.wikipedia.org/wiki/Straight_line "Straight line") between the points. However, if the curve is constrained to lie on a surface in space, then the solution is less obvious, and possibly many solutions may exist. Such solutions are known as _[geodesics](https://en.wikipedia.org/wiki/Geodesic "Geodesic")_. A related problem is posed by [Fermat's principle](https://en.wikipedia.org/wiki/Fermat%27s_principle "Fermat's principle"): light follows the path of shortest [optical length](https://en.wikipedia.org/wiki/Optical_length "Optical length") connecting two points, which depends upon the material of the medium. One corresponding concept in [mechanics](https://en.wikipedia.org/wiki/Mechanics "Mechanics") is the [principle of least/stationary action](https://en.wikipedia.org/wiki/Principle_of_least_action "Principle of least action").

Many important problems involve functions of several variables. Solutions of [boundary value problems](https://en.wikipedia.org/wiki/Boundary_value_problem "Boundary value problem") for the [Laplace equation](https://en.wikipedia.org/wiki/Laplace_equation "Laplace equation") satisfy the [Dirichlet's principle](https://en.wikipedia.org/wiki/Dirichlet%27s_principle "Dirichlet's principle"). [Plateau's problem](https://en.wikipedia.org/wiki/Plateau%27s_problem "Plateau's problem") requires finding a surface of minimal area that spans a given contour in space: a solution can often be found by dipping a frame in soapy water. Although such experiments are relatively easy to perform, their mathematical formulation is far from simple: there may be more than one locally minimizing surface, and they may have non-trivial [topology](https://en.wikipedia.org/wiki/Topology "Topology").

Typical problem:  
Find a function y(x) that **extremizes** the functional:

![Problem](https://quicklatex.com/cache3/44/ql_a8d5ff9f88ee34448ea227aa62f51c44_l3.png)

## 1.2 What’s the Goal?
You’re not just solving equations — you’re finding the function that makes something maximum or minimum (like shortest path, least time, etc).

This is how physics derives real-world behavior from a principle.

## 1.3 Functionals: What We Extremize
Idea:
A functional takes a whole function as input and gives a number.

Formula:

![](https://quicklatex.com/cache3/a0/ql_72e23b4fcd7b326c6646447430fdf5a0_l3.png)

- 𝑦(𝑥): function you're trying to find
- 𝐿: called the Lagrangian — it depends on 𝑥, 𝑦, 𝑦′
- J[y]: number (like length, time, energy)

## 1.4. Euler–Lagrange Equation: The Master Formula
This is what you apply to extremize (minimize or maximize) the functional.

Formula:

![](https://quicklatex.com/cache3/94/ql_faec71217cacc1a5fb893d81b9030994_l3.png)

Think of it like:
“Take the derivative of what you get when you partially differentiate with respect to 𝑦, and subtract the partial with respect to 
𝑦. Set that to 0.”

Example:
Find the shortest path between two points. The Lagrangian is:

![Shortest-Path](https://quicklatex.com/cache3/73/ql_2f64218c711a81ceb477e8e6a90b3f73_l3.png)

Apply Euler–Lagrange and solve — result: a straight line.

##  1.5. Principle of Least Action (Hamilton’s Principle)
This is THE guiding principle of theoretical mechanics.

"The actual path a system takes makes the action stationary."

Formula:

![Least-Action](https://quicklatex.com/cache3/db/ql_9f01cd77fa0589dd4dab157fc9a92edb_l3.png)

Then apply:

![Least-Action](https://quicklatex.com/cache3/cc/ql_d4a30a6d4991fa8863837850d206f5cc_l3.png)
This gives Lagrange's Equations — core of classical mechanics.

## 1.6. Lagrangian Mechanics
Step-by-step:
Choose coordinates 𝑞𝑖 ​(generalized positions)

- Compute kinetic energy 𝑇
- Compute potential energy 𝑉

Define:

![](https://quicklatex.com/cache3/35/ql_91f602564bb42479965e20717de14135_l3.png)

Plug into:

![Potential](https://quicklatex.com/cache3/f5/ql_ee2f8f989f2e2e7515e180aebc9234f5_l3.png)
That’s your equation of motion!

## 1.7. Hamiltonian Mechanics
Why?
Sometimes it’s better to describe motion in terms of position and momentum rather than position and velocity.

Define momentum:

![Momentum](https://quicklatex.com/cache3/aa/ql_1d77ee15d83a49a0dc6263e9b83c60aa_l3.png)

Define Hamiltonian:

![Hamilton](https://quicklatex.com/cache3/2e/ql_765fee50c96fe51bb10b52d04fda0c2e_l3.png)

Hamilton’s Equations:
![Hamilton](https://quicklatex.com/cache3/26/ql_2d8fdeb8d79609e4aaa9aae1b029a626_l3.png)Used in quantum mechanics, statistical mechanics, and more.

## 1.8. Noether’s Theorem
Symmetries lead to conserved quantities.

- Time symmetry → energy conserved
- Space symmetry → momentum conserved
- Rotation symmetry → angular momentum conserved

This is how physics links math structure to real-world conservation laws.


## 1.9. Common Problems You’ll See
### Shortest path (between two points)
Use the Euler–Lagrange equation with the arc length Lagrangian.

Lagrangian:

![Lagrangian](https://quicklatex.com/cache3/77/ql_5f5a4100250cf872618284cc04f39277_l3.png)

Solving gives a straight line.

### Lagrangian mechanics
Use the Lagrangian, defined as kinetic minus potential energy.

Lagrangian:

![](https://quicklatex.com/cache3/35/ql_91f602564bb42479965e20717de14135_l3.png)

Apply:

![](https://quicklatex.com/cache3/2d/ql_ca73ee55e90038043598dcad4aead72d_l3.png)

### Harmonic oscillator (mass-spring system)
A classic physics example. Use position 
𝑥 as the coordinate.

Lagrangian:

![](https://quicklatex.com/cache3/f1/ql_d572d342c1e121c9852723941ab92bf1_l3.png)

Resulting equation:

![](https://quicklatex.com/cache3/de/ql_e8ea426ba0e28a8436892a474730eede_l3.png)

Pendulum (simple planar)
Use angle 𝜃 as the coordinate (instead of x/y).

Lagrangian:

![](https://quicklatex.com/cache3/c1/ql_6fb2b333e49186a383bc5696491fb0c1_l3.png)

Apply Euler–Lagrange to get:

![](https://quicklatex.com/cache3/c7/ql_2f03ad2063dcc5fe8c7a2f9062e3c3c7_l3.png)

### Field theory (Lagrangian density)
Instead of a particle, you’re dealing with fields (like EM fields). Use spacetime variables.

Action:

![](https://quicklatex.com/cache3/91/ql_11687b6c0bd3d92192f235df70e34f91_l3.png)

Euler–Lagrange for fields:

![](https://quicklatex.com/cache3/83/ql_1a82b1b3cfd33ed5391dacb5c37a6283_l3.png)

