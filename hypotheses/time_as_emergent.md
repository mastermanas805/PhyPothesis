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


# 4. Addressing Major Criticisms (mathematical & conceptual fixes)

This section answers the reviewer’s main complaints by (i) giving explicit derivations linking frameworks, (ii) exposing and quantifying failure modes (clock imperfection, non-monotonic cosmologies), and (iii) placing the thermodynamic arrow inside the timeless formalism while admitting the remaining open questions.

---

## 4.1 Emergent WKB time — explicit minisuperspace derivation

**Set-up (minisuperspace):**
Consider a homogeneous, isotropic minisuperspace with scale factor $a$ and a homogeneous scalar field $\phi$ (working in units where constants may be set to 1 for clarity). A schematic Wheeler–DeWitt (WDW) equation takes the form

$$
\hat{\mathcal{H}}\Psi(a,\phi)=\bigl(\hat{\mathcal{H}}_{\text{grav}}(a,\partial_a)+\hat{\mathcal{H}}_{\text{matt}}(a,\phi,\partial_\phi)\bigr)\Psi(a,\phi)=0.
$$

For our purpose write it as the simplified model

$$
\Bigl(-\frac{\hbar^2}{2M_G}\partial_a^2 + U(a) + \hat H_{\rm m}(a,\phi)\Bigr)\Psi(a,\phi)=0,
$$

where $M_G$ is an effective gravitational inertia, $U(a)$ a gravitational potential term, and $\hat H_{\rm m}$ the matter Hamiltonian (which may depend parametrically on $a$).

**WKB ansatz:**
Seek a WKB form

$$
\Psi(a,\phi)=e^{\tfrac{i}{\hbar}S_0(a)}\,\chi(a,\phi),
$$

with $S_0$ large (classical gravity) and $\chi$ slowly varying in $\hbar$.

**Insert ansatz and expand.** Substituting into the WDW equation and separating orders of $\hbar$:

* $O(\hbar^0)$ (leading order, Hamilton–Jacobi for gravity):

  $$
  \frac{1}{2M_G}\bigl(S_0'(a)\bigr)^2 + U(a)=0,
  $$

  which is the classical Hamilton–Jacobi relation for the gravitational degree of freedom.

* $O(\hbar^1)$ (next order, evolution for matter):

  $$
  -\frac{i}{M_G}S_0'(a)\,\partial_a \chi(a,\phi) + \hat H_{\rm m}(a,\phi)\,\chi(a,\phi) + \mathcal{O}(\hbar) =0.
  $$

  Rearranging and defining an emergent derivative along the gravitational trajectory,

  $$
  i\hbar \frac{\partial \chi}{\partial t_{\rm WKB}} \equiv i\hbar \frac{1}{M_G} S_0'(a)\,\partial_a \chi = \hat H_{\rm m}(a,\phi)\,\chi,
  $$

  we identify the emergent **WKB time** $t_{\rm WKB}$ up to a normalization constant via

  $$
  \frac{\partial}{\partial t_{\rm WKB}} \equiv \frac{1}{M_G}S_0'(a)\,\partial_a.
  $$

**Interpretation:** $S_0'(a)$ is proportional to the classical momentum conjugate to $a$; the WKB time derivative is generated by the gravitational momentum and maps the stationary WDW equation into an effective Schrödinger equation for matter fields when gravity is semiclassical. This is the standard route in canonical quantum gravity, but here the steps are explicit and the emergent time is identified as a functional of the gravitational action $S_0$.

**Caveats:** the derivation requires (a) a clear Born–Oppenheimer separation between heavy (gravity) and light (matter) degrees of freedom, (b) a WKB (small $\hbar$) regime where $S_0$ varies rapidly, and (c) negligible backreaction of matter on $S_0$ at leading order. When these fail (deep quantum gravity, highly entangled matter–geometry states), $t_{\rm WKB}$ ceases to be a good clock.

---

## 4.2 Explicit toy connecting Jacobi-time, WKB-time and Page–Wootters

We now show, in a controlled toy setting, how the three time notions correspond in the semiclassical limit.

**Classical Jacobi identity (recall):** For a 1-D conservative system with action variable $W(q_1,q_2;E)=\int p(q;E)\,dq$,

$$
\frac{\partial W}{\partial E} = \Delta t,
$$

so classically $t$ is the derivative of the reduced action w\.r.t. energy.

**Semiclassical gravity ↔ Jacobi:** the WKB function $S_0$ from the minisuperspace HJ equation is precisely Hamilton’s principal function (action) for the gravitational sector. Thus $\partial S_0/\partial E_g$ (if one labels solutions by gravitational energy $E_g$) recovers the classical gravitational time parameter in the same way Jacobi’s relation does for finite systems.

**Page–Wootters toy (finite model):** Take clock $C$ with Hamiltonian $\hat H_C$ (spectrum $\{E_n\}$) and system $S$ with Hamiltonian $\hat H_S$. Impose the global constraint $(\hat H_C+\hat H_S)|\Psi\rangle=0$. One solution is the entangled stationary state

$$
|\Psi\rangle = \sum_n c_n\,|E_n\rangle_C\otimes|\psi_{-E_n}\rangle_S,
$$

where $|\psi_{-E_n}\rangle_S$ are system states correlated so the total energy is zero. Now define clock pointer states $|t\rangle_C$ by

$$
|t\rangle_C := \sum_n e^{-iE_n t/\hbar}\,|E_n\rangle_C
$$

(formal Fourier transform). The conditional system state is

$$
|\psi(t)\rangle_S \propto {}_C\langle t|\Psi\rangle = \sum_n c_n e^{-iE_n t/\hbar}\,|\psi_{-E_n}\rangle_S,
$$

which evolves according to $i\hbar\partial_t |\psi(t)\rangle = \hat H_S|\psi(t)\rangle$ whenever the $|\psi_{-E_n}\rangle$ are energy eigenstates of $\hat H_S$ with eigenvalues $-E_n$. In the semiclassical limit where the clock’s spectrum is dense and peaked (like a heavy gravitational background), the Page–Wootters conditional evolution reproduces the same Schrödinger evolution obtained from the WKB procedure.

**Summary:** Jacobi’s $\partial W/\partial E$ ↔ WKB $ \partial S_0/\partial(\text{grav.\ energy})$ ↔ Page–Wootters conditional $t$ all become the same effective parameter when (i) one degree of freedom is heavy/classical, (ii) the action $S_0$ is sharply peaked (WKB), and (iii) the clock subsystem has a sufficiently dense spectrum to provide a quasi-continuous label $t$.

---

## 4.3 The Past Hypothesis and low-entropy boundary conditions

**Problem statement (reviewer):** simply showing that $S(\tau)$ typically increases is not enough — a timeless theory must explain why initial (low-entropy) conditions are realized.

**Response (status & formalization):**

* In a timeless formalism one still needs a *measure* or a *boundary condition* on the space of histories (or wavefunction of the universe). The Past Hypothesis (low-entropy boundary) can be rephrased as a boundary condition on configuration space or on the WDW wavefunctional: choose $\Psi$ that gives high amplitude to configurations corresponding to low coarse-grained entropy at one “end” of the solution manifold. Concretely:

  $$
  \Psi[\text{config}] \;\text{peaked on low-}S\ \text{configurations at the chosen boundary surface}.
  $$
* Well-known examples: Hartle–Hawking no-boundary and Vilenkin tunnelling proposals impose boundary conditions on $\Psi$ that select particular histories. One may augment these proposals with an additional low-entropy selection rule; the justification for such a rule is arguably outside the mathematical formalism (it may be anthropic, dynamical, or a deeper law).
* **Honest assessment:** the need for a low-entropy boundary is real and not solved here. What the emergent-time program offers is a consistent mathematical setting in which such a boundary condition is expressed (as a selection of measure or wavefunctional), and where entropy increase follows for typical coarse-graining given that boundary. The *origin* of the Past Hypothesis remains an open foundational question.

---

## 4.4 Imperfect clocks, interactions, and quantitative corrections

**Ideal vs realistic clocks:** Page–Wootters and the WKB derivation assume “good” clocks: a subsystem with a dense spectrum, small quantum uncertainty in its pointer variable, and negligible interaction with the system being timed. Real clocks violate these assumptions; we now quantify leading corrections.

**Clock with finite energy spread $\Delta E_C$:** suppose the clock state has energy uncertainty $\Delta E_C$. Informally, the conditional Schrödinger evolution acquires corrections of order $\hbar/\Delta E_C$. A common perturbative estimate (see literature on clock-induced decoherence) yields:

* The conditional evolution for the system has additional nonunitary terms scaling like $(H_{\rm int})^2/(\hbar^2\Delta E_C)$, where $H_{\rm int}$ is the clock–system interaction. This produces an effective decoherence rate

  $$
  \Gamma \sim \frac{\langle H_{\rm int}^2\rangle}{\hbar^2\,\Delta E_C}.
  $$
* For weak coupling and large $\Delta E_C$ the corrections are tiny; for small, poorly resolved clocks they are significant.

**Operational consequence:** any proposed laboratory test must estimate $\Delta E_C$, $H_{\rm int}$, and required sensitivity. The scaling above gives a direct way to translate experimental sensitivity into limits on emergent-time deviations.

**References / known results:** Several works (see e.g. discussions by Gambini, Porto & Pullin; and by Peres/Brukner et al.) quantify such decoherence from imperfect clocks. I can fetch and append precise citations if you want.

---

## 4.5 Cosmology: clock monotonicity and multiple-clock strategy

**Scalar clock monotonicity:** using a scalar field $\phi$ as a relational clock works when $\phi$ is monotonic along the histories of interest (e.g. kinetic-dominated regimes). Failure modes:

* Near turning points (bounce/recollapse) $\phi(t)$ may stop being monotonic, invalidating it as a global clock.
* Field fluctuations and backreaction can spoil monotonicity locally.

**Strategy:** adopt a *patchwise* clocking method — use different internal clocks in different regimes, and stitch conditional descriptions together where overlapping regions allow consistent matching. This is analogous to coordinate patches on a manifold: no single global parameter may exist, yet physics is consistently described patchwise.

---

## 4.6 Causal order, manifold embedding, and Malament-type results

**What the reviewer wanted:** a real account of when a partial causal order $(E,\prec)$ can be embedded into a manifold with a metric and a time coordinate.

**Short answer:** results in the causal-structure literature show that, under appropriate technical conditions, the causal order + a suitable volume measure determine the spacetime geometry up to local conformal factors (see Malament-type theorems). In practice:

* Not every discrete partial order is manifold-like (this is the central challenge in causal set theory).
* Embedding a causal set into a Lorentzian manifold requires "manifold-likeness" criteria (e.g. sprinkling, approximate local finiteness).
* **Conclusion for emergent time:** macroscopic temporal ordering from a partial order is plausible and mathematically supported under reasonable regularity conditions — but the embedding problem is nontrivial and must be checked case-by-case.

---

## 4.7 Summary of this corrected/expanded section

1. The WKB minisuperspace derivation shows exactly how a gravitational action $S_0$ defines an emergent $t_{\rm WKB}$; the derivation above fills the reviewer's demand for explicit algebra.
2. The toy construction shows how Jacobi, WKB and Page–Wootters times become the same effective parameter in the semiclassical/heavy-clock limit. This is not a mysterious coincidence — it is the classical limit of action-based dynamics.
3. The Past Hypothesis remains a necessary boundary condition in any framework that recovers a macroscopic arrow; emergent-time formulations move the locus of the problem into boundary selection rather than eliminating it.
4. Imperfect clocks produce quantitative, testable deviations; we gave scaling relations that allow experimental design and falsifiability estimates.
5. Cosmological clock failures (nonmonotonicity) are real but manageable by patchwise clocks.
6. Embedding causal partial orders into manifolds is an active mathematical problem but has well-understood sufficient conditions and important theorems (so the approach is not handwavy — it needs technical checking for any proposed model).

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
