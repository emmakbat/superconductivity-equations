# Critical Current
- [Ginzburg-Landau Picture](#ginzburg-landau-picture)

## Ginzburg-Landau Picture
An adaptation of Tinkham's derivation plus some interpretation from the lectures of Christopher L. Henley at Cornell (2011).

The Ginzburg-Landau equations predict a critical current as a consequence of free energy introduced by a gradient in the phase of the order parameter, i.e. a supercurrent enforced by boundary conditions on a phase shift.

A quick digression:
We will assume that the variation of the phase is uniform, which is true provided we are solving for the critical velocity of the superfluid with respect to the frame of a stationary channel within which it flows, and then
computing critical current from there. Per Tinkham, this order of operations is required because GL starts from Helmholtz free energy, i.e. no induced electromotive force, i.e. constant $v_s$. Otherwise we'd need to start
from the Gibbs free energy, and the algebra would be more awkward, but in fact the end result would be the same. So we'll do it this way.

The contribution to free energy from supercurrent flow takes the form of kinetic energy caused by a gradient in the order parameter, so it can be written as:

(1) $F_{grad} = \frac{\hbar^2}{2m_*} |\nabla \Psi|^2$

We can separate the order parameter into its magnitude, i.e. the supercarrier density $n_s$ which we take to be invariant, and its phase $\theta$ which we take to vary. As a result, we rewrite the kinetic energy as

(2) $F_{grad} = \frac{\hbar^2}{2m_*} n_s|\nabla \theta|^2$

The total free energy must be minimized per usual. Taking equation (4) from [Microscopic Theories](#Microscopic-Theories.md) and replacing some constants via relationships, we have:

(3) $F_{grad} + F_{s} - F_{n} = -|\alpha| (1-|\nabla \theta|^2 \xi^2)|\Psi|^2 + \frac{1}{2}\beta |\Psi|^4$

which is minimized under the condition:

(4) $n_s = |\Psi|^2 = (1-|\nabla \theta|^2 \xi^2)n_{s0}$

Therefore we can see that the supercarrier density is decreased as the phase gradient is increased, because the phase gradient increases the free energy of the superconducting state.
As a result, there are competing factors affecting the supercurrent density, which is directly proportional to both phase gradient ("velocity") and supercarrier density; therefore,
$J_s(|\nabla \theta|^2)$ must have some maximum value, i.e. the critical current. We can substitute the phase gradient for $\frac{m* v_s}{\hbar}$ since they play the same role in the 
energy equations.

The resulting supercurrent equation is:

(5) $J_s = 2e|\Psi|^2 v_s = 2en_{s0}^2 (1-\frac{m* v_s^2}{2|\alpha|})v_s$

And this is maximized where $\partial J_s / \partial v_s = 0$:

(6) $J_c = 2e n_{s0}^2\frac{2}{3} (\frac{2|\alpha|}{3m*})^2 = \frac{c H_c(T)}{3\sqrt{6}\pi \lambda(T)}$

So critical current and critical field are related due to their relationship to underlying material properties.

## London Picture

A critical current can be estimated from the London equations by equating kinetic energy density to condensation energy. 

The kinetic energy density is:

(1) $KE = \frac{1}{2} n_s m* v^2$

The London condensation energy is:

(2) $F = \frac{2\pi}{c^2}\lambda^2 J_c^2 = \frac{H_c^2}{8\pi}$

[1] Tinkham, Introduction to Superconductivity.
[2] Henley, Lecture 6.4
