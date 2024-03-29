# Material Properties

- [Energy Gap](#energy-gap)
- [Kinetic Inductance](#kinetic-inductance)
  - [Sheet, unit and lumped inductance](#kinetic-inductance)
  - [Current Non-Linearity of Kinetic Inductance](#current-non-linearity-of-kinetic-inductance)
  - [Temperature dependance of Kinetic Inductance](#temperature-dependance-of-kinetic-inductance)
- [Cooper pair density](#cooper-pair-density)
- [Critical current](#critical-current)

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

(note on notation: $L_k'$ is unit inductance, as in a transmission line;
$L_k$ is lumped element inductance, as in a circuit)

> Analogy for sheet ($L_{k, sh}=L_k^\square$) vs lumped element ($L_k$) vs unit ($L_k'$) inductance with resistance analogues.
> $L_k \sim R = \rho \dfrac{l}{wt}$, $L_k^\square \sim R^\square = \dfrac{\rho}{t}$ and $L_k' \sim R' = \dfrac{R}{l} = \dfrac{\rho}{wt}$.
> Therefore since $R^\square = w R'$ then $L_k' = \dfrac{L_k^\square}{w}$

A good estimate from Mattis-Bardeen theory:

$$ L_k' \approx \frac{\hbar}{\pi \Delta} \rho $$

$$ L_{k, sh} \approx 1.378 \frac{Rs}{Tc} $$

From thin film material properties:

$$ L_k' = \mu_0 \lambda_L^2 $$

And in general, we use the sheet kinetic inductance:

$$ L_{ks} = L_k'/d $$

### Current Non-Linearity of Kinetic Inductance

Nonlinearity with a small applied current:

$$ L_k'(I) = L_k'(0) [1 + (I/I^{sw})^2] $$

Nonlinearity with a large bias current $I_b$:

$$ L_k'(0, T)/L_k'(I_b, T) = \left[1 - \left(\frac{|I_b|}{I_d(T)}\right)^n\right]^{1/n} $$

where $I_d$ is the actual depairing current of the wire, and $n$ is an experimentally 
determined value for each $T/T_c$.

From SPICE simulation of s/c nanowire paper [4] Nonlinearity kinetic inductance current dependance

$$ L_k(i_D) = \dfrac{L_\circ}{2\cos \left(  \frac{2}{3} \arcsin \left( 0.6 \frac{i_D}{I_{SW}}\right) \right) - 1} $$

where $I_{SW}$ is the switching current and $L_\circ$ is the zero-current inductance of the wire.

### Temperature dependance of Kinetic Inductance

Ginzburg-Landau (GL) theory temperature dependance of cooper pair density effect on kinetic inductance - works
in 1D for $T$ near $T_c$ and $I\approx 0$ [5]:

$$ L_k(T) = L_k(0) \left ( \dfrac{1}{1-T/T_c} \right )$$

Or expressed in terms of the GL magnetic penetration depth $\lambda$ [5]:

$$ L_k(T) = \mu_0 \left(\lambda\left(T\right)\right)^2 \left ( \dfrac{l}{wd}\right ) $$

## Cooper pair density

Temperature dependence of the Cooper pair density [5]:

$$ n_s(T) \approx n_s(0) \left( 1 - \dfrac{T}{T_c}\right)$$

## Critical current

Critical current dependance on temperature [6]:

$$ I_c(T) = I_c(0) \left (  1 - \left( \dfrac{T}{T_c} \right )^2 \right )^2$$

## References

[1] D. Zhu, "Microwave Engineering in Superconducting Nanowires for Single-Photon Detection" (2019).
[https://dspace.mit.edu/handle/1721.1/124123](https://dspace.mit.edu/handle/1721.1/124123)

[2] J. Bardeen, L. N. Cooper, and J. R. Schrieffer, "Theory of Superconductivity" (1957). 
[https://journals.aps.org/pr/abstract/10.1103/PhysRev.108.1175](https://journals.aps.org/pr/abstract/10.1103/PhysRev.108.1175)

[3] A. Semenov, G. Gol’tsman, and A. Korneev, "Quantum detection by current carrying
superconducting film" (2001). 

[4] K. K. Berggren et al., “A superconducting nanowire can be modeled by using SPICE,”
Supercond. Sci. Technol., vol. 31, no. 5, p. 055010, May 2018, doi: 10.1088/1361-6668/aab149.
https://www.rle.mit.edu/qnn/wp-content/uploads/2020/02/A_Superconducting_Nanowire_can_be_Modeled_by_Using_SPICE.pdf

[5] A. J. Annunziata et al., “Tunable superconducting nanoinductors,” Nanotechnology, vol. 21, no. 44, p. 445202, Nov. 2010, doi: 10.1088/0957-4484/21/44/445202. 
https://arxiv.org/pdf/1007.4187.pdf

[6] J. K. W. Yang, A. J. Kerman, E. A. Dauler, V. Anant, K. M. Rosfjord, and K. K. Berggren, “Modeling the Electrical and Thermal Response of Superconducting Nanowire Single-Photon Detectors,” IEEE Transactions on Applied Superconductivity, vol. 17, no. 2, pp. 581–585, Jun. 2007, doi: 10.1109/TASC.2007.898660.
https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4277823

