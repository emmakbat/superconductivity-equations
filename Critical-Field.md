# Critical Field

## The Simple Version

It was proposed by Chandresekhar [1] that superconductivity should be broken when the magnetic energy surpasses the superconducting energy gap, that is:

(1) $H_c = \Delta/2\mu$

Where $\mu$ is the Bohr magneton. This prediction is correct within order of magnitude in bulk alloy superconductors such as NbTi.

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
