# 🔢 Seeding & Planting Equipment PYQ Solutions

> Previous Year Questions with detailed solutions for GATE Agricultural Engineering

---

## 📊 Solutions Summary

| Year | Questions | Difficulty Distribution | Topics Covered |
|------|-----------|-------------------------|----------------|
| 2024 | 3 | Easy: 1, Medium: 2 | Seed Rate, Planter, Quality Index |
| 2023 | 2 | Easy: 1, Medium: 1 | Population, Metering |
| 2022 | 3 | Easy: 1, Medium: 1, Hard: 1 | Spacing, Transplanter, Draft |
| 2021 | 2 | Medium: 2 | Seed Drill, Furrow Opener |
| 2020 | 2 | Easy: 1, Medium: 1 | Broadcasting, Cell Size |
| **Total** | **12** | **Easy: 4, Medium: 7, Hard: 1** | **All Major Topics** |

---

## 2024 Questions

### Question 1 (Easy) - Seed Rate #SeedRate #2024
**A 9-row seed drill with 20 cm row spacing sows wheat at 100 kg/ha. If 1000-seed weight is 40 g, calculate the number of seeds per meter of row.**

**Solution:**

Given:
- Number of rows (n) = 9
- Row spacing (S) = 20 cm = 0.2 m
- Seed rate (Q) = 100 kg/ha
- 1000-seed weight (W) = 40 g

**Step 1:** Calculate seeds per hectare

$$
\text{Total seeds/ha} = \frac{Q \times 1000}{W} = \frac{100 \times 1000}{40} = \frac{100000}{40} = 2,500,000 \text{ seeds/ha}
$$

**Step 2:** Calculate row length per hectare

$$
\text{Row length/ha} = \frac{10000 \text{ m}^2}{0.2 \text{ m}} = 50,000 \text{ m}
$$

**Step 3:** Calculate seeds per meter of row

$$
\text{Seeds/m} = \frac{2,500,000}{50,000} = 50 \text{ seeds/m}
$$

**Alternative Method:**

$$
\text{Seeds/m/row} = \frac{Q \times 100}{n \times S \times W}
$$

$$
= \frac{100 \times 100}{9 \times 20 \times 40/1000} = \frac{10000}{72} \approx 139 \text{ seeds/m (total)}
$$

Wait, this doesn't match. Let me recalculate properly.

**Correct Approach:**

For 1 hectare = 10,000 m²

Area per row = 10,000 m² / (10,000 m / 0.2 m) = Length × 0.2

Length of one row in 1 ha with 0.2 m spacing:
$$
\text{Length} = \frac{10000}{0.2 \times \text{Number of passes}}
$$

Actually, simpler approach:

Seeds per hectare = 2,500,000

Total row length in 1 ha = (1 ha area) / (row spacing) = 10,000 m² / 0.2 m = 50,000 m (total for all rows)

But we have 9 rows, so in one pass of drill covering 9 × 0.2 = 1.8 m width:

Length to cover 1 ha = 10,000 / 1.8 = 5,555.56 m

Each row travels 5,555.56 m

Total row length for all 9 rows = 9 × 5,555.56 = 50,000 m

Seeds per meter = 2,500,000 / 50,000 = 50 seeds/m per row

**Answer:** 50 seeds per meter of row

**Time:** 3 minutes | **Marks:** 1

---

### Question 2 (Medium) - Precision Planter #Planter #2024
**A precision maize planter has a cell-type metering plate with 24 cells rotating at 18 rpm. The planter moves at 5.4 km/h (1.5 m/s). Calculate the plant spacing.**

**Solution:**

Given:
- Number of cells (N_c) = 24
- Plate RPM (N_p) = 18 rpm
- Forward speed (V) = 5.4 km/h = 1.5 m/s

**Plant spacing formula:**

$$
\text{Plant spacing (m)} = \frac{V}{N_c \times N_p / 60}
$$

**Step 1:** Calculate seed drop rate (seeds per second)

$$
\text{Seeds/sec} = \frac{N_c \times N_p}{60} = \frac{24 \times 18}{60} = \frac{432}{60} = 7.2 \text{ seeds/sec}
$$

**Step 2:** Calculate plant spacing

$$
\text{Spacing} = \frac{V}{\text{Seeds/sec}} = \frac{1.5}{7.2} = 0.208 \text{ m} = 20.8 \text{ cm}
$$

**Verification:**
In 1 minute:
- Distance traveled = 1.5 × 60 = 90 m
- Seeds dropped = 24 × 18 = 432 seeds
- Spacing = 90/432 = 0.208 m ✓

**Answer:** 20.8 cm or approximately 21 cm

**Time:** 3 minutes | **Marks:** 2

---

### Question 3 (Medium) - Quality of Feed Index #QualityIndex #2024
**In a planter performance test, out of 100 seed spacings measured, 8 were more than 1.5 times the mean spacing, and 5 were less than 0.5 times the mean spacing. Calculate the quality of feed index.**

**Solution:**

Given:
- Total spacings measured = 100
- Spacings > 1.5 × mean (Miss Index) = 8
- Spacings < 0.5 × mean (Multiple Index) = 5

**Quality of Feed Index Formula:**

**Miss Index (M):**
$$
M = \frac{\text{Number of misses}}{\text{Total}} \times 100 = \frac{8}{100} \times 100 = 8\%
$$

**Multiple Index (D):**
$$
D = \frac{\text{Number of multiples}}{\text{Total}} \times 100 = \frac{5}{100} \times 100 = 5\%
$$

**Quality Index (Q):**
$$
Q = 100 - (M + D) = 100 - (8 + 5) = 100 - 13 = 87\%
$$

**Interpretation:**
- Q > 85%: Good planting quality ✓
- Q = 70-85%: Acceptable
- Q < 70%: Poor

**Answer:** Quality of feed index = 87%

**Time:** 2 minutes | **Marks:** 2

---

## 2023 Questions

### Question 4 (Easy) - Plant Population #Population #2023
**Calculate the plant population per hectare for a crop planted with 60 cm row spacing and 20 cm plant spacing.**

**Solution:**

Given:
- Row spacing (R) = 60 cm = 0.6 m
- Plant spacing (S) = 20 cm = 0.2 m

**Plant population formula:**

$$
P = \frac{10000}{R \times S}
$$

Where 10,000 m² = 1 hectare

$$
P = \frac{10000}{0.6 \times 0.2} = \frac{10000}{0.12} = 83,333 \text{ plants/ha}
$$

**Verification:**
- Area per plant = 0.6 × 0.2 = 0.12 m²
- Number of plants in 10,000 m² = 10,000 / 0.12 = 83,333 ✓

**Answer:** 83,333 plants/ha (or approximately 83,000 plants/ha)

**Time:** 2 minutes | **Marks:** 1

---

### Question 5 (Medium) - Fluted Roller Metering #Metering #2023
**A seed drill has a fluted roller with effective length of 15 cm exposed. The roller diameter is 5 cm and rotates at 30 rpm. The ground wheel diameter is 40 cm. Calculate the forward speed of the drill.**

**Solution:**

Given:
- Effective flute length (L) = 15 cm
- Roller diameter (d_r) = 5 cm
- Roller RPM (N_r) = 30 rpm
- Ground wheel diameter (D_g) = 40 cm

**Relationship between ground wheel and roller:**

Assuming direct drive or known gear ratio (typically 1:1 for this problem):

**Ground wheel RPM = Roller RPM** (if 1:1 drive)

Actually, we need more information about the drive ratio. Let's assume the roller is driven by the ground wheel.

**Forward speed from ground wheel:**

$$
V = \frac{\pi D_g N_g}{60}
$$

If the ground wheel and roller have 1:1 speed ratio (both 30 rpm):

$$
V = \frac{3.14159 \times 0.4 \times 30}{60} = \frac{37.7}{60} = 0.628 \text{ m/s}
$$

Converting to km/h:
$$
V = 0.628 \times 3.6 = 2.26 \text{ km/h}
$$

**Alternative interpretation:**

If the roller speed determines the mechanism:

The forward speed depends on the ground wheel circumference and RPM:

$$
V = \pi D_g \times N_g / 60 = 3.14159 \times 0.4 \times 30 / 60 = 0.628 \text{ m/s} = 2.26 \text{ km/h}
$$

**Answer:** 2.26 km/h (or approximately 2.3 km/h)

**Time:** 3 minutes | **Marks:** 2

---

## 2022 Questions

### Question 6 (Easy) - Seed Drill vs Planter #Comparison #2022
**Which of the following is the main difference between a seed drill and a planter?**

**Options:**
(a) Depth of sowing  
(b) Precision of seed placement  
(c) Type of furrow opener  
(d) Draft requirement

**Solution:**

**Seed Drill vs Planter Comparison:**

| Feature | Seed Drill | Planter |
|---------|------------|---------|
| **Seed placement** | Continuous flow | **Precise spacing** |
| **Spacing control** | Random | **Fixed** |
| **Seeds per position** | Multiple | 1-3 (precise) |
| **Metering** | Fluted roller (force feed) | **Cell type/Vacuum** |
| **Crops** | Wheat, small grains | Maize, cotton, soybean |
| **Precision** | Medium | **Very High** |

**Analysis of options:**

(a) Depth: Both can sow at similar depths (not main difference)

(b) **Precision of seed placement:** ✓
- Drill: Seeds placed continuously with random spacing
- Planter: Seeds placed at precise, predetermined spacing
- This is the PRIMARY difference

(c) Type of furrow opener: Both can use similar types

(d) Draft: Similar for comparable sizes

**Answer:** (b) Precision of seed placement

**Time:** 2 minutes | **Marks:** 1

---

### Question 7 (Medium) - Rice Transplanter #Transplanter #2022
**A 6-row rice transplanter operates at 0.8 m/s with 30 cm row spacing and plants at 15 cm spacing within the row. Calculate the theoretical field capacity.**

**Solution:**

Given:
- Number of rows = 6
- Row spacing = 30 cm = 0.3 m
- Forward speed (V) = 0.8 m/s = 2.88 km/h
- Plant spacing = 15 cm (not needed for TFC)

**Working width:**
$$
W = \text{Number of rows} \times \text{Row spacing} = 6 \times 0.3 = 1.8 \text{ m}
$$

**Forward speed in km/h:**
$$
S = 0.8 \times 3.6 = 2.88 \text{ km/h}
$$

**Theoretical field capacity:**
$$
\text{TFC} = \frac{W \times S}{10} = \frac{1.8 \times 2.88}{10} = \frac{5.184}{10} = 0.518 \text{ ha/h}
$$

**Answer:** 0.518 ha/h or approximately 0.52 ha/h

**Time:** 3 minutes | **Marks:** 2

---

### Question 8 (Hard) - Draft Calculation #Draft #2022
**A 9-row seed drill with shoe-type furrow openers operates at 8 cm depth and 3 cm width per opener. If the specific draft is 0.6 N/cm², calculate the total draft. If the drill moves at 5 km/h, what is the power requirement?**

**Solution:**

Given:
- Number of rows (furrow openers) = 9
- Depth (d) = 8 cm
- Width per opener (w) = 3 cm
- Specific draft = 0.6 N/cm²
- Speed (S) = 5 km/h

**Part 1: Total Draft**

**Step 1:** Cross-sectional area per opener
$$
A = d \times w = 8 \times 3 = 24 \text{ cm}^2
$$

**Step 2:** Draft per opener
$$
D_{\text{opener}} = \text{Specific draft} \times A = 0.6 \times 24 = 14.4 \text{ N}
$$

**Step 3:** Total draft
$$
D_{\text{total}} = 9 \times 14.4 = 129.6 \text{ N} \approx 130 \text{ N} = 0.13 \text{ kN}
$$

**Part 2: Power Requirement**

$$
P = \frac{D \times V}{3.6} = \frac{0.13 \times 5}{3.6} = \frac{0.65}{3.6} = 0.181 \text{ kW} \approx 0.18 \text{ kW}
$$

**Note:** This is only for furrow openers. Actual draft would include soil resistance, rolling resistance, and seed metering friction.

**Answers:**
- Total draft = 130 N (or 0.13 kN)
- Power requirement = 0.18 kW

**Time:** 5 minutes | **Marks:** 2

---

## 2021 Questions

### Question 9 (Medium) - Seed Drill Performance #Performance #2021
**A fertilizer-cum-seed drill has a working width of 2.7 m and operates at 4.5 km/h with 72% field efficiency. Calculate the effective field capacity and time required to sow 15 hectares.**

**Solution:**

Given:
- Working width (W) = 2.7 m
- Speed (S) = 4.5 km/h
- Field efficiency (η_f) = 72% = 0.72
- Area to cover = 15 ha

**Step 1:** Calculate TFC
$$
\text{TFC} = \frac{W \times S}{10} = \frac{2.7 \times 4.5}{10} = \frac{12.15}{10} = 1.215 \text{ ha/h}
$$

**Step 2:** Calculate EFC
$$
\text{EFC} = \text{TFC} \times \eta_f = 1.215 \times 0.72 = 0.875 \text{ ha/h}
$$

**Step 3:** Calculate time required
$$
\text{Time} = \frac{\text{Area}}{\text{EFC}} = \frac{15}{0.875} = 17.14 \text{ hours}
$$

**Answers:**
- Effective field capacity = 0.875 ha/h (or 0.88 ha/h)
- Time required = 17.14 hours (or approximately 17 hours)

**Time:** 3 minutes | **Marks:** 2

---

### Question 10 (Medium) - Furrow Opener Selection #FurrowOpener #2021
**For sowing in heavy, wet clay soil with high trash content, which furrow opener would be most suitable?**

**Options:**
(a) Shoe type  
(b) Hoe type  
(c) Triple disc  
(d) Inverted-T

**Solution:**

**Furrow Opener Characteristics:**

| Type | Soil Type | Trash Handling | Soil Condition |
|------|-----------|----------------|----------------|
| **Shoe** | Light-Medium | Poor | Dry |
| **Hoe** | Heavy | Fair | Dry-Medium |
| **Triple Disc** | All types | **Excellent** | **Wet, Trashy** |
| **Inverted-T** | Medium | Good | Medium moisture |

**Analysis for Heavy, Wet Clay + High Trash:**

**Requirements:**
1. Handle heavy clay
2. Work in wet conditions
3. Handle high trash
4. Avoid clogging

**Shoe type:**
- Pushes soil, poor in wet clay ❌
- Clogs with trash ❌

**Hoe type:**
- Better than shoe in clay
- Still clogs with trash ❌

**Triple disc:**
- Cuts through trash ✓
- Works in wet conditions ✓
- Less soil disturbance ✓
- Doesn't clog ✓

**Inverted-T:**
- Moderate performance
- Not ideal for high trash ❌

**Answer:** (c) Triple disc

**Reasoning:** Triple disc furrow openers are specifically designed for:
- Conservation tillage
- Trashy conditions
- Wet soil
- Minimal soil disturbance
- No-till/minimum till systems

**Time:** 3 minutes | **Marks:** 2

---

## 2020 Questions

### Question 11 (Easy) - Broadcasting #Broadcasting #2020
**A centrifugal broadcaster with 12 m throw radius is used. For uniform coverage with 30% overlap, what should be the effective swath width?**

**Solution:**

Given:
- Throw radius (R) = 12 m
- Overlap = 30%
- Total throw width = 2 × R = 2 × 12 = 24 m

**For uniform distribution:**

With 30% overlap on each side:

**Effective width = Total width × (1 - Overlap)**

**Method 1:**
$$
\text{Effective width} = 24 \times (1 - 0.30) = 24 \times 0.70 = 16.8 \text{ m}
$$

**Method 2 (Standard practice):**
For broadcasters, effective width is typically:
$$
\text{Effective width} = 0.7 \times \text{Throw width}
$$

$$
= 0.7 \times 24 = 16.8 \text{ m}
$$

**Answer:** 16.8 m (or approximately 17 m)

**Time:** 2 minutes | **Marks:** 1

---

### Question 12 (Medium) - Cell Size Selection #CellSize #2020
**A planter is to be used for sowing seeds with average diameter of 8 mm. What should be the cell diameter for proper singulation?**

**Solution:**

Given:
- Seed diameter (d) = 8 mm

**Cell size selection formula:**

For proper singulation (picking one seed per cell):

$$
\text{Cell diameter} = (1.2 \text{ to } 1.5) \times \text{Seed diameter}
$$

**Minimum cell diameter:**
$$
D_{\text{min}} = 1.2 \times 8 = 9.6 \text{ mm}
$$

**Maximum cell diameter:**
$$
D_{\text{max}} = 1.5 \times 8 = 12 \text{ mm}
$$

**Optimal range:** 9.6 - 12 mm

**Standard practice:** Use 1.3 × seed diameter
$$
D_{\text{optimal}} = 1.3 \times 8 = 10.4 \text{ mm}
$$

**Reasoning:**
- Too small (< 1.2×): Seeds won't fit or get damaged
- Too large (> 1.5×): Multiple seeds picked, poor precision
- Optimal: 1.2-1.3× for round seeds

**Answer:** 10-11 mm (or range 9.6-12 mm)

**Time:** 3 minutes | **Marks:** 2

---

## 📈 Difficulty Analysis

| Difficulty | Count | Percentage | Topics |
|------------|-------|------------|--------|
| **Easy** | 4 | 33% | Basic concepts, simple calculations |
| **Medium** | 7 | 58% | Performance, design parameters |
| **Hard** | 1 | 9% | Complex multi-part problems |

---

## 🎯 Topic-wise Breakdown

| Topic | Questions | Key Concepts |
|-------|-----------|--------------|
| **Seed Rate & Spacing** | 3 | Population, metering, distribution |
| **Field Capacity** | 2 | TFC, EFC, efficiency |
| **Quality Index** | 1 | Miss, Multiple, Quality indices |
| **Metering Mechanisms** | 2 | Fluted roller, cell type |
| **Furrow Openers** | 1 | Selection criteria |
| **Planter Design** | 2 | Cell size, spacing |
| **Transplanter** | 1 | Performance parameters |

---

## 💡 Preparation Tips

### For Easy Questions:
- Know basic definitions (drill vs planter)
- Simple population calculations
- Standard specifications

### For Medium Questions:
- Master all formulas (seed rate, spacing, capacity)
- Understand quality indices
- Equipment selection criteria

### For Hard Questions:
- Multi-step calculations
- Combined concepts (draft + power)
- Performance optimization

---

## 🔗 Quick Links

- [Seeding & Planting Theory](./README.md)
- [Quick Reference](./CheatSheet.md)
- [Farm Machinery Index](../README.md)

---

**Total Questions:** 12  
**Last Updated:** November 2025  
**Source:** GATE AG Previous Year Papers (2020-2024)

---

*For theory concepts, see [Seeding & Planting README](./README.md)*  
*For quick revision, see [Seeding & Planting Cheat Sheet](./CheatSheet.md)*
