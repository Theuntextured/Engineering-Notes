# Heat Treatment of Steels
*Conventional heat treatments for Hypo- and Hyper-eutectoid steels. The goal is to modify microstructure (Grain size, phase distribution) to alter mechanical properties.*

> [!important]+ Reminder from [[Technology of Metallic Materials/Overview of Steels#Non-Equilibrium Phase Diagram]]
> * **$A_1$:** Eutectoid temperature (~727°C). Boundary between Austenite and Pearlite.
> * **$A_3$:** Upper critical temperature for **Hypo**-eutectoid steels (Austenite limit).
> * **$A_{cm}$:** Upper critical temperature for **Hyper**-eutectoid steels (Cementite solubility limit).

![[Technology of Metallic Materials/attachments/Pasted image 20260203164131.png]]

---

## Hypo-Eutectoid Steels ($C < 0.77\%$)

### Normalizing
* **Process:** Heat to **$A_3 + 55^\circ\text{C}$** (Austenitization) $\to$ **Air Cool**.
* **Result:** Moderate grain refinement.
* **Properties:** Harder and stronger than annealed; good mechanical properties at low cost.
* **Microstructure:** Fine Pearlite + Ferrite.

### Full Annealing
* **Process:** Heat to **$A_3 + 30^\circ\text{C}$** $\to$ **Furnace Cool** (Very slow).
* **Result:** Maximum chemical homogenization and softening.
* **Properties:** Maximum ductility, lowest hardness.
* **Microstructure:** Coarse Pearlite + Ferrite.

### Process Annealing
* **Process:** Heat to **$80-170^\circ\text{C}$ below $A_1$**.
* **Result:** Recrystallization of ferrite without phase transformation.
* **Use Case:** Restoring ductility after cold working (strain hardening recovery).

---

## Hyper-Eutectoid Steels ($C > 0.77\%$)

### Normalizing
* **Process:** Heat above **$A_{cm}$** $\to$ Air Cool.
* **Goal:** Break up the brittle Cementite network at grain boundaries.

### Spheroidizing
* **Process:** Pendulum heating (oscillating) around **$A_1$**.
* **Result:** Spheroidization of Pearlite and Cementite.
* **Properties:** The **softest, toughest** possible condition for high-carbon steel.
* **Use Case:** Essential for machinability of high-carbon steels.

---

## Overview of Heat Treatments
* **Austenitization:** Holding at $T$ to dissolve C into $\gamma$-Fe (max solubility/homogeneity).
* **Annealing:** Diffusion-driven. Max softening. Equilibrium microstructure.
* **Normalizing:** Air-cooled. Slightly non-equilibrium. Moderate refinement.

![[Technology of Metallic Materials/attachments/Pasted image 20260203164317.png]]

## Isothermal H.T. On a TTT/CCT Diagram

![[Technology of Metallic Materials/attachments/Pasted image 20260203164503.png]]

> [!check]+ Bainite
> A microstructure of Ferrite and Cementite that forms between the temperature ranges of Pearlite and Martensite (roughly 250°C – 550°C). While martensite is BCT, bainite is BCC.
>
**Formation:** Created via **Austempering** (isothermal holding). You cool the steel fast enough to miss the Pearlite nose, but hold it above the Martensite start ($M_s$) line until it fully transforms.
>
**The Two Types:**
> - **Upper Bainite (400°C – 550°C):** Forms at higher temps. Looks "feathery." The carbides precipitate *between* the ferrite plates. It's tough, but lower bainite is usually better.
> - **Lower Bainite (250°C – 400°C):** Forms at lower temps. Looks like needles (acicular). The carbides precipitate *inside* the ferrite needles. High strength and high toughness.
>
**Why it matters:**
It offers a unique balance. You get hardness similar to tempered martensite but with better ductility and toughness. Plus, since you don't do a violent quench to room temperature, you avoid the internal stresses and cracking risks associated with Martensite.
>
>![[Technology of Metallic Materials/attachments/Pasted image 20260203165503.png]]

> [!note]
> TTT (Time-temperature-Transformation) diagrams show transformations in isotermal environments. In the real world, this is impossible, since materials cannot change temperature instantly.
> CCT (Continuous Cooling Transformation) diagrams show the real world since things cool down gradually. Typically, reactions are slower than in an ideal world, so in a CCT diagram reactions are shifter bottom-right with respect to a TTT diagram.(reactions are slower and happen at lower temperatures).
> 
> ![[Technology of Metallic Materials/attachments/Pasted image 20260203171337.png]]


---
# Quenching

> [!bug]+ Quench Severity Coefficient aka. H-Value
> Describes how aggressively a medium (the liquid the metal is quenched in) cools down the material, with 1 being the baseline and the value for still water.
>
> $Q=HA\Delta T$
>
>| Quench Medium | Agitation? | H Coefficient | Cooling Rate (°C/s)* |
| :--- | :--- | :---: | :---: |
| **Oil** | No | 0.25 | 18 |
| **Oil** | Yes | 1.0 | 45 |
| **Water ($H_2O$)** | No | 1.0 | 45 |
| **Water ($H_2O$)** | Yes | 4.0 | 190 |
| **Brine** | No | 2.0 | 90 |
| **Brine** | Yes | 5.0 | 230 |
>*\*Cooling rate measured at the centre of a 1-inch bar.*
