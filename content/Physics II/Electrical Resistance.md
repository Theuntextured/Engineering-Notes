> [!check]- Current Density $\vec{J}$
> $$
> \vec{J}=qn\vec{v}
> $$

$$
I=\frac{dQ}{dt}=\int_{S}\vec{J}\cdot \vec{u}_{N}dS
$$
## Resistivity

When an electron flows in a conductor, it will (on average) collide with a particle and zero its velocity every $2\tau$ seconds, where $\tau$ is called the lifetime. When colliding, $K_{E}$ is transferred to the material, heating it.

$$
\begin{align}
&v_{max}=2\tau a=2\tau\frac{q}{m}E \\
&\implies \vec{v}_{\text{avg}}=\frac{q}{m}\vec{E}\tau \\
\end{align}
$$
And
$$
\vec{J}=\sigma \vec{E}=\frac{\vec{E}}{\rho}
$$
Where $\sigma$ is called electrical **conductivity** of the material, and $\rho$ is the electrical **resistivity**.

We therefore get (in a uniform wire of length $d$ and cross-sectional area $S$):

$$
\begin{align}
&I=\sigma ES \\
&\Delta V=Ed=\frac{d\rho}{S}I=IR \\
&R=\frac{d\rho}{S}=\frac{d}{\sigma S}
\end{align}
$$

Electrical conductance:

$$
G=\frac{1}{R}=\frac{\Delta V}{I}
$$
Its unit is a Siemen.

## Heating Effect

$$
P=I\Delta V=RI^2=\frac{\Delta V^2}{R}
$$
> [!warning]+
> Resistance varies with temperature!

# Resistors

![[Physics II/attachments/Pasted image 20260205225118.png]]

In **Series:**

$$
R_{tot}=\Sigma R_{i}
$$
In **Parallel:**
$$
\frac{1}{R_{tot}}=\Sigma {\frac{1}{R_{i}}}
$$
![[Physics II/attachments/Pasted image 20260205225733.png]]

