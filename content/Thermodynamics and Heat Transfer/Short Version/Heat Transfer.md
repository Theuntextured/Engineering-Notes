# Thermal Resistance

**Convection resistance**

$$
R_{\text{conv}}=\frac{1}{hA}
$$

**Conduction Resistance**

$$
R_{cond}=\frac{s}{kA}
$$

## 1D Steady State Heat Transfer Equation With Internal Generation 

$$
\frac{d^2T}{dx^2}+\frac{\dot{q}}{k}=0
$$

**Plate:**

$$
T_{max}-T_{s}=\frac{\dot{q}\cdot s^2}{2k}
$$

**Cylinder:**

$$
T_{max}-T_{s}=\frac{\dot{q}\cdot r^2}{4k}
$$

$$

$$

# Finned Heat Transfer

**Fin Parameter**:

$$
m=\sqrt{ \frac{hP}{kA_{c}} }
$$

**Temperature Profile:**

$$
T_{tip}=T_{f}+\frac{T_{0}-T_{f}}{\cosh {(mL)}}
$$

**Single Fin Heat Rate:**

$$
\dot{q}_{fin}=\sqrt{ hPkA_{c} }\cdot(T_{0}-T_{f})\tanh (mL)
$$

**Efficiency:**

$$
\eta_{f}=\frac{\tanh(mL)}{mL}
$$

**Effectiveness:**

$$
\epsilon_{f}=\frac{q_{fin}}{hA_{c}(T_{0}-T_{f})}
$$

---
**Biot Number:**

$$
\begin{align}
B_{i}=\frac{hL_{c}}{k} &  & L_{c}=\frac{V}{A_{s}}
\end{align}
$$

If $B_{i}<0.1$, then the internal conduction can be ignored, and only surface convection is considered.

**Cooling down object:**

$$
\frac{T(t)-T_{f}}{T_{i}-T_{f}}=e^{\frac{-hA_{s}}{mc}t}
$$
---
# Convection

$$
Nu=\frac{hL}{k_{fluid}}
$$

$$
Re=\frac{vL}{\nu}=\frac{\rho vD}{\mu}=\frac{\dot{m}D_{h}}{A\mu}
$$

$$
\begin{align}
Ra=Gr\cdot Pr &  & Pr=\frac{\mu c_{p}}{k} &  & Gr=\frac{{g\beta(T_{s}-T_{\infty})D^2}}{\nu^2} &  & \beta=-\frac{1}{\rho}\cdot \frac{{\partial \rho}}{\partial T}_{p}=\frac{1}{V}\cdot \frac{{\partial V}}{\partial T}_{p}
\end{align}
$$


**For ideal Gas:**

$$
\beta=\frac{1}{T_{f}}
$$

---
# Heat Exchangers

$$
\begin{align}
\varepsilon = \frac{{1-e^{ -NTU\cdot(1+C_{r}) }}}{1+C_{r}} &  & NTU=\frac{UA}{C_{min}} &  & C_{r}=\frac{C_{min}}{C_{max}}
\end{align}
$$

$$
\begin{align}
q=UA\Delta T_{lm} &  & \Delta T_{lm}=\frac{\Delta T_{1}-\Delta T_{2}}{\ln \left( \frac{\Delta T_{1}}{\Delta T_{2}} \right)}
\end{align}
$$


---

# Radiation Heat Transfer

$$
\sigma = 5.67 \times 10^{-8} \text{ W/(m}^2\text{K}^4\text{)}
$$
### Stefan-Boltzmann Law

$$
E_{b}=\sigma T^4
$$

### Reciprocity Relation

$$
A_{i}F_{ij}=A_{j}F_{ji}
$$

### Summation Rule

$$
\sum_{j=1}^{N} F_{ij} = 1
$$

### Net Heat Exchange (Two Black Surfaces)

$$
q_{12}=A_{1}F_{12}\sigma(T_{1}^4-T_{2}^4)
$$

### Surface Resistance

$$
R_{surf}=\frac{1-\epsilon}{\epsilon A}
$$

### Space Resistance

$$
R_{space}=\frac{1}{A_{i}F_{ij}}
$$

### Net Heat Transfer (Two Gray Surfaces)

$$
q_{12}=\frac{\sigma(T_{1}^4-T_{2}^4)}{\frac{1-\epsilon_{1}}{\epsilon_{1}A_{1}}+\frac{1}{A_{1}F_{12}}+\frac{1-\epsilon_{2}}{\epsilon_{2}A_{2}}}
$$

### Infinite Parallel Plates

$$
q=\frac{A\sigma(T_{1}^4-T_{2}^4)}{\frac{1}{\epsilon_{1}}+\frac{1}{\epsilon_{2}}-1}
$$

### Small Body in Large Enclosure

$$
q=\epsilon_{1}A_{1}\sigma(T_{1}^4-T_{2}^4)
$$

### Infinite Parallel Plates with One Shield

$$
q=\frac{A\sigma(T_{1}^4-T_{2}^4)}{\left(\frac{1}{\epsilon_{1}}+\frac{1}{\epsilon_{3}}-1\right)+\left(\frac{1}{\epsilon_{3}}+\frac{1}{\epsilon_{2}}-1\right)}
$$
