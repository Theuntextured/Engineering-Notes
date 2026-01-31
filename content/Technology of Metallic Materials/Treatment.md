# Quenching

The process of rapidly cooling a material, disallowing the crystal structure to realign as a result of the change in temperature.

> [!info]- Optional Diagram!
> ![[Technology of Metallic Materials/attachments/Pasted image 20260129021623.png]]

# Work Hardening

Work hardening (cold working is the process and work hardening is the result), or strain hardening, is the process of strengthening metal or polymer materials through plastic deformation (e.g., rolling, drawing, bending) below their recrystallization temperature. This increases dislocation density, making further deformation more difficult, which boosts strength and hardness while decreasing ductility. It is common in steels, aluminium, and copper.

Work hardening will create “dislocation forests” which slow down further dislocations, therefore increasing strength of the material, but a drop in toughness and resilience.

![[Technology of Metallic Materials/attachments/Pasted image 20260130172401.png]]

![[Technology of Metallic Materials/attachments/Pasted image 20260130172634.png]]

**For stretching:**
$$
\text{\%CW}=\frac{A_{0}-A_{d}}{A_{0}}\times 100\%
$$
* $A_{0}$: Initial area of the cross-section
* $A_{d}$: Final area of the cross-section

**For rolling:** 

$$
\text{\%CW}=\frac{{D_{0}-D_{f}}}{D_{0}}\times 100\%
$$

- $D_{0}$: Initial thickness
- $D_{f}$: Final thickness

By deforming, we create more dislocations via [[Technology of Metallic Materials/Defects#Frank-Read Dislocation Sources\|Frank-Read Dislocation Sources]]. The process is reversible via [[Technology of Metallic Materials/Treatment#Annealing]].

![[Technology of Metallic Materials/attachments/Pasted image 20260130192523.png]]

When the dislocation density gets high enough, we can observe that they cannot exist randomly any more, since they repel each other via their stress fields. Therefore, we get the following 'cell' structure:

![[Technology of Metallic Materials/attachments/Pasted image 20260130193125.png]]

Dislocations will end up clumping in cell walls, where certain ones will act as [[Technology of Metallic Materials/Defects#Frank-Read Dislocation Sources\|Frank-Read Dislocation Sources]]. Inside the cell interiors, the material is relatively free of defects.
## Ludwik-Hollomon Law

$$
\sigma_{T}=K\varepsilon^n_{T}
$$

- $\sigma_{T},\varepsilon_{T}$: True stress and true strain
	- $\varepsilon_{T}=\ln\left( \frac{L_{i}}{L_{0}} \right)$
- $K$: Strength coefficient. This is the value of $\sigma_{T}$ when $\varepsilon_{T}=1.0$.
- $n$: Strain Hardening Exponent
	- $n_{\text{FCC}}\approx 0.5$
	- $n_{\text{BCC}}\approx 0.2$
	- $n_{\text{HCP}}\approx 0.05$

> This is an approximation for a stress-strain curve.

When $\varepsilon_{T}=\varepsilon_{u}=n$, we can predict failure (necking) of the material.
## Taylor Equation

The Taylor Equation describes how much stronger a material gets as you deform it (cold work). The more dislocations $\rho$ are created, the more they interfere, making the material harder.

$$
\begin{align}
&\sigma_{i}=\alpha Gb\sqrt{ \rho } \\
&\tau_{\text{flow}}=\tau_{0}+k\sqrt{ \rho }
\end{align}
$$
- $\sigma_{i}$: The increase in yield strength
- $\alpha$: A material constant (usually between 0.2 and 0.5)
- $G$: Shear modulus (How stiff the material is in shear)
- $b$: Burgers Vector (Magnitude of the lattice distortion caused by one dislocation)
- $\rho$: Dislocation density (lines of dislocation per unit area)
- $\tau_{\text{flow}}$: Flow stress
# Solid Solutions

## Ageing

> [!important] The Orowan Loop
>
When second phases are present in a metal in the form of hard precipitate particles, dislocations need to “squeeze” through or around them to travel along the material. This leads to a harder material.
>
>$$
>\begin{align}
>&\sigma_{or}\approx \frac{Gb}{L}\\
>&\tau_{or}\approx \frac{G\,b}{2d}\sqrt{ f } \\
>&\sigma \approx 3\tau
>\end{align}
>$$
>
>- $G$: Shear modulus (How stiff the material is in shear)
>- $b$: Burgers Vector (Magnitude of the lattice distortion caused by one dislocation)
>- $L$: Inter-particle spacing (distance between precipitates)
>- $\sigma,\tau$: Tensile and shear stresses
>- $d$: Precipitate particle diameter
>- $f$: volume fraction of precipitate

![[Technology of Metallic Materials/attachments/Pasted image 20260130195531.png]]

Via [[Technology of Metallic Materials/Treatment#Quenching]] the material, and warming it to a lower temperature than originally, we can then wait and the particles in the material will re-arrange (We therefore want the temperature just high enough to allow movement of particles).

There are three main types of ageing results:
- Under-ageing: Impurities are very small, meaning that $L$ (Orowan loop equation) is small, leading to a very strong but brittle material.
- Over-ageing: Impurities grow too large and dislocations move very freely, easily creating Orowan Loops around precipitates.
- In between the two, we have a point where we can achieve a good balance between ductility and strength.

**Stages in the formation of the equilibrium precipitate $\theta$ phase (Ordered from the highest energy to lowest):**
1. Supersaturated $\alpha$ solution solid (there is more solute than can actually be stored)
2. GP1 (Guinier-Preston) zones (Coherent precipitate, tiny precipitates start to form)
3. GP2 (Or phase $\theta''$) zones (Coherent, ordered layers: Often max hardness occurs here or in the transition to the next phase)
4. Phase $\theta'$ (semi-coherent)
5. Phase $\theta \implies$ Equilibrium (incoherent, weak, over-aged, BCT structure in $CuAl_{2}$, while $Al$ is FCC) 
	- The material composed of aluminium matrix and $CuAl_{2}$ precipitate is called duralumin.

![[Technology of Metallic Materials/attachments/Pasted image 20260130222119.png]]


## Precipitation Hardening

Sometimes, precipitates forming on grain boundaries can actually make the material more ductile. GBs act as attractors for impurities because of their high energy state, and therefore clean up the inner parts of grains, forming an almost pure second phase. The presence of two pure second phases makes the material more ductile compared to an impure material with one phase.
## Solid Solution Strengthening (Size Misfit)

When a solid solution is formed between atoms with very different sizes, the material is in tension in some areas and in compression in others, creating a stress field that blocks dislocations. The increase in strength is approximately proportional to the size difference (As a percentage of the host's volume):

$$
\sigma_{\text{Solid Solution}}\approx \text{const.} \frac{\Delta \Omega}{\Omega}
$$

- $\Delta \Omega$: Difference in atomic volume between solute and solvent
- $\Omega$: Atomic volume of host matrix

Solid solutions increase strength but slightly decreases ductility.
$$
\Delta \tau \propto \sqrt{ c }
$$
> Increase of internal shear stress $\Delta \tau$ is proportional to the square root of the concentration $c$ of the added atoms, meaning that you get diminishing marginal returns as you add more solute.


## Coherency Strain

When a precipitate does not interrupt the crystal structure (For example using a BCC solute in a BCC solvent with similar atomic sizes) and direction, we can consider it a coherent structure. Since the alignment is not perfect, there is a slight misfit in spacing, but the effect is much less than if the lattice structure was interrupted.

$$
\sigma_{\text{coherency}}\approx \frac{\Delta a}{a}E=\varepsilon_{\text{misfit}}E
$$

- $a$: Lattice parameter (grid size) of the matrix
- $\Delta a$: Difference between precipitate's grid size and matrix's grid size
- $\varepsilon_{\text{misfit}}$: Lattice misfit strain (How much this second phase strains the matrix)
- $E$: Young's Modulus

![[Technology of Metallic Materials/attachments/Pasted image 20260130195016.png]]


# Annealing

Annealing is the process of warming up a metal close (but not over) $T_{m}$ in order to remove dislocations. This increases ductility.

# Strengthening by Hard Phase From Phase Transformation

When a material cools down at eutectoid temperature ($723-727°C, 0.76\, wt\%$ carbon austenite transforming into pearlite for steel) and therefore creates bands of different phases (For pearlite it is cementite and ferrite).

If steel is quenched, it will produce martensite instead, which is harder but more brittle than pearlite since it is in a meta-stable state.


