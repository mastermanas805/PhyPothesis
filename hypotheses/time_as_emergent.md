## **Time as an Emergent Quantity: A Multi-Framework Mathematical Argument**

---

### **Abstract**

We present a rigorous, multi-framework case for the non-fundamentality of time in physics. Building on classical mechanics, canonical general relativity, and relational quantum mechanics, we demonstrate that time can be removed from the fundamental formulation of dynamics and subsequently recovered as an emergent parameter from correlations, action, or state structure. In classical mechanics, the Jacobi reparametrization-invariant action generates dynamics without reference to an external parameter, with Newtonian time derivable from configuration change and energy. In canonical general relativity, the Hamiltonian constraint yields a timeless Wheeler–DeWitt equation, with semiclassical WKB expansion producing an emergent time functional. In the Page–Wootters construction of relational quantum mechanics, stationary global states yield Schrödinger evolution for subsystems conditional on clock readings. Across these contexts, time appears as a secondary bookkeeping variable rather than a primary ontological entity, suggesting that its fundamentality is at best an effective feature of semiclassical regimes.

---

### **1. Introduction**

In standard formulations of physics, time is treated as a fundamental coordinate or parameter: Newtonian mechanics defines motion with respect to $t$, special relativity includes time as part of the spacetime manifold, and the Schrödinger equation evolves wavefunctions in $t$. However, multiple modern developments challenge the necessity of fundamental time.

Two strands of theory motivate reconsidering time’s status:

1. **Reparametrization invariance** in classical mechanics and general relativity, where coordinate time is a gauge choice.
2. **Relational approaches** in quantum mechanics, where time emerges from correlations between subsystems.

Our goal is to provide a unified, mathematically precise demonstration that time can be removed from the fundamental formalism and recovered from more primitive structures.

---

### **2. Frameworks of Analysis**

We examine three independent but conceptually related frameworks:

1. **Jacobi Action Principle (Classical Mechanics)** — dynamics without time as a primitive parameter.
2. **Canonical GR and Wheeler–DeWitt Equation** — timeless quantum gravity constraints with semiclassical time emergence.
3. **Page–Wootters Relational Quantum Mechanics** — subsystem evolution from globally stationary states.

---

### **3. Mathematical Formulations**

#### **3.1 Jacobi Action: Time from Change and Energy**

Consider a system with configuration coordinates $q^i$ and kinetic metric $g_{ij}(q)$, total energy $E$, and potential $V(q)$. The reparametrization-invariant Jacobi action is:

$$
S_J[q(\lambda)] = \int_{\lambda_1}^{\lambda_2} \sqrt{2(E-V(q))}\, \sqrt{g_{ij}(q)\frac{dq^i}{d\lambda}\frac{dq^j}{d\lambda}}\, d\lambda.
$$

This action is invariant under reparametrizations $\lambda \mapsto f(\lambda)$ and fixes only the *path* in configuration space, not its parameterization.

Define the emergent time parameter along a solution as:

$$
dt = \frac{\sqrt{g_{ij}\,dq^i dq^j}}{\sqrt{2(E-V(q))}}.
$$

Using this definition recovers the standard Newtonian equations of motion, showing $t$ is *derivable*, not fundamental.

---

#### **3.2 Canonical GR and the Wheeler–DeWitt Equation**

In canonical general relativity, the Hamiltonian is a sum of constraints; the Hamiltonian constraint reads:

$$
\mathcal{H}(x) = 0.
$$

Quantization yields the Wheeler–DeWitt equation:

$$
\hat{\mathcal{H}}(x)\,\Psi[g_{ij},\phi] = 0,
$$

with no external $t$ present.

To recover time, we employ a WKB expansion:

$$
\Psi[g,\phi] \approx e^{\frac{i}{\hbar}S_0[g]} \chi[g,\phi].
$$

At leading order, $S_0[g]$ satisfies the Hamilton–Jacobi equation for gravity. At next order, $\chi$ obeys a Schrödinger equation with respect to a *WKB time functional* $t_{\text{WKB}}$ derived from $S_0[g]$.

Thus, in the fundamental equation, time is absent and only reappears as a semiclassical approximation.

---

#### **3.3 Page–Wootters Relational Quantum Mechanics**

Partition the Hilbert space into clock $C$ and system $S$: $\mathcal{H} = \mathcal{H}_C \otimes \mathcal{H}_S$. The global state satisfies the stationary constraint:

$$
(\hat{H}_C + \hat{H}_S) |\Psi\rangle = 0.
$$

Let $|t\rangle_C$ be clock states such that:

$$
e^{-i\hat{H}_C \delta t/\hbar} |t\rangle_C = |t+\delta t\rangle_C.
$$

The conditional system state given clock reading $t$ is:

$$
|\psi(t)\rangle_S \equiv {}_C\langle t | \Psi\rangle.
$$

Projecting the global constraint yields:

$$
i\hbar \frac{\partial}{\partial t} |\psi(t)\rangle = \hat{H}_S |\psi(t)\rangle.
$$

This is the Schrödinger equation for $S$, with $t$ now an *internal* variable — the reading of the clock subsystem.

---

### **4. Discussion**

Across all three frameworks:

* The **fundamental equations** are timeless (Jacobi action, Wheeler–DeWitt, stationary global state).
* Time emerges through a *choice* of a subsystem or background to serve as a clock and a relation between its change and other degrees of freedom.
* This approach naturally explains why time in quantum gravity is relational and why semiclassical time breaks down near Planck scales or in the absence of good clocks.

These results do not merely reinterpret time philosophically; they follow directly from the mathematical structure of reparametrization-invariant and constrained Hamiltonian systems.

---

### **5. Conclusion**

We have provided three independent derivations — in classical, gravitational, and quantum contexts — where time is not a fundamental primitive but emerges from deeper, timeless structures. While experimental evidence cannot yet distinguish a fundamentally timeless universe from one with intrinsic time, the existence of exact timeless formulations strongly suggests that time’s fundamentality is an *effective* property of semiclassical regimes rather than an ontological necessity.

---

### **References**

1. Barbour, J. (1994). *The timelessness of quantum gravity: I. The evidence from the classical theory*. Classical and Quantum Gravity, 11(12), 2853.
2. Misner, C. W., Thorne, K. S., & Wheeler, J. A. (1973). *Gravitation*. W. H. Freeman.
3. Kuchař, K. V. (1992). *Time and interpretations of quantum gravity*. In *Proceedings of the 4th Canadian Conference on General Relativity and Relativistic Astrophysics*.
4. Page, D. N., & Wootters, W. K. (1983). *Evolution without evolution: Dynamics described by stationary observables*. Phys. Rev. D, 27(12), 2885.
5. Rovelli, C. (1991). *Time in quantum gravity: An hypothesis*. Phys. Rev. D, 43(2), 442.

---

If you want, I can now make this into a **proper LaTeX-formatted academic paper** so it looks like a real physics preprint (ready for arXiv).
Do you want me to prepare that?
