# Diamagnetic Materials

> [!important]+ Definition
> No intrinsic magnetic dipoles, but will have magnetic dipoles when inside a magnetic field, generating a magnetic field opposing the external one.

Usually, they have [[Physics II/Magnetostatics#Magnetic Dipole\|magnetic susceptability]] $\chi_{m}\approx-10^{-5}$, meaning close but slightly lower than in a vacuum ($\chi_{m}=0$). This means that the diamagnetic property is typically ignored.
# Paramagnetic Materials

> [!important]+ Definition
> Has randomly oriented dipoles that do not interact. The overall dipole moment is zero, but when in a magnetic field, they all align, contributing positively to the overall magnetic field.

> [!check]+ Curie Law
> $$
> \chi_{m}T=\text{const}
> $$

For paramagnetic materials, $\chi_{m}\approx 10^{-4}$, so slightly greater than one. We can generally neglect the paramagnetic effect.

HOWEVER, when the external field is large enough, we can no longer use the approximate form for internal field, and therefore must use the more precise form:

$$
\vec{B}-\mu_{0}\vec{\mathcal M}+\mu_{0}\vec{H}
$$

# Ferromagnetic Materials
> [!important]+ Definition
> The material has magnetic dipoles which STRONGLY interact among them, leading to a collective behaviour influenced by an external field.

> [!check]+ Exchange Interaction
> Exchange interaction is a quantum phenomenon where all atoms have their magnetic dipoles which all interact, leading to collective behaviour.
> It is a short-range interaction (range of a few nm).

The behaviour of a ferromagnetic material is determined by:
- Exchange interaction between neighbouring atoms (keeping dipoles parallel). It is negative in energy
- Interaction with the external field, aligning dipoles to it.
- Interaction of every dipole with all other dipoles, pushing them antiparallel. This is longer range - $\mu m$ range.

> [!important]+ Magnetic Domains
> - A magnetic domain is a section of a material where all dipoles align. They are usually very small ($<1mm$ in diameter)
> - A large domain can create a huge magnetic field.
> - Within a domain, exchange interactions prevail, but between domains, dipole-dipole interactions prevail.
> - Increasing the size of domains increases energy of dipole-dipole interactions to increase, while $E$ from exchange interactions remains about the same. This leads to a limit in the size of domains without the help of an external $\vec{B}$.
>   
>   The limit for domain size is given by:
> 
> $$
> L^3_{Dom}=\mid\frac{e_{\text{exc}}}{e_{\text{dom}}}\mid L^3_{\text{exc}} 
> $$

For ferromagnetic materials, we must ALWAYS use the exact form for $B$:

$$
\vec{B}=\mu_{0}(\vec{H}+\vec{\mathcal M})
$$

## Hysteresis Loop

![[Physics II/attachments/Pasted image 20260206002031.png]]
> What happens when a ferromagnetic material is subjected to a varying magnetizing field.

The area within the graph is the energy wasted as heat per cycle.
- High coercivity means that it is easy to remove the magnetic property of a material (e.g. Transformer core). They have low energy.
- The opposite (low coercivity) is present in strong magnets (e.g. Neodymium magnet). They have high energy.