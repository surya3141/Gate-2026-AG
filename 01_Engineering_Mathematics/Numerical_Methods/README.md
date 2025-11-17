# 🔢 Numerical Methods - Concepts & Theory

> Comprehensive guide to Numerical Methods for GATE AG

---

## 📚 Table of Contents

1. [Solutions of Algebraic Equations](#1-solutions-of-algebraic-equations)
2. [Numerical Integration](#2-numerical-integration)
3. [Numerical Differentiation](#3-numerical-differentiation)
4. [Numerical Solutions of ODEs](#4-numerical-solutions-of-odes)
5. [Interpolation](#5-interpolation)
6. [Error Analysis](#6-error-analysis)

---

## 1. Solutions of Algebraic Equations

### 1.1 Linear Equations - Gaussian Elimination

**System of Linear Equations:**
$$
\begin{cases}
a_{11}x_1 + a_{12}x_2 + a_{13}x_3 = b_1 \\
a_{21}x_1 + a_{22}x_2 + a_{23}x_3 = b_2 \\
a_{31}x_1 + a_{32}x_2 + a_{33}x_3 = b_3
\end{cases}
$$

**Matrix Form:** $AX = B$

**Gaussian Elimination Steps:**

1. **Forward Elimination:** Convert to upper triangular form
2. **Back Substitution:** Solve from bottom to top

**Example:** Solve
$$
\begin{cases}
2x + y + z = 5 \\
4x - 6y = -2 \\
-2x + 7y + 2z = 9
\end{cases}
$$

**Augmented Matrix:**
$$
\left[\begin{array}{ccc|c}
2 & 1 & 1 & 5 \\
4 & -6 & 0 & -2 \\
-2 & 7 & 2 & 9
\end{array}\right]
$$

After forward elimination and back substitution: $x = 1$, $y = 2$, $z = 1$

### 1.2 Non-Linear Equations - Root Finding

#### 1.2.1 Bisection Method

**Concept:** If $f(a)$ and $f(b)$ have opposite signs, root exists in $[a,b]$

**Algorithm:**
1. Check: $f(a) \cdot f(b) < 0$
2. Find midpoint: $c = \frac{a+b}{2}$
3. Check: 
   - If $f(c) = 0$, root is $c$
   - If $f(a) \cdot f(c) < 0$, root in $[a,c]$, set $b = c$
   - If $f(c) \cdot f(b) < 0$, root in $[c,b]$, set $a = c$
4. Repeat until $|b-a| < \epsilon$ (tolerance)

**Formula for $n$-th iteration:**
$$
c_n = \frac{a_n + b_n}{2}
$$

**Number of iterations needed:**
$$
n = \left\lceil \frac{\ln(b-a) - \ln(\epsilon)}{\ln 2} \right\rceil
$$

**Advantages:**
- Always converges if $f(a) \cdot f(b) < 0$
- Simple and reliable

**Disadvantages:**
- Slow convergence (linear)
- Requires two initial points with opposite signs

**Example:** Find root of $f(x) = x^3 - x - 2$ in $[1, 2]$

$f(1) = -2 < 0$, $f(2) = 4 > 0$ → Root exists

$c_1 = \frac{1+2}{2} = 1.5$, $f(1.5) = -0.875 < 0$

$c_2 = \frac{1.5+2}{2} = 1.75$, $f(1.75) = 0.609 > 0$

Continue until desired accuracy...

#### 1.2.2 Newton-Raphson Method

**Formula:**
$$
x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}
$$

**Geometric Interpretation:** Tangent line approximation

**Algorithm:**
1. Start with initial guess $x_0$
2. Calculate $f(x_0)$ and $f'(x_0)$
3. Find $x_1 = x_0 - \frac{f(x_0)}{f'(x_0)}$
4. Repeat until $|x_{n+1} - x_n| < \epsilon$

**Convergence:** Quadratic (very fast near root)

**Advantages:**
- Very fast convergence
- Needs only one initial guess

**Disadvantages:**
- Requires derivative calculation
- May fail if $f'(x_n) = 0$ or near zero
- May diverge with poor initial guess

**Example:** Find root of $f(x) = x^2 - 2$ (finding $\sqrt{2}$)

$$
f'(x) = 2x
$$

Starting with $x_0 = 1$:

$$
x_1 = 1 - \frac{1^2-2}{2(1)} = 1 - \frac{-1}{2} = 1.5
$$

$$
x_2 = 1.5 - \frac{1.5^2-2}{2(1.5)} = 1.5 - \frac{0.25}{3} = 1.4167
$$

$$
x_3 = 1.4167 - \frac{1.4167^2-2}{2(1.4167)} \approx 1.4142
$$

Converges to $\sqrt{2} = 1.41421...$

#### 1.2.3 Secant Method

**Formula:**
$$
x_{n+1} = x_n - f(x_n) \frac{x_n - x_{n-1}}{f(x_n) - f(x_{n-1})}
$$

**Concept:** Approximates derivative using finite difference

$$
f'(x_n) \approx \frac{f(x_n) - f(x_{n-1})}{x_n - x_{n-1}}
$$

**Advantages:**
- No derivative needed
- Faster than bisection

**Disadvantages:**
- Needs two initial guesses
- May not converge

**Convergence Rate:** Superlinear ($\approx 1.618$)

#### 1.2.4 Fixed-Point Iteration

**Form:** Rewrite $f(x) = 0$ as $x = g(x)$

**Iteration:**
$$
x_{n+1} = g(x_n)
$$

**Convergence Condition:**
$$
|g'(x)| < 1 \text{ in the neighborhood of the root}
$$

**Example:** Solve $x^3 + x - 1 = 0$

Rewrite as: $x = \frac{1}{x^2+1} = g(x)$

Starting with $x_0 = 0.5$:

$x_1 = g(0.5) = \frac{1}{0.25+1} = 0.8$

$x_2 = g(0.8) = \frac{1}{0.64+1} = 0.6098$

Continue...

---

## 2. Numerical Integration

### 2.1 Trapezoidal Rule

**Concept:** Approximate area under curve using trapezoids

**Single Application:**
$$
\int_a^b f(x)dx \approx \frac{b-a}{2}[f(a) + f(b)]
$$

**Multiple Application (Composite):**

Divide $[a,b]$ into $n$ equal intervals of width $h = \frac{b-a}{n}$

$$
\int_a^b f(x)dx \approx \frac{h}{2}[f(x_0) + 2f(x_1) + 2f(x_2) + \cdots + 2f(x_{n-1}) + f(x_n)]
$$

**Compact Form:**
$$
\int_a^b f(x)dx \approx \frac{h}{2}\left[f(x_0) + f(x_n) + 2\sum_{i=1}^{n-1}f(x_i)\right]
$$

**Error:**
$$
E = -\frac{(b-a)^3}{12n^2}f''(\xi) \quad \text{for some } \xi \in [a,b]
$$

**Error is $O(h^2)$** - second-order accurate

**Example:** Evaluate $\int_0^1 x^2 dx$ using $n=4$ intervals

$h = \frac{1-0}{4} = 0.25$

Points: $x_0=0, x_1=0.25, x_2=0.5, x_3=0.75, x_4=1$

$$
\begin{aligned}
I &\approx \frac{0.25}{2}[0^2 + 1^2 + 2(0.25^2 + 0.5^2 + 0.75^2)] \\
&= 0.125[1 + 2(0.0625 + 0.25 + 0.5625)] \\
&= 0.125[1 + 2(0.875)] \\
&= 0.125[2.75] = 0.34375
\end{aligned}
$$

Exact value: $\frac{1}{3} = 0.33333...$

Error: $0.34375 - 0.33333 = 0.01042$

### 2.2 Simpson's 1/3 Rule

**Concept:** Approximate using parabolas (quadratic polynomials)

**Single Application:** (requires 3 points, 2 intervals)
$$
\int_a^b f(x)dx \approx \frac{h}{3}[f(x_0) + 4f(x_1) + f(x_2)]
$$

where $h = \frac{b-a}{2}$, $x_1 = \frac{a+b}{2}$

**Multiple Application:**

Requires **even number** of intervals ($n$ even)

$$
\int_a^b f(x)dx \approx \frac{h}{3}[f(x_0) + 4f(x_1) + 2f(x_2) + 4f(x_3) + 2f(x_4) + \cdots + 4f(x_{n-1}) + f(x_n)]
$$

**Pattern:** 1, 4, 2, 4, 2, 4, ..., 2, 4, 1

**Compact Form:**
$$
\int_a^b f(x)dx \approx \frac{h}{3}\left[f(x_0) + f(x_n) + 4\sum_{i=\text{odd}}f(x_i) + 2\sum_{i=\text{even}}f(x_i)\right]
$$

**Error:**
$$
E = -\frac{(b-a)^5}{180n^4}f^{(4)}(\xi)
$$

**Error is $O(h^4)$** - fourth-order accurate (more accurate than Trapezoidal)

**Example:** Evaluate $\int_0^1 x^2 dx$ using $n=4$ intervals

$h = 0.25$

$$
\begin{aligned}
I &\approx \frac{0.25}{3}[0^2 + 4(0.25^2) + 2(0.5^2) + 4(0.75^2) + 1^2] \\
&= \frac{0.25}{3}[0 + 4(0.0625) + 2(0.25) + 4(0.5625) + 1] \\
&= \frac{0.25}{3}[0 + 0.25 + 0.5 + 2.25 + 1] \\
&= \frac{0.25}{3}[4] = 0.33333...
\end{aligned}
$$

Exact value: $\frac{1}{3} = 0.33333...$

Error: Nearly zero! (Simpson's is exact for polynomials up to degree 3)

### 2.3 Simpson's 3/8 Rule

**Single Application:** (requires 4 points, 3 intervals)
$$
\int_a^b f(x)dx \approx \frac{3h}{8}[f(x_0) + 3f(x_1) + 3f(x_2) + f(x_3)]
$$

where $h = \frac{b-a}{3}$

**Pattern:** 1, 3, 3, 1

**Use:** When number of intervals is multiple of 3

**Error:** Similar to Simpson's 1/3, $O(h^4)$

### 2.4 Comparison of Methods

| Method | Points Needed | Multipliers | Error Order | Best For |
|--------|---------------|-------------|-------------|----------|
| Trapezoidal | 2+ | 1, 2, 2, ..., 2, 1 | $O(h^2)$ | Quick approximation |
| Simpson's 1/3 | 3+ (odd points) | 1, 4, 2, 4, ..., 1 | $O(h^4)$ | Better accuracy |
| Simpson's 3/8 | 4+ | 1, 3, 3, 1, ... | $O(h^4)$ | 3k intervals |

**Rule of Thumb:**
- Use **Simpson's 1/3** when possible (even intervals)
- Use **Trapezoidal** when data is limited
- Simpson's is **exact for polynomials** up to degree 3

---

## 3. Numerical Differentiation

### 3.1 Forward Difference Formula

$$
f'(x_0) \approx \frac{f(x_0 + h) - f(x_0)}{h}
$$

**Error:** $O(h)$

### 3.2 Backward Difference Formula

$$
f'(x_0) \approx \frac{f(x_0) - f(x_0 - h)}{h}
$$

**Error:** $O(h)$

### 3.3 Central Difference Formula

$$
f'(x_0) \approx \frac{f(x_0 + h) - f(x_0 - h)}{2h}
$$

**Error:** $O(h^2)$ - more accurate!

### 3.4 Second Derivative

$$
f''(x_0) \approx \frac{f(x_0 + h) - 2f(x_0) + f(x_0 - h)}{h^2}
$$

---

## 4. Numerical Solutions of ODEs

### 4.1 Euler's Method

**Problem:** Solve $\frac{dy}{dx} = f(x,y)$ with $y(x_0) = y_0$

**Formula:**
$$
y_{n+1} = y_n + h \cdot f(x_n, y_n)
$$

where $h$ is step size, $x_{n+1} = x_n + h$

**Geometric Interpretation:** Follow tangent line for small step

**Algorithm:**
1. Start with $(x_0, y_0)$
2. Calculate slope: $k = f(x_0, y_0)$
3. Next point: $y_1 = y_0 + h \cdot k$
4. Update: $x_1 = x_0 + h$
5. Repeat

**Example:** Solve $\frac{dy}{dx} = x + y$, $y(0) = 1$, find $y(0.2)$ with $h = 0.1$

**Step 1:** $x_0 = 0$, $y_0 = 1$
$$
y_1 = y_0 + h \cdot f(x_0, y_0) = 1 + 0.1(0 + 1) = 1.1
$$

**Step 2:** $x_1 = 0.1$, $y_1 = 1.1$
$$
y_2 = y_1 + h \cdot f(x_1, y_1) = 1.1 + 0.1(0.1 + 1.1) = 1.1 + 0.12 = 1.22
$$

Therefore, $y(0.2) \approx 1.22$

**Advantages:**
- Simple to implement
- Easy to understand

**Disadvantages:**
- First-order accuracy $O(h)$
- Can be unstable
- Accumulates error

### 4.2 Modified Euler's Method (Heun's Method)

**Predictor-Corrector Approach:**

**Predictor:**
$$
y_{n+1}^* = y_n + h \cdot f(x_n, y_n)
$$

**Corrector:**
$$
y_{n+1} = y_n + \frac{h}{2}[f(x_n, y_n) + f(x_{n+1}, y_{n+1}^*)]
$$

**Average slope** between start and predicted endpoint

**More accurate than standard Euler:** $O(h^2)$

**Example:** Same problem as above with $h = 0.1$

**Step 1:**
- Predictor: $y_1^* = 1 + 0.1(0+1) = 1.1$
- Corrector: $y_1 = 1 + \frac{0.1}{2}[f(0,1) + f(0.1, 1.1)]$
  $$
  = 1 + 0.05[1 + 1.2] = 1 + 0.11 = 1.11
  $$

**Step 2:**
- Predictor: $y_2^* = 1.11 + 0.1(0.1 + 1.11) = 1.231$
- Corrector: $y_2 = 1.11 + 0.05[(0.1+1.11) + (0.2+1.231)]$
  $$
  = 1.11 + 0.05[1.21 + 1.431] = 1.11 + 0.132 = 1.242
  $$

### 4.3 Runge-Kutta 2nd Order (RK2)

**Formula:**
$$
\begin{aligned}
k_1 &= h \cdot f(x_n, y_n) \\
k_2 &= h \cdot f(x_n + h, y_n + k_1) \\
y_{n+1} &= y_n + \frac{k_1 + k_2}{2}
\end{aligned}
$$

**Accuracy:** $O(h^2)$

### 4.4 Runge-Kutta 4th Order (RK4)

**Most Popular ODE Solver!**

**Formula:**
$$
\begin{aligned}
k_1 &= h \cdot f(x_n, y_n) \\
k_2 &= h \cdot f\left(x_n + \frac{h}{2}, y_n + \frac{k_1}{2}\right) \\
k_3 &= h \cdot f\left(x_n + \frac{h}{2}, y_n + \frac{k_2}{2}\right) \\
k_4 &= h \cdot f(x_n + h, y_n + k_3) \\
y_{n+1} &= y_n + \frac{1}{6}(k_1 + 2k_2 + 2k_3 + k_4)
\end{aligned}
$$

**Weighted Average:** $\frac{1}{6}k_1 + \frac{2}{6}k_2 + \frac{2}{6}k_3 + \frac{1}{6}k_4$

**Accuracy:** $O(h^4)$ - very accurate!

**Example:** Solve $\frac{dy}{dx} = x + y$, $y(0) = 1$, find $y(0.1)$

$$
\begin{aligned}
k_1 &= 0.1 \cdot f(0, 1) = 0.1(0+1) = 0.1 \\
k_2 &= 0.1 \cdot f(0.05, 1.05) = 0.1(0.05+1.05) = 0.11 \\
k_3 &= 0.1 \cdot f(0.05, 1.055) = 0.1(0.05+1.055) = 0.1105 \\
k_4 &= 0.1 \cdot f(0.1, 1.1105) = 0.1(0.1+1.1105) = 0.12105 \\
y_1 &= 1 + \frac{1}{6}(0.1 + 2(0.11) + 2(0.1105) + 0.12105) \\
&= 1 + \frac{1}{6}(0.6631) = 1.1105
\end{aligned}
$$

### 4.5 Comparison of ODE Methods

| Method | Order of Accuracy | Stability | Computational Cost |
|--------|-------------------|-----------|-------------------|
| Euler | $O(h)$ | Poor | Low |
| Modified Euler | $O(h^2)$ | Better | Medium |
| RK2 | $O(h^2)$ | Good | Medium |
| RK4 | $O(h^4)$ | Excellent | Higher |

**RK4 is the standard choice** - good balance of accuracy and efficiency

---

## 5. Interpolation

### 5.1 Linear Interpolation

**Two points:** $(x_0, y_0)$ and $(x_1, y_1)$

**Formula:**
$$
y(x) = y_0 + \frac{y_1 - y_0}{x_1 - x_0}(x - x_0)
$$

**Example:** Find $y(2.5)$ if $y(2) = 4$ and $y(3) = 7$

$$
y(2.5) = 4 + \frac{7-4}{3-2}(2.5-2) = 4 + 3(0.5) = 5.5
$$

### 5.2 Lagrange Interpolation

**For $n+1$ points:** $(x_0, y_0), (x_1, y_1), \ldots, (x_n, y_n)$

**Formula:**
$$
P(x) = \sum_{i=0}^{n} y_i L_i(x)
$$

where
$$
L_i(x) = \prod_{j=0, j \neq i}^{n} \frac{x - x_j}{x_i - x_j}
$$

**For 3 points (Quadratic):**
$$
P(x) = y_0 \frac{(x-x_1)(x-x_2)}{(x_0-x_1)(x_0-x_2)} + y_1 \frac{(x-x_0)(x-x_2)}{(x_1-x_0)(x_1-x_2)} + y_2 \frac{(x-x_0)(x-x_1)}{(x_2-x_0)(x_2-x_1)}
$$

### 5.3 Newton's Divided Difference

**Forward Difference Formula:**
$$
\Delta y_i = y_{i+1} - y_i
$$

$$
\Delta^2 y_i = \Delta y_{i+1} - \Delta y_i
$$

**Newton's Forward Interpolation:**
$$
y(x) = y_0 + u\Delta y_0 + \frac{u(u-1)}{2!}\Delta^2 y_0 + \frac{u(u-1)(u-2)}{3!}\Delta^3 y_0 + \cdots
$$

where $u = \frac{x - x_0}{h}$

**Use:** When interpolating near the beginning of data

**Newton's Backward Interpolation:**

Use when interpolating near the end of data

---

## 6. Error Analysis

### 6.1 Types of Errors

**1. Round-off Error:** Due to finite precision in computation

**2. Truncation Error:** Due to approximating infinite process with finite steps

**3. Absolute Error:**
$$
E_a = |\text{True Value} - \text{Approximate Value}|
$$

**4. Relative Error:**
$$
E_r = \frac{|\text{True Value} - \text{Approximate Value}|}{|\text{True Value}|} \times 100\%
$$

**5. Percentage Error:**
$$
E_p = E_r \times 100\%
$$

### 6.2 Significant Figures

Number of digits that carry meaningful information

**Example:** 0.00456 has 3 significant figures

### 6.3 Convergence

**Linear Convergence:** Error reduces by constant factor
$$
\frac{|e_{n+1}|}{|e_n|} = C < 1
$$

**Quadratic Convergence:** Error squares each iteration
$$
|e_{n+1}| \propto |e_n|^2
$$

**Examples:**
- Bisection: Linear
- Newton-Raphson: Quadratic
- Secant: Superlinear (~1.618)

---

## 📊 Topic Importance for GATE AG

| Topic | Weightage | Difficulty |
|-------|-----------|------------|
| Root Finding (Newton-Raphson, Bisection) | High | Medium |
| Numerical Integration (Trapezoidal, Simpson's) | Very High | Easy-Medium |
| Numerical Solutions of ODEs (Euler, RK4) | High | Medium |
| Interpolation | Medium | Medium |
| Gaussian Elimination | Medium | Easy-Medium |
| Error Analysis | Low | Easy |

---

## 🎯 Exam Strategy

1. **Master Simpson's 1/3 rule** - Most frequently tested
2. **Practice Newton-Raphson** - Fast and common
3. **Know RK4 formula** - Standard ODE solver
4. **Memorize multipliers** - 1-4-2-4-1 for Simpson's
5. **Understand convergence** - Know which method is fastest
6. **Error formulas** - At least know order of accuracy

---

## 💡 Quick Tips

### For Integration:
- **Trapezoidal:** Pattern 1-2-2-...-2-1, divide by 2
- **Simpson's 1/3:** Pattern 1-4-2-4-...-4-1, divide by 3
- **Simpson's 3/8:** Pattern 1-3-3-1-..., divide by 8, multiply by 3

### For Root Finding:
- **Bisection:** Always converges, but slow
- **Newton-Raphson:** Fast but needs derivative
- **Secant:** Middle ground - no derivative needed

### For ODEs:
- **Euler:** Simple but inaccurate
- **RK4:** Best accuracy, worth memorizing
- Smaller $h$ → more accurate (but more computation)

---

## 📚 Related Topics

- [Differential Equations](../Differential_Equations/)
- [Calculus](../Calculus/)
- [Linear Algebra](../Linear_Algebra/)

---

**Last Updated:** November 2025  
**Version:** 1.0
