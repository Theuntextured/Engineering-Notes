# 1st Law of Thermodynamics

> [!QUOTE] The Law
> Energy can be neither created nor destroyed during a process, it can only change form.
> 
> The net change in the total energy of the system during a process is equal to the difference between total energy entering and the total energy leaving the system during the process.

$$
\Delta E=Q-W
$$
In a [[Thermodynamics and Heat Transfer/Thermodynamics/1. Basics#Energy|thermodynamic cycle]] which is quasi static (quasi-equilibrium) we have the area inside the diagram being:

$$
W_{cycle}=Q_{cycle}
$$

# 2nd Law of Thermodynamics

> [!QUOTE]+ Kelvin-Planck Statement
> It is impossible for any system to operate in a thermodynamic cycle and deliver a net amount of energy by work to its surroundings while receiving energy by heat transfer from a single heat capacity (thermal reservoir).
> ![[Pasted image 20260525193519.png]]

- Kelvin-Planck applies only to **cycles**. A non-cyclic process can receive heat from one reservoir and do work, but a power cycle must **reject heat** to a colder reservoir: $Q_1>0$, $W>0$, $Q_2<0$, $T_1>T_2$.

> [!QUOTE]+ Clausius Statement
> It is impossible for any system to operate in a cycle that takes heat from a colder heat capacity (reservoir) and transfer it to a hotter heat capacity (reservoir) without converting some work into heat.
> ![[Pasted image 20260525193536.png]]

- Heat from cold → hot **is** possible (refrigerator, heat pump), but not as the **sole** result; work input (or other effects in surroundings) is required.

> [!TIP]+ Clausius Inequality
> "All spontaneous processes are irreversible."
> $$
> \begin{align}
> \oint \frac{\delta Q_{\text{int,rev}}}{T}=0 &  & \oint \frac{\delta Q}{T_b}\leq0
> \end{align}
> $$
> Entropy: $dS=\delta Q_{\text{int,rev}}/T$; $\Delta S$ is a **state function**. See [[5. Entropy]].

## Irreversibility (summary)
See [[3. Reversible and Irreversible Processes]].

- **Internal:** friction, unrestrained expansion, chemistry, …
- **External:** finite $\Delta T$ heat transfer, …
- **Reversible:** no internal *and* no external irreversibility.

# Carnot Cycle (summary)

Details: [[4. Carnot Cycle]]

![[Pasted image 20260525203845.png]]

$$
\eta=1-\frac{T_C}{T_H} \qquad \eta_{\text{irr}}<\eta_{\text{rev}} \text{ (same reservoirs)}
$$

# Device Performance (summary)

Details: [[6. Isentropic Efficiency]]

- Turbines: actual work output is smaller than isentropic work.
- Compressors / pumps: actual work input is larger than isentropic work.
- Reversible open-system shaft work (steady, one reservoir, negligible $KE/PE$):

$$
\frac{\dot{W}_{CV}}{\dot{m}}\bigg|_{rev}=-\int_1^2 v\,dp
$$
