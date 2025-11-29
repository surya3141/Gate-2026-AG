# 🌊 Land Drainage - Quick Reference CheatSheet

> Last-minute revision for GATE Agricultural Engineering

---

## 🔢 Critical Formula - Hooghoudt Equation

$$
\boxed{q = \frac{4K(2md + d^2)}{L^2}}
$$

**Rearranged for spacing:**

$$
\boxed{L = \sqrt{\frac{4K(2md + d^2)}{q}}}
$$

**Memory: "4K over L-squared"** ⭐

---

## 📐 Simplified Hooghoudt

**When m > 5d (deep impermeable layer):**

$$
\boxed{L = \sqrt{\frac{8Kmd}{q}}}
$$

**Much easier to calculate!**

---

## 📊 Hydraulic Conductivity (K)

| Soil Type | K (m/day) |
|-----------|-----------|
| **Clay** | **0.01-0.05** ⭐ |
| Silty clay | 0.05-0.15 |
| Silt loam | 0.15-0.50 |
| Loam | 0.25-0.50 |
| Sandy loam | 0.50-2.0 |
| **Sand** | **2.0-10.0** ⭐ |
| Gravel | >10.0 |

**Memory:**
- **"Clay slow: 0.01-0.05"**
- **"Sand fast: 2-10"**

---

## 💧 Drainage Coefficient (q)

| Application | q (mm/day) |
|-------------|------------|
| Rice | 5-8 |
| **Field crops** | **10-15** ⭐ |
| **Vegetables** | **15-20** ⭐ |
| Orchards | 10-12 |
| **Humid climate** | **15-25** |
| Arid climate | 8-12 |

**Memory: "Field crops = 10-15"** ⭐

---

## 📏 Drain Spacing by Soil

| Soil Texture | K (m/day) | Spacing (m) |
|--------------|-----------|-------------|
| **Heavy clay** | 0.01-0.05 | **10-20** ⭐ |
| Clay loam | 0.05-0.15 | 15-30 |
| Loam | 0.15-0.50 | 20-40 |
| **Sandy loam** | 0.50-2.0 | **30-60** ⭐ |
| Sand | 2-10 | 50-100 |

**Memory:**
- **"Clay close: 10-20m"**
- **"Sandy wide: 30-60m"**

**Lower K → Closer drains!**

---

## 🏗️ Drain Specifications

| Parameter | Value |
|-----------|-------|
| **Depth** | **1.0-2.0 m** ⭐ |
| **Optimum depth** | **1.0-1.5 m** |
| **Minimum slope** | **0.1-0.2%** ⭐ |
| **Good slope** | **0.2-0.5%** ⭐ |
| **Minimum diameter** | **75 mm** ⭐ |
| Typical diameter | 100-150 mm |
| Inspection chambers | Every 50-100 m |
| Envelope thickness | 50-100 mm |

**Memory:**
- **"1-2m deep"**
- **"0.2% slope"**
- **"75mm minimum"**

---

## 🧮 Quick Calculations

### Hooghoudt Example

**Given:** K=0.4, m=3.0, d=0.8, q=0.015 m/day

**Step 1: Calculate 2md + d²**
$$
2md + d^2 = 2(3.0)(0.8) + 0.8^2 = 4.8 + 0.64 = 5.44
$$

**Step 2: Apply formula**
$$
L = \sqrt{\frac{4 \times 0.4 \times 5.44}{0.015}} = \sqrt{\frac{8.704}{0.015}} = \sqrt{580} = 24 \text{ m}
$$

---

### Simplified Hooghoudt

**Given:** K=0.5, m=5, d=0.6, q=0.012

$$
L = \sqrt{\frac{8 \times 0.5 \times 5 \times 0.6}{0.012}} = \sqrt{\frac{12}{0.012}} = \sqrt{1000} = 32 \text{ m}
$$

---

### Spacing Ratio

**If K_B = 25 × K_A:**

$$
\frac{L_B}{L_A} = \sqrt{\frac{K_B}{K_A}} = \sqrt{25} = 5
$$

**Sandy soil can have 5× spacing of clay!**

---

## 📊 Comparison Tables

### Drain Spacing vs K

| K (m/day) | Spacing (m) | Soil Type |
|-----------|-------------|-----------|
| 0.02 | 10-15 | Heavy clay |
| 0.10 | 20-25 | Clay loam |
| 0.30 | 30-35 | Loam |
| 1.0 | 40-50 | Sandy loam |
| 5.0 | 60-80 | Sand |

**Pattern: Higher K → Wider spacing**

---

### Drain Depth Effects

| Depth (m) | Relative Spacing |
|-----------|------------------|
| 0.8 | 1.0× (baseline) |
| 1.0 | 1.2× |
| **1.2** | **1.4×** ⭐ |
| 1.5 | 1.6× |
| 2.0 | 1.8× |

**Deeper drains → Wider spacing OK**

---

### Drain Diameter Selection

| Area (ha) | Diameter (mm) |
|-----------|---------------|
| <5 | **75-100** ⭐ |
| 5-10 | **100-150** ⭐ |
| 10-20 | 150-200 |
| 20-40 | 200-300 |
| >40 | 300-400 |

---

## ⚠️ Common Exam Mistakes

### Mistake 1: K Values
❌ Clay has high K, Sand has low K  
✅ **Clay low (0.01-0.05), Sand high (2-10)**

---

### Mistake 2: Drain Spacing
❌ Clay needs wider spacing  
✅ **Clay needs CLOSER spacing (10-20m)**

---

### Mistake 3: Units in Hooghoudt
❌ Using q in mm/day directly  
✅ **Convert to m/day: q(m/day) = q(mm/day)/1000**

---

### Mistake 4: Drain Depth
❌ 2.5-3.5 m typical  
✅ **1.0-2.0 m typical**

---

### Mistake 5: Minimum Slope
❌ 0.5% minimum  
✅ **0.1-0.2% minimum**

---

### Mistake 6: Simplified Form
❌ Always use simplified Hooghoudt  
✅ **Only when m > 5d**

---

## 🎓 Memory Techniques

### "10-20 Clay Close"
**Heavy clay:** Spacing = **10-20 m** (closest)

---

### "30-60 Sandy Wide"
**Sandy loam:** Spacing = **30-60 m** (wider)

---

### "1-2 Meter Deep"
**Drain depth:** **1.0-2.0 m** standard

---

### "0.2% Slope"
**Minimum slope:** **0.2%** (ideal)

---

### "75 Minimum"
**Drain diameter:** **75 mm** absolute minimum

---

### "10-15 Field"
**Drainage coefficient:** **10-15 mm/day** for field crops

---

### "Clay 0.01-0.05"
**Hydraulic conductivity:** Clay = **0.01-0.05** (very low)

---

### "Sand 2-10"
**Hydraulic conductivity:** Sand = **2-10** (high)

---

### "4K Formula"
**Hooghoudt:** Numerator starts with **4K**

---

## 📋 Pre-Exam Checklist

**Must Remember:**
- [ ] **Hooghoudt:** L = √[4K(2md+d²)/q]
- [ ] **Simplified:** L = √(8Kmd/q) when m>5d
- [ ] **K values:** Clay 0.01-0.05, Sand 2-10
- [ ] **Spacing:** Clay 10-20m, Sandy 30-60m
- [ ] **q values:** Field crops 10-15, Vegetables 15-20
- [ ] **Depth:** 1.0-2.0 m typical
- [ ] **Slope:** 0.1-0.2% minimum
- [ ] **Diameter:** 75 mm minimum
- [ ] **L ∝ √K** (proportional relationship)
- [ ] **Convert q to m/day** before calculation

---

## 🔥 High-Yield Topics

**Must Know (Every Year):**
1. ✓ Hooghoudt equation application ⭐⭐⭐
2. ✓ K values by soil type ⭐⭐⭐
3. ✓ Drain spacing by soil ⭐⭐⭐
4. ✓ Drainage coefficient values ⭐⭐
5. ✓ Typical specifications ⭐⭐

**Moderate Priority:**
- Simplified Hooghoudt
- Drain depth/diameter
- Slope requirements
- Spacing relationships

**Lower Priority:**
- Installation details
- Material properties
- Envelope design

---

## 💡 Last-Minute Tips

**If short on time, FOCUS ON:**
1. ✓ Hooghoudt formula (know it cold!)
2. ✓ K values: Clay 0.01-0.05, Sand 2-10
3. ✓ Spacing: Clay 10-20m, Sandy 30-60m
4. ✓ q = 10-15 mm/day for field crops
5. ✓ Depth 1-2m, Slope 0.2%, Diameter 75mm min

**Can skip:**
- Detailed derivations
- Complex junction design
- Historical methods

---

## 🎯 Final Formula Card

**Top 3 - Commit to Memory:**

$$
\boxed{L = \sqrt{\frac{4K(2md + d^2)}{q}}}
$$

$$
\boxed{L = \sqrt{\frac{8Kmd}{q}} \quad \text{(when m>5d)}}
$$

$$
\boxed{L \propto \sqrt{K}}
$$

---

## 📱 Quick Reference Card

**Write on exam rough sheet:**

```
HOOGHOUDT: L = √[4K(2md+d²)/q]
SIMPLIFIED: L = √(8Kmd/q) if m>5d

K VALUES:
  Clay: 0.01-0.05 → Spacing 10-20m
  Sand: 2-10     → Spacing 30-60m

q: 10-15 mm/day (field crops)

SPECS:
  Depth: 1-2m
  Slope: 0.2% min
  Diameter: 75mm min

CONVERT: q(m/day) = q(mm/day)/1000
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

*Drain smart, grow better! 🌊*

💧 **Remove Excess, Retain Success!** 🏆
