# Schmid's Law

Any normal stress can be resolved into a shear stress component $\tau_{RSS}$ (resolved shear stress) and a normal stress component $\sigma$ with respect to a slip plane.

When the $F_{\tau}$ exceeds a threshold value, called **Critical Resolved Shear Stress** $\tau_{\text{CRSS}}$, the plane starts slipping.

> [!important] Schmid's law
> For a dislocation to move over its slip systems, a shear stress acting over the slip plane and along the slip direction must be applied; this is typically determined by an applied normal force to the sample such that as it happens in a tensile test.

$\tau_{\text{CRSS}}$ is a material property which is closely related to yield stress $\sigma_{y}$.

When planes start to slip, slip lines start forming and eventually, numerous aggregate dislocations form slip bands. The bands and lines follow the primary slip system, which is the direction with the lowest $\tau_{\text{CRSS}}$, as shown below.

![[Technology of Metallic Materials/attachments/Pasted image 20260128195120.png]]

We define the following angles $\lambda, \varphi$ and stress $\sigma$: 

![[Technology of Metallic Materials/attachments/Pasted image 20260128195633.png]]

$$
\begin{align}
&\sigma=\frac{F}{A} \\
&\tau=\frac{F}{A}\cos \varphi \cos \lambda \\
&\implies \tau_{\text{RSS}}=\sigma \cos \varphi \cos \lambda \\
&m=\cos \varphi \cos \lambda=\text{Schmid Factor}
\end{align}
$$
Note that $m_{max}$ is 0.5 (When $\lambda=\varphi=45°$) and the minimum is 0 (When $\lambda=0°,\varphi=90°$ or $\varphi=0,\lambda=90°$).

When $\tau_{RSS}$ is minimized we prevent slip from occurring. The material will therefore snap before it manages to slip.

Using the Schmid Factor, we can get:
$$
\sigma_{y}=\frac{\tau_{\text{CRSS}}}{m}
$$

> [!note]+
> Consider that not all crystal structures have a favourable slip plane and direction, and some will have several slip planes. For example FCC will almost always has at least one system with a favourable Schmid Factor.

If we consider HCP structures (`Hexagonal Close-Packed`, such as $Ti, Mg$), the Schmid's Law often gives 0 for the coefficient. This is because HCP has very few slip planes. This means that when plastically deforming, they will usually show [twinning](Defects#Twinning).

> [!check] What happens as we pull?
> Over time, as the material undergoes slip, the slip direction rotates TOWARDS the tensile axis, therefore making it harder to deform the material further, until we have $\cos \varphi=0$ leading to no more slipping.

# Taylor Factor

For polycrystalline materials, since the Schmid Factor is different for all grains, we cannot use a single value for it. If two neighbour grains tried to shapeshift in different ways, a crack would form between them. This means that plastic deformation in polycrystalline materials is **inhomogeneous**.

For real polycrystalline materials we therefore use the Taylor Factor $M$. Polycrystalline materials are harder to deform since grains “fight each other” while deforming. This is given by:
$$
\sigma_{y}=M\cdot \tau_{\text{CRSS}}
$$
A higher value for $\bar{m}$ will mean a greater $M$, but the correlation is not as simple, since $M$ takes into consideration both $\bar{m}$ and forces on grain boundaries. But we can gather the approximation:
$$
\begin{align}
&\sigma_{y}\approx 2\,\tau_{\text{CRSS, single crystal}} \\
&\sigma_{y}\approx 3\,\tau_{\text{CRSS, polycrystal}} \\
&\implies M\approx \frac{3}{2}\cdot \frac{1}{m_{max}}\\
&M\approx \overline{\left( \frac{1}{m} \right)}
\end{align}
$$
(Remember that $\bar{x}$ means the mean value for $x$)

HOWEVER, this does not always hold. But we can infer that the yield strength for the same metal can increase by 50% just by having grains rather than being a single crystal.

> [!info]
> In FCC metals (e.g. $Al,Cu$), with random texture, $M=3.06$

# Taylor-Von Mises Criterion
_Not to be confused with the [[Fundamentals of Strength of Materials/4. Stress#Von Mises Criterion\|Von Mises Criterion]] from FSM!_

In a polycrystal, every grain is surrounded by neighbours, therefore if one changes shape, the neighbours must also change shape, otherwise a crack forms and the material fails.
In order for this to happen, the **Von Mises Criterion** states that there must be at least 5 degrees of freedom in order for the shape of the sample to change shape arbitrarily in 3D space (stretch, compress, shear etc.).

Mathematically, there are 6 components to shape change in the strain tensor. Since volume is constant, $\varepsilon_{xx}+\varepsilon_{yy}+\varepsilon_{zz}=0$ so we have 5 independent components, meaning that at least 5 slip planes MUST exist for all components of the strain tensor to be independently manipulated.

At higher temperatures, more slip planes can be created, meaning that a material that is brittle at room temperature can become ductile at higher temperatures (such as high-carbon steel).

> [!example] Why do we care?
> The Von Mises Criterion tells us if a crystal structure is brittle or ductile. If it cannot be freely manipulated, then it will fracture if we try, meaning that the material is brittle.
> **FCC** ($Al,Cu,\text{Austenite}$): Has 12 slip systems, meaning that we can deform it and it is therefore ductile.
> **HCP** ($Mg, Zn$): Has only 3 slip planes, meaning that the criterion is not met and the structures are brittle.

# Lüders Bands

Yielding does not happen everywhere in the metal at the same time: it happens in Lüders Bands (bands where there is higher local stress concentration), and the yielding then propagates across the material.

![[Technology of Metallic Materials/attachments/Pasted image 20260130171226.png]]
Since these bands all happen at different stresses, the stress-strain graph for materials which show such behaviour will have a long **yield elongation** at $\sigma=\sigma_{y,\,\text{lower}}$ in the form of a jagged line (stress is not perfectly constant).

![[Technology of Metallic Materials/attachments/Pasted image 20260130171655.png]]

> [!example]- The ugly marks
> To get rid of Lüders Bands, since they can be ugly to look at, we can polish the surface using a [[Technology of Metallic Materials/Treatment\|treatment method]] called **skin passing**.

The reason Lüders Bands happen in steel is because of [[Technology of Metallic Materials/Overview of Steels#Cottrell Atmospheres\|Cottrell Atmospheres]]. Each atmosphere “snaps” with a different moment, leading to the yield elongation and the **phenomenon of plastic instability**.

