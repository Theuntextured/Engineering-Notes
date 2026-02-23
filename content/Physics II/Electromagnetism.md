As discussed in [[DC Generators#EMF]], [[Magnetostatics|magnetic]] and [[Electrostatics|electric]] fields are interchangeable with the right context and one cannot exist without the other.

# Maxwell Equations in a Vacuum

| **LAW**                      | **INTEGRAL FORM**                                                                                                                         | **DIFFERENTIAL FORM**                                                                                        |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **GAUSS FOR ELECTRIC FIELD** | $\displaystyle \oint_S \vec{E}(\vec{r}) \cdot \vec{u}_N \, dS = \frac{Q}{\epsilon_0}$                                                     | $\displaystyle \nabla \cdot \vec{E} = \frac{\rho}{\epsilon_0}$                                               |
| **GAUSS FOR MAGNETIC FIELD** | $\displaystyle \oint_S \vec{B}(\vec{r}) \cdot \vec{u}_N \, dS = 0$                                                                        | $\displaystyle \nabla \cdot \vec{B} = 0$                                                                     |
| **FARADAY-HENRY-LENZ**       | $\displaystyle \oint_\Gamma \vec{E}(\vec{r}) \cdot d\vec{s} = -\frac{d}{dt} \left[ \int_S \vec{B}(\vec{r}) \cdot \vec{u}_N \, dS \right]$ | $\displaystyle \nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}$                                 |
| **AMPERE-MAXWELL**           | $\displaystyle \oint_\Gamma \vec{B}(\vec{r}) \cdot d\vec{s} = \mu_0 I + \mu_0 \epsilon_0 \frac{d\Phi(\vec{E})}{dt}$                       | $\displaystyle \nabla \times \vec{B} = \mu_0 \vec{J} + \mu_0 \epsilon_0 \frac{\partial \vec{E}}{\partial t}$ |
## EM Waves

Accelerating charges create self-propagating $E$ and $B$ fields.

> [!example] EM Properties (In Vacuum)
> * **Speed:** $v_{em} = c = \frac{1}{\sqrt{\mu_0 \epsilon_0}} \approx 3 \times 10^8 \text{ ms}^{-1}$
> * **Geometry:** $\vec{E} \perp \vec{B} \perp \vec{k}$ (Transverse wave).
> * **Magnitude:** $|\vec{E}| = c|\vec{B}|$ (Electric field is much stronger).
> * **Vector Relation:** $\vec{k} \times \vec{E} = \omega \vec{B}$
>

> [!DANGER] The Poynting Vector ($\vec{S}$)
> Represents the **energy flux** (energy transfer per unit area per unit time).
>
> $$\vec{S} = \frac{1}{\mu_0} \vec{E} \times \vec{B}$$
>
> Simplified magnitude: $|\vec{S}| = c\varepsilon_0 |\vec{E}|^2$

---
### Light & Conservation of Energy
Light carries intensity ($I$). When it hits a surface, it splits into three fates: Transmitted ($T$), Reflected ($R$), or Absorbed ($A$).

> [!abstract] Conservation Law
> Since energy is conserved:
> $$I_0 = I_T + I_R + I_A$$
> Dividing by initial intensity $I_0$:
> $$1 = T + R + A$$
>

> [!NOTE] Refractive Index ($n$)
> In a material, light slows down.
> * **Speed:** $v = \frac{c}{n}$
> * **Wavelength:** $\lambda = \frac{\lambda_0}{n}$ (Frequency $f$ never changes!)
> * **Wavenumber:** $k = nk_0$
>

---

### Absorption (Beer-Lambert Law)
As light travels through a thick medium, it gets eaten up.

> [!DANGER] Beer-Lambert Law
> Intensity decays exponentially with distance $x$:
> $$I(x) = I_0 e^{-\alpha x}$$
> * **$\alpha$:** Absorption coefficient (depends on material).
> * **$\kappa$:** Extinction coefficient (linked to complex refractive index $N = n + i\kappa$).
> $$\alpha = \frac{4\pi\kappa}{\lambda_0}$$
>

---

### Reflection & Refraction (Geometric Optics)
How light bends and bounces.

> [!TIP] Snell's Law (Refraction)
> When moving between media with different indices ($n_i$ to $n_t$):
> $$n_i \sin \theta_i = n_t \sin \theta_t$$
> * $\theta$ is always measured from the **Normal** (vertical axis).
>

> [!INFO] Fermat's Principle
> Light always takes the path of **least time** (not necessarily shortest distance).
> * **Mirages:** Caused by hot air changing $n$, bending light so the "fastest" path curves through the sky.
> * **Reflection:** $\theta_{incident} = \theta_{reflected}$
>

---

### Material Behaviors
Why mirrors shine and glass is clear.

> [!example] Metals vs. Dielectrics
> **Metals (High $\kappa$):**
> * High absorption coefficient means light is absorbed instantly at the surface.
> * This energy vibrates electrons, which immediately re-emit the light.
> * Result: **High Reflection ($R \approx 1$)**.
>
> **Glass (Dielectric):**
> * $R \approx 0.04$ (Only ~4% reflected per surface).
> * Most light is transmitted ($T$).
>

> [!WARNING] Total Internal Reflection
> If you try to go from High $n$ to Low $n$ (e.g., Water to Air) at a steep angle, light gets trapped.
> * Happens when $\theta_i > \theta_{critical}$.

---

### Beatings
When two waves of slightly different frequencies overlap, they create a pulsing effect.

> [!abstract] The Envelope Effect
> The total wave looks like a high-frequency "carrier" wave inside a low-frequency "envelope."
> * **Carrier Frequency:** Average of the two ($\frac{\omega_1 + \omega_2}{2}$).
> * **Modulator (Beat) Frequency:** Difference of the two ($\frac{\omega_1 - \omega_2}{2}$).
>
> $$A_{tot}(x,t) = \left\{ 2A_0 \cos \left[ \frac{\Delta k}{2}x - \frac{\Delta \omega}{2}t \right] \right\} \sin[kx - \omega t]$$
>
> **Application:** AM Radio (Amplitude Modulation) uses this to encode sound onto a radio wave.

---

### Interference (Two Sources)
When two coherent waves (same frequency, constant phase difference) meet.

> [!TIP] Constructive vs. Destructive
> * **Phase Difference ($\Delta \phi$):** Depends on the path difference ($\Delta s$) traveled by the waves.
>   $$\Delta \phi = \frac{2\pi}{\lambda} \Delta s$$
> * **Constructive ($0, 2\pi, \dots$):** Waves add up. Peak intensity $\propto 4A_0^2$.
> * **Destructive ($\pi, 3\pi, \dots$):** Waves cancel out. Intensity is zero.

> [!example] Young's Double Slit
> > For two slits separated by distance $d$:
> * **Path Difference:** $\Delta s \approx d \sin \theta$
> * **Maxima (Bright Spots):** $\sin \theta = m \frac{\lambda}{d}$ (where $m$ is an integer).
> * **Minima (Dark Spots):** $\sin \theta = (m + \frac{1}{2}) \frac{\lambda}{d}$
>

---

### N-Slit Interference
What happens when you add more slits ($N > 2$).

> [!INFO] Sharper Peaks
> As $N$ increases:
> * **Brightness explodes:** Max Intensity $\propto N^2$.
> * **Sharpness increases:** Peak width $\propto 1/N$.
> * **Secondary Peaks:** Small ripples appear between the main bright spots.
>
> This is the principle behind **Phased Array Antennas** - you can steer a signal beam just by changing the timing (phase) of the emission, without physically moving the antenna.

---

### Diffraction
The bending of light when it passes through a single small opening (width $a$).

> [!WARNING] The Spreading Limit
> If the hole is smaller than the wavelength ($a < \lambda$), light spreads everywhere spherically.
> If the hole is large, you get a distinct pattern.
>
> **Fraunhofer Diffraction** (Long distance approximation):
> $$I(\theta) = I_0 \text{sinc}^2 \alpha \quad \text{where} \quad \alpha = \frac{\pi a \sin \theta}{\lambda}$$
>

> [!DANGER] Diffraction Minima (Dark Spots)
> The condition for **DARK** spots in a single slit is:
> $$\sin \theta_{min} = n \frac{\lambda}{a} \quad (n \neq 0)$$
> * **Crucial Note:** $n=0$ is the **Central Maximum** (the big bright spot in the middle).
> * The central spot is twice as wide as the other fringes.

