> [!ABSTRACT] Quick Stats
> * **Melting Point:** $660^\circ C$ (Softens at $150-200^\circ C$)
> * **Crystal Structure:** FCC (Face Centered Cubic) $\rightarrow$ **No ductile-to-brittle transition** (remains ductile at low temps)
> * **Density:** $2.7 \text{ g/cm}^3$ (vs $7.7$ for Fe) - *It is light!*
> * **Young's Modulus (E):** $70 \text{ GPa}$ (vs $210 \text{ GPa}$ for Fe) - *It is 1/3 as stiff as steel.*

---

## Why Aluminium? (Pros & Cons)

**The Good**
* **Conductivity:** High electrical conductivity ($62\%$ IASC). Good heat conductor.
* **Formability:** Easily formed by extrusion, forging, rolling. Can make intricate shapes due to FCC structure.
* **Corrosion Resistance:** Excellent due to a thin, strong oxide coating.
* **Machinability:** Good.

**The Bad**
* **Fatigue Strength:** Low. Be careful with cyclic loading.
* **Cost:** Sheet form is $\sim 4.5 \times$ mild steel cost.
* **Temperature:** Low melting point limits high-temp applications.

> [!WARNING] Critical Exam Concept: SCC
> Precipitation-hardened alloys can suffer from **Stress-Corrosion Cracking (SCC)** due to precipitate-free zones near grain boundaries. Do not forget this.

---

## Strengthening Mechanisms

How do we make soft aluminium strong?
* **Solid Solution Hardening:** Adding atoms that distort the lattice.
* **Cold Work (Strain Hardening):** Dislocation tangles.
* **Age Hardening (Precipitation):** The big one. Requires heat treatment.

$$\sigma_{ys} = \sigma_o + k d^{-1/2}$$
*(Hall-Petch relation: Smaller grains = Higher strength)*

---

## The Designation System (Wrought & Cast)

> [!TIP] Memorize the Series Logic
> The first digit tells you the **principal alloying element**.

### Wrought Alloys (4 Digits: xxxx)

| Series | Element | Treatable? | Main Characteristic |
| :--- | :--- | :--- | :--- |
| **1xxx** | Pure Al ($99\%+$) | No | Foil, electrical conductors. Weak. |
| **2xxx** | **Copper (Cu)** | **YES** | **Aircraft.** High strength, age-hardened. Not weldable. |
| **3xxx** | Manganese (Mn) | No | **Drink cans.** Ductile, good formability. |
| **4xxx** | Silicon (Si) | Some | **Pistons.** Forgeable, lowers melting point. |
| **5xxx** | **Magnesium (Mg)** | No | **Marine.** Best corrosion resistance. Weldable. |
| **6xxx** | **Mg + Si** | **YES** | **Structural.** Window frames. Good medium alloy, weldable. |
| **7xxx** | **Zinc (Zn)** | **YES** | **High Stress Aircraft.** Highest strength. Not weldable. |
| **8xxx** | Other (Li) | **YES** | Specialist (e.g., Al-Li for aerospace). |

> **Cast Alloys** use a decimal point (e.g., `3xx.x`). Most common is **Al-Si** eutectic for automotive castings.

### Practical Naming Examples
*How to read the code on the exam:*

**Example 1: AA 7075-T6** (Common aircraft alloy)
* **7:** Principal element is **Zinc**.
* **0:** No major modification to the original alloy limits (0 = original).
* **75:** Identifies the specific alloy in the 7xxx series.
* **T6:** Solution heat treated + **Artificially Aged** (Furnace).

**Example 2: AA 5083-H116** (Marine/Shipbuilding)
* **5:** Principal element is **Magnesium**.
* **0:** Original alloy limits.
* **83:** Specific alloy ID.
* **H1:** Cold worked only (Strain hardened).
* **16:** Specific degree of hardness/processing.

**Example 3: AA 1050** (Electrical wiring)
* **1:** Pure Aluminium ($99.00\%$ min).
* **0:** Original impurity limits.
* **50:** Indicates purity of $99.50\%$. (Last two digits in 1xxx series = decimal percentage above 99%).

---

## Temper Designations (The Suffixes)

This tells you the **history** of the metal.
* **F:** As Fabricated (Raw output).
* **O:** Annealed (Softest, lowest strength).

### H - Cold Worked (Strain Hardened)
*Used for Non-Heat Treatable alloys (1xxx, 3xxx, 5xxx)*
* **H1:** Cold worked only.
* **H2:** Cold worked + partially annealed.
* **H3:** Cold worked + stabilized.
* **Second Digit:** Indicates hardness (2 = 1/4 hard ... 8 = Hard).

### T - Heat Treated (The Important Ones)
*Used for Heat Treatable alloys (2xxx, 6xxx, 7xxx)*

> [!DANGER] Don't mix these up!
> * **T4:** Solution Heat Treated + **Natural Ageing** (Room temp).
> * **T6:** Solution Heat Treated + **Artificial Ageing** (Furnace).
> * **T3:** Solution + **Cold Work** + Natural Ageing.

---

## Age Hardening (Precipitation Hardening)
*Focus: 2xxx Series (Al-Cu)*

This is the primary way we strengthen high-performance aluminium. It is a process over time:

1.  **Solid Solution Treatment:** Cu is in solid solution.
2.  **GP Zones:** Cu forms clusters. Strain fields created.
3.  **$\theta''$ Precipitates:** *Coherent* precipitates. **PEAK AGED condition.** Maximum hardness.
4.  **$\theta'$ and $\theta$ (CuAl$_2$):** *Incoherent* precipitates. **Overaged.** Hardness drops.

> [!NOTE] The Curve
> The Yield Stress rises to a peak and then falls. Overaging (holding it in the oven too long) ruins the material strength.

---

## Applications Cheat Sheet

| Application | Series | Why? |
| :--- | :--- | :--- |
| **Cooking Foil** | 1xxx | Pure, ductile, corrosion resistant. |
| **Drink Cans** | 3xxx | Deep drawing capability (ductile). |
| **Airplane Fuselage** | 2xxx | High strength (but needs Alclad for corrosion). |
| **Airplane Wing Structures** | 7xxx | Highest strength available. |
| **Car Pistons** | 4xxx | Low thermal expansion, wear resistance (Si). |
| **Window Frames** | 6xxx | Extrudable, good corrosion resistance. |
| **Ship Hulls** | 5xxx | Saltwater corrosion resistance. |