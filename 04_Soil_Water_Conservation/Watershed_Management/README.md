# 🏞️ Watershed Management

> Integrated management of land and water resources

---

## 📚 Table of Contents

1. [Introduction](#introduction)
2. [Watershed Characteristics](#watershed-characteristics)
3. [Morphometric Parameters](#morphometric-parameters)
4. [Runoff Estimation - Rational Method](#runoff-estimation---rational-method)
5. [SCS Curve Number Method](#scs-curve-number-method)
6. [Time of Concentration](#time-of-concentration)
7. [Watershed Development](#watershed-development)

---

## 🎯 Introduction

### What is a Watershed?

**Watershed (catchment/drainage basin):** An area of land that drains all precipitation to a common outlet (stream, river, lake).

**Key concept:** Water falling anywhere in the watershed flows to the same point.

---

### Importance

**Benefits of watershed management:**
- Flood control
- Water conservation
- Erosion prevention
- Groundwater recharge
- Improved crop productivity
- Sustainable development

---

### Watershed Delineation

**Boundary:** Defined by topographic ridge (watershed divide)

**Outlet:** Lowest point where water exits

**Stream network:** Dendritic, trellis, radial, or rectangular patterns

---

## 🔥 High Priority Topics

**Must Master (GATE frequent):**
1. ✓ **Rational formula** Q = CIA/360 🎯
2. ✓ **SCS Curve Number method** 🎯
3. ✓ Runoff coefficient (C) values 🎯
4. ✓ **Time of concentration** formula 🎯
5. ✓ Morphometric parameters (form factor, etc.)

**Moderate Priority:**
- Stream ordering
- Watershed prioritization
- Development strategies

---

## 📐 Watershed Characteristics

### Basic Parameters

**1. Area (A)**
- Measured in km² or hectares
- From topographic map or GIS
- Most fundamental parameter

**2. Perimeter (P)**
- Length of watershed boundary
- Measured in km

**3. Length (L)**
- Distance from outlet to farthest point
- Along main stream channel

**4. Width (W)**
- Average width
- W = A / L

---

### Drainage Density

$$
\boxed{D_d = \frac{L_{total}}{A}}
$$

Where:
- L_total = Total length of all streams (km)
- A = Watershed area (km²)
- Units: km/km²

**Typical values:**

| D_d (km/km²) | Classification |
|--------------|----------------|
| <2.0 | Coarse drainage |
| 2.0-4.0 | Moderate |
| **4.0-6.0** | **Fine** ⭐ |
| >6.0 | Very fine |

**Higher Dd → More runoff, faster response**

---

## 🔢 Morphometric Parameters

### 1. Form Factor (R_f)

**Measure of watershed shape:**

$$
\boxed{R_f = \frac{A}{L^2}}
$$

Where:
- A = Area (km²)
- L = Length (km)

---

**Interpretation:**

| R_f | Shape | Flood Potential |
|-----|-------|-----------------|
| **0.8-1.0** | **Circular** | High peak, short duration |
| **0.5-0.8** | **Oval** | Moderate |
| **0.3-0.5** | **Elongated** ⭐ | Low peak, long duration |
| <0.3 | Very elongated | Very flat hydrograph |

**Memory:** Lower R_f = Elongated = Safer (lower flood peak)

---

### 2. Circularity Ratio (R_c)

$$
\boxed{R_c = \frac{4\pi A}{P^2}}
$$

Or: 

$$
\boxed{R_c = \frac{12.57A}{P^2}}
$$

---

**Interpretation:**

| R_c | Shape |
|-----|-------|
| **1.0** | **Perfect circle** |
| 0.7-1.0 | Circular |
| 0.5-0.7 | Oval |
| 0.3-0.5 | Elongated |
| <0.3 | Very elongated |

**Higher R_c → More circular → Higher flood peaks**

---

### 3. Elongation Ratio (R_e)

$$
\boxed{R_e = \frac{D_c}{L}}
$$

Where:
- D_c = Diameter of circle with same area = √(4A/π)
- L = Watershed length

Or:

$$
\boxed{R_e = \frac{1.128\sqrt{A}}{L}}
$$

---

**Classification:**

| R_e | Shape |
|-----|-------|
| 0.9-1.0 | Circular |
| 0.8-0.9 | Oval |
| **0.6-0.8** | **Elongated** ⭐ |
| <0.6 | Very elongated |

---

### 4. Compactness Coefficient (C_c)

$$
\boxed{C_c = \frac{P}{2\sqrt{\pi A}}}
$$

Or:

$$
\boxed{C_c = \frac{0.282P}{\sqrt{A}}}
$$

---

**Interpretation:**

| C_c | Shape |
|-----|-------|
| **1.0** | **Perfect circle** |
| 1.0-1.25 | Oval to circular |
| 1.25-1.5 | Moderately elongated |
| >1.5 | Very elongated |

**C_c = 1.0 → Circle → Maximum flood potential**

---

### Example Calculation

**Watershed:**
- Area (A) = 25 km²
- Perimeter (P) = 30 km
- Length (L) = 8 km

---

**1. Form Factor:**
$$
R_f = \frac{25}{8^2} = \frac{25}{64} = 0.391
$$

**Elongated shape** (0.3-0.5 range)

---

**2. Circularity Ratio:**
$$
R_c = \frac{12.57 \times 25}{30^2} = \frac{314.25}{900} = 0.349
$$

**Elongated** (<0.5)

---

**3. Elongation Ratio:**
$$
R_e = \frac{1.128 \times \sqrt{25}}{8} = \frac{1.128 \times 5}{8} = \frac{5.64}{8} = 0.705
$$

**Elongated** (0.6-0.8)

---

**4. Compactness Coefficient:**
$$
C_c = \frac{0.282 \times 30}{\sqrt{25}} = \frac{8.46}{5} = 1.692
$$

**Very elongated** (>1.5)

**All parameters confirm: Elongated watershed → Lower flood peaks**

---

## 🌊 Stream Ordering

### Strahler Method (Most Common)

**Rules:**
1. **1st order:** Smallest tributaries (no tributaries feeding them)
2. **2nd order:** Two 1st order streams join
3. **3rd order:** Two 2nd order streams join
4. **Rule:** i + i = i+1 (same order joining increases order by 1)
5. **Exception:** i + j = max(i,j) if i ≠ j (different orders, higher order continues)

---

**Example:**

```
        ─── 1 ─┐
               ├─ 2 ─┐
        ─── 1 ─┘     │
                     ├─ 3 ─┐
        ─── 1 ─┐     │     │
               ├─ 2 ─┘     │
        ─── 1 ─┘           ├─ 4 (Main)
                           │
        ─── 1 ─┐           │
               ├─ 2 ───────┘
        ─── 1 ─┘
```

**Main stream = 4th order**

---

### Bifurcation Ratio

$$
\boxed{R_b = \frac{N_u}{N_{u+1}}}
$$

Where:
- N_u = Number of streams of order u
- N_{u+1} = Number of streams of next higher order

**Typical value:** 3-5

**Higher Rb → More branching → Better drainage**

---

## 💧 Runoff Estimation - Rational Method

### Formula

$$
\boxed{Q = \frac{C \times I \times A}{360}}
$$

**Most Important Formula for GATE!** 🎯

---

### Parameters

**Q** = Peak runoff rate (m³/s)

**C** = Runoff coefficient (dimensionless)

**I** = Rainfall intensity (mm/hr)

**A** = Catchment area (hectares)

**360** = Conversion constant

---

### Runoff Coefficient (C)

| Surface/Land Use | C Value |
|------------------|---------|
| **Forest** | **0.05-0.20** ⭐ |
| **Grassland** | 0.10-0.30 |
| **Cultivated land** | **0.20-0.40** ⭐ |
| **Bare soil** | 0.30-0.60 |
| **Rocky terrain** | 0.60-0.90 |
| **Paved (urban)** | 0.80-0.95 |

**Memory:**
- Forest = 0.10 (typical)
- Cultivated = 0.30 (typical)
- Paved = 0.90 (typical)

---

### Factors Affecting C

**1. Soil type:**
- Sandy: Lower C (high infiltration)
- Clay: Higher C (low infiltration)

**2. Slope:**
- Steep: Higher C (rapid runoff)
- Gentle: Lower C (more infiltration)

**3. Vegetation:**
- Dense: Lower C (interception, transpiration)
- Sparse: Higher C

**4. Antecedent moisture:**
- Dry: Lower C
- Wet: Higher C

---

### Rainfall Intensity (I)

**From IDF curves (Intensity-Duration-Frequency)**

**General formula:**

$$
I = \frac{K \times T^m}{(t_c + b)^n}
$$

Where:
- T = Return period (years)
- t_c = Time of concentration (minutes)
- K, m, b, n = Regional constants

**For GATE:** Usually given directly

---

### Example Calculation

**Given:**
- Catchment area: 10 hectares
- Land use: Cultivated (C = 0.30)
- Rainfall intensity: 50 mm/hr

**Calculate peak runoff:**

$$
Q = \frac{C \times I \times A}{360} = \frac{0.30 \times 50 \times 10}{360}
$$

$$
= \frac{150}{360} = 0.417 \text{ m}^3/\text{s}
$$

---

### Unit Verification

**Why 360?**

$$
Q(\text{m}^3/\text{s}) = \frac{C \times I(\text{mm/hr}) \times A(\text{ha})}{360}
$$

Converts:
- mm/hr → m/hr (÷1000)
- ha → m² (×10,000)
- hr → s (÷3600)

Combined: (10,000)/(1000 × 3.6) = 10/3.6 ≈ 360

---

## 🌧️ SCS Curve Number Method

### Overview

**SCS (Soil Conservation Service)** method estimates runoff from rainfall.

**More accurate than Rational method**

**Accounts for:**
- Soil type
- Land use
- Antecedent moisture

---

### Runoff Equation

$$
\boxed{Q = \frac{(P - I_a)^2}{(P - I_a) + S}}
$$

Where:
- Q = Runoff depth (mm)
- P = Rainfall (mm)
- I_a = Initial abstraction (mm)
- S = Potential maximum retention (mm)

---

### Initial Abstraction

**Typically:**

$$
\boxed{I_a = 0.2S}
$$

**Substituting:**

$$
\boxed{Q = \frac{(P - 0.2S)^2}{(P - 0.2S) + S} = \frac{(P - 0.2S)^2}{P + 0.8S}}
$$

**Condition:** Q = 0 if P < 0.2S (no runoff)

---

### Curve Number (CN)

**Relationship with S:**

$$
\boxed{S = \frac{25400}{CN} - 254}
$$

Where CN is the Curve Number (dimensionless, 0-100)

**Or:**

$$
\boxed{CN = \frac{25400}{S + 254}}
$$

---

### CN Values

**Depends on:**
1. **Hydrologic soil group** (A, B, C, D)
2. **Land use/cover**
3. **Hydrologic condition**
4. **Antecedent moisture condition** (AMC)

---

### Hydrologic Soil Groups

| Group | Description | Infiltration | Examples |
|-------|-------------|--------------|----------|
| **A** | Low runoff potential | **High** | Sand, gravel |
| **B** | Moderately low | Moderate | Sandy loam, loam |
| **C** | Moderately high | Moderately low | Clay loam, silt loam |
| **D** | High runoff potential | **Low** | Clay, shallow soil |

---

### Typical CN Values

**For AMC-II (Normal conditions):**

| Land Use | Soil Group | | | |
|----------|------------|---|---|---|
| | **A** | **B** | **C** | **D** |
| **Fallow** | 77 | 86 | **91** | **94** ⭐ |
| **Row crops** | 67 | 78 | 85 | 89 |
| **Small grains** | 63 | 75 | 83 | 87 |
| **Pasture (good)** | 39 | 61 | 74 | 80 |
| **Meadow (good)** | 30 | 58 | 71 | 78 |
| **Forest (good)** | **30** | **55** | 70 | 77 ⭐ |
| **Residential (65% impervious)** | 77 | 85 | 90 | 92 |
| **Paved/roofs** | 98 | 98 | 98 | 98 |

**Memory:**
- Forest Group A = 30 (lowest, best infiltration)
- Fallow Group D = 94 (highest, worst)
- Paved = 98 (almost all runoff)

---

### Antecedent Moisture Condition (AMC)

**AMC-I (Dry):**
- 5-day rainfall < 12.5 mm (growing season)
- CN reduced

**AMC-II (Normal):** ⭐
- 5-day rainfall 12.5-27.5 mm
- **Standard condition** (use table values)

**AMC-III (Wet):**
- 5-day rainfall > 27.5 mm
- CN increased

---

**Conversion formulas:**

**AMC-I:**
$$
CN_I = \frac{CN_{II}}{2.334 - 0.01334 \times CN_{II}}
$$

**AMC-III:**
$$
CN_{III} = \frac{CN_{II}}{0.427 + 0.00573 \times CN_{II}}
$$

---

### Complete Example

**Given:**
- Rainfall (P) = 100 mm
- Land use: Pasture (good condition)
- Soil: Group B
- AMC: Normal (AMC-II)

---

**Step 1: Find CN**

From table: CN = 61 (Pasture-good, Group B)

---

**Step 2: Calculate S**

$$
S = \frac{25400}{61} - 254 = 416.4 - 254 = 162.4 \text{ mm}
$$

---

**Step 3: Calculate I_a**

$$
I_a = 0.2 \times 162.4 = 32.5 \text{ mm}
$$

---

**Step 4: Check if runoff occurs**

P = 100 mm > I_a = 32.5 mm ✓

Runoff will occur.

---

**Step 5: Calculate Q**

$$
Q = \frac{(P - I_a)^2}{(P - I_a) + S} = \frac{(100 - 32.5)^2}{(100 - 32.5) + 162.4}
$$

$$
= \frac{(67.5)^2}{67.5 + 162.4} = \frac{4556.25}{229.9} = 19.8 \text{ mm}
$$

**Runoff = 19.8 mm**

---

**Verification:**

**Rainfall:** 100 mm  
**Runoff:** 19.8 mm (19.8%)  
**Losses:** 80.2 mm (infiltration, evaporation)

Reasonable for pasture on loam soil! ✓

---

## ⏱️ Time of Concentration

### Definition

**Time of concentration (Tc):** Time for water to travel from the hydraulically most distant point to the outlet.

**Importance:** Used in Rational formula to determine design rainfall intensity.

---

### Kirpich Formula

**Most commonly used:**

$$
\boxed{T_c = 0.0195 \times L^{0.77} \times S^{-0.385}}
$$

Where:
- T_c = Time of concentration (minutes)
- L = Maximum travel length (m)
- S = Average slope (m/m)

---

**Memory:** **"0.02 L^0.8 S^-0.4"** (approximately)

---

### Example

**Watershed:**
- Length (L) = 2000 m
- Elevation drop = 50 m
- Slope (S) = 50/2000 = 0.025 m/m

**Calculate Tc:**

$$
T_c = 0.0195 \times (2000)^{0.77} \times (0.025)^{-0.385}
$$

**Step-by-step:**

$$
L^{0.77} = 2000^{0.77} = 471.6
$$

$$
S^{-0.385} = 0.025^{-0.385} = 3.35
$$

$$
T_c = 0.0195 \times 471.6 \times 3.35 = 30.8 \text{ minutes}
$$

**Tc ≈ 31 minutes**

---

### Alternative Formulas

**1. Bransby-Williams:**
$$
T_c = 14.6 \times \frac{L}{A^{0.1} \times S^{0.2}}
$$

**2. California Culverts Practice:**
$$
T_c = \frac{(0.87 \times L^3)^{0.385}}{H}
$$

Where H = elevation difference (m)

**3. FAA (Federal Aviation Administration):**
$$
T_c = 1.8 \times (1.1 - C) \times \sqrt{L} / \sqrt[3]{S}
$$

**For GATE:** Kirpich is most common! 🎯

---

## 🏞️ Watershed Development

### Objectives

1. **Water conservation:** Rainwater harvesting, recharge
2. **Soil conservation:** Erosion control
3. **Crop production:** Improved productivity
4. **Livelihood:** Income generation
5. **Sustainability:** Long-term resource management

---

### Ridge to Valley Approach

**Sequence:**

1. **Ridge area:**
   - Afforestation
   - Contour trenches
   - Boulder checks

2. **Upper slopes:**
   - Contour bunding
   - Bench terracing
   - Horticulture

3. **Middle slopes:**
   - Field bunding
   - Crop production
   - Farm ponds

4. **Valley:**
   - Check dams
   - Percolation tanks
   - Water harvesting structures

---

### Watershed Prioritization

**Based on:**

**1. Erosion severity:**
- High erosion → High priority

**2. Runoff potential:**
- High runoff → Need treatment

**3. Socio-economic:**
- Population density
- Poverty level

**4. Strategic importance:**
- Water supply
- Flood control

---

**Prioritization index:**

$$
PI = W_1 \times E + W_2 \times R + W_3 \times S
$$

Where:
- E = Erosion index
- R = Runoff index
- S = Socio-economic index
- W = Weights

---

## 📊 Key Formulas Summary

**1. Rational Method:**
$$
\boxed{Q = \frac{C \times I \times A}{360}}
$$

**2. SCS Runoff:**
$$
\boxed{Q = \frac{(P - 0.2S)^2}{P + 0.8S}}
$$

**3. CN-S Relationship:**
$$
\boxed{S = \frac{25400}{CN} - 254}
$$

**4. Time of Concentration:**
$$
\boxed{T_c = 0.0195 \times L^{0.77} \times S^{-0.385}}
$$

**5. Form Factor:**
$$
\boxed{R_f = \frac{A}{L^2}}
$$

---

## 🎯 Key Takeaways

**Must Remember:**

- ✓ **Rational formula:** Q = CIA/360 ⭐
- ✓ **C values:** Forest 0.05-0.20, Cultivated 0.20-0.40, Paved 0.80-0.95
- ✓ **SCS:** Q = (P-0.2S)²/(P+0.8S), S = 25400/CN - 254
- ✓ **CN values:** Forest A=30, Fallow D=94
- ✓ **Tc formula:** Kirpich 0.0195 L^0.77 S^-0.385
- ✓ **Form factor:** Rf = A/L² (lower = elongated = safer)
- ✓ **AMC-II:** Normal condition (standard)

---

## 🔗 Related Topics

- [Soil Erosion & Conservation](../Soil_Erosion/README.md)
- [Water Harvesting](../Water_Harvesting/README.md)
- [Land Drainage](../Land_Drainage/README.md)

---

## 📚 Practice

- [PYQ Solutions](./Solutions.md)
- [Quick CheatSheet](./CheatSheet.md)

---

**Last Updated:** November 2025  
**Section Complete!** ✓

---

*Manage watersheds, manage water! 🏞️*
