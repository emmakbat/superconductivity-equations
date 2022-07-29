Many equations or sources were found in Di Zhu's thesis [1].

## Energy Gap

The energy gap betweent the superconducting and normal ground states $2\Delta$ is one of
the fundamental features of BCS superconductivity. It is related to $T_c$, which in turn
predicts the temperature dependence of many other important material properties of 
superconductors.

From BCS theory [2]:

$$ \Delta(T \rightarrow 0) = 1.764 k_b T_c $$

$$ \Delta(T \rightarrow T_c) = 3.06 k_b \sqrt{1 - T/T_c} $$

From the literature [3]:

$$ \Delta = 2.15 k_b T_c $$

## Kinetic Inductance

A good estimate from Mattis-Bardeen theory:

$$ L_k = \frac{\hbar}{\pi \Delta} \rho \approx 1.378 \frac{Rs}{Tc} $$

From thin film material properties:

$$ L_k = \mu_0 \lambda_L^2 $$

And in general, we use the sheet kinetic inductance:

$$ L_{ks} = L_k/d $$

Nonlinearity with a small applied current:

$$ L_k(I) = L_k(0) [1 + (I/I^{sw})^2] $$

Nonlinearity with a large bias current $I_b$:

$$ L_k(0, T)/L_k(I_b, T) = \left[1 - \left(\frac{|I_b|}{I_d(T)}\right)^n\right]^{1/n} $$

where $I_d$ is the actual depairing current of the wire, and $n$ is an experimentally 
determined value for each $T/T_c$.

From SPICE simulation of s/c nanowire paper [4] Nonlinearity kinetic inductance current dependance

$$ L_k(i_D) = \dfrac{L_\circ}{2\cos \left(  \frac{2}{3} \arcsin \left( 0.6 \frac{i_D}{I_{SW}}\right) \right) - 1} $$

where $I_{SW}$ is the switching current.


[1] D. Zhu, "Microwave Engineering in Superconducting Nanowires for Single-Photon Detection" (2019).
[https://dspace.mit.edu/handle/1721.1/124123](https://dspace.mit.edu/handle/1721.1/124123)

[2] J. Bardeen, L. N. Cooper, and J. R. Schrieffer, "Theory of Superconductivity" (1957). 
[https://journals.aps.org/pr/abstract/10.1103/PhysRev.108.1175](https://journals.aps.org/pr/abstract/10.1103/PhysRev.108.1175)

[3] A. Semenov, G. Gol’tsman, and A. Korneev, "Quantum detection by current carrying
superconducting film" (2001). 

[4] K. K. Berggren et al., “A superconducting nanowire can be modeled by using SPICE,”
Supercond. Sci. Technol., vol. 31, no. 5, p. 055010, May 2018, doi: 10.1088/1361-6668/aab149.
https://www.rle.mit.edu/qnn/wp-content/uploads/2020/02/A_Superconducting_Nanowire_can_be_Modeled_by_Using_SPICE.pdf
