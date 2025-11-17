# 📊 Probability and Statistics - Quick Reference Cheat Sheet

> Fast formulas, shortcuts, and memory tricks for GATE AG Probability & Statistics

---

## 🎯 Most Important Formulas

### 1. Descriptive Statistics - The Core THREE

#### Mean
$$
\bar{x} = \frac{\sum x_i}{n}
$$

**For grouped data:**
$$
\bar{x} = \frac{\sum f_i x_i}{\sum f_i}
$$

---

#### Variance & Standard Deviation

**Population:**
$$
\sigma^2 = \frac{\sum (x_i - \mu)^2}{n}, \quad \sigma = \sqrt{\sigma^2}
$$

**Sample (use this for GATE):**
$$
s^2 = \frac{\sum (x_i - \bar{x})^2}{n-1}, \quad s = \sqrt{s^2}
$$

**Computational formula (FASTER!):**
$$
\sigma^2 = \frac{\sum x_i^2}{n} - \bar{x}^2 = \frac{\sum x_i^2}{n} - \left(\frac{\sum x_i}{n}\right)^2
$$

---

#### Coefficient of Variation
$$
CV = \frac{\sigma}{\bar{x}} \times 100\%
$$

**Use:** Compare variability between different datasets

---

### 2. Probability - The Essential Rules

#### Addition Rule (General)
$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$

**For mutually exclusive events:**
$$
P(A \cup B) = P(A) + P(B)
$$

---

#### Multiplication Rule (General)
$$
P(A \cap B) = P(A) \times P(B|A) = P(B) \times P(A|B)
$$

**For independent events:**
$$
P(A \cap B) = P(A) \times P(B)
$$

---

#### Conditional Probability
$$
P(A|B) = \frac{P(A \cap B)}{P(B)}
$$

---

#### Complement Rule
$$
P(A') = 1 - P(A)
$$

---

#### Bayes' Theorem ⭐
$$
P(A|B) = \frac{P(B|A) \times P(A)}{P(B)}
$$

**Extended form:**
$$
P(A_i|B) = \frac{P(B|A_i) \times P(A_i)}{\sum_j P(B|A_j) \times P(A_j)}
$$

---

### 3. Probability Distributions

#### Binomial Distribution

**When to use:** Fixed number of independent trials, two outcomes (success/failure)

**PMF:**
$$
P(X = r) = \binom{n}{r} p^r q^{n-r} = \frac{n!}{r!(n-r)!} p^r (1-p)^{n-r}
$$

**Parameters:**
$$
\text{Mean: } \mu = np
$$
$$
\text{Variance: } \sigma^2 = npq
$$
$$
\text{Standard Deviation: } \sigma = \sqrt{npq}
$$

**Quick Checks:**
- $n$ = fixed number of trials
- $p$ = probability of success (constant)
- $q = 1 - p$
- $r$ = number of successes

**Memory:** $\binom{n}{r}$ counts ways, $p^r$ for successes, $q^{n-r}$ for failures

---

#### Poisson Distribution

**When to use:** Number of events in fixed interval (time/space), rare events

**PMF:**
$$
P(X = r) = \frac{e^{-\lambda} \lambda^r}{r!}
$$

**Parameters:**
$$
\text{Mean: } \mu = \lambda
$$
$$
\text{Variance: } \sigma^2 = \lambda
$$

**KEY PROPERTY:** Mean = Variance = $\lambda$ (unique!)

**Common $e^{-\lambda}$ values (memorize):**
- $e^{-1} = 0.3679$
- $e^{-2} = 0.1353$
- $e^{-3} = 0.0498$
- $e^{-4} = 0.0183$
- $e^{-5} = 0.0067$

**Approximation:** Binomial → Poisson when $n$ large, $p$ small, $np = \lambda$

---

#### Normal Distribution (Gaussian)

**PDF:**
$$
f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

**Parameters:**
- $\mu$ = mean (center)
- $\sigma^2$ = variance
- $\sigma$ = standard deviation (spread)

**Standard Normal (Z-distribution):**
$$
Z = \frac{X - \mu}{\sigma}
$$

$Z \sim N(0, 1)$ (mean = 0, SD = 1)

---

#### Empirical Rule (68-95-99.7 Rule) ⭐⭐⭐

**MEMORIZE THIS:**

- **68%** of data within $\mu \pm 1\sigma$
- **95%** of data within $\mu \pm 2\sigma$
- **99.7%** of data within $\mu \pm 3\sigma$

```
         |←---- 68% ---->|
     |←-------- 95% -------->|
  |←---------- 99.7% ---------->|
μ-3σ  μ-2σ  μ-1σ   μ   μ+1σ  μ+2σ  μ+3σ
```

---

### 4. Correlation and Regression

#### Correlation Coefficient (Pearson's r)

**Formula 1 (standard):**
$$
r = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum (x_i - \bar{x})^2 \sum (y_i - \bar{y})^2}}
$$

**Formula 2 (computational - USE THIS!):**
$$
r = \frac{n\sum x_i y_i - \sum x_i \sum y_i}{\sqrt{[n\sum x_i^2 - (\sum x_i)^2][n\sum y_i^2 - (\sum y_i)^2]}}
$$

**Properties:**
- $-1 \leq r \leq 1$
- $r > 0$: Positive correlation
- $r < 0$: Negative correlation
- $r = 0$: No linear correlation
- $r = \pm 1$: Perfect correlation

**Strength interpretation:**
- $|r| < 0.3$: Weak
- $0.3 \leq |r| < 0.7$: Moderate
- $|r| \geq 0.7$: Strong

---

#### Simple Linear Regression

**Regression line (Y on X):**
$$
Y = a + bX
$$

**Slope:**
$$
b = \frac{n\sum x_i y_i - \sum x_i \sum y_i}{n\sum x_i^2 - (\sum x_i)^2}
$$

**Alternative:**
$$
b = r \times \frac{\sigma_Y}{\sigma_X}
$$

**Intercept:**
$$
a = \bar{y} - b\bar{x}
$$

**KEY PROPERTY:** Line always passes through $(\bar{x}, \bar{y})$ ✓

**Coefficient of Determination:**
$$
R^2 = r^2
$$

Interpretation: Proportion of variance in Y explained by X

---

## 📊 Quick Comparison Tables

### Distribution Selection Guide

| Distribution | Use When | Parameters | Mean | Variance |
|--------------|----------|------------|------|----------|
| **Binomial** | Fixed trials, binary outcomes | $n$, $p$ | $np$ | $npq$ |
| **Poisson** | Rate in fixed interval, rare events | $\lambda$ | $\lambda$ | $\lambda$ |
| **Normal** | Continuous, symmetric, bell-shaped | $\mu$, $\sigma^2$ | $\mu$ | $\sigma^2$ |
| **Exponential** | Time between events | $\lambda$ | $1/\lambda$ | $1/\lambda^2$ |
| **Uniform** | All values equally likely | $a$, $b$ | $(a+b)/2$ | $(b-a)^2/12$ |

---

### Common Z-values (Standard Normal)

| Confidence Level | Tail Area ($\alpha$) | $Z_{\alpha/2}$ | Use |
|------------------|----------------------|----------------|-----|
| 90% | 0.10 | 1.645 | CI, hypothesis tests |
| 95% | 0.05 | 1.96 | Most common |
| 98% | 0.02 | 2.33 | |
| 99% | 0.01 | 2.576 | High confidence |

**Symmetric property:**
$$
P(Z < -z) = P(Z > z) = 1 - P(Z < z)
$$

---

### Variance Properties (Quick Reference)

| Operation | Effect on Variance |
|-----------|-------------------|
| $X + c$ | No change |
| $X - c$ | No change |
| $cX$ | Multiply by $c^2$ |
| $aX + b$ | Multiply by $a^2$ |

**Formula:**
$$
\text{Var}(aX + b) = a^2 \times \text{Var}(X)
$$

---

## 🚀 Exam Shortcuts & Memory Tricks

### 1. Correlation Calculation Template

**Set up table with 5 columns:**

| $x_i$ | $y_i$ | $x_i^2$ | $y_i^2$ | $x_i y_i$ |
|-------|-------|---------|---------|-----------|
| ... | ... | ... | ... | ... |
| **Σ** | | | | |

**Then apply formula with $n$ and five sums.**

---

### 2. Binomial Quick Check

**Given:** $n = 10$, $p = 0.4$

**Mean:** $\mu = 10 \times 0.4 = 4$ (just multiply!)

**Variance:** $\sigma^2 = 10 \times 0.4 \times 0.6 = 2.4$

**Time:** 10 seconds!

---

### 3. Normal Distribution Strategy

**Always follow these steps:**

1. **Identify:** $\mu$, $\sigma$, and required value/range
2. **Standardize:** $Z = \frac{X - \mu}{\sigma}$
3. **Use Z-table** or memorized values
4. **Remember:** 
   - $P(Z > z) = 1 - P(Z < z)$
   - $P(a < Z < b) = P(Z < b) - P(Z < a)$

---

### 4. Poisson Shortcut

**Given:** Average 3 events per hour

**Mean = Variance = 3** (immediately!)

For probability calculations, just need $e^{-3} = 0.0498$ (memorize this!)

---

### 5. Regression Verification

**After calculating $a$ and $b$, always check:**
$$
\bar{y} = a + b\bar{x}
$$

If this doesn't work, you made an error!

---

## 🎓 Memory Devices

### BINOMIAL → "Binary Outcomes, Independent, N trials"

**Requirements checklist:**
- ✓ Fixed number of trials ($n$)
- ✓ Two outcomes only (success/failure)
- ✓ Trials independent
- ✓ Probability constant ($p$)

### POISSON → "Rate in time/space"

**Key word:** "Average rate per..."
- Calls per hour
- Defects per meter
- Arrivals per day

**Special property:** Mean = Variance!

### NORMAL → "Nature's distribution"

**Identifies:**
- Height, weight, test scores
- Errors in measurements
- Symmetric bell curve
- Described by $\mu$ and $\sigma$

---

## ⚠️ Common Mistakes to Avoid

### 1. Descriptive Statistics Mistakes

❌ **Wrong:** Using $n$ in sample variance
$$
s^2 = \frac{\sum(x - \bar{x})^2}{n} \quad \text{(WRONG!)}
$$

✅ **Correct:** Using $n-1$ (Bessel's correction)
$$
s^2 = \frac{\sum(x - \bar{x})^2}{n-1} \quad \text{(CORRECT)}
$$

❌ **Wrong:** $\text{Var}(2X + 3) = 2 \times \text{Var}(X) + 3$

✅ **Correct:** $\text{Var}(2X + 3) = 4 \times \text{Var}(X)$ (only $a^2$ matters)

---

### 2. Probability Mistakes

❌ **Wrong:** $P(A \cup B) = P(A) + P(B)$ (always)

✅ **Correct:** $P(A \cup B) = P(A) + P(B) - P(A \cap B)$ (general)
- Only use addition alone if mutually exclusive!

❌ **Wrong:** Confusing $P(A|B)$ with $P(B|A)$
- These are different! Use Bayes' theorem to relate them.

---

### 3. Distribution Mistakes

❌ **Wrong:** Using Binomial for "time until event"
- Binomial = fixed trials
- Geometric/Exponential = time until success

❌ **Wrong:** Forgetting to standardize before using Normal tables
- Must calculate $Z = \frac{X - \mu}{\sigma}$ first!

❌ **Wrong:** $P(X = x)$ for continuous distribution
- For continuous: $P(X = x) = 0$ always
- Use $P(a < X < b)$ instead

---

### 4. Correlation & Regression Mistakes

❌ **Wrong:** "High correlation means causation"
- Correlation ≠ Causation (ever!)
- Example: Ice cream sales and drownings correlate (both peak in summer)

❌ **Wrong:** Switching X and Y gives same regression line
- Regression of Y on X ≠ Regression of X on Y
- Correlation is symmetric, regression is not

❌ **Wrong:** Extrapolating beyond data range
- Regression only valid within observed range

---

## 🎯 Last-Minute Revision (5 minutes before exam)

### Must-Memorize Formulas

**1. Descriptive:**
$$
\bar{x} = \frac{\sum x}{n}, \quad s = \sqrt{\frac{\sum(x-\bar{x})^2}{n-1}}, \quad CV = \frac{s}{\bar{x}} \times 100\%
$$

**2. Probability:**
$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$
$$
P(A|B) = \frac{P(A \cap B)}{P(B)}
$$

**3. Binomial:**
$$
P(X=r) = \binom{n}{r}p^r q^{n-r}, \quad \mu = np, \quad \sigma^2 = npq
$$

**4. Poisson:**
$$
P(X=r) = \frac{e^{-\lambda}\lambda^r}{r!}, \quad \mu = \sigma^2 = \lambda
$$

**5. Normal:**
$$
Z = \frac{X-\mu}{\sigma}, \quad \text{68-95-99.7 Rule}
$$

**6. Correlation:**
$$
r = \frac{n\sum xy - \sum x \sum y}{\sqrt{[n\sum x^2 - (\sum x)^2][n\sum y^2 - (\sum y)^2]}}
$$

**7. Regression:**
$$
b = \frac{n\sum xy - \sum x \sum y}{n\sum x^2 - (\sum x)^2}, \quad a = \bar{y} - b\bar{x}
$$

---

### Key Concepts (One-Liners)

1. **Sample variance uses $n-1$** (unbiased estimator)
2. **Poisson: Mean = Variance** (unique property)
3. **Empirical Rule: 68-95-99.7** for $\pm 1\sigma, 2\sigma, 3\sigma$
4. **Regression line passes through** $(\bar{x}, \bar{y})$
5. **Correlation ≠ Causation** (always!)
6. **Independent events:** $P(A \cap B) = P(A) \times P(B)$
7. **$Z = 1.96$ for 95% confidence**

---

## 📱 Mobile-Friendly Quick Reference

### Distribution Quick-Pick

```
Fixed trials + Binary?          → BINOMIAL
Rate per interval + Rare?       → POISSON
Continuous + Symmetric?         → NORMAL
Time between events?            → EXPONENTIAL
All values equal chance?        → UNIFORM
```

### Correlation Strength

```
|r| < 0.3     → Weak        😐
0.3 ≤ |r| < 0.7 → Moderate   😊
|r| ≥ 0.7     → Strong      😍
```

### Variance Transform

```
Var(X + 5)     = Var(X)       (constant doesn't matter)
Var(3X)        = 9·Var(X)     (square the multiplier)
Var(2X + 7)    = 4·Var(X)     (only multiplier matters)
```

---

## 💪 Problem Templates

### Template 1: Mean and Variance

**Given:** Data set {values}

**Steps:**
1. $n$ = count
2. $\sum x = $ add all values
3. $\bar{x} = \frac{\sum x}{n}$
4. $\sum x^2 = $ add all squares
5. $s^2 = \frac{n\sum x^2 - (\sum x)^2}{n(n-1)}$ OR $\frac{\sum(x-\bar{x})^2}{n-1}$
6. $s = \sqrt{s^2}$

**Time:** 2 minutes

---

### Template 2: Binomial Probability

**Given:** $n$ trials, probability $p$, find $P(X = r)$

**Steps:**
1. $q = 1 - p$
2. $\binom{n}{r} = \frac{n!}{r!(n-r)!}$
3. $P(X=r) = \binom{n}{r} \times p^r \times q^{n-r}$

**Bonus:**
- Mean: $np$
- Variance: $npq$

**Time:** 1-2 minutes

---

### Template 3: Normal Probability

**Given:** $X \sim N(\mu, \sigma^2)$, find $P(X < a)$

**Steps:**
1. Standardize: $Z = \frac{a - \mu}{\sigma}$
2. Use Z-table: Find $P(Z < z)$
3. If $P(X > a)$: Use $1 - P(Z < z)$
4. If $P(a < X < b)$: Calculate $P(Z < z_b) - P(Z < z_a)$

**Time:** 1-2 minutes

---

### Template 4: Correlation

**Given:** Data pairs $(x_i, y_i)$

**Steps:**
1. Make table: $x_i$, $y_i$, $x_i^2$, $y_i^2$, $x_i y_i$
2. Calculate 5 sums and $n$
3. Plug into formula:
$$
r = \frac{n\sum xy - \sum x \sum y}{\sqrt{[n\sum x^2 - (\sum x)^2][n\sum y^2 - (\sum y)^2]}}
$$

**Time:** 3-4 minutes

---

### Template 5: Regression

**Given:** Data pairs, find $Y = a + bX$

**Steps:**
1. Use correlation table (same as above)
2. Calculate slope:
$$
b = \frac{n\sum xy - \sum x \sum y}{n\sum x^2 - (\sum x)^2}
$$
3. Calculate means: $\bar{x} = \frac{\sum x}{n}$, $\bar{y} = \frac{\sum y}{n}$
4. Calculate intercept: $a = \bar{y} - b\bar{x}$
5. **Verify:** $\bar{y} = a + b\bar{x}$ ✓

**Time:** 3-4 minutes

---

## 🔥 High-Yield Topics for GATE AG

### Must Know (Appear Almost Every Year)

1. ⭐⭐⭐⭐⭐ **Mean, Median, Mode, SD** - Basic calculations
2. ⭐⭐⭐⭐⭐ **Binomial Distribution** - Direct probability questions
3. ⭐⭐⭐⭐⭐ **Normal Distribution** - Standardization and Z-scores
4. ⭐⭐⭐⭐⭐ **Correlation Coefficient** - Calculation questions
5. ⭐⭐⭐⭐ **Poisson Distribution** - Average rate problems
6. ⭐⭐⭐⭐ **Regression Line** - Finding equation

### Good to Know (Appear Frequently)

7. ⭐⭐⭐ **Basic Probability Rules** - Addition, multiplication
8. ⭐⭐⭐ **Conditional Probability** - P(A|B) calculations
9. ⭐⭐⭐ **Coefficient of Variation** - Comparing variability
10. ⭐⭐⭐ **Variance Properties** - Transformations

### Less Common (But Possible)

- Bayes' Theorem
- Hypothesis Testing
- Confidence Intervals
- Sampling Distributions
- Chi-square tests

---

## 📌 Formula Summary Card (Print & Keep!)

```
┌──────────────────────────────────────────────────────────┐
│       PROBABILITY & STATISTICS - FORMULA CARD            │
├──────────────────────────────────────────────────────────┤
│                                                          │
│ DESCRIPTIVE:                                             │
│   Mean: x̄ = Σx/n                                        │
│   Variance: s² = Σ(x-x̄)²/(n-1)                         │
│   CV = (s/x̄) × 100%                                     │
│                                                          │
│ PROBABILITY:                                             │
│   P(A∪B) = P(A) + P(B) - P(A∩B)                         │
│   P(A|B) = P(A∩B)/P(B)                                  │
│   Independent: P(A∩B) = P(A)×P(B)                       │
│                                                          │
│ DISTRIBUTIONS:                                           │
│   Binomial: P(r) = C(n,r)·pʳ·qⁿ⁻ʳ,  μ=np, σ²=npq       │
│   Poisson: P(r) = e⁻λ·λʳ/r!,  μ=σ²=λ                   │
│   Normal: Z = (X-μ)/σ,  68-95-99.7 Rule                 │
│                                                          │
│ CORRELATION & REGRESSION:                                │
│   r = [nΣxy - ΣxΣy]/√[(nΣx²-(Σx)²)(nΣy²-(Σy)²)]       │
│   b = [nΣxy - ΣxΣy]/[nΣx² - (Σx)²]                     │
│   a = ȳ - bx̄                                            │
│                                                          │
│ REMEMBER:                                                │
│   • Sample variance uses n-1                             │
│   • Poisson: mean = variance                             │
│   • Regression passes through (x̄, ȳ)                    │
│   • Z = 1.96 for 95% confidence                          │
│   • Correlation ≠ Causation!                             │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

---

## 🎓 Pro Tips from Toppers

### Time Management
- **Descriptive stats:** 1-2 minutes
- **Binomial/Poisson:** 1-2 minutes
- **Normal distribution:** 2 minutes
- **Correlation:** 3-4 minutes (most time-consuming)
- **Regression:** 3-4 minutes

### Strategy
1. **Identify distribution type first** - saves time
2. **Make tables** for correlation/regression - organized = fewer errors
3. **Use computational formulas** - faster than deviation method
4. **Check reasonableness** - probability between 0 and 1?
5. **Verify regression** - does line pass through $(\bar{x}, \bar{y})$?

### Common Traps
- ❌ Forgetting $n-1$ in sample variance
- ❌ Not standardizing before Normal tables
- ❌ Confusing $P(A|B)$ and $P(B|A)$
- ❌ Using wrong distribution type
- ❌ Arithmetic errors in correlation (double-check sums!)

---

## 📖 Related Cheat Sheets

- [Calculus Cheat Sheet](../Calculus/CheatSheet.md)
- [Linear Algebra Cheat Sheet](../Linear_Algebra/CheatSheet.md)
- [Differential Equations Cheat Sheet](../Differential_Equations/CheatSheet.md)
- [Numerical Methods Cheat Sheet](../Numerical_Methods/CheatSheet.md)

---

**Last Updated:** November 2025  
**Version:** 1.0

---

*For detailed explanations, see [Probability & Statistics README](./README.md)*  
*For practice problems, see [Probability & Statistics PYQ Solutions](./Solutions.md)*

---

## ✅ Pre-Exam Checklist

**One day before exam:**
- [ ] Review all distribution formulas
- [ ] Practice 3 problems each: Binomial, Poisson, Normal
- [ ] Practice 2 correlation/regression problems
- [ ] Memorize Z-values (1.96, 1.645, 2.576)
- [ ] Review empirical rule (68-95-99.7)

**Morning of exam:**
- [ ] Review this cheat sheet (10 minutes)
- [ ] Practice one mean/SD problem
- [ ] Practice one distribution problem
- [ ] Review correlation table setup
- [ ] Memorize: $e^{-1} = 0.368$, $e^{-2} = 0.135$

**During exam:**
- [ ] Identify distribution type FIRST
- [ ] Make systematic tables
- [ ] Check all arithmetic twice
- [ ] Verify answers make sense
- [ ] Use remaining time to double-check calculations

**Common Values to Memorize:**

| Value | Result |
|-------|--------|
| $e^{-1}$ | 0.3679 |
| $e^{-2}$ | 0.1353 |
| $e^{-3}$ | 0.0498 |
| $Z_{0.05}$ | 1.645 |
| $Z_{0.025}$ | 1.96 |
| $Z_{0.01}$ | 2.33 |
| $Z_{0.005}$ | 2.576 |

---

## 🧮 Calculator Tips

**For correlation/regression:**
1. Calculate all sums first
2. Write them down clearly
3. Then substitute
4. Double-check each multiplication

**For factorials:**
- $3! = 6$
- $4! = 24$
- $5! = 120$
- $6! = 720$
- $7! = 5040$

**For combinations:**
$$
\binom{n}{r} = \binom{n}{n-r} \quad \text{(symmetry - use smaller number!)}
$$

Example: $\binom{10}{8} = \binom{10}{2} = 45$ (much easier!)

---

## 🌟 Final Words

**Probability & Statistics success formula:**

1. **Identify** distribution/concept correctly (50% of battle)
2. **Organize** data systematically (prevents errors)
3. **Calculate** carefully (arithmetic matters!)
4. **Verify** answer makes sense (catch mistakes)

**Most important skills:**
- Recognizing distribution types
- Making systematic calculation tables
- Using computational formulas efficiently
- Checking work for reasonableness

**Good luck! You've got this! 🚀**

---

*Remember: Statistics is about patterns, not perfection. Understand the concepts, practice the calculations, and trust your preparation!*
