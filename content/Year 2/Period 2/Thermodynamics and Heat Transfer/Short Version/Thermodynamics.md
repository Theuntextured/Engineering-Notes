# 1st Law of Thermodynamics

> [!IMPORTANT]+ For a process $A\to B$
> $$
> \begin{align}
> \text{Closed System:} &  & Q_{AB}-W_{AB}=\Delta U &  & W_{12}=\int_{V_{A}}^{V_{B}}p\cdot dV \\
> \text{Open System:} &  & \dot{Q}_{AB}-\dot{W}_{AB}=\dot{m}\cdot[\Delta h+\Delta ke+\Delta pe] &  & \underbrace{\dot{W}_{AB}=-\dot{m}\int_{p_{1}}^{p_{2}}v\cdot dp}_{\text{Internally reversible process, } \Delta pe\approx 0,\Delta ke\approx 0}
> \end{align}
> $$

> [!TIP]+ For a cycle
> 
> $$
> \begin{align}
> \text{Closed System:} &  & Q_{\text{cycle}}=W_{\text{cycle}} \\
> \text{Open System:} &  & \dot{Q}_{\text{cycle}}=\dot{W}_{\text{cycle}}
> \end{align}
> $$
> 

$$
Q=\int_{T_{1}}^{T_{2}}mc\,dT
$$

> [!CHECK]+ Polytropic Process
> 
> $$
> \begin{align}
> pV^n=\text{const}
> \end{align}
> $$
> 
> If the gas is ideal:
> 
> $$
> pV^k=\text{const},\,TV^{k-1}=const
> $$
> 
> Where $k$ is the **adiabatic index.** 

> [!SUMMARY]+ Gas Constants & Indices
> 
> $$
> \begin{align}
> R=c_{p}-c_{v} &  & k=\frac{c_{p}}{c_{v}}
> \end{align}
> $$


> [!WARNING]+ Efficiency
> $$
> \begin{align}
> \eta=\frac{W_{net}}{Q_{in}} &  & \eta=\frac{Q_{net}}{W_{in}}
> \end{align}
> $$
> > [!NOTE] Note that in the denominator, we exclude the outputs!

# 2nd Law of Thermodynamics

> [!TIP]+ For a Process $1\to 2$
> $$
> \begin{align}
> \underbrace{\sigma=\Delta S-\frac{Q_{12}}{T_{res}}\geq 0}  &  & \underbrace{\dot{\sigma}=\dot{m}\cdot \Delta S-\frac{\dot{Q}_{12}}{T_{res}}} \\
> \text{Closed System} &  & \text{Open System}
> \end{align}
> $$

> [!TIP]+ For a Cycle
> $$
> \begin{align}
> \underbrace{\sigma=-\sum_{j} \frac{Q_{j}}{T_{res,j}}\geq 0} &  & \underbrace{\dot{\sigma}=-\sum_{j} \frac{\dot{Q}_{j}}{T_{res,j}}\geq 0} \\
> \text{Closed System} &  & \text{Open System}
> \end{align}
> $$

> [!SUMMARY]+ Thermal Reswervoir
> $$
> \Delta S_{res}=\frac{Q_{12}}{T_{res}}\text{ or }\Delta \dot{S}_{res_{12}}=\frac{\dot{Q}_{12}}{T_{res}}
> $$

## Ideal Gas Energy

$$
E=mc_{v}T\implies Q=mc_{v}\Delta T
$$
---
# Rankine Cycle

## The Turbine (State 1 to 2)

> [!warning] Isentropic vs Actual
> Always calculate the mathematically perfect (isentropic) expansion first, then apply efficiency penalty.

Ideal Vapour Quality (if expanding into the wet region):

$$x_{2s} = \frac{s_1 - s_f}{s_g - s_f}$$

*Note: $s_1$ is the specific entropy of the steam entering the turbine.*

Ideal Specific Enthalpy at Exit:

$$
\begin{align}
h_{2s} &  = h_f + (x_{2s} \cdot h_{fg}) \\
 & = x_{2s}h_{g}+(1-x_{2s})h_{f}
\end{align}
$$

Actual Specific Enthalpy at Exit (using Isentropic Efficiency, $\eta_{is}$):

$$\eta_{is} = \frac{h_1 - h_2}{h_1 - h_{2s}}\implies h_2 = h_1 - [\eta_{is} \cdot (h_1 - h_{2s})]$$


## The Pump (State 3 to 4)

> [!info] Incompressible Fluids
> Because the water exiting the condenser is a liquid, we use specific volume and pressure difference instead of complex enthalpy tables to find the work.

Specific Pump Work:

$$
\begin{align}
v_{f} & =\text{const}\\
\therefore w_p  & = v_f \cdot (P_{boiler} - P_{condenser})
\end{align}
$$

*Note: Pressures must be in kPa to yield kJ/kg.*

## Cycle Performance Metrics

$$w_{net} = w_t - w_p$$

$$
\begin{align}
\eta_{th}  & = \frac{w_{net}}{q_{in}} \\
 & =1-\frac{q_{out}}{q_{in}}
\end{align}
$$

$$\text{BWR} = \frac{w_p}{w_t}$$

---
# Refrigeration

**Coefficient of Performance**

$$
\begin{align}
\beta=\frac{\dot{Q}_{in}}{|\dot{W}_{in}|} &  & \beta_{\text{carnot}} = \frac{T_{LO}}{\Delta T}
\end{align}
$$
---
## More Thermodynamic Cycles
#### Otto Cycle

1. Isentropic Compression
2. Isochoric Heat Addition (Combustion)
3. Isentropic Expansion
4. Isochoric Heat Release (Exhaust)

![[Pasted image 20260612192200.png]]

$$
\begin{align}
\eta & =1-\frac{1}{r^{k-1}} \\
 & =1-\frac{\Delta T_{\text{heat rekease}}}{\Delta T_{\text{heat addition}}}
\end{align}
$$
Where:

$$
r=\frac{V_{max}}{V_{min}}=\frac{v_{max}}{v_{min}}
$$
#### Diesel Cycle

1. Isentropic Compression
2. Isobaric Heat Addition (Fuel Ignition)
3. Isentropic Expansion
4. Isochoric Heat Release (Exhaust)

![[Pasted image 20260612192123.png]]

**Cut off Ratio:**

$$
r_{c}=\frac{v_{3}}{v_{2}}
$$

> Ratio between volume at end and start of combustion

$$
\begin{align}
\eta & =1-\left[ \frac{{r_{c}^k-1}}{k(r_{c}-1)} \right] \frac{1}{r^{k-1}} \\
 & =1-\frac{1}{k} \left[ \frac{{T_{4}-T_{1}}}{T_{3}-T_{2}} \right]
\end{align}
$$

#### Brayton-Joule Cycle

![[Pasted image 20260613154637.png]]

1. Isentropic compression (through compressor)
2. Isobaric heat addition (usually through combustion)
3. Isentropic expansion (through turbine)
4. Isobaric heat removal (exhaust)

$$
\eta=1-r_{p}^{\frac{1-k}{k}}
$$

Where:

$$
r_{p}=\frac{p_{\text{before compressor}}}{p_{\text{after compressor}}}=\frac{p_{\text{LO}}}{p_{\text{HI}}}
$$

#### Inverse Joule Cycle

![[Pasted image 20260614195757.png]]

$$
\begin{align}
\beta &  = \frac{q_{in}}{w_{net}} \\
 & = \frac{1}{r_{p}^{\frac{\gamma-1}{\gamma}}-1}
\end{align}
$$

1. Isentropic compression
2. Isobaric heat release
3. Isentropic expansion
4. Isobaric heat addition