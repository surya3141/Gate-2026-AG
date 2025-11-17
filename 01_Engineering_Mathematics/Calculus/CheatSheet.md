# 📋 Calculus - Cheat Sheet

> Quick reference formulas, shortcuts, and tips for GATE AG

---

## 🎯 Quick Formula Reference

### 1. Standard Limits

#### Fundamental Limits (⭐ Most Important!)
$$
\begin{aligned}
&\lim_{x \to 0} \frac{\sin x}{x} = 1 \\
&\lim_{x \to 0} \frac{\tan x}{x} = 1 \\
&\lim_{x \to 0} \frac{1 - \cos x}{x^2} = \frac{1}{2} \\
&\lim_{x \to 0} \frac{e^x - 1}{x} = 1 \\
&\lim_{x \to 0} \frac{\ln(1+x)}{x} = 1 \\
&\lim_{x \to 0} \frac{a^x - 1}{x} = \ln a \\
&\lim_{x \to \infty} \left(1 + \frac{1}{x}\right)^x = e \\
&\lim_{x \to 0} (1 + x)^{1/x} = e
\end{aligned}
$$

**Memory Trick:** For $\frac{\sin(ax)}{x}$ type: answer = $a$

#### Generalized Forms
$$
\begin{aligned}
&\lim_{x \to 0} \frac{\sin(ax)}{x} = a \\
&\lim_{x \to 0} \frac{\tan(ax)}{x} = a \\
&\lim_{x \to 0} \frac{e^{ax} - 1}{x} = a \\
&\lim_{x \to 0} \frac{\ln(1+ax)}{x} = a \\
&\lim_{x \to 0} \frac{(1+x)^n - 1}{x} = n
\end{aligned}
$$

---

### 2. Derivatives

#### Basic Functions
| Function | Derivative |
|----------|------------|
| $c$ (constant) | $0$ |
| $x^n$ | $nx^{n-1}$ |
| $\sqrt{x}$ | $\frac{1}{2\sqrt{x}}$ |
| $\frac{1}{x}$ | $-\frac{1}{x^2}$ |
| $e^x$ | $e^x$ |
| $a^x$ | $a^x \ln a$ |
| $\ln x$ | $\frac{1}{x}$ |
| $\log_a x$ | $\frac{1}{x \ln a}$ |

#### Trigonometric Functions
| Function | Derivative | Memory Trick |
|----------|------------|--------------|
| $\sin x$ | $\cos x$ | ✓ |
| $\cos x$ | $-\sin x$ | Negative! |
| $\tan x$ | $\sec^2 x$ | ✓ |
| $\cot x$ | $-\csc^2 x$ | Negative! |
| $\sec x$ | $\sec x \tan x$ | ✓ |
| $\csc x$ | $-\csc x \cot x$ | Negative! |

**Pattern:** Co-functions (cos, cot, csc) have **negative** derivatives!

#### Inverse Trigonometric Functions
| Function | Derivative |
|----------|------------|
| $\sin^{-1} x$ | $\frac{1}{\sqrt{1-x^2}}$ |
| $\cos^{-1} x$ | $-\frac{1}{\sqrt{1-x^2}}$ |
| $\tan^{-1} x$ | $\frac{1}{1+x^2}$ |
| $\cot^{-1} x$ | $-\frac{1}{1+x^2}$ |
| $\sec^{-1} x$ | $\frac{1}{\|x\|\sqrt{x^2-1}}$ |
| $\csc^{-1} x$ | $-\frac{1}{\|x\|\sqrt{x^2-1}}$ |

**Pattern:** Inverse co-functions have **negative** derivatives!

---

### 3. Differentiation Rules

#### Product Rule
$$
(uv)' = u'v + uv'
$$

**Memory:** "First times derivative of second, plus second times derivative of first"

#### Quotient Rule
$$
\left(\frac{u}{v}\right)' = \frac{u'v - uv'}{v^2}
$$

**Memory:** "lo-d-hi minus hi-d-lo, over lo-lo" (low·dhigh - high·dlow, over low²)

#### Chain Rule
$$
\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)
$$

**Memory:** "Derivative of outer × derivative of inner"

#### Power Chain Rule
$$
\frac{d}{dx}[f(x)]^n = n[f(x)]^{n-1} \cdot f'(x)
$$

---

### 4. Integration Formulas

#### Basic Integrals (⭐ Must Memorize!)
$$
\begin{aligned}
&\int x^n \, dx = \frac{x^{n+1}}{n+1} + C \quad (n \neq -1) \\
&\int \frac{1}{x} \, dx = \ln|x| + C \\
&\int e^x \, dx = e^x + C \\
&\int a^x \, dx = \frac{a^x}{\ln a} + C \\
&\int \sin x \, dx = -\cos x + C \\
&\int \cos x \, dx = \sin x + C \\
&\int \sec^2 x \, dx = \tan x + C \\
&\int \csc^2 x \, dx = -\cot x + C \\
&\int \sec x \tan x \, dx = \sec x + C \\
&\int \csc x \cot x \, dx = -\csc x + C
\end{aligned}
$$

#### Advanced Integrals
$$
\begin{aligned}
&\int \tan x \, dx = \ln|\sec x| + C = -\ln|\cos x| + C \\
&\int \cot x \, dx = \ln|\sin x| + C \\
&\int \sec x \, dx = \ln|\sec x + \tan x| + C \\
&\int \csc x \, dx = -\ln|\csc x + \cot x| + C
\end{aligned}
$$

#### Inverse Trigonometric Forms
$$
\begin{aligned}
&\int \frac{1}{x^2 + a^2} \, dx = \frac{1}{a}\tan^{-1}\left(\frac{x}{a}\right) + C \\
&\int \frac{1}{\sqrt{a^2 - x^2}} \, dx = \sin^{-1}\left(\frac{x}{a}\right) + C \\
&\int \frac{1}{x\sqrt{x^2 - a^2}} \, dx = \frac{1}{a}\sec^{-1}\left(\frac{x}{a}\right) + C
\end{aligned}
$$

---

### 5. Integration Techniques

#### ILATE Rule (Integration by Parts)

**Priority for choosing $u$:**
```
I - Inverse trigonometric (sin⁻¹x, tan⁻¹x, etc.)
L - Logarithmic (ln x, log x)
A - Algebraic (x, x², polynomials)
T - Trigonometric (sin x, cos x, tan x)
E - Exponential (eˣ, aˣ)
```

**Formula:**
$$
\int u \, dv = uv - \int v \, du
$$

**Example:** For $\int x \sin x \, dx$
- Choose $u = x$ (Algebraic) and $dv = \sin x \, dx$ (Trigonometric)

#### Substitution Method

**When to use:**
- Function is composite: $f(g(x)) \cdot g'(x)$
- Rational functions with square roots
- Trigonometric substitutions

**Common Substitutions:**
| Expression | Substitution |
|------------|--------------|
| $\sqrt{a^2 - x^2}$ | $x = a\sin\theta$ |
| $\sqrt{a^2 + x^2}$ | $x = a\tan\theta$ |
| $\sqrt{x^2 - a^2}$ | $x = a\sec\theta$ |

---

### 6. Definite Integration Properties

#### Fundamental Properties
$$
\begin{aligned}
&\int_a^b f(x) \, dx = F(b) - F(a) \\
&\int_a^b f(x) \, dx = -\int_b^a f(x) \, dx \\
&\int_a^b f(x) \, dx = \int_a^c f(x) \, dx + \int_c^b f(x) \, dx
\end{aligned}
$$

#### Symmetry Properties (⭐ Time Saver!)

**For symmetric limits $[-a, a]$:**

$$
\int_{-a}^a f(x) \, dx = \begin{cases} 
2\int_0^a f(x) \, dx & \text{if } f(-x) = f(x) \text{ (even)} \\
0 & \text{if } f(-x) = -f(x) \text{ (odd)}
\end{cases}
$$

**Quick Check:**
- **Even:** $x^2, x^4, \cos x, |x|$ → Integrate from $0$ to $a$ and multiply by 2
- **Odd:** $x, x^3, \sin x, \tan x$ → Answer = 0

#### King's Rule
$$
\int_0^a f(x) \, dx = \int_0^a f(a-x) \, dx
$$

**Application:** Useful when substitution $x \to a-x$ simplifies the integral

---

### 7. Series Expansions (Maclaurin)

#### Most Important Series (⭐ Memorize!)

**Exponential:**
$$
e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \cdots
$$

**Sine:**
$$
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \cdots
$$

**Cosine:**
$$
\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \cdots
$$

**Natural Logarithm:**
$$
\ln(1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \cdots, \quad |x| < 1
$$

**Binomial:**
$$
(1+x)^n = 1 + nx + \frac{n(n-1)}{2!}x^2 + \frac{n(n-1)(n-2)}{3!}x^3 + \cdots
$$

**Geometric:**
$$
\frac{1}{1-x} = 1 + x + x^2 + x^3 + \cdots, \quad |x| < 1
$$

**Inverse Tangent:**
$$
\tan^{-1} x = x - \frac{x^3}{3} + \frac{x^5}{5} - \frac{x^7}{7} + \cdots, \quad |x| \leq 1
$$

---

### 8. Maxima and Minima

#### Single Variable

**Critical Points:** Solve $f'(x) = 0$

**Second Derivative Test:**
$$
\begin{cases}
f''(c) > 0 & \implies \text{Local Minimum at } x = c \\
f''(c) < 0 & \implies \text{Local Maximum at } x = c \\
f''(c) = 0 & \implies \text{Test inconclusive}
\end{cases}
$$

**Memory:** Positive → Bowl shape → Minimum ⌣  
Negative → Hill shape → Maximum ⌢

#### Two Variables

**Critical Points:** Solve simultaneously
$$
\frac{\partial f}{\partial x} = 0 \quad \text{and} \quad \frac{\partial f}{\partial y} = 0
$$

**Discriminant Test:**
$$
D = f_{xx} \cdot f_{yy} - (f_{xy})^2
$$

**Classification:**
| Condition | Nature |
|-----------|--------|
| $D > 0$ and $f_{xx} > 0$ | **Local Minimum** |
| $D > 0$ and $f_{xx} < 0$ | **Local Maximum** |
| $D < 0$ | **Saddle Point** |
| $D = 0$ | **Inconclusive** |

---

### 9. Partial Derivatives

#### Basic Notation
$$
\frac{\partial f}{\partial x} = f_x, \quad \frac{\partial f}{\partial y} = f_y
$$

#### Mixed Partials (Clairaut's Theorem)
If continuous:
$$
f_{xy} = f_{yx}
$$

**What it means:** Order of differentiation doesn't matter!

#### Total Derivative
For $z = f(x, y)$ where $x = x(t)$, $y = y(t)$:
$$
\frac{dz}{dt} = \frac{\partial f}{\partial x}\frac{dx}{dt} + \frac{\partial f}{\partial y}\frac{dy}{dt}
$$

---

## ⚡ Quick Solution Methods

### L'Hôpital's Rule

**For indeterminate forms:** $\frac{0}{0}$ or $\frac{\infty}{\infty}$

$$
\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}
$$

**Steps:**
1. Check if form is $\frac{0}{0}$ or $\frac{\infty}{\infty}$
2. Differentiate numerator and denominator separately
3. Evaluate the new limit
4. Repeat if still indeterminate

**⚠️ Common Mistake:** Don't use quotient rule! Differentiate top and bottom separately.

---

### Implicit Differentiation Quick Formula

For $F(x, y) = 0$:
$$
\frac{dy}{dx} = -\frac{F_x}{F_y} = -\frac{\partial F/\partial x}{\partial F/\partial y}
$$

**Example:** For $x^2 + y^2 = 25$
$$
\frac{dy}{dx} = -\frac{2x}{2y} = -\frac{x}{y}
$$

---

### Logarithmic Differentiation Shortcut

**For:** $y = [f(x)]^{g(x)}$

**Formula:**
$$
\frac{dy}{dx} = y \left[g'(x)\ln f(x) + g(x)\frac{f'(x)}{f(x)}\right]
$$

**Special Case:** $y = x^x$
$$
\frac{d}{dx}(x^x) = x^x(\ln x + 1)
$$

---

## 🎯 GATE-Specific Shortcuts

### 1. Quick Limit Checks

**Polynomial Limits at Infinity:**
$$
\lim_{x \to \infty} \frac{a_nx^n + \cdots}{b_mx^m + \cdots} = \begin{cases}
\frac{a_n}{b_m} & \text{if } n = m \\
0 & \text{if } n < m \\
\pm\infty & \text{if } n > m
\end{cases}
$$

### 2. Integration Recognition

| If you see... | Think... |
|---------------|----------|
| $\frac{f'(x)}{f(x)}$ | $\ln\|f(x)\| + C$ |
| $f'(x) \cdot [f(x)]^n$ | $\frac{[f(x)]^{n+1}}{n+1} + C$ |
| $f'(x) \cdot e^{f(x)}$ | $e^{f(x)} + C$ |
| Product of algebraic and trig/exp | Integration by parts |

### 3. Maxima/Minima Quick Checks

**For $ax^2 + bx + c$:**
- Maximum at $x = -\frac{b}{2a}$ if $a < 0$
- Minimum at $x = -\frac{b}{2a}$ if $a > 0$

**For $ax^3 + bx^2 + cx + d$:**
- Critical points from $3ax^2 + 2bx + c = 0$ (quadratic formula)

---

## 💡 Problem-Solving Tips

### Tip 1: Continuity Quick Check
For piecewise functions at $x = a$:
1. Calculate $f(a)$ from definition
2. Calculate $\lim_{x \to a} f(x)$
3. If equal → continuous; if not → discontinuous

### Tip 2: Chain Rule Pattern Recognition
$$
\begin{aligned}
&\frac{d}{dx}[\sin^n(x)] = n\sin^{n-1}(x)\cos(x) \\
&\frac{d}{dx}[e^{f(x)}] = e^{f(x)} \cdot f'(x) \\
&\frac{d}{dx}[\ln(f(x))] = \frac{f'(x)}{f(x)}
\end{aligned}
$$

### Tip 3: Integration by Parts - Quick Decision
**Choose $u$ (first in ILATE):**
- $\int x \sin x \, dx$ → $u = x$ (A before T)
- $\int x e^x \, dx$ → $u = x$ (A before E)
- $\int \ln x \, dx$ → $u = \ln x$ (L before everything)
- $\int \tan^{-1} x \, dx$ → $u = \tan^{-1} x$ (I before everything)

### Tip 4: Symmetry Before Calculation
**Always check for odd/even functions in $\int_{-a}^{a}$!**
- Odd → Answer = 0 (5-second problem!)
- Even → Calculate $\int_0^a$ and double it

### Tip 5: Series Approximation
For small $x$:
$$
\begin{aligned}
&e^x \approx 1 + x \\
&\sin x \approx x \\
&\cos x \approx 1 - \frac{x^2}{2} \\
&\ln(1+x) \approx x
\end{aligned}
$$

---

## ⚠️ Common Mistakes to Avoid

### ❌ Mistake 1: L'Hôpital's Rule Misuse
**Wrong:** Apply L'Hôpital when limit is not $\frac{0}{0}$ or $\frac{\infty}{\infty}$  
**Correct:** Check form first!

**Wrong:** $\lim_{x \to 0} \frac{x^2 + x}{x} = \lim_{x \to 0} \frac{2x + 1}{1}$ (unnecessary!)  
**Correct:** Simplify first: $\lim_{x \to 0}(x + 1) = 1$

### ❌ Mistake 2: Chain Rule Forgotten
**Wrong:** $\frac{d}{dx}[\sin(3x)] = \cos(3x)$  
**Correct:** $\frac{d}{dx}[\sin(3x)] = 3\cos(3x)$

### ❌ Mistake 3: Integration by Parts - Wrong Choice of $u$
**Wrong:** For $\int x e^x dx$, choosing $u = e^x$ (makes it harder!)  
**Correct:** Choose $u = x$ (ILATE: A before E)

### ❌ Mistake 4: Forgetting Absolute Value
**Wrong:** $\int \frac{1}{x} dx = \ln x + C$  
**Correct:** $\int \frac{1}{x} dx = \ln|x| + C$

### ❌ Mistake 5: Partial Derivative Confusion
**Wrong:** Treating other variables as constants when they're not  
**Correct:** In $\frac{\partial}{\partial x}(x^2y)$, treat $y$ as constant → $2xy$

### ❌ Mistake 6: Mixing up $\frac{d}{dx}$ and $\frac{\partial}{\partial x}$
- $\frac{d}{dx}$: Total derivative (single variable)
- $\frac{\partial}{\partial x}$: Partial derivative (multivariable)

---

## 📊 Formula Priority List

### ⭐⭐⭐ Must Know (Exam Essential)
1. $\lim_{x \to 0} \frac{\sin x}{x} = 1$ and variants
2. L'Hôpital's Rule
3. Product Rule: $(uv)' = u'v + uv'$
4. Chain Rule: $(f \circ g)' = f' \circ g \cdot g'$
5. $\int x^n dx = \frac{x^{n+1}}{n+1} + C$
6. Integration by parts: $\int u \, dv = uv - \int v \, du$
7. Second derivative test for maxima/minima
8. Odd/Even function integration on $[-a, a]$

### ⭐⭐ Very Important
1. All trigonometric derivatives
2. $e^x$, $\ln x$ derivatives and integrals
3. Standard integration formulas
4. Partial derivative rules
5. Series expansions of $e^x$, $\sin x$, $\cos x$

### ⭐ Good to Know
1. Inverse trig derivatives
2. Complex integration techniques
3. Mixed partial derivatives
4. Taylor/Maclaurin general formula
5. Advanced limit techniques

---

## 🕐 Time Management

| Question Type | Target Time | Strategy |
|---------------|-------------|----------|
| Standard Limit | 30-60 sec | Direct formula |
| L'Hôpital's Rule | 1-2 min | One differentiation usually enough |
| Basic Differentiation | 1-2 min | Apply rules carefully |
| Maxima/Minima (1D) | 2-3 min | Find $f'=0$, test $f''$ |
| Integration (Standard) | 1-2 min | Pattern recognition |
| Integration by Parts | 2-3 min | ILATE, one iteration |
| Partial Derivatives | 2-3 min | Treat other variables as constants |
| Maxima/Minima (2D) | 3-4 min | Find critical points, discriminant |

---

## 🎓 Last-Minute Revision Checklist

**10 minutes before exam:**

✓ $\lim_{x \to 0} \frac{\sin x}{x} = 1$  
✓ L'Hôpital's Rule (for $\frac{0}{0}$, $\frac{\infty}{\infty}$)  
✓ Product Rule & Chain Rule  
✓ $\frac{d}{dx}(e^x) = e^x$, $\frac{d}{dx}(\ln x) = \frac{1}{x}$  
✓ $\frac{d}{dx}(\sin x) = \cos x$, $\frac{d}{dx}(\cos x) = -\sin x$  
✓ ILATE for integration by parts  
✓ $\int \frac{1}{x} dx = \ln|x| + C$  
✓ Odd function on $[-a, a]$ → integral = 0  
✓ Second derivative test: $f'' > 0$ → min, $f'' < 0$ → max  
✓ $e^x = 1 + x + \frac{x^2}{2!} + \cdots$

---

## 🔗 Related Topics

- [Differential Equations](../Differential_Equations/CheatSheet.md)
- [Vector Calculus](../Vector_Calculus/CheatSheet.md)
- [Numerical Methods](../Numerical_Methods/CheatSheet.md)

---

**Last Updated:** November 2025  
**Version:** 1.0

---

*For detailed solutions, refer to [Solutions.md](./Solutions.md)*  
*For concepts and theory, refer to [README.md](./README.md)*
