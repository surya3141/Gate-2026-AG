# ⚡ Post-Harvest Machinery - Quick Reference

> Essential formulas, specifications, and memory tricks for GATE AG

---

## 🔑 Key Formulas

### 1. Moisture Content Conversion

**Wet Basis to Dry Basis:**
$$
MC_{db} = \frac{MC_{wb}}{100 - MC_{wb}} \times 100
$$

**Dry Basis to Wet Basis:**
$$
MC_{wb} = \frac{MC_{db}}{100 + MC_{db}} \times 100
$$

**Memory Trick:** **"DB bigger than WB"** (for same grain)

---

### 2. Water to Remove

$$
W_r = W_i \times \frac{M_i - M_f}{100 - M_f}
$$

Where:
- W_r = Water to remove (kg)
- W_i = Initial weight (kg)
- M_i = Initial MC% (wb)
- M_f = Final MC% (wb)

**Quick Check:** Final weight = W_i - W_r

---

### 3. Storage Capacity

**Bulk Storage (Rectangular):**
$$
\text{Capacity (tons)} = L \times W \times H \times \rho
$$

**Cylindrical Silo:**
$$
M = \frac{\pi D^2 H}{4} \times \rho
$$

**Bag Storage:**
$$
\text{Capacity} = \text{Volume} \times \text{Utilization} \times \rho
$$

Where utilization = 0.55-0.60 (55-60%)

---

### 4. Silo Pressure

**Lateral Pressure:**
$$
P = k \times \rho \times g \times h
$$

Where k = 0.4-0.5 (lateral pressure coefficient)

---

### 5. Aeration Airflow

$$
Q_{air} = M \times \text{Specific airflow}
$$

**Specific airflow:** 5-20 m³/min/ton (depending on climate)

---

### 6. Milling Recovery

$$
\text{Recovery (\%)} = \frac{\text{Output weight}}{\text{Input weight}} \times 100
$$

**Head Rice Recovery:**
$$
\text{HRR} = \frac{\text{Head rice}}{\text{Paddy input}} \times 100
$$

---

### 7. Cleaning Efficiency

$$
\eta_c = \frac{\text{Impurity removed}}{\text{Total impurity}} \times 100
$$

---

### 8. Specific Energy Consumption (Dryer)

$$
\text{SEC} = \frac{\text{Total energy input}}{\text{Water removed}} \text{ (kJ/kg or MJ/kg)}
$$

---

## 📊 Safe Storage Moisture Content

| Grain | Safe MC (% wb) | Mold Growth Above |
|-------|----------------|-------------------|
| **Wheat** | 12-14% | >15% |
| **Paddy/Rice** | 13-14% | >16% |
| **Maize** | 13-14% | >16% |
| **Pulses** | 10-12% | >14% |
| **Soybean** | 10-11% | >13% |
| **Groundnut** | 8-9% | >10% |

**Memory:** **"Most grains safe at 12-14%"**

---

## 🌡️ Safe Drying Temperatures

| Grain | Seed (°C) | Commercial (°C) |
|-------|-----------|-----------------|
| **Paddy** | 40-43 | 60 |
| **Wheat** | 45-50 | 70 |
| **Maize** | 40-45 | 80 |
| **Pulses** | 40 | 60 |

**Memory:** **"Seeds need Cool (40s), Commercial can take Heat (60-80)"**

---

## 🧹 Cleaning Equipment Comparison

| Equipment | Principle | Removes | Efficiency |
|-----------|-----------|---------|------------|
| **Winnower** | Air + Screen | Chaff, dust, size | 85-95% |
| **Gravity separator** | Density | Stones, light grains | 90-98% |
| **Destoner** | Fluidization | Stones | >99% |
| **Magnetic** | Magnetism | Ferrous metals | ~100% |

**Memory:** **"Air for Light, Density for Weight, Magnet for Metal"**

---

## 📊 Grading Methods

### By Parameter

| Method | Separates By | Equipment | Application |
|--------|--------------|-----------|-------------|
| **Screen/Sieve** | Size (L, W, T) | Flat/rotary screens | All grains |
| **Indented cylinder** | Length | Rotating cylinder | Broken vs whole |
| **Gravity** | Density | Air classifier | Hollow vs filled |
| **Color sorter** | Color | Optical + air jet | Discolored, defects |

---

### Color Sorter Specs

| Parameter | Specification |
|-----------|---------------|
| **Capacity** | 1-5 t/h per chute |
| **Chutes** | 64-512 (multi-chute) |
| **Accuracy** | 98-99.9% |
| **Air pressure** | 5-7 bar |
| **Response time** | <10 milliseconds |

**Application:** Rice, pulses, coffee, spices

---

## 🔥 Dryer Types Comparison

| Dryer Type | Mode | Capacity | Drying Time | Use |
|------------|------|----------|-------------|-----|
| **Sun drying** | Batch | Any | 3-7 days | Small farms |
| **LSU/Bin** | Batch | 2-10 tons | 8-24 hours | Medium farms |
| **Column** | Continuous | 2-20 t/h | Single pass | Commercial |
| **Fluidized bed** | Batch | 1-5 tons | 30-60 min | Seed, high MC |

**Memory:** **"Sun Slow, Column Continuous, Fluidized Fast"**

---

### Dryer Performance

| Parameter | Value/Range |
|-----------|-------------|
| **Drying efficiency** | 40-60% |
| **Typical SEC** | 4-10 MJ/kg water |
| **Theoretical minimum** | 2.5 MJ/kg water |
| **Moisture reduction** | 4-8% per pass (column) |

---

## 🏗️ Storage Structures

### Types

| Type | Capacity | Cost | Use |
|------|----------|------|-----|
| **Godown (bag)** | Any | Medium | Flexible |
| **Godown (bulk)** | Any | Medium | Commercial |
| **Steel bin** | 5-100 tons | Low | Farm-level |
| **Tower silo** | 100-5000 tons | High | Large scale |

---

### Silo Design

| Parameter | Specification |
|-----------|---------------|
| **Height:Diameter** | 2-4:1 |
| **Typical height** | 15-30 m |
| **Typical diameter** | 3-10 m |
| **Cone angle** | 45-60° |
| **Fill level** | 85-95% of height |

**Memory:** **"Silo Tall (H = 2-4 × D), Cone Steep (45-60°)"**

---

### Bulk Density

| Material | Bulk Density (t/m³) |
|----------|---------------------|
| **Wheat** | 0.75-0.80 |
| **Paddy** | 0.55-0.60 |
| **Rice (milled)** | 0.75-0.80 |
| **Maize** | 0.70-0.75 |
| **Pulses** | 0.75-0.85 |

**Average for calculations:** **0.75-0.80 t/m³**

---

## 🌬️ Aeration System

### Airflow Requirements

| Climate/Purpose | Airflow (m³/min/ton) |
|-----------------|----------------------|
| **Cool - maintenance** | 2-5 |
| **Warm - maintenance** | 5-10 |
| **Hot - cooling** | 10-20 |
| **Drying** | 20-50 |

**Memory:** **"Cool 5, Warm 10, Hot 20"**

---

### Design Guidelines

| Parameter | Specification |
|-----------|---------------|
| **Duct spacing** | 2-4 m |
| **Duct diameter** | 20-50 cm |
| **Air velocity in grain** | 0.1-0.5 m/min |
| **Static pressure** | 50-500 Pa (depends on depth) |

---

## 🍚 Rice Milling

### Process Sequence

```
PADDY → CLEANING → DESTONING → DEHUSKING → 
PADDY SEPARATION → WHITENING → POLISHING → GRADING
```

---

### Milling Yields (from Paddy)

| Product | Typical Yield % |
|---------|-----------------|
| **Brown rice** | 80-82% |
| **Total milled rice** | 68-72% |
| **Head rice (HRR)** | 55-65% |
| **Broken rice** | 10-15% |
| **Husk** | 18-20% |
| **Bran** | 8-10% |

**Memory:** **"HRR 60, Total 70, Husk 20, Bran 10"** (rough averages)

---

### Rice Milling Equipment

| Equipment | Function | Output |
|-----------|----------|--------|
| **Rubber roll sheller** | Dehusk | Brown rice + husk |
| **Paddy separator** | Density separate | Paddy vs brown rice |
| **Abrasive whitener** | Remove bran | White rice + bran |
| **Friction whitener** | Polish bran | White rice |
| **Polisher** | Glossy finish | Polished rice |
| **Grader** | Size separate | Head vs broken |

---

### Sheller Specs

**Rubber Roll Sheller:**
- Roll diameter: 20-30 cm
- Speed ratio: 2.5:1
- Gap: 1-2 mm
- Dehusking: 85-95%

**Paddy Separator:**
- Based on density difference
- Paddy: 1100 kg/m³
- Brown rice: 1400 kg/m³

---

## 🌾 Wheat Milling

### Process

```
WHEAT → CLEANING → TEMPERING → GRINDING (ROLLER MILL) → 
SIEVING → PURIFICATION → FLOUR
```

---

### Tempering

**Purpose:** Add moisture (to 14-16%) for 8-24 hours

**Benefits:**
- Softens bran
- Toughens endosperm
- Easier separation

---

### Milling Yields

| Product | Yield % |
|---------|---------|
| **Flour (total)** | 72-76% |
| **Bran** | 18-22% |
| **Loss** | 4-8% |

---

## 🔧 Parboiling

### Process Steps

1. **Soaking:** 3-6 h (hot 60-70°C) or 20-24 h (cold)
2. **Steaming:** 10-20 min at 1-2 bar (100-120°C)
3. **Drying:** To 14% MC

---

### Benefits

| Benefit | Improvement |
|---------|-------------|
| **Head rice yield** | +10-15% (from 60% to 70%) |
| **Nutrition** | Vitamins migrate to endosperm |
| **Hardness** | Better storage, less insect damage |
| **Milling** | Easier, less breakage |

**Disadvantage:** Yellowish color

**Memory:** **"Parboil = Plus Yield Plus Nutrition"**

---

## 📦 Material Handling

### Equipment Selection

| Equipment | Best For | Height | Capacity |
|-----------|----------|--------|----------|
| **Belt conveyor** | Horizontal | Incline <20° | 10-1000 t/h |
| **Screw conveyor** | Short distance | Incline <45° | 5-100 t/h |
| **Bucket elevator** | **Vertical** | **Up to 50 m** | 10-200 t/h |
| **Pneumatic** | Flexible route | Any | 5-50 t/h |

**Memory:** **"Vertical = Bucket Elevator"**

---

## 🧮 Quick Calculation Templates

### Template 1: MC Conversion

**Given:** 20% wb

**To db:**
$$
MC_{db} = \frac{20}{100-20} \times 100 = \frac{20}{80} \times 100 = 25\%
$$

---

### Template 2: Water Removal

**Given:** 1000 kg at 20% → 14% MC

**Solution:**
$$
W_r = 1000 \times \frac{20-14}{100-14} = 1000 \times \frac{6}{86} = 69.77 \text{ kg}
$$

Final weight = 1000 - 69.77 = 930.23 kg

---

### Template 3: Silo Capacity

**Given:** D = 6 m, H = 20 m, ρ = 0.8 t/m³

**Solution:**
$$
M = \frac{3.14159 \times 6^2 \times 20}{4} \times 0.8 = 565.5 \times 0.8 = 452.4 \text{ tons}
$$

---

### Template 4: Godown Capacity (Bulk)

**Given:** 25 m × 12 m × 4 m, ρ = 0.75 t/m³

**Solution:**
$$
M = 25 \times 12 \times 4 \times 0.75 = 900 \text{ tons}
$$

---

### Template 5: Godown Capacity (Bags)

**Given:** Same dimensions, 55% utilization

**Solution:**
$$
M = 25 \times 12 \times 4 \times 0.55 \times 0.75 = 495 \text{ tons}
$$

---

### Template 6: Aeration Airflow

**Given:** 500 tons, specific airflow = 8 m³/min/ton

**Solution:**
$$
Q = 500 \times 8 = 4000 \text{ m}^3\text{/min}
$$

---

### Template 7: Milling Recovery

**Given:** 10 tons paddy → 6.8 tons rice

**Solution:**
$$
\text{Recovery} = \frac{6.8}{10} \times 100 = 68\%
$$

---

## 💡 Problem-Solving Strategy

### For MC Conversion:
1. Identify given basis (wb or db)
2. Use appropriate formula
3. Remember: db > wb for same grain

### For Water Removal:
1. Use formula: W_r = W_i × (M_i - M_f)/(100 - M_f)
2. Check answer: Final weight = Initial - Removed
3. Final MC verification optional

### For Storage Capacity:
1. Calculate volume (L×W×H or πD²H/4)
2. Multiply by bulk density (0.75-0.80)
3. For bags: Also multiply by utilization (0.55)

### For Milling:
1. Output/Input × 100 = Recovery
2. Check if asking for head rice or total rice
3. Sum of all products ≤ 100%

---

## ⚠️ Common Mistakes to Avoid

### ❌ Don't:
- Confuse wb and db (db is always higher)
- Forget to subtract M_f from 100 in water removal formula
- Use wrong bulk density (check grain type)
- Forget space utilization factor for bag storage
- Mix up head rice with total milled rice

### ✅ Do:
- Check moisture basis in question
- Verify final weight after water removal
- Use standard bulk density if not given (0.75-0.80)
- Remember silo fill = 85-95% of height
- Know equipment for vertical lifting = bucket elevator

---

## 📊 Comparison Tables

### Storage Methods

| Aspect | Bag Storage | Bulk Storage |
|--------|-------------|--------------|
| **Space utilization** | 55-60% | 90-95% |
| **Labor** | High | Low |
| **Cost** | Medium | High (initial) |
| **Flexibility** | High | Low |
| **Inspection** | Easy | Difficult |

---

### Drying Methods

| Method | Time | Cost | Quality | Weather Dependent |
|--------|------|------|---------|-------------------|
| **Sun** | 3-7 days | Zero | Fair | Yes |
| **Batch** | 8-24 h | Medium | Good | No |
| **Continuous** | Hours | High | Excellent | No |

---

## 💭 Memory Tricks

### Safe Storage MC:
**"Most grains 12-14, Oilseeds 8-10"**

### Silo Dimensions:
**"Height = 2 to 4 times Diameter"**

### Bulk Density:
**"Point Seven Five to Eight" (0.75-0.80)**

### MC Basis:
**"Dry Bigger" (db > wb)**

### Vertical Lift:
**"Bucket Beats All for Height"**

### Parboiling:
**"Soak-Steam-Dry = Stronger-Smarter-Safer grain"**

### HRR:
**"Higher HRR = Happier Rice Revenue"**

### Aeration:
**"Cool Five, Warm Ten, Hot Twenty"** (m³/min/ton)

---

## 📝 Pre-Exam Checklist

### Must Remember Formulas:
- [ ] MC conversion: MC_db = MC_wb/(100-MC_wb) × 100
- [ ] Water removal: W_r = W_i × (M_i-M_f)/(100-M_f)
- [ ] Silo capacity: M = πD²H/4 × ρ
- [ ] Godown capacity: L×W×H×ρ (×0.55 for bags)
- [ ] Milling recovery: Output/Input × 100

### Must Know Values:
- [ ] Safe MC: 12-14% for most grains
- [ ] Bulk density: 0.75-0.80 t/m³
- [ ] HRR: 55-65% typical, 65-70% parboiled
- [ ] Husk: 18-20%, Bran: 8-10%
- [ ] Bag utilization: 55-60%
- [ ] Silo fill: 85-95%

### Must Know Equipment:
- [ ] Gravity separator = density separation
- [ ] Bucket elevator = vertical lift
- [ ] Rubber roll sheller = dehusking
- [ ] Color sorter = optical grading
- [ ] Column dryer = continuous drying

---

## 🎯 Exam Strategy

### Time Management:
- **1 mark:** 1-2 minutes (concepts, equipment ID)
- **2 marks:** 3-5 minutes (calculations)
- MC conversion: 2 min
- Water removal: 3 min
- Capacity: 3-4 min

### High Weightage Topics:
1. Moisture content and drying (★★★)
2. Storage capacity calculations (★★★)
3. Milling yield and recovery (★★★)
4. Cleaning and grading equipment (★★)
5. Equipment selection (★★)

### Quick Win Topics:
- MC conversion (easy 1-2 marks)
- Equipment functions (1 mark each)
- Safe storage values (memory-based)
- Bucket elevator for vertical (1 mark)

---

## 🔗 Related Topics

- [Detailed Theory](./README.md)
- [PYQ Solutions](./Solutions.md)
- [Farm Machinery Overview](../README.md)
- [Complete GATE AG Package](../../)

---

**Quick Reference Version 1.0**  
**Last Updated:** November 2025  
**Topics Covered:** Cleaning, Grading, Drying, Storage, Milling, Handling  
**For:** GATE Agricultural Engineering

---

*Print this for last-minute revision!*  
*Master these formulas and values for guaranteed marks in post-harvest questions.*

🌾 **Store Smart, Mill Right, Grade Bright!** 🏗️
