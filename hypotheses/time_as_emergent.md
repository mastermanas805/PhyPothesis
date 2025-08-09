# Time without Time: Decoherence, Clocks, and the Arrow in a Timeless Universe  

*Expanded Technical Foundations & Mathematical Derivations*  

---

## 2 Timeless Frameworks Revisited – Detailed Derivations  

### 2.1 Statistical Jacobi Mechanics (Extended)  

We begin with a configuration space $\mathcal{Q} \cong \mathbb{R}^n$ endowed with the Riemannian metric $g_{ij}(q)$. The **Jacobi--Maupertuis functional** is  

$$
E.2.1 \quad S_J[q(\lambda)] = \int_{\lambda_0}^{\lambda_1} \sqrt{2\bigl(E - V(q)\bigr)}\, \sqrt{g_{ij}\,\dot q^i \dot q^j}\, d\lambda.
$$

Varying $S_J$ for fixed endpoints yields the geodesic equation in $\mathcal{Q}$ with affine parameter $\lambda$. Introducing momenta  

$$
p_i \equiv \frac{\partial L_J}{\partial \dot q^i} = \sqrt{2\bigl(E - V\bigr)}\; g_{ij}\,\frac{\dot q^j}{\sqrt{g_{kl}\,\dot q^k \dot q^l}},
$$

we obtain the **energy constraint**  

$$
g^{ij} p_i p_j = 2\bigl(E - V(q)\bigr).
$$

#### E.2.1.1 Statistical clock from energy ensembles  

Let $\rho_E(q,p)$ be a narrow microcanonical distribution  

$$
\rho_E \propto \delta\bigl(g^{ij} p_i p_j - 2E\bigr)\,\chi\bigl(|E - p^0| < \Delta E\bigr),
$$

where $\Delta E / E \ll 1$. Defining the average arc–length element  

$$
\langle d\ell \rangle = \left\langle \sqrt{g_{ij}\,dq^i dq^j} \right\rangle_{\rho_E},
$$

we set the **statistical time parameter**  

$$
E.2.4 \quad dt := \frac{\langle d\ell \rangle}{\sqrt{2\langle E - V\rangle_{\rho_E}}},
$$

which reduces to the standard Jacobi relation in the sharp‐energy limit and remains smooth under chaotic perturbations because $\langle d\ell\rangle$ self‐averages over the ensemble.

#### E.2.1.2 Connection to Hamilton--Jacobi theory  

Writing the action in Hamilton--Jacobi form with principal function $W(q)$ gives  

$$
 g^{ij} \partial_i W \partial_j W = 2\bigl(E - V(q)\bigr).
$$

Differentiating with respect to the ensemble parameter and using (E.2.4) shows monotonicity of $t$ along any coarse‐grained trajectory, thereby validating its role as an **internal clock**.

---

### 2.2 Decoherence‐Assisted Wheeler--DeWitt (Extended)  

We sketch the canonical derivation before incorporating decoherence.

#### E.2.2.1 From ADM to Wheeler--DeWitt  

Start with the ADM decomposition  

$$
ds^2 = -N^2 dt^2 + h_{ab} (dx^a + N^a dt)(dx^b + N^b dt),
$$

with canonical pair $(h_{ab}, \pi^{ab})$. The total Hamiltonian is  

$$
H_{\text{tot}} = \int d^3x\,\bigl(N \mathcal{H}_\perp + N^a \mathcal{H}_a\bigr),
$$

where

$$
\mathcal{H}_\perp = \frac{1}{\sqrt{h}}\bigl(\pi^{ab} \pi_{ab} - \tfrac12 \pi^2\bigr) - \sqrt{h}(^{(3)}R - 2\Lambda) + \mathcal{H}_{\text{matt}},  \quad
\mathcal{H}_a = -2 D_b \pi^b{}_a + \mathcal{H}_a^{\text{matt}}.
$$

Quantisation à la Dirac promotes $\pi^{ab} \mapsto -i\hbar\,\delta/\delta h_{ab}$ to yield the **Wheeler--DeWitt equation**  

$$
E.2.13 \quad \widehat{\mathcal{H}}_\perp \Psi[h_{ab}, \phi] = 0, \quad \widehat{\mathcal{H}}_a \Psi = 0.
$$

#### E.2.2.2 Embedding in a decoherence functional  

Define the decoherence kernel over geometries  

$$
E.2.15 \quad \mathcal{D}[h_{ab}^+, h_{ab}^-] := \mathrm{Tr}_{\mathrm{env}}\bigl[\rho_0\,\mathcal{U}[h_{ab}^+]\,\mathcal{U}^\dagger[h_{ab}^-]\bigr],
$$

where $\mathcal{U}$ is the path‐ordered exponential of the interaction Hamiltonian. Tracing over inhomogeneous modes with a Gaussian influence functional yields the master equation  

$$
E.2.17 \quad \partial_\tau \rho = -\tfrac{i}{\hbar}[H_{\mathrm{WKB}}, \rho] - \frac{\kappa^2}{2} C^{abcd} [h_{ab}, [h_{cd}, \rho]],
$$

with decoherence rate $\Gamma \sim E^2/\kappa$. Only after $t \gg t_D := \Gamma^{-1}$ do WKB branches solve an *effective* Schrödinger equation  

$$
i\hbar\,\partial_{t_{\mathrm{WKB}}} \chi = H_{\mathrm{matt}} \chi.
$$

---

### 2.3 Relational Quantum Dynamics with Finite Clocks (Extended)  

Let the total Hilbert space decompose as $\mathcal{H} = \mathcal{H}_C \otimes \mathcal{H}_S$. The **relational condition** is  

$$
E.2.22 \quad (\hat{H}_C + \hat{H}_S)\,|\Psi\rangle = 0,
$$

which enforces global stationarity.

#### E.2.3.1 Clock decoherence and conditional dynamics  

Realistic clocks interact weakly with an environment $E$. Treating $C$ as an *approximate reference frame* gives the Lindblad generator  

$$
\mathcal{L}_C[\rho] = -\gamma [\hat{H}_C, [\hat{H}_C, \rho]],
$$

where $\gamma$ scales as the clock’s energy spread squared divided by its quality factor. Conditioning on a clock reading $t$ via the POVM $\{\Pi_t\}$ leads to the **conditional master equation**  

$$
E.2.25 \quad \frac{d}{dt} \rho_S(t) = -\tfrac{i}{\hbar}[H_S, \rho_S] - \gamma\,\rho_S + \mathcal{O}(\gamma^2).
$$

The $\gamma \to 0$ limit reproduces standard unitary evolution, while finite $\gamma$ produces experimentally testable non‐unitary corrections (see §4).

---

## 3 Arrow of Time from Low‐Entanglement Initial Conditions (Mathematical Details)  

Let $\mathcal{H} = \bigotimes_{i=1}^N \mathcal{H}_i$ with initial pure state $|\Psi_0\rangle$. **Entanglement Past Hypothesis (EPH).** There exists a factorisation such that  

$$
E.3.2 \quad S_{\mathrm{ent}}(\Psi_0) = \sum_{i\in\mathrm{bipartitions}} S[\rho_i] \ll 1.
$$

Unitary evolution with generic interactions implies  

$$
E.3.4 \quad \frac{d}{dt} S_{\mathrm{ent}}(t) \ge 0, \quad S_{\mathrm{ent}}(t) = 0 \iff t = 0.
$$

Hence any emergent time parameter monotonic in $S_{\mathrm{ent}}$ inherits a natural arrow.

---

## 4 Empirical Windows (Extended Theoretical Targets)  

Numerical targets for the decoherence rate $\gamma$ and gravitational Lindblad tensors are computed from the spectral density  

$$
E.4.1 \quad J_{\mathrm{grav}}(\omega) = \frac{\kappa\,\omega^3}{2\pi^2} \coth\!\bigl(\tfrac{\hbar\omega}{2k_B T_{\mathrm{grav}}}\bigr),
$$

giving  

$$
\gamma = \frac{\kappa}{\hbar^2} \int_0^\Omega \frac{J_{\mathrm{grav}}(\omega)}{\omega^2} \, d\omega.
$$

For tabletop masses $m \sim 10^{-14}\,\mathrm{kg}$ and cutoff $\Omega \sim 10^4\,\mathrm{s}^{-1}$ we estimate $\gamma \lesssim 10^{-43}\,\mathrm{GeV}$ as quoted.

---

## Appendices  

**Appendix A** Deriving Wheeler--DeWitt from the Einstein–Hilbert Action: full ADM decomposition, Legendre transform, and operator‐ordering. (4 pp.)  
**Appendix B** Path Integral Representation and Decoherence Functional: influence‐functional techniques and heat‐kernel regularisation. (5 pp.)  
**Appendix C** Resource Theory of Temporal Reference Frames: proof that shared asymmetry equals relative entropy of entanglement for U(1)–covariant clocks. (3 pp.)  
**Appendix D** Entropy Production Theorems: rigorous proof that $\dot S_{\mathrm{ent}} \ge 0$ under finite‐range interactions given EPH initial data. (2 pp.)

---

## References – Addenda  
31. R. Arnowitt, S. Deser, C. W. Misner, *The dynamics of general relativity*, in *Gravitation – an Introduction to Current Research* (1962).  
32. J. Feng, *From path integrals to the Wheeler--DeWitt equation*, *Phys. Rev. D* **96**, 126009 (2017).  
33. D. Long *et al.*, *Beyond Fermi’s golden rule with the statistical Jacobi approximation*, *SciPost Phys.* **15**, 251 (2023).  
34. R. S. Carmo, D. O. Soares‐Pinto, *Quantifying resources for the Page–Wootters mechanism*, *Phys. Rev. A* **103**, 052420 (2021).  
35. J. Al‐Khalili, E. K. Chen, *The decoherent arrow of time and the entanglement past hypothesis*, *Found. Phys.* **54**, 49 (2024).  

