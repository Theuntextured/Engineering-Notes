> [!important]+ Charge
> Quantized property, incrementing in order $q_{e}=1.602\times 10^{-19}C$ which is always conserved in a closed system.
> Net charge of matter is EXACTLY zero.
> It does NOT depend on relativistic speed.

$$
\vec{F}_{1\to_{2}}=-\vec{F}_{2\to_{1}}=k \frac{Q_{1}Q_{2}}{r^2}u_{r_{1}}=\vec{E}q
$$
$$
\vec{E}=\frac{kQ}{r^2} \vec{u}_{r}
$$

$$
\vec{E}_{TOT}=\Sigma \vec{E}_{i}
$$

“Electrostatic” means that charges are stationary with respect to a reference frame.

> [!check]+ Electrostatic Field Properties
> - Central Force
> - Conservative Force
> - [[Gauss Law]] holds
> - NOT an acceleration field, since charge does not depend on mass
> - Has a [[Physics II/Electrostatics#Electrostatic Potential\|scalar potential]] associated
> - Force can be attractive or repulsive
> - Radial
> - Measured in $NC^{-1}$
> - A charge is needed to measure it

If the path is closed, then:

$$
\begin{align}
&\vec{A}=\vec{B} \\
&\implies \oint \vec{E}\cdot d\vec{s}=0
\end{align}
$$
Since electrostatic force is conservative.

### Hollow Charged Sphere
If we have a hollow sphere of radius $R$ with uniform charge on the surface (total charge is $Q$, $Q_{\text{inner}}=0$), at a distance $r$ from the centre of the sphere, we get two scenarios:

When $r\leq R$:
$$
\begin{align}
&E=0 \\
&V=k \frac{Q}{R}
\end{align}
$$
And when $r>R$ the sphere acts like a point charge at its centre, so laws below hold.

## Electrostatic Potential
$V_{es}$ with unit $V$. Can be used to find forces and field.

$$
\begin{align}
&\vec{E}=\frac{F}{q} \\
&\vec{F}=-\nabla U \\
&U=-\int \vec{F}\cdot d\vec{s} \\
&V_{es}=\frac{U}{q} \\
&\vec{E}=-\nabla V_{es} \\
&V_{es}=-\int \vec{E}\cdot d\vec{s} \\
&V_{TOT}=\Sigma V_{i}
\end{align}
$$
Potential difference:
$$
\Delta V_{AB}=-\int_{A}^B\vec{E}\cdot d\vec{s}=V_{A}-V_{B}
$$
---
# Gauss' Law

> [!warning]+ DEFINITION
> For a charge INSIDE a CLOSED surface generating an electrostatic field, we have [[Physics II/Fields#Flux\|flux]]:
> $$
> \Phi_{\vec{E}}=\oint_{S}\vec{E}\cdot d\vec{S}=\frac{Q}{\varepsilon_{0}}
>$$
> However, if the charge is outside the closed surface, we get:
> $$\Phi_{\vec{E}}=0$$


## Infinite Wire
Assume an infinite cylinder with charge density $\lambda=\frac{dq}{dL}$. We then have an IMAGINARY Gaussian surface as a cylinder with radius $r$ and length $h$ with central axis aligned with the wire.

$$
\implies Q=\lambda h
$$
On the top and bottom lids, $\Phi_{\vec{E}}=0$, while on the side walls:

$$
\begin{align}
&\Phi_{\vec{E}}=2E\pi rh=4k\lambda h\pi \\
&V_{es}=\text{const}-2j\lambda \ln r
\end{align}
$$
## Infinite Plane
Assume an infinite plane with charge density $\sigma$ ($[\sigma]=Cm^{-2}$). We then have a Gaussian surface being a cylinder cutting perpendicularly through the plane.

On the side walls, $\Phi_{\vec{E}}=0$, while on the taps:

$$
\Phi_{\vec{E}}=2ES={\frac{\sigma S}{\varepsilon_{0}}}=\frac{Q}{\varepsilon_{0}}
$$
Inside the cylinder,

$$
\begin{align}
&\vec{E}=\frac{\sigma}{2\varepsilon_{0}}\vec{u}_{\perp} \\
&\implies V_{es}=0
\end{align}
$$
## Summary

| Geometry                        | Field Formula                            |
| ------------------------------- | ---------------------------------------- |
| Point Charge / Sphere (Outside) | $E=\frac{kQ}{r^2}$                       |
| Sphere (Inside)                 | $E=0$                                    |
| Infinite wire                   | $E=\frac{\lambda}{2\pi\varepsilon_{0}r}$ |
| Infinite plane                  | $E=\frac{\sigma}{2\varepsilon_{0}}$      |
