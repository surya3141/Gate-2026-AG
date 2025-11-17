# 📋 Differential Equations - Cheat Sheet

> Quick reference formulas, shortcuts, and tips for GATE AG

---

## 🎯 Quick Formula Reference

### 1. First-Order ODE Types & Solutions

#### Variable Separable
**Form:** $\frac{dy}{dx} = g(x)h(y)$

**Solution:**
$$
\int \frac{dy}{h(y)} = \int g(x)dx
$$

**Quick Example:** $\frac{dy}{dx} = \frac{y}{x}$ → $y = Cx$

---

#### Linear First-Order
**Standard Form:**
$$
\frac{dy}{dx} + P(x)y = Q(x)
$$

**Solution Formula:**
$$
y \cdot e^{\int P dx} = \int Q \cdot e^{\int P dx} dx + C
$$

**Integrating Factor (⭐ Most Important!):**
$$
\mu(x) = e^{\int P(x)dx}
$$

**Steps:**
1. Find $\mu = e^{\int P dx}$
2. Multiply equation by $\mu$
3. Left side becomes $\frac{d}{dx}(\mu y)$
4. Integrate: $\mu y = \int \mu Q dx + C$

---

#### Homogeneous Equation
**Form:** $\frac{dy}{dx} = f\left(\frac{y}{x}\right)$

**Substitution:** $v = \frac{y}{x}$, so $y = vx$ and $\frac{dy}{dx} = v + x\frac{dv}{dx}$

**Result:** Equation becomes separable in $v$ and $x$

---

#### Exact Equation
**Form:** $M(x,y)dx + N(x,y)dy = 0$

**Exactness Test (⭐ Must Check!):**
$$
\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}
$$

**Solution:** Find $F(x,y)$ such that:
$$
\frac{\partial F}{\partial x} = M, \quad \frac{\partial F}{\partial y} = N
$$

Then $F(x,y) = C$ is the solution.

**Quick Method:**
$$
F = \int M dx + g(y)
$$

Find $g(y)$ by ensuring $\frac{\partial F}{\partial y} = N$

---

#### Bernoulli's Equation
**Form:**
$$
\frac{dy}{dx} + P(x)y = Q(x)y^n, \quad n \neq 0, 1
$$

**Substitution:** $v = y^{1-n}$

**Result:** Becomes linear in $v$

---

### 2. Second-Order Linear ODEs

#### Standard Form
$$
ay'' + by' + cy = f(x)
$$

**Complete Solution:**
$$
y = y_c + y_p
$$

- $y_c$ = Complementary function (homogeneous solution)
- $y_p$ = Particular integral

---

#### Characteristic Equation Method

**For:** $ay'' + by' + cy = 0$

**Characteristic Equation:**
$$
am^2 + bm + c = 0
$$

**Solution Based on Roots:**

| Root Type | Roots | Solution $y_c$ |
|-----------|-------|---------------|
| **Real & Distinct** | $m_1 \neq m_2$ | $C_1e^{m_1x} + C_2e^{m_2x}$ |
| **Real & Equal** | $m_1 = m_2 = m$ | $(C_1 + C_2x)e^{mx}$ |
| **Complex** | $\alpha \pm i\beta$ | $e^{\alpha x}(C_1\cos\beta x + C_2\sin\beta x)$ |

**Memory Aid:**
- Distinct → Two separate exponentials
- Repeated → Multiply by $(C_1 + C_2x)$
- Complex → Exponential times trig functions

---

#### Finding Roots Quickly

**Quadratic Formula:**
$$
m = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

**Discriminant:**
$$
\Delta = b^2 - 4ac
$$

| Discriminant | Root Type |
|--------------|-----------|
| $\Delta > 0$ | Real & Distinct |
| $\Delta = 0$ | Real & Equal (Repeated) |
| $\Delta < 0$ | Complex Conjugates |

**For Complex Roots:** $m = \alpha \pm i\beta$
$$
\alpha = \frac{-b}{2a}, \quad \beta = \frac{\sqrt{4ac - b^2}}{2a}
$$

---

#### Method of Undetermined Coefficients

**Choose $y_p$ based on $f(x)$:**

| $f(x)$ | Trial $y_p$ |
|--------|-------------|
| $ke^{ax}$ | $Ae^{ax}$ |
| $k\sin(bx)$ | $A\cos(bx) + B\sin(bx)$ |
| $k\cos(bx)$ | $A\cos(bx) + B\sin(bx)$ |
| $kx^n$ | $A_nx^n + A_{n-1}x^{n-1} + \cdots + A_0$ |
| $ke^{ax}\sin(bx)$ | $e^{ax}(A\cos bx + B\sin bx)$ |
| $ke^{ax}\cos(bx)$ | $e^{ax}(A\cos bx + B\sin bx)$ |

**⚠️ Modification Rule (Resonance):**

If any term of trial $y_p$ appears in $y_c$:
- Multiply trial $y_p$ by $x$
- If still matches, multiply by $x^2$

**Example:** For $y'' + 4y = \sin 2x$
- $y_c = C_1\cos 2x + C_2\sin 2x$ (contains $\sin 2x$!)
- Modified $y_p = x(A\cos 2x + B\sin 2x)$

---

### 3. Laplace Transforms

#### Standard Transforms (⭐ Must Memorize!)

| $f(t)$ | $\mathcal{L}\{f(t)\} = F(s)$ |
|--------|-------------------------------|
| $1$ | $\frac{1}{s}$ |
| $t$ | $\frac{1}{s^2}$ |
| $t^n$ | $\frac{n!}{s^{n+1}}$ |
| $e^{at}$ | $\frac{1}{s-a}$ |
| $\sin at$ | $\frac{a}{s^2+a^2}$ |
| $\cos at$ | $\frac{s}{s^2+a^2}$ |
| $\sinh at$ | $\frac{a}{s^2-a^2}$ |
| $\cosh at$ | $\frac{s}{s^2-a^2}$ |
| $t^n e^{at}$ | $\frac{n!}{(s-a)^{n+1}}$ |
| $e^{at}\sin bt$ | $\frac{b}{(s-a)^2+b^2}$ |
| $e^{at}\cos bt$ | $\frac{s-a}{(s-a)^2+b^2}$ |

**Memory Tricks:**
- $\sin$ → numerator has just $a$
- $\cos$ → numerator has $s$
- Hyperbolic → denominator has minus sign

---

#### Laplace Transform Properties

**Linearity:**
$$
\mathcal{L}\{af(t) + bg(t)\} = aF(s) + bG(s)
$$

**First Shifting Theorem (⭐ Very Useful!):**
$$
\mathcal{L}\{e^{at}f(t)\} = F(s-a)
$$

**Pattern:** Replace $s$ with $(s-a)$ in $F(s)$

**Derivative Transform (⭐ Most Important!):**
$$
\begin{aligned}
\mathcal{L}\{f'(t)\} &= sF(s) - f(0) \\
\mathcal{L}\{f''(t)\} &= s^2F(s) - sf(0) - f'(0) \\
\mathcal{L}\{f'''(t)\} &= s^3F(s) - s^2f(0) - sf'(0) - f''(0)
\end{aligned}
$$

**General Form:**
$$
\mathcal{L}\{f^{(n)}(t)\} = s^nF(s) - s^{n-1}f(0) - s^{n-2}f'(0) - \cdots - f^{(n-1)}(0)
$$

**Integration Transform:**
$$
\mathcal{L}\left\{\int_0^t f(\tau)d\tau\right\} = \frac{F(s)}{s}
$$

**Multiplication by $t$:**
$$
\mathcal{L}\{tf(t)\} = -\frac{dF(s)}{ds}
$$

**Division by $t$:**
$$
\mathcal{L}\left\{\frac{f(t)}{t}\right\} = \int_s^\infty F(u)du
$$

---

### 4. Inverse Laplace Transforms

#### Standard Inverse Transforms

| $F(s)$ | $\mathcal{L}^{-1}\{F(s)\} = f(t)$ |
|--------|-----------------------------------|
| $\frac{1}{s}$ | $1$ |
| $\frac{1}{s^n}$ | $\frac{t^{n-1}}{(n-1)!}$ |
| $\frac{1}{s-a}$ | $e^{at}$ |
| $\frac{a}{s^2+a^2}$ | $\sin at$ |
| $\frac{s}{s^2+a^2}$ | $\cos at$ |
| $\frac{a}{s^2-a^2}$ | $\sinh at$ |
| $\frac{s}{s^2-a^2}$ | $\cosh at$ |
| $\frac{1}{(s-a)^n}$ | $\frac{t^{n-1}e^{at}}{(n-1)!}$ |
| $\frac{b}{(s-a)^2+b^2}$ | $e^{at}\sin bt$ |
| $\frac{s-a}{(s-a)^2+b^2}$ | $e^{at}\cos bt$ |

---

#### Partial Fractions Method (⭐ Essential Skill!)

**For:** $\frac{P(s)}{Q(s)}$ where degree of $P < $ degree of $Q$

**Step 1:** Factor $Q(s)$ completely

**Step 2:** Decompose based on factor type:

| Factor in $Q(s)$ | Partial Fraction Terms |
|------------------|------------------------|
| $(s-a)$ | $\frac{A}{s-a}$ |
| $(s-a)^2$ | $\frac{A}{s-a} + \frac{B}{(s-a)^2}$ |
| $(s-a)^n$ | $\frac{A_1}{s-a} + \frac{A_2}{(s-a)^2} + \cdots + \frac{A_n}{(s-a)^n}$ |
| $s^2+as+b$ (irreducible) | $\frac{As+B}{s^2+as+b}$ |

**Step 3:** Find constants using:

**Method 1: Cover-up (Fastest for linear factors)**

For $\frac{A}{s-a}$: Cover $(s-a)$ in denominator, substitute $s = a$ in remaining expression

**Method 2: Equating coefficients**

Multiply out and compare coefficients of powers of $s$

**Example:**
$$
\frac{2s+3}{(s+1)(s+2)} = \frac{A}{s+1} + \frac{B}{s+2}
$$

Cover-up at $s = -1$: $A = \frac{2(-1)+3}{(-1+2)} = 1$

Cover-up at $s = -2$: $B = \frac{2(-2)+3}{(-2+1)} = 1$

Result: $\frac{1}{s+1} + \frac{1}{s+2}$

---

#### Completing the Square

**For quadratic in denominator:** $s^2 + bs + c$

$$
s^2 + bs + c = \left(s + \frac{b}{2}\right)^2 + \left(c - \frac{b^2}{4}\right)
$$

**Then use shifting theorem:**

$$
\mathcal{L}^{-1}\left\{\frac{1}{(s+a)^2+b^2}\right\} = \frac{e^{-at}\sin bt}{b}
$$

---

### 5. Solving ODEs with Laplace Transform

**Standard Steps:**

1. Take Laplace transform of entire equation
2. Use derivative formulas with initial conditions
3. Solve algebraically for $Y(s) = \mathcal{L}\{y(t)\}$
4. Decompose $Y(s)$ (partial fractions if needed)
5. Take inverse Laplace transform to get $y(t)$

**Example Template:**

For: $y'' + ay' + by = f(t)$, $y(0) = y_0$, $y'(0) = v_0$

$$
[s^2Y(s) - sy_0 - v_0] + a[sY(s) - y_0] + bY(s) = F(s)
$$

$$
Y(s)[s^2 + as + b] = F(s) + sy_0 + v_0 + ay_0
$$

$$
Y(s) = \frac{F(s) + sy_0 + v_0 + ay_0}{s^2 + as + b}
$$

---

### 6. Partial Differential Equations

#### Classification of Second-Order PDEs

**Standard Form:**
$$
Au_{xx} + Bu_{xy} + Cu_{yy} + \text{lower order terms} = 0
$$

**Discriminant:**
$$
\Delta = B^2 - 4AC
$$

**Classification:**

| $\Delta$ | Type | Example |
|----------|------|---------|
| $> 0$ | **Hyperbolic** | Wave equation |
| $= 0$ | **Parabolic** | Heat equation |
| $< 0$ | **Elliptic** | Laplace equation |

**Memory Aid:**
- **H**yperbolic: Discriminant is **H**igh
- **P**arabolic: Discriminant is **P**erfect zero
- **E**lliptic: Discriminant **E**xtremely negative

---

#### Important PDEs - Standard Forms

**1. One-Dimensional Wave Equation (Hyperbolic)**
$$
\frac{\partial^2 u}{\partial t^2} = c^2\frac{\partial^2 u}{\partial x^2}
$$

- Physical meaning: Vibrating string, sound waves
- $c$ = wave velocity
- Solution: $u(x,t) = f(x-ct) + g(x+ct)$ (D'Alembert)

**2. One-Dimensional Heat Equation (Parabolic)**
$$
\frac{\partial u}{\partial t} = \alpha^2\frac{\partial^2 u}{\partial x^2}
$$

- Physical meaning: Heat conduction, diffusion
- $\alpha^2$ = thermal diffusivity
- First derivative in time, second in space

**3. Two-Dimensional Laplace Equation (Elliptic)**
$$
\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0 \quad \text{or} \quad \nabla^2 u = 0
$$

- Physical meaning: Steady-state temperature, electrostatics
- No time derivative (steady state)

**Quick Recognition:**

| Equation | Time Derivative | Space Derivative | Type |
|----------|-----------------|------------------|------|
| Wave | $\frac{\partial^2 u}{\partial t^2}$ | $\frac{\partial^2 u}{\partial x^2}$ | Hyperbolic |
| Heat | $\frac{\partial u}{\partial t}$ | $\frac{\partial^2 u}{\partial x^2}$ | Parabolic |
| Laplace | None | $\nabla^2 u$ | Elliptic |

---

#### Method of Separation of Variables

**For PDEs of form:** $u(x,t)$ or $u(x,y)$

**Steps:**

1. **Assume product form:**
   - $u(x,t) = X(x)T(t)$ for time-dependent
   - $u(x,y) = X(x)Y(y)$ for spatial

2. **Substitute into PDE**

3. **Separate variables:**
   $$
   \frac{\text{function of } x \text{ only}}{\text{function of } x} = \frac{\text{function of } t \text{ only}}{\text{function of } t} = \text{constant}
   $$

4. **Get two ODEs** (one for each variable)

5. **Solve each ODE** with boundary conditions

6. **Combine solutions** (often as series)

**Example: Heat Equation**

$$
\frac{\partial u}{\partial t} = \alpha^2\frac{\partial^2 u}{\partial x^2}
$$

Assume $u = X(x)T(t)$:

$$
XT' = \alpha^2 X''T
$$

$$
\frac{T'}{\alpha^2 T} = \frac{X''}{X} = -\lambda \quad \text{(separation constant)}
$$

Two ODEs:
$$
X'' + \lambda X = 0, \quad T' + \lambda\alpha^2 T = 0
$$

---

## ⚡ Quick Solution Strategies

### Strategy 1: First-Order ODE Recognition

**See this → Think this:**

| Form | Type | Method |
|------|------|--------|
| $\frac{dy}{dx} = f(x)g(y)$ | Separable | Separate and integrate |
| $\frac{dy}{dx} + Py = Q$ | Linear | Integrating factor |
| $\frac{dy}{dx} = f(y/x)$ | Homogeneous | Substitute $v = y/x$ |
| $Mdx + Ndy = 0$ | Exact (if $M_y = N_x$) | Find $F: F_x = M, F_y = N$ |
| $\frac{dy}{dx} + Py = Qy^n$ | Bernoulli | Substitute $v = y^{1-n}$ |

---

### Strategy 2: Characteristic Equation Quick Solve

**For:** $ay'' + by' + cy = 0$

**Step 1:** Write $am^2 + bm + c = 0$

**Step 2:** Check discriminant $\Delta = b^2 - 4ac$

**Step 3:** Apply formula:

| $\Delta$ | Solution |
|----------|----------|
| $> 0$ | $y = C_1e^{m_1x} + C_2e^{m_2x}$ |
| $= 0$ | $y = (C_1 + C_2x)e^{-b/2a \cdot x}$ |
| $< 0$ | $y = e^{\alpha x}(C_1\cos\beta x + C_2\sin\beta x)$ where $\alpha = -b/2a$, $\beta = \sqrt{-\Delta}/2a$ |

---

### Strategy 3: Laplace Transform Shortcuts

**Derivative shortcuts:**
$$
\begin{aligned}
y' &\to sY - y(0) \\
y'' &\to s^2Y - sy(0) - y'(0) \\
y''' &\to s^3Y - s^2y(0) - sy'(0) - y''(0)
\end{aligned}
$$

**Pattern:** Each derivative adds one power of $s$ and subtracts initial condition terms

**Exponential shifting:**
- See $e^{at}$ → Replace $s$ with $(s-a)$ in transform
- $\mathcal{L}\{e^{3t}t^2\} = \frac{2!}{(s-3)^3}$

---

### Strategy 4: Partial Fractions Fast Track

**For simple factors:**

$$
\frac{P(s)}{(s-a)(s-b)} = \frac{A}{s-a} + \frac{B}{s-b}
$$

**Cover-up rule:**
- $A$: Cover $(s-a)$, substitute $s = a$ in rest
- $B$: Cover $(s-b)$, substitute $s = b$ in rest

**Example:**
$$
\frac{5s-1}{(s-2)(s+3)}
$$

$A$ (at $s=2$): $\frac{5(2)-1}{2+3} = \frac{9}{5}$

$B$ (at $s=-3$): $\frac{5(-3)-1}{-3-2} = \frac{-16}{-5} = \frac{16}{5}$

---

## 💡 Problem-Solving Tips

### Tip 1: Always Check for Simpler Method

**Before using complex techniques:**
- Can you separate variables? (Fastest!)
- Is it in standard linear form? (Use IF directly)
- Does it factor easily? (Quick solve)

### Tip 2: Initial Conditions Plug-in

**After finding general solution:**
1. Substitute $x = 0$ (or given point) to find $C_1$
2. If second-order, differentiate and substitute to find $C_2$
3. Always verify your answer satisfies IC!

### Tip 3: Characteristic Equation Patterns

**Common patterns:**

| Equation | Char. Eq. | Roots | Solution |
|----------|-----------|-------|----------|
| $y'' + y = 0$ | $m^2+1=0$ | $\pm i$ | $C_1\cos x + C_2\sin x$ |
| $y'' - y = 0$ | $m^2-1=0$ | $\pm 1$ | $C_1e^x + C_2e^{-x}$ |
| $y'' + 4y = 0$ | $m^2+4=0$ | $\pm 2i$ | $C_1\cos 2x + C_2\sin 2x$ |
| $y'' - 4y = 0$ | $m^2-4=0$ | $\pm 2$ | $C_1e^{2x} + C_2e^{-2x}$ |

### Tip 4: Laplace Transform Exam Strategy

**Memorize these 5:**
1. $\mathcal{L}\{t^n\} = \frac{n!}{s^{n+1}}$
2. $\mathcal{L}\{e^{at}\} = \frac{1}{s-a}$
3. $\mathcal{L}\{\sin at\} = \frac{a}{s^2+a^2}$
4. $\mathcal{L}\{\cos at\} = \frac{s}{s^2+a^2}$
5. $\mathcal{L}\{y''\} = s^2Y - sy(0) - y'(0)$

**With these + shifting theorem, you can solve 90% of questions!**

### Tip 5: PDE Classification Instant Recall

**Just remember the discriminant:**
- Wave: $B^2 - 4AC > 0$ (most common: $B=0, A=1, C=-c^2$ → positive)
- Heat: $B^2 - 4AC = 0$ (usually $A=0$)
- Laplace: $B^2 - 4AC < 0$ (usually $B=0, A=C=1$ → negative)

---

## ⚠️ Common Mistakes to Avoid

### ❌ Mistake 1: Forgetting Absolute Value
**Wrong:** $\int \frac{dy}{y} = \ln y + C$  
**Correct:** $\int \frac{dy}{y} = \ln|y| + C$

### ❌ Mistake 2: Integrating Factor Error
**Wrong:** For $\frac{dy}{dx} + 2xy = x$, using $\mu = e^{2x}$  
**Correct:** $\mu = e^{\int 2x dx} = e^{x^2}$ (Don't forget to integrate $P$!)

### ❌ Mistake 3: Characteristic Equation Roots
**Wrong:** $m^2 + 4 = 0 \implies m = \pm 4$  
**Correct:** $m^2 = -4 \implies m = \pm 2i$ (Complex roots!)

### ❌ Mistake 4: Forgetting Resonance Condition
**Wrong:** For $y'' + 4y = \cos 2x$, trying $y_p = A\cos 2x + B\sin 2x$ directly  
**Correct:** This matches $y_c$! Use $y_p = x(A\cos 2x + B\sin 2x)$

### ❌ Mistake 5: Initial Conditions in Laplace
**Wrong:** $\mathcal{L}\{y''\} = s^2Y(s)$  
**Correct:** $\mathcal{L}\{y''\} = s^2Y(s) - sy(0) - y'(0)$ (Don't forget IC terms!)

### ❌ Mistake 6: Partial Fractions Sign Errors
**Wrong:** $\frac{1}{(s-2)(s+3)} = \frac{A}{s-2} + \frac{B}{s-3}$  
**Correct:** $\frac{1}{(s-2)(s+3)} = \frac{A}{s-2} + \frac{B}{s+3}$ (Keep the signs!)

### ❌ Mistake 7: PDE Classification
**Wrong:** Calculating $B^2 - AC$ instead of $B^2 - 4AC$  
**Correct:** Always use $\Delta = B^2 - 4AC$ (Don't forget the 4!)

---

## 📊 Formula Priority List

### ⭐⭐⭐ Must Know (Exam Essential)

1. **Integrating factor:** $\mu = e^{\int P dx}$
2. **Characteristic equation solutions** (all three cases)
3. **Laplace of derivatives:** $\mathcal{L}\{f''\} = s^2F - sf(0) - f'(0)$
4. **Basic Laplace transforms:** $e^{at}$, $\sin at$, $\cos at$, $t^n$
5. **Partial fractions** decomposition
6. **PDE classification:** $B^2 - 4AC$

### ⭐⭐ Very Important

1. Exact equation condition: $M_y = N_x$
2. First shifting theorem: $\mathcal{L}\{e^{at}f(t)\} = F(s-a)$
3. Inverse Laplace of common forms
4. Method of undetermined coefficients (trial solutions)
5. Standard PDE forms (wave, heat, Laplace)

### ⭐ Good to Know

1. Homogeneous equation substitution
2. Bernoulli equation substitution
3. Variation of parameters
4. Convolution theorem
5. Separation of variables for PDEs

---

## 🕐 Time Management

| Question Type | Target Time | Strategy |
|---------------|-------------|----------|
| Variable Separable | 30-60 sec | Direct integration |
| Linear First-Order | 1-2 min | IF formula |
| Characteristic Equation | 1-2 min | Quick discriminant check |
| Particular Integral | 2-3 min | Trial solution, check resonance |
| Direct Laplace Transform | 1 min | Use table |
| Laplace Solution of ODE | 3-4 min | Transform, algebra, inverse |
| Inverse Laplace | 2-3 min | Partial fractions |
| PDE Classification | 30-60 sec | Calculate discriminant |
| Exact Equation | 2-3 min | Check condition, integrate |

---

## 🎓 Last-Minute Revision Checklist

**10 minutes before exam:**

✓ Integrating factor: $\mu = e^{\int P dx}$  
✓ Characteristic equation root cases (3 types)  
✓ $\mathcal{L}\{t^n\} = \frac{n!}{s^{n+1}}$, $\mathcal{L}\{e^{at}\} = \frac{1}{s-a}$  
✓ $\mathcal{L}\{\sin at\} = \frac{a}{s^2+a^2}$, $\mathcal{L}\{\cos at\} = \frac{s}{s^2+a^2}$  
✓ $\mathcal{L}\{f''\} = s^2F - sf(0) - f'(0)$  
✓ Partial fractions: cover-up method  
✓ PDE: $B^2 - 4AC$ for classification  
✓ Wave: $u_{tt} = c^2u_{xx}$, Heat: $u_t = \alpha^2u_{xx}$, Laplace: $u_{xx} + u_{yy} = 0$  
✓ Resonance: multiply by $x$ if $y_p$ term matches $y_c$  
✓ Exact: check $M_y = N_x$ first

---

## 🔑 Quick Reference Table

### ODE Solution Flowchart

```
First-Order ODE
    │
    ├── Can separate variables? → Separate & integrate
    │
    ├── Linear form (dy/dx + Py = Q)? → Use integrating factor
    │
    ├── Homogeneous (dy/dx = f(y/x))? → Substitute v = y/x
    │
    ├── Exact (M_y = N_x)? → Find F: F_x=M, F_y=N
    │
    └── Bernoulli (dy/dx + Py = Qy^n)? → Substitute v = y^(1-n)

Second-Order ODE
    │
    ├── Find y_c: Characteristic equation
    │
    └── Find y_p: Undetermined coefficients or Variation of parameters
```

---

## 🎯 Exam Day Strategy

### DO:
- ✓ Identify ODE type before solving
- ✓ Check for simplest method first
- ✓ Verify initial conditions after solving
- ✓ Use Laplace for ODEs with ICs given
- ✓ Check resonance condition for particular integral
- ✓ Always factor denominators completely for partial fractions

### DON'T:
- ✗ Skip exactness check for exact equations
- ✗ Forget absolute value in logarithms
- ✗ Miss the factor of 4 in PDE discriminant
- ✗ Apply complex formulas when simple ones work
- ✗ Forget to multiply by $x$ in resonance cases
- ✗ Rush through characteristic equation discriminant

---

## 🔗 Related Topics

- [Calculus](../Calculus/CheatSheet.md)
- [Linear Algebra](../Linear_Algebra/CheatSheet.md)
- [Vector Calculus](../Vector_Calculus/CheatSheet.md)
- [Numerical Methods](../Numerical_Methods/CheatSheet.md)

---

**Last Updated:** November 2025  
**Version:** 1.0

---

*For detailed solutions, refer to [Solutions.md](./Solutions.md)*  
*For concepts and theory, refer to [README.md](./README.md)*
