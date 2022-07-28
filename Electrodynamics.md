## The London Equations [1]

A set of basic constitutive relations for superconductivity.

### London penetration depth

The characteristic length scale of the London equations and many derived models -- typically thought of as the magnetic field
penetration depth for bulk superconductors.

$$ \lambda_L^2 = \frac{m}{n_s \mu_0 e^2} $$

Due to the temperature dependence of $n_s$ (see Material-Properties):

$$ \lambda_L^2(T) = \lambda_L^2(0) [1 - (T/T_c)^4] $$

### Electrodynamics

The current dynamics for a superconductor in the London model are given by:

$$ \vec{J_s} = e n_s \vec{v} $$

where $n_s$ is the Cooper pair (superelectron) density;

$$ \vec{E} = \mu_0 \lambda_L^2 \frac{\partial \vec{J_s}}{\partial t} $$

$$ \nabla \times \vec{J_s} = -\frac{1}{\lambda_L^2} \vec{H} $$

## Modifications to the London Equations

In some cases, the London penetration depth is not an appropriate description of field dynamics, and modifications are given.

### Coherence Length [2]

Similar to the anomalous skin effect in normal metals, there can be nonlocal modifications to the field strength over
a characteristic length called the coherence length $\xi_0$.

$$ \xi_0 = 0.15 \frac{\hbar}{k} \frac{\sqrt{F}}{T_c} $$

We define another parameter $\xi$:

$$ \frac{1}{\xi} = \frac{1}{\xi_0} + \frac{1}{\alpha l} $$

Where $\alpha$ is empirically determined to be about 1, and $l$ is the superelectron mean free path. 
Then there are two limits for the modified penetration depth $\lambda$.

For $\xi << \lambda$:

$$ \lambda =  \lambda_L \sqrt{\frac{\xi_0}{\xi}} $$

For $\xi >> \lambda$:

$$ \lambda = [\frac{\sqrt{3}}{2\pi} \xi_0 \lambda_L^2]^{1/3} $$

### Pearl Length [3]

Thin films (the 2D limit of the London equations) are less effective at screening magnetic field. As a result, the more
appropriate characteristic length scale is the Pearl length $\Lambda$.

$$ \Lambda = \frac{2\lambda^2}{d} $$


[1] F. London, H. London, "The electromagnetic equations of the supraconductor" (1935). 
[https://doi.org/10.1098/rspa.1935.0048](https://doi.org/10.1098/rspa.1935.0048)

[2] A. B. Pippard, "Field variation of the superconducting penetration depth" (1950).
[https://doi.org/10.1098/rspa.1950.0135](https://doi.org/10.1098/rspa.1950.0135)

[3] J. Pearl, "Vortex Theory of Superconducting Memories" (1965).
