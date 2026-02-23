For two equal, but opposite charges $+q,-q$ separated by a small distance $d$, dipole moment is:

$$
\vec{p}=q\vec{d}
$$
> [!note]+
> $\vec{d}$ goes from the negative charge to the positive.

$$
\begin{align}
&V_{p}\approx k \frac{\vec{p}\cdot \vec{u}_{r}}{r^2} \\
&\implies\vec{E}_{p}=k \frac{{3(\vec{p}\cdot \vec{u}_{r})\vec{u}_{r}-\vec{p}}}{r^3}
\end{align}

$$
## Dipole in an Electric Field
A torque is applied since there are two opposite charges.

$$
\begin{align}
&\vec{F}_{\text{NET}}=\vec{0} \\
&\vec{\tau}=\vec{p}\times \vec{E}
\end{align}
$$

> [!example] The torque aligns the charges with the field.

# Polarization

> [!important]+ Definition
> When a neutral atom is in a magnetic field electrons and protons are forced in opposite directions, creating a dipole moment $\vec{p}$ which depends on field strength and atom properties $\alpha$.
> The total dipole moment of all atoms in a solid is called polarization $\mathcal{P}$.

For small intensities of fields we can approximate using Maclaurin Expansion:

$$
\begin{align}
&\vec{p}=\varepsilon_{0}\alpha \vec{E}+o(\vec{E}) \\
&[\alpha]=C^2mN^{-1} \\
&\mathcal{P}=n\vec{p}=\varepsilon_{0}\chi \vec{E}
\end{align}
$$
Where $\chi=n\alpha$ is the material's electrical susceptibility. 

> [!warning]+
> There is a limit as to how much a dielectric can be polarized. After this limit (the field is greater than the dielectric strength), the atoms break down and become conductive.

When a material is polarized, it has its own field, so it will contribute to the overall field:

$$
\vec{E}_{\text{net}}=\vec{E}_{0}+\vec{E}_{P}
$$
Since $\vec{E}_{P}$ is opposite to the external field,

$$
\begin{align}
E_{\text{net}}&=E_{0}-E_{P} \\
&=E_{0}-\frac{\sigma_{P}}{\varepsilon_{0}} \\
&=E_{0}-\frac{Q_{P}}{S\varepsilon_{0}}
\end{align}
$$
Finally, we can say:

$$
E=\frac{E_{0}}{1+\chi}
$$
Where $\varepsilon_{r}=\kappa=1+\chi$ is the relative dielectric constant of the material, or relative permittivity.

$$
\varepsilon=\varepsilon_{0}\varepsilon_{r}
$$

## Electrical Displacement Vector

> [!important]+ Definition
The electrical displacement vector $\mathbf{D}$, is a vector field that represents the effect of free charges within dielectric materials, separating their contribution from bound charge polarization.

$$
\begin{align}
&\vec{D}\approx \varepsilon \vec{E} \\
&\implies \oint_{S}\vec{D}\cdot \vec{u}_{n}dS=Q_{\text{FREE}}
\end{align}
$$
