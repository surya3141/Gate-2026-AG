# 📐 Calculus - Concepts & Theory

> Comprehensive guide to Calculus for GATE AG

---

## 📚 Table of Contents

1. [Limits](#1-limits)
2. [Continuity](#2-continuity)
3. [Differentiation](#3-differentiation)
4. [Partial Derivatives](#4-partial-derivatives)
5. [Maxima and Minima](#5-maxima-and-minima)
6. [Integration](#6-integration)
7. [Series Expansions](#7-series-expansions)
8. [Applications](#8-applications)

---

## 1. Limits

### 1.1 Definition

The limit of a function $f(x)$ as $x$ approaches $a$ is $L$ if $f(x)$ gets arbitrarily close to $L$ as $x$ gets close to $a$.

$$
\lim_{x \to a} f(x) = L
$$

### 1.2 Basic Limit Properties

$$
\begin{aligned}
&\lim_{x \to a} [f(x) \pm g(x)] = \lim_{x \to a} f(x) \pm \lim_{x \to a} g(x) \\
&\lim_{x \to a} [f(x) \cdot g(x)] = \lim_{x \to a} f(x) \cdot \lim_{x \to a} g(x) \\
&\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{\lim_{x \to a} f(x)}{\lim_{x \to a} g(x)}, \quad \text{if } \lim_{x \to a} g(x) \neq 0 \\
&\lim_{x \to a} [cf(x)] = c \lim_{x \to a} f(x)
\end{aligned}
$$

### 1.3 Standard Limits

#### Fundamental Limits
$$
\begin{aligned}
&\lim_{x \to 0} \frac{\sin x}{x} = 1 \\
&\lim_{x \to 0} \frac{\tan x}{x} = 1 \\
&\lim_{x \to 0} \frac{1 - \cos x}{x} = 0 \\
&\lim_{x \to 0} \frac{e^x - 1}{x} = 1 \\
&\lim_{x \to 0} \frac{\ln(1+x)}{x} = 1 \\
&\lim_{x \to 0} \frac{a^x - 1}{x} = \ln a \\
&\lim_{x \to \infty} \left(1 + \frac{1}{x}\right)^x = e \\
&\lim_{x \to 0} (1 + x)^{1/x} = e
\end{aligned}
$$

#### Exponential Limits
$$
\begin{aligned}
&\lim_{x \to 0} \frac{e^{ax} - 1}{x} = a \\
&\lim_{x \to 0} \frac{e^{ax} - e^{bx}}{x} = a - b
\end{aligned}
$$

### 1.4 Indeterminate Forms

Common forms: $\frac{0}{0}$, $\frac{\infty}{\infty}$, $0 \cdot \infty$, $\infty - \infty$, $0^0$, $1^\infty$, $\infty^0$

**Solution Methods:**
1. **Factorization and simplification**
2. **L'Hôpital's Rule** (for $\frac{0}{0}$ or $\frac{\infty}{\infty}$)
3. **Series expansion**
4. **Standard limit substitution**

---

## 2. Continuity

### 2.1 Definition

A function $f(x)$ is **continuous at $x = a$** if:

$$
\lim_{x \to a} f(x) = f(a)
$$

**Three conditions for continuity:**
1. $f(a)$ exists
2. $\lim_{x \to a} f(x)$ exists
3. $\lim_{x \to a} f(x) = f(a)$

### 2.2 Types of Discontinuity

**1. Removable Discontinuity:** Limit exists but $\lim_{x \to a} f(x) \neq f(a)$

**2. Jump Discontinuity:** Left and right limits exist but are not equal
$$
\lim_{x \to a^-} f(x) \neq \lim_{x \to a^+} f(x)
$$

**3. Infinite Discontinuity:** Function approaches $\pm\infty$

### 2.3 Properties of Continuous Functions

- Sum, difference, product of continuous functions is continuous
- Quotient of continuous functions is continuous (where denominator ≠ 0)
- Composition of continuous functions is continuous

### 2.4 Important Continuous Functions

All polynomial, exponential, logarithmic, trigonometric, and inverse trigonometric functions are continuous in their domains.

---

## 3. Differentiation

### 3.1 Definition

The derivative of $f(x)$ at $x = a$ is:

$$
f'(a) = \lim_{h \to 0} \frac{f(a+h) - f(a)}{h}
$$

**Notations:** $f'(x)$, $\frac{df}{dx}$, $\frac{dy}{dx}$, $Df(x)$

### 3.2 Standard Derivatives

#### Algebraic Functions
$$
\begin{aligned}
&\frac{d}{dx}(c) = 0 \\
&\frac{d}{dx}(x^n) = nx^{n-1} \\
&\frac{d}{dx}(\sqrt{x}) = \frac{1}{2\sqrt{x}} \\
&\frac{d}{dx}\left(\frac{1}{x}\right) = -\frac{1}{x^2}
\end{aligned}
$$

#### Exponential and Logarithmic
$$
\begin{aligned}
&\frac{d}{dx}(e^x) = e^x \\
&\frac{d}{dx}(a^x) = a^x \ln a \\
&\frac{d}{dx}(\ln x) = \frac{1}{x} \\
&\frac{d}{dx}(\log_a x) = \frac{1}{x \ln a}
\end{aligned}
$$

#### Trigonometric Functions
$$
\begin{aligned}
&\frac{d}{dx}(\sin x) = \cos x \\
&\frac{d}{dx}(\cos x) = -\sin x \\
&\frac{d}{dx}(\tan x) = \sec^2 x \\
&\frac{d}{dx}(\cot x) = -\csc^2 x \\
&\frac{d}{dx}(\sec x) = \sec x \tan x \\
&\frac{d}{dx}(\csc x) = -\csc x \cot x
\end{aligned}
$$

#### Inverse Trigonometric Functions
$$
\begin{aligned}
&\frac{d}{dx}(\sin^{-1} x) = \frac{1}{\sqrt{1-x^2}} \\
&\frac{d}{dx}(\cos^{-1} x) = -\frac{1}{\sqrt{1-x^2}} \\
&\frac{d}{dx}(\tan^{-1} x) = \frac{1}{1+x^2} \\
&\frac{d}{dx}(\cot^{-1} x) = -\frac{1}{1+x^2} \\
&\frac{d}{dx}(\sec^{-1} x) = \frac{1}{|x|\sqrt{x^2-1}} \\
&\frac{d}{dx}(\csc^{-1} x) = -\frac{1}{|x|\sqrt{x^2-1}}
\end{aligned}
$$

### 3.3 Differentiation Rules

#### Sum/Difference Rule
$$
\frac{d}{dx}[f(x) \pm g(x)] = f'(x) \pm g'(x)
$$

#### Product Rule
$$
\frac{d}{dx}[f(x) \cdot g(x)] = f'(x)g(x) + f(x)g'(x)
$$

#### Quotient Rule
$$
\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{f'(x)g(x) - f(x)g'(x)}{[g(x)]^2}
$$

#### Chain Rule
$$
\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)
$$

### 3.4 Implicit Differentiation

For equations in the form $F(x, y) = 0$:

$$
\frac{dy}{dx} = -\frac{\frac{\partial F}{\partial x}}{\frac{\partial F}{\partial y}}
$$

**Example:** For $x^2 + y^2 = 25$

$$
2x + 2y\frac{dy}{dx} = 0 \implies \frac{dy}{dx} = -\frac{x}{y}
$$

### 3.5 Logarithmic Differentiation

Useful for functions of the form $y = [f(x)]^{g(x)}$

**Steps:**
1. Take $\ln$ on both sides: $\ln y = g(x) \ln f(x)$
2. Differentiate both sides
3. Solve for $\frac{dy}{dx}$

**Example:** $y = x^x$

$$
\ln y = x \ln x \implies \frac{1}{y}\frac{dy}{dx} = \ln x + 1 \implies \frac{dy}{dx} = x^x(\ln x + 1)
$$

---

## 4. Partial Derivatives

### 4.1 Definition

For a function $f(x, y)$ of two variables:

**Partial derivative with respect to $x$:**
$$
\frac{\partial f}{\partial x} = \lim_{h \to 0} \frac{f(x+h, y) - f(x, y)}{h}
$$

**Partial derivative with respect to $y$:**
$$
\frac{\partial f}{\partial y} = \lim_{h \to 0} \frac{f(x, y+h) - f(x, y)}{h}
$$

**Notation:** $\frac{\partial f}{\partial x}$, $f_x$, $\partial_x f$

### 4.2 Higher Order Partial Derivatives

$$
\begin{aligned}
&\frac{\partial^2 f}{\partial x^2} = f_{xx} = \text{second partial w.r.t. } x \\
&\frac{\partial^2 f}{\partial y^2} = f_{yy} = \text{second partial w.r.t. } y \\
&\frac{\partial^2 f}{\partial x \partial y} = f_{xy} = \text{mixed partial}
\end{aligned}
$$

**Schwarz's Theorem (Clairaut's Theorem):**
If mixed partials are continuous, then:
$$
f_{xy} = f_{yx}
$$

### 4.3 Total Derivative

For $z = f(x, y)$ where $x = x(t)$ and $y = y(t)$:

$$
\frac{dz}{dt} = \frac{\partial f}{\partial x}\frac{dx}{dt} + \frac{\partial f}{\partial y}\frac{dy}{dt}
$$

---

## 5. Maxima and Minima

### 5.1 Critical Points

A point $x = c$ is a **critical point** if:
$$
f'(c) = 0 \quad \text{or} \quad f'(c) \text{ does not exist}
$$

### 5.2 First Derivative Test

For critical point $x = c$:

| $f'(x)$ behavior | Type |
|------------------|------|
| $f'(x)$ changes from $+$ to $-$ | **Local Maximum** |
| $f'(x)$ changes from $-$ to $+$ | **Local Minimum** |
| $f'(x)$ does not change sign | **Neither** (inflection point) |

### 5.3 Second Derivative Test

For critical point $x = c$ where $f'(c) = 0$:

$$
\begin{cases}
f''(c) > 0 & \implies \text{Local Minimum} \\
f''(c) < 0 & \implies \text{Local Maximum} \\
f''(c) = 0 & \implies \text{Test is inconclusive}
\end{cases}
$$

### 5.4 Maxima/Minima for Functions of Two Variables

For $f(x, y)$, critical points satisfy:
$$
\frac{\partial f}{\partial x} = 0 \quad \text{and} \quad \frac{\partial f}{\partial y} = 0
$$

**Second Derivative Test:**

Calculate the discriminant:
$$
D = f_{xx} f_{yy} - (f_{xy})^2
$$

At critical point $(a, b)$:

$$
\begin{cases}
D > 0 \text{ and } f_{xx} > 0 & \implies \text{Local Minimum} \\
D > 0 \text{ and } f_{xx} < 0 & \implies \text{Local Maximum} \\
D < 0 & \implies \text{Saddle Point} \\
D = 0 & \implies \text{Test is inconclusive}
\end{cases}
$$

---

## 6. Integration

### 6.1 Definition

Integration is the reverse process of differentiation.

$$
\int f(x) \, dx = F(x) + C \quad \text{where } F'(x) = f(x)
$$

### 6.2 Standard Integrals

#### Basic Forms
$$
\begin{aligned}
&\int x^n \, dx = \frac{x^{n+1}}{n+1} + C, \quad n \neq -1 \\
&\int \frac{1}{x} \, dx = \ln|x| + C \\
&\int e^x \, dx = e^x + C \\
&\int a^x \, dx = \frac{a^x}{\ln a} + C \\
&\int \frac{1}{x^2 + a^2} \, dx = \frac{1}{a}\tan^{-1}\left(\frac{x}{a}\right) + C \\
&\int \frac{1}{\sqrt{a^2 - x^2}} \, dx = \sin^{-1}\left(\frac{x}{a}\right) + C \\
&\int \frac{1}{x\sqrt{x^2 - a^2}} \, dx = \frac{1}{a}\sec^{-1}\left(\frac{x}{a}\right) + C
\end{aligned}
$$

#### Trigonometric Integrals
$$
\begin{aligned}
&\int \sin x \, dx = -\cos x + C \\
&\int \cos x \, dx = \sin x + C \\
&\int \tan x \, dx = -\ln|\cos x| + C = \ln|\sec x| + C \\
&\int \cot x \, dx = \ln|\sin x| + C \\
&\int \sec x \, dx = \ln|\sec x + \tan x| + C \\
&\int \csc x \, dx = -\ln|\csc x + \cot x| + C \\
&\int \sec^2 x \, dx = \tan x + C \\
&\int \csc^2 x \, dx = -\cot x + C
\end{aligned}
$$

### 6.3 Integration Techniques

#### Substitution Method
For $\int f(g(x))g'(x) \, dx$, substitute $u = g(x)$

#### Integration by Parts
$$
\int u \, dv = uv - \int v \, du
$$

**ILATE Rule** (priority for choosing $u$):
- **I**nverse trigonometric
- **L**ogarithmic
- **A**lgebraic
- **T**rigonometric
- **E**xponential

#### Partial Fractions
Decompose rational functions into simpler fractions.

### 6.4 Definite Integration

$$
\int_a^b f(x) \, dx = F(b) - F(a)
$$

**Properties:**
$$
\begin{aligned}
&\int_a^b f(x) \, dx = -\int_b^a f(x) \, dx \\
&\int_a^b f(x) \, dx = \int_a^c f(x) \, dx + \int_c^b f(x) \, dx \\
&\int_0^a f(x) \, dx = \int_0^a f(a-x) \, dx \\
&\int_{-a}^a f(x) \, dx = \begin{cases} 2\int_0^a f(x) \, dx & \text{if } f(-x) = f(x) \\ 0 & \text{if } f(-x) = -f(x) \end{cases}
\end{aligned}
$$

---

## 7. Series Expansions

### 7.1 Taylor Series

For function $f(x)$ about $x = a$:

$$
f(x) = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 + \frac{f'''(a)}{3!}(x-a)^3 + \cdots
$$

### 7.2 Maclaurin Series (Taylor series at $a = 0$)

$$
f(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \frac{f'''(0)}{3!}x^3 + \cdots
$$

### 7.3 Important Series Expansions

$$
\begin{aligned}
e^x &= 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots = \sum_{n=0}^{\infty} \frac{x^n}{n!} \\
\sin x &= x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \cdots = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{(2n+1)!} \\
\cos x &= 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \cdots = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n}}{(2n)!} \\
\ln(1+x) &= x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \cdots, \quad |x| < 1 \\
(1+x)^n &= 1 + nx + \frac{n(n-1)}{2!}x^2 + \frac{n(n-1)(n-2)}{3!}x^3 + \cdots \\
\tan^{-1} x &= x - \frac{x^3}{3} + \frac{x^5}{5} - \frac{x^7}{7} + \cdots, \quad |x| \leq 1 \\
\frac{1}{1-x} &= 1 + x + x^2 + x^3 + \cdots, \quad |x| < 1
\end{aligned}
$$

---

## 8. Applications

### 8.1 Rate of Change

The derivative represents the instantaneous rate of change:
$$
\text{Rate} = \frac{dy}{dx}
$$

### 8.2 Tangent and Normal

**Equation of tangent at $(x_0, y_0)$:**
$$
y - y_0 = f'(x_0)(x - x_0)
$$

**Equation of normal at $(x_0, y_0)$:**
$$
y - y_0 = -\frac{1}{f'(x_0)}(x - x_0)
$$

### 8.3 Area Under Curve

Area between $y = f(x)$, $x$-axis, and lines $x = a$ and $x = b$:
$$
A = \int_a^b f(x) \, dx
$$

### 8.4 Mean Value Theorem

If $f(x)$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists $c \in (a, b)$ such that:
$$
f'(c) = \frac{f(b) - f(a)}{b - a}
$$

### 8.5 Rolle's Theorem

If $f(x)$ is continuous on $[a, b]$, differentiable on $(a, b)$, and $f(a) = f(b)$, then there exists $c \in (a, b)$ such that:
$$
f'(c) = 0
$$

---

## 📊 Topic Importance for GATE AG

| Topic | Weightage | Difficulty |
|-------|-----------|------------|
| Limits & Continuity | Medium | Easy-Medium |
| Differentiation | High | Easy-Medium |
| Maxima/Minima | High | Medium-Hard |
| Partial Derivatives | Medium | Medium |
| Integration | Medium | Medium |
| Series Expansion | Low-Medium | Medium |

---

## 🎯 Exam Strategy

1. **Master standard formulas** - Most questions are direct applications
2. **Practice L'Hôpital's Rule** - Commonly tested for limits
3. **Focus on maxima/minima** - High weightage topic
4. **Remember trigonometric identities** - Helpful in integration
5. **Practice partial derivatives** - Often combined with optimization

---

## 📚 Related Topics

- [Differential Equations](../Differential_Equations/)
- [Vector Calculus](../Vector_Calculus/)
- [Numerical Methods](../Numerical_Methods/)

---

**Last Updated:** November 2025  
**Version:** 1.0
