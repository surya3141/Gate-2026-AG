# 📝 Seeding & Planting Equipment Cheat Sheet

> Quick reference for GATE Agricultural Engineering

---

## 🌱 Seeding Methods

| Method | Precision | Equipment | Crops | Seed Rate |
|--------|-----------|-----------|-------|-----------|
| **Broadcasting** | Low | Broadcaster | Wheat, Rice | High |
| **Drilling** | Medium | Seed Drill | Cereals | Medium |
| **Precision Planting** | High | Planter | Maize, Cotton | Low |
| **Transplanting** | High | Transplanter | Rice | Very Low |
| **Dibbling** | Medium | Dibbler | Maize, Beans | Medium |

---

## 🔧 Seed Drill vs Planter

| Feature | Seed Drill | Planter |
|---------|------------|---------|
| **Placement** | Continuous | Precise spacing |
| **Metering** | Fluted roller | Cell/Vacuum |
| **Crops** | Small grains | Row crops |
| **Precision** | Medium | Very High |
| **Spacing** | Random in row | Fixed |
| **Seeds/position** | Multiple | 1-3 |

---

## ⚙️ Seed Drill Components

### Main Parts
1. **Hopper** - Stores seeds
2. **Metering device** - Controls rate
3. **Furrow opener** - Makes furrow
4. **Seed tube** - Conveys seeds
5. **Covering device** - Covers seeds
6. **Ground wheel** - Drives mechanism
7. **Markers** - Next row marking

### Specifications
- Rows: **7-13**
- Row spacing: **15-23 cm**
- Depth: **2-10 cm**
- Width: **2-3 m**
- Speed: **3-5 km/h**
- Tractor: **25-35 HP**

---

## 🔄 Metering Mechanisms

### Types

| Type | Principle | Precision | Seed Types | Cost |
|------|-----------|-----------|------------|------|
| **Fluted Roller** | Force feed | Medium | All sizes | Low |
| **Cell Type** | Mechanical | High | Large | Medium |
| **Vacuum** | Air suction | Very High | All | High |
| **Brush** | Gravity | Medium | Small, round | Low |

### Fluted Roller

**Seed Rate Formula:**
$$
Q = \frac{60 \times A \times L \times N_r \times \rho}{10^6}
$$

Where:
- Q = Seed rate (kg/ha)
- A = Flute area (cm²)
- L = Effective length (cm)
- N_r = Roller RPM
- ρ = Bulk density (kg/m³)

**Simplified:**
$$
Q = K \times L \times N
$$

---

## 🌾 Furrow Openers

### Types and Applications

| Type | Soil Type | Trash | Draft | Best Use |
|------|-----------|-------|-------|----------|
| **Shoe** | Light-Medium | Poor | Low | General |
| **Hoe** | Heavy | Fair | Medium | Hard soil |
| **Inverted-T** | Medium | Good | Medium | Precision |
| **Disc** | All | Good | Medium | Trashy |
| **Triple Disc** | All | Excellent | Low | No-till |

### Disc Furrow Opener
- Diameter: **35-45 cm**
- Angle: **8-12°**
- Best for: Trashy, wet conditions

---

## 🌽 Planter Specifications

### General
- Row spacing: **60-90 cm**
- Plant spacing: **10-30 cm**
- Metering: Cell type/Vacuum
- Precision: Very high

### Plant Spacing Formula

$$
\text{Spacing (cm)} = \frac{V \times 100}{N_c \times N_p / 60}
$$

Where:
- V = Forward speed (m/s)
- N_c = Number of cells
- N_p = Plate RPM

**Simplified:**
$$
S = \frac{60 \times V}{N_c \times N_p}
$$

### Cell Size
$$
D_{\text{cell}} = (1.2 \text{ to } 1.5) \times D_{\text{seed}}
$$

**Typical:** 1.3 × seed diameter

---

## 🌾 Rice Transplanter

### Types
- **Manual:** 0.1-0.15 ha/h
- **Walking:** 0.2-0.4 ha/h
- **Riding:** 0.3-0.5 ha/h

### Specifications
- Rows: **4-8**
- Row spacing: **20-30 cm**
- Plant spacing: **12-20 cm**
- Depth: **2-4 cm**
- Seedlings/hill: **2-6**
- Seedling age: **15-25 days**

### Mat Seedling
- Tray size: **30×60 cm**
- Height: **12-20 cm**
- Root length: **2-3 cm**
- Density: **3000-4000 plants/m²**

---

## 📐 Key Formulas

### Plant Population

$$
P = \frac{10000}{R \times S}
$$

Where:
- P = Plants/ha
- R = Row spacing (m)
- S = Plant spacing (m)

**Example:** R=0.6m, S=0.2m → P = 83,333 plants/ha

---

### Seed Rate

$$
Q = \frac{N \times n \times W}{S \times 10}
$$

Where:
- Q = Seed rate (kg/ha)
- N = Seeds/m/row
- n = Number of rows
- W = 1000-seed weight (g)
- S = Row spacing (cm)

---

### Quality of Feed Index

**Miss Index (M):**
% of spacings > 1.5 × mean

**Multiple Index (D):**
% of spacings < 0.5 × mean

**Quality Index:**
$$
Q = 100 - (M + D)
$$

**Rating:**
- Q > 85%: **Good**
- Q = 70-85%: **Acceptable**
- Q < 70%: **Poor**

---

### Field Capacity

**TFC:**
$$
\text{TFC (ha/h)} = \frac{W \times S}{10}
$$

**EFC:**
$$
\text{EFC} = \text{TFC} \times \eta_f
$$

**Typical Efficiency:**
- Seed drill: **70-80%**
- Planter: **65-75%**
- Transplanter: **60-70%**

---

### Broadcasting

**Effective Width:**
$$
W_{\text{eff}} = 0.7 \times W_{\text{total}}
$$

**Uniformity (CV):**
$$
\text{CV} = \frac{\sigma}{\mu} \times 100\%
$$

**Good:** CV < 15%

---

## 📊 Quick Comparison Tables

### Sowing Depth Guide

| Seed Type | Depth | Examples |
|-----------|-------|----------|
| **Small** | 1-2 cm | Mustard, Millet |
| **Medium** | 3-5 cm | Wheat, Barley |
| **Large** | 5-8 cm | Maize, Soybean |

### Seed Rate Ranges

| Crop | Seed Rate (kg/ha) | Row Spacing (cm) |
|------|-------------------|------------------|
| **Wheat** | 100-125 | 20-23 |
| **Rice** | 80-100 | 20-25 |
| **Maize** | 18-25 | 60-75 |
| **Cotton** | 12-20 | 60-90 |
| **Soybean** | 60-80 | 45-60 |

---

## 💡 Problem-Solving Guide

### Type 1: Plant Population
**Given:** Row spacing (R), Plant spacing (S)  
**Find:** Population (P)

$$
P = \frac{10000}{R \times S}
$$

**Units:** R and S in meters

---

### Type 2: Plant Spacing (Planter)
**Given:** Cells (N_c), RPM (N_p), Speed (V)  
**Find:** Spacing (S)

$$
S = \frac{60 \times V}{N_c \times N_p}
$$

**Units:** V in m/s, S in m

---

### Type 3: Quality Index
**Given:** Miss (M%), Multiple (D%)  
**Find:** Quality (Q)

$$
Q = 100 - (M + D)
$$

---

### Type 4: Seed Rate
**Given:** Seeds/m (N), Rows (n), Weight (W), Spacing (S)  
**Find:** Rate (Q)

$$
Q = \frac{N \times n \times W}{S \times 10}
$$

---

### Type 5: Field Capacity
**Given:** Width (W), Speed (S), Efficiency (η)  
**Find:** EFC

1. TFC = (W × S) / 10
2. EFC = TFC × η

---

## 🎯 Memory Tricks

### Drill vs Planter (Mnemonic: "DCP")
- **D**rill - **D**istributed continuously
- **P**lanter - **P**recise placement

### Quality Index
- **Q** = 100 - (M + D)
- **M**iss = Too far
- **D**ouble = Too close
- **Q**uality = What remains

### Cell Size
- **1.2 to 1.5** times seed diameter
- Remember: **1.3** is optimal

### Furrow Opener Selection
- **Trashy + Wet** = **Triple Disc**
- **Hard + Dry** = **Hoe**
- **General** = **Shoe**

---

## 🚨 Common Mistakes

1. **Units confusion:** Row spacing in m, not cm
2. **Population formula:** 10000, not 10^6
3. **Quality index:** Q = 100 - (M+D), not M+D
4. **Cell size:** 1.2-1.5×, not 2×
5. **Field capacity:** Divide by 10, not 1000
6. **Spacing:** Use correct formula for planter
7. **Seed rate:** Include all rows

---

## 🎓 GATE Strategy

### High Weightage Topics ⭐⭐⭐⭐⭐
1. **Plant population calculation**
2. **Seed rate formulas**
3. **Quality of feed index**
4. **Drill vs Planter differences**
5. **Field capacity**

### Medium Weightage ⭐⭐⭐
- Metering mechanisms
- Furrow opener selection
- Transplanter specifications
- Cell size calculation

### Time Allocation
- **1 mark (Easy):** 2 minutes
- **2 marks (Medium):** 3-4 minutes
- **2 marks (Hard):** 5 minutes

---

## 📋 Quick Check Questions

**Q1:** Formula for plant population?  
**A:** P = 10000/(R×S)

**Q2:** Drill vs Planter main difference?  
**A:** Precision of placement

**Q3:** Quality index formula?  
**A:** Q = 100 - (M + D)

**Q4:** Cell size for 8mm seed?  
**A:** 10-12 mm (1.2-1.5×)

**Q5:** Transplanter rows?  
**A:** 4-8 rows

**Q6:** Good quality index?  
**A:** Q > 85%

**Q7:** Effective broadcast width?  
**A:** 0.7 × Total width

**Q8:** Seed drill efficiency?  
**A:** 70-80%

---

## 🔢 Standard Values

| Parameter | Value | Unit |
|-----------|-------|------|
| **Drill rows** | 7-13 | - |
| **Drill spacing** | 15-23 | cm |
| **Planter spacing** | 60-90 | cm |
| **Transplanter rows** | 4-8 | - |
| **Cell size factor** | 1.2-1.5 | × seed dia |
| **Disc opener dia** | 35-45 | cm |
| **Disc angle** | 8-12 | degrees |
| **Quality index** | >85 | % (good) |
| **Drill efficiency** | 70-80 | % |

---

## ✅ Pre-Exam Checklist

- [ ] Know P = 10000/(R×S)
- [ ] Master Q = 100-(M+D)
- [ ] Remember cell size: 1.2-1.5×
- [ ] Drill vs Planter differences
- [ ] TFC = (W×S)/10
- [ ] Furrow opener selection
- [ ] Typical efficiencies
- [ ] Metering types
- [ ] Transplanter specs

---

## 🔗 Related Topics

- **Tillage:** Seedbed preparation
- **Farm Power:** Tractor requirements
- **Crop Science:** Seed rates, spacing

---

**Created for:** GATE Agricultural Engineering  
**Last Updated:** November 2025  
**Total Formulas:** 10+  
**Key Topics:** 8

---

*For detailed theory, see [Seeding & Planting README](./README.md)*  
*For practice problems, see [PYQ Solutions](./Solutions.md)*
