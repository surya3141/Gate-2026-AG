# 📝 Vector Calculus Cheat Sheet

> Quick reference for GATE Agricultural Engineering

---

## 📐 Vector Algebra

### Vector Operations
$$
\mathbf{A} \pm \mathbf{B} = (A_x \pm B_x)\mathbf{i} + (A_y \pm B_y)\mathbf{j} + (A_z \pm B_z)\mathbf{k}
$$

$$
\mathbf{A} \cdot \mathbf{B} = A_x B_x + A_y B_y + A_z B_z = |\mathbf{A}||\mathbf{B}|\cos\theta
$$

$$
\mathbf{A} \times \mathbf{B} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
A_x & A_y & A_z \\
B_x & B_y & B_z
\end{vmatrix} = (A_y B_z - A_z B_y)\mathbf{i} + (A_z B_x - A_x B_z)\mathbf{j} + (A_x B_y - A_y B_x)\mathbf{k}
$$

### Vector Identities
- **Commutative:** $\mathbf{A} \cdot \mathbf{B} = \mathbf{B} \cdot \mathbf{A}$
- **Anti-commutative:** $\mathbf{A} \times \mathbf{B} = -(\mathbf{B} \times \mathbf{A})$
- **Scalar Triple Product:** $\mathbf{A} \cdot (\mathbf{B} \times \mathbf{C}) = \begin{vmatrix} A_x & A_y & A_z \\ B_x & B_y & B_z \\ C_x & C_y & C_z \end{vmatrix}$
- **Vector Triple Product:** $\mathbf{A} \times (\mathbf{B} \times \mathbf{C}) = (\mathbf{A} \cdot \mathbf{C})\mathbf{B} - (\mathbf{A} \cdot \mathbf{B})\mathbf{C}$

---

## 🔺 Differential Operators

### Gradient (∇f)
$$
\nabla f = \frac{\partial f}{\partial x}\mathbf{i} + \frac{\partial f}{\partial y}\mathbf{j} + \frac{\partial f}{\partial z}\mathbf{k}
$$

**Directional Derivative:** $\frac{df}{ds} = \nabla f \cdot \mathbf{u}$

**Maximum Rate:** $|\nabla f|$

### Divergence (∇·F)
$$
\nabla \cdot \mathbf{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y} + \frac{\partial F_z}{\partial z}
$$

**Physical Meaning:**
- ∇·F > 0: Source
- ∇·F < 0: Sink
- ∇·F = 0: Incompressible

### Curl (∇×F)
$$
\nabla \times \mathbf{F} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
F_x & F_y & F_z
\end{vmatrix}
$$

**Physical Meaning:**
- ∇×F = 0: Irrotational (conservative)
- ∇×F ≠ 0: Rotational

---

## ∫ Line Integrals

### Scalar Line Integral
$$
\int_C f(x,y,z) \, ds = \int_a^b f(x(t),y(t),z(t)) \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2 + \left(\frac{dz}{dt}\right)^2} \, dt
$$

### Vector Line Integral
$$
\int_C \mathbf{F} \cdot d\mathbf{r} = \int_a^b \mathbf{F}(x(t),y(t),z(t)) \cdot \frac{d\mathbf{r}}{dt} \, dt
$$

**Work Done:** W = ∫_C F · dr

**Conservative Field:** ∫_C F · dr = φ(A) - φ(B)

---

## ∬ Surface Integrals

### Scalar Surface Integral
$$
\iint_S f(x,y,z) \, dS = \iint_D f(x(u,v),y(u,v),z(u,v)) \sqrt{EG - F^2} \, du \, dv
$$

### Vector Surface Integral (Flux)
$$
\iint_S \mathbf{F} \cdot d\mathbf{S} = \iint_D \mathbf{F} \cdot \left( \frac{\partial \mathbf{r}}{\partial u} \times \frac{\partial \mathbf{r}}{\partial v} \right) du \, dv
$$

**Flux:** Φ = ∬_S F · n̂ dS

---

## ∭ Volume Integrals

### Scalar Volume Integral
$$
\iiint_V f(x,y,z) \, dV
$$

### Applications
**Mass:** M = ∭_V ρ dV

**Center of Mass:** $\bar{x} = \frac{1}{M} \iiint_V x \rho \, dV$

---

## 📏 Green's Theorem (2D)

For region D with boundary C:

$$
\oint_C P \, dx + Q \, dy = \iint_D \left( \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} \right) dA
$$

**Vector Form:** $\oint_C \mathbf{F} \cdot d\mathbf{r} = \iint_D (\nabla \times \mathbf{F}) \cdot \mathbf{k} \, dA$

**Area Formula:** Area = $\frac{1}{2} \oint_C (x dy - y dx)$

---

## 🌀 Stokes' Theorem

For surface S with boundary C:

$$
\oint_C \mathbf{F} \cdot d\mathbf{r} = \iint_S (\nabla \times \mathbf{F}) \cdot d\mathbf{S}
$$

**Right-Hand Rule:** Thumb in direction of normal, fingers along boundary.

**Applications:**
- Circulation: Γ = ∮_C V · dr
- Conservative field check

---

## 🌐 Gauss' Divergence Theorem

For closed surface S enclosing volume V:

$$
\iiint_V (\nabla \cdot \mathbf{F}) \, dV = \oint_S \mathbf{F} \cdot d\mathbf{S}
$$

**Physical Meaning:**
- Left: Total source strength
- Right: Net outward flux

**Applications:**
- Continuity equation
- Gauss's law
- Heat conduction

---

## 🧮 Key Formulas & Identities

### Vector Operator Identities
1. ∇ · (∇ × F) = 0
2. ∇ × (∇f) = 0
3. ∇ · (∇f) = ∇²f (Laplacian)
4. ∇ · (F × G) = G · (∇ × F) - F · (∇ × G)
5. ∇ × (F × G) = (G · ∇)F - (F · ∇)G + F(∇ · G) - G(∇ · F)
6. ∇ × (∇ × F) = ∇(∇ · F) - ∇²F

### Product Rules
- ∇(fg) = f∇g + g∇f
- ∇ · (fF) = f(∇ · F) + F · ∇f
- ∇ × (fF) = f(∇ × F) + ∇f × F

### Chain Rule
- ∇(f(g)) = f'(g) ∇g

---

## 📊 Comparison Table

| Operator | Scalar Field f | Vector Field F | Result Type |
|----------|----------------|----------------|-------------|
| **Gradient** | ∇f | - | Vector |
| **Divergence** | - | ∇·F | Scalar |
| **Curl** | - | ∇×F | Vector |
| **Laplacian** | ∇²f | ∇²F | Scalar/Vector |

---

## 🎯 Problem-Solving Templates

### For Gradient Problems:
1. Write f(x,y,z)
2. Compute ∂f/∂x, ∂f/∂y, ∂f/∂z
3. Combine: ∇f = (∂f/∂x)i + (∂f/∂y)j + (∂f/∂z)k

### For Divergence Problems:
1. Write F = Fx i + Fy j + Fz k
2. Compute ∂Fx/∂x + ∂Fy/∂y + ∂Fz/∂z
3. Result is scalar

### For Curl Problems:
1. Write F components in determinant
2. Compute i, j, k components
3. Result is vector

### For Line Integrals:
1. Parametrize curve: x(t), y(t), z(t)
2. Find dr/dt
3. Substitute and integrate

### For Surface Integrals:
1. Parametrize surface: x(u,v), y(u,v), z(u,v)
2. Find ∂r/∂u × ∂r/∂v
3. Substitute F · (normal) into double integral

### For Theorems:
1. **Green's:** Check if 2D, closed curve
2. **Stokes':** Check surface orientation
3. **Gauss':** Check closed surface

---

## ⚡ Quick Memory Tricks

### Curl Determinant:
- i component: ∂/∂y (Fz) - ∂/∂z (Fy)
- j component: ∂/∂z (Fx) - ∂/∂x (Fz)
- k component: ∂/∂x (Fy) - ∂/∂y (Fx)

### Cross Product:
- i: Ay Bz - Az By
- j: Az Bx - Ax Bz
- k: Ax By - Ay Bx

### Triple Products:
- Scalar: Determinant of matrix
- Vector: BAC - CAB rule

---

## 🚨 Common Mistakes

1. **Wrong curl order** in determinant
2. **Missing negative signs** in cross products
3. **Incorrect parametrization** limits
4. **Wrong normal direction** for surfaces
5. **Forgetting orientation** in theorems
6. **Mixing scalar/vector** operations
7. **Wrong theorem application**

---

## 📈 GATE Weightage & Tips

| Topic | Marks (Typical) | Frequency | Key Points |
|-------|-----------------|-----------|------------|
| **Gradient** | 1-2 | High | Component calculation |
| **Divergence** | 1-2 | High | Sum of partials |
| **Curl** | 1-2 | High | Determinant form |
| **Line Integrals** | 2-3 | Medium | Parametrization |
| **Green's Theorem** | 2-3 | Medium | 2D regions |
| **Stokes' Theorem** | 2-3 | Low | Orientation |
| **Gauss' Theorem** | 2-3 | Low | Closed surfaces |

### Exam Strategy:
- **Easy marks:** Basic grad/div/curl calculations
- **Medium marks:** Line integrals, Green's theorem
- **Hard marks:** Stokes'/Gauss' theorem applications
- **Time management:** 2-3 minutes per question

---

## 🔗 Related Formulas

### From Calculus:
- **Partial Derivatives:** ∂f/∂x, ∂f/∂y, ∂f/∂z
- **Multiple Integrals:** ∬, ∭
- **Chain Rule:** df/dx = ∂f/∂u · du/dx

### From Linear Algebra:
- **Vector Operations:** Dot, cross products
- **Matrix Operations:** Determinants
- **Coordinate Systems:** Cartesian, cylindrical, spherical

---

## 📝 Quick Check Questions

1. **Gradient of x² + y² + z²?** → 2(x i + y j + z k)
2. **Divergence of x i + y j + z k?** → 3
3. **Curl of y i + x j?** → 2 k
4. **Green's theorem converts?** → Line integral to double integral
5. **Stokes' theorem relates?** → Line integral to surface integral
6. **Gauss' theorem relates?** → Volume integral to surface integral

---

## 🎯 Final Tips

- **Practice parametrization** for curves and surfaces
- **Master determinant forms** for curl and cross products
- **Understand physical meanings** of operators
- **Know when to apply** each theorem
- **Check orientations** carefully
- **Use symmetry** to simplify calculations

---

**Created for:** GATE Agricultural Engineering  
**Last Updated:** November 2025  
**Total Formulas:** 25+  
**Key Topics:** 10

---

*For detailed theory, see [Vector Calculus README](./README.md)*  
*For practice problems, see [PYQ Solutions](./Solutions.md)*
