# 🔢 Harvesting & Threshing Equipment PYQ Solutions

> Previous Year Questions with detailed solutions for GATE Agricultural Engineering

---

## 📊 Solutions Summary

| Year | Questions | Difficulty Distribution | Topics Covered |
|------|-----------|-------------------------|----------------|
| 2024 | 3 | Easy: 1, Medium: 1, Hard: 1 | Cylinder Speed, Losses, Combine |
| 2023 | 3 | Easy: 1, Medium: 2 | Thresher, Efficiency, Reel Index |
| 2022 | 2 | Medium: 2 | Field Capacity, Concave |
| 2021 | 2 | Easy: 1, Medium: 1 | Components, Cleaning |
| 2020 | 2 | Easy: 1, Medium: 1 | Cylinder Types, Loss Measurement |
| **Total** | **12** | **Easy: 4, Medium: 7, Hard: 1** | **All Major Topics** |

---

## 2024 Questions

### Question 1 (Easy) - Cylinder Speed #CylinderSpeed #2024
**A threshing cylinder with 50 cm diameter needs to operate at 20 m/s peripheral speed for wheat threshing. Calculate the required RPM.**

**Solution:**

Given:
- Cylinder diameter (D) = 50 cm = 0.5 m
- Peripheral speed (V_c) = 20 m/s

**Formula for peripheral speed:**
$$
V_c = \frac{\pi D N}{60}
$$

**Solve for N:**
$$
N = \frac{60 \times V_c}{\pi D} = \frac{60 \times 20}{3.14159 \times 0.5} = \frac{1200}{1.5708} = 763.9 \text{ rpm}
$$

**Verification:**
$$
V_c = \frac{3.14159 \times 0.5 \times 764}{60} = \frac{1199.7}{60} = 20 \text{ m/s} \quad \checkmark
$$

**Answer:** 764 rpm (or approximately 760 rpm)

**Time:** 2 minutes | **Marks:** 1

---

### Question 2 (Medium) - Crop Losses #Losses #2024
**During combine harvesting, 0.15 kg of grain was found lost in a 10 m² area. If the crop yield is 35 quintals per hectare, calculate the percentage loss.**

**Solution:**

Given:
- Grain lost in 10 m² = 0.15 kg
- Yield = 35 q/ha = 3500 kg/ha
- Area = 10 m² = 0.001 ha

**Step 1:** Calculate grain lost per hectare
$$
\text{Grain lost/ha} = \frac{0.15 \text{ kg}}{0.001 \text{ ha}} = 150 \text{ kg/ha}
$$

**Step 2:** Calculate percentage loss
$$
\text{Loss (\%)} = \frac{\text{Grain lost}}{\text{Total yield}} \times 100 = \frac{150}{3500} \times 100 = 4.29\%
$$

**Interpretation:**
- Loss of 4.29% is HIGH (acceptable limit is <2%)
- Machine needs adjustment
- Could be due to high forward speed, improper reel position, or excessive fan speed

**Answer:** 4.29% (or approximately 4.3%)

**Time:** 3 minutes | **Marks:** 2

---

### Question 3 (Hard) - Combine Performance #Combine #2024
**A self-propelled combine harvester with 4 m cutting width operates at 4.5 km/h with 70% field efficiency. The crop yield is 40 q/ha. Calculate:**
**(a) Theoretical field capacity**
**(b) Effective field capacity**
**(c) Feed rate to the threshing cylinder**

**Solution:**

Given:
- Cutting width (W) = 4 m
- Forward speed (S) = 4.5 km/h
- Field efficiency (η_f) = 70% = 0.70
- Crop yield (Y) = 40 q/ha = 4000 kg/ha

**Part (a): Theoretical Field Capacity**

$$
\text{TFC} = \frac{W \times S}{10} = \frac{4 \times 4.5}{10} = \frac{18}{10} = 1.8 \text{ ha/h}
$$

**Part (b): Effective Field Capacity**

$$
\text{EFC} = \text{TFC} \times \eta_f = 1.8 \times 0.70 = 1.26 \text{ ha/h}
$$

**Part (c): Feed Rate**

The feed rate includes grain + straw. Assuming grain:straw ratio of 1:1.5 (typical for cereals):

Total crop material = Grain + Straw = 4000 + (4000 × 1.5) = 4000 + 6000 = 10,000 kg/ha

**Feed rate:**
$$
Q_f = \text{EFC} \times \text{Total crop/ha} = 1.26 \times 10000 = 12,600 \text{ kg/h}
$$

Alternatively, if only grain is considered:
$$
Q_f (\text{grain}) = \text{EFC} \times \text{Yield} = 1.26 \times 4000 = 5040 \text{ kg/h}
$$

**Answers:**
- (a) TFC = 1.8 ha/h
- (b) EFC = 1.26 ha/h
- (c) Feed rate = 12,600 kg/h (total material) or 5,040 kg/h (grain only)

**Note:** Typically, feed rate refers to total material fed to cylinder.

**Time:** 6 minutes | **Marks:** 2

---

## 2023 Questions

### Question 4 (Easy) - Thresher Component #Thresher #2023
**Which component of a thresher provides the stationary surface against which grain is threshed?**

**Options:**
(a) Threshing cylinder  
(b) Concave  
(c) Blower  
(d) Oscillating sieve

**Solution:**

**Thresher Components and Functions:**

**Threshing Cylinder:**
- Rotating component
- Has rasp bars or pegs
- Provides IMPACT for threshing

**Concave:**
- Stationary semicircular grate
- Below the cylinder
- Provides RESISTANCE surface
- Grain passes through openings
- Straw retained and moved forward

**Blower:**
- Provides air stream
- For cleaning

**Oscillating Sieve:**
- For separating grain from chaff

**Threshing Action:**
Rotating cylinder + Stationary concave = Threshing by impact and rubbing

**Answer:** (b) Concave

**Time:** 1 minute | **Marks:** 1

---

### Question 5 (Medium) - Threshing Efficiency #Efficiency #2023
**A thresher processes 500 kg of wheat crop. After threshing, 2 kg of unthreshed grain is found in the straw. Calculate the threshing efficiency.**

**Solution:**

Given:
- Total crop processed = 500 kg
- Unthreshed grain in straw = 2 kg

**Threshing efficiency formula:**
$$
\eta_t = \frac{\text{Grain threshed}}{\text{Total grain in crop}} \times 100\%
$$

Assuming grain:straw ratio = 1:1.5 (typical)
- Total grain in crop = 500 / 2.5 = 200 kg
- Grain threshed = 200 - 2 = 198 kg

$$
\eta_t = \frac{198}{200} \times 100 = 99\%
$$

**Alternative interpretation:**
If we consider the unthreshed grain directly:

$$
\eta_t = \frac{\text{Total grain} - \text{Unthreshed grain}}{\text{Total grain}} \times 100
$$

Assuming total grain = 200 kg (40% of crop)

$$
\eta_t = \frac{200 - 2}{200} \times 100 = \frac{198}{200} \times 100 = 99\%
$$

**Interpretation:**
- 99% efficiency is EXCELLENT
- Meets the requirement (>99%)
- Very little loss

**Answer:** 99%

**Time:** 3 minutes | **Marks:** 2

---

### Question 6 (Medium) - Reel Index #ReelIndex #2023
**A reaper operates at 3 km/h forward speed. The reel has 60 cm diameter and rotates at 40 rpm. Calculate the reel index.**

**Solution:**

Given:
- Forward speed (V_f) = 3 km/h = 3000/3600 = 0.833 m/s
- Reel diameter (D_r) = 60 cm = 0.6 m
- Reel RPM (N_r) = 40 rpm

**Step 1:** Calculate peripheral speed of reel

$$
V_r = \frac{\pi D_r N_r}{60} = \frac{3.14159 \times 0.6 \times 40}{60} = \frac{75.4}{60} = 1.257 \text{ m/s}
$$

**Step 2:** Calculate reel index

$$
\text{Reel Index} = \frac{V_r}{V_f} = \frac{1.257}{0.833} = 1.51
$$

**Interpretation:**
- Reel index = 1.51
- Optimal range: 1.2 to 1.5
- This value (1.51) is slightly above optimal
- Acceptable but could be reduced to 1.4-1.5 for better performance

**Answer:** 1.51 (or approximately 1.5)

**Time:** 4 minutes | **Marks:** 2

---

## 2022 Questions

### Question 7 (Medium) - Field Capacity #FieldCapacity #2022
**A combine harvester with 3.6 m cutting width operates at 4 km/h. If it harvested 8 hectares in 6 hours, calculate the field efficiency.**

**Solution:**

Given:
- Cutting width (W) = 3.6 m
- Speed (S) = 4 km/h
- Area harvested = 8 ha
- Time taken = 6 hours

**Step 1:** Calculate TFC

$$
\text{TFC} = \frac{W \times S}{10} = \frac{3.6 \times 4}{10} = \frac{14.4}{10} = 1.44 \text{ ha/h}
$$

**Step 2:** Calculate EFC

$$
\text{EFC} = \frac{\text{Area}}{\text{Time}} = \frac{8}{6} = 1.333 \text{ ha/h}
$$

**Step 3:** Calculate field efficiency

$$
\eta_f = \frac{\text{EFC}}{\text{TFC}} \times 100 = \frac{1.333}{1.44} \times 100 = 92.6\%
$$

**Interpretation:**
- 92.6% efficiency is VERY HIGH
- Typical for combines: 70-80%
- This suggests either:
  - Very skilled operator
  - Ideal field conditions
  - Minimal turning time

**Answer:** 92.6% (or approximately 93%)

**Time:** 3 minutes | **Marks:** 2

---

### Question 8 (Medium) - Concave Clearance #Concave #2022
**In a thresher, why is the concave clearance kept wider at the entry (25-30 mm) and narrower at the exit (10-15 mm)?**

**Options:**
(a) To reduce power consumption  
(b) To facilitate gradual threshing and prevent grain damage  
(c) To increase cleaning efficiency  
(d) To improve straw quality

**Solution:**

**Concave Clearance Function:**

**Entry (25-30 mm) - WIDER:**
- Crop enters with full stalks and heads
- Needs space to enter smoothly
- Initial impact separates some grain
- Gradual threshing begins

**Exit (10-15 mm) - NARROWER:**
- Most grain already separated
- Narrower gap for final threshing
- More rubbing action on remaining grain
- Completes the threshing process

**Progressive Threshing:**
The tapering clearance provides:
1. **Gradual threshing** - Not all at once
2. **Less grain damage** - Gentle initial impact
3. **Complete separation** - Multiple chances
4. **Better straw quality** - Not over-beaten

**Why NOT other options:**

(a) Power: Clearance doesn't significantly affect power  
(c) Cleaning: That's done by sieves and blower  
(d) Straw quality: Secondary benefit, not primary reason

**Answer:** (b) To facilitate gradual threshing and prevent grain damage

**Time:** 3 minutes | **Marks:** 2

---

## 2021 Questions

### Question 9 (Easy) - Combine Components #Components #2021
**Arrange the following combine harvester components in the correct sequence of crop flow:**

**Components:**
I. Cleaning unit  
II. Header  
III. Separation unit  
IV. Threshing unit

**Options:**
(a) II → IV → III → I  
(b) II → III → IV → I  
(c) II → IV → I → III  
(d) IV → II → III → I

**Solution:**

**Crop Flow in Combine Harvester:**

**1. HEADER (II):**
- First point of contact
- Cutting and gathering
- Feeds crop to threshing

**2. THRESHING UNIT (IV):**
- Cylinder and concave
- Separates grain from straw
- ~60-70% grain separated here

**3. SEPARATION UNIT (III):**
- Straw walkers or rotary separator
- Separates remaining grain from straw
- ~25-35% grain recovered
- Straw discharged

**4. CLEANING UNIT (I):**
- Sieves and blower
- Removes chaff and impurities
- Final cleaning
- Clean grain to tank

**Sequence:** Header → Threshing → Separation → Cleaning

**Answer:** (a) II → IV → III → I

**Time:** 2 minutes | **Marks:** 1

---

### Question 10 (Medium) - Cleaning Unit #Cleaning #2021
**In a combine harvester cleaning unit, what happens if the fan speed is increased excessively?**

**Options:**
(a) Better cleaning with no grain loss  
(b) Grain blown away with chaff, increasing cleaning loss  
(c) More power consumption only  
(d) Reduced cleaning efficiency

**Solution:**

**Cleaning Unit Function:**

**Fan Purpose:**
- Blows air through falling grain-chaff mixture
- Light chaff blown away
- Heavy grain falls through

**Air Velocity Effects:**

**Optimal Fan Speed:**
- Chaff (light) blown away ✓
- Grain (heavy) falls through ✓
- Clean grain collected

**Too Low Fan Speed:**
- Insufficient air
- Chaff not blown away
- Poor cleaning
- Impure grain

**Too High Fan Speed (EXCESSIVE):**
- Very strong air stream
- Chaff blown away ✓
- **Lightweight/small grain also blown away** ❌
- **Cleaning loss increases**
- Good grains lost with chaff

**Terminal Velocity:**
- Chaff: 3-5 m/s
- Grain: 8-12 m/s

If fan produces >8 m/s, grain loss occurs.

**Answer:** (b) Grain blown away with chaff, increasing cleaning loss

**Time:** 3 minutes | **Marks:** 2

---

## 2020 Questions

### Question 11 (Easy) - Cylinder Types #CylinderTypes #2020
**Which type of threshing cylinder is most suitable for pulses and soybeans?**

**Options:**
(a) Rasp bar type  
(b) Peg tooth type  
(c) Wire loop type  
(d) Spike tooth type

**Solution:**

**Cylinder Types and Applications:**

**Rasp Bar:**
- Blunt rectangular bars
- For: Wheat, Rice, Barley
- Speed: 18-25 m/s
- Less grain damage

**Peg Tooth:**
- Pointed pegs/teeth
- **For: Pulses, Soybean** ✓
- Speed: 10-15 m/s
- Better threshing action for pod crops

**Wire Loop:**
- Gentle action
- For: Very delicate crops
- Minimal damage

**Spike Tooth:**
- Sharp spikes
- For: Maize, Sorghum
- Medium impact

**Why Peg Tooth for Pulses:**
- Pulses have pods (not heads)
- Need more aggressive action to open pods
- Peg teeth penetrate and separate
- Rasp bars would slip over pods
- Lower speed prevents seed damage

**Answer:** (b) Peg tooth type

**Time:** 2 minutes | **Marks:** 1

---

### Question 12 (Medium) - Loss Measurement #LossMeasurement #2020
**Describe the procedure to measure combine harvester field losses. What is the acceptable limit?**

**Solution:**

**Loss Measurement Procedure:**

**Equipment Needed:**
- Frame of known area (1 m × 1 m = 1 m²)
- Collection bags
- Weighing scale

**Step-by-Step Procedure:**

**1. Select Sampling Points:**
- Random locations across field
- Minimum 10 sampling points
- After combine has passed

**2. Place Frame:**
- 1 m² frame on ground
- In the combine's path

**3. Collect Lost Grain:**
- Pick up ALL grain within frame
- Check stubble for attached grains
- Collect from ground surface
- Separate from soil/debris

**4. Weigh the Grain:**
- Weigh collected grain
- Record weight (kg)

**5. Calculate Loss:**

$$
\text{Loss (kg/ha)} = \frac{\text{Weight of grain (kg)}}{1 \text{ m}^2} \times 10000
$$

$$
\text{Loss (\%)} = \frac{\text{Loss (kg/ha)}}{\text{Yield (kg/ha)}} \times 100
$$

**6. Repeat:**
- Take 10-20 samples
- Calculate average loss

**Example Calculation:**

Sample area = 1 m² = 0.0001 ha
Grain found = 0.08 kg
Yield = 40 q/ha = 4000 kg/ha

Loss/ha = 0.08 / 0.0001 = 800 kg/ha
Loss % = (800 / 4000) × 100 = 2%

**Acceptable Limits:**

| Loss Type | Limit |
|-----------|-------|
| **Total combine loss** | < 2% |
| **Header loss** | < 0.5% |
| **Threshing loss** | < 0.3% |
| **Separation loss** | < 0.7% |
| **Cleaning loss** | < 0.5% |

**Answer:**
- Procedure: Use 1 m² frame, collect all lost grain, weigh, calculate percentage
- Acceptable limit: **Less than 2% total loss**

**Time:** 5 minutes | **Marks:** 2

---

## 📈 Difficulty Analysis

| Difficulty | Count | Percentage | Topics |
|------------|-------|------------|--------|
| **Easy** | 4 | 33% | Component identification, basic concepts |
| **Medium** | 7 | 58% | Calculations, efficiency, adjustments |
| **Hard** | 1 | 9% | Multi-part complex problems |

---

## 🎯 Topic-wise Breakdown

| Topic | Questions | Key Concepts |
|-------|-----------|--------------|
| **Cylinder Speed** | 2 | V = πDN/60, crop-specific speeds |
| **Losses** | 3 | Measurement, calculation, limits |
| **Field Capacity** | 2 | TFC, EFC, efficiency |
| **Efficiency** | 1 | Threshing efficiency >99% |
| **Components** | 2 | Sequence, function, selection |
| **Adjustments** | 2 | Concave, fan speed, reel index |

---

## 💡 Preparation Tips

### For Easy Questions:
- Know component functions
- Cylinder types for different crops
- Basic concepts and terminology

### For Medium Questions:
- Master all formulas
- Speed calculations (cylinder, reel)
- Loss measurement procedures
- Efficiency calculations

### For Hard Questions:
- Multi-step problems
- Feed rate calculations
- Combined concepts
- Real-world applications

---

## 🔗 Quick Links

- [Harvesting & Threshing Theory](./README.md)
- [Quick Reference](./CheatSheet.md)
- [Farm Machinery Index](../README.md)

---

**Total Questions:** 12  
**Last Updated:** November 2025  
**Source:** GATE AG Previous Year Papers (2020-2024)

---

*For theory concepts, see [Harvesting & Threshing README](./README.md)*  
*For quick revision, see [Harvesting & Threshing Cheat Sheet](./CheatSheet.md)*
