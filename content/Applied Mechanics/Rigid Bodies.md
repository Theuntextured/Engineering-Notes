> [!TIP]+ Definition
> A rigid body is one where the distance between any two points remains unchanged in time.
> 

> [!CHECK]+ 2D Rigid Bodies
> In 2D, it can be observed to move in three ways:
> - Translation motion
> - Rotation about a fixed axis
> - General plane motion (combination of translation and rotation)
>   
>   To describe its position, we use three measurements:
> - $x_{0},y_{0}$: position of a generic point $O$
> - $\theta$: angle between a fixed axis $r$ fixed to the object and a given reference axis (fixed to the world)
>
> ![[rigid-body-diagram.excalidraw]]
> 
> The three variables are enough to describe the whole body:
> - If the body is translating, then all points have the same $v$
> - If the body is rotating, all points have the same angular velocity $\omega$ and angular acceleration $\dot{\omega}$.

**In translational motion**, $\theta$ remains constant.

---
### Rotation around a fixed axis

At any point $P$ on the rigid body (except for $P=O$), we can define

$$
\vec{r}=\overrightarrow{OP}
$$

and therefore:

$$
\begin{align}
\vec{v}&=r\omega \vec{\mu} \\
\vec{a}_{n}&=-r\omega^2 \vec{\lambda} \\
\vec{a}_{t}&=r\dot{\omega}\vec{\mu} \\
\implies\vec{a}&=r\dot{\omega}\vec{\mu}-r\omega^{2}\vec{\lambda}
\end{align}
$$

Where $\vec{\lambda},\vec{\mu}$ are normal and tangential versors (unit vectors) with respect to circular motion.

$$
\implies a=\sqrt{ a^2_{n}+a^2_{t} }=r\sqrt{ \omega^4+\dot{\omega}^2 }
$$

Let

$$
\tan \gamma=\frac{a_{t}}{a_{n}}=\frac{\dot{\omega}}{\omega^{2}}
$$
*$\gamma$ is the angle between tangential acceleration and normal acceleration.*

> [!NOTE]-
> 
> $$
> \begin{align}
> \gamma=0\implies &\dot{\omega}=0 \\
> \gamma=\frac{\pi}{2}\implies&\omega=0
> \end{align}
> $$
> 

---
### General Plane Motion
*The combination of translation and rotation.*

Generally,

$$
\Delta \vec{r}_{A}=\Delta \vec{r}_{B}+\Delta \vec{r}_{A|B}
$$

Where $\Delta \vec{r}_{A|B}$ is the change in position of $B$ relative to point $A$. This is the *fundamental kinematic formula*. We can then use:

$$
\vec{V}_{A|B}=\vec{\omega}\times \vec{l}=\omega l\vec{\mu}
$$

#### Instantaneous Centre of Rotation

During planar motion, if $\omega \neq 0$, there is always an "instantaneous centre of rotation": a point (inside or outside the body) that describes the planar motion simply as a rotation. This point can be found using instantaneous velocities (or simply their direction) of any two different points of the body.

![[Pasted image 20260307182257.png]]

After finding the ICR point, it is easy to find angular velocity and therefore velocity of any point in the body.

$$
\omega=\frac{V_{A}}{r_{A}}=\frac{V_{B}}{r_{B}}
$$

> [!NOTE]
> ICR is generally NOT a fixed point and changes over time. It is useful to find for instantaneous states.

---
# Coupled Bodies
> [!ABSTRACT]
> When two rigid bodies are coupled, they are connected via *conjugated surfaces* of the pair: surfaces of both objects which are in contact. Their shape determines the constraints between the two bodies.
> If the shape of the conjugated surfaces couples the two objects we get a *kinematic pair*, otherwise, if the coupling is caused by other forces, we get *force coupling*.

> [!NOTE]
> We often talk about absolute motion of a component, but at times it is useful to analyse motion relative to its "parent" component, or relative motion using a moving reference frame.

### Prismatic Pair
A prismatic pair (or sliding pair) is a kinematic pair that allows only 1D linear translation between two bodies while restricting rotation, offering **one degree of freedom**. Prismatic pairs have (no shit) prismatic conjugated surfaces, i.e. polygonal.

Common examples: 
- Piston moving inside a cylinder
- Desk drawer
- Hydraulic/pneumatic cylinders
- Machine tool slideways

> [!TIP] Lubrication is used to reduce friction in this case!

### Revolute Pair or Hinge
In hinges, cylindrical conjugated surfaces are used to allow for rotation. Translation is therefore prevented. To reduce friction, we can use lubrication, plane bearings (left) or roller/ball bearings (right).

![[Pasted image 20260307184214.png]]

### Screw Pair
In a screw pair, rotation and one axis of translation are allowed, e.g. $\theta,x$ while the other axis of translation is locked (e.g. $y$). However, $\theta$ and $x$ are not independent due to threads in the screw. Therefore, there is only 1 degree of freedom.

![[Pasted image 20260307184440.png]]

Given $p$ as the pitch and $t$ as time, we get:

$$
\begin{align}
V=\frac{p}{t} && \omega=\frac{2\pi}{t} \\
\implies V=\frac{p\omega}{2\pi}
\end{align}
$$
### Cam-Follower
A cam disk is a non-circular disk which displaces a point vertically. An example is what is used in the cam shaft of a car (especially older ones, shown below). They push the follower up and down.

> [!EXAMPLE]- Camshaft
> ![[Pasted image 20260307185004.png]]

![[Pasted image 20260307185011.png]]
> The spring is used to guarantee the contact of point A with the cam disk.

If contact is guarantied, then the system has one degree of freedom, since the rotation of the cam disk directly affects the vertical position of the follower. Horizontal position is therefore locked.

### Wheel-Ground Coupling

![[Pasted image 20260307185359.png]]

The wheel is attached to the vehicle via a shaft, and is in contact with the ground.

> [!EXAMPLE]+ Case A: Static Friction
> In case A (above image), the contact point between the wheel and the ground has no sliding, meaning that the centre of rotation of the wheel is its centre $B$, with angular velocity:
> 
> $$
> \omega_{a}=\frac{V}{r}
> $$

> [!EXAMPLE]+ Case B: Wheel Sliding Forward
> In case B, the wheel slides while it also rotates (such as when the car is braking hard). In this case, point $B$ is **NOT** the instantaneous point of rotation: that is point $C$, which is outside the wheel (since $V\parallel V_{A}$). In this case,
> 
> $$
> \omega_{b}=\frac{V}{\overrightarrow{BC}}<\omega_{A}
> $$

> [!EXAMPLE]+ Case C: Wheel Sliding Backward
> In case C, the wheel slides backwards relative to the ground as it rotates (such as when the car accelerates hard). The instantaneous rotation centre in this case is inside the wheel, and we have:
> 
> $$
> \omega_{c}=\frac{V}{\overrightarrow{BC}}>\omega_{A}
> $$

---
