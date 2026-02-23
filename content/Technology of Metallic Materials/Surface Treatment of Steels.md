---
publish: true
cssclasses: ""
---

## Hardening by Carburizing
The primary goal here is to achieve a surface that is hard and wear-resistant while maintaining a tough, ductile core to absorb shock.

**The Mechanism**
This process exploits specific metallurgical factors:
* Martensite hardness increases as the carbon percentage increases.
* Martensite forms from austenite upon quenching.
* Carbon is highly soluble in austenite.
* The diffusion/absorption rate increases significantly with temperature.

**Process Parameters**
* **Temperature ($T_c$):** $870-950^{\circ}C$.
* **Time:** $10-20$ hours.
* **Applicable Materials:** Plain carbon steels ($<0.2\% C$) and low carbon low alloy steels.

**Applications**
Used for components requiring durability under load, such as gears, shafts, bearings, and piston rods.

**Outcome**
* A carbon concentration profile develops along the thickness, achieving maximum Vickers Hardness (HV) on the surface.
* The austenite transforms into martensite via oil quenching.

---

## Hardening by Nitriding
Unlike carburizing, this process aims for an *extremely* hard surface while retaining a tough core.

**The Mechanism**
* Nitrogen forms very hard compounds (nitrides) with Iron.
* Nitrogen solubility in ferrite is very low.
* At ferrite stability temperatures, diffusion is slow, and the formation of nitrides inhibits further Nitrogen diffusion.

**Process Parameters**
* **Temperature ($T_N$):** $500-600^{\circ}C$.
* **Time:** Approx. 70 hours (can range 40-100h).
* **Chemical Reaction:** Ammonia dissociates: $2NH_3 \Rightarrow 2N + 3H_2$. Atomic Nitrogen then dissolves into the steel.

**Applicable Materials**
* Nitriding steels: Plain medium carbon steel ($0.4-0.6\% C$) and medium carbon low alloy steels (tempered/semi-finished).
* Common alloying elements: Al, Cr, V, Mo.

**Structure of the Nitrided Layer**
* **Outer Layer:** $(Fe,Al,Cr)_2N$.
* **Inner Layer:** $(Fe,Al,Cr)_4N$.
* **Depth:** A thin layer, typically $0.2-0.3$ mm.
* **Hardness:** Very high superficial hardness ($\sim 1100$ HV).

![[Technology of Metallic Materials/attachments/Pasted image 20260204165230.png]]


### The Fe-N Metastable Phase Diagram

![[Technology of Metallic Materials/attachments/Pasted image 20260204165410.png]]

**Nitriding Steel Compositions**
Specific alloys are required for optimal nitriding results.

| Steel Type        | %C   | %Si  | %Mn  | %Cr  | %Mo  | %Al  | Hardness after Nitriding |
| :---------------- | :--- | :--- | :--- | :--- | :--- | :--- | :----------------------- |
| **30 Cr Mo 10**   | 0.30 | 0.35 | 0.60 | 2.50 | 0.40 | -    | 650 HV                   |
| **38 Cr Al Mo 7** | 0.38 | 0.30 | 0.60 | 1.70 | 0.25 | 1.0  | 1050 HV                  |
| **42 Cr Al Mo 7** | 0.42 | 0.35 | 0.55 | 1.70 | 0.35 | 0.40 | 900 HV                   |

---

## Comparison: Nitriding Steels vs. Carburizing

**Performance Comparison**
* **Nitrided Steel:** Achieves higher surface hardness (up to 1000-1200 HV) but the depth of penetration is shallow ($<0.6$ mm).
* **Carburized Steel:** Lower peak surface hardness ($\sim 800$ HV) but maintains hardness to a greater depth ($>1.0$ mm).

![[Technology of Metallic Materials/attachments/Pasted image 20260204165929.png]]

**Harris' Formula for Penetration Depth**
To calculate the depth of the treatment:
$$\text{Depth} (mm) = 660 \cdot \sqrt{t} \cdot e^{-\frac{8287}{T}}$$
Where $T$ is temperature in **Kelvin** and $t$ is time in **hours**.

**Post-Treatment Processing**

| Process Step | Carburized Parts | Nitrided Parts |
| :--- | :--- | :--- |
| **Pre-treatment** | Normalizing + work hardening annealing | Normalizing + Work hardening annealing |
| **Machining** | Roughing (medium thickness) | Roughing (medium thickness) |
| **Main Process** | Carburizing | Tempering |
| **Hardening** | Quenching + tempering at $150^{\circ}C$ | Finish Nitriding |
| **Finishing** | Finish by grinding | Finish by grinding |


---

## Induction Hardening

> [!important]+ Definition
The process uses alternating current to generate a magnetic field, which creates induced currents in the workpiece. This results in localized thermal energy.

**Current Penetration Depth ($\delta$)**
The depth of heating is controlled by the frequency:
$$\delta \cong \sqrt{\frac{\rho}{\pi \mu f}}$$


![[Technology of Metallic Materials/attachments/Pasted image 20260204170710.png]]

**Inductor Types**
Various shapes exists for different geometries:
* Single-shot coils for cylindrical parts.
* Shaped coils for slideways or gears.


> [!example]- Slideways vs Coils
> ![[Technology of Metallic Materials/attachments/Pasted image 20260204170826.png]]

**Hardness Profiles**
Induction hardening creates a sharp transition in hardness. For example, in Tempered 4140 steel, hardness holds steady around 700 HV before dropping sharply to the core hardness ($\sim 330$ HV) at a specific depth determined by the induction frequency and speed.

![[Technology of Metallic Materials/attachments/Pasted image 20260204170935.png]]

---

## Heat vs. Chemical Surface Treatments Overview

All surface heat treatments generally confer a **compressive stress state** on the surface, which increases fatigue resistance.

**Process Comparison Table**

| Process | Steel Type | Component | Conditions |
| :--- | :--- | :--- | :--- |
| **Induction (3 kHz)** | 0.38% C | Axle | Water Quenched, Tempered at $210^{\circ}C$ |
| **Flame Hardening** | 0.67% C | Wheel | Water Quenched, Tempered at $490^{\circ}C$ |
| **Carburizing** | 0.2% C (Ni-Cr-Mo alloy) | Gear | Oil Quenched, Tempered at $200^{\circ}C$ |
| **Laser (15 kW)** | 0.43% C (Mn alloy) | Gear | Self Quenched |
| **Nitriding** | 0.2% C (Cr-V-Al alloy) | Gear | Process carried out at $570^{\circ}C$ |


**Residual Stress Profiles**
* **Nitriding (Turferrit/Soft Gas):** Creates the highest compressive residual stress ($-600$ to $-1000$ MPa) right at the surface.
* **Induction:** Creates deep compressive stress, but lower magnitude at the surface compared to nitriding.
* **Laser:** High surface hardness but shallower stress profile.

![[Technology of Metallic Materials/attachments/Pasted image 20260204171152.png]]

---

## Weldability and Heat Affected Zone (HAZ)

When welding steels, the thermal cycle alters the microstructure adjacent to the weld. This is the Heat Affected Zone (HAZ).

**Structure of the Welding Zone**
1.  **Solidified Weld:** The melt zone.
2.  **Grain Growth Zone:** Liquid + $\gamma$ (austenite) transition.
3.  **Recrystallized Zone:** $\gamma$ region.
4.  **Partially Transformed Zone:** $\gamma + Fe_3C$.
5.  **Tempered Zone:** Below $A_1$ temperature.
6.  **Unaffected Base Material:** Original microstructure.

![[Technology of Metallic Materials/attachments/Pasted image 20260204171519.png]]

**Microstructural Evolution**
The final structure depends heavily on the [[Technology of Metallic Materials/Overview of Steels#Hardenability\|hardenability]] of the steel.
* **At $T_{max}$:** The structure becomes Austenite ($\gamma$) near the melt line.
* **Cooling (Low Hardenable Steel):** Reverts to Pearlite and Ferrite ($\alpha$).
* **Cooling (High Hardenable Steel):** Forms **Martensite**, which is brittle and prone to cracking.

**Weldability Criteria**
* To be weldable, steel must have **low hardenability** (low alloying elements).
* Steels up to $0.4\% C$ are weldable, but caution is needed for higher carbon contents.
* **Risk:** Cracks can form underneath the welding bead in the HAZ.

![[Technology of Metallic Materials/attachments/Pasted image 20260204171838.png]]

---

## Summary Tables

### Chemical Surface Treatments Summary

| Process | Compound | Temp ($^{\circ}C$) | Time (h) | Thickness ($\mu m$) | Hardness (HV) | Distortion |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Nitriding** | Fe-N | 500-550 | 1-70 | 50-100 | 700-1000 | Min |
| **Nitro-carb.** | Fe-(C,N) | 550-650 | 1-6 | 50-200 | 700-1000 | Min |
| **Boriding** | Fe-B | 600-1000 | 1-4 | 50-500 | 1000-1800 | High |
| **Carburizing** | Fe-C | 700-1050 | 1-46 | 100-7000 | 750-950 | High |
| **Process QUAD** | CrCN, VCN, TiCN | 400-700 | 1-8 | 5-20 | 1200-2500 | Min |


### Wear Resistant Ceramic Coatings

| Process           | Surface Layer  | Method         | Surface T ($^{\circ}C$) | Thickness ($\mu m$) | Hardness (HV) | Distortion |
| :---------------- | :------------- | :------------- | :---------------------- | :------------------ | :------------ | :--------- |
| **Cr hard**       | Cr             | Electrolysis   | 50-80                   | 20-50               | 700-800       | Low        |
| **Thermal CVD**   | TiC, TiCN, TiN | Gas            | 800-1100                | 3-15                | 1500-2000     | High       |
| **Plasma CVD**    | TiC, TiN       | Arc in vacuum  | 300-600                 | 1-6                 | 1500-2000     | Low        |
| **PVD**           | TiN, CrN       | N in vacuum    | 300-600                 | 1-6                 | 2000-4000     | Low        |
| **Flame coating** | Ni, Cr, B, Si  | Powder melting | 1000-1100               | 500-2000            | 600-800       | High       |
| **Stellite**      | Ni, Cr, B, Si  | Melting (arc)  | $T_{fus}$               | 2000-5000           | 300-900       | High       |