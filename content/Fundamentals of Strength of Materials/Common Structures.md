# Truss
![[Fundamentals of Strength of Materials/attachments/Pasted image 20260207211335.png]]

> [!NOTE] External forces are only applied to the internal hinges (nodes).

In each rod, the only internal action is the normal load $N$
- If $N>0$, then the beam is loaded by traction
- If $N<0$, then the beam is loaded by compression

> [!check]+ Simplified [[Fundamentals of Strength of Materials/1. Basics#Determinacy of Structures\|degree of static determinacy]]
> $$
> h=\text{Number of Rods}+\text{Number of External Reactions}-2\cdot \text{Number of Internal Hunges}
> $$

### Solution Strategy
1. **Compute $h$** (Check if isostatic).
2. **External Reactions:** Treat the whole truss as a *single rigid body* first. Ignore the insides. Solve for the ground supports ($H_A, V_A, etc.$).
3. **Internal Forces ($N$):** 
    - **Method of Nodes:** Solves *every* rod (good for full analysis).
    - **Method of Sections (Ritter):** Solves *specific* rods (good for finding just one or two forces).

---

### Method 1: Equilibrium at Nodes
> [!TIP] The Logic
> Isolate a specific node (hinge) and treat it as a particle. Since the node is in equilibrium, the sum of forces acting on it must be zero.

**Procedure:**
1.  **Isolate a Node:** Start with a node where you have **at least 1 known force** and **no more than 2 unknown rods** (since you only have 2 equations: $\sum F_x, \sum F_y$).
2.  **Draw Vectors:**
    * Draw known external forces.
    * Draw unknown rod forces ($N$) pointing **AWAY** from the node.
    * *Note:* We always assume **Traction (+)** initially.
3.  **Solve:**
    * $\sum F_x = 0$
    * $\sum F_y = 0$
4.  **Interpret signs:**
    * Result $> 0$: Assumption correct (Traction).
    * Result $< 0$: Rod is in Compression.
5.  **Repeat:** Move to the next connected node and use the values you just found.

> [!EXAMPLE]- Spotting "Zero Force" Members
> Sometimes you can spot rods with $N=0$ just by looking.
> * *Example:* Look at Node B. A vertical force $F$ balances the vertical rod ($N_3$). However, **nothing** opposes the horizontal rod ($N_2$). Therefore, to maintain equilibrium, $N_2$ **must be zero**.
> ![[Fundamentals of Strength of Materials/attachments/Pasted image 20260207213039.png]]

---
### Method 2: Method of Sections (Ritter)
> [!INFO] The Logic
> Instead of solving node-by-node, you "cut" the truss into two separate rigid bodies. The internal forces of the cut rods become external forces on the new sections.

**The Rules of the Cut:**
1.  **Cut Max 3 Rods:** You only have 3 equilibrium equations ($\sum F_x, \sum F_y, \sum M$), so you cannot solve for more than 3 unknowns.
2.  **No Common Node:** The three cut rods cannot all meet at the same node (otherwise the moment equation becomes useless).

**The “Ritter” Strategy:**
To find the force in a specific rod (e.g., Rod A) without doing extra maths:
1.  **Identify the other two rods** you cut (Rods B and C).
2.  **Find their intersection point** (Point P).
3.  **Sum Moments about Point P** ($\sum M_P = 0$).
    * Since Rods B and C pass through P, their moment is **zero**.
    * You are left with an equation containing *only* Rod A.
