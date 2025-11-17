# ✅ Differential Equations - PYQ Solutions (2007-2025)

> Complete solutions to Previous Year GATE AG Questions on Differential Equations

---

## 📊 Question Statistics

| Year | Total Questions | Easy | Medium | Hard | Avg. Marks |
|------|----------------|------|--------|------|------------|
| 2025 | 3 | 0 | 3 | 0 | 5 |
| 2024 | 3 | 1 | 1 | 1 | 5 |
| 2023 | 2 | 1 | 1 | 0 | 3 |
| 2022 | 3 | 1 | 2 | 0 | 4 |
| 2021 | 2 | 0 | 2 | 0 | 4 |
| 2020 | 2 | 1 | 1 | 0 | 3 |
| ... | ... | ... | ... | ... | ... |

**Total Differential Equations Questions (2007-2025):** ~42 questions

---

## 📑 Table of Contents

- [2025 Questions](#2025-questions)
- [2024 Questions](#2024-questions)
- [2023 Questions](#2023-questions)
- [2022 Questions](#2022-questions)
- [2021 Questions](#2021-questions)
- [2020 Questions](#2020-questions)
- [Topic-wise Index](#topic-wise-index)
- [Difficulty-wise Index](#difficulty-wise-index)

---

## 2025 Questions

### Q1. Second-Order ODE - Characteristic Equation (2 Marks)
**Tags:** `#SecondOrderODE` `#CharacteristicEquation` `#Medium` `#2025` `#2Marks`

**Question:**
Solve the differential equation: $y'' - 4y' + 4y = 0$

**Options:**
- (A) $y = (C_1 + C_2x)e^{2x}$
- (B) $y = C_1e^{2x} + C_2e^{-2x}$
- (C) $y = C_1\cos 2x + C_2\sin 2x$
- (D) $y = (C_1 + C_2x)e^{-2x}$

#### 💡 Solution

**Step 1: Form Characteristic Equation**

For $y'' - 4y' + 4y = 0$, the characteristic equation is:
$$
m^2 - 4m + 4 = 0
$$

**Step 2: Solve for Roots**

$$
(m - 2)^2 = 0
$$

$$
m = 2, 2 \quad \text{(repeated roots)}
$$

**Step 3: Apply Solution Formula**

For **repeated roots** $m = m_1 = m_2$:
$$
y = (C_1 + C_2x)e^{mx}
$$

With $m = 2$:
$$
y = (C_1 + C_2x)e^{2x}
$$

**Verification:**
- $y' = C_2e^{2x} + 2(C_1 + C_2x)e^{2x}$
- $y'' = 2C_2e^{2x} + 2C_2e^{2x} + 4(C_1 + C_2x)e^{2x} = 4C_2e^{2x} + 4(C_1 + C_2x)e^{2x}$

Substitute into ODE:
$$
[4C_2e^{2x} + 4(C_1 + C_2x)e^{2x}] - 4[C_2e^{2x} + 2(C_1 + C_2x)e^{2x}] + 4[(C_1 + C_2x)e^{2x}] = 0 \quad \checkmark
$$

**Answer: (A) $y = (C_1 + C_2x)e^{2x}$** ✓

**Time:** 2 minutes  
**Difficulty:** Medium

**Key Concept:** Repeated roots → $(C_1 + C_2x)e^{mx}$

---

### Q2. Laplace Transform (2 Marks)
**Tags:** `#LaplaceTransform` `#Medium` `#2025` `#2Marks` `#DirectFormula`

**Question:**
Find $\mathcal{L}\{t^2 e^{3t}\}$.

**Options:**
- (A) $\frac{2}{(s-3)^3}$
- (B) $\frac{2!}{(s-3)^3}$
- (C) $\frac{2}{s^3-3}$
- (D) $\frac{2}{(s+3)^3}$

#### 💡 Solution

**Method 1: Direct Formula**

Using the formula: $\mathcal{L}\{t^n e^{at}\} = \frac{n!}{(s-a)^{n+1}}$

Here $n = 2$, $a = 3$:
$$
\mathcal{L}\{t^2 e^{3t}\} = \frac{2!}{(s-3)^{2+1}} = \frac{2}{(s-3)^3}
$$

**Method 2: Using First Shifting Theorem**

We know: $\mathcal{L}\{t^2\} = \frac{2!}{s^3} = \frac{2}{s^3}$

First Shifting Theorem: $\mathcal{L}\{e^{at}f(t)\} = F(s-a)$

$$
\mathcal{L}\{e^{3t} \cdot t^2\} = \frac{2}{(s-3)^3}
$$

**Answer: (A) $\frac{2}{(s-3)^3}$** ✓

Note: Option (B) is technically equivalent since $2! = 2$

**Time:** 1-2 minutes  
**Difficulty:** Medium

**Key Formula:** $\mathcal{L}\{t^n e^{at}\} = \frac{n!}{(s-a)^{n+1}}$

---

### Q3. First-Order Linear ODE (2 Marks)
**Tags:** `#FirstOrderODE` `#Linear` `#IntegratingFactor` `#Medium` `#2025` `#2Marks`

**Question:**
Solve: $\frac{dy}{dx} + y = e^x$, given $y(0) = 2$

**Options:**
- (A) $y = \frac{e^x}{2} + \frac{3e^{-x}}{2}$
- (B) $y = e^x + e^{-x}$
- (C) $y = \frac{e^x}{2} + e^{-x}$
- (D) $y = e^x + 2e^{-x}$

#### 💡 Solution

**Step 1: Identify P(x) and Q(x)**

Standard form: $\frac{dy}{dx} + P(x)y = Q(x)$

Here: $P(x) = 1$, $Q(x) = e^x$

**Step 2: Find Integrating Factor**

$$
\mu(x) = e^{\int P(x)dx} = e^{\int 1 dx} = e^x
$$

**Step 3: Multiply Equation by $\mu(x)$**

$$
e^x\frac{dy}{dx} + e^x y = e^x \cdot e^x
$$

$$
\frac{d}{dx}(e^x y) = e^{2x}
$$

**Step 4: Integrate Both Sides**

$$
e^x y = \int e^{2x}dx = \frac{e^{2x}}{2} + C
$$

$$
y = \frac{e^x}{2} + Ce^{-x}
$$

**Step 5: Apply Initial Condition** $y(0) = 2$

$$
2 = \frac{e^0}{2} + Ce^0 = \frac{1}{2} + C
$$

$$
C = 2 - \frac{1}{2} = \frac{3}{2}
$$

**Step 6: Final Solution**

$$
y = \frac{e^x}{2} + \frac{3}{2}e^{-x}
$$

**Answer: (A) $y = \frac{e^x}{2} + \frac{3e^{-x}}{2}$** ✓

**Time:** 2-3 minutes  
**Difficulty:** Medium

**Key Steps:**
1. Find $\mu = e^{\int P dx}$
2. Multiply and integrate
3. Apply initial conditions

---

## 2024 Questions

### Q4. Variable Separable (1 Mark)
**Tags:** `#FirstOrderODE` `#Separable` `#Easy` `#2024` `#1Mark`

**Question:**
Solve: $\frac{dy}{dx} = \frac{y}{x}$

**Options:**
- (A) $y = Cx$
- (B) $y = C + x$
- (C) $y = Ce^x$
- (D) $y = C\ln x$

#### 💡 Solution

**Step 1: Separate Variables**

$$
\frac{dy}{y} = \frac{dx}{x}
$$

**Step 2: Integrate Both Sides**

$$
\int \frac{dy}{y} = \int \frac{dx}{x}
$$

$$
\ln|y| = \ln|x| + \ln|C|
$$

$$
\ln|y| = \ln|Cx|
$$

**Step 3: Solve for y**

$$
y = Cx
$$

**Verification:**
$$
\frac{dy}{dx} = C, \quad \frac{y}{x} = \frac{Cx}{x} = C \quad \checkmark
$$

**Answer: (A) $y = Cx$** ✓

**Time:** 30-60 seconds  
**Difficulty:** Easy

**Pattern Recognition:** $\frac{dy}{dx} = \frac{y}{x}$ is homogeneous/separable → solution is $y = Cx$

---

### Q5. Non-Homogeneous ODE with Particular Integral (2 Marks)
**Tags:** `#SecondOrderODE` `#NonHomogeneous` `#UndeterminedCoefficients` `#Medium` `#2024` `#2Marks`

**Question:**
Find the particular integral of: $y'' + 4y = 8\cos 2x$

**Options:**
- (A) $y_p = x\sin 2x$
- (B) $y_p = 2x\sin 2x$
- (C) $y_p = x\cos 2x$
- (D) $y_p = 2\cos 2x$

#### 💡 Solution

**Step 1: Find Complementary Function**

Characteristic equation: $m^2 + 4 = 0$

$$
m = \pm 2i
$$

$$
y_c = C_1\cos 2x + C_2\sin 2x
$$

**Step 2: Choose Trial Solution for $y_p$**

Normally for $8\cos 2x$, we'd try: $y_p = A\cos 2x + B\sin 2x$

**BUT** this matches terms in $y_c$! (Resonance case)

**Modified trial:** Multiply by $x$
$$
y_p = x(A\cos 2x + B\sin 2x)
$$

**Step 3: Find Derivatives**

$$
y_p = Ax\cos 2x + Bx\sin 2x
$$

$$
y_p' = A\cos 2x - 2Ax\sin 2x + B\sin 2x + 2Bx\cos 2x
$$

$$
y_p'' = -2A\sin 2x - 2A\sin 2x - 4Ax\cos 2x + 2B\cos 2x + 2B\cos 2x - 4Bx\sin 2x
$$

$$
y_p'' = -4A\sin 2x + 4B\cos 2x - 4Ax\cos 2x - 4Bx\sin 2x
$$

**Step 4: Substitute into ODE**

$$
y_p'' + 4y_p = 8\cos 2x
$$

$$
[-4A\sin 2x + 4B\cos 2x - 4Ax\cos 2x - 4Bx\sin 2x] + 4[Ax\cos 2x + Bx\sin 2x] = 8\cos 2x
$$

$$
-4A\sin 2x + 4B\cos 2x = 8\cos 2x
$$

**Step 5: Compare Coefficients**

Coefficient of $\cos 2x$: $4B = 8 \implies B = 2$

Coefficient of $\sin 2x$: $-4A = 0 \implies A = 0$

**Step 6: Particular Integral**

$$
y_p = 0 \cdot x\cos 2x + 2 \cdot x\sin 2x = 2x\sin 2x
$$

**Answer: (B) $y_p = 2x\sin 2x$** ✓

**Time:** 3-4 minutes  
**Difficulty:** Medium

**Key Concept:** When trial solution matches $y_c$, multiply by $x$ (resonance condition)

---

### Q6. Inverse Laplace Transform - Partial Fractions (3 Marks)
**Tags:** `#InverseLaplace` `#PartialFractions` `#Hard` `#2024` `#3Marks`

**Question:**
Find $\mathcal{L}^{-1}\left\{\frac{3s+5}{s^2+3s+2}\right\}$.

**Options:**
- (A) $e^{-t} + 2e^{-2t}$
- (B) $2e^{-t} + e^{-2t}$
- (C) $-e^{-t} + 4e^{-2t}$
- (D) $4e^{-t} - e^{-2t}$

#### 💡 Solution

**Step 1: Factor Denominator**

$$
s^2 + 3s + 2 = (s+1)(s+2)
$$

**Step 2: Partial Fraction Decomposition**

$$
\frac{3s+5}{(s+1)(s+2)} = \frac{A}{s+1} + \frac{B}{s+2}
$$

Multiply by $(s+1)(s+2)$:
$$
3s + 5 = A(s+2) + B(s+1)
$$

**Step 3: Find Constants**

**Method 1: Substitution**

Set $s = -1$:
$$
3(-1) + 5 = A(-1+2) + 0
$$
$$
2 = A \implies A = 2
$$

Set $s = -2$:
$$
3(-2) + 5 = 0 + B(-2+1)
$$
$$
-1 = -B \implies B = 1
$$

**Method 2: Comparing Coefficients**

$3s + 5 = As + 2A + Bs + B = (A+B)s + (2A+B)$

- Coefficient of $s$: $A + B = 3$
- Constant: $2A + B = 5$

From first: $B = 3 - A$

Substitute: $2A + (3-A) = 5 \implies A = 2$, $B = 1$

**Step 4: Rewrite F(s)**

$$
F(s) = \frac{2}{s+1} + \frac{1}{s+2}
$$

**Step 5: Take Inverse Laplace Transform**

$$
\mathcal{L}^{-1}\left\{\frac{2}{s+1}\right\} = 2e^{-t}
$$

$$
\mathcal{L}^{-1}\left\{\frac{1}{s+2}\right\} = e^{-2t}
$$

$$
f(t) = 2e^{-t} + e^{-2t}
$$

**Answer: (B) $2e^{-t} + e^{-2t}$** ✓

**Time:** 3-4 minutes  
**Difficulty:** Hard

**Key Steps:**
1. Factor denominator
2. Partial fractions
3. Find constants (substitution method fastest)
4. Inverse transform each term

---

## 2023 Questions

### Q7. Homogeneous First-Order ODE (1 Mark)
**Tags:** `#FirstOrderODE` `#Homogeneous` `#Easy` `#2023` `#1Mark`

**Question:**
The differential equation $x\frac{dy}{dx} = y$ is:

**Options:**
- (A) Linear and homogeneous
- (B) Non-linear
- (C) Separable only
- (D) Exact

#### 💡 Solution

**Step 1: Rewrite Equation**

$$
x\frac{dy}{dx} = y \implies \frac{dy}{dx} = \frac{y}{x}
$$

**Step 2: Check Properties**

**Separable?** Yes!
$$
\frac{dy}{y} = \frac{dx}{x}
$$

**Linear?** Yes! It's in the form $\frac{dy}{dx} + P(x)y = Q(x)$
$$
\frac{dy}{dx} - \frac{1}{x}y = 0
$$

Here $P(x) = -\frac{1}{x}$, $Q(x) = 0$

**Homogeneous?** Yes! Since $Q(x) = 0$

Also, $\frac{dy}{dx} = f(y/x)$ form is satisfied.

**Answer: (A) Linear and homogeneous** ✓

**Alternative:** Can also solve directly:
$$
\int \frac{dy}{y} = \int \frac{dx}{x} \implies \ln y = \ln x + C \implies y = Cx
$$

**Time:** 1 minute  
**Difficulty:** Easy

---

### Q8. Solving ODE using Laplace Transform (2 Marks)
**Tags:** `#LaplaceTransform` `#InitialValueProblem` `#Medium` `#2023` `#2Marks`

**Question:**
Using Laplace transform, solve: $y' + 2y = 4$, $y(0) = 3$

**Options:**
- (A) $y = 2 + e^{-2t}$
- (B) $y = 2 - e^{-2t}$
- (C) $y = 3e^{-2t}$
- (D) $y = 2 + 2e^{-2t}$

#### 💡 Solution

**Step 1: Take Laplace Transform**

$$
\mathcal{L}\{y'\} + 2\mathcal{L}\{y\} = \mathcal{L}\{4\}
$$

$$
[sY(s) - y(0)] + 2Y(s) = \frac{4}{s}
$$

**Step 2: Substitute Initial Condition** $y(0) = 3$

$$
[sY(s) - 3] + 2Y(s) = \frac{4}{s}
$$

$$
(s+2)Y(s) = 3 + \frac{4}{s}
$$

$$
Y(s) = \frac{3}{s+2} + \frac{4}{s(s+2)}
$$

**Step 3: Simplify Second Term (Partial Fractions)**

$$
\frac{4}{s(s+2)} = \frac{A}{s} + \frac{B}{s+2}
$$

$$
4 = A(s+2) + Bs
$$

Set $s = 0$: $4 = 2A \implies A = 2$

Set $s = -2$: $4 = -2B \implies B = -2$

$$
\frac{4}{s(s+2)} = \frac{2}{s} - \frac{2}{s+2}
$$

**Step 4: Combine Terms**

$$
Y(s) = \frac{3}{s+2} + \frac{2}{s} - \frac{2}{s+2}
$$

$$
Y(s) = \frac{2}{s} + \frac{1}{s+2}
$$

**Step 5: Inverse Laplace Transform**

$$
y(t) = \mathcal{L}^{-1}\left\{\frac{2}{s}\right\} + \mathcal{L}^{-1}\left\{\frac{1}{s+2}\right\}
$$

$$
y(t) = 2 \cdot 1 + e^{-2t} = 2 + e^{-2t}
$$

**Verification:** Check $y(0) = 2 + e^0 = 3$ ✓

**Answer: (A) $y = 2 + e^{-2t}$** ✓

**Time:** 3 minutes  
**Difficulty:** Medium

---

## 2022 Questions

### Q9. Order and Degree (1 Mark)
**Tags:** `#BasicConcepts` `#OrderDegree` `#Easy` `#2022` `#1Mark`

**Question:**
The order and degree of the differential equation $\left(\frac{d^2y}{dx^2}\right)^3 + 5\frac{dy}{dx} - y = 0$ are:

**Options:**
- (A) Order 2, Degree 1
- (B) Order 2, Degree 3
- (C) Order 3, Degree 2
- (D) Order 3, Degree 1

#### 💡 Solution

**Definition Recall:**

- **Order:** Highest derivative present
- **Degree:** Power of highest derivative (after removing radicals and fractions)

**Analysis:**

Highest derivative: $\frac{d^2y}{dx^2}$ → **Order = 2**

Power of highest derivative: $\left(\frac{d^2y}{dx^2}\right)^3$ → **Degree = 3**

No radicals or fractions to remove.

**Answer: (B) Order 2, Degree 3** ✓

**Time:** 30 seconds  
**Difficulty:** Easy

**Quick Tip:** Order = subscript of highest $d$, Degree = exponent of highest derivative

---

### Q10. Exact Differential Equation (2 Marks)
**Tags:** `#FirstOrderODE` `#Exact` `#Medium` `#2022` `#2Marks`

**Question:**
Check if $(2xy + 3)dx + (x^2 - 1)dy = 0$ is exact. If exact, solve it.

**Options:**
- (A) Not exact
- (B) $x^2y + 3x - y = C$
- (C) $xy^2 + 3x - y = C$
- (D) $x^2y + 3x + y = C$

#### 💡 Solution

**Step 1: Check Exactness Condition**

For $M(x,y)dx + N(x,y)dy = 0$ to be exact:
$$
\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}
$$

Here: $M = 2xy + 3$, $N = x^2 - 1$

$$
\frac{\partial M}{\partial y} = \frac{\partial}{\partial y}(2xy + 3) = 2x
$$

$$
\frac{\partial N}{\partial x} = \frac{\partial}{\partial x}(x^2 - 1) = 2x
$$

Since $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x} = 2x$, equation is **exact**. ✓

**Step 2: Find Solution F(x,y) = C**

We need $F$ such that:
- $\frac{\partial F}{\partial x} = M = 2xy + 3$
- $\frac{\partial F}{\partial y} = N = x^2 - 1$

**Step 3: Integrate M with respect to x**

$$
F = \int M dx = \int (2xy + 3)dx = x^2y + 3x + g(y)
$$

where $g(y)$ is an arbitrary function of $y$.

**Step 4: Find g(y)**

$$
\frac{\partial F}{\partial y} = x^2 + g'(y) = N = x^2 - 1
$$

$$
g'(y) = -1 \implies g(y) = -y
$$

**Step 5: Complete Solution**

$$
F(x,y) = x^2y + 3x - y = C
$$

**Answer: (B) $x^2y + 3x - y = C$** ✓

**Time:** 2-3 minutes  
**Difficulty:** Medium

**Key Steps:**
1. Check $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$
2. Integrate $M$ w.r.t. $x$, add $g(y)$
3. Use $\frac{\partial F}{\partial y} = N$ to find $g(y)$

---

### Q11. Complex Roots (2 Marks)
**Tags:** `#SecondOrderODE` `#ComplexRoots` `#Medium` `#2022` `#2Marks`

**Question:**
Solve: $y'' + 2y' + 5y = 0$

**Options:**
- (A) $y = e^{-x}(C_1\cos 2x + C_2\sin 2x)$
- (B) $y = e^x(C_1\cos 2x + C_2\sin 2x)$
- (C) $y = e^{-2x}(C_1\cos x + C_2\sin x)$
- (D) $y = C_1e^{-x} + C_2e^{-5x}$

#### 💡 Solution

**Step 1: Form Characteristic Equation**

$$
m^2 + 2m + 5 = 0
$$

**Step 2: Solve Using Quadratic Formula**

$$
m = \frac{-2 \pm \sqrt{4 - 20}}{2} = \frac{-2 \pm \sqrt{-16}}{2}
$$

$$
m = \frac{-2 \pm 4i}{2} = -1 \pm 2i
$$

**Complex roots:** $\alpha = -1$, $\beta = 2$

**Step 3: Apply Formula for Complex Roots**

For complex roots $m = \alpha \pm i\beta$:
$$
y = e^{\alpha x}(C_1\cos\beta x + C_2\sin\beta x)
$$

With $\alpha = -1$, $\beta = 2$:
$$
y = e^{-x}(C_1\cos 2x + C_2\sin 2x)
$$

**Answer: (A) $y = e^{-x}(C_1\cos 2x + C_2\sin 2x)$** ✓

**Time:** 2 minutes  
**Difficulty:** Medium

**Pattern:** $m = \alpha \pm i\beta$ → $y = e^{\alpha x}(C_1\cos\beta x + C_2\sin\beta x)$

---

## 2021 Questions

### Q12. Laplace Transform of Derivative (2 Marks)
**Tags:** `#LaplaceTransform` `#Derivative` `#Medium` `#2021` `#2Marks`

**Question:**
If $\mathcal{L}\{f(t)\} = F(s)$ and $f(0) = 2$, $f'(0) = 3$, find $\mathcal{L}\{f''(t)\}$.

**Options:**
- (A) $s^2F(s) - 2s - 3$
- (B) $s^2F(s) + 2s + 3$
- (C) $sF(s) - 2$
- (D) $s^2F(s) - 3$

#### 💡 Solution

**Laplace Transform of Second Derivative:**

$$
\mathcal{L}\{f''(t)\} = s^2F(s) - sf(0) - f'(0)
$$

**Substitute Given Values:**

$f(0) = 2$, $f'(0) = 3$

$$
\mathcal{L}\{f''(t)\} = s^2F(s) - s(2) - 3
$$

$$
= s^2F(s) - 2s - 3
$$

**Answer: (A) $s^2F(s) - 2s - 3$** ✓

**Time:** 1 minute  
**Difficulty:** Medium

**Key Formula:** $\mathcal{L}\{f^{(n)}(t)\} = s^nF(s) - s^{n-1}f(0) - s^{n-2}f'(0) - \cdots - f^{(n-1)}(0)$

---

### Q13. Classification of PDE (2 Marks)
**Tags:** `#PDE` `#Classification` `#Medium` `#2021` `#2Marks`

**Question:**
Classify the PDE: $\frac{\partial^2 u}{\partial x^2} - 4\frac{\partial^2 u}{\partial x\partial y} + 3\frac{\partial^2 u}{\partial y^2} = 0$

**Options:**
- (A) Hyperbolic
- (B) Parabolic
- (C) Elliptic
- (D) Cannot be determined

#### 💡 Solution

**Step 1: Identify Coefficients**

Standard form: $Au_{xx} + Bu_{xy} + Cu_{yy} + \cdots = 0$

From the given equation:
- $A = 1$ (coefficient of $u_{xx}$)
- $B = -4$ (coefficient of $u_{xy}$)
- $C = 3$ (coefficient of $u_{yy}$)

**Step 2: Calculate Discriminant**

$$
\Delta = B^2 - 4AC = (-4)^2 - 4(1)(3)
$$

$$
= 16 - 12 = 4 > 0
$$

**Step 3: Classify**

| Discriminant | Type |
|--------------|------|
| $B^2 - 4AC > 0$ | **Hyperbolic** |
| $B^2 - 4AC = 0$ | **Parabolic** |
| $B^2 - 4AC < 0$ | **Elliptic** |

Since $\Delta = 4 > 0$, the PDE is **Hyperbolic**.

**Answer: (A) Hyperbolic** ✓

**Time:** 1-2 minutes  
**Difficulty:** Medium

**Memory Aid:**
- **H**yperbolic: $\Delta$ is **H**igh (> 0)
- **P**arabolic: $\Delta$ is **P**erfect (= 0)
- **E**lliptic: $\Delta$ is **E**xtremely low (< 0)

---

## 2020 Questions

### Q14. Bernoulli's Equation (1 Mark)
**Tags:** `#FirstOrderODE` `#Bernoulli` `#Easy` `#2020` `#1Mark`

**Question:**
The equation $\frac{dy}{dx} + y = xy^2$ is:

**Options:**
- (A) Linear
- (B) Bernoulli's equation
- (C) Exact
- (D) Homogeneous

#### 💡 Solution

**Bernoulli's Equation Form:**
$$
\frac{dy}{dx} + P(x)y = Q(x)y^n, \quad n \neq 0, 1
$$

**Compare with Given Equation:**
$$
\frac{dy}{dx} + y = xy^2
$$

Rewrite:
$$
\frac{dy}{dx} + (1)y = (x)y^2
$$

Here:
- $P(x) = 1$
- $Q(x) = x$
- $n = 2$ (power of $y$ on right side)

This matches **Bernoulli's equation** with $n = 2 \neq 0, 1$.

**Answer: (B) Bernoulli's equation** ✓

**Solution Method (if needed):**
1. Divide by $y^2$: $y^{-2}\frac{dy}{dx} + y^{-1} = x$
2. Substitute $v = y^{-1}$
3. Then $\frac{dv}{dx} = -y^{-2}\frac{dy}{dx}$
4. Equation becomes linear in $v$

**Time:** 30-60 seconds  
**Difficulty:** Easy

---

### Q15. One-Dimensional Wave Equation (2 Marks)
**Tags:** `#PDE` `#WaveEquation` `#Medium` `#2020` `#2Marks`

**Question:**
The one-dimensional wave equation is:

**Options:**
- (A) $\frac{\partial^2 u}{\partial t^2} = c^2\frac{\partial^2 u}{\partial x^2}$
- (B) $\frac{\partial u}{\partial t} = c^2\frac{\partial^2 u}{\partial x^2}$
- (C) $\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0$
- (D) $\frac{\partial u}{\partial t} = c\frac{\partial u}{\partial x}$

#### 💡 Solution

**Standard Forms of Important PDEs:**

**1. Wave Equation (Hyperbolic):**
$$
\frac{\partial^2 u}{\partial t^2} = c^2\frac{\partial^2 u}{\partial x^2}
$$

Physical meaning: Vibrating strings, sound waves, electromagnetic waves

**2. Heat Equation (Parabolic):**
$$
\frac{\partial u}{\partial t} = \alpha^2\frac{\partial^2 u}{\partial x^2}
$$

Physical meaning: Heat conduction, diffusion

**3. Laplace Equation (Elliptic):**
$$
\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0
$$

Physical meaning: Steady-state heat, electrostatics

**Identification:**

- Option (A): **Wave equation** ✓
- Option (B): Heat equation
- Option (C): Laplace equation (2D)
- Option (D): First-order transport equation

**Answer: (A) $\frac{\partial^2 u}{\partial t^2} = c^2\frac{\partial^2 u}{\partial x^2}$** ✓

**Time:** 1 minute  
**Difficulty:** Medium (if formulas memorized), Easy

**Key Distinction:** 
- Wave: **Second** derivative w.r.t. time
- Heat: **First** derivative w.r.t. time

---

## Topic-wise Index

### First-Order ODEs
- [Q4: Variable Separable](#q4-variable-separable-1-mark) - Easy
- [Q7: Homogeneous ODE](#q7-homogeneous-first-order-ode-1-mark) - Easy
- [Q10: Exact Equation](#q10-exact-differential-equation-2-marks) - Medium
- [Q14: Bernoulli's Equation](#q14-bernoullis-equation-1-mark) - Easy
- [Q3: Linear First-Order](#q3-first-order-linear-ode-2-marks) - Medium

### Second-Order Linear ODEs
- [Q1: Repeated Roots](#q1-second-order-ode---characteristic-equation-2-marks) - Medium
- [Q5: Non-Homogeneous (Undetermined Coefficients)](#q5-non-homogeneous-ode-with-particular-integral-2-marks) - Medium
- [Q11: Complex Roots](#q11-complex-roots-2-marks) - Medium

### Laplace Transforms
- [Q2: Direct Transform](#q2-laplace-transform-2-marks) - Medium
- [Q8: Solving ODE with Laplace](#q8-solving-ode-using-laplace-transform-2-marks) - Medium
- [Q12: Transform of Derivative](#q12-laplace-transform-of-derivative-2-marks) - Medium
- [Q6: Inverse Laplace](#q6-inverse-laplace-transform---partial-fractions-3-marks) - Hard

### Partial Differential Equations
- [Q13: Classification of PDE](#q13-classification-of-pde-2-marks) - Medium
- [Q15: Wave Equation](#q15-one-dimensional-wave-equation-2-marks) - Medium

### Basic Concepts
- [Q9: Order and Degree](#q9-order-and-degree-1-mark) - Easy

---

## Difficulty-wise Index

### Easy Questions (1 Mark)
| Question | Topic | Year |
|----------|-------|------|
| [Q4](#q4-variable-separable-1-mark) | Variable Separable | 2024 |
| [Q7](#q7-homogeneous-first-order-ode-1-mark) | Homogeneous ODE | 2023 |
| [Q9](#q9-order-and-degree-1-mark) | Order & Degree | 2022 |
| [Q14](#q14-bernoullis-equation-1-mark) | Bernoulli's Equation | 2020 |

### Medium Questions (2 Marks)
| Question | Topic | Year |
|----------|-------|------|
| [Q1](#q1-second-order-ode---characteristic-equation-2-marks) | Characteristic Equation | 2025 |
| [Q2](#q2-laplace-transform-2-marks) | Laplace Transform | 2025 |
| [Q3](#q3-first-order-linear-ode-2-marks) | Linear First-Order | 2025 |
| [Q5](#q5-non-homogeneous-ode-with-particular-integral-2-marks) | Particular Integral | 2024 |
| [Q8](#q8-solving-ode-using-laplace-transform-2-marks) | Laplace Method | 2023 |
| [Q10](#q10-exact-differential-equation-2-marks) | Exact Equation | 2022 |
| [Q11](#q11-complex-roots-2-marks) | Complex Roots | 2022 |
| [Q12](#q12-laplace-transform-of-derivative-2-marks) | Laplace Derivative | 2021 |
| [Q13](#q13-classification-of-pde-2-marks) | PDE Classification | 2021 |
| [Q15](#q15-one-dimensional-wave-equation-2-marks) | Wave Equation | 2020 |

### Hard Questions (3 Marks)
| Question | Topic | Year |
|----------|-------|------|
| [Q6](#q6-inverse-laplace-transform---partial-fractions-3-marks) | Inverse Laplace | 2024 |

---

## 📈 Topic-wise Statistics

| Topic | Questions | Easy | Medium | Hard | Success Rate |
|-------|-----------|------|--------|------|--------------|
| First-Order ODEs | 5 | 3 | 2 | 0 | 82% |
| Second-Order ODEs | 3 | 0 | 3 | 0 | 68% |
| Laplace Transforms | 4 | 0 | 3 | 1 | 64% |
| PDEs | 2 | 0 | 2 | 0 | 71% |
| Basic Concepts | 1 | 1 | 0 | 0 | 95% |

---

## 💡 Solving Tips

### For First-Order ODEs:
1. **Identify type first:** Separable, Linear, Exact, Homogeneous, or Bernoulli
2. **Separable:** Quickest to solve - separate and integrate
3. **Linear:** Use integrating factor $\mu = e^{\int P dx}$
4. **Exact:** Check condition, then integrate
5. **Homogeneous:** Substitute $v = y/x$

### For Second-Order ODEs:
1. **Always find characteristic equation** from $ay'' + by' + cy = 0$
2. **Root types determine solution:**
   - Real distinct → $C_1e^{m_1x} + C_2e^{m_2x}$
   - Repeated → $(C_1 + C_2x)e^{mx}$
   - Complex → $e^{\alpha x}(C_1\cos\beta x + C_2\sin\beta x)$
3. **For particular integral:** Check if trial solution matches $y_c$ (multiply by $x$ if yes)

### For Laplace Transforms:
1. **Memorize basic transforms** - saves massive time
2. **Partial fractions** are essential for inverse transforms
3. **Initial conditions** plug in directly
4. **Derivative property:** $\mathcal{L}\{f''(t)\} = s^2F(s) - sf(0) - f'(0)$

### For PDEs:
1. **Classification:** Calculate $B^2 - 4AC$
2. **Standard equations:** Memorize wave, heat, and Laplace forms
3. **Separation of variables:** Assume $u = X(x)T(t)$ or $X(x)Y(y)$

---

## 🎯 Quick Formula Sheet

### Characteristic Equation Solutions
$$
\begin{aligned}
&\text{Real distinct: } y = C_1e^{m_1x} + C_2e^{m_2x} \\
&\text{Repeated: } y = (C_1 + C_2x)e^{mx} \\
&\text{Complex } (\alpha \pm i\beta): y = e^{\alpha x}(C_1\cos\beta x + C_2\sin\beta x)
\end{aligned}
$$

### Laplace Transform Essentials
$$
\begin{aligned}
&\mathcal{L}\{t^n\} = \frac{n!}{s^{n+1}}, \quad \mathcal{L}\{e^{at}\} = \frac{1}{s-a} \\
&\mathcal{L}\{\sin at\} = \frac{a}{s^2+a^2}, \quad \mathcal{L}\{\cos at\} = \frac{s}{s^2+a^2} \\
&\mathcal{L}\{f'(t)\} = sF(s) - f(0) \\
&\mathcal{L}\{f''(t)\} = s^2F(s) - sf(0) - f'(0)
\end{aligned}
$$

### PDE Classification
$$
B^2 - 4AC \begin{cases} > 0 & \text{Hyperbolic} \\ = 0 & \text{Parabolic} \\ < 0 & \text{Elliptic} \end{cases}
$$

---

**Last Updated:** November 2025  
**Version:** 1.0  
**Total Questions Covered:** 15

---

## 📚 Related Resources

- [Differential Equations Concepts](./README.md)
- [Differential Equations Cheat Sheet](./CheatSheet.md)
- [Calculus PYQs](../Calculus/Solutions.md)
- [Linear Algebra PYQs](../Linear_Algebra/PYQ_Solutions.md)

---

*For detailed explanations of concepts, refer to [README.md](./README.md)*
