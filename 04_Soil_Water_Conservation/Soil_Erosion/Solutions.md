# 📝 Soil Erosion & Conservation - PYQ Solutions

> GATE Agricultural Engineering Previous Year Questions (2020-2024)

---

## 📋 Solutions Index

| # | Year | Topic | Difficulty | Time |
|---|------|-------|-----------|------|
| 1 | 2024 | USLE calculation | ⭐⭐ Medium | 4 min |
| 2 | 2024 | C factor | ⭐ Easy | 2 min |
| 3 | 2023 | LS factor | ⭐⭐⭐ Hard | 5 min |
| 4 | 2023 | Permissible soil loss | ⭐ Easy | 2 min |
| 5 | 2023 | P factor | ⭐⭐ Medium | 3 min |
| 6 | 2022 | USLE application | ⭐⭐ Medium | 4 min |
| 7 | 2022 | K factor | ⭐ Easy | 2 min |
| 8 | 2022 | Terrace spacing | ⭐⭐ Medium | 3 min |
| 9 | 2021 | Erosion types | ⭐ Easy | 2 min |
| 10 | 2021 | Conservation practice | ⭐⭐ Medium | 3 min |
| 11 | 2020 | USLE factors | ⭐⭐ Medium | 3 min |
| 12 | 2020 | Strip cropping | ⭐ Easy | 2 min |

**Total:** 12 questions | **Easy:** 5 | **Medium:** 6 | **Hard:** 1

---

## ✅ Question 1 (2024) - USLE Calculation

**[⭐⭐ Medium | 2 Marks | ~4 minutes]**

### Question
A field has the following erosion parameters:
- Rainfall erosivity factor (R) = 300
- Soil erodibility factor (K) = 0.35
- Slope length-steepness factor (LS) = 2.5
- Crop management factor (C) = 0.4
- Conservation practice factor (P) = 0.6

Calculate the average annual soil loss.

**Options:**
- (A) 31.5 t/ha/yr
- (B) 45.8 t/ha/yr
- (C) 63.0 t/ha/yr
- (D) 78.5 t/ha/yr

---

### Solution

**Given:**
- R = 300
- K = 0.35
- LS = 2.5
- C = 0.4
- P = 0.6

**USLE Formula:**
$$
\boxed{A = R \times K \times LS \times C \times P}
$$

**Calculation:**
$$
A = 300 \times 0.35 \times 2.5 \times 0.4 \times 0.6
$$

**Step-by-step:**
$$
= 300 \times 0.35 = 105
$$
$$
= 105 \times 2.5 = 262.5
$$
$$
= 262.5 \times 0.4 = 105
$$
$$
= 105 \times 0.6 = 63.0 \text{ t/ha/yr}
$$

**Answer: (C) 63.0 t/ha/yr ✓**

---

### Analysis
- Soil loss of **63 t/ha/yr** is **very high**
- Permissible for agriculture: 4.5-11.2 t/ha/yr
- This field needs **urgent conservation measures**
- Could reduce by:
  - Improving C factor (better crop cover) → 0.1 would give 15.8 t/ha/yr
  - Better practice (terracing P=0.2) → would give 21 t/ha/yr

---

## ✅ Question 2 (2024) - C Factor

**[⭐ Easy | 1 Mark | ~2 minutes]**

### Question
Which land use has the lowest crop management factor (C) in the Universal Soil Loss Equation?

**Options:**
- (A) Row crops
- (B) Small grains
- (C) Dense grass
- (D) Fallow land

---

### Solution

**C Factor values:**

| Land Use | C Factor |
|----------|----------|
| Fallow land (bare) | 1.0 (worst) |
| Row crops | 0.4-0.9 |
| Small grains | 0.2-0.5 |
| **Dense grass** | **0.01-0.05** ✓ |
| Forest | 0.001-0.01 (best) |

**Lower C = Better protection**

Dense grass provides excellent ground cover, protecting soil from raindrop impact and runoff.

**Answer: (C) Dense grass ✓**

---

### Concept Note
**C factor hierarchy (best to worst):**
Forest < Dense grass < Small grains < Row crops < Bare fallow

---

## ✅ Question 3 (2023) - LS Factor

**[⭐⭐⭐ Hard | 2 Marks | ~5 minutes]**

### Question
Calculate the LS factor for a field with:
- Slope length (λ) = 100 m
- Slope steepness (S) = 8%

Use simplified formula: $LS = (\lambda/22)^{0.5} \times (S/9)^{1.3}$

**Options:**
- (A) 1.85
- (B) 2.14
- (C) 2.58
- (D) 3.02

---

### Solution

**Given:**
- λ = 100 m
- S = 8%

**Formula:**
$$
LS = \left(\frac{\lambda}{22}\right)^{0.5} \times \left(\frac{S}{9}\right)^{1.3}
$$

---

**Step 1: Calculate L component**
$$
L = \left(\frac{100}{22}\right)^{0.5} = (4.545)^{0.5} = 2.132
$$

---

**Step 2: Calculate S component**
$$
S_{factor} = \left(\frac{8}{9}\right)^{1.3} = (0.889)^{1.3}
$$

To calculate $(0.889)^{1.3}$:
$$
\ln(0.889) = -0.1178
$$
$$
1.3 \times (-0.1178) = -0.1531
$$
$$
e^{-0.1531} = 0.858
$$

---

**Step 3: Combine**
$$
LS = 2.132 \times 0.858 = 1.829 \approx 1.85
$$

**Answer: (A) 1.85 ✓**

---

### Quick Check
**For standard reference (λ=22m, S=9%):**
$$
LS = 1.0 \times 1.0 = 1.0
$$

Our field:
- Longer slope (100 vs 22) → increases LS
- Slightly gentler slope (8% vs 9%) → decreases LS
- Net effect: LS ≈ 1.85 ✓

---

## ✅ Question 4 (2023) - Permissible Soil Loss

**[⭐ Easy | 1 Mark | ~2 minutes]**

### Question
What is the permissible soil loss for forest land?

**Options:**
- (A) 2.5 t/ha/yr
- (B) 5.0 t/ha/yr
- (C) 7.5 t/ha/yr
- (D) 11.2 t/ha/yr

---

### Solution

**Permissible soil loss values:**

| Land Use | Permissible Loss |
|----------|------------------|
| **Forest land** | **2.5 t/ha/yr** ⭐ |
| Agricultural land | 4.5-11.2 t/ha/yr |
| Pasture | 2.5-11.2 t/ha/yr |
| Marginal land | <2.5 t/ha/yr |

**Answer: (A) 2.5 t/ha/yr ✓**

---

### Concept
**Why lower for forest?**
- Forests have slower soil formation
- Cannot be plowed/replaced easily
- Ecological importance
- Need stricter conservation

---

## ✅ Question 5 (2023) - P Factor

**[⭐⭐ Medium | 2 Marks | ~3 minutes]**

### Question
A field with 10% slope is cultivated using contour farming. What is the approximate conservation practice factor (P)?

**Options:**
- (A) 0.3
- (B) 0.5
- (C) 0.7
- (D) 1.0

---

### Solution

**P factor for contour farming:**

| Slope (%) | P Factor |
|-----------|----------|
| 2-7 | 0.5-0.6 |
| **7-12** | **0.6-0.7** ✓ |
| 12-18 | 0.7-0.8 |
| 18-24 | 0.8-0.9 |

**10% slope falls in 7-12% range**

Typical value: **0.6-0.7**

**Answer: (C) 0.7 ✓**

---

### Comparison

| Practice | Slope 10% | P Factor |
|----------|-----------|----------|
| Up-down slope | - | 1.0 |
| **Contour farming** | ✓ | **0.6-0.7** |
| Strip cropping | - | 0.3-0.4 |
| Terracing | - | 0.1-0.3 |

---

## ✅ Question 6 (2022) - USLE Application

**[⭐⭐ Medium | 2 Marks | ~4 minutes]**

### Question
A watershed has R=250, K=0.30, LS=1.5, and is under dense grass cover (C=0.02). If no conservation practices are adopted (P=1.0), calculate the soil loss. Is this within permissible limits for agricultural land?

---

### Solution

**Given:**
- R = 250
- K = 0.30
- LS = 1.5
- C = 0.02 (dense grass)
- P = 1.0 (no practice)

---

**Step 1: Calculate soil loss**
$$
A = R \times K \times LS \times C \times P
$$

$$
A = 250 \times 0.30 \times 1.5 \times 0.02 \times 1.0
$$

$$
= 75 \times 1.5 \times 0.02 = 112.5 \times 0.02 = 2.25 \text{ t/ha/yr}
$$

**Soil loss: 2.25 t/ha/yr**

---

**Step 2: Compare with permissible**

Permissible for agriculture: **4.5-11.2 t/ha/yr**

**2.25 < 4.5**

**Yes, within permissible limits! ✓**

---

### Analysis
Dense grass (C=0.02) provides excellent protection:
- Even with no conservation practice (P=1.0)
- Soil loss remains very low (2.25 t/ha/yr)
- This demonstrates the power of good ground cover

If this were bare fallow (C=1.0):
$$
A = 250 \times 0.30 \times 1.5 \times 1.0 \times 1.0 = 112.5 \text{ t/ha/yr (excessive!)}
$$

---

## ✅ Question 7 (2022) - K Factor

**[⭐ Easy | 1 Mark | ~2 minutes]**

### Question
Which soil texture generally has the highest erodibility factor (K)?

**Options:**
- (A) Sand
- (B) Silt loam
- (C) Clay loam
- (D) Clay

---

### Solution

**K factor by texture:**

| Soil Texture | K Value | Erodibility |
|--------------|---------|-------------|
| Sand | 0.05-0.10 | Low |
| Sandy loam | 0.15-0.25 | Moderate |
| Loam | 0.25-0.40 | Moderate-High |
| **Silt loam** | **0.40-0.50** | **Highest** ⭐ |
| Clay loam | 0.20-0.35 | Moderate |
| Clay | 0.10-0.25 | Low |

**Answer: (B) Silt loam ✓**

---

### Why Silt Loam?

**Sand:**
- Large particles, heavy
- Hard to detach
- But easily transported once detached

**Silt:**
- Small particles (0.002-0.05 mm)
- **Easily detached AND easily transported**
- Low cohesion
- Forms hard crust when dry

**Clay:**
- Very small, cohesive
- Forms aggregates
- Harder to erode

**Silt loam = worst combination!**

---

## ✅ Question 8 (2022) - Terrace Spacing

**[⭐⭐ Medium | 2 Marks | ~3 minutes]**

### Question
Calculate the vertical interval for terraces on a field with 12% slope using the formula: VI = 0.3S + 1.0 (where S is in %, VI in meters).

**Options:**
- (A) 2.8 m
- (B) 3.6 m
- (C) 4.6 m
- (D) 5.2 m

---

### Solution

**Given:**
- Slope, S = 12%
- Formula: VI = 0.3S + 1.0

**Calculation:**
$$
VI = 0.3 \times 12 + 1.0
$$

$$
= 3.6 + 1.0 = 4.6 \text{ m}
$$

**Answer: (C) 4.6 m ✓**

---

### Interpretation
**Vertical interval = 4.6 m**

This means:
- Vertical drop between terrace crests = 4.6 m
- On 12% slope (rise/run = 12/100)
- Horizontal distance = 4.6 / 0.12 = **38.3 m**

**Terrace spacing ≈ 38 m** (horizontal)

---

### Check
Steeper slope → Smaller VI → Closer terraces ✓

---

## ✅ Question 9 (2021) - Erosion Types

**[⭐ Easy | 1 Mark | ~2 minutes]**

### Question
Which type of soil erosion is most difficult to detect in early stages but removes valuable topsoil uniformly?

**Options:**
- (A) Splash erosion
- (B) Sheet erosion
- (C) Rill erosion
- (D) Gully erosion

---

### Solution

**Characteristics of erosion types:**

**Splash erosion:**
- Visible raindrop impacts
- Easy to observe

**Sheet erosion:**
- **Uniform removal of thin layer**
- **Difficult to detect initially** ✓
- **Most destructive** (removes topsoil uniformly)
- Indicators appear later (exposed subsoil, poor crop growth)

**Rill erosion:**
- Visible channels
- Easy to see

**Gully erosion:**
- Very obvious
- Large channels

**Answer: (B) Sheet erosion ✓**

---

### Key Point
**Sheet erosion** is called **"silent killer"**
- Farmer may not notice until significant loss
- By the time detected, damage is substantial
- Prevention through mulching, cover crops essential

---

## ✅ Question 10 (2021) - Conservation Practice

**[⭐⭐ Medium | 2 Marks | ~3 minutes]**

### Question
Arrange the following conservation practices in order of increasing effectiveness (least to most effective):
I. Contour farming
II. Terracing
III. Strip cropping
IV. Up-down slope cultivation

**Options:**
- (A) IV, I, III, II
- (B) I, III, IV, II
- (C) IV, III, I, II
- (D) I, IV, III, II

---

### Solution

**P factor values (lower = more effective):**

| Practice | P Factor | Effectiveness |
|----------|----------|---------------|
| **Up-down slope** | **1.0** | None (baseline) |
| **Contour farming** | **0.5-0.7** | Moderate |
| **Strip cropping** | **0.25-0.40** | Good |
| **Terracing** | **0.10-0.30** | **Best** |

---

**Order (least → most effective):**
1. **IV. Up-down slope** (P = 1.0) - Worst
2. **I. Contour farming** (P = 0.6) - Moderate
3. **III. Strip cropping** (P = 0.3) - Good
4. **II. Terracing** (P = 0.2) - Best

**Answer: (A) IV, I, III, II ✓**

---

### Soil Loss Reduction

**If baseline (up-down) = 100 t/ha/yr:**
- Contour: 60 t/ha/yr (40% reduction)
- Strip cropping: 30 t/ha/yr (70% reduction)
- Terracing: 20 t/ha/yr (80% reduction)

---

## ✅ Question 11 (2020) - USLE Factors

**[⭐⭐ Medium | 2 Marks | ~3 minutes]**

### Question
In the Universal Soil Loss Equation, if all other factors remain constant and the LS factor is doubled, how does it affect soil loss?

Also, what happens if C factor is halved?

---

### Solution

**USLE:**
$$
A = R \times K \times LS \times C \times P
$$

---

### Part 1: LS doubled

**Original:**
$$
A_1 = R \times K \times LS \times C \times P
$$

**After doubling LS:**
$$
A_2 = R \times K \times (2 \times LS) \times C \times P
$$

$$
A_2 = 2 \times (R \times K \times LS \times C \times P) = 2A_1
$$

**Soil loss doubles ✓**

---

### Part 2: C halved

**After halving C:**
$$
A_3 = R \times K \times LS \times \frac{C}{2} \times P
$$

$$
A_3 = \frac{1}{2} \times (R \times K \times LS \times C \times P) = \frac{A_1}{2}
$$

**Soil loss reduced by half ✓**

---

### Key Insight
**USLE is multiplicative:**
- Change in any factor → proportional change in soil loss
- Double LS → Double loss
- Halve C → Halve loss
- **Very sensitive to all factors!**

---

## ✅ Question 12 (2020) - Strip Cropping

**[⭐ Easy | 1 Mark | ~2 minutes]**

### Question
In contour strip cropping, what is the typical width of each strip?

**Options:**
- (A) 5-10 m
- (B) 15-30 m
- (C) 40-60 m
- (D) 80-100 m

---

### Solution

**Strip cropping specifications:**

**Strip width:**
- Typical: **15-30 m** ⭐
- Depends on:
  - Slope steepness
  - Crop type
  - Machinery size

**Too narrow (<15 m):**
- Difficult to farm
- Frequent turns

**Too wide (>30 m):**
- Loses effectiveness
- More erosion within strip

**Answer: (B) 15-30 m ✓**

---

### Design Considerations

**Strip pattern:**
- Alternate: Dense crop ↔ Regular crop
- Example: Grass strip (15m) ↔ Corn (20m)

**Benefits:**
- Dense strip traps sediment
- Reduces runoff velocity
- 50-75% erosion reduction

---

## 📊 Topic-wise Summary

| Topic | Questions | Marks | Priority |
|-------|-----------|-------|----------|
| **USLE calculation** | 4 | 8 | 🔥 High |
| **C and P factors** | 3 | 4 | 🔥 High |
| **LS factor** | 1 | 2 | Medium |
| **K factor** | 1 | 1 | Medium |
| **Erosion types** | 1 | 1 | Medium |
| **Terrace spacing** | 1 | 2 | Medium |
| **Conservation practices** | 1 | 2 | Medium |

---

## 🎯 Key Formulas Used

**1. USLE (Most Important!):**
$$
A = R \times K \times LS \times C \times P
$$

**2. LS Factor:**
$$
LS = \left(\frac{\lambda}{22}\right)^{0.5} \times \left(\frac{S}{9}\right)^{1.3}
$$

**3. Terrace spacing:**
$$
VI = 0.3S + 1.0
$$

---

## 💡 Common Mistakes

1. **USLE units:** Result is in t/ha/yr (not kg or other)
2. **P factor:** Lower is better (1.0 = worst, no practice)
3. **C factor:** Lower is better (1.0 = bare fallow)
4. **Silt loam:** Highest K (most erodible), not sand
5. **Sheet erosion:** Hard to detect, not splash erosion
6. **Strip width:** 15-30 m, not 5-10 m

---

**Last Updated:** November 2025  
**Total Solutions:** 12  
**Next:** [CheatSheet](./CheatSheet.md)

---

*Master USLE for GATE success! 🎯*
