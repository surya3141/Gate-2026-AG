# 🌱 Crop Water Requirements - CheatSheet

> **Quick Reference for GATE Exam**

---

## 🔥 Critical Formulas

### 1. Pan Evaporation Method ⭐⭐⭐

$$
\boxed{ET_0 = K_p \times E_{pan}}
$$

**Most important for GATE!**

---

### 2. Crop Evapotranspiration ⭐⭐⭐

$$
\boxed{ET_c = K_c \times ET_0}
$$

---

### 3. Net Irrigation Requirement ⭐⭐

$$
\boxed{IR_{net} = ET_c - P_e - GW - S}
$$

---

### 4. Gross Irrigation Requirement ⭐⭐⭐

$$
\boxed{IR_{gross} = \frac{IR_{net}}{E_a}}
$$

---

### 5. Irrigation Interval ⭐⭐

$$
\boxed{\text{Interval} = \frac{\text{Available water} \times MAD}{ET_c}}
$$

---

### 6. Penman-Monteith (Recognition Only)

$$
ET_0 = \frac{0.408\Delta(R_n - G) + \gamma\frac{900}{T+273}u_2(e_s - e_a)}{\Delta + \gamma(1 + 0.34u_2)}
$$

**Just recognize structure; not for calculation in GATE**

---

## 📊 Must-Memorize Values

### Pan Coefficient (Kp)

| Pan Type & Environment | Kp | Memory Tip |
|------------------------|-----|------------|
| **Class A, green area** | **0.75** | **"3/4 or 0.75"** 🔥 |
| Class A, dry area | 0.65 | Lower by 0.10 |
| Colorado sunken | 0.83 | Highest ~0.83 |

**Default for GATE:** **Kp = 0.75**

---

### Crop Coefficients (Kc) - Mid-Season Peak

| Crop | Kc (Mid) | Memory Tip |
|------|----------|------------|
| **Rice** 🌾 | **1.15-1.20** | **Highest (flooded)** 🔥 |
| **Wheat** 🌾 | **1.10** | **Second highest** 🔥 |
| **Maize** 🌽 | **1.15** | Like rice |
| **Cotton** | **1.15** | High demand |
| Sugarcane | 1.25 | Very high (long season) |
| Potato | 1.10 | Medium-high |
| Vegetables | 1.00-1.05 | Around 1.0 |
| Soybean | 1.00 | Exactly 1.0 |

**Memory:** "Rice needs Nice water" → 1.20 highest

---

### Kc by Growth Stage (Pattern)

| Stage | Duration | Kc Range | Description |
|-------|----------|----------|-------------|
| **Initial** | ~15-20% | **0.3-0.5** | Germination, min Kc |
| **Development** | ~25-30% | **0.5-0.8** | Increasing |
| **Mid-Season** | ~30-40% | **0.8-1.2** | Peak, max Kc 🔥 |
| **Late** | ~15-25% | **0.6-0.9** | Maturity, decreasing |

**Trend:** Low → High → Peak → Medium

---

### Application Efficiency (Ea)

| Irrigation Method | Ea (%) | Ea (decimal) | Memory |
|-------------------|--------|--------------|--------|
| **Surface** (basin, border) | **40-60** | **0.50** | **Half lost** 🔥 |
| **Sprinkler** | **65-85** | **0.75** | **Three-quarter** 🔥 |
| **Drip** (micro) | **85-95** | **0.90** | **Nine-tenth (best)** 🔥 |

**Order:** Surface < Sprinkler < Drip  
**Default values:** 50%, 75%, 90%

---

### Management Allowed Depletion (MAD)

| Crop/Condition | MAD (%) | Memory |
|----------------|---------|--------|
| **General field crops** | **50** | **Default = 50%** 🔥 |
| Shallow-rooted vegetables | 30-40 | Lower (frequent irrigation) |
| Stress-sensitive | 30-40 | Lower is safer |
| Deep-rooted trees | 50-70 | Higher (less frequent) |
| Stress-tolerant | 50-70 | Can deplete more |

**GATE Default:** **MAD = 50% = 0.50**

---

## 📈 Typical ET₀ Ranges

| Climate | ET₀ (mm/day) | Epan (mm/day) | Region Example |
|---------|--------------|---------------|----------------|
| Humid | 3-5 | 4-7 | Coastal, NE India |
| Sub-humid | 4-6 | 6-9 | Central India |
| Semi-arid | 5-8 | 8-12 | Rajasthan |
| Arid | 6-10 | 10-15 | Desert regions |

**Typical GATE values:** ET₀ = 5-7 mm/day

---

## 🧮 Quick Calculation Aids

### Volume Conversions

$$
\boxed{1 \text{ cm on 1 ha} = 100 \text{ m}^3}
$$

**Examples:**
- 10 cm on 2 ha = 10 × 2 × 100 = 2000 m³
- 55 mm on 3.5 ha = 5.5 × 3.5 × 100 = 1925 m³

---

### Depth Conversions

- **1 cm = 10 mm**
- **1 m = 100 cm = 1000 mm**
- **1 ha-m = 10,000 m³**

---

### Efficiency as Decimal

- **50% = 0.50**
- **60% = 0.60**
- **75% = 0.75**
- **90% = 0.90**

**For IRgross:** Divide by decimal (not multiply!)

---

## 🎯 Step-by-Step Problem Solving

### Type 1: Pan Method → ET₀

**Given:** Epan, Kp  
**Find:** ET₀

**Steps:**
1. Identify Kp (if not given, use 0.75)
2. Multiply: **ET₀ = Kp × Epan**

**Example:** Epan = 8 mm/day, Kp = 0.75  
→ ET₀ = 0.75 × 8 = **6 mm/day**

---

### Type 2: ET₀ → ETc

**Given:** ET₀, Kc (or crop + stage)  
**Find:** ETc

**Steps:**
1. Identify Kc from crop/stage (rice = 1.15, wheat = 1.10)
2. Multiply: **ETc = Kc × ET₀**

**Example:** ET₀ = 6 mm/day, rice mid-season  
→ Kc = 1.15  
→ ETc = 1.15 × 6 = **6.9 mm/day**

---

### Type 3: Net → Gross IR

**Given:** IRnet, Ea (or irrigation method)  
**Find:** IRgross

**Steps:**
1. Convert Ea to decimal if in % (50% → 0.50)
2. Divide: **IRgross = IRnet / Ea**

**Example:** IRnet = 50 cm, surface irrigation  
→ Ea = 0.50  
→ IRgross = 50 / 0.50 = **100 cm**

---

### Type 4: Seasonal Requirement

**Given:** Daily ETc, season length  
**Find:** Total water

**Steps:**
1. Multiply: **Total = ETc × Days**
2. Convert units if needed

**Example:** ETc = 6 mm/day, 120 days  
→ Total = 6 × 120 = **720 mm = 72 cm**

---

### Type 5: Irrigation Interval

**Given:** Available water (AW), ETc, MAD  
**Find:** Days between irrigations

**Steps:**
1. Calculate allowable depletion: **AD = AW × MAD**
2. Calculate interval: **Days = AD / ETc**

**Example:** AW = 80 mm, ETc = 6 mm/day, MAD = 50%  
→ AD = 80 × 0.50 = 40 mm  
→ Interval = 40 / 6 = **6.67 days ≈ 7 days**

---

### Type 6: Water Volume

**Given:** Depth (cm or mm), Area (ha)  
**Find:** Volume (m³)

**Steps:**
1. Convert depth to cm
2. Use formula: **V = Depth(cm) × Area(ha) × 100**

**Example:** 55 mm on 3.5 ha  
→ 5.5 cm on 3.5 ha  
→ V = 5.5 × 3.5 × 100 = **1925 m³**

---

## 💡 Memory Techniques

### "PEKEG" Chain

**P**an × **K**p = **E**T₀  
**E**T₀ × **K**c = **E**Tc  
**E**Tc - **P**e = **IR**net  
**IR**net / **E**a = **IR**gross

---

### "0.75 Everywhere"

- Kp for Class A pan = **0.75**
- Sprinkler efficiency ≈ **75%**
- Pan evaporation 75% becomes ET₀

---

### "Rice 1.2, Wheat 1.1"

Peak Kc values:
- Rice = **1.20** (highest)
- Wheat = **1.10**
- Maize = **1.15**
- Others ≈ **1.00**

---

### "Half, Three-quarter, Nine-tenth"

Efficiency (decimal):
- Surface = **0.50** (half)
- Sprinkler = **0.75** (three-quarter)
- Drip = **0.90** (nine-tenth)

---

### "50-50 Rule"

- MAD = **50%** typical
- Effective rainfall = **50-70%** of total
- Surface efficiency = **50%**

---

## ⚠️ Common Mistakes

### Mistake 1: Efficiency Confusion

❌ **Wrong:** IRgross = IRnet × Ea  
✅ **Right:** IRgross = IRnet / Ea

**Remember:** Gross > Net (losses occur), so divide!

---

### Mistake 2: Units Mix-up

❌ **Wrong:** 55 mm on 3.5 ha = 55 × 3.5 × 100 = 19,250 m³  
✅ **Right:** 55 mm = 5.5 cm, then 5.5 × 3.5 × 100 = 1,925 m³

**Remember:** Convert mm to cm first!

---

### Mistake 3: Kc Selection

❌ **Wrong:** Using initial Kc for peak season  
✅ **Right:** Match Kc to growth stage

**Remember:** Mid-season Kc is highest (1.0-1.2)

---

### Mistake 4: MAD Confusion

❌ **Wrong:** Interval = AW / ETc (forgetting MAD)  
✅ **Right:** Interval = (AW × MAD) / ETc

**Remember:** Only MAD fraction can be depleted!

---

### Mistake 5: ET₀ vs ETc

❌ **Wrong:** Using ET₀ as crop requirement  
✅ **Right:** ET₀ is reference, need ETc = Kc × ET₀

**Remember:** ET₀ is grass reference, not crop-specific!

---

## 📝 Pre-Exam Quick Check

### 30 Seconds Before Exam

**Memorize these:**

1. **Kp = 0.75** (Class A pan)
2. **Kc(rice) = 1.15-1.20** (highest)
3. **Ea: 50% (surface), 75% (sprinkler), 90% (drip)**
4. **MAD = 50%** (default)
5. **IRgross = IRnet / Ea** (divide!)
6. **1 cm on 1 ha = 100 m³**

---

### 5-Minute Formula Review

Write these on rough paper:

$$
ET_0 = K_p \times E_{pan}
$$

$$
ET_c = K_c \times ET_0
$$

$$
IR_{gross} = \frac{IR_{net}}{E_a}
$$

$$
\text{Interval} = \frac{AW \times MAD}{ET_c}
$$

$$
V = d(\text{cm}) \times A(\text{ha}) \times 100
$$

---

## 🎯 GATE Success Strategy

### High-Priority Topics (Practice Most)

1. ⭐⭐⭐ **Pan evaporation** → ET₀ calculation
2. ⭐⭐⭐ **Kc values** → Crop/stage identification
3. ⭐⭐⭐ **Efficiency** → Net to Gross IR
4. ⭐⭐ **Irrigation interval** → MAD calculations
5. ⭐⭐ **Water volume** → Unit conversions

### Expected Questions in GATE

- Pan method: 2-3 questions (direct)
- Kc selection: 1-2 questions (conceptual)
- Efficiency: 1-2 questions (calculation)
- Seasonal requirement: 1 question
- Method comparison: 1 question (Penman vs Pan vs Blaney)

**Total expected:** 3-4 marks from crop water requirements

---

## 📊 Value Comparison Table

| Parameter | Low | Medium | High | Very High |
|-----------|-----|--------|------|-----------|
| **ET₀ (mm/day)** | 3-4 | 5-6 | 7-8 | 9-10 |
| **Kc (peak)** | 0.9 | 1.0 | 1.1 | 1.2 |
| **Ea (%)** | 40 | 60 | 75 | 90 |
| **MAD (%)** | 30 | 50 | 70 | - |
| **Kp** | 0.65 | 0.75 | 0.85 | - |

---

## ✅ Final Checklist

Before exam, confirm you can:

- [ ] Calculate ET₀ from pan evaporation
- [ ] Select appropriate Kc for crop/stage
- [ ] Convert net to gross irrigation requirement
- [ ] Calculate irrigation interval with MAD
- [ ] Determine seasonal water requirement
- [ ] Convert between mm, cm, m³, ha
- [ ] Identify Penman-Monteith components
- [ ] Compare different ET methods
- [ ] Calculate water volume per hectare
- [ ] Apply effective rainfall concepts

**Target:** 10/10 checked = Ready for exam!

---

## 🚀 Quick Revision (5 Minutes)

**Repeat 3 times:**

"Kp is **0.75**, multiply with pan.  
Rice Kc is **1.20**, wheat is **1.10**.  
Surface **50%**, sprinkler **75%**, drip **90%**.  
Gross equals net **divided** by Ea.  
MAD is **50%**, that's the rule.  
One cm on one ha is **100 cubic**!"

---

## 💯 Score Booster

**Easy marks (2 marks each):**
- Pan evaporation calculation
- Kc identification
- Efficiency comparison
- Unit conversion

**Aim:** Don't miss these! 100% accuracy target.

---

**Perfect Score Formula:**
1. Know values by heart
2. Watch units carefully
3. Divide for gross (not multiply)
4. Check answer magnitude
5. Practice 20+ problems

---

**Print this page → Keep on desk → Revise daily!**

---

*[Back to Solutions](./Solutions.md) | [Theory](./README.md) | [Section Home](../README.md)*
