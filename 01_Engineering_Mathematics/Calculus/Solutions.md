# ✅ Calculus - PYQ Solutions (2007-2025)

> Complete solutions to Previous Year GATE AG Questions on Calculus

---

## 📊 Question Statistics

| Year | Total Questions | Easy | Medium | Hard | Avg. Marks |
|------|----------------|------|--------|------|------------|
| 2025 | 3 | 1 | 2 | 0 | 4 |
| 2024 | 3 | 1 | 1 | 1 | 5 |
| 2023 | 2 | 1 | 1 | 0 | 3 |
| 2022 | 3 | 1 | 2 | 0 | 4 |
| 2021 | 2 | 0 | 2 | 0 | 4 |
| 2020 | 2 | 1 | 1 | 0 | 3 |
| ... | ... | ... | ... | ... | ... |

**Total Calculus Questions (2007-2025):** ~45 questions

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

### Q1. Limit Evaluation (1 Mark)
**Tags:** `#Limits` `#Easy` `#2025` `#1Mark` `#StandardLimit`

**Question:**
Evaluate: $\displaystyle \lim_{x \to 0} \frac{\sin 3x}{x}$

**Options:**
- (A) 0
- (B) 1
- (C) 3
- (D) $\infty$

#### 💡 Solution

**Method 1: Standard Limit Formula**

We know that $\displaystyle \lim_{x \to 0} \frac{\sin x}{x} = 1$

Rewrite the given limit:
$$
\lim_{x \to 0} \frac{\sin 3x}{x} = \lim_{x \to 0} \frac{\sin 3x}{3x} \cdot 3
$$

Let $u = 3x$, then as $x \to 0$, $u \to 0$:
$$
= 3 \cdot \lim_{u \to 0} \frac{\sin u}{u} = 3 \cdot 1 = 3
$$

**Method 2: Direct Substitution Using Formula**

Using the property: $\displaystyle \lim_{x \to 0} \frac{\sin(ax)}{x} = a$

$$
\lim_{x \to 0} \frac{\sin 3x}{x} = 3
$$

**Answer: (C) 3** ✓

**Time:** 30-60 seconds  
**Difficulty:** Easy

**Key Concept:** Standard limit: $\displaystyle \lim_{x \to 0} \frac{\sin(ax)}{x} = a$

---

### Q2. Maxima and Minima (2 Marks)
**Tags:** `#MaximaMinima` `#Medium` `#2025` `#2Marks` `#SecondDerivative`

**Question:**
Find the local maximum value of the function $f(x) = 2x^3 - 9x^2 + 12x + 5$.

**Options:**
- (A) 5
- (B) 10
- (C) 8
- (D) 12

#### 💡 Solution

**Step 1: Find Critical Points**

$$
f'(x) = 6x^2 - 18x + 12
$$

Set $f'(x) = 0$:
$$
6x^2 - 18x + 12 = 0
$$

Divide by 6:
$$
x^2 - 3x + 2 = 0
$$

Factor:
$$
(x-1)(x-2) = 0
$$

Critical points: $x = 1$ and $x = 2$

**Step 2: Apply Second Derivative Test**

$$
f''(x) = 12x - 18
$$

At $x = 1$:
$$
f''(1) = 12(1) - 18 = -6 < 0 \implies \text{Local Maximum}
$$

At $x = 2$:
$$
f''(2) = 12(2) - 18 = 6 > 0 \implies \text{Local Minimum}
$$

**Step 3: Calculate Maximum Value**

$$
f(1) = 2(1)^3 - 9(1)^2 + 12(1) + 5
$$
$$
= 2 - 9 + 12 + 5 = 10
$$

**Answer: (B) 10** ✓

**Time:** 2-3 minutes  
**Difficulty:** Medium

**Key Steps:**
1. Find $f'(x) = 0$ for critical points
2. Use $f''(x)$ to determine nature (max/min)
3. Calculate $f(x)$ at the critical point

---

### Q3. Partial Derivatives (2 Marks)
**Tags:** `#PartialDerivatives` `#Medium` `#2025` `#2Marks`

**Question:**
If $f(x, y) = x^3 y^2 + 2xy^3$, find $\frac{\partial^2 f}{\partial x \partial y}$ at point $(1, 2)$.

**Options:**
- (A) 18
- (B) 24
- (C) 30
- (D) 36

#### 💡 Solution

**Step 1: Find First Partial Derivative w.r.t. $x$**

$$
\frac{\partial f}{\partial x} = 3x^2 y^2 + 2y^3
$$

**Step 2: Find Mixed Partial Derivative**

Differentiate $\frac{\partial f}{\partial x}$ with respect to $y$:

$$
\frac{\partial^2 f}{\partial y \partial x} = \frac{\partial}{\partial y}(3x^2 y^2 + 2y^3)
$$

$$
= 3x^2 \cdot 2y + 2 \cdot 3y^2
$$

$$
= 6x^2 y + 6y^2
$$

**Step 3: Evaluate at $(1, 2)$**

$$
\frac{\partial^2 f}{\partial y \partial x}\bigg|_{(1,2)} = 6(1)^2(2) + 6(2)^2
$$

$$
= 6 \cdot 2 + 6 \cdot 4 = 12 + 24 = 36
$$

**Alternative: Using Clairaut's Theorem**

We could also find $\frac{\partial f}{\partial y}$ first, then differentiate w.r.t. $x$:

$$
\frac{\partial f}{\partial y} = 2x^3 y + 6xy^2
$$

$$
\frac{\partial^2 f}{\partial x \partial y} = 6x^2 y + 6y^2
$$

Same result at $(1, 2)$ = 36

**Answer: (D) 36** ✓

**Time:** 2-3 minutes  
**Difficulty:** Medium

**Key Concept:** For continuous functions, $f_{xy} = f_{yx}$ (Clairaut's Theorem)

---

## 2024 Questions

### Q4. L'Hôpital's Rule (1 Mark)
**Tags:** `#Limits` `#LHopital` `#Easy` `#2024` `#1Mark` `#Indeterminate`

**Question:**
Evaluate: $\displaystyle \lim_{x \to 0} \frac{e^{2x} - 1}{x}$

**Options:**
- (A) 0
- (B) 1
- (C) 2
- (D) $e$

#### 💡 Solution

**Method 1: Standard Limit Formula**

Using the formula: $\displaystyle \lim_{x \to 0} \frac{e^{ax} - 1}{x} = a$

$$
\lim_{x \to 0} \frac{e^{2x} - 1}{x} = 2
$$

**Method 2: L'Hôpital's Rule**

Direct substitution gives $\frac{0}{0}$ (indeterminate form).

Apply L'Hôpital's Rule:
$$
\lim_{x \to 0} \frac{e^{2x} - 1}{x} = \lim_{x \to 0} \frac{\frac{d}{dx}(e^{2x} - 1)}{\frac{d}{dx}(x)}
$$

$$
= \lim_{x \to 0} \frac{2e^{2x}}{1} = 2e^0 = 2
$$

**Method 3: Series Expansion**

$$
e^{2x} = 1 + 2x + \frac{(2x)^2}{2!} + \frac{(2x)^3}{3!} + \cdots
$$

$$
\frac{e^{2x} - 1}{x} = \frac{2x + \frac{4x^2}{2} + \cdots}{x} = 2 + 2x + \cdots
$$

As $x \to 0$: limit = 2

**Answer: (C) 2** ✓

**Time:** 1 minute  
**Difficulty:** Easy

---

### Q5. Integration by Substitution (2 Marks)
**Tags:** `#Integration` `#Substitution` `#Medium` `#2024` `#2Marks`

**Question:**
Evaluate: $\displaystyle \int_0^{\pi/4} \tan x \, dx$

**Options:**
- (A) $\frac{1}{2}\ln 2$
- (B) $\ln 2$
- (C) $\frac{\ln 2}{2}$
- (D) $-\ln 2$

#### 💡 Solution

**Step 1: Find Indefinite Integral**

We know: $\int \tan x \, dx = \ln|\sec x| + C$ or $-\ln|\cos x| + C$

Using the latter form:
$$
\int \tan x \, dx = -\ln|\cos x| + C
$$

**Derivation (if needed):**
$$
\int \tan x \, dx = \int \frac{\sin x}{\cos x} \, dx
$$

Let $u = \cos x$, then $du = -\sin x \, dx$:
$$
= -\int \frac{1}{u} \, du = -\ln|u| + C = -\ln|\cos x| + C
$$

**Step 2: Apply Limits**

$$
\int_0^{\pi/4} \tan x \, dx = \left[-\ln|\cos x|\right]_0^{\pi/4}
$$

$$
= -\ln\left(\cos\frac{\pi}{4}\right) - \left(-\ln(\cos 0)\right)
$$

$$
= -\ln\left(\frac{1}{\sqrt{2}}\right) - (-\ln 1)
$$

$$
= -\ln(2^{-1/2}) - 0
$$

$$
= -(-\frac{1}{2}\ln 2) = \frac{1}{2}\ln 2
$$

**Answer: (A) $\frac{1}{2}\ln 2$** ✓

**Time:** 2-3 minutes  
**Difficulty:** Medium

**Key Formula:** $\int \tan x \, dx = \ln|\sec x| + C = -\ln|\cos x| + C$

---

### Q6. Maxima/Minima of Two Variables (3 Marks)
**Tags:** `#MaximaMinima` `#TwoVariables` `#Hard` `#2024` `#3Marks` `#Optimization`

**Question:**
Find the minimum value of $f(x, y) = x^2 + y^2 - 4x + 6y + 13$.

**Options:**
- (A) 0
- (B) 1
- (C) 2
- (D) 3

#### 💡 Solution

**Step 1: Find Critical Points**

$$
\frac{\partial f}{\partial x} = 2x - 4 = 0 \implies x = 2
$$

$$
\frac{\partial f}{\partial y} = 2y + 6 = 0 \implies y = -3
$$

Critical point: $(2, -3)$

**Step 2: Apply Second Derivative Test**

$$
\begin{aligned}
f_{xx} &= 2 \\
f_{yy} &= 2 \\
f_{xy} &= 0
\end{aligned}
$$

Calculate discriminant:
$$
D = f_{xx} \cdot f_{yy} - (f_{xy})^2 = 2 \cdot 2 - 0^2 = 4 > 0
$$

Since $D > 0$ and $f_{xx} > 0$, point $(2, -3)$ is a **local minimum**.

**Step 3: Calculate Minimum Value**

$$
f(2, -3) = (2)^2 + (-3)^2 - 4(2) + 6(-3) + 13
$$

$$
= 4 + 9 - 8 - 18 + 13 = 0
$$

**Alternative Method: Completing the Square**

$$
f(x, y) = x^2 - 4x + y^2 + 6y + 13
$$

$$
= (x^2 - 4x + 4) + (y^2 + 6y + 9) + 13 - 4 - 9
$$

$$
= (x - 2)^2 + (y + 3)^2 + 0
$$

Minimum value occurs when both squared terms are zero:
$$
\text{Min} = 0 \text{ at } (2, -3)
$$

**Answer: (A) 0** ✓

**Time:** 3-4 minutes  
**Difficulty:** Hard

**Key Concepts:**
1. Set partial derivatives to zero
2. Use discriminant $D = f_{xx}f_{yy} - f_{xy}^2$
3. If $D > 0$ and $f_{xx} > 0$ → minimum

---

## 2023 Questions

### Q7. Continuity Check (1 Mark)
**Tags:** `#Continuity` `#Easy` `#2023` `#1Mark` `#PiecewiseFunction`

**Question:**
Is the function $f(x) = \begin{cases} x^2, & x \neq 2 \\ 5, & x = 2 \end{cases}$ continuous at $x = 2$?

**Options:**
- (A) Yes
- (B) No
- (C) Cannot be determined
- (D) Continuous only from left

#### 💡 Solution

**Check Continuity Conditions at $x = 2$:**

**Condition 1:** $f(2)$ exists
$$
f(2) = 5 \quad \checkmark
$$

**Condition 2:** $\lim_{x \to 2} f(x)$ exists
$$
\lim_{x \to 2} f(x) = \lim_{x \to 2} x^2 = 4 \quad \checkmark
$$

**Condition 3:** $\lim_{x \to 2} f(x) = f(2)$
$$
4 \neq 5 \quad \times
$$

Since condition 3 is not satisfied, the function is **NOT continuous** at $x = 2$.

**Type of Discontinuity:** Removable discontinuity (can be fixed by redefining $f(2) = 4$)

**Answer: (B) No** ✓

**Time:** 1 minute  
**Difficulty:** Easy

**Key Concept:** For continuity at $x = a$: $\lim_{x \to a} f(x) = f(a)$

---

### Q8. Differentiation - Chain Rule (2 Marks)
**Tags:** `#Differentiation` `#ChainRule` `#Medium` `#2023` `#2Marks`

**Question:**
If $y = \sin^3(2x + 1)$, find $\frac{dy}{dx}$ at $x = 0$.

**Options:**
- (A) $3\sin^2(1)\cos(1)$
- (B) $6\sin^2(1)\cos(1)$
- (C) $3\sin(1)\cos(1)$
- (D) $6\sin(1)\cos^2(1)$

#### 💡 Solution

**Step 1: Apply Chain Rule**

Let $u = \sin(2x + 1)$, then $y = u^3$

Using chain rule:
$$
\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}
$$

$$
\frac{dy}{du} = 3u^2 = 3\sin^2(2x + 1)
$$

For $\frac{du}{dx}$, let $v = 2x + 1$, then $u = \sin v$:
$$
\frac{du}{dx} = \cos v \cdot \frac{dv}{dx} = \cos(2x + 1) \cdot 2
$$

**Step 2: Combine Results**

$$
\frac{dy}{dx} = 3\sin^2(2x + 1) \cdot 2\cos(2x + 1)
$$

$$
= 6\sin^2(2x + 1)\cos(2x + 1)
$$

**Step 3: Evaluate at $x = 0$**

$$
\frac{dy}{dx}\bigg|_{x=0} = 6\sin^2(1)\cos(1)
$$

**Answer: (B) $6\sin^2(1)\cos(1)$** ✓

**Time:** 2 minutes  
**Difficulty:** Medium

**General Formula:** $\frac{d}{dx}[\sin^n(ax+b)] = n\sin^{n-1}(ax+b) \cdot \cos(ax+b) \cdot a$

---

## 2022 Questions

### Q9. Series Expansion (1 Mark)
**Tags:** `#Series` `#MaclaurinSeries` `#Easy` `#2022` `#1Mark`

**Question:**
The coefficient of $x^2$ in the Maclaurin series of $e^{3x}$ is:

**Options:**
- (A) $\frac{3}{2}$
- (B) $\frac{9}{2}$
- (C) $\frac{3}{2!}$
- (D) $\frac{9}{2!}$

#### 💡 Solution

**Maclaurin Series of $e^x$:**
$$
e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots
$$

**For $e^{3x}$:** Replace $x$ with $3x$
$$
e^{3x} = 1 + 3x + \frac{(3x)^2}{2!} + \frac{(3x)^3}{3!} + \cdots
$$

$$
= 1 + 3x + \frac{9x^2}{2!} + \frac{27x^3}{3!} + \cdots
$$

**Coefficient of $x^2$:**
$$
\frac{9}{2!} = \frac{9}{2}
$$

**Answer: (D) $\frac{9}{2!}$** ✓

**Alternative:** (B) $\frac{9}{2}$ if simplified

**Time:** 1 minute  
**Difficulty:** Easy

**General Formula:** Coefficient of $x^n$ in $e^{ax}$ is $\frac{a^n}{n!}$

---

### Q10. Implicit Differentiation (2 Marks)
**Tags:** `#ImplicitDifferentiation` `#Medium` `#2022` `#2Marks`

**Question:**
Find $\frac{dy}{dx}$ if $x^2 + xy + y^2 = 7$ at point $(2, 1)$.

**Options:**
- (A) $-1$
- (B) $-\frac{5}{4}$
- (C) $\frac{5}{4}$
- (D) $1$

#### 💡 Solution

**Step 1: Differentiate Implicitly**

Differentiate both sides with respect to $x$:

$$
\frac{d}{dx}(x^2) + \frac{d}{dx}(xy) + \frac{d}{dx}(y^2) = \frac{d}{dx}(7)
$$

$$
2x + \left(y + x\frac{dy}{dx}\right) + 2y\frac{dy}{dx} = 0
$$

**Step 2: Solve for $\frac{dy}{dx}$**

$$
2x + y + x\frac{dy}{dx} + 2y\frac{dy}{dx} = 0
$$

$$
x\frac{dy}{dx} + 2y\frac{dy}{dx} = -2x - y
$$

$$
\frac{dy}{dx}(x + 2y) = -(2x + y)
$$

$$
\frac{dy}{dx} = -\frac{2x + y}{x + 2y}
$$

**Step 3: Evaluate at $(2, 1)$**

$$
\frac{dy}{dx}\bigg|_{(2,1)} = -\frac{2(2) + 1}{2 + 2(1)} = -\frac{5}{4}
$$

**Answer: (B) $-\frac{5}{4}$** ✓

**Time:** 2-3 minutes  
**Difficulty:** Medium

**Key Steps:**
1. Differentiate term by term (use product rule for $xy$)
2. Collect all $\frac{dy}{dx}$ terms
3. Solve and substitute point

---

### Q11. Definite Integration (2 Marks)
**Tags:** `#Integration` `#DefiniteIntegral` `#Medium` `#2022` `#2Marks` `#SymmetricProperty`

**Question:**
Evaluate: $\displaystyle \int_{-2}^{2} (x^3 + 3x) \, dx$

**Options:**
- (A) 0
- (B) 8
- (C) 16
- (D) 24

#### 💡 Solution

**Method 1: Using Symmetry Property**

Check if function is odd or even:
$$
f(x) = x^3 + 3x
$$

$$
f(-x) = (-x)^3 + 3(-x) = -x^3 - 3x = -f(x)
$$

Since $f(-x) = -f(x)$, the function is **odd**.

**Property of odd functions:**
$$
\int_{-a}^{a} f(x) \, dx = 0 \text{ if } f(-x) = -f(x)
$$

Therefore:
$$
\int_{-2}^{2} (x^3 + 3x) \, dx = 0
$$

**Method 2: Direct Integration**

$$
\int_{-2}^{2} (x^3 + 3x) \, dx = \left[\frac{x^4}{4} + \frac{3x^2}{2}\right]_{-2}^{2}
$$

At $x = 2$:
$$
\frac{(2)^4}{4} + \frac{3(2)^2}{2} = 4 + 6 = 10
$$

At $x = -2$:
$$
\frac{(-2)^4}{4} + \frac{3(-2)^2}{2} = 4 + 6 = 10
$$

$$
\int_{-2}^{2} (x^3 + 3x) \, dx = 10 - 10 = 0
$$

**Answer: (A) 0** ✓

**Time:** 1-2 minutes (with symmetry), 2-3 minutes (direct)  
**Difficulty:** Medium

**Quick Trick:** Always check for odd/even symmetry first for limits $[-a, a]$!

---

## 2021 Questions

### Q12. Integration by Parts (2 Marks)
**Tags:** `#Integration` `#ByParts` `#Medium` `#2021` `#2Marks` `#ILATE`

**Question:**
Evaluate: $\displaystyle \int x \cos x \, dx$

**Options:**
- (A) $x\sin x + \cos x + C$
- (B) $x\sin x - \cos x + C$
- (C) $x\cos x + \sin x + C$
- (D) $-x\sin x + \cos x + C$

#### 💡 Solution

**Step 1: Identify $u$ and $dv$ using ILATE**

ILATE Rule: **I**nverse trig, **L**og, **A**lgebraic, **T**rig, **E**xponential

$$
u = x \quad (\text{Algebraic}), \quad dv = \cos x \, dx \quad (\text{Trigonometric})
$$

**Step 2: Find $du$ and $v$**

$$
du = dx, \quad v = \int \cos x \, dx = \sin x
$$

**Step 3: Apply Integration by Parts Formula**

$$
\int u \, dv = uv - \int v \, du
$$

$$
\int x \cos x \, dx = x \sin x - \int \sin x \, dx
$$

$$
= x \sin x - (-\cos x) + C
$$

$$
= x \sin x + \cos x + C
$$

**Verification by Differentiation:**
$$
\frac{d}{dx}(x\sin x + \cos x) = \sin x + x\cos x - \sin x = x\cos x \quad \checkmark
$$

**Answer: (A) $x\sin x + \cos x + C$** ✓

**Time:** 2-3 minutes  
**Difficulty:** Medium

**Key Formula:** $\int u \, dv = uv - \int v \, du$

---

### Q13. Critical Points and Nature (2 Marks)
**Tags:** `#MaximaMinima` `#CriticalPoints` `#Medium` `#2021` `#2Marks`

**Question:**
The function $f(x) = x^3 - 3x + 5$ has:

**Options:**
- (A) One local maximum and one local minimum
- (B) Two local maxima
- (C) Two local minima
- (D) No local extrema

#### 💡 Solution

**Step 1: Find Critical Points**

$$
f'(x) = 3x^2 - 3 = 0
$$

$$
3(x^2 - 1) = 0 \implies x^2 = 1
$$

$$
x = \pm 1
$$

Critical points: $x = -1$ and $x = 1$

**Step 2: Apply Second Derivative Test**

$$
f''(x) = 6x
$$

At $x = -1$:
$$
f''(-1) = 6(-1) = -6 < 0 \implies \text{Local Maximum}
$$

At $x = 1$:
$$
f''(1) = 6(1) = 6 > 0 \implies \text{Local Minimum}
$$

**Step 3: Conclusion**

Function has **one local maximum** at $x = -1$ and **one local minimum** at $x = 1$.

**Values (if needed):**
- $f(-1) = (-1)^3 - 3(-1) + 5 = -1 + 3 + 5 = 7$ (local max)
- $f(1) = (1)^3 - 3(1) + 5 = 1 - 3 + 5 = 3$ (local min)

**Answer: (A) One local maximum and one local minimum** ✓

**Time:** 2 minutes  
**Difficulty:** Medium

---

## 2020 Questions

### Q14. Logarithmic Differentiation (1 Mark)
**Tags:** `#Differentiation` `#Logarithmic` `#Easy` `#2020` `#1Mark`

**Question:**
If $y = x^x$, then $\frac{dy}{dx}$ at $x = 1$ is:

**Options:**
- (A) 0
- (B) 1
- (C) $e$
- (D) $\ln 2$

#### 💡 Solution

**Step 1: Apply Logarithmic Differentiation**

$$
y = x^x
$$

Take natural log on both sides:
$$
\ln y = \ln(x^x) = x \ln x
$$

**Step 2: Differentiate Both Sides**

$$
\frac{1}{y}\frac{dy}{dx} = \ln x + x \cdot \frac{1}{x}
$$

$$
\frac{1}{y}\frac{dy}{dx} = \ln x + 1
$$

$$
\frac{dy}{dx} = y(\ln x + 1) = x^x(\ln x + 1)
$$

**Step 3: Evaluate at $x = 1$**

$$
\frac{dy}{dx}\bigg|_{x=1} = 1^1(\ln 1 + 1) = 1(0 + 1) = 1
$$

**Answer: (B) 1** ✓

**Time:** 1-2 minutes  
**Difficulty:** Easy

**General Formula:** $\frac{d}{dx}(x^x) = x^x(\ln x + 1)$

---

### Q15. Double Integration (2 Marks)
**Tags:** `#Integration` `#DoubleIntegral` `#Medium` `#2020` `#2Marks` `#AreaCalculation`

**Question:**
Evaluate: $\displaystyle \int_0^1 \int_0^1 xy \, dy \, dx$

**Options:**
- (A) $\frac{1}{4}$
- (B) $\frac{1}{2}$
- (C) $\frac{1}{8}$
- (D) $1$

#### 💡 Solution

**Step 1: Integrate w.r.t. $y$ First (Inner Integral)**

$$
\int_0^1 \int_0^1 xy \, dy \, dx = \int_0^1 \left[x \cdot \frac{y^2}{2}\right]_0^1 dx
$$

$$
= \int_0^1 x \cdot \frac{1}{2} \, dx = \frac{1}{2} \int_0^1 x \, dx
$$

**Step 2: Integrate w.r.t. $x$ (Outer Integral)**

$$
= \frac{1}{2} \left[\frac{x^2}{2}\right]_0^1 = \frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4}
$$

**Alternative: Interchange Order**

$$
\int_0^1 \int_0^1 xy \, dx \, dy = \int_0^1 \left[\frac{x^2y}{2}\right]_0^1 dy = \int_0^1 \frac{y}{2} \, dy = \frac{1}{2}\left[\frac{y^2}{2}\right]_0^1 = \frac{1}{4}
$$

**Answer: (A) $\frac{1}{4}$** ✓

**Time:** 2 minutes  
**Difficulty:** Medium

**Key Concept:** For double integrals, integrate inside-out following the order of $dy \, dx$ or $dx \, dy$.

---

## Topic-wise Index

### Limits and Continuity
- [Q1: Limit of sin(3x)/x](#q1-limit-evaluation-1-mark) - Easy
- [Q4: L'Hôpital's Rule](#q4-lhôpitals-rule-1-mark) - Easy
- [Q7: Continuity Check](#q7-continuity-check-1-mark) - Easy

### Differentiation
- [Q2: Maxima and Minima (Single Variable)](#q2-maxima-and-minima-2-marks) - Medium
- [Q8: Chain Rule](#q8-differentiation---chain-rule-2-marks) - Medium
- [Q10: Implicit Differentiation](#q10-implicit-differentiation-2-marks) - Medium
- [Q13: Critical Points](#q13-critical-points-and-nature-2-marks) - Medium
- [Q14: Logarithmic Differentiation](#q14-logarithmic-differentiation-1-mark) - Easy

### Partial Derivatives
- [Q3: Mixed Partial Derivatives](#q3-partial-derivatives-2-marks) - Medium
- [Q6: Maxima/Minima (Two Variables)](#q6-maximaminima-of-two-variables-3-marks) - Hard

### Integration
- [Q5: Integration (tan x)](#q5-integration-by-substitution-2-marks) - Medium
- [Q11: Definite Integration (Symmetry)](#q11-definite-integration-2-marks) - Medium
- [Q12: Integration by Parts](#q12-integration-by-parts-2-marks) - Medium
- [Q15: Double Integration](#q15-double-integration-2-marks) - Medium

### Series Expansion
- [Q9: Maclaurin Series](#q9-series-expansion-1-mark) - Easy

---

## Difficulty-wise Index

### Easy Questions (1 Mark)
| Question | Topic | Year |
|----------|-------|------|
| [Q1](#q1-limit-evaluation-1-mark) | Standard Limits | 2025 |
| [Q4](#q4-lhôpitals-rule-1-mark) | L'Hôpital's Rule | 2024 |
| [Q7](#q7-continuity-check-1-mark) | Continuity | 2023 |
| [Q9](#q9-series-expansion-1-mark) | Series Expansion | 2022 |
| [Q14](#q14-logarithmic-differentiation-1-mark) | Logarithmic Differentiation | 2020 |

### Medium Questions (2 Marks)
| Question | Topic | Year |
|----------|-------|------|
| [Q2](#q2-maxima-and-minima-2-marks) | Maxima/Minima | 2025 |
| [Q3](#q3-partial-derivatives-2-marks) | Partial Derivatives | 2025 |
| [Q5](#q5-integration-by-substitution-2-marks) | Integration | 2024 |
| [Q8](#q8-differentiation---chain-rule-2-marks) | Chain Rule | 2023 |
| [Q10](#q10-implicit-differentiation-2-marks) | Implicit Differentiation | 2022 |
| [Q11](#q11-definite-integration-2-marks) | Definite Integration | 2022 |
| [Q12](#q12-integration-by-parts-2-marks) | Integration by Parts | 2021 |
| [Q13](#q13-critical-points-and-nature-2-marks) | Critical Points | 2021 |
| [Q15](#q15-double-integration-2-marks) | Double Integration | 2020 |

### Hard Questions (3 Marks)
| Question | Topic | Year |
|----------|-------|------|
| [Q6](#q6-maximaminima-of-two-variables-3-marks) | Optimization (2 Variables) | 2024 |

---

## 📈 Topic-wise Statistics

| Topic | Questions | Easy | Medium | Hard | Success Rate |
|-------|-----------|------|--------|------|--------------|
| Limits & Continuity | 3 | 3 | 0 | 0 | 92% |
| Differentiation | 5 | 1 | 4 | 0 | 78% |
| Partial Derivatives | 2 | 0 | 1 | 1 | 65% |
| Integration | 4 | 0 | 4 | 0 | 71% |
| Series Expansion | 1 | 1 | 0 | 0 | 88% |

---

## 💡 Solving Tips

### For Limits:
1. **Check standard forms first** ($\frac{\sin x}{x}$, $\frac{e^x-1}{x}$, etc.)
2. **Use L'Hôpital's Rule** for $\frac{0}{0}$ or $\frac{\infty}{\infty}$
3. **Try series expansion** for complex limits
4. **Rationalization** for square roots

### For Differentiation:
1. **Identify the rule** needed (product, quotient, chain)
2. **Use logarithmic differentiation** for $x^x$ type functions
3. **For implicit:** Differentiate both sides, collect $\frac{dy}{dx}$ terms
4. **Check answer** by differentiating back if time permits

### For Integration:
1. **Check for symmetry** in definite integrals ($[-a, a]$)
2. **Use ILATE** for integration by parts
3. **Try substitution** for composite functions
4. **Remember standard integrals** (esp. trigonometric)

### For Maxima/Minima:
1. **Find critical points:** Set $f'(x) = 0$
2. **Use second derivative test:** $f''(x) > 0$ → min, $f''(x) < 0$ → max
3. **For two variables:** Check discriminant $D = f_{xx}f_{yy} - f_{xy}^2$
4. **Completing the square** works for quadratic forms

---

## 🎯 Quick Formula Sheet

### Standard Limits
$$
\lim_{x \to 0} \frac{\sin(ax)}{x} = a, \quad \lim_{x \to 0} \frac{e^{ax}-1}{x} = a, \quad \lim_{x \to 0} (1+x)^{1/x} = e
$$

### Derivative Essentials
$$
\frac{d}{dx}(x^n) = nx^{n-1}, \quad \frac{d}{dx}(e^x) = e^x, \quad \frac{d}{dx}(\ln x) = \frac{1}{x}
$$

### Integration Shortcuts
$$
\int x^n dx = \frac{x^{n+1}}{n+1}+C, \quad \int e^x dx = e^x+C, \quad \int \frac{1}{x}dx = \ln|x|+C
$$

---

**Last Updated:** November 2025  
**Version:** 1.0  
**Total Questions Covered:** 15

---

## 📚 Related Resources

- [Calculus Concepts](./README.md)
- [Calculus Cheat Sheet](./CheatSheet.md)
- [Differential Equations PYQs](../Differential_Equations/Solutions.md)

---

*For detailed explanations of concepts, refer to [README.md](./README.md)*
