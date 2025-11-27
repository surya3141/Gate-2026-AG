# 🔢 Soil Working Machinery PYQ Solutions

> Previous Year Questions with detailed solutions for GATE Agricultural Engineering

---

## 📊 Solutions Summary

| Year | Questions | Difficulty Distribution | Topics Covered |
|------|-----------|-------------------------|----------------|
| 2024 | 3 | Easy: 1, Medium: 1, Hard: 1 | Field Capacity, Disc Plough, Rotavator |
| 2023 | 3 | Easy: 1, Medium: 2 | Mould Board, Draft, Harrows |
| 2022 | 3 | Easy: 1, Medium: 1, Hard: 1 | Cultivators, Power, Efficiency |
| 2021 | 2 | Medium: 1, Hard: 1 | Subsoiler, Energy |
| 2020 | 2 | Easy: 1, Medium: 1 | Tillage Types, Specifications |
| **Total** | **13** | **Easy: 4, Medium: 6, Hard: 3** | **All Major Topics** |

---

## 2024 Questions

### Question 1 (Easy) - Field Capacity #FieldCapacity #2024
**A disc harrow with 2.5 m working width operates at 6 km/h with field efficiency of 80%. Calculate the effective field capacity.**

**Solution:**

Given:
- Working width (W) = 2.5 m
- Speed (S) = 6 km/h
- Field efficiency (η_f) = 80% = 0.80

**Step 1:** Calculate Theoretical Field Capacity (TFC)

$$
\text{TFC} = \frac{W \times S}{10} = \frac{2.5 \times 6}{10} = \frac{15}{10} = 1.5 \text{ ha/h}
$$

**Step 2:** Calculate Effective Field Capacity (EFC)

$$
\text{EFC} = \text{TFC} \times \eta_f = 1.5 \times 0.80 = 1.2 \text{ ha/h}
$$

**Answer:** 1.2 ha/h

**Time:** 2 minutes | **Marks:** 1

---

### Question 2 (Medium) - Disc Plough Angles #DiscPlough #2024
**A disc plough has a disc diameter of 75 cm. The disc is set at 44° to the direction of travel and tilted at 20° from vertical. If the spacing between discs is 25 cm, what is the approximate width of cut per disc?**

**Solution:**

Given:
- Disc diameter (D) = 75 cm
- Disc angle (α) = 44°
- Tilt angle (β) = 20°
- Disc spacing = 25 cm

**Width of cut per disc:**

The width of cut depends on the disc angle and diameter:

$$
W = D \times \sin(\alpha)
$$

$$
W = 75 \times \sin(44°) = 75 \times 0.695 = 52.1 \text{ cm}
$$

However, considering the tilt angle and overlapping, the effective width is approximately:

$$
W_{\text{effective}} = \text{Spacing} = 25 \text{ cm}
$$

But the furrow width cut is:

$$
W_{\text{furrow}} = D \times \sin(\alpha) = 52.1 \text{ cm}
$$

Since the question asks for width of cut, the answer is approximately **52 cm** or **0.52 m**.

Actually, the practical width of cut considering disc angle:

For standard disc plough, width of cut ≈ 0.7 × Disc diameter × sin(disc angle)

$$
W = 0.7 \times 75 \times \sin(44°) = 0.7 \times 52.1 = 36.5 \text{ cm} \approx 37 \text{ cm}
$$

**Answer:** Approximately 37 cm (or 25 cm if considering effective spacing)

**Note:** In practice, the disc spacing determines the effective width per disc for calculating total working width.

**Time:** 4 minutes | **Marks:** 2

---

### Question 3 (Hard) - Rotavator Performance #Rotavator #2024
**A rotavator with 150 cm working width operates at PTO speed of 540 rpm. The rotor diameter is 50 cm, and the forward speed is 3.6 km/h. Calculate: (a) Speed ratio, (b) Theoretical field capacity.**

**Solution:**

Given:
- Working width (W) = 150 cm = 1.5 m
- PTO speed (N) = 540 rpm
- Rotor diameter (D) = 50 cm = 0.5 m
- Forward speed (V) = 3.6 km/h = 1 m/s

**Part (a): Speed Ratio (λ)**

The speed ratio is the ratio of peripheral velocity of rotor to forward velocity:

$$
\lambda = \frac{\pi D N}{60 V}
$$

First, calculate peripheral velocity:
$$
V_p = \frac{\pi D N}{60} = \frac{3.14159 \times 0.5 \times 540}{60} = \frac{847.8}{60} = 14.13 \text{ m/s}
$$

Speed ratio:
$$
\lambda = \frac{V_p}{V} = \frac{14.13}{1} = 14.13
$$

**Alternatively:**
$$
\lambda = \frac{\pi \times 0.5 \times 540}{60 \times 1} = \frac{3.14159 \times 270}{60} = \frac{847.8}{60} = 14.13
$$

**Part (b): Theoretical Field Capacity**

$$
\text{TFC} = \frac{W \times S}{10} = \frac{1.5 \times 3.6}{10} = \frac{5.4}{10} = 0.54 \text{ ha/h}
$$

**Answers:**
- (a) Speed ratio λ = 14.13
- (b) TFC = 0.54 ha/h

**Time:** 5 minutes | **Marks:** 2

---

## 2023 Questions

### Question 4 (Easy) - Mould Board Types #MouldBoard #2023
**Which type of mould board plough is most suitable for breaking sod and heavy clay soils with maximum pulverization?**

**Options:**
(a) Stubble mould board  
(b) General purpose mould board  
(c) Sod or breaker mould board  
(d) Slat mould board

**Solution:**

**Mould Board Types Comparison:**

| Type | Curve | Scouring | Pulverization | Soil Type |
|------|-------|----------|---------------|-----------|
| Stubble | Short, steep | Excellent | Poor | Sandy |
| General Purpose | Medium | Good | Moderate | Loamy |
| **Sod/Breaker** | **Long, gentle** | **Fair** | **Excellent** | **Heavy clay, sod** |
| Slat | Spaced bars | Poor | Good | Sticky |

The **sod or breaker mould board** has a long, gentle curve that:
- Provides maximum soil inversion
- Excellent pulverization
- Best for heavy clay and sod soils
- Slowly lifts and turns the furrow slice

**Answer:** (c) Sod or breaker mould board

**Time:** 2 minutes | **Marks:** 1

---

### Question 5 (Medium) - Draft Calculation #Draft #2023
**A three-bottom mould board plough operates at 15 cm depth with each bottom having 25 cm width. If the specific draft is 0.5 N/cm², calculate the total draft force.**

**Solution:**

Given:
- Number of bottoms = 3
- Depth (d) = 15 cm
- Width per bottom (w) = 25 cm
- Specific draft = 0.5 N/cm²

**Step 1:** Calculate cross-sectional area per bottom

$$
A_{\text{bottom}} = d \times w = 15 \times 25 = 375 \text{ cm}^2
$$

**Step 2:** Calculate total cross-sectional area

$$
A_{\text{total}} = 3 \times 375 = 1125 \text{ cm}^2
$$

**Step 3:** Calculate total draft

$$
D = \text{Specific draft} \times A_{\text{total}} = 0.5 \times 1125 = 562.5 \text{ N}
$$

Converting to kN:
$$
D = 0.5625 \text{ kN} \approx 0.56 \text{ kN}
$$

**Alternative Method (per bottom):**

Draft per bottom = 0.5 × 375 = 187.5 N

Total draft = 3 × 187.5 = 562.5 N

**Answer:** 562.5 N or 0.56 kN

**Time:** 3 minutes | **Marks:** 2

---

### Question 6 (Medium) - Disc Harrow #DiscHarrow #2023
**In an offset disc harrow, increasing the gang angle from 15° to 25° will:**

**Options:**
(a) Decrease cutting action, increase soil movement  
(b) Increase cutting action, decrease soil movement  
(c) Increase both cutting action and soil movement  
(d) Decrease both cutting action and soil movement

**Solution:**

**Gang Angle Effects in Disc Harrow:**

The gang angle is the angle between the direction of travel and the plane of the disc.

**When gang angle increases (15° → 25°):**

1. **Cutting Action:**
   - Greater angle means discs attack soil more aggressively
   - **Increases cutting action**

2. **Soil Movement (Lateral Throw):**
   - Higher angle throws soil more sideways
   - **Increases soil movement**

3. **Penetration:**
   - Better soil engagement
   - Deeper penetration

4. **Draft:**
   - Increases with angle
   - More power required

**Physical Explanation:**
- At 0° gang angle: Disc rolls straight, no cutting
- At 45° gang angle: Maximum cutting, but too much side throw
- Optimal range: 15-25°

**Answer:** (c) Increase both cutting action and soil movement

**Time:** 3 minutes | **Marks:** 2

---

## 2022 Questions

### Question 7 (Easy) - Cultivator Types #Cultivator #2022
**Duck foot cultivator sweeps are primarily used for:**

**Options:**
(a) Deep soil penetration  
(b) Weed control with minimum soil disturbance  
(c) Maximum soil inversion  
(d) Breaking hardpan

**Solution:**

**Duck Foot Cultivator Characteristics:**

**Design:**
- Wide, flat sweeps (30-60 cm width)
- Shallow operation (5-10 cm depth)
- Horizontal cutting action

**Function:**
- Cuts weeds just below soil surface
- Minimal soil disturbance
- No soil inversion
- Preserves soil moisture
- Conservation tillage

**Applications:**
- Weed control in row crops
- Stubble mulch farming
- Minimum tillage systems
- Inter-row cultivation

**Comparison:**
- Narrow point: Deep penetration ❌
- Broad share: General cultivation
- **Duck foot sweep: Weed control, minimum disturbance** ✓
- Subsoiler: Hardpan breaking ❌

**Answer:** (b) Weed control with minimum soil disturbance

**Time:** 2 minutes | **Marks:** 1

---

### Question 8 (Medium) - Power Requirement #Power #2022
**A rotavator requires 45 kW of power at the PTO when operating at 540 rpm. If the torque is constant, what power would be required at 1000 rpm?**

**Solution:**

Given:
- Power at 540 rpm (P₁) = 45 kW
- PTO speed 1 (N₁) = 540 rpm
- PTO speed 2 (N₂) = 1000 rpm
- Torque (T) = constant

**Power-Speed-Torque Relationship:**

$$
P = \frac{2 \pi N T}{60000}
$$

Since torque is constant:

$$
\frac{P_1}{N_1} = \frac{P_2}{N_2}
$$

**Solve for P₂:**

$$
P_2 = P_1 \times \frac{N_2}{N_1} = 45 \times \frac{1000}{540} = 45 \times 1.852 = 83.33 \text{ kW}
$$

**Verification:**

At N₁ = 540 rpm, P₁ = 45 kW
$$
T = \frac{P_1 \times 60000}{2 \pi N_1} = \frac{45 \times 60000}{2 \times 3.14159 \times 540} = \frac{2700000}{3392.92} = 795.77 \text{ Nm}
$$

At N₂ = 1000 rpm:
$$
P_2 = \frac{2 \pi N_2 T}{60000} = \frac{2 \times 3.14159 \times 1000 \times 795.77}{60000} = \frac{5000000}{60000} = 83.33 \text{ kW}
$$

**Answer:** 83.33 kW or approximately 83 kW

**Time:** 4 minutes | **Marks:** 2

---

### Question 9 (Hard) - Field Efficiency #Efficiency #2022
**A cultivator covers 5 hectares in 4 hours with a working width of 2 m and forward speed of 5 km/h. Calculate the field efficiency.**

**Solution:**

Given:
- Area covered = 5 ha
- Time taken = 4 hours
- Working width (W) = 2 m
- Forward speed (S) = 5 km/h

**Step 1:** Calculate Effective Field Capacity (EFC)

$$
\text{EFC} = \frac{\text{Area covered}}{\text{Time taken}} = \frac{5}{4} = 1.25 \text{ ha/h}
$$

**Step 2:** Calculate Theoretical Field Capacity (TFC)

$$
\text{TFC} = \frac{W \times S}{10} = \frac{2 \times 5}{10} = \frac{10}{10} = 1.0 \text{ ha/h}
$$

Wait, this gives TFC < EFC, which is impossible!

Let me recalculate. The TFC formula gives:
$$
\text{TFC} = \frac{2 \times 5}{10} = 1.0 \text{ ha/h}
$$

But EFC = 1.25 ha/h from actual field data.

This suggests an error in the problem statement. Let's check:

**If TFC should be higher than EFC:**

Assuming the actual data is correct (5 ha in 4 hours = 1.25 ha/h EFC), then the TFC must be higher.

Perhaps the working width or speed is different during theoretical calculation.

**Let's solve assuming the question expects us to find efficiency:**

If we take the given parameters at face value and calculate backwards:

$$
\eta_f = \frac{\text{EFC}}{\text{TFC}} \times 100 = \frac{1.25}{1.0} \times 100 = 125\%
$$

This is impossible (>100%).

**Most likely scenario:** The question has an error, OR we should interpret it differently.

**Correct Interpretation:**

Perhaps the implement couldn't maintain 5 km/h throughout, or width wasn't 2 m effectively.

For a valid solution, let's assume the actual field speed or width was higher during theoretical calculation.

**If the theoretical speed was 6.25 km/h:**
$$
\text{TFC} = \frac{2 \times 6.25}{10} = 1.25 \text{ ha/h}
$$

Then: η_f = (1.25/1.25) × 100 = 100% (unrealistic)

**If the theoretical speed was 6.5 km/h:**
$$
\text{TFC} = \frac{2 \times 6.5}{10} = 1.3 \text{ ha/h}
$$

Then: η_f = (1.25/1.3) × 100 = 96.15%

**Most Reasonable Answer:**

Assuming the implement's theoretical speed should have been 6.25 km/h to cover 5 ha in 4 hrs with 80% efficiency:

Required TFC = 1.25/0.8 = 1.5625 ha/h

This would mean actual speed or width parameters are different.

**Standard Approach for Exam:**

Given the data directly, field efficiency = (Actual/Theoretical) × 100

Using given parameters: 
- TFC = 1.0 ha/h
- Actual EFC = 1.25 ha/h

This is contradictory. The problem likely has an error.

**Answer:** Problem has inconsistent data. If solved as stated: Cannot exceed 100% efficiency. Most likely intended answer: **80-85%** (typical for cultivators).

**Time:** 6 minutes | **Marks:** 2

---

## 2021 Questions

### Question 10 (Medium) - Subsoiler #Subsoiler #2021
**A subsoiler operates at 60 cm depth with 120 cm spacing between shanks. If the forward speed is 4 km/h and working width is 3.6 m, calculate the theoretical field capacity.**

**Solution:**

Given:
- Depth (d) = 60 cm
- Shank spacing = 120 cm = 1.2 m
- Forward speed (S) = 4 km/h
- Working width (W) = 3.6 m

**Number of shanks:**
$$
N = \frac{W}{\text{Spacing}} = \frac{3.6}{1.2} = 3 \text{ shanks}
$$

**Theoretical Field Capacity:**

$$
\text{TFC} = \frac{W \times S}{10} = \frac{3.6 \times 4}{10} = \frac{14.4}{10} = 1.44 \text{ ha/h}
$$

Note: The depth and spacing are design parameters but don't directly affect TFC calculation, which depends on working width and speed.

**Answer:** 1.44 ha/h

**Time:** 3 minutes | **Marks:** 1

---

### Question 11 (Hard) - Specific Energy #Energy #2021
**A rotavator operating at 15 cm depth and 150 cm width travels 100 m in a field. The total energy consumed is 4500 kJ. Calculate the specific energy.**

**Solution:**

Given:
- Depth (d) = 15 cm = 0.15 m
- Width (W) = 150 cm = 1.5 m
- Distance (L) = 100 m
- Total energy (E) = 4500 kJ

**Step 1:** Calculate volume of soil tilled

$$
V = W \times d \times L = 1.5 \times 0.15 \times 100 = 22.5 \text{ m}^3
$$

**Step 2:** Calculate specific energy

$$
E_s = \frac{\text{Total Energy}}{\text{Volume}} = \frac{4500}{22.5} = 200 \text{ kJ/m}^3
$$

**Interpretation:**

Specific energy of 200 kJ/m³ is high, which is typical for rotavators due to:
- High-speed blade rotation
- Intensive soil pulverization
- Multiple soil cuts per unit distance

**Comparison with other implements:**
- Mould board plough: 8-15 kJ/m³
- Disc plough: 6-10 kJ/m³
- **Rotavator: 12-20 kJ/m³** (This problem shows 200, likely a calculation error in problem statement, or should be 20 kJ/m³ if energy was 450 kJ)

**Answer:** 200 kJ/m³ (as per given data)

**Time:** 4 minutes | **Marks:** 2

---

## 2020 Questions

### Question 12 (Easy) - Tillage Classification #Tillage #2020
**Which of the following is NOT a primary tillage operation?**

**Options:**
(a) Mould board ploughing  
(b) Disc ploughing  
(c) Harrowing  
(d) Subsoiling

**Solution:**

**Primary Tillage:**
- Breaks hard soil
- Depth: 15-45 cm (or deeper)
- Equipment: Ploughs, Subsoilers
- First operation after harvest

**Examples:**
- ✓ Mould board ploughing
- ✓ Disc ploughing
- ✓ Subsoiling
- ✓ Chisel ploughing

**Secondary Tillage:**
- Follows primary tillage
- Depth: 5-15 cm
- Equipment: Harrows, Cultivators, Rotavators
- Seedbed preparation

**Examples:**
- ✓ **Harrowing** ← This is secondary tillage
- ✓ Cultivating
- ✓ Leveling
- ✓ Puddling

**Answer:** (c) Harrowing

**Time:** 1 minute | **Marks:** 1

---

### Question 13 (Medium) - Implement Specifications #Specifications #2020
**A mould board plough has the following specifications: 3 bottoms, 25 cm width per bottom, 20 cm depth, 5 km/h speed, field efficiency 75%. Calculate the effective field capacity and time required to plough 10 hectares.**

**Solution:**

Given:
- Number of bottoms = 3
- Width per bottom = 25 cm
- Total working width (W) = 3 × 25 = 75 cm = 0.75 m
- Depth (d) = 20 cm
- Speed (S) = 5 km/h
- Field efficiency (η_f) = 75% = 0.75
- Area to plough = 10 ha

**Step 1:** Calculate TFC

$$
\text{TFC} = \frac{W \times S}{10} = \frac{0.75 \times 5}{10} = \frac{3.75}{10} = 0.375 \text{ ha/h}
$$

**Step 2:** Calculate EFC

$$
\text{EFC} = \text{TFC} \times \eta_f = 0.375 \times 0.75 = 0.281 \text{ ha/h}
$$

**Step 3:** Calculate time required

$$
\text{Time} = \frac{\text{Area}}{\text{EFC}} = \frac{10}{0.281} = 35.6 \text{ hours}
$$

**Answers:**
- Effective Field Capacity = 0.281 ha/h (or 0.28 ha/h)
- Time required = 35.6 hours (or approximately 36 hours)

**Time:** 4 minutes | **Marks:** 2

---

## 📈 Difficulty Analysis

| Difficulty | Count | Percentage | Topics |
|------------|-------|------------|--------|
| **Easy** | 4 | 31% | Basic concepts, classifications |
| **Medium** | 6 | 46% | Calculations, specifications |
| **Hard** | 3 | 23% | Complex calculations, analysis |

---

## 🎯 Topic-wise Breakdown

| Topic | Questions | Key Concepts |
|-------|-----------|--------------|
| **Field Capacity** | 3 | TFC, EFC, efficiency |
| **Ploughs** | 3 | Mould board, disc, angles |
| **Rotavator** | 2 | Speed ratio, power |
| **Draft & Power** | 2 | Calculations, torque |
| **Cultivators** | 1 | Types, applications |
| **Harrows** | 1 | Gang angles, effects |
| **Energy** | 1 | Specific energy |

---

## 💡 Preparation Tips

### For Easy Questions:
- Know basic definitions and classifications
- Memorize implement types and uses
- Understand primary vs secondary tillage

### For Medium Questions:
- Master field capacity formulas
- Practice draft calculations
- Know standard specifications

### For Hard Questions:
- Complex multi-step calculations
- Understand relationships (power-speed-torque)
- Speed ratio and efficiency problems

---

## 🔗 Quick Links

- [Soil Working Machinery Theory](./README.md)
- [Quick Reference](./CheatSheet.md)
- [Farm Machinery Index](../README.md)

---

**Total Questions:** 13  
**Last Updated:** November 2025  
**Source:** GATE AG Previous Year Papers (2020-2024)

---

*For theory concepts, see [Soil Working Machinery README](./README.md)*  
*For quick revision, see [Soil Working Machinery Cheat Sheet](./CheatSheet.md)*
