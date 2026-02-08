# The Specimen

![[Fundamentals of Strength of Materials/attachments/Pasted image 20260208145212.png]]

> [!warning]- Standardization
> Specimens are standardized to allow for consistent results across labs.

Specimens are said to be **proportional** when gauge length $L_{0}$ is proportional to the square root of the area of the cross-section $A_{0}$.

**Circular Cross-Section**

![[Fundamentals of Strength of Materials/attachments/Pasted image 20260208145602.png]]

$$
\begin{align}
&L_{0}=5d\text{ Rounded to nearest 5mm} \\
&L_{0}+\frac{d}{2}<L_{C}<L_{0}+2d
\end{align}
$$

**Rectangular Cross-Section**

![[Fundamentals of Strength of Materials/attachments/Pasted image 20260208150007.png]]

$$
\begin{align}
&L_{0}=5.65\sqrt{ A_{0} } \text{ Rounded to nearest 5mm}\\
&L_{0}+1.5\sqrt{ A_{0} }\leq L_{C}\leq L_{0}+2.5\sqrt{ A_{0} }
\end{align}
$$

---
# The Setup

![[Fundamentals of Strength of Materials/attachments/Pasted image 20260208150144.png]]

The specimen is slowly pulled, measuring the elongation $\Delta L=L-L_{0}$.

> [!ERROR] Loading rate matters!
> We therefore have the following standard rates for steel and aluminium respectively (units in $Nmm^{-2}s^{-1}$):
> 
> $$
> \begin{align}
> & 6\leq \frac{d\sigma}{dt}\leq 30 \\
> & 2\leq \frac{d\sigma}{dt}\leq 10
> \end{align}
> $$

---
# Results

From any point we can get [[Fundamentals of Strength of Materials/5. Strain\|strain]] percent:

$$
\varepsilon=\frac{\Delta L}{L_{0}}=\frac{{L_{i}-L_{0}}}{L_{0}}
$$

We can also get [[Fundamentals of Strength of Materials/5. Strain#Linear Elasticity (1D)\|poisson's ratio]] by using:

$$
\varepsilon_{x}=\varepsilon_{y}=-\nu\varepsilon_{z}
$$
For isotropic materials.

