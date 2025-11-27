# 📝 Soil Working Machinery Cheat Sheet

> Quick reference for GATE Agricultural Engineering

---

## 🚜 Tillage Classification

### Types by Depth

| Type | Depth | Purpose | Equipment |
|------|-------|---------|-----------|
| **Primary** | 15-45 cm | Breaking soil | Ploughs, Subsoilers |
| **Secondary** | 5-15 cm | Seedbed prep | Harrows, Cultivators |
| **Deep** | >45 cm | Hardpan breaking | Subsoilers |

---

## 🔧 Mould Board Plough

### Types and Soil Suitability

| Type | Curve | Pulverization | Best For |
|------|-------|---------------|----------|
| **Stubble** | Short, steep | Poor | Sandy, well-drained |
| **General Purpose** | Medium | Moderate | Loamy soils |
| **Sod/Breaker** | Long, gentle | Excellent | Heavy clay, sod |
| **Slat** | Spaced bars | Good | Sticky soils |

### Components
1. **Share** - Horizontal cutting
2. **Mould board** - Inversion
3. **Landside** - Side support
4. **Frog** - Assembly base
5. **Coulter** - Vertical cutting

### Specifications
- Width per bottom: **20-30 cm**
- Depth: **15-30 cm**
- Speed: **4-6 km/h**
- Draft: **600-1000 N/bottom**

---

## 💿 Disc Plough

### Key Angles

$$
\text{Disc Angle (α)} = 42° \text{ to } 45° \text{ (horizontal)}
$$

$$
\text{Tilt Angle (β)} = 15° \text{ to } 25° \text{ (vertical)}
$$

### Specifications
- Diameter: **60-90 cm**
- Depth: **10-25 cm**
- Spacing: **25-30 cm**
- Speed: **5-8 km/h**

### Draft Formula
$$
D = K \times d \times w \times N
$$
- K = Soil constant (N/cm²)
- d = Depth (cm)
- w = Width per disc (cm)
- N = Number of discs

### Advantages over Mould Board
✓ Works in hard, dry soil  
✓ Less draft  
✓ Better trash handling  
✓ Self-sharpening

---

## 🌾 Harrows

### Disc Harrow

**Gang Angle:** 15° to 25°

**Effects of Increasing Gang Angle:**
- ↑ Cutting action
- ↑ Soil movement
- ↑ Penetration
- ↑ Draft

**Disc Specifications:**
- Diameter: **40-70 cm**
- Spacing: **20-25 cm**
- Concavity: **4-10 cm**
- Depth: **10-15 cm**

### Types
- **Offset:** Two gangs in tandem
- **Tandem:** Four gangs (front + rear)

---

## 🔱 Cultivators

### Shovel Types

| Type | Width | Application |
|------|-------|-------------|
| **Narrow Point** | 5-8 cm | Deep penetration |
| **Broad Share** | 20-30 cm | Shallow cultivation |
| **Sweep (Duck foot)** | 30-60 cm | Weed control |
| **Reversible** | 8-15 cm | General purpose |

### Specifications
- Working width: **1.5-3 m**
- Depth: **5-15 cm**
- Tine spacing: **10-15 cm**

---

## ⚙️ Rotavator

### Speed Ratio

$$
\lambda = \frac{\pi D N}{60 V}
$$

Where:
- λ = Speed ratio
- D = Rotor diameter (m)
- N = Rotor speed (rpm)
- V = Forward speed (m/s)

**Typical Range:** λ = **10-20**

### Specifications
- Width: **100-200 cm**
- Depth: **10-20 cm**
- PTO speed: **540 rpm**
- Tractor power: **35-60 HP**
- Speed: **2-4 km/h**

### Blade Types
- **L-type:** Simple, general purpose
- **C-type:** Curved, better penetration

### Blade Arrangement
- Spacing: **10-15 cm**
- Number: **24-48 blades**
- Pattern: Offset on flanges

---

## 📐 Performance Formulas

### Field Capacity

**Theoretical Field Capacity:**
$$
\text{TFC (ha/h)} = \frac{W \times S}{10}
$$
- W = Width (m)
- S = Speed (km/h)

**Effective Field Capacity:**
$$
\text{EFC} = \text{TFC} \times \eta_f
$$

**Field Efficiency:**
$$
\eta_f = \frac{\text{EFC}}{\text{TFC}} \times 100\%
$$

### Typical Efficiency Values

| Equipment | Efficiency |
|-----------|------------|
| Ploughs | 70-85% |
| Harrows | 75-90% |
| Cultivators | 70-85% |
| Rotavators | 75-85% |

---

## ⚡ Power & Draft

### Drawbar Power
$$
P_{db} \text{ (kW)} = \frac{D \times V}{3.6}
$$
- D = Draft (kN)
- V = Speed (km/h)

### PTO Power
$$
P_{PTO} \text{ (kW)} = \frac{2\pi N T}{60000}
$$
- N = Speed (rpm)
- T = Torque (Nm)

### Specific Draft
$$
\text{Specific Draft} = \frac{\text{Total Draft (N)}}{\text{Area (cm}^2\text{)}}
$$

Unit: **N/cm²**

### Power-Speed Relationship
$$
\frac{P_1}{N_1} = \frac{P_2}{N_2} \quad \text{(constant torque)}
$$

---

## 🔋 Energy

### Specific Energy
$$
E_s = \frac{\text{Energy (kJ)}}{\text{Volume (m}^3\text{)}}
$$

### Typical Values

| Equipment | Specific Energy |
|-----------|----------------|
| Mould board | 8-15 kJ/m³ |
| Disc plough | 6-10 kJ/m³ |
| Rotavator | 12-20 kJ/m³ |
| Cultivator | 4-8 kJ/m³ |

---

## 📊 Equipment Comparison

### Plough Comparison

| Feature | Mould Board | Disc | Chisel |
|---------|-------------|------|--------|
| **Inversion** | Complete | Partial | None |
| **Pulverization** | Excellent | Good | Poor |
| **Draft** | High | Medium | Low |
| **Trash Handling** | Poor | Good | Excellent |
| **Depth** | 15-30 cm | 10-25 cm | 20-60 cm |

### Secondary Tillage

| Equipment | Depth | Pulverization | Speed |
|-----------|-------|---------------|-------|
| **Disc Harrow** | 10-15 cm | Good | 6-8 km/h |
| **Cultivator** | 5-15 cm | Moderate | 4-6 km/h |
| **Rotavator** | 10-20 cm | Excellent | 2-4 km/h |
| **Spike Harrow** | 5-10 cm | Poor | 8-10 km/h |

---

## 🎯 Quick Calculation Guide

### Problem Type 1: Field Capacity
**Given:** W, S, η_f  
**Find:** EFC

1. TFC = (W × S) / 10
2. EFC = TFC × η_f

### Problem Type 2: Time Required
**Given:** Area, EFC  
**Find:** Time

$$
\text{Time} = \frac{\text{Area}}{\text{EFC}}
$$

### Problem Type 3: Draft
**Given:** Specific draft, Area  
**Find:** Total draft

$$
D = \text{Specific draft} \times \text{Area}
$$

### Problem Type 4: Power
**Given:** Draft, Speed  
**Find:** Power

$$
P = \frac{D \times V}{3.6}
$$

### Problem Type 5: Speed Ratio
**Given:** D, N, V  
**Find:** λ

$$
\lambda = \frac{\pi D N}{60 V}
$$

---

## 💡 Memory Tricks

### Mould Board Types (Mnemonic: "SSG")
- **S**tubble - **S**andy soil
- **S**od - **S**tick clay (heavy)
- **G**P - **G**eneral **P**urpose (loamy)

### Disc Plough Angles
- **Disc angle:** ~44° (close to 45°)
- **Tilt angle:** ~20° (lower)
- **Gang angle (harrow):** 15-25°

### Rotavator Speed Ratio
- **Range:** 10-20
- **Typical:** ~15
- **Remember:** Higher = more cuts per meter

### Field Efficiency
- **High efficiency (80-90%):** Harrows
- **Medium (70-85%):** Ploughs, Cultivators
- **Remember:** Secondary > Primary

---

## 🚨 Common Mistakes

1. **Wrong units:** Always convert W to meters, S to km/h
2. **Efficiency > 100%:** Impossible, check TFC calculation
3. **Forgetting factor 10:** In TFC formula
4. **Mixing angles:** Disc vs gang vs tilt
5. **Draft units:** N vs kN confusion
6. **Speed ratio:** Use consistent units (m, m/s)

---

## 🎓 GATE Strategy

### High Weightage Topics
1. **Field capacity calculations** ⭐⭐⭐⭐⭐
2. **Mould board types** ⭐⭐⭐⭐
3. **Disc angles** ⭐⭐⭐⭐
4. **Rotavator speed ratio** ⭐⭐⭐⭐
5. **Power calculations** ⭐⭐⭐

### Time Allocation
- **Easy (1 mark):** 1-2 minutes
- **Medium (2 marks):** 3-4 minutes
- **Hard (2 marks):** 5-6 minutes

### Formula Priority
1. **TFC = (W × S) / 10** - Most important
2. **EFC = TFC × η_f**
3. **λ = πDN / 60V**
4. **P = D × V / 3.6**

---

## 📋 Quick Check Questions

**Q1:** Which mould board for clay soil?  
**A:** Sod/Breaker

**Q2:** Disc plough angle range?  
**A:** 42-45° (disc), 15-25° (tilt)

**Q3:** Rotavator speed ratio typical value?  
**A:** 10-20 (typically ~15)

**Q4:** Field efficiency of harrows?  
**A:** 75-90%

**Q5:** Primary tillage depth?  
**A:** 15-45 cm

**Q6:** TFC formula?  
**A:** (W × S) / 10

**Q7:** Duck foot cultivator use?  
**A:** Weed control, minimum disturbance

**Q8:** Subsoiler depth?  
**A:** 45-90 cm

---

## 🔢 Standard Values Table

| Parameter | Value | Unit |
|-----------|-------|------|
| **Mould board width** | 20-30 | cm/bottom |
| **Mould board depth** | 15-30 | cm |
| **Disc diameter** | 60-90 | cm |
| **Disc angle** | 42-45 | degrees |
| **Gang angle** | 15-25 | degrees |
| **Rotavator width** | 100-200 | cm |
| **Rotavator depth** | 10-20 | cm |
| **PTO speed** | 540 | rpm |
| **Speed ratio (λ)** | 10-20 | - |
| **Cultivator depth** | 5-15 | cm |

---

## 📐 Conversion Factors

- **1 ha** = 10,000 m²
- **1 kW** = 1000 W
- **1 kN** = 1000 N
- **Speed:** km/h = m/s × 3.6
- **Power:** kW = HP × 0.746

---

## ✅ Pre-Exam Checklist

- [ ] Know all mould board types
- [ ] Memorize disc angles (42-45°, 15-25°)
- [ ] Master TFC formula
- [ ] Understand speed ratio concept
- [ ] Practice power calculations
- [ ] Review typical efficiency values
- [ ] Know primary vs secondary tillage
- [ ] Understand draft relationships

---

## 🔗 Related Topics

- **Farm Power:** Tractor specifications, power transmission
- **Soil Mechanics:** Soil properties, compaction
- **Seeding Equipment:** Follow-up operations

---

**Created for:** GATE Agricultural Engineering  
**Last Updated:** November 2025  
**Total Formulas:** 12+  
**Key Topics:** 8

---

*For detailed theory, see [Soil Working Machinery README](./README.md)*  
*For practice problems, see [PYQ Solutions](./Solutions.md)*
