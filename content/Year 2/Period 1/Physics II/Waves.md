A physical perturbation carrying energy (not matter) through space and time.

> [!abstract]+ The Wave Function (1D)
> $$f(x,t) = A \sin\left[ 2\pi \left(\frac{x}{\lambda} - \frac{t}{T}\right) \right] = A \sin[kx - \omega t]$$
>
> **Key Relationships:**
> * **Wavenumber:** $k = \frac{2\pi}{\lambda}$
> * **Angular Frequency:** $\omega = 2\pi \nu = \frac{2\pi}{T}$
> * **Phase Velocity:** $v_\phi = \lambda \nu = \frac{\omega}{k}$
>
> To be a wave, it must satisfy the **Wave Equation**:
> $$\nabla^2 f = \frac{1}{v^2} \frac{\partial^2 f}{\partial t^2}$$
>

---

### Wave Packets & Velocities
Real waves are often “packets” (localized), not infinite sinusoids.

> [!INFO] Phase vs. Group Velocity
> * **Phase Velocity ($v_\phi$):** Speed of a single peak. $v_\phi = \frac{\omega}{k}$
> * **Group Velocity ($v_g$):** Speed of the "envelope" (information).
>     $$v_g = \frac{\partial \omega}{\partial k}$$
> * **Dispersion:** If $v_\phi$ depends on frequency, the packet spreads out over time. If all frequencies move at the same speed, it is **non-dispersive**.
>

> [!WARNING] Bandwidth Theorem
> You cannot have a wave perfectly localized in both space and frequency.
> $$\Delta x \Delta k \ge 1 \quad \text{and} \quad \Delta t \Delta \nu \ge 1$$
> A tighter packet requires more frequencies to build.

---

### Standing Waves (Strings)
Waves trapped between two boundaries (fixed ends).

> [!TIP] Harmonics
> For a string of length $L$ fixed at both ends ($A(0)=A(L)=0$):
>
> * **Wavelength:** $\lambda_n = \frac{2L}{n}$
> * **Frequency:** $\nu_n = \frac{v_\phi}{2L}n = n \nu_1$ (for $n=1, 2, 3...$)
> * **Nodes:** Points of zero amplitude. There are $n-1$ nodes (excluding ends).
>

> [!NOTE] String Velocity
> The speed of the wave depends on tension ($T$) and linear mass density ($\mu$):
> $$v_\phi = \sqrt{\frac{T}{\mu}}$$
>
