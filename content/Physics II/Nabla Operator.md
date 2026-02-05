$$
\begin{align}
&f(x_{1},x_{2}\dots x_{n}) \\
&\nabla f=\left( \begin{matrix}
\frac{\delta f}{\delta x_{1}} \\
\frac{\delta f}{\delta x_{2}} \\
\dots \\
\frac{\delta f}{\delta x_{n}}
\end{matrix} \right)
\end{align}
$$
**Cylindrical $(r,\theta,z)$:**

$$
\nabla f=\frac{\delta f}{\delta r}\vec{u}_{r}+\frac{1}{r}\frac{\delta f}{\delta\theta}\vec{u}_{\theta}+\frac{\delta f}{\delta z}\vec{k}
$$

**Spherical $(r,\theta,\phi)$:**

$$
\nabla f=\frac{\delta f}{\delta r}\vec{u}_{r}+\frac{1}{r}\frac{\delta f}{\delta\theta}\vec{u}_{\theta}+\frac{1}{r \sin\theta}\frac{\delta f}{\delta \phi}\vec{u}_{\phi}
$$

# Curl
$$
\nabla \times \mathbf{\vec{A}} = \begin{Bmatrix} \frac{\partial}{\partial x} \\ \frac{\partial}{\partial y} \\ \frac{\partial}{\partial z} \end{Bmatrix} \times \begin{Bmatrix} A_x \\ A_y \\ A_z \end{Bmatrix} = \begin{Bmatrix} \frac{\partial A_z}{\partial y} - \frac{\partial A_y}{\partial z} \\ \frac{\partial A_x}{\partial z} - \frac{\partial A_z}{\partial x} \\ \frac{\partial A_y}{\partial x} - \frac{\partial A_x}{\partial y} \end{Bmatrix}
$$

# Divergence

$$
div(\vec{A}) = \nabla \cdot \vec{A} = \frac{\delta A_{x_1}}{\delta x_1} + \frac{\delta A_{x_2}}{\delta x_2} + \dots + \frac{\delta A_{x_n}}{\delta x_n}
$$
## Gauss' Divergence Theorem
$$
\oint_{S}\vec{A}\cdot \vec{u}_{n}dS=\int_{V}(\nabla \cdot \vec{A})dV
$$
## Gauss' Law (Differential Form)
$$
\nabla \cdot \vec{E}=\frac{\rho}{\varepsilon_{0}}
$$
