# 💧 Water Harvesting Structures

> Capturing and conserving rainwater for agricultural use

---

## 📚 Table of Contents

1. [Introduction](#introduction)
2. [Farm Ponds](#farm-ponds)
3. [Check Dams](#check-dams)
4. [Percolation Tanks](#percolation-tanks)
5. [Contour Bunding](#contour-bunding)
6. [Terracing for Water Conservation](#terracing-for-water-conservation)
7. [Design Calculations](#design-calculations)

---

## 🎯 Introduction

### What is Water Harvesting?

**Water harvesting** is the collection and storage of rainwater for productive use.

**Objectives:**
- Capture runoff water
- Store for dry periods
- Recharge groundwater
- Prevent soil erosion
- Increase water availability

---

### Why Water Harvesting?

**Statistics:**
- India receives **1170 mm** average annual rainfall
- **75-80%** falls during monsoon (June-September)
- Only **8-10%** is currently captured
- **Potential to store:** 30-40% of rainfall

**Benefits:**
- Reduces water scarcity
- Increases crop productivity
- Prevents erosion
- Recharges aquifers
- Reduces flood peaks

---

### Types of Structures

1. **Surface storage:** Farm ponds, tanks
2. **Subsurface storage:** Percolation tanks, trenches
3. **In-situ conservation:** Bunding, terracing
4. **Gully control:** Check dams, gabions
5. **Roof harvesting:** For domestic use

---

## 🔥 High Priority Topics

**Must Master (GATE frequent):**
1. ✓ **Farm pond capacity** calculations 🎯
2. ✓ **Runoff coefficient** values 🎯
3. ✓ **Check dam design** parameters 🎯
4. ✓ Contour bund spacing
5. ✓ Water storage calculations

**Moderate Priority:**
- Percolation tank design
- Site selection criteria
- Construction specifications

---

## 🌊 Farm Ponds

### Definition

**Farm pond:** Small earthen or lined reservoir for storing rainwater runoff from catchment area.

**Typical size:**
- Area: 200-2000 m²
- Depth: 2.5-3.5 m
- Capacity: 500-5000 m³

---

### Components

**1. Catchment Area**
- Area that drains into pond
- Should be 5-10 times pond area
- Slope: 2-6% ideal

**2. Embankment**
- Height: 2.5-4.0 m
- Top width: 2.0-3.0 m
- Side slopes:
  - Water side: 2:1 to 3:1
  - Outer side: 1.5:1 to 2:1

**3. Spillway**
- Width: 1.5-3.0 m
- Depth: 0.3-0.6 m
- Grade: 1-2%

---

### Storage Capacity Calculation

**For trapezoidal pond:**

$$
\boxed{V = \frac{H}{3}(A_1 + A_2 + \sqrt{A_1 \times A_2})}
$$

Where:
- V = Volume (m³)
- H = Depth (m)
- A₁ = Top area (m²)
- A₂ = Bottom area (m²)

---

**Simplified for rectangular pond:**

$$
\boxed{V = \frac{D}{3}[(L \times W) + (L_b \times W_b) + \sqrt{(L \times W) \times (L_b \times W_b)}]}
$$

Where:
- D = Depth (m)
- L, W = Top length, width (m)
- L_b, W_b = Bottom length, width (m)

---

**Quick approximation:**

$$
\boxed{V \approx \frac{L \times W \times D}{2}}
$$

(For side slopes of 2:1)

---

### Example Calculation

**Given:**
- Top dimensions: 30 m × 20 m
- Depth: 3 m
- Side slope: 2:1 (H:V)

**Solution:**

Bottom dimensions:
- L_b = 30 - 2(2 × 3) = 30 - 12 = 18 m
- W_b = 20 - 2(2 × 3) = 20 - 12 = 8 m

$$
A_1 = 30 \times 20 = 600 \text{ m}^2
$$

$$
A_2 = 18 \times 8 = 144 \text{ m}^2
$$

$$
V = \frac{3}{3}[600 + 144 + \sqrt{600 \times 144}]
$$

$$
= 600 + 144 + \sqrt{86400} = 600 + 144 + 294
$$

$$
= 1038 \text{ m}^3
$$

---

### Runoff Available

$$
\boxed{R = C \times I \times A}
$$

Where:
- R = Runoff volume (m³)
- C = Runoff coefficient (dimensionless)
- I = Rainfall (m)
- A = Catchment area (m²)

---

### Runoff Coefficient (C)

| Land Use / Surface | C Value |
|-------------------|---------|
| **Forest** | 0.05-0.20 |
| **Grassland** | 0.10-0.30 |
| **Cultivated land** | **0.20-0.40** ⭐ |
| **Bare soil** | 0.30-0.60 |
| **Rocky terrain** | 0.60-0.90 |
| **Paved surfaces** | 0.80-0.95 |

**Typical for agriculture:** 0.25-0.35

---

### Design Steps

**Step 1:** Determine water requirement
- Crop water need
- Irrigation area
- Season length

**Step 2:** Calculate available runoff
- Catchment area
- Rainfall
- Runoff coefficient

**Step 3:** Size the pond
- Storage = Max(requirement, available runoff × 0.7)
- Allow 30% losses (seepage, evaporation)

**Step 4:** Design dimensions
- Depth: 2.5-3.5 m
- Side slopes: 2:1 or 3:1
- Freeboard: 0.5 m

---

### Site Selection

**Good site characteristics:**
- ✓ Natural depression
- ✓ Good catchment (5-10 times pond area)
- ✓ Impermeable soil (clay)
- ✓ Easy access
- ✓ Slope 2-6%

**Avoid:**
- ✗ Rocky/sandy soil (high seepage)
- ✗ Very steep slopes
- ✗ Areas prone to flooding
- ✗ Near structures

---

### Lining Options

**1. Earthen (unlined)**
- Cheap
- High seepage (20-30%)
- Needs impermeable soil

**2. Plastic liner**
- LDPE/HDPE sheets
- Thickness: 500-1000 micron
- Low cost, moderate life

**3. Concrete lining**
- Durable
- Expensive
- Thickness: 75-100 mm

**4. Brick lining**
- Moderate cost
- Good durability
- Traditional method

---

## 🏗️ Check Dams

### Definition

**Check dam:** Small barrier across gully/stream to:
- Reduce flow velocity
- Trap sediment
- Store water temporarily
- Recharge groundwater

---

### Types

**1. Temporary check dams**
- Brush/log dams
- Sandbag dams
- Life: 1-2 years

**2. Semi-permanent**
- Gabion dams
- Life: 5-10 years

**3. Permanent**
- Masonry dams
- Concrete dams
- Life: 20-50+ years

---

### Design Parameters

**Height:**
- Small: 0.5-1.5 m
- Medium: 1.5-2.5 m
- Large: 2.5-4.0 m

**Maximum height:** Usually **3-4 m** ⭐

**Length:**
- Depends on gully width
- Typical: 5-20 m

**Thickness:**

$$
\boxed{t = 0.5H \text{ to } 0.7H}
$$

Where:
- t = Base thickness (m)
- H = Dam height (m)

For H = 2 m: t = 1.0-1.4 m

---

### Key Features

**1. Foundation**
- Depth: 0.5-1.0 m below streambed
- In firm soil/rock

**2. Cut-off wall**
- Depth: 0.5 m minimum
- Prevents undermining

**3. Spillway**
- Central or side
- Width: 1-3 m
- Drop: 0.3-0.6 m

**4. Apron**
- Downstream protection
- Length: 1.5-2.0 m
- Slope: 1:2 to 1:3

**5. Side walls (wing walls)**
- Extend into banks
- Prevent flanking
- Length: 1-2 m

---

### Storage Capacity

**For trapezoidal section:**

$$
\boxed{V = \frac{L}{2}(A_1 + A_2)}
$$

Where:
- L = Length of reservoir
- A₁ = Cross-section at dam
- A₂ = Cross-section at upstream end

---

**Approximate (triangular profile):**

$$
\boxed{V = \frac{1}{3} \times L \times W \times H}
$$

Where:
- L = Reservoir length upstream (m)
- W = Average width (m)
- H = Dam height (m)

Typical L = 20-50 m

---

### Spacing

**Distance between check dams:**

$$
\boxed{D = \frac{H}{S}}
$$

Where:
- D = Spacing (m)
- H = Dam height (m)
- S = Slope (m/m)

**Example:**
- H = 2 m
- S = 0.05 (5%)
- D = 2/0.05 = **40 m**

---

### Site Selection

**Good locations:**
- ✓ Narrow gully sections
- ✓ Firm foundation (rock/hard soil)
- ✓ Upstream catchment 5-50 ha
- ✓ Slope 2-15%

**Avoid:**
- ✗ Soft/sandy foundations
- ✗ Very steep slopes (>15%)
- ✗ Large catchments (flooding risk)
- ✗ Active landslide areas

---

## 💧 Percolation Tanks

### Definition

**Percolation tank:** Storage structure to detain runoff and allow it to percolate into the soil, recharging groundwater.

**Key difference from farm pond:**
- Farm pond: Store water for direct use
- Percolation tank: Recharge groundwater

---

### Suitable Conditions

**Geology:**
- ✓ Fractured/weathered rock
- ✓ Jointed formations
- ✓ Good permeability (>5 mm/hr)

**Soil:**
- Top: Impermeable (to hold water initially)
- Subsurface: Permeable (for recharge)

**Topography:**
- Natural depression
- Slope: 1-5%

---

### Design Specifications

**Capacity:**
- Small: 1,000-5,000 m³
- Medium: 5,000-50,000 m³
- Large: 50,000-500,000 m³

**Depth:**
- Shallow: 1-2 m
- Moderate: 2-3 m
- Deep: 3-5 m

**Catchment:**
- Ratio 10:1 to 20:1 (catchment:tank area)

---

### Components

**1. Embankment**
- Height: 2-4 m
- Top width: 2-3 m
- Side slopes: 2:1 to 3:1

**2. Spillway**
- Capacity for 25-year return period
- Width: 2-5 m

**3. Waste weir**
- Dispose excess water
- Prevent overtopping

**4. Silt trap**
- Before inlet
- Removes sediment
- Size: 10% of tank capacity

---

### Percolation Rate

**Measurement:** Cylinder infiltrometer test

**Classification:**

| Rate (mm/hr) | Suitability |
|--------------|-------------|
| <1 | Poor |
| 1-5 | Marginal |
| **5-15** | **Good** ⭐ |
| **15-50** | **Excellent** ⭐ |
| >50 | Too fast (won't store) |

---

### Recharge Calculation

$$
\boxed{R = A \times I_r \times T}
$$

Where:
- R = Recharge volume (m³)
- A = Tank bed area (m²)
- I_r = Infiltration rate (m/day)
- T = Time water is available (days)

---

### Example

**Tank:**
- Area: 5000 m²
- Infiltration: 0.15 m/day
- Water available: 100 days/year

**Recharge:**
$$
R = 5000 \times 0.15 \times 100 = 75,000 \text{ m}^3/\text{year}
$$

---

## 🏔️ Contour Bunding

### Definition

**Contour bund:** Embankment along contour line to intercept runoff and conserve water in-situ.

**Purpose:**
- Reduce runoff velocity
- Increase infiltration
- Prevent erosion
- Conserve moisture

---

### Design Specifications

**Bund dimensions:**
- Height: 0.5-1.0 m
- Top width: 0.5-1.0 m
- Side slopes: 1.5:1 to 2:1

**Spacing:**

$$
\boxed{VI = \frac{XS + Y}{100}}
$$

Where:
- VI = Vertical interval (m)
- S = Slope (%)
- X, Y = Constants (region-specific)

**Typical:** X = 0.3, Y = 1.0

$$
\boxed{VI = \frac{0.3S + 1.0}{1} = 0.3S + 1.0}
$$

---

**Horizontal spacing:**

$$
\boxed{HI = \frac{VI}{S/100} = \frac{VI \times 100}{S}}
$$

---

### Example

**Slope = 8%**

**Vertical interval:**
$$
VI = 0.3 \times 8 + 1.0 = 3.4 \text{ m}
$$

**Horizontal spacing:**
$$
HI = \frac{3.4 \times 100}{8} = 42.5 \text{ m}
$$

---

### Bund Capacity

**Storage per meter length:**

$$
\boxed{V = \frac{H^2}{2} \times \left(B + \frac{2H}{3}(S_1 + S_2)\right)}
$$

Where:
- H = Bund height (m)
- B = Top width (m)
- S₁, S₂ = Side slopes

**Simplified (triangular):**

$$
\boxed{V = \frac{H^2}{2}(S_1 + S_2)}
$$

For H = 0.6 m, slopes 2:1 and 2:1:
$$
V = \frac{0.6^2}{2}(2 + 2) = \frac{0.36 \times 4}{2} = 0.72 \text{ m}^3/\text{m}
$$

---

### Suitable Conditions

**Slope:**
- Minimum: 1% (for drainage)
- Maximum: 6-8% (too steep needs terracing)
- **Ideal: 2-5%** ⭐

**Soil:**
- Moderate permeability
- Depth >50 cm

**Rainfall:**
- 500-1000 mm annual
- Arid/semi-arid regions

---

### Layout

**1. Survey contours**
- Contour interval: 0.5-1.0 m
- Mark bund lines

**2. Grading**
- Slight grade: 0.1-0.3% ⭐
- Toward outlet
- Prevents waterlogging

**3. Outlets**
- Every 100-200 m
- Vegetated waterways

---

## 🌾 Terracing for Water Conservation

### Level Terraces

**Objective:** Hold all rainwater (no runoff)

**Features:**
- Zero grade
- High bunds
- Small spacing

**Suitable:**
- Arid regions (<500 mm rainfall)
- Gentle slopes (2-6%)

---

### Storage Capacity

**Per terrace unit:**

$$
\boxed{V = L \times W \times H_{storage}}
$$

Where:
- L = Terrace length (m)
- W = Spacing (m)
- H_storage = Storage depth (m)

**Example:**
- L = 100 m
- W = 30 m
- H = 0.15 m
$$
V = 100 \times 30 \times 0.15 = 450 \text{ m}^3
$$

---

### Design Criteria

**Storage depth:**
- **0.10-0.20 m** typical ⭐
- Based on maximum daily rainfall

**Freeboard:**
- 0.15-0.25 m above storage depth

**Bund height:**
$$
H_{bund} = H_{storage} + Freeboard
$$

For storage 0.15 m, freeboard 0.20 m:
$$
H_{bund} = 0.15 + 0.20 = 0.35 \text{ m}
$$

---

## 📊 Design Calculations

### Rational Method for Runoff

$$
\boxed{Q = \frac{C \times I \times A}{360}}
$$

Where:
- Q = Peak runoff (m³/s)
- C = Runoff coefficient
- I = Rainfall intensity (mm/hr)
- A = Catchment area (ha)

---

### Example

**Catchment:**
- Area: 10 ha
- Land use: Cultivated (C = 0.30)
- Rainfall intensity: 50 mm/hr

**Runoff:**
$$
Q = \frac{0.30 \times 50 \times 10}{360} = \frac{150}{360} = 0.417 \text{ m}^3/\text{s}
$$

---

### Storage Volume

**Required storage:**

$$
\boxed{V_{storage} = R \times A \times E}
$$

Where:
- R = Runoff depth (m)
- A = Catchment area (m²)
- E = Storage efficiency (0.7-0.8)

---

**Runoff depth:**

$$
\boxed{R = C \times P}
$$

Where:
- P = Rainfall (m)

---

### Example

**Catchment:**
- Area: 50,000 m² (5 ha)
- Rainfall: 0.8 m (800 mm)
- Runoff coefficient: 0.25
- Efficiency: 0.75

**Runoff depth:**
$$
R = 0.25 \times 0.8 = 0.20 \text{ m}
$$

**Storage:**
$$
V = 0.20 \times 50,000 \times 0.75 = 7,500 \text{ m}^3
$$

---

### Spillway Design

**Weir formula:**

$$
\boxed{Q = C_d \times L \times H^{1.5}}
$$

Where:
- Q = Discharge (m³/s)
- C_d = Discharge coefficient (1.7-1.9)
- L = Spillway length (m)
- H = Head over weir (m)

---

**Required spillway length:**

$$
\boxed{L = \frac{Q}{C_d \times H^{1.5}}}
$$

---

### Example

**Design discharge:** Q = 2.0 m³/s  
**Head:** H = 0.4 m  
**Coefficient:** C_d = 1.8

**Spillway length:**
$$
L = \frac{2.0}{1.8 \times (0.4)^{1.5}} = \frac{2.0}{1.8 \times 0.253} = \frac{2.0}{0.455} = 4.4 \text{ m}
$$

Use **L = 5 m** (rounded up)

---

## 📏 Specifications Table

### Farm Pond

| Parameter | Value |
|-----------|-------|
| **Capacity** | 500-5000 m³ |
| **Depth** | 2.5-3.5 m |
| **Side slope** | 2:1 to 3:1 |
| **Freeboard** | 0.5 m |
| **Embankment top** | 2-3 m |
| **Catchment ratio** | 5:1 to 10:1 |

---

### Check Dam

| Parameter | Value |
|-----------|-------|
| **Height** | 2-4 m (max) |
| **Base thickness** | 0.5H to 0.7H |
| **Spillway width** | 1-3 m |
| **Foundation depth** | 0.5-1.0 m |
| **Apron length** | 1.5-2.0 m |
| **Spacing** | H/S meters |

---

### Percolation Tank

| Parameter | Value |
|-----------|-------|
| **Capacity** | 1,000-500,000 m³ |
| **Depth** | 2-4 m |
| **Catchment ratio** | 10:1 to 20:1 |
| **Infiltration rate** | 5-15 mm/hr (good) |
| **Embankment slope** | 2:1 to 3:1 |

---

### Contour Bund

| Parameter | Value |
|-----------|-------|
| **Height** | 0.5-1.0 m |
| **Top width** | 0.5-1.0 m |
| **Side slope** | 1.5:1 to 2:1 |
| **VI formula** | 0.3S + 1.0 |
| **Grade** | 0.1-0.3% |
| **Suitable slope** | 2-5% |

---

## 🎯 Key Takeaways

**Critical Formulas:**

1. **Farm pond volume:**
$$
V = \frac{H}{3}(A_1 + A_2 + \sqrt{A_1 A_2})
$$

2. **Runoff:**
$$
R = C \times I \times A
$$

3. **Rational method:**
$$
Q = \frac{CIA}{360}
$$

4. **Check dam spacing:**
$$
D = \frac{H}{S}
$$

5. **Contour bund VI:**
$$
VI = 0.3S + 1.0
$$

---

**Must Remember:**

- ✓ Runoff coefficient: Cultivated land **0.20-0.40** ⭐
- ✓ Farm pond depth: **2.5-3.5 m** ⭐
- ✓ Check dam max height: **3-4 m** ⭐
- ✓ Percolation rate (good): **5-15 mm/hr** ⭐
- ✓ Contour bund suitable slope: **2-5%** ⭐

---

## 🔗 Related Topics

- [Soil Erosion & Conservation](../Soil_Erosion/README.md)
- [Land Drainage](../Land_Drainage/README.md)
- [Watershed Management](../Watershed_Management/README.md)

---

## 📚 Practice

- [PYQ Solutions](./Solutions.md)
- [Quick CheatSheet](./CheatSheet.md)

---

**Last Updated:** November 2025  
**Next Topic:** [Land Drainage](../Land_Drainage/README.md)

---

*Harvest water, harvest prosperity! 💧*
