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

# Cast Iron

Cast iron is a high-carbon form of steel and graphite formed by casting of carbon-rich iron.
Graphite is the most stable form of $C$ in ferrous alloys, but is only present in cast iron with high $C$ and $Si$ content. The shape of this graphite can be controlled to produce different formations from flakes to lamellae to noodles.

![[Technology of Metallic Materials/attachments/Pasted image 20260128172306.png]]
> Above is the result of chemical [etching](QA#Etching) on a sample of cast iron.

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

<svg viewBox="0 0 800 500" xmlns="http://www.w3.org/2000/svg" style="background-color: #1e1e1e; border-radius: 8px; font-family: sans-serif;">
  <defs>
    <pattern id="grid" width="50" height="50" patternUnits="userSpaceOnUse">
      <path d="M 50 0 L 0 0 0 50" fill="none" stroke="#333" stroke-width="1"/>
    </pattern>
  </defs>
  <rect width="100%" height="100%" fill="url(#grid)" />

  <line x1="50" y1="450" x2="750" y2="450" stroke="#fff" stroke-width="2" /> <line x1="50" y1="450" x2="50" y2="50" stroke="#fff" stroke-width="2" /> <text x="700" y="480" fill="#fff" font-size="14">TIME (t)</text>
  <text x="20" y="40" fill="#fff" font-size="14">TEMP (T)</text>

  <line x1="50" y1="250" x2="750" y2="250" stroke="#666" stroke-width="2" stroke-dasharray="5,5" />
  <text x="60" y="240" fill="#888" font-size="12">Equilibrium A1 (Theoretical)</text>

  <path d="M 50 400 Q 200 400, 300 100" fill="none" stroke="#ff4d4d" stroke-width="4" />
  <text x="150" y="300" fill="#ff4d4d" font-size="16" font-weight="bold" transform="rotate(-45 150,300)">HEATING</text>

  <line x1="50" y1="200" x2="300" y2="200" stroke="#ff4d4d" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="310" y="205" fill="#ff4d4d" font-size="14">Ac1 (Start Austenite)</text>
  
  <line x1="50" y1="150" x2="300" y2="150" stroke="#ff4d4d" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="310" y="155" fill="#ff4d4d" font-size="14">Ac3 (Full Austenite)</text>


  <path d="M 300 100 Q 450 100, 550 400" fill="none" stroke="#4d79ff" stroke-width="4" />
  <text x="450" y="220" fill="#4d79ff" font-size="16" font-weight="bold" transform="rotate(50 450,220)">SLOW COOLING</text>

  <line x1="300" y1="280" x2="750" y2="280" stroke="#4d79ff" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="560" y="285" fill="#4d79ff" font-size="14">Ar3 (Start Ferrite)</text>

  <line x1="300" y1="330" x2="750" y2="330" stroke="#4d79ff" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="560" y="335" fill="#4d79ff" font-size="14">Ar1 (End Ferrite)</text>


  <path d="M 300 100 Q 350 100, 380 450" fill="none" stroke="#d54dff" stroke-width="3" stroke-dasharray="10,5" />
  <text x="320" y="380" fill="#d54dff" font-size="14" font-weight="bold">QUENCH</text>

  <line x1="50" y1="400" x2="750" y2="400" stroke="#d54dff" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="400" y="415" fill="#d54dff" font-size="14">Ms (Martensite Start)</text>

</svg>

<svg viewBox="0 0 800 500" xmlns="http://www.w3.org/2000/svg" style="background-color: #1e1e1e; border-radius: 8px; font-family: sans-serif;">
  <defs>
    <pattern id="grid_hc" width="50" height="50" patternUnits="userSpaceOnUse">
      <path d="M 50 0 L 0 0 0 50" fill="none" stroke="#333" stroke-width="1"/>
    </pattern>
  </defs>
  <rect width="100%" height="100%" fill="url(#grid_hc)" />

  <line x1="50" y1="450" x2="750" y2="450" stroke="#fff" stroke-width="2" /> <line x1="50" y1="450" x2="50" y2="50" stroke="#fff" stroke-width="2" /> <text x="700" y="480" fill="#fff" font-size="14">TIME (t)</text>
  <text x="20" y="40" fill="#fff" font-size="14">TEMP (T)</text>

  <line x1="50" y1="300" x2="750" y2="300" stroke="#666" stroke-width="2" stroke-dasharray="5,5" />
  <text x="60" y="290" fill="#888" font-size="12">Equilibrium A1 (727°C)</text>

  <line x1="50" y1="180" x2="750" y2="180" stroke="#666" stroke-width="2" stroke-dasharray="5,5" />
  <text x="60" y="170" fill="#888" font-size="12">Equilibrium Acm (Cementite Limit)</text>

  <path d="M 50 400 Q 200 400, 300 100" fill="none" stroke="#ff4d4d" stroke-width="4" />
  <text x="130" y="280" fill="#ff4d4d" font-size="16" font-weight="bold" transform="rotate(-55 130,280)">HEATING</text>

  <line x1="50" y1="260" x2="250" y2="260" stroke="#ff4d4d" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="260" y="265" fill="#ff4d4d" font-size="14">Ac1 (Start Austenite)</text>
  
  <line x1="50" y1="140" x2="290" y2="140" stroke="#ff4d4d" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="300" y="145" fill="#ff4d4d" font-size="14">Accm (End Cementite)</text>


  <path d="M 300 100 Q 450 100, 550 400" fill="none" stroke="#4d79ff" stroke-width="4" />
  <text x="470" y="200" fill="#4d79ff" font-size="16" font-weight="bold" transform="rotate(50 470,200)">SLOW COOLING</text>

  <line x1="300" y1="220" x2="750" y2="220" stroke="#4d79ff" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="560" y="225" fill="#4d79ff" font-size="14">Arcm (Start Cementite)</text>

  <line x1="300" y1="340" x2="750" y2="340" stroke="#4d79ff" stroke-width="1" stroke-dasharray="4,2"/>
  <text x="560" y="345" fill="#4d79ff" font-size="14">Ar1 (End Transformation)</text>

  <text x="350" y="50" fill="#aaa" font-size="14" font-style="italic">Hypereutectoid Steel (>0.8% C)</text>

</svg>

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
> The effect of austenitizers and fertilizers on eutectoid temperature and composition ($wt\%\ C$)

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
> BCC structure of almost pure iron
> Very low solubility for carbon ($C\leq_{0}.0025\%$)
> Iron atoms can be replaced in the crystal lattice by other alloying elements such as $Cr,Mo,Si$.
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

