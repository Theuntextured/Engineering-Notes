![[Technology of Metallic Materials/attachments/Pasted image 20260131162355.png]]

![[Technology of Metallic Materials/attachments/Pasted image 20260131162644.png]]

![[Technology of Metallic Materials/attachments/Pasted image 20260131162933.png]]



# Raw Costs for Stainless Steels

| Material                                 | Price in $/tonne |
| ---------------------------------------- | ---------------- |
| Scrap Iron                               | 149              |
| Chromium (as high-carbon ferro-chromium) | 1000             |
| Nickel                                   | 6755             |
| Molybdenum (As ferro-molybdenum)         | 10000            |
| Manganese (As ferro-manganese)           | 396              |
| Copper                                   | 2323             |
| Titanium (As ferro-titanium)             | 3465             |
| Niobium (As ferro-niobium)               | 15000            |

---
# Cottrell Atmospheres

A Cottrell atmosphere is a type of [[Technology of Metallic Materials/Defects\|defect]] that tends to occur most often in steels. It involves an edge dislocation creating space for carbon atoms in the section of the material in tension (Circled in red below).

![[Technology of Metallic Materials/attachments/Pasted image 20260130170356.png]]

The setup allows for carbon atoms to block dislocation movement. This is why in steel we have an upper and lower yield strength: as long as the carbon in Cottrell Atmospheres is intact and can prevent dislocation movement, the yield strength will be higher, but once these are broken, dislocations can move more easily and therefore $\sigma_{y}$ decreases to the lower value.

![[Technology of Metallic Materials/attachments/Pasted image 20260130170504.png]]


> [!note]- Why “Atmosphere?”
> The defect is called an atmosphere because it is not one single carbon ion sitting in the empty spaces, but a dense fog or cloud of atoms hovering around the dislocation line, locking it in place.
> Given this, we can say that the Cottrell Atmosphere is a cloud of point defects (the carbon atoms) around a line defect (the dislocation).


# High Strength Low Alloy Steels (HSLA)

![[Technology of Metallic Materials/attachments/Pasted image 20260130194100.png]]

# Non-Equilibrium Phase Diagram

![[Technology of Metallic Materials/attachments/graph1.png]]

![[Technology of Metallic Materials/attachments/graph2.png]]

> The above diagrams show a time vs temperature diagram of how different forms of steel are created.
> The first diagram shows hypoeutectoid steel (low carbon), while the second one shows hypereutectoid steel (high carbon)

## Austenitizers and Ferritizers

To control at what temperatures steel is stable in a certain form ($\alpha,\gamma,\delta$) we can add alloying elements to the steel. These are:
- Austenitizers
	- FCC $\gamma$ phase.
	- Increase temperature range at which austenite is stable.
	- $Ni,Mn,Co$ and weaker ones are $C,N,Cu$
	- Lower transformation temperatures
		- This is why austenitic stainless steel remains non-magnetic and ductile even at room temperatures and is therefore used in kitchens
- Ferritizers
	- BCC $\alpha$ phase
	- Widen temperature range at which ferrite is stable
	- $Cr,Si,Al,Mo,Ti,V$, or weaker ones being $B,S,Ze,Nb,Ce,Ta$
	- Raise transformation temperatures
		- Adding enough of these prevents phase transformation as a whole (especially chromium)

![[Technology of Metallic Materials/attachments/Pasted image 20260201153032.png]]
> The effect of austenitizers and ferritizers on eutectoid temperature and composition ($wt\%\ C$)

# Forms of Steel

> [!important]+ Cementite
> - Hard and brittle compound
> - $Fe_{3}C$
> - Contains 6.67 $wt\%\ C$
> - It is present in all steels when carbon amount is above 0.025% as: 
> 	- Lamellae (pearlite, bainite)
> 	- Needle (martensite)
> 	- Spheroids
> 	- Or as film around austenite GB (in iper-eutectoidic steels)
> - It is the reason steels are useful: in the form of impurities in softer forms, it pins the structure in place, allowing it to be harder than it would otherwise be.
> - Other alloying elements such as $Cr,Mo,Mn$ can be added, resulting in harder and more stable structures. These can form complex carbides or even pure alloy carbides.
> ![[Technology of Metallic Materials/attachments/Pasted image 20260201154224.png]]

> [!important]+ Graphite
> - Less dense than cementite and is NOT a metallic phase
> - It is promoted by:
> 	- Extremely slow cooling
> 	- High concentration of carbon ($>2\%$)
> 	- a small amount of silicon
> - It acts as a lubricant in machining operations due to its low internal friction, which increases with temperature
> - Can be found in lamellar (small filaments) which provides strong heat dissipation and dampening of vibrations and impacts. It can also take a bulls-eye (spherulitic) form when a strong spheroidizing agent is present (e.g. $Mg,Ce$), providing great mechanical resistance and ductility.

> [!important]+ Ferrite
> - BCC structure of almost pure iron
> - Very low solubility for carbon ($C\leq_{0}.0025\%$)
> - Iron atoms can be replaced in the crystal lattice by other alloying elements such as $Cr,Mo,Si$.
> ![[Technology of Metallic Materials/attachments/Pasted image 20260201154859.png]]

> [!important]+ Austenite
> - FCC structure of iron
> - Increased solubility of any interstitial atoms, such as carbon
> - $Fe$ can be replaced by $Ni,Mn$, which can integrate into the lattice without causing significant distortion.
> - ![[Technology of Metallic Materials/attachments/Pasted image 20260201155208.png]]

> [!important]+ Pearlite
> - Eutectoidic steel
> - Layers of ferrite ($\alpha$) and cementite in an alternating form
> - Formed when carbon-rich austenite is cooled at eutectoid temperature, and the speed of the cooling affects the width of the layers.
> - Is formed from seeds on grain boundaries.
> ![[Technology of Metallic Materials/attachments/Pasted image 20260201155408.png]]

**Summary:**

![[Technology of Metallic Materials/attachments/Pasted image 20260201214659.png]]



**Thermal expansion for iron:**

![[Technology of Metallic Materials/attachments/Pasted image 20260201214620.png]]

# Classification of Steels

![[Technology of Metallic Materials/attachments/Pasted image 20260201232708.png]]

## UNI EN 10020
The [UNI EN 10020](https://www.infotech-ved.it/wp-content/uploads/2021/01/CLASSIFICAZIONE-E-DESIGNAZIONE-DEGLI-ACCIAI.pdf) standard is used to categorize steels into:
- Alloyed: If one of the elements in the table below is over the limit (Plain carbon)
	- General use quality
	- High purity, specific hardenability requirements
- Unalloyed: If all elements below are within the limits.
	- Weldable, magnetic use, useful for rails
	- Useful for tools, high speed components

| **Element** | **Limit (%)** |
| ----------- | ------------- |
| Mn          | 1.65          |
| Cr          | 0.30          |
| Ni          | 0.30          |
| W           | 0.30          |
| V           | 0.10          |
| Mo          | 0.06          |

> [!example]-
> Stainless steels have over 10.5% $Cr$ and less than 1.2% $C$

> [!note]- UNI EN 10020 Official Document
![[Technology of Metallic Materials/attachments/CLASSIFICAZIONE-E-DESIGNAZIONE-DEGLI-ACCIAI.pdf]]
> Source: https://www.infotech-ved.it/wp-content/uploads/2021/01/CLASSIFICAZIONE-E-DESIGNAZIONE-DEGLI-ACCIAI.pdf
## UNI EN 10027-1

>[!note]- UNI EN 10027-1 Official Document
![[Technology of Metallic Materials/attachments/Classificazione_acciai_10027.pdf]]
> Source: http://www.emmeengineering.com/didattica/Acciaio/Acciaio_5/Classificazione_acciai_10027.pdf

The standard describes how steels can be named according to their use and properties.

In this standard, steels are named via the following naming convention:
`<Prefix>[Application Symbol]<Sub-category>[Mechanical/Physical Characteristic]<Additional Symbols>`
For example:
```
S235JR

S: Structural Use
235: 235 MPa Yield strength (Min.), from S category
JR: Can take a 27J impact (J) without breaking in a Charpy V-notch test at room temperature (R). Defined by UNI EN 10025 standard.
```
[Further reading about UNI EN 10025](https://www.collegiotecniciacciaio.it/wp-content/uploads/simple-file-list/SCHEDE-TECNICHE-CTA/SCHEDA-TECNICA-Norma-EN-10025.pdf)


<table>
  <thead>
    <tr>
      <th>Group</th>
      <th>Prefix</th>
      <th>Application Symbol</th>
      <th>Mechanical/Physical Characteristics</th>
      <th>Additional Symbols</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="12"><strong>Group 1</strong><br>Steels designated by application and mechanical/physical properties</td>
      <td rowspan="12"><strong>G</strong> = Cast Steel (if applicable)</td>
      <td><strong>S</strong> = Structural applications</td>
      <td>Min. Yield Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>P</strong> = Pressure purposes</td>
      <td>Min. Yield Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>L</strong> = Line pipe</td>
      <td>Min. Yield Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>E</strong> = Engineering / Machine construction</td>
      <td>Min. Yield Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>B</strong> = Reinforced concrete</td>
      <td>Characteristic Yield Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>Y</strong> = Pre-stressing concrete</td>
      <td>Min. Tensile Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>R</strong> = Rails</td>
      <td>Min. Tensile Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>H</strong> = Cold rolled flat products, high strength for cold forming</td>
      <td>Min. Yield Strength (MPa)<br><em>OR</em><br>Min. Tensile Strength (MPa) (if followed by 'T')</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>D</strong> = Flat products for cold forming</td>
      <td>
        <strong>C</strong> = Cold rolled<br>
        <strong>D</strong> = Hot rolled for immediate cold forming<br>
        <strong>X</strong> = Rolling condition not specified
      </td>
      <td>Two symbols characterizing the steel (defined by the responsible body)</td>
    </tr>
    <tr>
      <td><strong>T</strong> = Tinmill products (Packaging)</td>
      <td>Hardness (HR 30 Tm) <em>OR</em> Nominal Yield Strength (MPa)</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>M</strong> = Magnetic steels</td>
      <td>
        100 &times; Specific Loss (W/kg)<br>
        - (hyphen)<br>
        100 &times; Product Thickness (mm)
      </td>
      <td>
        <strong>A</strong> = Non-oriented grain<br>
        <strong>D</strong> = Semi-finished (non-alloy)<br>
        <strong>E</strong> = Semi-finished (alloy)<br>
        <strong>N</strong> = Normal grain oriented<br>
        <strong>S</strong> = Low loss grain oriented<br>
        <strong>P</strong> = High permeability grain oriented
      </td>
    </tr>
  </tbody>
</table>

### S Group

The number in the middle indicates min. Yield strength for the steel.

Usually for group S, the final two characters are one of:

| First Character | Meaning of First Character | Second character | Meaning of Second Character |
| :-------------: | :------------------------: | :--------------: | :-------------------------: |
|        J        |            >27J            |        R         |   20°C (Room temperature)   |
|        K        |            >40J            |        0         |             0°C             |
|        L        |            >60J            |        2         |            -20°C            |
|                 |                            |        3         |            -30°C            |
|                 |                            |      $[n]$       |          $-10n °C$          |

### D Group
Deep drawing sheets

![[Technology of Metallic Materials/attachments/Pasted image 20260201225304.png]]

### H Group
High strength deep drawing sheets
![[Technology of Metallic Materials/attachments/Pasted image 20260201225417.png]]

---

## Naming Based on Chemical Composition

|                 Type                  |                                       Syntax Rule                                       |   Example    |                How to read it                 |
| :-----------------------------------: | :-------------------------------------------------------------------------------------: | :----------: | :-------------------------------------------: |
|               Non-Alloy               |                                 $C[C\ wt\% \times 100]$                                 |    $C45$     |                   0.45% $C$                   |
|               Low Alloy               | $[C\ wt\% \times 100]+[\text{Elements in ascending order of wt. \%}]+[\text{Code No.}]$ |  $42CrMo4$   |      0.42% $C$<br>1% $Cr$<br>Trace $Mo$       |
|   High Alloy (One element with >5%)   |                 $X+[C\times_{1}00]+[\text{Elements}]+[\text{Real \%}]$                  | X100CrMoV5-2 | 1% $C$<br>5% $Cr$<br>2% $Mo$<br>Traces of $V$ |
| Rapid Steels (High Speed Steels - HS) |                          $\text{HS [\%W]-[\%Mo]-[\%V]-[\%Co]}$                          |  HS 6-5-3-8  |    6% $W$<br>5% $Mo$<br>3% $V$<br>8% $Co$     |

Code numbers are based on the following table:

| Elements           | Factor (Divide by) |
| ------------------ | ------------------ |
| $Cr,Ni,Mn,Si,W,Co$ | 4                  |
| $Al,Mo,Ti,V,Cu$    | 10                 |
| $P,S,N$            | 100                |
| $B$                | 1000               |
### Examples

**Tempering Steels**

|**Grade**|**S (%)**|**C (%)**|**Mn (%)**|**Cr (%)**|**Mo (%)**|**P (%)**|
|---|---|---|---|---|---|---|
|**C45E**|< 0.035|0.42 - 0.5|0.5 - 0.8|-|-|< 0.035|
|**C45R**|0.02 - 0.08|0.42 - 0.5|0.5 - 0.8|-|-|< 0.035|
|**42CrMo4**|< 0.035|0.38 - 0.45|0.6 - 0.9|0.9 - 1.2|0.15 - 0.3|< 0.035|
|**42CrMoS4**|0.02 - 0.08|0.38 - 0.45|0.6 - 0.9|0.9 - 1.2|0.15 - 0.3|< 0.035|

**Carburizing Steels**

|**Grade**|**S (%)**|**C (%)**|**Mn (%)**|**Cr (%)**|**Ni (%)**|**Mo (%)**|
|---|---|---|---|---|---|---|
|**C10E**|< 0.035|0.07 - 0.13|0.3 - 0.6|-|-|-|
|**C10R**|0.02 - 0.04|0.07 - 0.13|0.3 - 0.6|-|-|-|
|**20NiCrMo2-2**|< 0.035|0.17 - 0.23|0.65 - 0.95|0.35 - 0.7|0.4 - 0.7|0.15 - 0.25|
|**20NiCrMoS2-2**|0.02 - 0.04|0.17 - 0.23|0.65 - 0.95|0.35 - 0.7|0.4 - 0.7|0.15 - 0.25|

**Tool Steel**

| **Grade**       | **C (%)**   | **Mn (%)** | **Cr (%)** | **Mo (%)** | **V (%)**   | **Si (%)** |
| --------------- | ----------- | ---------- | ---------- | ---------- | ----------- | ---------- |
| **X100CrMoV5**  | 0.95 - 1.05 | 0.2 - 0.6  | 4.8 - 5.5  | 0.9 - 1.2  | 0.15 - 0.35 | 0.1 - 0.4  |
| **X38CrMoV5-3** | 0.35 - 0.4  | 0.3 - 0.5  | 2.7 - 3.2  | 2.7 - 3.2  | 0.4 - 0.6   | 0.3 - 0.5  |
****
## AISI/SAE Equivalents
|**Series**|**Type / Main Alloy**|**Description**|
|---|---|---|
|**10XX**|Plain Carbon|Plain carbon steels|
|**11XX**|Free machining S|Low carbon, added Sulfur|
|**12XX**|Free machining S, P|Added Sulfur and Phosphorus|
|**13XX**|Mn|Manganese steels|
|**2XXX**|Nickel (Ni)|Increases UTS without reducing toughness.|
|**3XXX**|Ni-Cr|Highly tough and ductile.|
|**40XX**|Mo|Molybdenum steels|
|**41XX**|Cr-Mo|Strong carbide former, prevents temper embrittlement.|
|**43XX**|Ni-Cr-Mo|High strength alloy.|
|**51XX**|Cr|Strong ferrite strengthener; increases wear resistance.|
|**86XX+**|Ni, Cr, Mo, V, Si|Complex alloys for high specific strength.|

---
# Hardenability

> [!important]+ Definition
> How deep hardness goes into the core.
> * *High Hardenability:* The center of a thick bar gets just as hard as the surface.
> * *Low Hardenability:* The surface is hard, but the core remains soft.
> 
> The unit technically is $m$ or $cm$, but it is not often used in its pure form.

Hardenability shifts the TTT curve to the right.

**The Standard Test (Jominy End Quench):**
1.  Heat a steel bar to Austenite.
2.  Spray water on **one end only**.
3.  Measure hardness along the bar.
    * The “hardened depth” is where the structure drops to **50% Martensite**.

Adding **$Mo, Mn, Cr$** increases hardenability, allowing larger parts to be hardened all the way through.

![[Technology of Metallic Materials/attachments/Pasted image 20260204155253.png]]

---
# Stainless Steels

>[!important]+ What Makes Steel "Stainless"?
For a steel to be considered "stainless," it must contain **at least 11.5% Chromium**.
>
Why? Because at this concentration, Chromium reacts with Oxygen to form a continuous, invisible, and self-healing [[Technology of Metallic Materials/Corrosion#Coatings & Active Protection\|passive film]] ($Cr_2O_3$) on the surface. If you scratch it, it reforms immediately (provided there is oxygen).

* **The Enemy:** Reducing environments (lack of oxygen) or chlorides ($Cl^-$) which break the film.
* **The Fix:** Alloying elements like Nickel (Ni) and Molybdenum (Mo).

---
## The Schaeffler Diagram

This is the map we use to predict the structure of a stainless steel (especially after welding). It plots **Chromium Equivalent** against **Nickel Equivalent**.

* **X-Axis ($Cr_{eq}$):** $\%Cr + \%Mo + 1.5\%Si + 0.5\%Nb$
* **Y-Axis ($Ni_{eq}$):** $\%Ni + 30\%C + 0.5\%Mn$

By calculating these two values, you can see if your steel will be Martensitic, Ferritic, Austenitic, or a mix (Duplex).

![[Technology of Metallic Materials/attachments/Pasted image 20260204180240.png]]

---

## The Families of Stainless Steel

### Ferritic SS
* **Composition:** High Cr (12-30%), Low C, No Ni.
* **Properties:** Magnetic. Good corrosion resistance (better than [[Technology of Metallic Materials/Overview of Steels#Martensitic SS]]).
* **Weakness:** Brittle at low temps (DBTT). Grain growth during welding reduces toughness.
* **Use:** Exhaust systems, cheaper chemical equipment.
* Series 400
	* E.g. AISI 430

### Martensitic SS
* **Composition:** Medium Cr (12-17%), High C (>0.1%).
* **Properties:** Can be quenched and tempered! High hardness and strength. Magnetic.
* **Weakness:** Lowest corrosion resistance of the bunch. Hard to weld (cracking risk).
* **Use:** Knife blades, surgical tools, shafts.
* Series 400
	* E.g. AISI 410, 420

### 3. Austenitic SS
* **Composition:** Cr (16-26%) + Ni (6-22%).
* **Properties:** Non-magnetic. Excellent corrosion resistance. High toughness (no DBTT — good for cryogenics). Highly ductile.
* **Series 300.**  Examples:
    * **AISI 304:** The standard “18/8” stainless. Kitchen sinks, food industry.
    * **AISI 316:** Adds **Molybdenum (2-3%)**. This drastically improves resistance to chlorides (saltwater) and pitting.
* **Weakness:** Expensive (Ni price). Susceptible to SCC (Stress Corrosion Cracking).

### 4. Duplex SS (e.g., 2205)
* **Structure:** A roughly 50/50 mix of Ferrite and Austenite.
* **Properties:** Best of both worlds. Higher strength than Austenitic, better SCC resistance.
* **Use:** Heat exchangers, desalination plants.
* E.g. AISI 2205

---

## Pitting Resistance (PREN)

How do we know if a steel will survive in seawater? We calculate the **Pitting Resistance Equivalent Number**.

$$PREN = \%Cr + 3.3 \cdot (\%Mo + 0.5\%W) + 16 \cdot \%N$$

* **Rule of Thumb:**
    * **PREN > 40:** "Superduplex" or "Superaustenitic" (Safe for severe seawater use).
    * Nitrogen (N) is extremely potent here (multiplier of 16!).

---

## Sensitization

This is the most common failure mode for Austenitic steels (like 304) after welding.

**The Mechanism:**
1.  Heat the steel to **500-800°C** (e.g., in the Heat Affected Zone of a weld).
2.  Carbon loves Chromium. They react to form **Chromium Carbides** ($Cr_{23}C_6$) at the grain boundaries.
3.  These carbides suck the Chromium out of the surrounding metal.
4.  The local Chromium level drops below 11.5% (the “Depleted Zone”).
5.  **Result:** The grain boundaries are no longer stainless. They corrode rapidly (Intergranular Corrosion).

**The Solutions:**
1.  **Low Carbon Grades:** Use "L" grades (e.g., **304L**, **316L**) where $C < 0.03\%$. Less carbon = less carbides.
2.  **Stabilization:** Add elements that love Carbon even more than Chromium does, like **Titanium (Ti)** or **Niobium (Nb)**.
    * *Example:* AISI 321 (Ti stabilized) or AISI 347 (Nb stabilized).

![[Technology of Metallic Materials/attachments/Pasted image 20260204181624.png]]