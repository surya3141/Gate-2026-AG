# 💧 Water Harvesting Structures - Quick Reference CheatSheet

> Last-minute revision for GATE Agricultural Engineering

---

## 🔢 Critical Formulas

### 1. Farm Pond Capacity

$$
\boxed{V = \frac{H}{3}(A_1 + A_2 + \sqrt{A_1 \times A_2})}
$$

**Quick approximation:**
$$
V \approx \frac{L \times W \times D}{2}
$$

---

### 2. Runoff Calculation

$$
\boxed{R = C \times I \times A}
$$

**Or:**
$$
\boxed{V = C \times P \times A \times E}
$$

Where E = Collection efficiency (0.7-0.8)

---

### 3. Rational Method

$$
\boxed{Q = \frac{C \times I \times A}{360}}
$$

Units: Q (m³/s), I (mm/hr), A (ha)

---

### 4. Check Dam Spacing

$$
\boxed{D = \frac{H}{S}}
$$

H = Dam height (m), S = Slope (m/m)

---

### 5. Contour Bund VI

$$
\boxed{VI = 0.3S + 1.0}
$$

S = Slope (%)

**Horizontal spacing:**
$$
HI = \frac{VI \times 100}{S}
$$

---

### 6. Spillway Design

$$
\boxed{Q = C_d \times L \times H^{1.5}}
$$

Typical C_d = 1.7-1.9

---

## 📊 Runoff Coefficient (C) Values

| Land Use | C Value |
|----------|---------|
| **Forest** | 0.05-0.20 |
| Grassland | 0.10-0.30 |
| **Cultivated land** | **0.20-0.40** ⭐ |
| **Bare soil** | 0.30-0.60 |
| Rocky terrain | 0.60-0.90 |
| Paved surface | 0.80-0.95 |

**Memory: "Cultivated = 0.3 typical"** ⭐

---

## 📏 Farm Pond Specifications

| Parameter | Value |
|-----------|-------|
| **Capacity** | 500-5000 m³ |
| **Depth** | **2.5-3.5 m** ⭐ |
| **Side slope** | **2:1 to 3:1** ⭐ |
| Freeboard | 0.5 m |
| Embankment top | 2-3 m |
| **Catchment ratio** | **5:1 to 10:1** ⭐ |

**Memory:** 
- **"3m deep"**
- **"2:1 slope"**
- **"10:1 catchment"**

---

## 🏗️ Check Dam Specifications

| Parameter | Value |
|-----------|-------|
| **Height** | **2-4 m (max)** ⭐ |
| **Base thickness** | **0.5H to 0.7H** ⭐ |
| Spillway width | 1-3 m |
| Foundation depth | 0.5-1.0 m |
| Apron length | 1.5-2.0 m |
| **Spacing formula** | **D = H/S** ⭐ |

**Memory: "Thickness = 0.6H"** ⭐

---

## 💧 Percolation Tank

| Parameter | Value |
|-----------|-------|
| Capacity | 1,000-500,000 m³ |
| Depth | 2-4 m |
| Catchment ratio | 10:1 to 20:1 |
| **Infiltration (good)** | **5-15 mm/hr** ⭐ |
| Infiltration (excellent) | 15-50 mm/hr |
| Embankment slope | 2:1 to 3:1 |

**Memory: "5-15 mm/hr = Good"** ⭐

---

## 🏔️ Contour Bund

| Parameter | Value |
|-----------|-------|
| **Height** | 0.5-1.0 m |
| Top width | 0.5-1.0 m |
| Side slope | 1.5:1 to 2:1 |
| **VI formula** | **0.3S + 1.0** ⭐ |
| **Grade** | **0.1-0.3%** ⭐ |
| **Suitable slope** | **2-5%** ⭐ |

**Memory: "VI = 0.3S + 1"** ⭐

---

## 🧮 Quick Calculations

### Farm Pond Volume

**Given:** L=30m, W=20m, D=3m, slope=2:1

**Bottom:**
- L_b = 30 - 2(2×3) = 18 m
- W_b = 20 - 2(2×3) = 8 m

**Areas:**
- A₁ = 30×20 = 600 m²
- A₂ = 18×8 = 144 m²

**Volume:**
$$
V = \frac{3}{3}[600 + 144 + \sqrt{600 \times 144}]
$$
$$
= 744 + 294 = 1038 \text{ m}^3
$$

---

### Runoff Volume

**Given:** Area=5ha, Rainfall=800mm, C=0.30, E=0.75

**Runoff depth:**
$$
R = 0.30 \times 0.8 = 0.24 \text{ m}
$$

**Volume:**
$$
V = 0.24 \times 50,000 \times 0.75 = 9,000 \text{ m}^3
$$

---

### Check Dam Spacing

**Given:** H=2.5m, S=5%=0.05

$$
D = \frac{2.5}{0.05} = 50 \text{ m}
$$

---

### Contour Bund Spacing

**Given:** Slope=6%

**VI:**
$$
VI = 0.3 \times 6 + 1.0 = 2.8 \text{ m}
$$

**HI:**
$$
HI = \frac{2.8 \times 100}{6} = 47 \text{ m}
$$

---

### Rational Method

**Given:** C=0.35, I=60mm/hr, A=8ha

$$
Q = \frac{0.35 \times 60 \times 8}{360} = \frac{168}{360} = 0.467 \text{ m}^3/\text{s}
$$

---

### Spillway Length

**Given:** Q=3.0m³/s, C_d=1.8, H=0.5m

$$
H^{1.5} = (0.5)^{1.5} = 0.354
$$

$$
L = \frac{3.0}{1.8 \times 0.354} = 4.7 \text{ m}
$$

---

## 🎯 Comparison Tables

### Pond Side Slope Reduction

| Slope | Depth 3m | Bottom Reduction |
|-------|----------|------------------|
| 1:1 | 3 m | 2×(1×3) = 6 m |
| **2:1** | **3 m** | **2×(2×3) = 12 m** ⭐ |
| 3:1 | 3 m | 2×(3×3) = 18 m |

**Memory: "2:1 slope → 12m total reduction for 3m depth"**

---

### Check Dam Height vs Spacing

| H (m) | S=5% | S=10% |
|-------|------|-------|
| 2.0 | 40 m | 20 m |
| **2.5** | **50 m** | **25 m** ⭐ |
| 3.0 | 60 m | 30 m |

**Memory: Steeper slope → Closer dams**

---

### Contour Bund VI by Slope

| Slope (%) | VI (m) | HI (m) |
|-----------|--------|--------|
| 2 | 1.6 | 80 |
| 4 | 2.2 | 55 |
| **6** | **2.8** | **47** ⭐ |
| 8 | 3.4 | 43 |
| 10 | 4.0 | 40 |

**Memory: "6% → VI=2.8m, HI=47m"**

---

## ⚠️ Common Exam Mistakes

### Mistake 1: Runoff Coefficient
❌ Forest = 0.5, Cultivated = 0.1  
✅ **Forest = 0.1, Cultivated = 0.3**

---

### Mistake 2: Pond Depth
❌ 5-6 m typical  
✅ **2.5-3.5 m typical**

---

### Mistake 3: Check Dam Thickness
❌ 0.5-0.7 m fixed  
✅ **0.5-0.7 × Height**

---

### Mistake 4: Percolation Rate
❌ 1-5 mm/hr is good  
✅ **5-15 mm/hr is good**

---

### Mistake 5: Side Slope
❌ Reducing only one dimension  
✅ **Reduce BOTH L and W** (each by 2×slope×depth)

---

### Mistake 6: VI Formula
❌ VI = 0.3 + S  
✅ **VI = 0.3S + 1.0**

---

## 🎓 Memory Techniques

### "3-2-10"
**Farm pond specs:**
- **3** m depth
- **2:1** slope
- **10:1** catchment ratio

---

### "0.3 Cultivated"
**Runoff coefficient:** Cultivated land = **0.3**

---

### "H/S Spacing"
**Check dams:** Spacing = **H/S** (Height ÷ Slope)

---

### "0.6H Thick"
**Check dam:** Base thickness = **0.6 × Height**

---

### "5-15 Good"
**Percolation:** **5-15 mm/hr** = Good recharge rate

---

### "0.3S+1"
**Contour VI:** VI = **0.3 × Slope% + 1.0**

---

### "2-5% Bund"
**Contour bunds:** Suitable for **2-5%** slope

---

## 📋 Pre-Exam Checklist

**Must Remember:**
- [ ] **Pond depth:** 2.5-3.5 m
- [ ] **Side slope:** 2:1 to 3:1
- [ ] **Runoff C:** Cultivated 0.20-0.40 (typical 0.3)
- [ ] **Check dam:** Max height 3-4 m
- [ ] **Check dam thickness:** 0.5-0.7H
- [ ] **Check dam spacing:** D = H/S
- [ ] **Percolation good:** 5-15 mm/hr
- [ ] **VI formula:** 0.3S + 1.0
- [ ] **Rational:** Q = CIA/360
- [ ] **Catchment ratio:** 5:1 to 10:1

---

## 🔥 High-Yield Topics

**Must Know (Every Year):**
1. ✓ Farm pond capacity calculation ⭐⭐⭐
2. ✓ Runoff coefficient values ⭐⭐⭐
3. ✓ Runoff volume calculation ⭐⭐⭐
4. ✓ Check dam spacing ⭐⭐
5. ✓ Contour bund VI ⭐⭐

**Moderate Priority:**
- Rational formula
- Check dam thickness
- Spillway design
- Percolation rate

**Lower Priority:**
- Detailed embankment design
- Silt trap calculations
- Apron length specifics

---

## 💡 Last-Minute Tips

**If short on time, FOCUS ON:**
1. ✓ Pond capacity formula (trapezoidal)
2. ✓ Runoff coefficient table (know cultivated=0.3)
3. ✓ Check dam spacing (D=H/S)
4. ✓ VI formula (0.3S+1)
5. ✓ Typical specifications (3m depth, 2:1 slope, 0.6H thick)

**Can skip:**
- Complex spillway calculations
- Detailed embankment volumes
- Advanced percolation theory

---

## 🎯 Final Formula Card

**Top 5 - Commit to Memory:**

$$
\boxed{V = \frac{H}{3}(A_1 + A_2 + \sqrt{A_1 A_2})}
$$

$$
\boxed{R = C \times P \times A \times E}
$$

$$
\boxed{Q = \frac{CIA}{360}}
$$

$$
\boxed{D = \frac{H}{S}}
$$

$$
\boxed{VI = 0.3S + 1.0}
$$

---

## 📱 Quick Reference Card

**Write on exam rough sheet:**

```
POND: V = H/3(A1+A2+√A1A2)
      Depth 2.5-3.5m, Slope 2:1
      
RUNOFF: R = C×P×A×E
        C cultivated = 0.3
        
RATIONAL: Q = CIA/360

CHECK DAM: D = H/S
           Thickness = 0.6H
           Max height 3-4m
           
PERCOLATION: 5-15 mm/hr good

BUND: VI = 0.3S+1
      Slope 2-5%
```

---

## 🔗 Navigation

- [Detailed Theory](./README.md)
- [PYQ Solutions](./Solutions.md)
- [Back to Section](../README.md)

---

**Last Updated:** November 2025  
**Exam Ready!** ✓

---

*Harvest every drop, ace every question! 💧*

🌊 **Water is Life!** 🏆
