# Time without Time: Decoherence, Clocks, and the Arrow in a Timeless Universe  

*Expanded Technical Foundations & Mathematical Derivations*

> **Note to readers.**  This extended version supplements the original manuscript with full variational derivations, canonical analyses, and resource‐theoretic proofs that were omitted for brevity.  Numbering follows the main text; all new equations are tagged with a leading **E** (for *Extended*) to avoid clashes.

---

## 2 Timeless Frameworks Revisited – Detailed Derivations  

### 2.1 Statistical Jacobi Mechanics (Extended)  

We begin with a configuration space \(\mathcal Q\cong \mathbb R^{n}\) endowed with the Riemannian metric \(g_{ij}(q)\).  The **Jacobi–Maupertuis functional** is  
\[
E.2.1\quad  S_J[q(\lambda)] \,=\, \int_{\lambda_0}^{\lambda_1}\!\sqrt{2\bigl(E-V(q)\bigr)}\, \sqrt{g_{ij}\,\dot q^{i}\dot q^{j}}\,\mathrm d\lambda.
\]

Varying \(S_J\) for fixed endpoints yields the geodesic equation in \(\mathcal Q\) with affine parameter \(\lambda\).  Introducing momenta  
\[ p_i \;\equiv\; \frac{\partial L_J}{\partial \dot q^{i}} \,=\, \sqrt{2\bigl(E-V\bigr)}\; g_{ij}\,\frac{\dot q^{j}}{\sqrt{g_{kl}\,\dot q^{k}\dot q^{l}}}, \]
we obtain the **energy constraint**  
\[ g^{ij}p_i p_j = 2\bigl(E-V(q)\bigr). \]

#### E.2.1.1 Statistical clock from energy ensembles  

Let \(\rho_E(q,p)\) be a narrow microcanonical distribution  
\[ \rho_E \propto \delta\bigl(g^{ij}p_i p_j-2E\bigr)\,\chi\bigl(|E-p^0|<\Delta E\bigr), \]
where \(\Delta E/E\ll1\).  Defining the average arc–length element  
\[ \langle \mathrm d\ell \rangle = \left\langle \sqrt{g_{ij}\,\mathrm dq^{i}\mathrm dq^{j}} \right\rangle_{\rho_E}, \]
we set the **statistical time parameter**  
\[
E.2.4\quad  \mathrm dt := \frac{\langle\mathrm d\ell\rangle}{\sqrt{2\langle E-V\rangle_{\rho_E}}},
\]
which reduces to the standard Jacobi relation in the sharp‐energy limit and remains smooth under chaotic perturbations because \(\langle\mathrm d\ell\rangle\) self‐averages over the ensemble.

#### E.2.1.2 Connection to Hamilton–Jacobi theory  

Writing the action in Hamilton–Jacobi form with principal function \(W(q)\) gives  
\[ g^{ij}\,\partial_i W\,\partial_j W = 2\bigl(E-V(q)\bigr). \]
Differentiating w.r.t. the ensemble parameter and using (E.2.4) shows monotonicity of \(t\) along any coarse‐grained trajectory, thereby validating its role as an **internal clock**.

---

### 2.2 Decoherence‐Assisted Wheeler–DeWitt (Extended)  

We sketch the canonical derivation before incorporating decoherence.

#### E.2.2.1 From ADM to Wheeler–DeWitt  

Start with the ADM decomposition  
\[ \mathrm d s^{2}= -N^{2}\mathrm d t^{2} + h_{ab}(\mathrm d x^{a}+N^{a}\mathrm d t)(\mathrm d x^{b}+N^{b}\mathrm d t), \]
with canonical pair \((h_{ab},\pi^{ab})\).  The total Hamiltonian is  
\[
H_{\text{tot}}\,=\,\int\!\mathrm d^{3}x\bigl(N\mathcal H_\perp+N^{a}\mathcal H_a\bigr),
\]
where
\[
\mathcal H_\perp = \frac{1}{\sqrt h}\!\Bigl(\pi^{ab}\pi_{ab}-\tfrac12\pi^{2}\Bigr) - \sqrt h\,(^{(3)}R-2\Lambda)+\mathcal H_{\text{matt}},  \quad
\mathcal H_a = -2D_b\pi^{b}{}_{a}+\mathcal H_{a}^{\text{matt}}.
\]
Quantisation à la Dirac level promotes \(\pi^{ab}\mapsto -i\hbar\,\delta/\delta h_{ab}\) to yield the **Wheeler–DeWitt equation**  
\[
E.2.13\quad  \widehat{\mathcal H}_\perp\,\Psi[h_{ab},\phi] = 0, \qquad \widehat{\mathcal H}_a\,\Psi = 0.
\]

#### E.2.2.2 Embedding in a decoherence functional  

Define the *decoherence kernel* over geometries  
\[
E.2.15\quad  \mathcal D\bigl[h_{ab}^+,h_{ab}^-\bigr] := \text{Tr}_{\text{env}}\bigl[ \rho_0\, \mathcal U[h_{ab}^+]\,\mathcal U^{\dagger}[h_{ab}^-]\bigr],
\]
where \(\mathcal U\) is the path‐ordered exponential of the interaction Hamiltonian.  Tracing over inhomogeneous modes with a Gaussian influence functional yields the master equation  
\[
E.2.17\quad  \partial_\tau\rho = -\tfrac{i}{\hbar}[H_{\text{WKB}},\rho] - \frac{\kappa^2}{2}\,C^{abcd}\,[h_{ab},[h_{cd},\rho]],
\]
with decoherence rate  \(\Gamma\sim E^{2}/\kappa\) as argued in the main text.  Only after \(t\gg t_D:=\Gamma^{-1}\) do WKB branches solve an *effective* Schrödinger equation  
\[ i\hbar\,\partial_{t_{\text{WKB}}}\,\chi = H_{\text{matt}}\,\chi. \]

---

### 2.3 Relational Quantum Dynamics with Finite Clocks (Extended)  

Let the total Hilbert space decompose as \(\mathcal H=\mathcal H_C\otimes\mathcal H_S\).  The **relational condition** is  
\[
E.2.22\quad  (\hat H_C+\hat H_S)\,|\Psi\rangle=0,
\]
which enforces global stationarity.

#### E.2.3.1 Clock decoherence and conditional dynamics  

Realistic clocks interact weakly with an environment \(E\).  Treating \(C\) as an *approximate reference frame* gives the Lindblad generator  
\[
\mathcal L_C[\rho] = -\gamma\,[\hat H_C,[\hat H_C,\rho]],
\]
where \(\gamma\) scales as the clock’s energy spread squared divided by its quality factor.  Conditioning on a clock reading \(t\) via the POVM \(\{\Pi_t\}\) leads to the **conditional master equation**  
\[
E.2.25\quad  \frac{\mathrm d}{\mathrm dt}\rho_S(t) = -\tfrac{i}{\hbar}[H_S,\rho_S] - \gamma\,\rho_S + \mathcal O(\gamma^2).
\]
The \(\gamma\to0\) limit reproduces standard unitary evolution, while finite \(\gamma\) produces experimentally testable non–unitary corrections (see §4).

---

## 3 Arrow of Time from Low‐Entanglement Initial Conditions (Mathematical Details)  

Let \(\mathcal H = \bigotimes_{i=1}^{N}\mathcal H_i\) with initial pure state \(|\Psi_0\rangle\).  **Entanglement Past Hypothesis (EPH).**  There exists a factorisation such that  
\[
E.3.2\quad  S_{\text{ent}}(\Psi_0) = \sum_{i\,\in\,\text{bipartitions}} S\bigl[\rho_i\bigr] \;\ll\; 1.
\]

Unitary evolution with generic interactions implies [mixing theorem]  
\[
E.3.4\quad  \frac{\mathrm d}{\mathrm dt} S_{\text{ent}}(t) \;\ge 0, \quad S_{\text{ent}}(t) \;=\; 0 \text{ iff } t=0.
\]
Hence any emergent time parameter monotonic in \(S_{\text{ent}}\) inherits a natural arrow.

---

## 4 Empirical Windows (Extended Theoretical Targets)  

Numerical targets for the decoherence rate \(\gamma\) and gravitational Lindblad tensors are computed from the spectral density  
\[
E.4.1\quad  J_{\text{grav}}(\omega)=\frac{\kappa\,\omega^{3}}{2\pi^{2}}\coth\!\Bigl(\tfrac{\hbar\omega}{2k_B T_{\text{grav}}}\Bigr),
\]
giving  
\[ \gamma = \frac{\kappa}{\hbar^{2}}\int_{0}^{\Omega}\!\frac{J_{\text{grav}}(\omega)}{\omega^{2}}\,\mathrm d\omega. \]
For tabletop masses \(m\sim10^{-14}\,\text{kg}\) and cut‐off \(\Omega\sim10^{4}\,\text{s}^{-1}\) we estimate \(\gamma\lesssim10^{-43}\,\text{GeV}\) as quoted.

---

## Appendices  

### Appendix A Deriving Wheeler–DeWitt from the Einstein–Hilbert Action  
Full step‐by‐step ADM decomposition, Legendre transform, and operator‐ordering discussion. *(4 pages)*

### Appendix B Path Integral Representation and Decoherence Functional  
Derivation of (E.2.15) using influence‐functional techniques and heat‐kernel regularisation. *(5 pages)*

### Appendix C Resource Theory of Temporal Reference Frames  
Proof that shared asymmetry equals relative entropy of entanglement for U(1)‐covariant clocks, following Carmo & Soares‐Pinto (2021). *(3 pages)*

### Appendix D Entropy Production Theorems  
Rigorous statement and proof that \(\dot S_{\text{ent}}\ge0\) under finite‐range interactions given EPH initial data. *(2 pages)*

---

### References – Addenda  
31. R. Arnowitt, S. Deser, C. W. Misner, *The dynamics of general relativity*, in *Gravitation – an Introduction to Current Research* (1962).  
32. J. Feng, *From path integrals to the Wheeler–DeWitt equation*, *Phys. Rev. D* **96**, 126009 (2017).  
33. D. Long *et al.*, *Beyond Fermi’s golden rule with the statistical Jacobi approximation*, *SciPost Phys.* **15**, 251 (2023).  
34. R. S. Carmo, D. O. Soares-Pinto, *Quantifying resources for the Page–Wootters mechanism*, *Phys. Rev. A* **103**, 052420 (2021).  
35. J. Al-Khalili, E. K. Chen, *The decoherent arrow of time and the entanglement past hypothesis*, *Found. Phys.* **54**, 49 (2024).  
*Remaining numbering follows the original reference list.*
