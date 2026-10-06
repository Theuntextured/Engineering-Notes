
# 1. Statics

$$
\begin{align}
v_{B}=v_{A}+\omega \times r_{B/A} &  & a_{B}=a_{A}+\dot{\omega}\times r_{B/A}-\omega^2r_{B/A}
\end{align}
$$

$$
\omega=\frac{{\vec{r}\times \vec{v}}}{|\vec{r}|^2}
$$

# 2 Dynamics

![[Pasted image 20260630155542.png]]

# 3. Friction

# Pin Friction and the Friction Circle

## Definition
The **pin friction angle** ($\varphi$) is the angle whose tangent represents the coefficient of kinetic friction ($\mu$) between a rotating pin and its bearing/pulley interface.
$$\tan\varphi = \mu$$

## The Friction Circle Concept
When a pulley rotates at a constant velocity, the distributed normal and frictional forces combine into a single **resultant reaction force**. 
* Due to friction, this resultant force does not pass through the geometric center $O$ of the pin.
* Instead, it shifts to create a resisting torque opposing the angular velocity $\omega$.
* The shifted reaction force is always **tangent** to an imaginary concentric circle called the **friction circle**.

## Mathematical Relation
The radius of the friction circle ($\rho$) is determined by the pin radius ($r$) and the pin friction angle ($\varphi$):
$$\rho = r \sin\varphi$$

## Application in Static Equilibrium
To solve for the applied force $F$ in systems like a pulley with pin friction:
1. Identify the direction of rotation ($\omega$).
2. Draw the resultant reaction force tangent to the friction circle of radius $\rho$, positioned such that it opposes the rotation.
3. Take the moment equilibrium about the contact point or use the geometry of the force vectors intersecting the friction circle.

# 5. Motion Transmission and Transformation

> [!TIP]+ **Power Balance Theorem:**
> 
> $$
> I_{eq}=I_{m}i^2\eta+I_{u}
> $$
> 
> Where :
> - $I_{m}$ is the moment of inertia of the motor side
> - $I_{u}$ is the moment of inertia of the user side
> - $\eta$ is the efficiency of transmission
> - $i=\frac{\omega_{m}}{\omega_{u}}$
> - $I_{eq}$ is the equivalent moment of inertia of the system from the user's part

# 6. Vibrations

## Free Vibrations (The System Left Alone)
*This section is for when you pull a mass back, let it go, and just watch it bounce until friction kills the movement.*

* **Damping Ratio**
    * **Formula:** $\zeta = \frac{c}{2\sqrt{km}}$
    * **WTF it is:** A dimensionless percentage of how fast the system kills its own energy. $c$ is the damping coefficient (in $Nsm^{-1}$)
    * **Application:** It tells you if the system will actually bounce ($\zeta < 1$, underdamped) or if it is so stiff with friction it just oozes back to the start line without crossing it ($\zeta \geq 1$, overdamped).
* **Damped Natural Frequency**
    * **Formula:** $\omega_d = \omega_n \sqrt{1 - \zeta^2}$
    * **WTF it is:** The actual, physical speed of oscillation when friction (damping) is dragging it down. It is always slightly slower than the theoretical undamped speed ($\omega_n$).
    * **Application:** Use this to find the actual time period between bounces in the real world.
* **Logarithmic Decrement**
    * **Formula:** $\delta = \ln\left(\frac{x_n}{x_{n+1}}\right) = \frac{2\pi\zeta}{\sqrt{1-\zeta^2}}$
    * **WTF it is:** The natural log of the ratio between two consecutive peaks of a bouncing mass.
    * **Application:** Purely experimental. You smack a machine, measure peak 1, measure peak 2, calculate $\delta$, and use that to work backwards to find the hidden damping ratio ($\zeta$) of the machine.

## Forced Vibrations (The System Being Shaken)
*This section applies when an external motor or oscillating force is continuously shaking the system.*

* **Frequency Ratio**
    * **Formula:** $r = \frac{\omega}{\omega_n}$
    * **WTF it is:** The speed of the external shaking motor ($\omega$) divided by the system's natural preferred bouncing speed ($\omega_n$).
    * **Application:** The single most important parameter in vibration. If $r=1$, the motor matches the system's natural frequency perfectly, causing **resonance** (the machine tears itself apart).
* **Steady-State Amplitude**
    * **Formula:** $X = \frac{F_0}{k\sqrt{(1 - r^2)^2 + (2\zeta r)^2}}$
    * **WTF it is:** How violently the system shakes once the startup jitters die out and it settles into a constant rhythm.
    * **Application:** Sizing physical clearances so vibrating parts do not smash into their housings during continuous operation.
* **Phase Angle**
    * **Formula:** $\phi = \arctan\left(\frac{2\zeta r}{1 - r^2}\right)$
    * **WTF it is:** The time delay between the push of the motor and the actual swing of the mass.
    * **Application:** Crucial for balancing rotating machinery. The heavy spot on a rotor does not always correspond to where the shaft bends the most.

## Transmissibility & Instruments (Isolation)
*This section is about stopping vibrations from spreading, or how to measure them properly.*

* **Force Transmissibility**
    * **Formula:** $T_r = \sqrt{\frac{1 + (2\zeta r)^2}{(1 - r^2)^2 + (2\zeta r)^2}}$
    * **WTF it is:** A percentage. The force transmitted into the floor divided by the force generated by the shaking machine.
    * **Application:** Designing rubber engine mounts. You want $T_r$ to be as small as possible so your car chassis does not rattle to pieces.
* **Vibration Instruments**
    * **Seismograph condition:** $r \gg 1$ (Instrument natural frequency must be super low compared to the earthquake).
    * **Accelerometer condition:** $r \ll 1$ (Instrument must be super stiff/high frequency compared to the vibration it is measuring).

## Transients (Random Impacts)
*This section is for when the force is a chaotic mess, like a car hitting a pothole, rather than a neat, repeating sine wave.*

* **Impulse Response**
    * **Formula:** $h(t) = \frac{1}{m\omega_d} e^{-\zeta\omega_n t} \sin(\omega_d t)$
    * **WTF it is:** The exact mathematical fingerprint of how the system twangs after a single, instantaneous hammer strike.
* **Duhamel's Integral**
    * **Formula:** $x(t) = \int_0^t F(\tau) h(t-\tau) d\tau=\frac{1}{m\omega_d} \int_0^t F(\tau) e^{-\zeta\omega_n (t-\tau)} \sin(\omega_d (t-\tau)) d\tau$
    * **WTF it is:** A continuous sum of thousands of tiny hammer strikes.
    * **Application:** You plug any weird, generic force graph $F(\tau)$ into this nightmare of an integral to find exactly how the system reacts over time. It is the brute-force ultimate weapon for non-periodic forces.

# 8. Bearings

## Viscosity (The Resistance to Flow)
* **Formula:** $\tau = \mu \frac{du}{dy}$ (Newton's Law of Viscosity)
* **WTF it is:** $\tau$ is the shear stress (friction force per area), $\mu$ is the dynamic viscosity (the oil's thickness), and $\frac{du}{dy}$ is the velocity gradient (how fast the oil layers are sliding past each other).
* **Application:** This proves mathematically that the harder you shear the oil (higher RPM), the more friction force it generates. Oil is not just slippery; it is a structural component that resists being torn apart.

## The Reynolds Equation (What the fuck is this?)
* **Formula:** $\frac{\partial}{\partial x}\left( h^3 \frac{\partial p}{\partial x} \right) = 6\mu U \frac{\partial h}{\partial x}$ (1D steady-state wedge)
* **WTF it is:** The absolute core of hydrodynamic lubrication. $h$ is the physical film thickness, $p$ is the generated pressure, $\mu$ is viscosity, and $U$ is the sliding velocity.
* **Application:** It proves that you *must* have a converging physical wedge ($\frac{\partial h}{\partial x} < 0$) to generate positive pressure. If two parallel plates slide against each other, the right side becomes zero, no pressure is generated, and your machine destroys itself in seconds.

## Forces on the Pad
* **Normal Force ($F_n$):** $F_n = \int \int p \, dx \, dz$
    * **WTF it is:** The mathematical integration of the pressure mountain generated by the Reynolds equation over the surface area of the pad. 
    * **Application:** This is the lifting capacity. It carries the vertical weight of your machine.
* **Tangential Force ($F_t$):** $F_t = \int \int \tau \, dx \, dz$
    * **WTF it is:** The integration of the shear stress over the pad. 
    * **Application:** This is the viscous drag. It tells you exactly how much torque you are wasting just stirring and heating up the oil.

## Radial (Journal) Bearings
* **Eccentricity Ratio ($\epsilon$):** $\epsilon = \frac{e}{c}$
    * **WTF it is:** The ratio of how far off-centre the shaft is sitting ($e$) compared to the total physical radial clearance ($c$). $\epsilon = 0$ is perfectly centred; $\epsilon = 1$ is catastrophic metal-to-metal contact.
* **Sommerfeld Number ($S$):** $S = \left(\frac{r}{c}\right)^2 \frac{\mu N}{P}$
    * **WTF it is:** The master dimensionless number for journal bearing design. It combines geometry ($r/c$), oil thickness ($\mu$), rotational speed ($N$), and load pressure ($P$).
    * **Application:** You calculate $S$ to look up design charts for high-performance rotating machinery (like sizing the main crankshaft bearings in a high-revving boxer engine) to find exactly where the shaft will settle inside the housing during operation.

## Hydrodynamic vs. Hydrostatic Lubrication
* **Hydrodynamic:** The motion of the shaft itself physically drags the oil into the wedge to build its own pressure. Fails at zero RPM—startup and shutdown are when 99% of engine wear happens.
* **Hydrostatic:** An external mechanical pump forces oil in at massive pressure to float the shaft *before* it even starts moving. Zero startup wear, but requires a bulky, parasitic pump system.