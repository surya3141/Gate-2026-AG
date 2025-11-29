# 🥛 Milk Processing & Products

> **Comprehensive Theory for GATE 2026**

---

## 📚 Table of Contents
1. [Milk Composition](#milk-composition)
2. [Milk Properties](#milk-properties)
3. [Heat Treatment](#heat-treatment)
4. [Cream Separation](#cream-separation)
5. [Homogenization](#homogenization)
6. [Milk Standardization](#milk-standardization)
7. [Dairy Products](#dairy-products)

---

## 🥛 Milk Composition

### Standard Composition (Buffalo Milk)
```
Component        Buffalo    Cow      Goat
─────────────────────────────────────────
Fat              7-8%      3.5-4%   3.5-4%
SNF              9-10%     8.5-9%   8.5-9%
Protein          4.0%      3.2-3.5% 3.5%
  - Casein       3.1%      2.6%     2.7%
  - Whey         0.9%      0.6%     0.8%
Lactose          4.8%      4.6-4.8% 4.5%
Ash              0.8%      0.7%     0.8%
Total Solids     16-18%    12-13%   12.5%
```

**Critical relationships:**
$$
\text{Total Solids (TS)} = \text{Fat} + \text{SNF}
$$
$$
\text{SNF} = \text{TS} - \text{Fat}
$$
$$
\text{SNF} = \text{Protein} + \text{Lactose} + \text{Ash}
$$

### Milk Proteins 🔥

**1. Casein (80% of total protein)**
- Phosphoprotein, forms micelles
- Precipitates at pH 4.6
- Heat stable (up to 100°C)
- Used: Cheese, casein products

**2. Whey Proteins (20%)**
- Albumin, globulin
- Heat sensitive (denature 70-80°C)
- Nutritionally superior
- Used: Whey protein concentrates

**Calculation:**
$$
\text{Casein} = \text{Total Protein} - \text{Whey Protein}
$$

For cow milk: 3.2 - 0.6 = **2.6% casein**

### Milk Fat

**Characteristics:**
- Emulsion: Fat globules in water
- Size: 0.5-15 μm (average 4-5 μm)
- Cream rises: Lower density than water
- Melting point: 28-38°C

**Composition:**
- Triglycerides: 98%
- Phospholipids: 1%
- Sterols: 0.5%

**Fatty acids:**
- Saturated: 65% (palmitic, stearic)
- Unsaturated: 35% (oleic)

---

## 📊 Milk Properties

### Physical Properties

**1. Density:**
$$
\rho_{milk} = 1.028 - 1.032 \text{ kg/L at 15°C}
$$

**Factors affecting:**
- Fat content ↓ → Density ↑
- Temperature ↑ → Density ↓
- SNF ↑ → Density ↑

**Lactometer:** Measures density, detects adulteration

**2. pH:**
- **Fresh milk: 6.6-6.8** (slightly acidic)
- Due to casein, phosphates, citrates
- Sour milk: pH < 6.0 (lactic acid formation)

**3. Viscosity:**
- Cow milk: 1.5-2.0 cP at 20°C
- Affected by: Fat, protein, temperature
- ↑ Homogenization → ↑ Viscosity

**4. Specific Heat:**
- Whole milk: 3.93 kJ/(kg·°C)
- Skim milk: 4.02 kJ/(kg·°C)
- Higher fat → Lower specific heat

**5. Freezing Point:**
- -0.525 to -0.550°C
- Used to detect water addition
- Cryoscope test

---

## 🌡️ Heat Treatment (Pasteurization & Sterilization)

### Pasteurization Methods 🔥🔥🔥

**1. LTLT (Low Temperature Long Time)**
- **Temperature:** 63°C
- **Time:** 30 minutes
- **Method:** Batch (vat pasteurizer)
- **Use:** Small dairies, specialty products

**2. HTST (High Temperature Short Time)**
- **Temperature:** 72°C
- **Time:** 15 seconds
- **Method:** Continuous (plate heat exchanger)
- **Use:** Commercial standard ✓

**3. UHT (Ultra High Temperature)**
- **Temperature:** 135-150°C
- **Time:** 2-4 seconds
- **Method:** Direct (steam injection) or Indirect (plate/tubular)
- **Shelf life:** 6-9 months at room temperature

### Comparison Table

| Method | Temp | Time | Equipment | Quality | Shelf Life |
|--------|------|------|-----------|---------|------------|
| LTLT | 63°C | 30 min | Batch vat | Good | 7-10 days |
| **HTST** | **72°C** | **15 sec** | **PHE** | **Best** ✓ | **14-16 days** |
| UHT | 135-150°C | 2-4 sec | Direct/Indirect | Fair | 6-9 months |

**HTST advantages:**
- Better organoleptic quality than LTLT
- Continuous process (higher capacity)
- Energy recovery (regeneration 85-95%)
- Less protein denaturation

**PHE (Plate Heat Exchanger):**
- Stainless steel plates with gaskets
- Counter-current flow
- Regeneration section (milk-to-milk heat exchange)
- Heating section (hot water/steam)
- Cooling section (chilled water/glycol)

### Phosphatase Test

**Purpose:** Verify adequate pasteurization

**Principle:**
- Phosphatase enzyme in milk
- Inactivated at 72°C/15s
- If positive → Under-pasteurized

**Result:**
- **Negative (no color):** Proper pasteurization ✓
- **Positive (blue/yellow):** Under-pasteurized ✗

---

## 🌊 Cream Separation

### Stokes' Law 🔥

Fat globules rise due to density difference:
$$
v = \frac{2gr^2(\rho_m - \rho_f)}{9\mu}
$$

where:
- v = Rising velocity (m/s)
- g = Acceleration due to gravity (9.81 m/s²)
- r = Fat globule radius (m)
- ρₘ = Milk density (kg/m³)
- ρf = Fat density (kg/m³)
- μ = Viscosity (Pa·s)

**Key relationships:**
- v ∝ g (velocity proportional to acceleration)
- v ∝ r² (larger globules rise faster)
- v ∝ (ρₘ - ρf) (greater density difference → faster)

### Centrifugal Separation

**Centrifugal force:**
$$
F_c = m \omega^2 r = m \times \frac{v^2}{r}
$$

**Acceleration:**
$$
a_c = \omega^2 r = \frac{v^2}{r}
$$

where:
- ω = Angular velocity (rad/s) = 2πN/60
- N = Speed (rpm)
- r = Radius (m)

**Important:** 
$$
F_c \propto N^2
$$

**Doubling speed → 4× centrifugal force**

**Cream separator:**
- Conical disc stack
- Centrifugal acceleration: 5,000-10,000 g
- Separation efficiency: >99%
- Capacity: 5,000-50,000 L/hr

---

## 🔬 Homogenization

### Purpose
- Reduce fat globule size: 4-5 μm → 0.5-2 μm
- Prevent creaming
- Improve mouthfeel, whiteness

### Process
```
Milk → Pump → Homogenization valve → Homogenized milk
         ↓
     High pressure
     (10-20 MPa)
```

**Pressure:** 10-20 MPa (100-200 bar)
- First stage: 15 MPa
- Second stage: 3-5 MPa (prevents clustering)

### Homogenization Valve

**Principle:**
- Milk forced through narrow gap under high pressure
- Shear forces + cavitation break fat globules
- New surface formed → Casein micelles adsorb

**Effects:**
- ↑ Viscosity (more surface area)
- ↑ Whiteness (light scattering)
- ↑ Stability (no cream separation)
- ↓ Churning tendency

**Temperature:** 60-70°C during homogenization

---

## ⚖️ Milk Standardization 🔥🔥

### Purpose
Adjust fat/SNF to meet standards (e.g., Toned milk 3% fat)

### Pearson's Square Method

**Example:** Standardize 100 kg milk (5% fat) to 3% fat using skim milk (0% fat)

**Setup:**
```
      Milk (5%)          3-0 = 3 parts
          ╲            ╱
           ╲          ╱
            ╲        ╱
             Target (3%)
            ╱        ╲
           ╱          ╲
          ╱            ╲
   Skim milk (0%)    5-3 = 2 parts
```

**Calculation:**
- Milk parts: 3
- Skim parts: 2
- Total parts: 3+2 = 5

**For 100 kg total:**
- Milk: (3/5) × 100 = **60 kg**
- Skim: (2/5) × 100 = **40 kg**

**Verification:**
$$
\frac{60 \times 5 + 40 \times 0}{100} = \frac{300}{100} = 3\% \text{ ✓}
$$

### Another Example: Using Cream

Standardize 100 kg milk (3% fat) to 4.5% fat using cream (40% fat)

**Pearson's Square:**
```
      Milk (3%)         40-4.5 = 35.5 parts
                     ╱
                Target (4.5%)
                     ╲
      Cream (40%)    4.5-3 = 1.5 parts
```

**Total parts:** 35.5 + 1.5 = 37

**For 100 kg standardized milk:**
- Milk: (35.5/37) × 100 = 95.9 kg
- Cream: (1.5/37) × 100 = **4.1 kg**

---

## 🧈 Dairy Products

### 1. Butter (80% Fat) 🔥

**Process:**
```
Cream (30-40% fat) → Aging/Ripening → Churning → Butter + Buttermilk
```

**Steps:**
1. **Cream separation:** 30-40% fat
2. **Pasteurization:** 85-95°C (destroys enzymes)
3. **Aging:** 12-15°C, 12-24 hrs (fat crystallization)
4. **Churning:** Agitation → Phase inversion (fat continuous)
5. **Washing:** Remove buttermilk
6. **Salting:** 1-2% (optional)
7. **Working:** Distribute moisture evenly

**Composition (IS 1155):**
- Fat: Minimum **80%**
- Moisture: Maximum 16%
- SNF: 1-2%
- Salt: 0-3%

**Types:**
- Salted butter
- Unsalted (sweet) butter
- Cultured butter (with lactic culture)

### 2. Cheese

**Process:**
```
Milk → Standardization → Pasteurization → Coagulation → Curd cutting → Whey drainage → Salting → Aging
```

**Coagulation methods:**
1. **Acid coagulation:** Lactic acid lowers pH to 4.6 (casein isoelectric point)
   - Example: Paneer, cottage cheese
2. **Rennet coagulation:** Enzyme (chymosin) cleaves casein
   - Example: Cheddar, Gouda

**Classification by moisture:**

| Type | Moisture | Examples | Aging |
|------|----------|----------|-------|
| Hard | 30-40% | Cheddar, Parmesan | 3-24 months |
| Semi-hard | 40-50% | Gouda, Edam | 1-6 months |
| Soft | 50-80% | Cottage, Camembert | 0-2 months |

**Cheddar (hard cheese):**
- Moisture: 36-38%
- Aging: 3-12 months
- Characteristic: Firm texture, sharp flavor

### 3. Yogurt (Dahi)

**Culture:**
- *Lactobacillus bulgaricus* (rods, acid producer)
- *Streptococcus thermophilus* (cocci, aroma producer)
- **Symbiotic relationship** ✓

**Process:**
```
Milk → Heat treatment (90°C, 5 min) → Cool (43-45°C) → Inoculate (2-3%) → Incubate (4-6 hrs) → Cool → Store
```

**Fermentation:**
- Lactose → Lactic acid
- pH: 6.6 → 4.5
- Acidity: 0.15% → 0.85-0.90% LA
- Protein coagulation at pH 4.6

**Quality:**
- Smooth gel
- No wheying off
- Mild acid flavor

### 4. Ice Cream

**Composition:**
- Fat: 10-16%
- SNF: 9-12%
- Sugar: 12-16%
- Stabilizer: 0.2-0.5%
- Emulsifier: 0.1-0.2%
- Total solids: 36-40%

**Process:**
```
Mix preparation → Pasteurization (68°C/30 min) → Homogenization (15-20 MPa) → Aging (4°C, 4-24 hrs) → Freezing (-5 to -6°C) → Hardening (-30°C)
```

**Overrun:**
$$
\text{Overrun (\%)} = \frac{V_{ice cream} - V_{mix}}{V_{mix}} \times 100
$$

Typical: 80-100%

**Purpose:** Light texture, scoopability

### 5. Milk Powder

**Spray Drying:**
- Atomization → Hot air drying → Powder collection
- Inlet: 180-230°C
- Outlet: 70-100°C
- Moisture: 3-4%

**Types:**
- Skim milk powder (SMP): <1.5% fat
- Whole milk powder (WMP): 26-28% fat

**Advantages:**
- Long shelf life (6-12 months)
- Easy transport
- Reduced volume/weight

---

## 📈 Summary

### Critical Formulas
```
TS = Fat + SNF
SNF = TS - Fat
Casein = Total Protein - Whey
v ∝ g (Stokes' law)
F ∝ N² (centrifugal force)
```

### Must-Remember Values
```
Fat: 3.5-4% (cow)
SNF: 8.5-9%
TS: 12-13%
Density: 1.028-1.032 kg/L
pH: 6.6-6.8
HTST: 72°C/15 sec ← Most important
UHT: 135-150°C/2-4 sec
Butter: 80% fat minimum
Homogenization: 10-20 MPa
```

---

*[Solutions](./Solutions.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
