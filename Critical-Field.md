# Critical Field

## The Simple Version

It was proposed by Chandresekhar [1] that superconductivity should be broken when the magnetic energy surpasses the superconducting energy gap, that is:

(1) $H_c = \Delta/2\mu$

Where $\mu$ is the Bohr magneton. This prediction is correct within order of magnitude in bulk alloy superconductors such as NbTi.

## Thermodynamical Critical Field

As outlined by Huh [2], the reversible Meissner effect (perfect diamagnetism) allows us to use thermodynamics to describe superconductivity. We can compute the thermodynamic critical field by integrating the magnetization curve as a function of magnetism. In terms of Gibbs free energy, this turns out to be:

(1) $-\int{MdH}=G_n-G_s=H_c^2/8\pi$

This definition still seems tautological to me, but it turns out this can be written more clearly by BCS theory:

(2) $H_c(0) = \sqrt{4\pi N(0)} \Delta(0)$

Where $N(0)$ is the electronic density of states for a system of unit volume. This is kind of like the simple version, but now we include density of states. This is related to a measurable quantity,
the electronic specific heat coefficient, which is related to normal-state electronic specific heat as $C_{en} = \gamma T$:

(3) $\gamma = \frac{2}{3} \pi^2 N(0) k^2_B$

We can rewrite equation (2) to yield:

(4) $H_c(0)/T_c = \sqrt{\frac{6}{\pi} \gamma} (\Delta(0)/k_bT_c) = 1.76 \sqrt{\frac{6}{\pi} \gamma}$

assuming BCS theory.

To me, it's interesting to note that the critical field is not a totally fundamental material property, but is a consequence of two properties of the band structure, $N(0)$ and $\Delta(0)$.

## Ginzburg-Landau Parallel Field in Thin Films

We assume that at the critical field a thin film undergoes a second-order phase transition such that the order parameter goes to zero and the screening length goes to infinity.
As a result, the gauge choice allows us to set $\mathbf{A} = A_y \approx Hx$ for some applied field magnitude $H$. The phase and amplitude of the order parameter will be constant
with this gauge choice. Per Tinkham, minimizing the Gibbs free energy per unit area gives us this amplitude.

(1) $|\Psi|^2 = \Psi^2_0 (1 - \frac{d^2H^2}{24 \lambda(H=0)^2 H^2_c})$

The film is normal, by definition, when $|\Psi|^2=0$, that is,

(2) $H_{c||} = 2\sqrt{6}\frac{H_c \lambda}{d}$

We observe enhancement of the parallel critical field above the thermodynamic critical field for thin films.

## Type II Superconductors in Ginzburg-Landau

Tinkham defines $H_{c2}$ as "the highest field at which superconductivity can nucleate in the interior of a large sample in a decreasing external field." From this definition,
one can derive from the GL equations:

(1) $H_{c2} = \frac{\Phi_0}{2\pi\xi_{GL}^2(T)} = \sqrt(2)\kappa H_c$

With $\kappa$ being the ratio between the GL coherence length and penetration depth. So for $\kappa < 1/\sqrt{2}$ we have $H_{c2} < H_c$ (Type I), otherwise $H_{c2} > H_c$ (Type II).
Due to the way this was derived, it gives the perpendicular critical field.

[1] Chandrasekhar, APL 1962.

[2] Huh, Thesis. Iowa State University, 2001.
