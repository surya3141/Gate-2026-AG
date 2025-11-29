# 🏞️ Watershed Management - Quick Reference CheatSheet

> Last-minute revision for GATE Agricultural Engineering

---

## 🔢 Critical Formula - Rational Method

$$
\boxed{Q = \frac{C \times I \times A}{360}}
$$

**Units:**
- Q: m³/s
- C: dimensionless
- I: mm/hr
- A: hectares

**Memory: "CIA/360"** ⭐

---

## 📐 SCS Curve Number Method

$$
\boxed{Q = \frac{(P - 0.2S)^2}{P + 0.8S}}
$$

$$
\boxed{S = \frac{25400}{CN} - 254}
$$

**Condition:** Q = 0 if P < 0.2S

**Memory: "Quarter S initial, 25400 for S"** ⭐

---

## 📊 Runoff Coefficient (C) Values

| Land Use/Surface | C Value |
|------------------|---------|
| **Forest** | **0.05-0.20** ⭐ |
| **Grassland** | 0.10-0.30 |
| **Cultivated land** | **0.20-0.40** ⭐ |
| **Bare soil** | 0.30-0.60 |
| Rocky terrain | 0.60-0.90 |
| **Paved/Urban** | **0.80-0.95** ⭐ |

**Typical values:**
- Forest: **0.10**
- Cultivated: **0.30**
- Paved: **0.90**

**Memory: "10-30-90 Forest-Farm-Paved"** ⭐

---

## 🌧️ SCS Curve Numbers (CN)

**AMC-II (Normal conditions):**

| Land Use | Soil Group | | | |
|----------|---|---|---|---|
| | **A** | **B** | **C** | **D** |
| **Forest (good)** | **30** ⭐ | 55 | 70 | 77 |
| Pasture (good) | 39 | **61** | 74 | 80 |
| Small grains | 63 | 75 | **83** | 87 |
| Row crops | 67 | 78 | 85 | 89 |
| **Fallow (bare)** | 77 | 86 | 91 | **94** ⭐ |
| **Paved** | **98** | **98** | **98** | **98** ⭐ |

**Memory:**
- **"Forest A = 30"** (lowest)
- **"Fallow D = 94"** (highest agricultural)
- **"Paved = 98"** (almost all runoff)

---

## 🏞️ Soil Groups

| Group | Infiltration | Runoff Potential | Examples |
|-------|--------------|------------------|----------|
| **A** | **High** | **Low** | Sand, gravel |
| B | Moderate | Moderate-low | Sandy loam, loam |
| C | Low | Moderate-high | Clay loam, silt loam |
| **D** | **Very low** | **High** | Clay, shallow soil |

**Memory: "A-high infiltration, D-low infiltration"** ⭐

---

## ⏱️ Time of Concentration

**Kirpich Formula:**

$$
\boxed{T_c = 0.0195 \times L^{0.77} \times S^{-0.385}}
$$

**Units:**
- T_c: minutes
- L: meters
- S: m/m (slope)

**Memory: "0.02 L^0.8 S^-0.4"** (approximately) ⭐

---

## 📏 Morphometric Parameters

### Form Factor

$$
\boxed{R_f = \frac{A}{L^2}}
$$

| R_f | Shape | Flood Risk |
|-----|-------|------------|
| 0.8-1.0 | Circular | **High** ⚠️ |
| 0.5-0.8 | Oval | Moderate |
| **0.3-0.5** | **Elongated** ⭐ | **Low** ✓ |
| <0.3 | Very elongated | Very low |

**Memory: "Lower Rf = Safer"** ⭐

---

### Circularity Ratio

$$
\boxed{R_c = \frac{12.57A}{P^2}}
$$

**Perfect circle:** Rc = 1.0

**Interpretation:** Higher Rc → More circular → Higher peaks

---

### Elongation Ratio

$$
\boxed{R_e = \frac{1.128\sqrt{A}}{L}}
$$

| Re | Shape |
|----|-------|
| 0.9-1.0 | Circular |
| **0.6-0.8** | **Elongated** ⭐ |
| <0.6 | Very elongated |

---

### Compactness Coefficient

$$
\boxed{C_c = \frac{0.282P}{\sqrt{A}}}
$$

**Perfect circle:** Cc = 1.0

**Higher Cc → More elongated**

---

## 🧮 Quick Calculations

### Rational Method

**Given:** C=0.30, I=50 mm/hr, A=10 ha

$$
Q = \frac{0.30 \times 50 \times 10}{360} = \frac{150}{360} = 0.417 \text{ m}^3/\text{s}
$$

---

### SCS-CN Runoff

**Given:** P=100mm, CN=70

**Step 1: Calculate S**
$$
S = \frac{25400}{70} - 254 = 362.9 - 254 = 108.9 \text{ mm}
$$

**Step 2: Calculate Ia**
$$
I_a = 0.2 \times 108.9 = 21.8 \text{ mm}
$$

**Step 3: Check P > Ia**
100 > 21.8 ✓

**Step 4: Calculate Q**
$$
Q = \frac{(100-21.8)^2}{100+0.8 \times 108.9} = \frac{6115.24}{187.1} = 32.7 \text{ mm}
$$

---

### Time of Concentration

**Given:** L=2000m, S=0.02

$$
T_c = 0.0195 \times 2000^{0.77} \times 0.02^{-0.385}
$$

$$
≈ 0.0195 \times 472 \times 3.35 = 30.8 \text{ min}
$$

---

### Form Factor

**Given:** A=36 km², L=9 km

$$
R_f = \frac{36}{81} = 0.44
$$

**Elongated watershed** (0.3-0.5)

---

## 📊 Comparison Tables

### CN by AMC

| Condition | CN_II=70 | Runoff |
|-----------|----------|--------|
| AMC-I (Dry) | 50 | Low |
| **AMC-II (Normal)** | **70** ⭐ | Medium |
| AMC-III (Wet) | 85 | High |

**Memory: "Wetter = Higher CN = More runoff"**

---

### Watershed Shape Comparison

| Parameter | Circular | Elongated |
|-----------|----------|-----------|
| Form factor (Rf) | 0.8-1.0 | 0.3-0.5 |
| Flood peak | High | Low |
| Response time | Short | Long |
| Safety | Lower | Higher |

---

### C Values by Surface

| Surface | C | Runoff % |
|---------|---|----------|
| Forest | 0.10 | 10% |
| Cultivated | 0.30 | 30% |
| Bare soil | 0.45 | 45% |
| Rocky | 0.75 | 75% |
| Paved | 0.90 | 90% |

---

## ⚠️ Common Exam Mistakes

### Mistake 1: Rational Formula Divisor
❌ Using 100 or other divisor  
✅ **Always 360 for Q(m³/s), I(mm/hr), A(ha)**

---

### Mistake 2: C Values
❌ Forest = 0.5, Paved = 0.3  
✅ **Forest = 0.1, Paved = 0.9**

---

### Mistake 3: SCS Initial Abstraction
❌ Ia = 0.5S or Ia = 0.1S  
✅ **Ia = 0.2S** (one-fifth)

---

### Mistake 4: CN Values
❌ Forest has high CN  
✅ **Forest A = 30 (lowest), Fallow D = 94**

---

### Mistake 5: Form Factor Interpretation
❌ Higher Rf = Elongated  
✅ **Lower Rf = Elongated = Safer**

---

### Mistake 6: SCS Condition
❌ Calculate Q even if P < Ia  
✅ **Q = 0 if P < 0.2S**

---

### Mistake 7: Stream Ordering
❌ 2 + 2 = 2  
✅ **2 + 2 = 3** (same order → next higher)

---

## 🎓 Memory Techniques

### "CIA/360"
**Rational formula:** Q = **C × I × A / 360**

---

### "10-30-90"
**C values:**
- Forest: **0.10**
- Cultivated: **0.30**
- Paved: **0.90**

---

### "Forest 30"
**CN value:** Forest on soil A = **30** (lowest)

---

### "Fallow 94"
**CN value:** Fallow on soil D = **94** (highest agricultural)

---

### "0.2S Initial"
**SCS:** Initial abstraction Ia = **0.2S** (one-fifth)

---

### "25400 for S"
**SCS:** S = **25400/CN - 254**

---

### "0.02 L-slope"
**Kirpich:** Tc ≈ **0.02 × L^0.8 × S^-0.4**

---

### "Lower Rf Safer"
**Form factor:** **Lower** Rf = Elongated = **Safer** (lower peaks)

---

### "Same Same Next"
**Stream order:** Same + Same = Next (2+2=3)

---

## 📋 Pre-Exam Checklist

**Must Remember:**
- [ ] **Rational:** Q = CIA/360
- [ ] **C values:** Forest 0.10, Cultivated 0.30, Paved 0.90
- [ ] **SCS:** Q = (P-0.2S)²/(P+0.8S)
- [ ] **SCS:** S = 25400/CN - 254
- [ ] **SCS:** Q = 0 if P < 0.2S
- [ ] **CN:** Forest A=30, Fallow D=94, Paved=98
- [ ] **AMC-II:** Normal condition (use table values)
- [ ] **Tc:** 0.0195 L^0.77 S^-0.385
- [ ] **Form factor:** Rf = A/L² (lower = elongated = safer)
- [ ] **Stream order:** Same + Same = Next higher

---

## 🔥 High-Yield Topics

**Must Know (Every Year):**
1. ✓ Rational formula application ⭐⭐⭐
2. ✓ C values (know the table) ⭐⭐⭐
3. ✓ SCS-CN method calculation ⭐⭐⭐
4. ✓ CN values (Forest 30, Fallow 94) ⭐⭐⭐
5. ✓ Form factor interpretation ⭐⭐

**Moderate Priority:**
- Time of concentration (Kirpich)
- Other morphometric parameters
- AMC conversions
- Stream ordering

**Lower Priority:**
- Detailed watershed development
- Drainage density
- Bifurcation ratio

---

## 💡 Last-Minute Tips

**If short on time, FOCUS ON:**
1. ✓ Rational formula (Q = CIA/360)
2. ✓ C values table (0.1, 0.3, 0.9 for forest, cultivated, paved)
3. ✓ SCS-CN formulas (both Q and S)
4. ✓ CN table (Forest A=30, Fallow D=94, Paved=98)
5. ✓ Form factor (lower = elongated = safer)

**Can skip:**
- Complex morphometric derivations
- Multiple Tc formulas
- Detailed watershed prioritization
- Advanced stream analysis

---

## 🎯 Final Formula Card

**Top 5 - Commit to Memory:**

$$
\boxed{Q = \frac{C \times I \times A}{360}}
$$

$$
\boxed{Q = \frac{(P - 0.2S)^2}{P + 0.8S}}
$$

$$
\boxed{S = \frac{25400}{CN} - 254}
$$

$$
\boxed{T_c = 0.0195 \times L^{0.77} \times S^{-0.385}}
$$

$$
\boxed{R_f = \frac{A}{L^2}}
$$

---

## 📱 Quick Reference Card

**Write on exam rough sheet:**

```
RATIONAL: Q = CIA/360
C: Forest 0.1, Cultivated 0.3, Paved 0.9

SCS-CN: Q = (P-0.2S)²/(P+0.8S)
        S = 25400/CN - 254
        Q=0 if P<0.2S
        
CN: Forest A=30 (low)
    Fallow D=94 (high)
    Paved=98 (highest)

Tc: 0.0195×L^0.77×S^-0.385

Rf: A/L² (lower=elongated=safer)

STREAM: Same+Same=Next (2+2=3)
```

---

## 🔗 Navigation

- [Detailed Theory](./README.md)
- [PYQ Solutions](./Solutions.md)
- [Back to Section](../README.md)

---

**Last Updated:** November 2025  
**Section 04 COMPLETE!** ✓

---

*Master watersheds, master water! 🏞️*

🌊 **Every Drop Counts!** 🏆
