# **Time as an Emergent Quantity: A Multi-Framework Mathematical Argument with Empirical Predictions**

---

## **Abstract**

We present a rigorous, multi-framework case for the non-fundamentality of time in physics. Building on classical mechanics, canonical general relativity, and relational quantum mechanics, we demonstrate that time can be removed from the fundamental formulation of dynamics and subsequently recovered as an emergent parameter from correlations, action, or state structure.

In classical mechanics, the Jacobi reparametrization-invariant action generates dynamics without reference to an external parameter, with Newtonian time derivable from configuration change and energy. In canonical general relativity, the Hamiltonian constraint yields a timeless Wheeler–DeWitt equation, with semiclassical WKB expansion producing an emergent time functional. In the Page–Wootters construction of relational quantum mechanics, stationary global states yield Schrödinger evolution for subsystems conditional on clock readings.

We extend these frameworks to address four major objections to emergent time theories:

1. The thermodynamic arrow of time
2. Macroscopic temporal ordering from timeless microscopics
3. Compatibility with quantum entanglement experiments
4. Cosmological evolution without fundamental time

Finally, we propose concrete empirical tests to distinguish emergent time from fundamental time.

---

## **1. Introduction**

In standard formulations of physics, time is treated as a fundamental coordinate or parameter: Newtonian mechanics defines motion with respect to $t$, special relativity includes time as part of the spacetime manifold, and the Schrödinger equation evolves wavefunctions in $t$. However, multiple modern developments challenge the necessity of fundamental time.

Two strands of theory motivate reconsidering time’s status:

1. **Reparametrization invariance** in classical mechanics and general relativity, where coordinate time is a gauge choice.
2. **Relational approaches** in quantum mechanics, where time emerges from correlations between subsystems.

Our goal is to provide a unified, mathematically precise demonstration that time can be removed from the fundamental formalism and recovered from more primitive structures, while also answering major conceptual and empirical objections.

---

## **2. Frameworks of Analysis**

We examine three independent but conceptually related frameworks:

1. **Jacobi Action Principle (Classical Mechanics)** — dynamics without time as a primitive parameter.
2. **Canonical GR and Wheeler–DeWitt Equation** — timeless quantum gravity constraints with semiclassical time emergence.
3. **Page–Wootters Relational Quantum Mechanics** — subsystem evolution from globally stationary states.

---

## **3. Mathematical Formulations**

### **3.1 Jacobi Action: Time from Change and Energy**

For configuration coordinates $q^i$ with kinetic metric $g_{ij}(q)$, total energy $E$, and potential $V(q)$, the reparametrization-invariant Jacobi action is:

$$
S_J[q(\lambda)] = \int_{\lambda_1}^{\lambda_2} \sqrt{2(E-V(q))}\, \sqrt{g_{ij}(q)\frac{dq^i}{d\lambda}\frac{dq^j}{d\lambda}}\, d\lambda.
$$

This action is invariant under reparametrizations $\lambda \mapsto f(\lambda)$ and fixes only the *path* in configuration space.

Define emergent time:

$$
dt = \frac{\sqrt{g_{ij}\,dq^i dq^j}}{\sqrt{2(E-V(q))}}.
$$

Using this recovers Newtonian equations of motion, showing $t$ is *derived*, not fundamental.

---

### **3.2 Canonical GR and the Wheeler–DeWitt Equation**

In canonical GR, the Hamiltonian constraint is:

$$
\mathcal{H}(x) = 0.
$$

Quantization gives:

$$
\hat{\mathcal{H}}(x)\,\Psi[g_{ij},\phi] = 0,
$$

with no $t$.

WKB expansion:

$$
\Psi[g,\phi] \approx e^{\frac{i}{\hbar}S_0[g]} \chi[g,\phi]
$$

yields classical gravity from $S_0[g]$ and a Schrödinger equation for matter with emergent **WKB time** $t_{\text{WKB}}$.

---

### **3.3 Page–Wootters Relational Quantum Mechanics**

Split Hilbert space: $\mathcal{H} = \mathcal{H}_C \otimes \mathcal{H}_S$.

Global constraint:

$$
(\hat{H}_C + \hat{H}_S) |\Psi\rangle = 0.
$$

Clock states $|t\rangle_C$ satisfy:

$$
e^{-i\hat{H}_C \delta t/\hbar} |t\rangle_C = |t+\delta t\rangle_C.
$$

Conditional system state:

$$
|\psi(t)\rangle_S \equiv {}_C\langle t | \Psi\rangle
$$

obeys:

$$
i\hbar \frac{\partial}{\partial t} |\psi(t)\rangle = \hat{H}_S |\psi(t)\rangle.
$$

Here $t$ is internal — a clock reading.

---

## **4. Addressing Major Criticisms**

### **4.1 Thermodynamic Arrow of Time**

Define macrostates $M$ in microstate space $\Gamma$ with Boltzmann entropy:

$$
S = k_B \ln \Omega(M).
$$

In a timeless framework, introduce ordering parameter $\tau$ such that $S(\tau)$ increases for almost all trajectories. The arrow of time is thus an emergent statistical property of coarse-grained relational states.

---

### **4.2 Macroscopic Temporal Ordering**

Introduce a partial order $\prec$ on events via causal correlations, as in causal set theory. The macroscopic “timeline” is the embedding of $(E, \prec)$ into a manifold admitting an effective time coordinate.

---

### **4.3 Quantum Entanglement Compatibility**

Entanglement correlations can be reproduced in a static Hilbert space by using one subsystem as a relational clock for the other, preserving Bell-test statistics without fundamental $t$.

---

### **4.4 Cosmological Evolution**

In the Wheeler–DeWitt framework, choose a matter field $\phi_c$ as a clock. Condition on $\phi_c$ to recover FLRW-like expansion without introducing an absolute time coordinate.

---

## **5. Predictions and Falsifiability**

**1. Clock-Choice Anomalies in Quantum Correlations**
Test Bell-type experiments with different clock subsystems; small deviations may appear in extreme conditions.

**2. Entropy-Defined Arrow Reversals**
In mesoscopic isolated systems, entropy-defined ordering may fluctuate — impossible under universal fundamental time.

**3. Early-Universe Relational Signatures**
CMB or LSS correlations might show patterns incompatible with standard FLRW time evolution.

**4. Thermodynamic Clock Divergence**
Different entropy-based clocks may drift over cosmological scales; compare pulsar timing arrays with atomic clocks.

---

## **6. Discussion**

* **Arrow:** From entropy growth in coarse-grained state space.
* **Ordering:** From causal correlation partial orders.
* **Quantum:** From relational Hilbert space decomposition.
* **Cosmology:** From conditioning on matter clocks.
* **Testability:** Concrete experimental predictions proposed.

---

## **7. Conclusion**

We have shown that time can be formulated as emergent in three major frameworks, addressed key conceptual criticisms, and proposed falsifiable predictions. Time may be a robust emergent construct, not a fundamental unit of physics.

---

## **References**

1. Barbour, J. (1994). *The timelessness of quantum gravity: I. The evidence from the classical theory*. Classical and Quantum Gravity, 11(12), 2853.
2. Misner, C. W., Thorne, K. S., & Wheeler, J. A. (1973). *Gravitation*. W. H. Freeman.
3. Kuchař, K. V. (1992). *Time and interpretations of quantum gravity*. In *Proceedings of the 4th Canadian Conference on General Relativity and Relativistic Astrophysics*.
4. Page, D. N., & Wootters, W. K. (1983). *Evolution without evolution: Dynamics described by stationary observables*. Phys. Rev. D, 27(12), 2885.
5. Rovelli, C. (1991). *Time in quantum gravity: An hypothesis*. Phys. Rev. D, 43(2), 442.
6. Connes, A., & Rovelli, C. (1994). *Von Neumann algebra automorphisms and time-thermodynamics relation in generally covariant quantum theories*. Class. Quantum Grav., 11(12), 2899.
