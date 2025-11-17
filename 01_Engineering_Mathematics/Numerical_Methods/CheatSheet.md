# 📐 Numerical Methods - Quick Reference Cheat Sheet

> Fast formulas, patterns, and shortcuts for GATE AG Numerical Methods

---

## 🎯 Most Important Formulas

### 1. Numerical Integration - The BIG THREE

#### Trapezoidal Rule
$$
\int_a^b f(x)dx \approx \frac{h}{2}[f(x_0) + 2f(x_1) + 2f(x_2) + \cdots + 2f(x_{n-1}) + f(x_n)]
$$

**Pattern:** `1 - 2 - 2 - 2 - ... - 2 - 1` then multiply by $\frac{h}{2}$

**Quick Check:**
- $h = \frac{b-a}{n}$
- Works for any $n$
- Error: $O(h^2)$

---

#### Simpson's 1/3 Rule
$$
\int_a^b f(x)dx \approx \frac{h}{3}[f(x_0) + 4f(x_1) + 2f(x_2) + 4f(x_3) + 2f(x_4) + \cdots + f(x_n)]
$$

**Pattern:** `1 - 4 - 2 - 4 - 2 - ... - 4 - 1` then multiply by $\frac{h}{3}$

**Quick Check:**
- $n$ must be EVEN
- More accurate than Trapezoidal
- Error: $O(h^4)$

**Memory Trick:** "1-4-2 repeats, ends with 4-1"

---

#### Simpson's 3/8 Rule
$$
\int_a^b f(x)dx \approx \frac{3h}{8}[f(x_0) + 3f(x_1) + 3f(x_2) + f(x_3)]
$$

**Pattern:** `1 - 3 - 3 - 1` (for 3 intervals only) then multiply by $\frac{3h}{8}$

**Quick Check:**
- Exactly 3 intervals required
- $h = \frac{b-a}{3}$
- Error: $O(h^4)$ (same as Simpson's 1/3)

---

### 2. Root Finding Methods

#### Bisection Method
$$
c = \frac{a + b}{2}
$$

**Algorithm:**
1. Check: $f(a) \cdot f(b) < 0$ (root exists)
2. Find midpoint: $c = \frac{a+b}{2}$
3. If $f(a) \cdot f(c) < 0$: root in $[a, c]$
4. Else: root in $[c, b]$
5. Repeat

**Convergence:** Linear (error halves each time)

---

#### Newton-Raphson Method
$$
x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}
$$

**Steps:**
1. Calculate $f(x_n)$
2. Calculate $f'(x_n)$
3. Apply formula
4. Repeat until convergence

**Pros:** 
- Very fast (quadratic convergence)
- Usually 3-4 iterations enough

**Cons:** 
- Needs derivative
- Can fail if $f'(x_n) = 0$

---

#### Secant Method
$$
x_{n+1} = x_n - f(x_n) \cdot \frac{x_n - x_{n-1}}{f(x_n) - f(x_{n-1})}
$$

**Alternative form:**
$$
x_{n+1} = \frac{x_{n-1}f(x_n) - x_n f(x_{n-1})}{f(x_n) - f(x_{n-1})}
$$

**Pros:**
- No derivative needed
- Faster than bisection

**Cons:**
- Needs two initial guesses
- Slower than Newton-Raphson

---

### 3. Numerical Solutions of ODEs

#### Euler's Method
$$
y_{n+1} = y_n + h \cdot f(x_n, y_n)
$$

**Steps:**
1. Calculate slope at current point: $f(x_n, y_n)$
2. Move forward: $y_{n+1} = y_n + h \times \text{slope}$
3. Update $x$: $x_{n+1} = x_n + h$

**Accuracy:** $O(h)$ - first order (least accurate)

---

#### Modified Euler (Predictor-Corrector)

**Predictor:**
$$
y_{n+1}^* = y_n + h \cdot f(x_n, y_n)
$$

**Corrector:**
$$
y_{n+1} = y_n + \frac{h}{2}[f(x_n, y_n) + f(x_{n+1}, y_{n+1}^*)]
$$

**Memory:** Average the slopes at start and predicted end

**Accuracy:** $O(h^2)$ - second order

---

#### Runge-Kutta 2nd Order (RK2)
$$
\begin{aligned}
k_1 &= h \cdot f(x_n, y_n) \\
k_2 &= h \cdot f(x_n + h, y_n + k_1) \\
y_{n+1} &= y_n + \frac{1}{2}(k_1 + k_2)
\end{aligned}
$$

**Accuracy:** $O(h^2)$ - second order

---

#### Runge-Kutta 4th Order (RK4) ⭐ MOST IMPORTANT
$$
\begin{aligned}
k_1 &= h \cdot f(x_n, y_n) \\
k_2 &= h \cdot f\left(x_n + \frac{h}{2}, y_n + \frac{k_1}{2}\right) \\
k_3 &= h \cdot f\left(x_n + \frac{h}{2}, y_n + \frac{k_2}{2}\right) \\
k_4 &= h \cdot f(x_n + h, y_n + k_3) \\
y_{n+1} &= y_n + \frac{1}{6}(k_1 + 2k_2 + 2k_3 + k_4)
\end{aligned}
$$

**Memory Trick:** "1-2-2-1 weighted average" for final step

**Accuracy:** $O(h^4)$ - fourth order (very accurate!)

**Steps at:** $0, \frac{h}{2}, \frac{h}{2}, h$

---

### 4. Interpolation

#### Linear Interpolation
$$
y(x) = y_0 + \frac{y_1 - y_0}{x_1 - x_0}(x - x_0)
$$

**For midpoint:** Just average!
$$
y\left(\frac{x_0 + x_1}{2}\right) = \frac{y_0 + y_1}{2}
$$

---

#### Lagrange Interpolation (2 points = Linear)
$$
P(x) = \frac{x - x_1}{x_0 - x_1}y_0 + \frac{x - x_0}{x_1 - x_0}y_1
$$

#### Lagrange Interpolation (3 points = Quadratic)
$$
P(x) = \frac{(x-x_1)(x-x_2)}{(x_0-x_1)(x_0-x_2)}y_0 + \frac{(x-x_0)(x-x_2)}{(x_1-x_0)(x_1-x_2)}y_1 + \frac{(x-x_0)(x-x_1)}{(x_2-x_0)(x_2-x_1)}y_2
$$

**Pattern:** Each term has:
- Numerator: $(x - \text{all other } x_i)$
- Denominator: $(x_k - \text{all other } x_i)$
- Multiply by $y_k$

---

#### Newton's Divided Difference
$$
f[x_0, x_1] = \frac{f(x_1) - f(x_0)}{x_1 - x_0}
$$

$$
f[x_0, x_1, x_2] = \frac{f[x_1, x_2] - f[x_0, x_1]}{x_2 - x_0}
$$

**Polynomial:**
$$
P(x) = f(x_0) + f[x_0,x_1](x-x_0) + f[x_0,x_1,x_2](x-x_0)(x-x_1) + \cdots
$$

---

### 5. Numerical Differentiation

#### Forward Difference
$$
f'(x_0) \approx \frac{f(x_0 + h) - f(x_0)}{h}
$$

#### Backward Difference
$$
f'(x_0) \approx \frac{f(x_0) - f(x_0 - h)}{h}
$$

#### Central Difference (Most Accurate)
$$
f'(x_0) \approx \frac{f(x_0 + h) - f(x_0 - h)}{2h}
$$

**Second Derivative:**
$$
f''(x_0) \approx \frac{f(x_0 + h) - 2f(x_0) + f(x_0 - h)}{h^2}
$$

---

## 📊 Quick Comparison Tables

### Integration Methods

| Method | Intervals | Pattern | Divisor | Error | Exactness |
|--------|-----------|---------|---------|-------|-----------|
| Trapezoidal | Any $n$ | 1-2-2-...-2-1 | $\frac{h}{2}$ | $O(h^2)$ | Degree 1 |
| Simpson's 1/3 | Even $n$ | 1-4-2-4-...-4-1 | $\frac{h}{3}$ | $O(h^4)$ | Degree 3 |
| Simpson's 3/8 | $n = 3$ | 1-3-3-1 | $\frac{3h}{8}$ | $O(h^4)$ | Degree 3 |

**Choose:**
- **Trapezoidal:** Simple, quick, less accurate
- **Simpson's 1/3:** Best for even intervals, high accuracy
- **Simpson's 3/8:** When exactly 3 intervals

---

### Root Finding Methods

| Method | Initial Guess | Derivative? | Convergence | Speed |
|--------|---------------|-------------|-------------|-------|
| Bisection | Interval $[a,b]$ | No | Linear | Slow |
| Newton-Raphson | One point $x_0$ | Yes | Quadratic | Very Fast |
| Secant | Two points | No | Superlinear | Fast |
| Fixed-Point | One point | No | Linear | Slow |

**Choose:**
- **Bisection:** Always works if root exists, but slow
- **Newton-Raphson:** Fastest, but needs derivative
- **Secant:** Good compromise (no derivative, faster than bisection)

---

### ODE Solution Methods

| Method | Steps | Accuracy | Computational Cost |
|--------|-------|----------|-------------------|
| Euler | 1 | $O(h)$ | Very Low |
| Modified Euler | 2 | $O(h^2)$ | Low |
| RK2 | 2 | $O(h^2)$ | Medium |
| RK4 | 4 | $O(h^4)$ | High |

**Choose:**
- **Euler:** Quick estimate, not very accurate
- **Modified Euler/RK2:** Balance of accuracy and speed
- **RK4:** High accuracy needed, worth the extra work

---

## 🚀 Exam Shortcuts & Tricks

### Integration Shortcuts

#### 1. Remember Multipliers
- **Trapezoidal:** Ends with 1, middles with 2
- **Simpson's 1/3:** Starts 1, alternates 4-2-4-2..., ends 4-1
- **Simpson's 3/8:** Just 1-3-3-1

#### 2. Quick h Calculation
$$
h = \frac{b - a}{n}
$$

**Example:** $\int_0^4$ with $n=4$ → $h = \frac{4-0}{4} = 1$

#### 3. Check Your n
- Simpson's 1/3 **NEEDS EVEN** $n$
- Trapezoidal works for any $n$
- Simpson's 3/8 needs $n=3$

---

### Newton-Raphson Shortcut

**For common functions:**

| $f(x)$ | $f'(x)$ | Formula |
|--------|---------|---------|
| $x^2 - a$ | $2x$ | $x_{n+1} = \frac{x_n + \frac{a}{x_n}}{2}$ (√a) |
| $x^3 - a$ | $3x^2$ | $x_{n+1} = \frac{2x_n + \frac{a}{x_n^2}}{3}$ (∛a) |
| $e^x - a$ | $e^x$ | $x_{n+1} = x_n - 1 + \frac{a}{e^{x_n}}$ |

---

### RK4 Memory Device

**The "Half-Half-Full" Pattern:**
- $k_1$: Start (0, full)
- $k_2$: Half step, half increment
- $k_3$: Half step, half increment (using $k_2$)
- $k_4$: Full step, full increment (using $k_3$)

**Final:** $\frac{1}{6}(k_1 + 2k_2 + 2k_3 + k_4)$ → Think "1-2-2-1"

---

### Error Analysis Quick Guide

| Method | Local Error | Global Error |
|--------|-------------|--------------|
| Trapezoidal | $O(h^3)$ | $O(h^2)$ |
| Simpson's 1/3 | $O(h^5)$ | $O(h^4)$ |
| Euler | $O(h^2)$ | $O(h)$ |
| RK4 | $O(h^5)$ | $O(h^4)$ |

**Rule:** Global error = Local error - 1 power of $h$

---

## ⚠️ Common Mistakes to Avoid

### 1. Integration Mistakes

❌ **Wrong:** Using Simpson's 1/3 with odd $n$
✅ **Correct:** Check $n$ is even first!

❌ **Wrong:** Forgetting the divisor (h/2, h/3, 3h/8)
✅ **Correct:** Pattern × Divisor = Answer

❌ **Wrong:** Pattern 1-2-4-2-4-1 for Simpson's
✅ **Correct:** Pattern 1-4-2-4-2-4-1

### 2. Root Finding Mistakes

❌ **Wrong:** Newton-Raphson without checking $f'(x_n) \neq 0$
✅ **Correct:** Always verify derivative isn't zero

❌ **Wrong:** Bisection without checking sign change
✅ **Correct:** Must have $f(a) \cdot f(b) < 0$

### 3. ODE Mistakes

❌ **Wrong:** Mixing up $k_1, k_2, k_3, k_4$ in RK4
✅ **Correct:** Follow the half-step pattern carefully

❌ **Wrong:** Forgetting to update $x_n$ in Euler
✅ **Correct:** $x_{n+1} = x_n + h$, $y_{n+1} = y_n + h \cdot f(x_n, y_n)$

---

## 🎯 Last-Minute Revision (5 minutes before exam)

### Must Remember Formulas

1. **Trapezoidal:** 
   $$\frac{h}{2}[\text{first} + \text{last} + 2(\text{all middles})]$$

2. **Simpson's 1/3:** 
   $$\frac{h}{3}[1\cdot f_0 + 4\cdot f_1 + 2\cdot f_2 + 4\cdot f_3 + \cdots + 1\cdot f_n]$$

3. **Newton-Raphson:** 
   $$x_{\text{new}} = x_{\text{old}} - \frac{f}{f'}$$

4. **Euler:** 
   $$y_{\text{new}} = y_{\text{old}} + h \times \text{slope}$$

5. **RK4 Final Step:** 
   $$y_{\text{new}} = y_{\text{old}} + \frac{1}{6}(k_1 + 2k_2 + 2k_3 + k_4)$$

### Key Concepts
- Simpson's needs **even** $n$
- Newton-Raphson is **fastest** (quadratic convergence)
- RK4 is **most accurate** for ODEs
- Central difference is **most accurate** for derivatives

---

## 📱 Mobile-Friendly Quick Reference

### Integration Patterns (memorize these!)

```
Trapezoidal:  1 - 2 - 2 - 2 - ... - 2 - 1   ÷ 2
Simpson 1/3:  1 - 4 - 2 - 4 - 2 - 4 - 1   ÷ 3
Simpson 3/8:  1 - 3 - 3 - 1               × 3 ÷ 8
```

### Root Finding (which to use?)

```
Given: Interval [a,b]          → Bisection
Given: Derivative available    → Newton-Raphson  
Given: No derivative          → Secant
Given: Need guaranteed result → Bisection
```

### ODE Methods (accuracy ranking)

```
Euler          O(h)    ⭐
Modified Euler O(h²)   ⭐⭐
RK2            O(h²)   ⭐⭐
RK4            O(h⁴)   ⭐⭐⭐⭐⭐
```

---

## 💪 Practice Problem Templates

### Template 1: Integration with Trapezoidal

**Given:** $\int_a^b f(x)dx$, $n$ intervals

**Steps:**
1. Calculate $h = \frac{b-a}{n}$
2. List points: $x_0, x_1, x_2, \ldots, x_n$
3. Calculate $f(x_i)$ for each point
4. Apply: $\frac{h}{2}[f_0 + 2f_1 + 2f_2 + \cdots + 2f_{n-1} + f_n]$

**Time:** 2-3 minutes

---

### Template 2: Newton-Raphson

**Given:** $f(x) = 0$, initial guess $x_0$

**Steps:**
1. Find $f'(x)$ (derivative)
2. Calculate $f(x_0)$ and $f'(x_0)$
3. Apply: $x_1 = x_0 - \frac{f(x_0)}{f'(x_0)}$
4. Repeat if needed

**Time:** 1-2 minutes per iteration

---

### Template 3: Euler's Method

**Given:** $\frac{dy}{dx} = f(x,y)$, $y(x_0) = y_0$, find $y(x_0 + h)$

**Steps:**
1. Calculate slope: $m = f(x_0, y_0)$
2. Move forward: $y_1 = y_0 + h \cdot m$
3. Update: $x_1 = x_0 + h$

**Time:** 1 minute per step

---

### Template 4: RK4 Method

**Given:** $\frac{dy}{dx} = f(x,y)$, $y(x_0) = y_0$, step $h$

**Steps:**
1. $k_1 = h \cdot f(x_0, y_0)$
2. $k_2 = h \cdot f(x_0 + \frac{h}{2}, y_0 + \frac{k_1}{2})$
3. $k_3 = h \cdot f(x_0 + \frac{h}{2}, y_0 + \frac{k_2}{2})$
4. $k_4 = h \cdot f(x_0 + h, y_0 + k_3)$
5. $y_1 = y_0 + \frac{1}{6}(k_1 + 2k_2 + 2k_3 + k_4)$

**Time:** 3-4 minutes

---

## 🔥 High-Yield Topics for GATE AG

### Must Know (appear almost every year)

1. ⭐⭐⭐ **Simpson's 1/3 Rule** - Direct calculation questions
2. ⭐⭐⭐ **Trapezoidal Rule** - Comparison with exact value
3. ⭐⭐⭐ **Newton-Raphson Method** - One or two iterations
4. ⭐⭐⭐ **Euler's Method** - First step calculation
5. ⭐⭐ **RK4 Method** - $k_1, k_2$ calculation

### Good to Know (appear frequently)

6. ⭐⭐ **Bisection Method** - Finding intervals
7. ⭐⭐ **Modified Euler** - Predictor-corrector
8. ⭐⭐ **Error Analysis** - Order of accuracy
9. ⭐ **Simpson's 3/8 Rule** - Specific applications
10. ⭐ **Secant Method** - Alternative to Newton

### Less Common (but possible)

- Lagrange Interpolation
- Numerical Differentiation
- Convergence Analysis
- Gaussian Elimination

---

## 📌 Formula Summary Card (Print & Keep!)

```
┌─────────────────────────────────────────────────────────┐
│          NUMERICAL METHODS - FORMULA CARD               │
├─────────────────────────────────────────────────────────┤
│                                                         │
│ INTEGRATION:                                            │
│   Trapezoidal:  (h/2)[1-2-2-...-2-1]                   │
│   Simpson 1/3:  (h/3)[1-4-2-4-...-4-1]  (n even!)      │
│   Simpson 3/8:  (3h/8)[1-3-3-1]                        │
│                                                         │
│ ROOT FINDING:                                           │
│   Bisection:     c = (a+b)/2                           │
│   Newton:        x₁ = x₀ - f/f'                        │
│   Secant:        x₁ = x₀ - f₀(x₀-x₋₁)/(f₀-f₋₁)        │
│                                                         │
│ ODEs:                                                   │
│   Euler:         y₁ = y₀ + h·f(x₀,y₀)                  │
│   RK4 Final:     y₁ = y₀ + (k₁+2k₂+2k₃+k₄)/6          │
│                                                         │
│ REMEMBER:                                               │
│   • Simpson 1/3 needs EVEN n                           │
│   • Central diff most accurate                         │
│   • RK4 pattern: 0, h/2, h/2, h                       │
│   • Newton fastest, Bisection most reliable            │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

---

## 🎓 Pro Tips from Toppers

### Time Management
- **Integration problems:** 2 minutes max
- **Root finding (1 iteration):** 1-2 minutes
- **Euler (1 step):** 1 minute
- **RK4 (complete):** 3-4 minutes

### Strategy
1. **Read carefully:** Is $n$ even for Simpson's?
2. **Write patterns:** Don't calculate in your head
3. **Check units:** $h$ value correct?
4. **Verify signs:** Important for bisection

### Common Traps
- ❌ Using degree symbol instead of radian in trig
- ❌ Forgetting negative signs
- ❌ Arithmetic errors (use calculator!)
- ❌ Wrong convergence criteria

---

## 📖 Related Cheat Sheets

- [Calculus Cheat Sheet](../Calculus/CheatSheet.md)
- [Differential Equations Cheat Sheet](../Differential_Equations/CheatSheet.md)
- [Linear Algebra Cheat Sheet](../Linear_Algebra/CheatSheet.md)

---

**Last Updated:** November 2025  
**Version:** 1.0

---

*For detailed explanations, see [Numerical Methods README](./README.md)*  
*For practice problems, see [Numerical Methods PYQ Solutions](./Solutions.md)*

---

## ✅ Pre-Exam Checklist

**One day before exam:**
- [ ] Review all integration patterns
- [ ] Practice 3 problems of each type
- [ ] Memorize RK4 formula
- [ ] Quick revision of error orders

**Morning of exam:**
- [ ] Review this cheat sheet (10 minutes)
- [ ] Practice one integration problem
- [ ] Practice one Newton-Raphson problem
- [ ] Review common mistakes section

**Good luck! You've got this! 🚀**
