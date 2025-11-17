# 📊 Probability and Statistics

> Complete guide to Probability and Statistics for GATE Agricultural Engineering

---

## 📑 Table of Contents

1. [Descriptive Statistics](#1-descriptive-statistics)
2. [Probability Theory](#2-probability-theory)
3. [Random Variables](#3-random-variables)
4. [Probability Distributions](#4-probability-distributions)
5. [Correlation and Regression](#5-correlation-and-regression)
6. [Sampling and Estimation](#6-sampling-and-estimation)
7. [Hypothesis Testing](#7-hypothesis-testing)

---

## 1. Descriptive Statistics

### 1.1 Measures of Central Tendency

Descriptive statistics summarize and describe the main features of a dataset.

#### Mean (Arithmetic Average)

**For ungrouped data:**
$$
\bar{x} = \frac{\sum_{i=1}^{n} x_i}{n} = \frac{x_1 + x_2 + \cdots + x_n}{n}
$$

**For grouped data (frequency distribution):**
$$
\bar{x} = \frac{\sum_{i=1}^{k} f_i x_i}{\sum_{i=1}^{k} f_i} = \frac{\sum f_i x_i}{N}
$$

where:
- $x_i$ = midpoint of $i$-th class
- $f_i$ = frequency of $i$-th class
- $N$ = total frequency

**Example:**

Find the mean of: 5, 8, 12, 15, 20

$$
\bar{x} = \frac{5 + 8 + 12 + 15 + 20}{5} = \frac{60}{5} = 12
$$

---

#### Median

The **median** is the middle value when data is arranged in order.

**For odd n:**
$$
\text{Median} = \left(\frac{n+1}{2}\right)^{\text{th}} \text{ term}
$$

**For even n:**
$$
\text{Median} = \frac{\left(\frac{n}{2}\right)^{\text{th}} \text{ term} + \left(\frac{n}{2}+1\right)^{\text{th}} \text{ term}}{2}
$$

**For grouped data:**
$$
\text{Median} = L + \left(\frac{\frac{N}{2} - CF}{f}\right) \times h
$$

where:
- $L$ = lower boundary of median class
- $N$ = total frequency
- $CF$ = cumulative frequency before median class
- $f$ = frequency of median class
- $h$ = class width

**Example:**

Data: 3, 7, 9, 12, 15 (odd n = 5)

Median = 3rd term = **9**

Data: 2, 5, 7, 10 (even n = 4)

Median = $\frac{7 + 5}{2} = \frac{12}{2} = 6$

---

#### Mode

The **mode** is the value that occurs most frequently.

**For grouped data:**
$$
\text{Mode} = L + \left(\frac{f_1 - f_0}{2f_1 - f_0 - f_2}\right) \times h
$$

where:
- $L$ = lower boundary of modal class
- $f_1$ = frequency of modal class
- $f_0$ = frequency of class before modal class
- $f_2$ = frequency of class after modal class
- $h$ = class width

**Example:**

Data: 2, 3, 3, 5, 7, 3, 9

Mode = **3** (appears 3 times)

---

### 1.2 Measures of Dispersion

#### Range
$$
\text{Range} = \text{Maximum value} - \text{Minimum value}
$$

#### Variance

**Population variance:**
$$
\sigma^2 = \frac{\sum_{i=1}^{n} (x_i - \mu)^2}{n}
$$

**Sample variance:**
$$
s^2 = \frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n-1}
$$

**Alternative formula (computational):**
$$
\sigma^2 = \frac{\sum x_i^2}{n} - \left(\frac{\sum x_i}{n}\right)^2 = \frac{\sum x_i^2}{n} - \bar{x}^2
$$

#### Standard Deviation

$$
\sigma = \sqrt{\sigma^2} = \sqrt{\frac{\sum (x_i - \mu)^2}{n}}
$$

**Sample standard deviation:**
$$
s = \sqrt{s^2} = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n-1}}
$$

**Example:**

Data: 2, 4, 6, 8, 10

Mean: $\bar{x} = \frac{30}{5} = 6$

Variance:
$$
\sigma^2 = \frac{(2-6)^2 + (4-6)^2 + (6-6)^2 + (8-6)^2 + (10-6)^2}{5}
$$
$$
= \frac{16 + 4 + 0 + 4 + 16}{5} = \frac{40}{5} = 8
$$

Standard Deviation: $\sigma = \sqrt{8} = 2.83$

---

#### Coefficient of Variation (CV)

Measures relative variability:
$$
CV = \frac{\sigma}{\bar{x}} \times 100\%
$$

Used to compare variability between datasets with different units or means.

---

### 1.3 Important Properties

**Properties of Mean:**
- $\sum(x_i - \bar{x}) = 0$ (deviations sum to zero)
- Affected by extreme values (outliers)
- Unique for a dataset

**Properties of Median:**
- Not affected by extreme values
- Better measure for skewed distributions

**Properties of Standard Deviation:**
- Always non-negative
- If all values are equal, $\sigma = 0$
- Adding/subtracting constant: $\sigma$ unchanged
- Multiplying by constant $k$: new $\sigma = k \times \sigma$

---

## 2. Probability Theory

### 2.1 Basic Definitions

**Sample Space (S):** Set of all possible outcomes

**Event (E):** A subset of sample space

**Probability of event E:**
$$
P(E) = \frac{\text{Number of favorable outcomes}}{\text{Total number of outcomes}} = \frac{n(E)}{n(S)}
$$

**Properties:**
- $0 \leq P(E) \leq 1$
- $P(S) = 1$ (certain event)
- $P(\phi) = 0$ (impossible event)
- $P(E') = 1 - P(E)$ (complement rule)

---

### 2.2 Addition Rules

**For mutually exclusive events (disjoint):**
$$
P(A \cup B) = P(A) + P(B)
$$

**For any two events:**
$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$

**For three events:**
$$
P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(A \cap B) - P(B \cap C) - P(A \cap C) + P(A \cap B \cap C)
$$

---

### 2.3 Conditional Probability

Probability of A given B has occurred:
$$
P(A|B) = \frac{P(A \cap B)}{P(B)}, \quad P(B) > 0
$$

**Multiplication Rule:**
$$
P(A \cap B) = P(B) \times P(A|B) = P(A) \times P(B|A)
$$

---

### 2.4 Independent Events

Events A and B are independent if:
$$
P(A \cap B) = P(A) \times P(B)
$$

**Equivalently:**
- $P(A|B) = P(A)$
- $P(B|A) = P(B)$

---

### 2.5 Bayes' Theorem

$$
P(A|B) = \frac{P(B|A) \times P(A)}{P(B)}
$$

**Extended form:**
$$
P(A_i|B) = \frac{P(B|A_i) \times P(A_i)}{\sum_{j=1}^{n} P(B|A_j) \times P(A_j)}
$$

**Example:**

A factory has two machines. Machine A produces 60% of items, Machine B produces 40%. Defect rates: A = 2%, B = 5%. If a randomly selected item is defective, what's the probability it came from Machine A?

$$
P(A|D) = \frac{P(D|A) \times P(A)}{P(D|A) \times P(A) + P(D|B) \times P(B)}
$$
$$
= \frac{0.02 \times 0.6}{0.02 \times 0.6 + 0.05 \times 0.4} = \frac{0.012}{0.012 + 0.02} = \frac{0.012}{0.032} = 0.375
$$

---

## 3. Random Variables

### 3.1 Definition

A **random variable** is a function that assigns a numerical value to each outcome in a sample space.

**Types:**
- **Discrete:** Takes countable values (e.g., number of defects)
- **Continuous:** Takes any value in an interval (e.g., height, weight)

---

### 3.2 Probability Mass Function (PMF) - Discrete

For discrete random variable X:
$$
P(X = x) = p(x)
$$

**Properties:**
- $p(x) \geq 0$ for all $x$
- $\sum_{\text{all } x} p(x) = 1$

---

### 3.3 Probability Density Function (PDF) - Continuous

For continuous random variable X:
$$
P(a \leq X \leq b) = \int_a^b f(x) \, dx
$$

**Properties:**
- $f(x) \geq 0$ for all $x$
- $\int_{-\infty}^{\infty} f(x) \, dx = 1$
- $P(X = x) = 0$ (probability at a single point)

---

### 3.4 Cumulative Distribution Function (CDF)

$$
F(x) = P(X \leq x)
$$

**For discrete:**
$$
F(x) = \sum_{t \leq x} p(t)
$$

**For continuous:**
$$
F(x) = \int_{-\infty}^{x} f(t) \, dt
$$

**Properties:**
- $0 \leq F(x) \leq 1$
- $F(x)$ is non-decreasing
- $\lim_{x \to -\infty} F(x) = 0$
- $\lim_{x \to \infty} F(x) = 1$
- $f(x) = \frac{dF(x)}{dx}$ (for continuous)

---

### 3.5 Expected Value (Mean)

**For discrete random variable:**
$$
E(X) = \mu = \sum_{i} x_i \cdot p(x_i)
$$

**For continuous random variable:**
$$
E(X) = \mu = \int_{-\infty}^{\infty} x \cdot f(x) \, dx
$$

**Properties:**
- $E(aX + b) = aE(X) + b$
- $E(X + Y) = E(X) + E(Y)$
- If X and Y are independent: $E(XY) = E(X) \cdot E(Y)$

---

### 3.6 Variance

$$
\text{Var}(X) = \sigma^2 = E[(X - \mu)^2] = E(X^2) - [E(X)]^2
$$

**For discrete:**
$$
\text{Var}(X) = \sum x_i^2 \cdot p(x_i) - \mu^2
$$

**For continuous:**
$$
\text{Var}(X) = \int_{-\infty}^{\infty} x^2 \cdot f(x) \, dx - \mu^2
$$

**Properties:**
- $\text{Var}(aX + b) = a^2 \text{Var}(X)$
- $\text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y)$ (if independent)

**Standard Deviation:**
$$
\sigma = \sqrt{\text{Var}(X)}
$$

---

## 4. Probability Distributions

### 4.1 Binomial Distribution

Models number of successes in $n$ independent Bernoulli trials.

**Notation:** $X \sim B(n, p)$

**PMF:**
$$
P(X = r) = \binom{n}{r} p^r (1-p)^{n-r} = \frac{n!}{r!(n-r)!} p^r q^{n-r}
$$

where:
- $n$ = number of trials
- $p$ = probability of success
- $q = 1 - p$ = probability of failure
- $r$ = number of successes

**Mean:** $\mu = np$

**Variance:** $\sigma^2 = npq$

**Standard Deviation:** $\sigma = \sqrt{npq}$

**Example:**

A coin is tossed 5 times. Find probability of exactly 3 heads.

$n = 5$, $p = 0.5$, $r = 3$

$$
P(X = 3) = \binom{5}{3} (0.5)^3 (0.5)^2 = 10 \times 0.125 \times 0.25 = 0.3125
$$

---

### 4.2 Poisson Distribution

Models number of events in a fixed interval (time/space).

**Notation:** $X \sim \text{Poisson}(\lambda)$

**PMF:**
$$
P(X = r) = \frac{e^{-\lambda} \lambda^r}{r!}, \quad r = 0, 1, 2, \ldots
$$

where $\lambda$ = average rate (mean number of occurrences)

**Mean:** $\mu = \lambda$

**Variance:** $\sigma^2 = \lambda$

**Standard Deviation:** $\sigma = \sqrt{\lambda}$

**Properties:**
- Mean = Variance (special characteristic)
- Used for rare events
- Approximation to Binomial when $n$ large, $p$ small, $np = \lambda$ moderate

**Example:**

Average 3 calls per hour. Find probability of exactly 5 calls in an hour.

$\lambda = 3$, $r = 5$

$$
P(X = 5) = \frac{e^{-3} \times 3^5}{5!} = \frac{0.0498 \times 243}{120} = \frac{12.1}{120} = 0.1008
$$

---

### 4.3 Normal Distribution (Gaussian)

Most important continuous distribution.

**Notation:** $X \sim N(\mu, \sigma^2)$

**PDF:**
$$
f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}, \quad -\infty < x < \infty
$$

**Parameters:**
- $\mu$ = mean
- $\sigma^2$ = variance
- $\sigma$ = standard deviation

**Properties:**
- Symmetric about mean $\mu$
- Bell-shaped curve
- Mean = Median = Mode = $\mu$
- Total area under curve = 1
- 68% data within $\mu \pm \sigma$
- 95% data within $\mu \pm 2\sigma$
- 99.7% data within $\mu \pm 3\sigma$ (Empirical Rule)

---

#### Standard Normal Distribution

**Notation:** $Z \sim N(0, 1)$

**PDF:**
$$
\phi(z) = \frac{1}{\sqrt{2\pi}} e^{-\frac{z^2}{2}}
$$

**Standardization (Z-score):**
$$
Z = \frac{X - \mu}{\sigma}
$$

**Uses:**
- Convert any normal to standard normal
- Use standard normal tables (Z-tables)
- Compare different normal distributions

**Example:**

$X \sim N(50, 100)$ (mean = 50, variance = 100, so $\sigma = 10$)

Find $P(X < 65)$

$$
Z = \frac{65 - 50}{10} = 1.5
$$

From Z-table: $P(Z < 1.5) = 0.9332$

---

### 4.4 Common Z-values (Standard Normal)

| Probability | Z-value |
|-------------|---------|
| 0.90 | 1.28 |
| 0.95 | 1.645 |
| 0.975 | 1.96 |
| 0.99 | 2.33 |
| 0.995 | 2.576 |

**Symmetric property:**
$$
P(Z > z) = P(Z < -z)
$$
$$
P(-z < Z < z) = 2P(Z < z) - 1
$$

---

### 4.5 Exponential Distribution

Models time between events in Poisson process.

**PDF:**
$$
f(x) = \lambda e^{-\lambda x}, \quad x \geq 0
$$

**CDF:**
$$
F(x) = 1 - e^{-\lambda x}
$$

**Mean:** $\mu = \frac{1}{\lambda}$

**Variance:** $\sigma^2 = \frac{1}{\lambda^2}$

**Memoryless property:**
$$
P(X > s + t | X > s) = P(X > t)
$$

---

### 4.6 Uniform Distribution

All values equally likely.

**PDF:**
$$
f(x) = \frac{1}{b-a}, \quad a \leq x \leq b
$$

**Mean:** $\mu = \frac{a+b}{2}$

**Variance:** $\sigma^2 = \frac{(b-a)^2}{12}$

---

## 5. Correlation and Regression

### 5.1 Correlation

Measures strength and direction of linear relationship between two variables.

#### Covariance

$$
\text{Cov}(X, Y) = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{n}
$$

**Alternative formula:**
$$
\text{Cov}(X, Y) = \frac{\sum x_i y_i}{n} - \bar{x}\bar{y}
$$

---

#### Correlation Coefficient (Pearson's r)

$$
r = \frac{\text{Cov}(X, Y)}{\sigma_X \sigma_Y} = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum (x_i - \bar{x})^2 \sum (y_i - \bar{y})^2}}
$$

**Alternative formula:**
$$
r = \frac{n\sum x_i y_i - \sum x_i \sum y_i}{\sqrt{[n\sum x_i^2 - (\sum x_i)^2][n\sum y_i^2 - (\sum y_i)^2]}}
$$

**Properties:**
- $-1 \leq r \leq 1$
- $r = 1$: Perfect positive correlation
- $r = -1$: Perfect negative correlation
- $r = 0$: No linear correlation
- $|r| < 0.3$: Weak correlation
- $0.3 \leq |r| < 0.7$: Moderate correlation
- $|r| \geq 0.7$: Strong correlation

**Interpretation:**
- $r > 0$: Positive relationship (both increase together)
- $r < 0$: Negative relationship (one increases, other decreases)

---

### 5.2 Linear Regression

Predicts one variable (Y) from another (X).

#### Simple Linear Regression

**Regression line:**
$$
Y = a + bX
$$

where:
- $Y$ = dependent variable (response)
- $X$ = independent variable (predictor)
- $a$ = y-intercept
- $b$ = slope (regression coefficient)

---

#### Calculating Coefficients

**Slope:**
$$
b = \frac{n\sum x_i y_i - \sum x_i \sum y_i}{n\sum x_i^2 - (\sum x_i)^2} = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sum (x_i - \bar{x})^2}
$$

**Alternative:**
$$
b = r \times \frac{\sigma_Y}{\sigma_X}
$$

**Intercept:**
$$
a = \bar{y} - b\bar{x}
$$

**Key fact:** The regression line always passes through $(\bar{x}, \bar{y})$

---

#### Coefficient of Determination (R²)

$$
R^2 = r^2
$$

**Interpretation:**
- Proportion of variance in Y explained by X
- $R^2 = 0.80$ means 80% of variation in Y is explained by X
- $0 \leq R^2 \leq 1$
- Higher $R^2$ indicates better fit

---

### 5.3 Regression of X on Y

If predicting X from Y:
$$
X = a' + b'Y
$$

$$
b' = \frac{n\sum x_i y_i - \sum x_i \sum y_i}{n\sum y_i^2 - (\sum y_i)^2} = r \times \frac{\sigma_X}{\sigma_Y}
$$

$$
a' = \bar{x} - b'\bar{y}
$$

**Relationship between slopes:**
$$
b \times b' = r^2
$$

---

### 5.4 Example: Complete Regression Problem

**Data:**

| X | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| Y | 2 | 4 | 5 | 4 | 5 |

**Step 1: Calculate means**
$$
\bar{x} = \frac{15}{5} = 3, \quad \bar{y} = \frac{20}{5} = 4
$$

**Step 2: Calculate sums**

| $x_i$ | $y_i$ | $x_i^2$ | $y_i^2$ | $x_i y_i$ |
|-------|-------|---------|---------|-----------|
| 1 | 2 | 1 | 4 | 2 |
| 2 | 4 | 4 | 16 | 8 |
| 3 | 5 | 9 | 25 | 15 |
| 4 | 4 | 16 | 16 | 16 |
| 5 | 5 | 25 | 25 | 25 |
| **Σ** | **15** | **20** | **55** | **86** | **66** |

**Step 3: Calculate correlation**
$$
r = \frac{5(66) - 15(20)}{\sqrt{[5(55) - 225][5(86) - 400]}} = \frac{330 - 300}{\sqrt{[50][30]}} = \frac{30}{\sqrt{1500}} = \frac{30}{38.73} = 0.77
$$

**Step 4: Calculate regression coefficients**
$$
b = \frac{5(66) - 15(20)}{5(55) - 225} = \frac{30}{50} = 0.6
$$

$$
a = 4 - 0.6(3) = 4 - 1.8 = 2.2
$$

**Regression line:** $Y = 2.2 + 0.6X$

**Step 5: Predictions**

For $X = 6$:
$$
Y = 2.2 + 0.6(6) = 2.2 + 3.6 = 5.8
$$

---

## 6. Sampling and Estimation

### 6.1 Sampling Distributions

#### Standard Error of Mean

$$
SE = \frac{\sigma}{\sqrt{n}}
$$

where:
- $\sigma$ = population standard deviation
- $n$ = sample size

**If $\sigma$ unknown, use sample SD:**
$$
SE = \frac{s}{\sqrt{n}}
$$

---

#### Central Limit Theorem (CLT)

For large sample size $n$ (typically $n \geq 30$):

$$
\bar{X} \sim N\left(\mu, \frac{\sigma^2}{n}\right)
$$

**Standardized:**
$$
Z = \frac{\bar{X} - \mu}{\sigma/\sqrt{n}}
$$

**Importance:** Even if population is not normal, sample means are approximately normal for large $n$.

---

### 6.2 Confidence Intervals

#### For Population Mean (σ known)

**95% Confidence Interval:**
$$
\bar{x} - 1.96 \times \frac{\sigma}{\sqrt{n}} < \mu < \bar{x} + 1.96 \times \frac{\sigma}{\sqrt{n}}
$$

**General form:**
$$
\bar{x} \pm Z_{\alpha/2} \times \frac{\sigma}{\sqrt{n}}
$$

| Confidence Level | $Z_{\alpha/2}$ |
|------------------|----------------|
| 90% | 1.645 |
| 95% | 1.96 |
| 99% | 2.576 |

---

#### For Population Mean (σ unknown, n < 30)

Use t-distribution:
$$
\bar{x} \pm t_{\alpha/2, n-1} \times \frac{s}{\sqrt{n}}
$$

where $t_{\alpha/2, n-1}$ is from t-table with $n-1$ degrees of freedom.

---

#### For Population Proportion

$$
\hat{p} \pm Z_{\alpha/2} \times \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}
$$

where $\hat{p} = \frac{x}{n}$ (sample proportion)

---

### 6.3 Sample Size Determination

**For estimating mean:**
$$
n = \left(\frac{Z_{\alpha/2} \times \sigma}{E}\right)^2
$$

where $E$ = desired margin of error

**For estimating proportion:**
$$
n = \left(\frac{Z_{\alpha/2}}{E}\right)^2 \times p(1-p)
$$

If $p$ unknown, use $p = 0.5$ (most conservative)

---

## 7. Hypothesis Testing

### 7.1 Basic Concepts

**Null Hypothesis ($H_0$):** Statement of no effect/no difference

**Alternative Hypothesis ($H_1$ or $H_a$):** What we want to prove

**Types of tests:**
- **Two-tailed:** $H_1: \mu \neq \mu_0$
- **Right-tailed:** $H_1: \mu > \mu_0$
- **Left-tailed:** $H_1: \mu < \mu_0$

**Significance level ($\alpha$):** Probability of Type I error (typically 0.05 or 0.01)

**Type I Error:** Reject $H_0$ when it's true
**Type II Error:** Fail to reject $H_0$ when it's false

---

### 7.2 Test for Population Mean (σ known)

**Test statistic:**
$$
Z = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}}
$$

**Decision rule:**
- **Two-tailed:** Reject $H_0$ if $|Z| > Z_{\alpha/2}$
- **Right-tailed:** Reject $H_0$ if $Z > Z_\alpha$
- **Left-tailed:** Reject $H_0$ if $Z < -Z_\alpha$

---

### 7.3 Test for Population Mean (σ unknown)

**Test statistic:**
$$
t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}
$$

with $n-1$ degrees of freedom

---

### 7.4 Test for Population Proportion

**Test statistic:**
$$
Z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}
$$

where:
- $\hat{p}$ = sample proportion
- $p_0$ = hypothesized proportion

---

### 7.5 p-value Method

**p-value:** Probability of obtaining test results at least as extreme as observed, assuming $H_0$ is true.

**Decision:**
- If $p\text{-value} < \alpha$: Reject $H_0$
- If $p\text{-value} \geq \alpha$: Fail to reject $H_0$

**Interpretation:**
- $p < 0.01$: Very strong evidence against $H_0$
- $0.01 \leq p < 0.05$: Strong evidence against $H_0$
- $0.05 \leq p < 0.10$: Weak evidence against $H_0$
- $p \geq 0.10$: Little or no evidence against $H_0$

---

### 7.6 Example: Complete Hypothesis Test

**Problem:** A manufacturer claims mean battery life is 500 hours. A sample of 36 batteries has mean 485 hours and SD 40 hours. Test at 5% significance level.

**Solution:**

**Step 1: Hypotheses**
- $H_0: \mu = 500$
- $H_1: \mu \neq 500$ (two-tailed)

**Step 2: Significance level**
$$
\alpha = 0.05, \quad Z_{\alpha/2} = 1.96
$$

**Step 3: Test statistic**
$$
Z = \frac{485 - 500}{40/\sqrt{36}} = \frac{-15}{40/6} = \frac{-15}{6.67} = -2.25
$$

**Step 4: Decision**

$|Z| = 2.25 > 1.96$

Reject $H_0$

**Conclusion:** There is sufficient evidence to reject the manufacturer's claim at 5% significance level.

---

## 📊 Topic Importance for GATE AG

| Topic | Frequency | Difficulty | GATE Weightage |
|-------|-----------|------------|----------------|
| **Mean, Median, Mode, SD** | Very High | Easy-Medium | ⭐⭐⭐⭐⭐ |
| **Binomial Distribution** | Very High | Medium | ⭐⭐⭐⭐⭐ |
| **Normal Distribution** | Very High | Medium-Hard | ⭐⭐⭐⭐⭐ |
| **Poisson Distribution** | High | Medium | ⭐⭐⭐⭐ |
| **Correlation** | High | Medium | ⭐⭐⭐⭐ |
| **Regression** | High | Medium | ⭐⭐⭐⭐ |
| **Probability Basics** | High | Easy-Medium | ⭐⭐⭐⭐ |
| **Hypothesis Testing** | Medium | Hard | ⭐⭐⭐ |
| **Confidence Intervals** | Medium | Medium | ⭐⭐⭐ |

---

## 🎯 Key Formulas Quick Reference

### Descriptive Statistics
$$
\bar{x} = \frac{\sum x}{n}, \quad \sigma = \sqrt{\frac{\sum(x-\bar{x})^2}{n}}, \quad CV = \frac{\sigma}{\bar{x}} \times 100\%
$$

### Probability
$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$

### Distributions
$$
\begin{aligned}
\text{Binomial: } & P(X=r) = \binom{n}{r}p^r q^{n-r}, \quad \mu = np, \quad \sigma^2 = npq \\
\text{Poisson: } & P(X=r) = \frac{e^{-\lambda}\lambda^r}{r!}, \quad \mu = \sigma^2 = \lambda \\
\text{Normal: } & Z = \frac{X-\mu}{\sigma}
\end{aligned}
$$

### Correlation & Regression
$$
r = \frac{n\sum xy - \sum x \sum y}{\sqrt{[n\sum x^2 - (\sum x)^2][n\sum y^2 - (\sum y)^2]}}
$$

$$
b = \frac{n\sum xy - \sum x \sum y}{n\sum x^2 - (\sum x)^2}, \quad a = \bar{y} - b\bar{x}
$$

---

## 💡 Problem-Solving Strategy

### For Descriptive Statistics:
1. Organize data in table
2. Calculate required sums ($\sum x$, $\sum x^2$, etc.)
3. Apply formulas systematically
4. Check units and reasonableness

### For Probability:
1. Identify sample space
2. Define events clearly
3. Check for independence/mutual exclusivity
4. Use appropriate addition/multiplication rules

### For Distributions:
1. Identify the distribution type
2. Extract parameters ($n$, $p$, $\lambda$, $\mu$, $\sigma$)
3. Write what's given and what's required
4. Apply appropriate formula
5. Use tables/calculator for values

### For Correlation & Regression:
1. Make a systematic table with columns
2. Calculate all required sums
3. Substitute in formulas carefully
4. Interpret results in context

### For Hypothesis Testing:
1. State hypotheses clearly
2. Identify test type (one/two-tailed)
3. Calculate test statistic
4. Compare with critical value or find p-value
5. State conclusion in context

---

## 🔍 Common Mistakes to Avoid

1. **Confusing population vs. sample formulas** (n vs. n-1 in variance)
2. **Using wrong distribution** (Binomial vs. Poisson vs. Normal)
3. **Arithmetic errors** in correlation/regression calculations
4. **Not standardizing** before using normal tables
5. **Interpreting correlation as causation**
6. **Wrong tail** in hypothesis testing
7. **Forgetting to take square root** for standard deviation
8. **Using mean when median is more appropriate** (skewed data)

---

## 📚 Related Topics

- [Calculus](../Calculus/README.md) - For continuous distributions
- [Differential Equations](../Differential_Equations/README.md) - For stochastic processes
- [Linear Algebra](../Linear_Algebra/README.md) - For multivariate statistics
- [Numerical Methods](../Numerical_Methods/README.md) - For computational statistics

---

**Last Updated:** November 2025  
**Version:** 1.0

---

*For practice problems, see [Probability & Statistics PYQ Solutions](./Solutions.md)*  
*For quick revision, see [Probability & Statistics Cheat Sheet](./CheatSheet.md)*
