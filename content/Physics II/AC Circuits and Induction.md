Self-inductance $L$ describes how much of an inductor's (solenoid) current creates flux through itself.

$$
L=\frac{\Phi}{I}
$$
The unit is $H$ (Henry).

Mutual inductance $M$ describes how much of one loop's current creates flux though another.

$$
M=\frac{\Phi_{21}}{I_{1}}=\frac{\Phi_{12}}{I_{2}}
$$
(Form $\Phi_{\text{target, source}}$).

Total flux is:

$$
\Phi_{1}=L_{1}I_{1}+M_{12}I_{2}
$$
Tor recall, in solenoids:

$$
B=\mu_{0}nI
$$
Therefore

$$
\begin{align}
&\Phi_{1}=BS=\mu_{0}nSI \\
&\Phi_{N}=BSN=d\mu_{0}n^2SI
\end{align}
$$
Where $N=dn$, being $\text{Total loops}=\text{length}\times \text{loop density}$.

Flux per unit length:
$$
\Phi_{UL}=\frac{\Phi_{N}}{d}
$$
To find inductance per unit length:

$$
L=\frac{\Phi_{UL}}{I}=\mu_{0}n^2S
$$
# Inductors

> [!important]- definition.
> A solenoid is a sequence of loops with current flowing through them. An inductor is simply a solenoid in a circuit.
> 
> ![[Pasted image 20260205233930.png]]

> [!example]- Application of [[Magnetostatics#Ampere Law|Ampere's Law]]
> We use the Amperian Loop below:
> 
> ![[Pasted image 20260205234047.png]]
> 
> To get:
> 
> $$
> \begin{align}
> &\oint_{\Gamma_{A}}\vec{B}(\vec{r})\cdot d\vec{s}=\mu_{0}n\alpha I \\
> &\implies B_{\text{Outside}}\approx 0&&B_{\text{Inside}}=\mu_{0}nI
> \end{align}
> $$

If we have self-inductance in a circuit:

$$
\begin{align}
&\Phi=LI \\
&\text{emf}=-L \frac{dI}{dt}
\end{align}
$$
In an inductor:

$$
V_{L}=-\text{emf}=L \frac{dI}{dt}
$$

![[Pasted image 20260206014915.png]]
> An RL circuit

Inductors resist a change in current.

> [!check]- How do $V,I$ vary over time?
> 
> $$
> I=\frac{{\mathcal E}}{R}[1-e^{\frac{R}{L} t}]
> $$
> $$
> V_{L}={\mathcal E}e^{\frac{R}{L} t}
> $$
> 
> ![[Pasted image 20260206015330.png]]


$$
U=\frac{1}{2}LI_{0}^2=\frac{1}{2\mu_{0}}B^2\mathcal V
$$

Where $\mathcal V$ is the volume.

# Transformers

![[Pasted image 20260206015503.png]]

> [!warning]-
> NO POWER IS CREATED! If voltage increases, current decreases!

$$
\frac{I_{2}}{I_{1}}=\frac{{\mathcal E}_{1}}{{\mathcal E}_{2}}=\frac{N_{1}}{N_{2}}
$$
> [!warning]+
> Transformers ONLY work with AC current.

# Common Circuits
## RC Circuits
![[Pasted image 20260206015841.png]]

When the switch is closed we get the following time-dependant properties:
$$
\begin{align}
&I=\frac{V_{C0}}{R}e^{\frac{1}{RC}t} \\
&V_{C}=RI \\
&q_{C}=CV_{C 0}e^{\frac{1}{RC}t}
\end{align}
$$
## Inductor and AC Generator

We have:

$$
\begin{align}
&I_{\text{max}}=-\frac{V_{m}}{\omega L} \\
&V_{L,\text{max}}=\omega LI_{\text{max}}=X_{L}I_{\text{max}}
\end{align}
$$
HOWEVER, current has a $\frac{\pi}{2}$ phase delay with respect to voltage. 

> [!important]+ Inductive Reactance
> $X_{L}$, measured in $\Omega$. Zero when DC current is present.

![[Pasted image 20260206020633.png]]

We can deduct that inductors block high-frequency signals.
## Capacitor and AC Circuit

This time, current is $\frac{\pi}{2}$ ahead of voltage.

> [!important]+ Capacitive Reactance
> $$
> X_{C}=\frac{1}{\omega C}
> $$

![[Pasted image 20260206020639.png]]

$$
\begin{align}
&I_{\text{max}}=\omega CV_{m}
\end{align}
$$
Capacitors block low frequency signals.

## RLC Circuits

Resistor + Capacitor + Inductor

### The Setup: Free RLC (No Generator)
When there is no external power source, the energy just sloshes back and forth between the inductor and capacitor while the resistor burns it off as heat.

> [!abstract]+ Governing Equation
> The differential equation for the current $I(t)$ is a damped harmonic oscillator:
> $$
> \frac{d^2I}{dt^2} + \frac{R}{L}\frac{dI}{dt} + \frac{1}{LC}I(t) = 0
> $$

#### The Three Destinies (Damping)
Depending on the resistance $R$, the circuit behaves in one of three ways:

* **Overdamped** ($R > 2\sqrt{L/C}$): The current lazily decays to zero. No oscillations. It's like moving through molasses.
* **Underdamped** ($R < 2\sqrt{L/C}$): The system vibrates! The current oscillates back and forth, slowly dying out. This happens at the resonant frequency $\omega_{res}$.
* **Critically Damped** ($R = 2\sqrt{L/C}$): The perfect balance. The current returns to zero as fast as physically possible without overshooting.

---

### The Driven RLC (With Generator)
Now we attach a generator with frequency $\omega$. The circuit fights back with **Impedance** ($Z$).

> [!INFO]+ Impedance ($Z$)
> Think of this as "AC Resistance." It has a real part (Resistor) and an imaginary part (Reactance from $L$ and $C$).
> $$Z = R + i(X_L - X_C)$$
> $$|Z| = \sqrt{R^2 + (X_L - X_C)^2}$$
> * $X_L = \omega L$ (Inductor hates fast changes)
> * $X_C = \frac{1}{\omega C}$ (Capacitor hates slow changes)
>
>

#### Resonance
Resonance happens when the Inductor and Capacitor perfectly cancel each other out ($X_L = X_C$).

> [!TIP] At Resonance ($\omega = \omega_0$)
> * **Impedance is minimized:** $Z = R$ (Pure resistance).
> * **Current is maximized:** The circuit accepts maximum power.
> * **Phase:** Voltage and Current are perfectly in sync ($\phi = 0$).
> * **Frequency:** $\omega_0 = \frac{1}{\sqrt{LC}}$
>
>

---

### Frequency Behaviour
If you are not at resonance, one component dominates the other:

| Frequency | Dominant | Type | Phase |
| :--- | :--- | :--- | :--- |
| **Low** ($\omega < \omega_0$) | Capacitor ($X_C > X_L$) | Capacitive | Voltage **lags** Current |
| **Resonance** ($\omega = \omega_0$) | Resistor | Resistive | In Phase |
| **High** ($\omega > \omega_0$) | Inductor ($X_L > X_C$) | Inductive | Voltage **leads** Current |

> [!NOTE] The Q-Factor
> The **Quality Factor ($Q$)** tells you how "sharp" the resonance peak is.
> * **High Q (Low R):** A very sharp, narrow peak. The circuit is very selective.
> * **Low Q (High R):** A flat, wide hill. The damping is heavy.
> $$q = \frac{1}{R}\sqrt{\frac{L}{C}}$$
>

---

### Power
Finally, how much energy are we actually using?

> [!WARNING] Power Factor
> You cannot just multiply max voltage and max current. You must account for the phase difference ($\cos \phi$) and use RMS (Root Mean Square) values.
>
> $$\bar{P} = V_{rms} I_{rms} \cos \phi = \frac{V_{rms}^2 \cos \phi}{\sqrt{(X_L - X_C)^2 + R^2}}$$
>
> If the phase difference is $90^{\circ}$ ($\frac{\pi}{2}$), power is **zero**. The capacitor/inductor just store and release energy without burning it.

