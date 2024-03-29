## Ginzburg-Landau [1]

Valid near $T_c$.

(1) $\frac{1}{2m*}(-i\hbar \vec{\nabla} - e^* \vec{A})^2 \Psi + \alpha \Psi + \beta |\Psi|^2 \Psi = 0$

(2) $-\vec{\nabla}^2 \frac{\vec{A}}{\mu_0} = \vec{J_s} = \frac{e^{* 2}}{m^* } [-\vec{A}|\Psi|^2 + \frac{i\hbar}{2e^* } (\Psi^* \vec{\nabla}\Psi - \Psi \vec{\nabla}\Psi^* )]$

where $-\alpha/\beta = |\Psi_0|^2$ and $\alpha^2/\beta = \mu_0 H_c^2$

Equation (2) reduces to the 2nd London Equation if the phase of $\Psi$ is uniform.

Also important is the Ginzburg-Landau free energy [2], which gives the free-energy density of the superconducting state as a function of the above defined variables.

(3) $f = f_{n0}+ \alpha |\Psi|^2+ \frac{\beta}{2} |\Psi|^4+ \frac{1}{2 m*} |(\frac{\hbar}{i} \nabla - \frac{e*}{c} \mathbf{A}) \Psi|^2 + \frac{h^2}{8 \pi}$

If $\Psi =0$, then this reduces to the free energy of the normal state, i.e. the contributions of the first and last terms. The fourth term gives the contributions from gradients and from the electromagnetic field. Without these effects, the energy difference between the superconducting state and the normal state is:

(4) $f_s - f_n = \alpha |\Psi|^2 + \frac{1}{2} \beta |\Psi|^4$

The reason GL theory only works near $T_c$ is because this expansion is sufficient only where the order parameter is small, i.e. where $\beta > 0$. If $\alpha >0$ then free energy is minimized where $|\Psi|^2 = 0$, i.e. in the normal state. If $\alpha < 0$ then the minimum occurs where $|\Psi|^2 = -\alpha/\beta$, which when substituted into the free energy equation yields 
$\frac{-H_c^2}{8\pi} = \frac{-\alpha^2}{2\beta}$, hence the above definitions.

We can actually rewrite the paramters $|\Psi_0|^2$, $\alpha(T)$, and $\beta(T)$ in more practical terms, provided we assign $m*=2m_e$ and $e*=2e$ for our superconducting carriers. 
The latter is easily justifiable theoretically and experimentally, but the former is more complicated since it's really referring to the effective mass of the carriers *within the lattice* 
and will inevitably vary from material to material. Regardless, we conventionally take:

(5) $|\Psi_0|^2 \equiv n_s* = \frac{m_ec^2}{8\pi e^2 \lambda^2_{eff}}$

(6) $\alpha(T) = -\frac{2e^2}{mc^2}H^2_c(T)\lambda^2_{eff}(T)$

(7) $\beta(T) = \frac{16\pi e^4}{m^2c^4}H^2_c(T) \lambda^4_{eff}(T)$

The Ginzburg-Landau coherence length arises from taking the case in which no fields are present, such that $\mathbf{A}=0$ and $\Psi$ therefore is real. Then defining a normalized wavefunction $\psi = \Psi/\Psi_0$, then the equations of motion yield the following:

(8) $\frac{\hbar^2}{2m*|\alpha|}\frac{d^2\psi}{dx^2} + \psi -\psi^3=0$

We take the coefficient on the second-order derivative of the normalized wavefunction as a sort of characteristic length, or a coherence length for the Ginzburg-Landau picture.

(9) $\xi^2_{GL} = \frac{\hbar^2}{2m*|\alpha(T)|}$

This is *not* the same as the Pippard coherence length from our [Electrodynamics](#Electrodynamics.md) discussion, most notably because it diverges at $T_c$. However it will turn out they take on similar values so long as you're well below $T_c$.

We can also define a Ginzburg-Landua penetration depth:

(10) $\lambda^2_{GL} = \frac{m*\beta(T) c^2}{4\pi |\alpha(T)| e*^2}$

And finally, the Ginzburg-Landau parameter, which will later allow us to define Type-I vs Type-II superconductors:

(11) $\kappa = \lambda_{GL}/\xi_{GL}$

## Bardeen-Cooper-Schrieffer

## Relating Different Theories

- $n_s = |\Psi|^2 = \Delta(x)$ and $e* = 2e$ allows derivation of G-L from BCS

[1] Ginzburg, V. L., and Landau, L. D., "On the Theory of Superconductivity" (1950). 
[Chapter 4](https://link.springer.com/content/pdf/10.1007/978-3-540-68008-6.pdf)
[2] Tinkham, "Introduction to Superconductivity" Chapter 4.
