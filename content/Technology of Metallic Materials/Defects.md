# Surface Corrosion
Inside a material, metal atoms are surrounded by other atoms. This makes them low-energy since they are bound everywhere. However, on the surface of the material, atoms are not bound everywhere and are therefore in a thermodynamically unstable state, making them more reactive.

This allows for the surface of metals to be prone to corrosion (reaction with outside elements) on the surface.

$$
E_{\text{Free Energy Surface}}>E_{\text{Internal}}
$$

# Stacking Faults
![[Pasted image 20260127135301.png]]
> In FCC crystals, we can have stacking faults: a layer is missing and therefore resembles an HCP structure for a small segment. This makes the materials with more of these faults to be more resistant to plastic deformation.

We define “Stacking Fault Energy” as the energy per unit area required to create a stacking fault. When this is high (such as in aluminium), it is common to see slipping occur as the material gets deformed.

# Twinning

When stacking fault energy is low, such as in brass, stainless steel (also common in HCP metals such as titanium and magnesium), we tend to get **Mechanical Twinning**: a planar defect where small fractions of the crystal volume which rotate to form a mirror image (a twin) of the original lattice.

> [!note] Twinning
> Mechanical twinning is a plastic deformation mechanism in crystalline materials where a shear stress causes a portion of the lattice to reorient into a mirror image of the surrounding matrix. 
> It occurs as a rapid, stress-mediated process often at low temperatures or high strain rates, particularly in HCP metals and low-stacking fault energy FCC alloys, typically forming thin, lens-shaped regions. 

> [!warning]
> Twinning involves only small sections of the lattice. These small sections will reverse the direction with respect to the rest of the structure.

**Twinning is promoted by:**
- Low temperatures
- High strain rates
	- Explosions, impacts, or ballistic hits (slip is too slow to accommodate rapid deformation)
- Large grain size
	- Small grains resist twinning.
- Low SFE

> [!faq]- A use for this
> The presence of “twins” in a material which has failed can hint at the reason for its failure. For example, in a plane crash in the 90s, an investigation showed that parts of the steel of the plane's frame had signs of twinning, which told them that the plane was likely hit by an explosive rocket. (Explosion = high $\frac{d\varepsilon}{dt}$)

![[Pasted image 20260128231102.png]]
![[Pasted image 20260128231120.png]]
![[Pasted image 20260128231137.png]]
> [!info] Deformation Mechanism Map
> The following diagram shows how different stress rates and temperatures affect the way the material plastically deforms.
> ![[Pasted image 20260128231545.png]]

# Grain Boundaries

1. We can't always see grain boundaries. We need to use some sort of [etching](QA#Etching) to actually see them.
2. Grain boundaries are high-energy and usually have free [interstitial sites](Crystal%20Mictostrictures#Types%20of%20Interstitial%20Sites).
3. Because of these interstitial sites, impurities tend to clump up on grain boundaries

**We have two different types of grain boundaries depending on the difference in orientation between the two grains $\theta$:**
- Low Angle Grain Boundaries (*LAGB*)
	- $\theta<15°$
	- Since the misalignment is not significant, the energy of the GB is relatively low and closer to the energy within the grain
	- The structure is adjusted by inserting an occasional “extra half-plane” of atoms to “bridge the gap”
	- Mathematically, this acts just like a vertical stack of edge dislocations
		- The energy is the sum of energies of those dislocations
		- Higher angle $\implies$ More dislocations needed $\implies$ Higher energy (linear-ish behaviour)
- High Angle Grain Boundaries (*HAGB*)
	- $\theta>15°$
	- Beyond around 15°, the misalignment is huge
	- In these GBs, grain boundaries have a layer of disordered (quasi-amorphous) structure as the material transitions from one orientation to another
	- At this point, energy is maximized and increasing energy beyond $\sim15°$ will not increase it much further.
		- Here, energy is constant and at its maximum

> [!example]- An example for Copper
> ![[Pasted image 20260129024452.png]]

**Consequences of grain boundaries:**
- They are sources and sinks for dislocations
- They contribute to mechanical strengthening and change the sliding system
- They act as synks for impurities dissolved in the alloy
- Tey contribute to the formation of second phases
	- Primary nucleation sites for the growth of second phases
- They are material portions with no crystallinity (amorphous)

# Grains

ASTM defines a value that describes grain density.
$$
N=2^{n-1}
\implies n=\log_2N+1
$$
Where:
- $N$ is the number of grains per square inch
- $n$ is the **grain size number**

> [!error] NEXT IS PAGE 10!!!!!!!!!

