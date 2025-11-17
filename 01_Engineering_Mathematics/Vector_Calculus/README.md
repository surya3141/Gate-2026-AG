# 📐 Vector Calculus

> Complete guide to Vector Calculus for GATE Agricultural Engineering

---

## 📑 Table of Contents

1. [Vector Algebra](#1-vector-algebra)
2. [Scalar and Vector Point Functions](#2-scalar-and-vector-point-functions)
3. [Vector Differentiation](#3-vector-differentiation)
4. [Gradient, Divergence, and Curl](#4-gradient-divergence-and-curl)
5. [Line Integrals](#5-line-integrals)
6. [Surface Integrals](#6-surface-integrals)
7. [Volume Integrals](#7-volume-integrals)
8. [Green's Theorem](#8-greens-theorem)
9. [Stokes' Theorem](#9-stokes-theorem)
10. [Gauss' Divergence Theorem](#10-gauss-divergence-theorem)

---

## 1. Vector Algebra

### 1.1 Vector Representation

A **vector** is a quantity with both magnitude and direction.

**Notation:**
- Bold letters: $\mathbf{A}$, $\mathbf{B}$, $\mathbf{r}$
- Magnitude: $|\mathbf{A}|$ or $A$
- Unit vector: $\hat{\mathbf{A}} = \frac{\mathbf{A}}{|\mathbf{A}|}$

**Position vector:** $\mathbf{r} = x\mathbf{i} + y\mathbf{j} + z\mathbf{k}$

---

### 1.2 Vector Operations

#### Addition and Subtraction
$$
\mathbf{A} + \mathbf{B} = (A_x + B_x)\mathbf{i} + (A_y + B_y)\mathbf{j} + (A_z + B_z)\mathbf{k}
$$

$$
\mathbf{A} - \mathbf{B} = (A_x - B_x)\mathbf{i} + (A_y - B_y)\mathbf{j} + (A_z - B_z)\mathbf{k}
$$

#### Scalar Multiplication
$$
k\mathbf{A} = (kA_x)\mathbf{i} + (kA_y)\mathbf{j} + (kA_z)\mathbf{k}
$$

#### Dot Product (Scalar Product)
$$
\mathbf{A} \cdot \mathbf{B} = A_x B_x + A_y B_y + A_z B_z = |\mathbf{A}||\mathbf{B}|\cos\theta
$$

**Properties:**
- Commutative: $\mathbf{A} \cdot \mathbf{B} = \mathbf{B} \cdot \mathbf{A}$
- Distributive: $\mathbf{A} \cdot (\mathbf{B} + \mathbf{C}) = \mathbf{A} \cdot \mathbf{B} + \mathbf{A} \cdot \mathbf{C}$
- Scalar multiplication: $(k\mathbf{A}) \cdot \mathbf{B} = k(\mathbf{A} \cdot \mathbf{B})$

#### Cross Product (Vector Product)
$$
\mathbf{A} \times \mathbf{B} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
A_x & A_y & A_z \\
B_x & B_y & B_z
\end{vmatrix} = (A_y B_z - A_z B_y)\mathbf{i} + (A_z B_x - A_x B_z)\mathbf{j} + (A_x B_y - A_y B_x)\mathbf{k}
$$

**Properties:**
- Anti-commutative: $\mathbf{A} \times \mathbf{B} = -(\mathbf{B} \times \mathbf{A})$
- Distributive: $\mathbf{A} \times (\mathbf{B} + \mathbf{C}) = \mathbf{A} \times \mathbf{B} + \mathbf{A} \times \mathbf{C}$
- Magnitude: $|\mathbf{A} \times \mathbf{B}| = |\mathbf{A}||\mathbf{B}|\sin\theta$

---

### 1.3 Vector Identities

**Triple Products:**

**Scalar Triple Product:**
$$
\mathbf{A} \cdot (\mathbf{B} \times \mathbf{C}) = \begin{vmatrix}
A_x & A_y & A_z \\
B_x & B_y & B_z \\
C_x & C_y & C_z
\end{vmatrix}
$$

**Properties:**
- Cyclic permutation: $\mathbf{A} \cdot (\mathbf{B} \times \mathbf{C}) = \mathbf{B} \cdot (\mathbf{C} \times \mathbf{A}) = \mathbf{C} \cdot (\mathbf{A} \times \mathbf{B})$
- Anti-cyclic: $\mathbf{A} \cdot (\mathbf{B} \times \mathbf{C}) = -(\mathbf{A} \cdot (\mathbf{C} \times \mathbf{B}))$

**Vector Triple Product:**
$$
\mathbf{A} \times (\mathbf{B} \times \mathbf{C}) = (\mathbf{A} \cdot \mathbf{C})\mathbf{B} - (\mathbf{A} \cdot \mathbf{B})\mathbf{C}
$$

---

## 2. Scalar and Vector Point Functions

### 2.1 Scalar Point Function

A **scalar field** assigns a scalar value to each point in space.

**Examples:**
- Temperature: $T(x, y, z)$
- Pressure: $P(x, y, z)$
- Potential: $\phi(x, y, z)$

### 2.2 Vector Point Function

A **vector field** assigns a vector to each point in space.

**Examples:**
- Velocity field: $\mathbf{v}(x, y, z) = v_x\mathbf{i} + v_y\mathbf{j} + v_z\mathbf{k}$
- Force field: $\mathbf{F}(x, y, z)$
- Electric field: $\mathbf{E}(x, y, z)$

**Types of Vector Fields:**

**Conservative Field:** If $\mathbf{F} = -\nabla \phi$ (derivable from scalar potential)

**Solenoidal Field:** If $\nabla \cdot \mathbf{F} = 0$

**Irrotational Field:** If $\nabla \times \mathbf{F} = \mathbf{0}$

---

## 3. Vector Differentiation

### 3.1 Differentiation of Vector Functions

For $\mathbf{r}(t) = x(t)\mathbf{i} + y(t)\mathbf{j} + z(t)\mathbf{k}$:

**Velocity:**
$$
\mathbf{v} = \frac{d\mathbf{r}}{dt} = \frac{dx}{dt}\mathbf{i} + \frac{dy}{dt}\mathbf{j} + \frac{dz}{dt}\mathbf{k}
$$

**Acceleration:**
$$
\mathbf{a} = \frac{d\mathbf{v}}{dt} = \frac{d^2\mathbf{r}}{dt^2}
$$

**Unit Tangent Vector:**
$$
\mathbf{T} = \frac{\mathbf{v}}{|\mathbf{v}|} = \frac{d\mathbf{r}/dt}{|d\mathbf{r}/dt|}
$$

---

### 3.2 Partial Derivatives

For a scalar function $f(x, y, z)$:

**Partial derivatives:**
$$
\frac{\partial f}{\partial x}, \quad \frac{\partial f}{\partial y}, \quad \frac{\partial f}{\partial z}
$$

**Higher order derivatives:**
$$
\frac{\partial^2 f}{\partial x^2}, \quad \frac{\partial^2 f}{\partial x \partial y}, \quad \text{etc.}
$$

---

## 4. Gradient, Divergence, and Curl

### 4.1 Gradient (∇f)

The **gradient** of a scalar field $f(x, y, z)$ is a vector field:

$$
\nabla f = \left( \frac{\partial f}{\partial x} \right)\mathbf{i} + \left( \frac{\partial f}{\partial y} \right)\mathbf{j} + \left( \frac{\partial f}{\partial z} \right)\mathbf{k}
$$

**Geometrical meaning:** Points in direction of maximum rate of increase of $f$.

**Directional derivative:**
$$
\frac{d f}{ds} = \nabla f \cdot \mathbf{u}
$$

where $\mathbf{u}$ is unit vector in direction of differentiation.

**Example:**
$$
f(x, y, z) = x^2 + y^2 + z^2
$$

$$
\nabla f = 2x\mathbf{i} + 2y\mathbf{j} + 2z\mathbf{k}
$$

---

### 4.2 Divergence (∇·F)

The **divergence** of a vector field $\mathbf{F} = F_x\mathbf{i} + F_y\mathbf{j} + F_z\mathbf{k}$ is a scalar field:

$$
\nabla \cdot \mathbf{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y} + \frac{\partial F_z}{\partial z}
$$

**Physical meaning:**
- Positive divergence: Source (field spreads out)
- Negative divergence: Sink (field converges)
- Zero divergence: Incompressible flow

**Example:**
$$
\mathbf{F} = xy\mathbf{i} + yz\mathbf{j} + zx\mathbf{k}
$$

$$
\nabla \cdot \mathbf{F} = \frac{\partial}{\partial x}(xy) + \frac{\partial}{\partial y}(yz) + \frac{\partial}{\partial z}(zx) = y + z + x
$$

---

### 4.3 Curl (∇×F)

The **curl** of a vector field $\mathbf{F}$ is a vector field:

$$
\nabla \times \mathbf{F} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
F_x & F_y & F_z
\end{vmatrix}
$$

$$
= \left( \frac{\partial F_z}{\partial y} - \frac{\partial F_y}{\partial z} \right)\mathbf{i} + \left( \frac{\partial F_x}{\partial z} - \frac{\partial F_z}{\partial x} \right)\mathbf{j} + \left( \frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right)\mathbf{k}
$$

**Physical meaning:**
- Measures rotation of the field
- Zero curl: Irrotational field
- Non-zero curl: Rotational field

**Example:**
$$
\mathbf{F} = y\mathbf{i} + x\mathbf{j}
$$

$$
\nabla \times \mathbf{F} = \left( \frac{\partial}{\partial y}(0) - \frac{\partial}{\partial z}(x) \right)\mathbf{i} + \left( \frac{\partial}{\partial z}(y) - \frac{\partial}{\partial x}(0) \right)\mathbf{j} + \left( \frac{\partial}{\partial x}(x) - \frac{\partial}{\partial y}(y) \right)\mathbf{k}
$$

$$
= (0 - 0)\mathbf{i} + (0 - 0)\mathbf{j} + (1 - 1)\mathbf{k} = \mathbf{0}
$$

---

### 4.4 Vector Operator Identities

**Important Identities:**

1. $\nabla \cdot (\nabla \times \mathbf{F}) = 0$ (curl is solenoidal)

2. $\nabla \times (\nabla f) = \mathbf{0}$ (gradient is irrotational)

3. $\nabla \cdot (\nabla f) = \nabla^2 f$ (Laplacian)

4. $\nabla \cdot (\mathbf{F} \times \mathbf{G}) = \mathbf{G} \cdot (\nabla \times \mathbf{F}) - \mathbf{F} \cdot (\nabla \times \mathbf{G})$

5. $\nabla \times (\mathbf{F} \times \mathbf{G}) = (\mathbf{G} \cdot \nabla)\mathbf{F} - (\mathbf{F} \cdot \nabla)\mathbf{G} + \mathbf{F}(\nabla \cdot \mathbf{G}) - \mathbf{G}(\nabla \cdot \mathbf{F})$

6. $\nabla \times (\nabla \times \mathbf{F}) = \nabla(\nabla \cdot \mathbf{F}) - \nabla^2 \mathbf{F}$

---

## 5. Line Integrals

### 5.1 Definition

A **line integral** along a curve C from point A to B:

**Scalar Line Integral:**
$$
\int_C f(x, y, z) \, ds
$$

**Vector Line Integral:**
$$
\int_C \mathbf{F} \cdot d\mathbf{r} = \int_C \mathbf{F} \cdot \mathbf{T} \, ds
$$

where $\mathbf{T} = \frac{d\mathbf{r}}{ds}$ is the unit tangent vector.

---

### 5.2 Parametric Form

For a curve parametrized by $x = x(t), y = y(t), z = z(t)$, $t: a \to b$:

**Scalar line integral:**
$$
\int_C f(x, y, z) \, ds = \int_a^b f(x(t), y(t), z(t)) \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2 + \left(\frac{dz}{dt}\right)^2} \, dt
$$

**Vector line integral:**
$$
\int_C \mathbf{F} \cdot d\mathbf{r} = \int_a^b \mathbf{F}(x(t), y(t), z(t)) \cdot \frac{d\mathbf{r}}{dt} \, dt
$$

---

### 5.3 Work Done

The line integral $\int_C \mathbf{F} \cdot d\mathbf{r}$ represents the work done by force $\mathbf{F}$ along path C.

**Conservative Field:** If $\mathbf{F} = -\nabla \phi$, then:
$$
\int_C \mathbf{F} \cdot d\mathbf{r} = \phi(A) - \phi(B)
$$

**Path Independence:** For conservative fields, the integral depends only on endpoints, not the path.

---

## 6. Surface Integrals

### 6.1 Definition

A **surface integral** over surface S:

**Scalar Surface Integral:**
$$
\iint_S f(x, y, z) \, dS
$$

**Vector Surface Integral:**
$$
\iint_S \mathbf{F} \cdot d\mathbf{S} = \iint_S \mathbf{F} \cdot \mathbf{n} \, dS
$$

where $\mathbf{n}$ is the unit normal to the surface.

---

### 6.2 Parametric Form

For a surface parametrized by $x = x(u, v), y = y(u, v), z = z(u, v)$:

**Scalar surface integral:**
$$
\iint_S f(x, y, z) \, dS = \iint_D f(x(u, v), y(u, v), z(u, v)) \sqrt{EG - F^2} \, du \, dv
$$

where $E, F, G$ are coefficients of the first fundamental form.

**Vector surface integral:**
$$
\iint_S \mathbf{F} \cdot d\mathbf{S} = \iint_D \mathbf{F} \cdot \left( \frac{\partial \mathbf{r}}{\partial u} \times \frac{\partial \mathbf{r}}{\partial v} \right) \, du \, dv
$$

---

### 6.3 Flux

The surface integral $\iint_S \mathbf{F} \cdot d\mathbf{S}$ represents the flux of vector field $\mathbf{F}$ through surface S.

**Direction:** The normal vector $\mathbf{n}$ determines the orientation.

---

## 7. Volume Integrals

### 7.1 Definition

A **volume integral** over region V:

**Scalar Volume Integral:**
$$
\iiint_V f(x, y, z) \, dV
$$

**Vector Volume Integral:**
$$
\iiint_V \mathbf{F} \, dV
$$

---

### 7.2 Applications

**Mass:** If $\rho(x, y, z)$ is density:
$$
M = \iiint_V \rho(x, y, z) \, dV
$$

**Center of Mass:**
$$
\bar{x} = \frac{1}{M} \iiint_V x \rho(x, y, z) \, dV
$$

---

## 8. Green's Theorem

### 8.1 Green's Theorem in Plane

For a region D bounded by simple closed curve C:

$$
\oint_C P \, dx + Q \, dy = \iint_D \left( \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} \right) \, dA
$$

**Vector form:**
$$
\oint_C \mathbf{F} \cdot d\mathbf{r} = \iint_D (\nabla \times \mathbf{F}) \cdot \mathbf{k} \, dA
$$

---

### 8.2 Physical Interpretation

Green's theorem relates a line integral around a closed curve to a double integral over the region it encloses.

**Applications:**
- Area calculation
- Work done by conservative fields
- Fluid flow calculations

---

### 8.3 Example

Evaluate $\oint_C (x^2 - y^2) \, dx + (x^2 + y^2) \, dy$ where C is the circle $x^2 + y^2 = 1$.

**Using Green's theorem:**
$$
P = x^2 - y^2, \quad Q = x^2 + y^2
$$

$$
\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} = \frac{\partial}{\partial x}(x^2 + y^2) - \frac{\partial}{\partial y}(x^2 - y^2) = 2x - (-2y) = 2x + 2y
$$

$$
\oint_C = \iint_D (2x + 2y) \, dA = 2 \iint_D (x + y) \, dA
$$

For circle $x^2 + y^2 = 1$, the integral of $x + y$ over the region is 0 (symmetry).

So $\oint_C = 0$

---

## 9. Stokes' Theorem

### 9.1 Stokes' Theorem

For a surface S bounded by curve C:

$$
\oint_C \mathbf{F} \cdot d\mathbf{r} = \iint_S (\nabla \times \mathbf{F}) \cdot d\mathbf{S}
$$

**Right-hand rule:** Thumb points in direction of normal, fingers curl in direction of integration.

---

### 9.2 Physical Interpretation

Stokes' theorem relates the line integral around a closed curve to the surface integral of the curl over any surface bounded by that curve.

**Applications:**
- Circulation of fluid flow
- Electromagnetic field calculations
- Conservative field identification

---

### 9.3 Example

Verify Stokes' theorem for $\mathbf{F} = (x - y)\mathbf{i} + xz\mathbf{j} - yzk\mathbf{k}$ over the triangle with vertices (0,0,0), (1,0,0), (0,1,0).

**First, compute curl:**
$$
\nabla \times \mathbf{F} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
x-y & xz & -yz
\end{vmatrix}
$$

$$
= \left( \frac{\partial}{\partial y}(-yz) - \frac{\partial}{\partial z}(xz) \right)\mathbf{i} + \left( \frac{\partial}{\partial z}(x-y) - \frac{\partial}{\partial x}(-yz) \right)\mathbf{j} + \left( \frac{\partial}{\partial x}(xz) - \frac{\partial}{\partial y}(x-y) \right)\mathbf{k}
$$

$$
= (-z - 0)\mathbf{i} + (0 - 0)\mathbf{j} + (z - 0)\mathbf{k} = -z\mathbf{i} + z\mathbf{k}
$$

**Surface integral:** $\iint_S (-z\mathbf{i} + z\mathbf{k}) \cdot d\mathbf{S}$

**Line integral:** $\oint_C \mathbf{F} \cdot d\mathbf{r}$

Both should equal for Stokes' theorem to hold.

---

## 10. Gauss' Divergence Theorem

### 10.1 Gauss' Divergence Theorem

For a closed surface S enclosing volume V:

$$
\iiint_V (\nabla \cdot \mathbf{F}) \, dV = \oint_S \mathbf{F} \cdot d\mathbf{S}
$$

---

### 10.2 Physical Interpretation

Gauss' theorem relates the volume integral of the divergence to the surface integral of the vector field over the boundary.

**Physical meaning:**
- Left side: Total "source strength" inside volume
- Right side: Net flux through boundary surface

**Applications:**
- Continuity equation in fluid dynamics
- Gauss's law in electrostatics
- Heat conduction problems

---

### 10.3 Example

Verify Gauss' theorem for $\mathbf{F} = x\mathbf{i} + y\mathbf{j} + z\mathbf{k}$ over the unit sphere $x^2 + y^2 + z^2 = 1$.

**First, compute divergence:**
$$
\nabla \cdot \mathbf{F} = \frac{\partial}{\partial x}(x) + \frac{\partial}{\partial y}(y) + \frac{\partial}{\partial z}(z) = 1 + 1 + 1 = 3
$$

**Volume integral:** $\iiint_V 3 \, dV = 3 \times \frac{4}{3}\pi(1)^3 = 4\pi$

**Surface integral:** $\oint_S \mathbf{F} \cdot d\mathbf{S}$

For unit sphere, $d\mathbf{S} = \mathbf{r} \, dS$ where $\mathbf{r} = x\mathbf{i} + y\mathbf{j} + z\mathbf{k}$

So $\mathbf{F} \cdot d\mathbf{S} = (x\mathbf{i} + y\mathbf{j} + z\mathbf{k}) \cdot (x\mathbf{i} + y\mathbf{j} + z\mathbf{k}) \, dS = (x^2 + y^2 + z^2) \, dS = 1 \cdot dS$

Thus $\oint_S = \oint_S dS = 4\pi$ (surface area of unit sphere)

Both sides equal: $4\pi = 4\pi$ ✓

---

## 📊 Topic Importance for GATE AG

| Topic | Frequency | Difficulty | GATE Weightage |
|-------|-----------|------------|----------------|
| **Gradient, Divergence, Curl** | Very High | Medium | ⭐⭐⭐⭐⭐ |
| **Line Integrals** | High | Medium | ⭐⭐⭐⭐ |
| **Green's Theorem** | High | Medium-Hard | ⭐⭐⭐⭐ |
| **Stokes' Theorem** | Medium | Hard | ⭐⭐⭐ |
| **Gauss' Theorem** | Medium | Hard | ⭐⭐⭐ |
| **Surface Integrals** | Medium | Medium | ⭐⭐⭐ |
| **Vector Algebra** | High | Easy-Medium | ⭐⭐⭐⭐ |
| **Volume Integrals** | Low | Medium | ⭐⭐ |

---

## 🎯 Key Formulas Quick Reference

### Vector Operations
$$
\mathbf{A} \cdot \mathbf{B} = A_x B_x + A_y B_y + A_z B_z
$$

$$
\mathbf{A} \times \mathbf{B} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
A_x & A_y & A_z \\
B_x & B_y & B_z
\end{vmatrix}
$$

### Differential Operators
$$
\nabla f = \frac{\partial f}{\partial x}\mathbf{i} + \frac{\partial f}{\partial y}\mathbf{j} + \frac{\partial f}{\partial z}\mathbf{k}
$$

$$
\nabla \cdot \mathbf{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y} + \frac{\partial F_z}{\partial z}
$$

$$
\nabla \times \mathbf{F} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
F_x & F_y & F_z
\end{vmatrix}
$$

### Theorems
$$
\oint_C P \, dx + Q \, dy = \iint_D \left( \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} \right) \, dA \quad \text{(Green's)}
$$

$$
\oint_C \mathbf{F} \cdot d\mathbf{r} = \iint_S (\nabla \times \mathbf{F}) \cdot d\mathbf{S} \quad \text{(Stokes')}
$$

$$
\iiint_V (\nabla \cdot \mathbf{F}) \, dV = \oint_S \mathbf{F} \cdot d\mathbf{S} \quad \text{(Gauss')}
$$

---

## 💡 Problem-Solving Strategy

### For Gradient, Divergence, Curl:
1. **Identify the operation** (∇f, ∇·F, ∇×F)
2. **Write the components** of the vector/scalar field
3. **Apply partial derivatives** systematically
4. **Combine terms** according to the formula

### For Line Integrals:
1. **Parametrize the curve** if needed
2. **Find ds or dr** depending on the integral type
3. **Substitute** the parametrization
4. **Evaluate** the definite integral

### For Surface Integrals:
1. **Choose parametrization** (u,v) for the surface
2. **Find the normal vector** dS
3. **Substitute** into the integral
4. **Evaluate** over the parameter domain

### For Theorems:
1. **Identify which theorem** applies (Green's/Stokes'/Gauss')
2. **Check conditions** (closed curve, orientable surface, etc.)
3. **Compute both sides** if verification is needed
4. **Interpret physically** what the result means

---

## 🔍 Common Mistakes to Avoid

1. **Wrong cross product order** - Remember determinant form
2. **Missing negative signs** in curl calculations
3. **Incorrect parametrization** for curves/surfaces
4. **Wrong orientation** for normal vectors
5. **Forgetting limits** in definite integrals
6. **Mixing scalar and vector** operations
7. **Wrong theorem application** (Green's is 2D, Stokes' and Gauss' are 3D)

---

## 📚 Related Topics

- [Calculus](../Calculus/README.md) - For partial derivatives and multiple integrals
- [Differential Equations](../Differential_Equations/README.md) - For vector fields
- [Linear Algebra](../Linear_Algebra/README.md) - For vector operations
- [Numerical Methods](../Numerical_Methods/README.md) - For numerical integration

---

**Last Updated:** November 2025  
**Version:** 1.0

---

*For practice problems, see [Vector Calculus PYQ Solutions](./Solutions.md)*  
*For quick revision, see [Vector Calculus Cheat Sheet](./CheatSheet.md)*
