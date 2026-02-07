![[Fundamentals of Strength of Materials/attachments/Pasted image 20260207233848.png]]

> [!QUOTE] The Purpose
> We know the stress state ($\sigma_x, \sigma_y, \tau_{xy}$) on the horizontal/vertical faces. Mohr's Circle allows us to find the stress on **any inclined plane** ($\theta$) graphically, without solving complex rotation equations.
>
> Most importantly, it reveals the **Principal Stresses** (Max/Min normal stress) and the **Maximum Shear Stress**.

![[Fundamentals of Strength of Materials/attachments/Pasted image 20260207235125.png]]
![[Fundamentals of Strength of Materials/attachments/Pasted image 20260207234930.png]]

---

### The Sign Convention
* **Normal Stress ($\sigma$):**
    * **Tension (+):** Pulling away from the element (Right on the graph).
    * **Compression (-):** Pushing into the element (Left on the graph).
* **Shear Stress ($\tau$):**
    * *Standard Convention:*
        * Face X: If $\tau$ rotates the element **Counter-Clockwise** $\to$ Plot Down (-).
        * Face X: If $\tau$ rotates the element **Clockwise** $\to$ Plot Up (+).
    * *Note:* The vertical axis is usually $\tau$ (positive down) or $\tau$ (positive up).
---

### Construction Steps

**1. Identify the Points:**
* **Point X (Face X):** Plot $(\sigma_x, -\tau_{xy})$
* **Point Y (Face Y):** Plot $(\sigma_y, \tau_{xy})$
* *Note:* One point will be above the axis, one below.

**2. Find the Centre ($C$):**
The circle lies on the $\sigma$ axis (horizontal).
$$C = \frac{\sigma_x + \sigma_y}{2}$$
* This is the **Average Normal Stress** ($\sigma_{avg}$).

**3. Calculate the Radius ($R$):**
Distance from Centre $C$ to Point X.
$$R = \sqrt{ \left( \frac{\sigma_x - \sigma_y}{2} \right)^2 + \tau_{xy}^2 }$$
---

### Critical Values

Once drawn, the circle reveals the failure points immediately:

**1. Principal Stresses ($\sigma_1, \sigma_2$):**
The points where the circle crosses the horizontal $\sigma$-axis. Shear is **Zero** here.
* **Max Tension/Compression:**
$$\sigma_{1,2} = C \pm R$$

**2. Maximum Shear Stress ($\tau_{max}$):**
The highest/lowest point of the circle (top/bottom).
$$\tau_{max} = R$$

**3. Principal Orientation ($\theta_p$):**
The angle on the circle ($2\theta$) is **double** the physical angle ($\theta$).
* If you rotate $90^\circ$ on the circle (from Point X to $\sigma_1$), you rotate $45^\circ$ on the real element.
$$\tan(2\theta_p) = \frac{2\tau_{xy}}{\sigma_x - \sigma_y}$$

---

### Special Cases

* **Uniaxial Tension:** Circle touches the origin. $\sigma_2 = 0$.
* **Pure Shear:** Centre is at origin ($C=0$). $\sigma_1 = -\sigma_2$.
* **Hydrostatic Pressure:** $\sigma_x = \sigma_y$. Radius = 0. The circle is a **Dot**.

---
# Mohr's Circle (Inverse Construction)

> [!QUOTE] The Goal
> You start with the **Principal Stresses** ($\sigma_1, \sigma_2$) and want to find the normal ($\sigma$) and shear ($\tau$) stress on a plane inclined at a specific angle $\theta$.

---

### The Setup

**1. Plot Principal Stresses**
* Mark $\sigma_1$ (Max) and $\sigma_2$ (Min) on the horizontal $\sigma$-axis.
* *Note:* Shear is zero at these points.

**2. Draw the Circle**
* **Centre ($C$):** Midpoint between $\sigma_1$ and $\sigma_2$.
* **Radius ($R$):** Distance from $C$ to $\sigma_1$.
* Draw the full circle.

---

### The Rotation Rule ($2\theta$)

> [!DANGER] The Golden Rule of Mohr
> **Real World vs. Circle World**
>
> * **Real Element:** Angle is $\theta$.
> * **Mohr's Circle:** Angle is **$2\theta$**.
> * **Direction:** The direction is the **SAME**.
>     * If you rotate the cut **Counter-Clockwise (CCW)** by $\theta$ in reality, you rotate the radius **Counter-Clockwise (CCW)** by $2\theta$ on the circle.

**The Procedure**
1.  **Start at the Reference Point:** Usually Point 1 ($\sigma_1, 0$), which represents the Principal Plane (where max stress acts).
2.  **Rotate:** Measure an angle of **$2\theta$** from the horizontal axis in the correct direction.
3.  **Find Point P:** The end of this new radius is your state $(\sigma_{\theta}, \tau_{\theta})$.
4.  **Read Values:** The coordinates of P are the Normal and Shear stress on that inclined plane.

---

### The “Pole” Method (Origin of Planes)

![[Fundamentals of Strength of Materials/attachments/Pasted image 20260208000308.png]]

This is a graphical trick to find the stress on **any** plane without calculating angles first. It is often faster for complex problems.

**1. Find the Pole ($P$)**
* Start at a known point on the circle (e.g., the Principal Stress point $\sigma_1, 0$).
* Draw a line through that point **PARALLEL** to the physical face it represents (e.g., since $\sigma_1$ acts on a vertical plane, draw a vertical line through the point).
* Where this line crosses the circle again is the **Pole ($P$)**.

**2. Use the Pole**
* Draw a line from the Pole ($P$) parallel to **any physical cut** you want to analyse (angle $\theta$).
* The point where this line hits the circle gives you the exact $(\sigma, \tau)$ for that cut.