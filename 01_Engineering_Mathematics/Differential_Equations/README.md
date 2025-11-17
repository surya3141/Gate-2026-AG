# 📐 Differential Equations - Concepts & Theory

> Comprehensive guide to Differential Equations for GATE AG

---

## 📚 Table of Contents

1. [First-Order ODEs](#1-first-order-odes)
2. [Higher-Order Linear ODEs](#2-higher-order-linear-odes)
3. [Laplace Transforms](#3-laplace-transforms)
4. [Inverse Laplace Transforms](#4-inverse-laplace-transforms)
5. [Partial Differential Equations](#5-partial-differential-equations)
6. [Applications](#6-applications)

---

## 1. First-Order ODEs

### 1.1 Basic Definitions

A **differential equation** is an equation involving derivatives of an unknown function.

**Order:** Highest derivative present  
**Degree:** Power of the highest derivative (after removing radicals and fractions)

**General form of first-order ODE:**
$$
\frac{dy}{dx} = f(x, y)
$$

### 1.2 Separable Equations

**Form:**
$$
\frac{dy}{dx} = g(x)h(y) \quad \text{or} \quad M(x)dx + N(y)dy = 0
$$

**Solution Method:**
1. Separate variables: $\frac{dy}{h(y)} = g(x)dx$
2. Integrate both sides: $\int \frac{dy}{h(y)} = \int g(x)dx$

**Example:**
$$
\frac{dy}{dx} = xy
$$

Solution:
$$
\frac{dy}{y} = x\,dx \implies \ln|y| = \frac{x^2}{2} + C \implies y = Ae^{x^2/2}
$$

### 1.3 Homogeneous Equations

**Form:** Equation where $f(x,y)$ can be written as $g(y/x)$
$$
\frac{dy}{dx} = f\left(\frac{y}{x}\right)
$$

**Solution Method:**
1. Substitute $v = \frac{y}{x}$, so $y = vx$
2. Then $\frac{dy}{dx} = v + x\frac{dv}{dx}$
3. Equation becomes separable in $v$ and $x$

**Example:**
$$
\frac{dy}{dx} = \frac{x+y}{x}
$$

This simplifies to: $\frac{dy}{dx} = 1 + \frac{y}{x}$ (homogeneous)

### 1.4 Linear First-Order ODEs

**Standard Form:**
$$
\frac{dy}{dx} + P(x)y = Q(x)
$$

**Solution Method (Integrating Factor):**

1. Find integrating factor: $\mu(x) = e^{\int P(x)dx}$
2. Multiply equation by $\mu(x)$
3. Left side becomes: $\frac{d}{dx}[\mu(x)y]$
4. Integrate: $\mu(x)y = \int \mu(x)Q(x)dx + C$

**General Solution:**
$$
y = \frac{1}{\mu(x)}\left[\int \mu(x)Q(x)dx + C\right]
$$

**Example:**
$$
\frac{dy}{dx} + 2y = e^{3x}
$$

Here $P(x) = 2$, $Q(x) = e^{3x}$

$$
\mu = e^{\int 2dx} = e^{2x}
$$

$$
e^{2x}y = \int e^{2x} \cdot e^{3x}dx = \int e^{5x}dx = \frac{e^{5x}}{5} + C
$$

$$
y = \frac{e^{5x}}{5e^{2x}} + \frac{C}{e^{2x}} = \frac{e^{3x}}{5} + Ce^{-2x}
$$

### 1.5 Exact Equations

**Form:**
$$
M(x,y)dx + N(x,y)dy = 0
$$

**Exactness Condition:**
$$
\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}
$$

**Solution Method:**
1. Check exactness condition
2. Find function $F(x,y)$ such that:
   - $\frac{\partial F}{\partial x} = M$
   - $\frac{\partial F}{\partial y} = N$
3. Solution is: $F(x,y) = C$

**Finding F:**
$$
F = \int M(x,y)dx + g(y)
$$

where $g(y)$ is found by ensuring $\frac{\partial F}{\partial y} = N$

### 1.6 Bernoulli's Equation

**Form:**
$$
\frac{dy}{dx} + P(x)y = Q(x)y^n, \quad n \neq 0, 1
$$

**Solution Method:**
1. Divide by $y^n$: $y^{-n}\frac{dy}{dx} + P(x)y^{1-n} = Q(x)$
2. Substitute $v = y^{1-n}$
3. Then $\frac{dv}{dx} = (1-n)y^{-n}\frac{dy}{dx}$
4. Equation becomes linear in $v$

---

## 2. Higher-Order Linear ODEs

### 2.1 General Form

**$n$-th order linear ODE with constant coefficients:**
$$
a_n\frac{d^ny}{dx^n} + a_{n-1}\frac{d^{n-1}y}{dx^{n-1}} + \cdots + a_1\frac{dy}{dx} + a_0y = f(x)
$$

**Homogeneous:** $f(x) = 0$  
**Non-homogeneous:** $f(x) \neq 0$

### 2.2 Second-Order Linear ODEs

**Standard Form:**
$$
\frac{d^2y}{dx^2} + P\frac{dy}{dx} + Qy = R(x)
$$

**Homogeneous form:** $R(x) = 0$

### 2.3 Solution of Homogeneous Equations

**Characteristic Equation Method:**

For: $ay'' + by' + cy = 0$

**Step 1:** Form characteristic equation:
$$
am^2 + bm + c = 0
$$

**Step 2:** Solve for roots $m_1, m_2$

**Step 3:** General solution depends on roots:

| Type of Roots | General Solution |
|---------------|------------------|
| Real and distinct: $m_1 \neq m_2$ | $y = C_1e^{m_1x} + C_2e^{m_2x}$ |
| Real and equal: $m_1 = m_2 = m$ | $y = (C_1 + C_2x)e^{mx}$ |
| Complex: $m = \alpha \pm i\beta$ | $y = e^{\alpha x}(C_1\cos\beta x + C_2\sin\beta x)$ |

**Example 1:** $y'' - 5y' + 6y = 0$

Characteristic equation: $m^2 - 5m + 6 = 0$

$(m-2)(m-3) = 0 \implies m = 2, 3$

Solution: $y = C_1e^{2x} + C_2e^{3x}$

**Example 2:** $y'' + 4y' + 4y = 0$

Characteristic equation: $m^2 + 4m + 4 = 0$

$(m+2)^2 = 0 \implies m = -2, -2$ (repeated)

Solution: $y = (C_1 + C_2x)e^{-2x}$

**Example 3:** $y'' + 4y = 0$

Characteristic equation: $m^2 + 4 = 0$

$m = \pm 2i$ (complex: $\alpha = 0, \beta = 2$)

Solution: $y = C_1\cos 2x + C_2\sin 2x$

### 2.4 Non-Homogeneous Equations

**Complete Solution:**
$$
y = y_c + y_p
$$

where:
- $y_c$ = Complementary function (solution of homogeneous equation)
- $y_p$ = Particular integral (particular solution)

### 2.5 Method of Undetermined Coefficients

**For:** $ay'' + by' + cy = f(x)$

**Choose $y_p$ based on $f(x)$:**

| $f(x)$ | Trial $y_p$ |
|--------|-------------|
| $ke^{ax}$ | $Ae^{ax}$ |
| $k\sin(ax)$ or $k\cos(ax)$ | $A\cos(ax) + B\sin(ax)$ |
| $kx^n$ (polynomial) | $A_nx^n + A_{n-1}x^{n-1} + \cdots + A_1x + A_0$ |
| $ke^{ax}\sin(bx)$ | $e^{ax}(A\cos bx + B\sin bx)$ |
| $ke^{ax}\cos(bx)$ | $e^{ax}(A\cos bx + B\sin bx)$ |

**⚠️ Modification Rule:** If trial $y_p$ matches any term in $y_c$, multiply by $x$ (or $x^2$ if needed).

**Example:** $y'' - 3y' + 2y = e^{2x}$

1. Find $y_c$: $m^2 - 3m + 2 = 0 \implies m = 1, 2$
   
   $y_c = C_1e^x + C_2e^{2x}$

2. Try $y_p = Ae^{2x}$, but this matches $y_c$ term!
   
   **Modified:** $y_p = Axe^{2x}$

3. Find $y_p'$ and $y_p''$, substitute, solve for $A$

### 2.6 Method of Variation of Parameters

**For:** $y'' + Py' + Qy = R(x)$

**Steps:**
1. Find $y_c = C_1y_1 + C_2y_2$ (homogeneous solution)
2. Particular solution:
$$
y_p = u_1y_1 + u_2y_2
$$

where:
$$
u_1 = -\int \frac{y_2R}{W}dx, \quad u_2 = \int \frac{y_1R}{W}dx
$$

**Wronskian:**
$$
W = \begin{vmatrix} y_1 & y_2 \\ y_1' & y_2' \end{vmatrix} = y_1y_2' - y_2y_1'
$$

---

## 3. Laplace Transforms

### 3.1 Definition

The **Laplace Transform** of a function $f(t)$ is:
$$
\mathcal{L}\{f(t)\} = F(s) = \int_0^\infty e^{-st}f(t)dt
$$

where $s$ is a complex parameter.

### 3.2 Standard Laplace Transforms

#### Basic Functions
$$
\begin{aligned}
&\mathcal{L}\{1\} = \frac{1}{s} \\
&\mathcal{L}\{t\} = \frac{1}{s^2} \\
&\mathcal{L}\{t^n\} = \frac{n!}{s^{n+1}} \\
&\mathcal{L}\{e^{at}\} = \frac{1}{s-a} \\
&\mathcal{L}\{\sin at\} = \frac{a}{s^2+a^2} \\
&\mathcal{L}\{\cos at\} = \frac{s}{s^2+a^2} \\
&\mathcal{L}\{\sinh at\} = \frac{a}{s^2-a^2} \\
&\mathcal{L}\{\cosh at\} = \frac{s}{s^2-a^2}
\end{aligned}
$$

#### Combined Functions
$$
\begin{aligned}
&\mathcal{L}\{e^{at}\sin bt\} = \frac{b}{(s-a)^2+b^2} \\
&\mathcal{L}\{e^{at}\cos bt\} = \frac{s-a}{(s-a)^2+b^2} \\
&\mathcal{L}\{t^n e^{at}\} = \frac{n!}{(s-a)^{n+1}}
\end{aligned}
$$

### 3.3 Properties of Laplace Transform

#### Linearity
$$
\mathcal{L}\{af(t) + bg(t)\} = a\mathcal{L}\{f(t)\} + b\mathcal{L}\{g(t)\}
$$

#### First Shifting Theorem
$$
\mathcal{L}\{e^{at}f(t)\} = F(s-a)
$$

#### Second Shifting Theorem
$$
\mathcal{L}\{f(t-a)u(t-a)\} = e^{-as}F(s)
$$

where $u(t-a)$ is the unit step function.

#### Derivative Property
$$
\begin{aligned}
&\mathcal{L}\{f'(t)\} = sF(s) - f(0) \\
&\mathcal{L}\{f''(t)\} = s^2F(s) - sf(0) - f'(0) \\
&\mathcal{L}\{f^{(n)}(t)\} = s^nF(s) - s^{n-1}f(0) - s^{n-2}f'(0) - \cdots - f^{(n-1)}(0)
\end{aligned}
$$

#### Integration Property
$$
\mathcal{L}\left\{\int_0^t f(\tau)d\tau\right\} = \frac{F(s)}{s}
$$

#### Multiplication by $t^n$
$$
\mathcal{L}\{t^n f(t)\} = (-1)^n \frac{d^n F(s)}{ds^n}
$$

#### Division by $t$
$$
\mathcal{L}\left\{\frac{f(t)}{t}\right\} = \int_s^\infty F(u)du
$$

### 3.4 Solving ODEs using Laplace Transform

**Steps:**
1. Take Laplace transform of entire equation
2. Use initial conditions to simplify
3. Solve algebraically for $Y(s) = \mathcal{L}\{y(t)\}$
4. Take inverse Laplace transform to get $y(t)$

**Example:** Solve $y'' + 4y = 0$, $y(0) = 1$, $y'(0) = 0$

$$
\mathcal{L}\{y''\} + 4\mathcal{L}\{y\} = 0
$$

$$
[s^2Y(s) - s \cdot 1 - 0] + 4Y(s) = 0
$$

$$
(s^2 + 4)Y(s) = s
$$

$$
Y(s) = \frac{s}{s^2+4}
$$

$$
y(t) = \mathcal{L}^{-1}\left\{\frac{s}{s^2+4}\right\} = \cos 2t
$$

---

## 4. Inverse Laplace Transforms

### 4.1 Definition

If $\mathcal{L}\{f(t)\} = F(s)$, then:
$$
f(t) = \mathcal{L}^{-1}\{F(s)\}
$$

### 4.2 Standard Inverse Transforms

$$
\begin{aligned}
&\mathcal{L}^{-1}\left\{\frac{1}{s}\right\} = 1 \\
&\mathcal{L}^{-1}\left\{\frac{1}{s^n}\right\} = \frac{t^{n-1}}{(n-1)!} \\
&\mathcal{L}^{-1}\left\{\frac{1}{s-a}\right\} = e^{at} \\
&\mathcal{L}^{-1}\left\{\frac{a}{s^2+a^2}\right\} = \sin at \\
&\mathcal{L}^{-1}\left\{\frac{s}{s^2+a^2}\right\} = \cos at \\
&\mathcal{L}^{-1}\left\{\frac{a}{s^2-a^2}\right\} = \sinh at \\
&\mathcal{L}^{-1}\left\{\frac{s}{s^2-a^2}\right\} = \cosh at
\end{aligned}
$$

### 4.3 Partial Fractions Method

**For rational functions:** $\frac{P(s)}{Q(s)}$ where degree of $P < $ degree of $Q$

**Step 1:** Factor denominator $Q(s)$

**Step 2:** Decompose into partial fractions:

| Factor Type | Partial Fraction |
|-------------|------------------|
| Linear $(s-a)$ | $\frac{A}{s-a}$ |
| Repeated $(s-a)^n$ | $\frac{A_1}{s-a} + \frac{A_2}{(s-a)^2} + \cdots + \frac{A_n}{(s-a)^n}$ |
| Quadratic $s^2+as+b$ | $\frac{As+B}{s^2+as+b}$ |

**Step 3:** Find constants $A, B, C, \ldots$

**Step 4:** Take inverse transform of each term

**Example:**
$$
F(s) = \frac{2s+1}{s^2+3s+2} = \frac{2s+1}{(s+1)(s+2)}
$$

Partial fractions:
$$
\frac{2s+1}{(s+1)(s+2)} = \frac{A}{s+1} + \frac{B}{s+2}
$$

Solving: $2s+1 = A(s+2) + B(s+1)$

$s = -1$: $-1 = A(1) \implies A = -1$

$s = -2$: $-3 = B(-1) \implies B = 3$

$$
F(s) = \frac{-1}{s+1} + \frac{3}{s+2}
$$

$$
f(t) = -e^{-t} + 3e^{-2t}
$$

### 4.4 Convolution Theorem

$$
\mathcal{L}^{-1}\{F(s)G(s)\} = \int_0^t f(\tau)g(t-\tau)d\tau = f(t) * g(t)
$$

**Useful when inverse of product is needed.**

---

## 5. Partial Differential Equations

### 5.1 Basic Definitions

A **PDE** contains partial derivatives of an unknown function of two or more variables.

**Order:** Highest partial derivative  
**Degree:** Power of highest partial derivative (when rationalized)

**General first-order PDE:**
$$
F\left(x, y, u, \frac{\partial u}{\partial x}, \frac{\partial u}{\partial y}\right) = 0
$$

**General second-order PDE:**
$$
A\frac{\partial^2 u}{\partial x^2} + B\frac{\partial^2 u}{\partial x\partial y} + C\frac{\partial^2 u}{\partial y^2} + \text{lower order terms} = 0
$$

### 5.2 Classification of Second-Order PDEs

For: $Au_{xx} + Bu_{xy} + Cu_{yy} + \cdots = 0$

**Discriminant:** $\Delta = B^2 - 4AC$

| Type | Condition | Example |
|------|-----------|---------|
| **Hyperbolic** | $B^2 - 4AC > 0$ | Wave equation |
| **Parabolic** | $B^2 - 4AC = 0$ | Heat equation |
| **Elliptic** | $B^2 - 4AC < 0$ | Laplace equation |

### 5.3 One-Dimensional Wave Equation

**Physical Meaning:** Vibration of strings, sound waves

**Standard Form:**
$$
\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}
$$

where $c$ is the wave velocity.

**D'Alembert's Solution:**
$$
u(x,t) = f(x-ct) + g(x+ct)
$$

where $f$ and $g$ are arbitrary functions determined by initial/boundary conditions.

**Solution by Separation of Variables:**

Assume $u(x,t) = X(x)T(t)$

Substituting:
$$
X(x)T''(t) = c^2X''(x)T(t)
$$

$$
\frac{T''(t)}{c^2T(t)} = \frac{X''(x)}{X(x)} = -\lambda \quad \text{(separation constant)}
$$

This gives two ODEs:
$$
X'' + \lambda X = 0, \quad T'' + \lambda c^2 T = 0
$$

### 5.4 One-Dimensional Heat Equation

**Physical Meaning:** Heat conduction, diffusion

**Standard Form:**
$$
\frac{\partial u}{\partial t} = \alpha^2 \frac{\partial^2 u}{\partial x^2}
$$

where $\alpha^2$ is the thermal diffusivity.

**Solution by Separation of Variables:**

Assume $u(x,t) = X(x)T(t)$

$$
\frac{T'(t)}{\alpha^2 T(t)} = \frac{X''(x)}{X(x)} = -\lambda
$$

Two ODEs:
$$
X'' + \lambda X = 0, \quad T' + \lambda\alpha^2 T = 0
$$

**General solution** (with boundary conditions):
$$
u(x,t) = \sum_{n=1}^{\infty} B_n e^{-\alpha^2 n^2\pi^2 t/L^2}\sin\frac{n\pi x}{L}
$$

### 5.5 Two-Dimensional Laplace Equation

**Physical Meaning:** Steady-state heat distribution, electrostatics

**Standard Form:**
$$
\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0 \quad \text{or} \quad \nabla^2 u = 0
$$

**Solution by Separation of Variables:**

Assume $u(x,y) = X(x)Y(y)$

$$
\frac{X''(x)}{X(x)} + \frac{Y''(y)}{Y(y)} = 0
$$

$$
\frac{X''(x)}{X(x)} = -\frac{Y''(y)}{Y(y)} = \pm\lambda
$$

Leads to:
$$
X'' \mp \lambda X = 0, \quad Y'' \pm \lambda Y = 0
$$

**Solutions depend on sign and boundary conditions.**

### 5.6 Method of Separation of Variables

**General Steps:**

1. Assume $u(x,t)$ or $u(x,y)$ can be written as product: $u = X(x)T(t)$ or $X(x)Y(y)$
2. Substitute into PDE
3. Separate variables to get two ODEs
4. Solve each ODE with boundary conditions
5. Combine solutions (often as infinite series)

---

## 6. Applications

### 6.1 Population Growth Models

**Exponential Growth:**
$$
\frac{dP}{dt} = kP \implies P(t) = P_0e^{kt}
$$

**Logistic Growth:**
$$
\frac{dP}{dt} = kP\left(1 - \frac{P}{M}\right)
$$

where $M$ is carrying capacity.

### 6.2 Newton's Law of Cooling

$$
\frac{dT}{dt} = -k(T - T_s)
$$

where $T$ is object temperature, $T_s$ is surrounding temperature.

**Solution:**
$$
T(t) = T_s + (T_0 - T_s)e^{-kt}
$$

### 6.3 RL and RC Circuits

**RL Circuit:**
$$
L\frac{di}{dt} + Ri = V(t)
$$

**RC Circuit:**
$$
R\frac{dq}{dt} + \frac{q}{C} = V(t)
$$

### 6.4 Simple Harmonic Motion

**Undamped:**
$$
m\frac{d^2x}{dt^2} + kx = 0
$$

**Solution:** $x(t) = A\cos(\omega t + \phi)$ where $\omega = \sqrt{k/m}$

**Damped:**
$$
m\frac{d^2x}{dt^2} + c\frac{dx}{dt} + kx = 0
$$

---

## 📊 Topic Importance for GATE AG

| Topic | Weightage | Difficulty |
|-------|-----------|------------|
| First-Order ODEs | High | Easy-Medium |
| Second-Order Linear ODEs | Very High | Medium |
| Laplace Transforms | High | Medium-Hard |
| Inverse Laplace | High | Medium |
| PDEs (Wave, Heat, Laplace) | Medium | Medium-Hard |
| Applications | Medium | Medium |

---

## 🎯 Exam Strategy

1. **Master characteristic equation method** - Most common question type
2. **Memorize Laplace transform table** - Direct application questions
3. **Practice partial fractions** - Essential for inverse Laplace
4. **Understand boundary conditions** - Critical for PDEs
5. **Know method of undetermined coefficients** - Fast for particular solutions
6. **Learn separation of variables** - Standard PDE technique

---

## 📚 Related Topics

- [Calculus](../Calculus/)
- [Linear Algebra](../Linear_Algebra/)
- [Vector Calculus](../Vector_Calculus/)
- [Numerical Methods](../Numerical_Methods/)

---

**Last Updated:** November 2025  
**Version:** 1.0
