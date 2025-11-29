# 🌊 Land Drainage

> Removing excess water from agricultural land

---

## 📚 Table of Contents

1. [Introduction](#introduction)
2. [Types of Drainage](#types-of-drainage)
3. [Drainage Coefficient](#drainage-coefficient)
4. [Hooghoudt Equation](#hooghoudt-equation)
5. [Drain Spacing](#drain-spacing)
6. [Design Criteria](#design-criteria)
7. [Drainage Materials](#drainage-materials)

---

## 🎯 Introduction

### What is Land Drainage?

**Land drainage:** Removal of excess water (surface or subsurface) from agricultural land to:
- Prevent waterlogging
- Improve aeration
- Enable timely operations
- Increase crop productivity

---

### Need for Drainage

**Problems with excess water:**
- Reduced oxygen in root zone
- Nutrient leaching
- Disease/pest problems
- Delayed planting/harvesting
- Soil structure damage
- Reduced crop yields (20-60%)

---

### Causes of Waterlogging

**1. Natural:**
- Heavy rainfall
- Floods
- High water table
- Poor soil drainage

**2. Human-induced:**
- Over-irrigation
- Canal seepage
- Lack of drainage
- Blocked natural drainage

---

## 🔥 High Priority Topics

**Must Master (GATE frequent):**
1. ✓ **Hooghoudt equation** for drain spacing 🎯
2. ✓ **Drainage coefficient** values 🎯
3. ✓ Drain spacing by soil type 🎯
4. ✓ **Donnan equation** (backup) 🎯
5. ✓ Design criteria

**Moderate Priority:**
- Surface drainage methods
- Drain materials
- Installation depth

---

## 📊 Types of Drainage

### 1. Surface Drainage

**Purpose:** Remove excess water from land surface

**Methods:**

**A. Land forming/grading**
- Create gentle slopes (0.1-0.5%)
- Direct water to outlets
- Cost: Low
- Suitable: Flat lands

**B. Open drains/ditches**
- Depth: 0.5-1.5 m
- Side slopes: 1:1 to 2:1
- Spacing: 50-200 m
- Suitable: Heavy rainfall areas

**C. Field ditches**
- Shallow (0.3-0.6 m)
- Temporary or permanent
- Connect to main drains

---

### 2. Subsurface Drainage

**Purpose:** Lower water table, remove deep seepage

**Methods:**

**A. Tile drains (Pipe drains)**
- Buried pipes with perforations
- Depth: 1.0-2.0 m ⭐
- Spacing: 10-100 m (soil-dependent)
- Most effective method

**B. Mole drains**
- Unlined channels formed by mole plow
- Depth: 0.5-0.8 m
- Spacing: 2-4 m
- Suitable: Clay soils
- Life: 5-10 years

**C. Deep open drains**
- Depth: 2-3 m
- Permanent structures
- Combined with pipe drains

---

## 💧 Drainage Coefficient

### Definition

**Drainage coefficient (q):** The rate at which water must be removed from a given area to prevent crop damage.

**Units:** mm/day or cm/day

---

### Typical Values

| Crop/Situation | q (mm/day) |
|----------------|------------|
| **Rice** | 5-8 |
| **Field crops** | **10-15** ⭐ |
| **Vegetables** | **15-20** |
| **Orchards** | 10-12 |
| **Humid climate** | **15-25** |
| **Arid climate** | 8-12 |

**Memory: "Field crops = 10-15 mm/day"** ⭐

---

### Factors Affecting q

**1. Rainfall:**
- Higher rainfall → Higher q
- Design based on 10-year or 25-year storm

**2. Crop tolerance:**
- Sensitive crops → Higher q
- Tolerant crops → Lower q

**3. Soil type:**
- Heavy clay → Lower q acceptable
- Sandy soil → Higher q needed

**4. Climate:**
- Humid → Higher q
- Arid → Lower q

---

### Selection Guidelines

**Conservative design:** Use **10-15 mm/day** for field crops ⭐

**For vegetables/high-value crops:** 15-20 mm/day

**Formula relation:**
$$
q = \frac{P_{excess}}{T}
$$

Where:
- P_excess = Excess rainfall/irrigation (mm)
- T = Time to remove (days, typically 1-3 days)

---

## 🔢 Hooghoudt Equation

### Most Important Formula for GATE!

**For subsurface drain spacing:**

$$
\boxed{q = \frac{4K(2md + d^2)}{L^2}}
$$

**Rearranged for spacing:**

$$
\boxed{L = \sqrt{\frac{4K(2md + d^2)}{q}}}
$$

---

### Parameters

**q** = Drainage coefficient (m/day)
- Convert mm/day to m/day: q(m/day) = q(mm/day)/1000

**K** = Hydraulic conductivity (m/day)

**m** = Depth from drain to impermeable layer (m)

**d** = Equivalent depth above drain level (m)
- Approximately: d = (h₁ + h₂)/2
- Or use: d ≈ 0.5 to 1.0 m typical

**L** = Drain spacing (m)

---

### Hydraulic Conductivity (K)

| Soil Type | K (m/day) |
|-----------|-----------|
| **Clay** | **0.01-0.05** ⭐ |
| **Silty clay** | 0.05-0.15 |
| **Silt loam** | 0.15-0.50 |
| **Sandy loam** | 0.50-2.0 |
| **Sand** | **2.0-10.0** ⭐ |
| **Gravel** | >10.0 |

**Memory:** 
- **Clay slow (0.01-0.05)**
- **Sand fast (2-10)**

---

### Example Calculation

**Given:**
- K = 0.5 m/day (silt loam)
- m = 3 m (to impermeable layer)
- d = 1.0 m (equivalent depth)
- q = 12 mm/day = 0.012 m/day

**Find drain spacing (L):**

$$
L = \sqrt{\frac{4 \times 0.5 \times (2 \times 3 \times 1 + 1^2)}{0.012}}
$$

$$
= \sqrt{\frac{2.0 \times (6 + 1)}{0.012}} = \sqrt{\frac{2.0 \times 7}{0.012}}
$$

$$
= \sqrt{\frac{14}{0.012}} = \sqrt{1167} = 34.2 \text{ m}
$$

**Use L = 30-35 m** ⭐

---

### Simplified Hooghoudt

**When m >> d (deep impermeable layer):**

$$
\boxed{q = \frac{8Kmd}{L^2}}
$$

$$
\boxed{L = \sqrt{\frac{8Kmd}{q}}}
$$

This is easier to calculate!

---

## 📏 Drain Spacing Guidelines

### By Soil Type

| Soil Texture | Spacing (m) |
|--------------|-------------|
| **Heavy clay** | **10-20** ⭐ |
| Clay loam | 15-30 |
| Loam | 20-40 |
| **Sandy loam** | **30-60** ⭐ |
| Sand | 50-100 |

**Memory:**
- **Clay = 10-20 m (closer)**
- **Sandy = 30-60 m (wider)**

**Why?**
- Clay: Low K → Need closer drains
- Sandy: High K → Can space wider

---

### By Crop Type

| Crop | Spacing (m) |
|------|-------------|
| Rice | 20-30 |
| **Wheat/Cereals** | **20-40** |
| **Vegetables** | **15-30** |
| Orchards | 25-50 |
| Pasture | 30-60 |

---

### By Depth

**Drain depth affects spacing:**

| Depth (m) | Relative Spacing |
|-----------|------------------|
| 0.8 | 1.0 × (baseline) |
| 1.0 | 1.2 × |
| **1.2** | **1.4 ×** ⭐ |
| 1.5 | 1.6 × |

**Deeper drains → Wider spacing possible**

---

## 🏗️ Design Criteria

### Drain Depth

**Typical depth:** **1.0-2.0 m** ⭐

**Factors:**

**Minimum depth:**
- Below plow layer (0.3-0.4 m)
- Below root zone
- Minimum 0.6 m for protection

**Maximum depth:**
- Economic limit (~2-3 m)
- Installation difficulty
- Outlet availability

**Optimum:** **1.0-1.5 m** for most crops

---

### Drain Diameter

**Based on discharge:**

| Drainage Area (ha) | Diameter (mm) |
|--------------------|---------------|
| <5 | **75-100** ⭐ |
| 5-10 | **100-150** ⭐ |
| 10-20 | 150-200 |
| 20-40 | 200-300 |
| >40 | 300-400 |

**Minimum:** 75 mm (to prevent clogging)

---

### Drain Slope

**Minimum gradient:** **0.1-0.2%** ⭐

| Slope (%) | Suitability |
|-----------|-------------|
| <0.1 | Inadequate (siltation) |
| **0.1-0.2** | **Minimum acceptable** ⭐ |
| **0.2-0.5** | **Good** ⭐ |
| 0.5-1.0 | Excellent |
| >1.0 | May need energy dissipation |

**Too flat (<0.1%):** Sediment deposits  
**Too steep (>1%):** High velocity, erosion

---

### Envelope/Filter

**Purpose:** Prevent soil particles entering drain

**Material:**
- Gravel (10-20 mm size)
- Synthetic fabric
- Coconut fiber

**Thickness:** 50-100 mm around pipe

**When needed:**
- Fine sandy soils
- Unstable soils
- High silt load

---

## 🧮 Donnan Equation (Alternative)

**Another formula for drain spacing:**

$$
\boxed{L = \sqrt{\frac{4K \times H \times (2d + H)}{q}}}
$$

Where:
- H = Height of water table above drain
- d = Depth from drain to impermeable layer
- Other terms same as Hooghoudt

**Less common in GATE, but know it exists!**

---

## 🔧 Drainage Materials

### Pipe Materials

**1. Concrete pipes**
- Diameter: 75-300 mm
- Life: 30-50 years
- Cost: Moderate
- Heavy (difficult to handle)

**2. PVC pipes**
- Diameter: 50-200 mm
- Life: 25-40 years
- Cost: Moderate
- **Lightweight (easy installation)** ⭐
- **Most popular currently**

**3. Corrugated plastic (HDPE)**
- Flexible
- Life: 30-50 years
- Cost: Low-moderate
- Good for uneven settling

**4. Clay tiles (Traditional)**
- Diameter: 75-150 mm
- Life: 50+ years
- Brittle, difficult to handle
- Rarely used now

---

### Comparison

| Material | Cost | Life | Weight | Popularity |
|----------|------|------|--------|------------|
| Concrete | ₹₹ | 50 yr | Heavy | Low |
| **PVC** | **₹₹** | **40 yr** | **Light** | **High** ⭐ |
| HDPE | ₹ | 40 yr | Light | Medium |
| Clay | ₹ | 60 yr | Heavy | Low |

---

## 📐 Installation Guidelines

### Layout

**1. Main drain**
- Lowest elevation
- Adequate outlet
- Usually along field boundary

**2. Lateral drains**
- Perpendicular to contours
- Flow into main drain
- Parallel spacing (L)

**3. Collector drains**
- Connect laterals to main
- Larger diameter

---

### Installation Depth

**Steps:**

1. Survey field elevations
2. Determine outlet elevation
3. Calculate drain depths
4. Check minimum depth (1.0 m)
5. Maintain minimum slope (0.2%)

---

### Junction Design

**At junctions:**
- Smooth transitions
- Drop of 2-5 cm (energy dissipation)
- Inspection chambers (every 50-100 m)

---

## 📊 Design Example

### Complete Drainage Design

**Problem:**
Design a subsurface drainage system for:
- Field area: 10 ha
- Soil: Clay loam
- K = 0.2 m/day
- Crop: Wheat (q = 12 mm/day)
- Impermeable layer: 4 m below surface
- Desired drain depth: 1.2 m

---

**Step 1: Calculate drain spacing**

**m** = 4 - 1.2 = 2.8 m (drain to impermeable layer)

**d** ≈ 0.8 m (assume)

**q** = 0.012 m/day

**Hooghoudt equation:**
$$
L = \sqrt{\frac{4K(2md + d^2)}{q}}
$$

$$
= \sqrt{\frac{4 \times 0.2 \times (2 \times 2.8 \times 0.8 + 0.8^2)}{0.012}}
$$

$$
= \sqrt{\frac{0.8 \times (4.48 + 0.64)}{0.012}} = \sqrt{\frac{0.8 \times 5.12}{0.012}}
$$

$$
= \sqrt{\frac{4.096}{0.012}} = \sqrt{341.3} = 18.5 \text{ m}
$$

**Use spacing L = 18-20 m** ⭐

---

**Step 2: Number of laterals**

Field width = √(10 × 10,000) ≈ 316 m (if square)

Number of drains = 316 / 18 ≈ **17-18 laterals**

---

**Step 3: Drain diameter**

Each lateral drains: 10 / 18 ≈ 0.55 ha

For <5 ha per drain: **Use 100 mm diameter** ⭐

---

**Step 4: Slope**

Maintain minimum **0.2%** slope

For 300 m length: Drop = 300 × 0.002 = 0.6 m

---

**Step 5: Outlet**

Ensure main drain outlet is at least:
- 1.2 m + 0.6 m = 1.8 m below field surface at upper end

---

## 📏 Specifications Table

### Subsurface Drainage

| Parameter | Value |
|-----------|-------|
| **Drain depth** | **1.0-2.0 m** ⭐ |
| **Drain spacing** | 10-100 m (soil-dependent) |
| **Drain diameter** | 75-300 mm |
| **Minimum slope** | **0.1-0.2%** ⭐ |
| **Envelope thickness** | 50-100 mm |
| **Inspection chambers** | Every 50-100 m |

---

### By Soil Type

| Soil | K (m/day) | Spacing (m) |
|------|-----------|-------------|
| **Heavy clay** | **0.01-0.05** | **10-20** ⭐ |
| Clay loam | 0.05-0.15 | 15-30 |
| Silt loam | 0.15-0.50 | 20-40 |
| **Sandy loam** | **0.5-2.0** | **30-60** ⭐ |
| Sand | 2-10 | 50-100 |

---

### Drainage Coefficient

| Application | q (mm/day) |
|-------------|------------|
| **Field crops** | **10-15** ⭐ |
| **Vegetables** | **15-20** ⭐ |
| Rice | 5-8 |
| Orchards | 10-12 |
| **Humid climate** | 15-25 |
| Arid climate | 8-12 |

---

## 🎯 Key Takeaways

**Critical Formulas:**

1. **Hooghoudt equation:**
$$
q = \frac{4K(2md + d^2)}{L^2}
$$

$$
L = \sqrt{\frac{4K(2md + d^2)}{q}}
$$

2. **Simplified:**
$$
L = \sqrt{\frac{8Kmd}{q}}
$$

---

**Must Remember:**

- ✓ Drain depth: **1.0-2.0 m** ⭐
- ✓ Drain slope: **0.1-0.2% minimum** ⭐
- ✓ Drainage coefficient: **10-15 mm/day (field crops)** ⭐
- ✓ Clay spacing: **10-20 m** ⭐
- ✓ Sandy spacing: **30-60 m** ⭐
- ✓ K value: **Clay 0.01-0.05, Sand 2-10 m/day** ⭐
- ✓ Minimum diameter: **75-100 mm** ⭐

---

## 🔗 Related Topics

- [Soil Erosion & Conservation](../Soil_Erosion/README.md)
- [Water Harvesting](../Water_Harvesting/README.md)
- [Watershed Management](../Watershed_Management/README.md)

---

## 📚 Practice

- [PYQ Solutions](./Solutions.md)
- [Quick CheatSheet](./CheatSheet.md)

---

**Last Updated:** November 2025  
**Next Topic:** [Watershed Management](../Watershed_Management/README.md)

---

*Drain smart, farm better! 🌊*
