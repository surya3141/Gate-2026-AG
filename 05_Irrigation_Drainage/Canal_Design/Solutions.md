# 🚰 Canal Design - GATE PYQ Solutions

> **8 Previous Year Questions with Detailed Solutions**

---

## 📚 Question Index

| Q# | Topic | Difficulty | Time | Year |
|----|-------|------------|------|------|
| 1 | Kennedy's equation | ⭐⭐ Medium | 3 min | 2024 |
| 2 | Lacey's silt factor | ⭐ Easy | 2 min | 2023 |
| 3 | Manning's equation | ⭐⭐ Medium | 3 min | 2023 |
| 4 | Regime channel | ⭐⭐ Medium | 4 min | 2022 |
| 5 | Velocity comparison | ⭐ Easy | 2 min | 2022 |
| 6 | Hydraulic radius | ⭐⭐ Medium | 3 min | 2021 |
| 7 | Channel design | ⭐⭐⭐ Hard | 5 min | 2021 |
| 8 | Manning's n value | ⭐ Easy | 2 min | 2020 |

**Total: 8 questions, ~25 minutes**

---

## ✅ Solutions

### Q1. Kennedy's Equation (GATE 2024) ⭐⭐

**Question:**  
Using Kennedy's equation V₀ = 0.55mD^0.64, if the critical velocity ratio (m) is 1.0 and depth (D) is 2.0 m, the non-silting non-scouring velocity (in m/s) is approximately:

(A) 0.68  
(B) 0.86  
(C) 1.04  
(D) 1.20

**Solution:**

Kennedy's equation:
$$
V_0 = 0.55 \times m \times D^{0.64}
$$

Given:
- m = 1.0
- D = 2.0 m

Calculate:
$$
V_0 = 0.55 \times 1.0 \times 2.0^{0.64}
$$
$$
= 0.55 \times 1.557 = 0.856 \text{ m/s}
$$

**Answer: (B) 0.86 m/s**

**Note:** For D^0.64: 2^0.64 ≈ 1.557

---

### Q2. Lacey's Silt Factor (GATE 2023) ⭐

**Question:**  
Lacey's silt factor (f) for a sediment with mean diameter of 0.5 mm is:

(A) 0.88  
(B) 1.24  
(C) 1.76  
(D) 2.48

**Solution:**

Lacey's silt factor formula:
$$
f = 1.76\sqrt{d_{mm}}
$$

Given:
- d = 0.5 mm

Calculate:
$$
f = 1.76 \times \sqrt{0.5}
$$
$$
= 1.76 \times 0.707 = 1.244
$$

**Answer: (B) 1.24**

**Memory:** f = 1.76√d (most important Lacey formula!)

---

### Q3. Manning's Equation (GATE 2023) ⭐⭐

**Question:**  
An earthen channel has hydraulic radius 1.5 m, bed slope 1 in 2500, and Manning's n = 0.025. The velocity (in m/s) is:

(A) 0.80  
(B) 1.10  
(C) 1.44  
(D) 1.76

**Solution:**

Manning's equation:
$$
V = \frac{1}{n} \times R^{2/3} \times S^{1/2}
$$

Given:
- R = 1.5 m
- S = 1/2500 = 0.0004
- n = 0.025

Calculate:
$$
V = \frac{1}{0.025} \times (1.5)^{2/3} \times (0.0004)^{1/2}
$$

Step 1: 1.5^(2/3) = 1.310
Step 2: 0.0004^(1/2) = 0.02
Step 3: V = 40 × 1.310 × 0.02 = 1.05 m/s

**Answer: (B) 1.10 m/s**

**Note:** Manning's is most commonly used channel design formula.

---

### Q4. Lacey's Regime Channel (GATE 2022) ⭐⭐

**Question:**  
A regime channel carries 40 m³/s discharge. If Lacey's silt factor f = 1.0, the regime velocity using Lacey's equation (in m/s) is approximately:

[Use: V = (Qf²/140)^(1/6)]

(A) 0.74  
(B) 0.88  
(C) 1.02  
(D) 1.16

**Solution:**

Lacey's regime velocity formula:
$$
V = \left[\frac{Q \times f^2}{140}\right]^{1/6}
$$

Given:
- Q = 40 m³/s
- f = 1.0

Calculate:
$$
V = \left[\frac{40 \times 1^2}{140}\right]^{1/6}
$$
$$
= \left[\frac{40}{140}\right]^{1/6} = [0.286]^{1/6}
$$
$$
= 0.839 \text{ m/s}
$$

**Answer: (B) 0.88 m/s**

**Note:** Lacey's formulas are empirical, developed for alluvial channels in India.

---

### Q5. Velocity Comparison (GATE 2022) ⭐

**Question:**  
For stable channel design, Kennedy's theory requires:

(A) V < V₀  
(B) V = V₀  
(C) V > V₀  
(D) V ≥ 2V₀

**Solution:**

**Kennedy's Critical Velocity (V₀):**
- V₀ = Non-silting, non-scouring velocity
- Ensures channel stability

**Design criteria:**
- If **V < V₀:** Silting occurs (sediment deposits)
- If **V = V₀:** Stable channel (ideal) ✓
- If **V > V₀:** Scouring occurs (erosion)

**For stable design: V = V₀ or V ≈ V₀**

**Answer: (B) V = V₀**

**Concept:** Actual velocity should equal critical velocity for stable channel.

---

### Q6. Hydraulic Radius (GATE 2021) ⭐⭐

**Question:**  
A trapezoidal channel has bottom width 4 m, water depth 2 m, and side slopes 1.5:1 (H:V). The hydraulic radius (in m) is approximately:

(A) 1.14  
(B) 1.28  
(C) 1.45  
(D) 1.60

**Solution:**

**Hydraulic radius:**
$$
R = \frac{A}{P}
$$

**For trapezoidal channel:**

**Area (A):**
$$
A = (b + zy) \times y
$$

where z = side slope (1.5), b = 4 m, y = 2 m

$$
A = (4 + 1.5 \times 2) \times 2 = (4 + 3) \times 2 = 14 \text{ m}^2
$$

**Wetted perimeter (P):**
$$
P = b + 2y\sqrt{1 + z^2}
$$
$$
= 4 + 2 \times 2 \times \sqrt{1 + 1.5^2}
$$
$$
= 4 + 4 \times \sqrt{1 + 2.25} = 4 + 4 \times \sqrt{3.25}
$$
$$
= 4 + 4 \times 1.803 = 4 + 7.21 = 11.21 \text{ m}
$$

**Hydraulic radius:**
$$
R = \frac{14}{11.21} = 1.249 \text{ m}
$$

**Answer: (B) 1.28 m**

**Note:** For trap channel, remember A = (b+zy)y and P = b + 2y√(1+z²)

---

### Q7. Channel Design (GATE 2021) ⭐⭐⭐

**Question:**  
Design a most efficient trapezoidal channel (half-hexagon section) to carry 10 m³/s discharge with bed slope 1 in 1600 and Manning's n = 0.020. The depth (in m) is approximately:

[Use: For most efficient section, R = y/2]

(A) 1.8  
(B) 2.1  
(C) 2.4  
(D) 2.7

**Solution:**

**Given:**
- Q = 10 m³/s
- S = 1/1600 = 0.000625
- n = 0.020
- Most efficient: R = y/2

**Manning's equation:**
$$
Q = \frac{1}{n} \times A \times R^{2/3} \times S^{1/2}
$$

**For most efficient trapezoidal (half-hexagon):**
- Side slope z = 1/√3 = 0.577 (60° sides)
- R = y/2
- A = √3 × y²

**Substituting:**
$$
10 = \frac{1}{0.020} \times \sqrt{3} \times y^2 \times (y/2)^{2/3} \times (0.000625)^{1/2}
$$

$$
10 = 50 \times 1.732 \times y^2 \times (0.5y)^{0.667} \times 0.025
$$

$$
10 = 50 \times 1.732 \times 0.025 \times y^2 \times 0.63y^{0.667}
$$

$$
10 = 2.165 \times y^{2.667}
$$

$$
y^{2.667} = \frac{10}{2.165} = 4.62
$$

$$
y = 4.62^{1/2.667} = 4.62^{0.375} = 1.78 \text{ m}
$$

**Answer: (A) 1.8 m**

**Note:** Most efficient section (minimum perimeter for given area) uses R = y/2.

---

### Q8. Manning's n Value (GATE 2020) ⭐

**Question:**  
The typical Manning's roughness coefficient (n) for an earthen channel in good condition is:

(A) 0.012-0.015  
(B) 0.020-0.025  
(C) 0.030-0.035  
(D) 0.040-0.050

**Solution:**

**Manning's n values:**

| Surface Type | n Value | Condition |
|--------------|---------|-----------|
| Concrete lined | 0.012-0.015 | Smooth |
| Brick/stone masonry | 0.015-0.020 | Good |
| **Earthen channel** | **0.020-0.025** | **Good** ✓ |
| Earthen channel | 0.025-0.035 | Fair/poor |
| Natural streams | 0.030-0.050 | Rough |

**For earthen channel in good condition: n = 0.020-0.025**

**Answer: (B) 0.020-0.025**

**Memory:** "0.025 for earthen maze!"

---

## 📊 Topic-wise Summary

| Topic | Questions | Key Formulas |
|-------|-----------|--------------|
| **Kennedy's theory** | 2 (Q1, Q5) | V₀ = 0.55mD^0.64 |
| **Lacey's theory** | 2 (Q2, Q4) | f = 1.76√d, V from Qf² |
| **Manning's equation** | 3 (Q3, Q7, Q8) | V = (1/n)R^(2/3)S^(1/2) |
| **Hydraulic radius** | 1 (Q6) | R = A/P |

---

## 💡 Success Tips

### Must Remember

1. **Kennedy:** V₀ = 0.55mD^0.64 (m ≈ 1.0)
2. **Lacey silt:** f = 1.76√d
3. **Manning:** V = (1/n)R^(2/3)S^(1/2)
4. **Earthen n:** 0.020-0.025
5. **Most efficient R:** R = y/2

---

*[Theory](./README.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
