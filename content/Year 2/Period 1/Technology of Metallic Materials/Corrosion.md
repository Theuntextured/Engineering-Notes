## Dry vs. Wet Corrosion
### Dry Corrosion (High Temperature Oxidation)
* **Environment:** Vapours and gases at **High Temperatures**.
* **Mechanism:** Direct chemical reaction between the metal and the gas (usually $O_2$).
* **Process:** $M + O_2 \rightarrow Oxide$.
* **Outcome:** Formation of an oxide film (scale).
    * Adhesion and porosity of the scale determine if it protects the metal or allows further attack.

### Wet Corrosion (Electrochemical)
* **Environment:** Humidity (liquid $H_2O$) + Oxygen at **Room Temperature**.
* **Mechanism:** Electrochemical process involving an electrolyte.
* **Components Required:**
    1.  **Anode:** Gives up electrons (Corrodes).
    2.  **Cathode:** Accepts electrons (Protected).
    3.  **Electrolyte:** Conducts ions ($M^{2+}$).
    4.  **Electrical Connection:** Conducts electrons ($e^-$).
* **Outcome:** Loss of material (crater formation) at the anode; often electroplating or byproduct formation at the cathode.

![[Pasted image 20260204172708.png]]

---

## The Electrochemical Reactions

> [!warning] Stopping Wet Corrosion
> For wet corrosion to occur, two simultaneous reactions must happen. If you stop one, you stop the corrosion.

### The Anodic Reaction (Oxidation)
This is where the metal is lost. The metal dissolves into the electrolyte as ions.
$$M \rightarrow M^{n+} + ne^-$$
*Examples:*
* $Fe \rightarrow Fe^{2+} + 2e^-$
* $Zn \rightarrow Zn^{2+} + 2e^-$ 

### The Cathodic Reaction (Reduction)
This occurs at the surface that *does not* corrode. The specific reaction depends on the environment's pH and oxygen content.

| Environment       | Condition       | Reaction                                 |
| :---------------- | :-------------- | :--------------------------------------- |
| **Acidic**        | High $H^+$ ions | $2H^+ + 2e^- \rightarrow H_2$            |
| **Acidic**        | Dissolved $O_2$ | $O_2 + 4H^+ + 4e^- \rightarrow 2H_2O$    |
| **Neutral/Basic** | Dissolved $O_2$ | $O_2 + 2H_2O + 4e^- \rightarrow 4(OH)^-$ |

*Note:* Metal ions can also be reduced (Electroplating): $M^{n+} + ne^- \rightarrow M$.

---

## Classification of Corrosion Phenomena

![[Pasted image 20260204173555.png]]


### 1. Uniform Corrosion
* **Appearance:** Even removal of metal across the surface.
* **Mechanism:** Micro-corrosion cells shift randomly over time.
* **Risk:** Greatest destruction by mass, but **least dangerous** technically because it is predictable and easy to measure.

### 2. Galvanic (Bimetallic) Corrosion
* **Mechanism:** Two dissimilar metals in electrical contact in an electrolyte.
* **The Law:** The **less noble** (anodic) metal corrodes; the **more noble** (cathodic) metal is protected.
* **Driving Force:** The difference in electrical potential (Voltage) between the metals.

> [!warning]+ The “Area Ratio” Effect
> The rate of corrosion is determined by the current density ($i = I/Area$).
> * **Big Cathode + Small Anode = DISASTER.**
>     * The massive cathode demands a huge flow of electrons. The tiny anode must corrode furiously to supply them.
>     * *Example:* Steel rivets in a Copper plate $\rightarrow$ Rivets disintegrate rapidly.
> * **Small Cathode + Large Anode = Safe.**
>     * The corrosion is spread out over a large area and is sluggish.

### 3. Localized Corrosion
These are dangerous because the overall mass loss is low, but the structural damage is high.

#### Crevice Corrosion
* **Location:** Narrow gaps (crevices) under bolts, gaskets, or deposits.
* **Mechanism:**
    1.  Oxygen is depleted inside the crevice.
    2.  The crevice becomes strictly Anodic (dissolution of metal).
    3.  The area outside remains Cathodic (plenty of $O_2$).
    4.  Positive metal ions accumulate in the crevice, attracting negative ions ($Cl^-$) and lowering pH (creating acid), which accelerates the attack.

![[Pasted image 20260204173724.png]]

#### Pitting Corrosion
* **Appearance:** Small, deep holes.
* **Mechanism:** Similar to crevice corrosion but autocatalytic. Often initiated by **Chloride ions ($Cl^-$)** breaking the passive film.
* **Danger:** Occurs in materials that are otherwise passive (like Stainless Steel). It is insidious and hard to detect.

![[Pasted image 20260204173744.png]]


---

## Synergistic Phenomena
### Stress Corrosion Cracking (SCC)
* **Formula:** Tensile Stress + Specific Corrosive Environment + Susceptible Material.
* **Mechanism:** A crack initiates (frequently at a pit). The crack tip is active (anodic), while the walls are passive. The stress keeps opening the tip, exposing fresh metal to corrosion.
* **Result:** Sudden brittle failure in ductile materials.

### Hydrogen Embrittlement
* **Mechanism:** Atomic Hydrogen ($H$) diffuses into the metal lattice (interstitial).
* **Sources of H:** Corrosion reactions, welding, electroplating.
* **Effect:** Low ductility fracture. Can be confused with SCC, but strictly due to Hydrogen presence preventing plastic deformation (dislocation movement).

### Others
* **Corrosion Fatigue:** Fatigue limit is lowered (or eliminated) by a corrosive environment.
* **Selective Leaching:** One element is removed (e.g., Zinc removed from Brass).
* **Fretting Corrosion:** Corrosion assisted by small-scale vibration/sliding.
* **Erosion Corrosion:** Flowing fluid strips protective films.

![[Pasted image 20260204174205.png]]

---

## The Galvanic Series (Seawater)

| Rank                     | Metals                                      | Role                                  |
| :----------------------- | :------------------------------------------ | :------------------------------------ |
| **Noble (Cathodic)**     | Platinum, Gold, Graphite, Titanium          | **Protected** (Will eat other metals) |
| **Passive**              | Stainless Steel (Passive), Nickel (Passive) |                                       |
| **Active**               | Steel, Iron, Aluminum Alloys                |                                       |
| **Sacrificial (Anodic)** | Zinc, Magnesium                             | **Corrodes** (Used to protect others) |

> [!warning]+ Design Rule
> Never couple a metal from the top of this list with a small piece of metal from the bottom.

---

## Prevention and Protection

### Design Rules
1.  **Weld rather than rivet** (avoids crevices).
2.  **Drainage:** Design containers to drain completely (avoid standing liquid).
3.  **Stress:** Avoid residual tensile stresses in exposed components (prevents SCC).
4.  **Galvanic:** Insulate dissimilar metals or keep them far apart in the series.
5.  **Heterogeneity:** Avoid varying conditions (heat, stress, aeration) across the surface.

### Coatings & Active Protection
* **Sacrificial Anodes:** Connect the steel to Zinc or Magnesium. The Zn/Mg corrodes (anode), forcing the steel to be the cathode (immune).
* **Passivation:** Relying on stable oxide films (e.g., $Cr_2O_3$ on Stainless Steel). 
	* An oxide layer forms on the surface, leading to decreased conductivity and therefore slower corrosion.
	* *Warning:* If the film is damaged and cannot reform (no Oxygen), pitting occurs.
* **Coatings:** Paints, polymers, or metal plating (Cladding, Hot-dipping).

![[Pasted image 20260204174821.png]]