# 💦 Irrigation Methods - CheatSheet

> **Quick Reference for GATE Exam**

---

## 🔥 Critical Formulas

### Sprinkler Irrigation ⭐⭐⭐

**1. Spacing (No Wind)**
$$
\boxed{S_L = S_s = 0.65D}
$$

**2. Spacing (Moderate Wind)**
$$
\boxed{S_L = 0.50D, \quad S_s = 0.65D}
$$

**3. Application Rate**
$$
\boxed{I = \frac{Q \times 1000}{S_L \times S_s}}
$$
(Q in L/s, I in mm/hr)

**4. Operating Time**
$$
\boxed{t = \frac{d}{I}}
$$

**5. Christiansen's Uniformity**
$$
\boxed{CU = 100 \times \left(1 - \frac{\sum |X - \overline{X}|}{n \times \overline{X}}\right)}
$$

---

### Drip Irrigation ⭐⭐

**1. Emitter Equation**
$$
\boxed{q = K \times H^x}
$$

**2. System Capacity**
$$
\boxed{Q = \frac{N \times q}{3600}}
$$
(q in L/hr, Q in L/s)

**3. Emission Uniformity**
$$
\boxed{EU = 100 \times \frac{q_{min}}{q_{avg}}}
$$

---

### Surface Irrigation ⭐

**Application Efficiency**
$$
\boxed{E_a = \frac{W_s}{W_d} \times 100}
$$

---

## 📊 Must-Memorize Values

### Efficiency Comparison 🔥

| Method | Efficiency (%) | Memory Tip |
|--------|----------------|------------|
| **Drip** 💧 | **85-95** | **"90% = Best!"** 🔥 |
| **Sprinkler** 💨 | **65-85** | **"75% = Good"** 🔥 |
| **Surface** 🌊 | **40-60** | **"50% = Half"** 🔥 |

**Order:** Drip > Sprinkler > Surface  
**Quick:** 90% > 75% > 50%

---

### Sprinkler System Values

| Parameter | Value | Memory |
|-----------|-------|--------|
| **Spacing factor (no wind)** | **0.65D** | **"65% of diameter"** 🔥 |
| Spacing factor (wind - along) | 0.50D | "Half diameter" |
| Spacing factor (wind - between) | 0.65D | Same as no wind |
| **Operating pressure** | **200-300 kPa** | "2-3 bar typical" |
| Wetted diameter | 15-30 m | Medium size |
| **Uniformity (CU) excellent** | **>85%** | "Above 85 is great!" 🔥 |
| CU good | 75-85% | Acceptable |
| Application rate | 5-20 mm/hr | Depends on spacing |

---

### Drip System Values

| Parameter | Value | Memory |
|-----------|-------|--------|
| **Standard emitter** | **4 L/hr** | **"4 is magic!"** 🔥 |
| Emitter range | 2-8 L/hr | Standard drippers |
| **Operating pressure** | **100 kPa** | **"1.0 bar"** 🔥 |
| Pressure range | 50-150 kPa | 0.5-1.5 bar |
| **Emission uniformity (EU)** | **>90%** | "Above 90 excellent" 🔥 |
| Filter mesh | 120-150 | "150 mesh standard" |
| Wetted diameter | 30-100 cm | For 4 L/hr ~50 cm |

---

### Surface Irrigation Values

| Parameter | Border | Furrow | Basin |
|-----------|--------|--------|-------|
| **Optimum slope** | 0.2-0.5% | **0.2-0.5%** 🔥 | <0.2% |
| Maximum slope | 1.0% | 2.0% | - |
| Width | 10-15 m | - | - |
| Length | 100-200 m | 100-400 m | - |
| Discharge | 1-3 L/s/m | 0.5-3 L/s | - |
| Efficiency | 50-70% | 50-75% | 40-60% |

**Key:** Furrow optimum slope = **0.2-0.5%**

---

## 🎯 Quick Calculation Steps

### Type 1: Sprinkler Spacing

**Given:** Wetted diameter (D), wind condition  
**Find:** Spacing

**Steps:**
1. If **no wind:** S = 0.65D (both directions)
2. If **moderate wind:** SL = 0.50D, Ss = 0.65D

**Example:** D = 20 m, no wind  
→ S = 0.65 × 20 = **13 m × 13 m**

---

### Type 2: Application Rate

**Given:** Discharge (Q in L/s), Spacing (SL × Ss in m)  
**Find:** Application rate (I in mm/hr)

**Steps:**
1. Multiply Q by 1000
2. Divide by (SL × Ss)

**Formula:** I = Q × 1000 / (SL × Ss)

**Example:** Q = 1.2 L/s, spacing 12m × 15m  
→ I = 1.2 × 1000 / (12 × 15) = 1200 / 180 = **6.67 mm/hr**

---

### Type 3: Operating Time

**Given:** Depth (d in mm), Application rate (I in mm/hr)  
**Find:** Time (t in hr)

**Steps:**
1. Divide depth by rate

**Formula:** t = d / I

**Example:** d = 60 mm, I = 8 mm/hr  
→ t = 60 / 8 = **7.5 hours**

---

### Type 4: Drip System Capacity

**Given:** Number of emitters (N), Discharge per emitter (q in L/hr)  
**Find:** System capacity (Q in L/s)

**Steps:**
1. Multiply N × q (gives L/hr)
2. Divide by 3600 (converts to L/s)

**Formula:** Q = (N × q) / 3600

**Example:** 1000 emitters, 4 L/hr each  
→ Q = (1000 × 4) / 3600 = 4000 / 3600 = **1.11 L/s**

---

### Type 5: Daily Water Volume

**Given:** System capacity (Q), Operating hours (t)  
**Find:** Daily volume (m³)

**Steps:**
1. If Q in L/s: V = Q × t × 3600 / 1000
2. If Q in L/hr: V = Q × t / 1000

**Example:** Q = 4000 L/hr, t = 8 hr  
→ V = 4000 × 8 / 1000 = **32 m³**

---

### Type 6: Christiansen's CU

**Given:** Catch can data  
**Find:** CU (%)

**Steps:**
1. Calculate mean: X̄ = ΣX / n
2. Calculate deviations: |X - X̄| for each
3. Sum deviations: Σ|X - X̄|
4. Apply formula: CU = 100 × (1 - Σ|X - X̄| / (n × X̄))

**Example:** Data: 10, 12, 11, 13, 12 (n=5)  
→ X̄ = 58/5 = 11.6  
→ |deviations|: 1.6, 0.4, 0.6, 1.4, 0.4 → Sum = 4.4  
→ CU = 100 × (1 - 4.4/(5×11.6)) = 100 × (1 - 0.076) = **92.4%**

---

## 💡 Memory Techniques

### "90-75-50 Rule"

Efficiency progression:
- **Drip = 90%** (nine-tenth)
- **Sprinkler = 75%** (three-quarter)
- **Surface = 50%** (half)

**Chant:** "Ninety, seventy-five, fifty - Drip, Sprinkle, Surface!"

---

### "0.65D Spacing"

For sprinkler **no wind:**
- **Both directions = 0.65D**

**Memory:** "65 cents for both directions"

---

### "4 L/hr Standard"

**Most common emitter = 4 L/hr**

**Memory:** "Four drops fall for an hour"

---

### "Point-Two to Point-Five"

**Furrow optimum slope = 0.2-0.5%**

**Memory:** "0.2 to 0.5, furrow stays alive!"

---

### "85 for Excellence"

**CU > 85% = Excellent uniformity**

**Memory:** "85 to thrive, excellence arrives!"

---

## 📊 Comparison Tables

### Method Selection Guide

| Condition | Best Method | Reason |
|-----------|-------------|--------|
| **Water scarce** | Drip | Highest efficiency (90%) |
| **Undulating land** | Sprinkler/Drip | No leveling needed |
| **Rice (paddy)** | Basin | Flooding required |
| **Row crops** | Furrow/Drip | Between rows |
| **Sandy soil** | Sprinkler | High infiltration |
| **Heavy soil** | Surface | Slow infiltration |
| **High-value crops** | Drip | Precise control |
| **Large areas (level)** | Border | Cost-effective |
| **Wind-free area** | Sprinkler | Good uniformity |
| **Saline water** | Drip | Salt pushed away |

---

### Cost Comparison

| Method | Initial Cost | Operating Cost | Total |
|--------|--------------|----------------|-------|
| **Surface** | Low | Low | Cheapest |
| **Sprinkler** | High | Moderate | Medium |
| **Drip** | Very High | Moderate | Expensive |

---

### Crop Suitability

| Crop Type | Surface | Sprinkler | Drip |
|-----------|---------|-----------|------|
| **Rice** | ✅ Best | ❌ | ❌ |
| **Wheat** | ✅ Good | ✅ Good | - |
| **Cotton** | ✅ Furrow | ✅ | ✅ Best |
| **Vegetables** | - | ✅ Good | ✅ Best |
| **Fruit trees** | - | ✅ | ✅ Best |
| **Sugarcane** | ✅ Furrow | - | ✅ |
| **Lawns** | - | ✅ Best | - |

---

## ⚠️ Common Mistakes

### Mistake 1: Spacing Confusion

❌ **Wrong:** Using 0.65D for wind conditions  
✅ **Right:** 0.50D (along) × 0.65D (between) for wind

---

### Mistake 2: Unit Errors in Application Rate

❌ **Wrong:** I = Q / (SL × Ss) [missing 1000 factor]  
✅ **Right:** I = Q × 1000 / (SL × Ss)  
[Q in L/s, I in mm/hr]

---

### Mistake 3: Drip Capacity Calculation

❌ **Wrong:** Q = N × q (in L/hr, should be L/s)  
✅ **Right:** Q = (N × q) / 3600  
[Convert L/hr to L/s]

---

### Mistake 4: CU Absolute Values

❌ **Wrong:** Using X - X̄ (can be negative)  
✅ **Right:** Using |X - X̄| (always positive)

---

### Mistake 5: Efficiency vs Uniformity

❌ **Wrong:** Confusing Ea (efficiency) with CU (uniformity)  
✅ **Right:** Ea = water stored/delivered, CU = distribution pattern

---

## 📝 Pre-Exam Quick Check

### 30 Seconds Before Exam

**Memorize:**

1. **Efficiency: 90%, 75%, 50%** (Drip, Sprinkler, Surface)
2. **Spacing: 0.65D** (no wind)
3. **Emitter: 4 L/hr** (standard)
4. **Furrow slope: 0.2-0.5%** (optimum)
5. **CU excellent: >85%**
6. **Drip pressure: 100 kPa**

---

### 5-Minute Formula Review

**Write on rough paper:**

$$
S = 0.65D
$$

$$
I = \frac{Q \times 1000}{S_L \times S_s}
$$

$$
t = \frac{d}{I}
$$

$$
Q = \frac{N \times q}{3600}
$$

$$
CU = 100 \times \left(1 - \frac{\sum |X - \overline{X}|}{n \times \overline{X}}\right)
$$

---

## 🎯 GATE Success Strategy

### High-Yield Topics

1. ⭐⭐⭐ **Efficiency comparison** (easiest marks!)
2. ⭐⭐⭐ **Sprinkler spacing** (direct formula)
3. ⭐⭐⭐ **Application rate** (common calculation)
4. ⭐⭐ **Drip discharge** (value recall)
5. ⭐⭐ **Method selection** (conceptual)

### Expected GATE Questions

- Efficiency comparison: 1 question (2 marks)
- Sprinkler calculations: 2 questions (4-5 marks)
- Drip system: 1 question (2 marks)
- CU calculation: 0-1 question (2 marks)
- Method suitability: 1 question (1-2 marks)

**Total expected:** 4-5 questions, 8-12 marks

---

## ✅ Final Checklist

Before exam, confirm you can:

- [ ] Compare efficiencies (Drip > Sprinkler > Surface)
- [ ] Calculate sprinkler spacing (0.65D rule)
- [ ] Find application rate from Q and spacing
- [ ] Determine operating time (t = d/I)
- [ ] Calculate drip system capacity
- [ ] Compute Christiansen's CU
- [ ] Select method for given crop/condition
- [ ] Identify furrow optimum slope (0.2-0.5%)
- [ ] Know standard emitter discharge (4 L/hr)
- [ ] Understand uniformity threshold (85%)

**Target:** 10/10 = Ready!

---

## 🚀 Quick Revision (3 Minutes)

**Repeat aloud:**

"Drip **90**, Sprinkler **75**, Surface **50** - efficiency flow!  
Spacing **0.65D** when no wind blow.  
Four L per hour, drip standard power.  
Furrow slope **point-two to five**, keeps uniformity alive.  
CU above **eighty-five**, excellent system will thrive!"

---

## 💯 Score Booster Tips

### Easy 2-Markers (Don't Miss!)

1. **Efficiency comparison** → Drip highest
2. **Standard emitter** → 4 L/hr
3. **Spacing factor** → 0.65D
4. **Rice irrigation** → Basin
5. **Furrow slope** → 0.2-0.5%

**Aim for 100% on these!**

---

### Calculation Safety

1. **Check units:** L/s vs L/hr
2. **Watch factors:** 1000 for mm/hr, 3600 for L/s conversion
3. **Spacing:** Along vs between for wind
4. **CU:** Use absolute values |X - X̄|
5. **Verify magnitude:** CU should be 75-95%, not 7.5 or 9500!

---

### Time Management

- **Value recall:** 30 sec (efficiency, spacing factor)
- **Direct formula:** 1-2 min (spacing, operating time)
- **Multi-step calc:** 3-4 min (application rate, system capacity)
- **CU calculation:** 4-5 min (if data given)

**Total time budget:** 10-15 minutes for irrigation methods section

---

**Print → Laminate → Revise daily for 1 week = GATE ready!**

---

*[Back to Solutions](./Solutions.md) | [Theory](./README.md) | [Section Home](../README.md)*
