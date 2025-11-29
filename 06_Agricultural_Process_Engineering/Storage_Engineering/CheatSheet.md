# 🏪 Storage Engineering - CheatSheet

> **Quick Reference for GATE 2026**

---

## 🔥 Critical Formulas (MUST MEMORIZE)

### Janssen's Equation (Most Important!)
```
Pv = (γR / kμ) × [1 - exp(-kμh / R)]

Ph = k × Pv

At large depth: Pv,max = γR / (kμ)
```

### Hydraulic Radius
```
Cylinder: R = D / 4
Square:   R = Side / 4
```

### Aeration
```
Q = m × q  (m³/min)
Standard rate: 0.01-0.02 m³/(min·tonne)
```

---

## 📋 Must-Know Values

### Bulk Density (kg/m³) 🔥

| Grain | Density | Memory |
|-------|---------|--------|
| **Paddy** | **550-600** | Lightest (husk) |
| Maize | 700-750 | Medium |
| **Wheat** | **750-800** | Standard |
| Rice | 800-850 | Heaviest |

**Quick:** Paddy 550-600, Wheat 750-800 (most asked)

### Angle of Repose (°) 🔥

| Grain | Angle | Flowability |
|-------|-------|-------------|
| **Wheat** | **25-30** | Good |
| **Paddy** | **30-35** | Fair |
| Maize | 25-30 | Good |
| Rice | 30-35 | Fair |

**Quick:** Wheat ~28°, Paddy ~32°

### Janssen Parameters

**Lateral pressure ratio (k):** 0.3-0.6 (typical **0.4**)
**Friction coefficient (μ):** 0.25-0.40 (typical **0.3**)

### Aeration Rate 🔥

| Purpose | Rate (m³/min/tonne) |
|---------|---------------------|
| **Maintenance** | **0.01-0.02** ← MOST COMMON |
| Cooling | 0.02-0.05 |
| Emergency | 0.05-0.10 |

### CAS (Controlled Atmosphere Storage) 🔥

- **O₂:** 2-5% (reduced from 21%)
- **CO₂:** 10-20% (increased from 0.03%)
- **Effect:** Low O₂ + High CO₂

**Memory:** "Low O₂, High CO₂" kills insects

---

## 🎯 Quick Calculation Steps

### Problem Type 1: Bulk Density Recognition (15 sec)

**Question:** "Typical bulk density of wheat?"

**Answer:** **750-800 kg/m³**

**Quick check:** Paddy lighter (~600), Rice heavier (~850)

### Problem Type 2: Janssen's Equation (3-4 min)

**Given:** D = 4 m cylinder, h = 10 m, γ = 8 kN/m³, k = 0.4, μ = 0.3

**Steps:**

1. **Hydraulic radius:** R = D/4 = 4/4 = **1 m**

2. **Calculate exponent:**
   ```
   kμh/R = (0.4 × 0.3 × 10) / 1 = 1.2
   exp(-1.2) = 0.301
   1 - exp(-1.2) = 0.699
   ```

3. **Calculate coefficient:**
   ```
   γR/(kμ) = (8 × 1) / (0.4 × 0.3) = 8/0.12 = 66.7 kPa
   ```

4. **Vertical pressure:**
   ```
   Pv = 66.7 × 0.699 = 46.6 kPa
   ```

5. **Lateral pressure:**
   ```
   Ph = k × Pv = 0.4 × 46.6 = 18.6 kPa
   ```

### Problem Type 3: Lateral Pressure (30 sec)

**Given:** Pv = 50 kPa, k = 0.4

**Steps:**
1. Write: Ph = k × Pv
2. Calculate: = 0.4 × 50 = **20 kPa**

### Problem Type 4: Aeration Rate (30 sec)

**Question:** "Recommended aeration rate?"

**Answer:** **0.01-0.02 m³/(min·tonne)**

### Problem Type 5: CAS Composition (15 sec)

**Question:** "In CAS, O₂ and CO₂ levels?"

**Answer:** **O₂: Low (2-5%), CO₂: High (10-20%)**

---

## 💡 Memory Techniques

### 1. "Paddy Light, Rice Heavy"
**Bulk density:**
- **Paddy** (with husk): **~600** kg/m³ (lighter)
- **Rice** (without husk): **~850** kg/m³ (heavier)
- **Wheat**: **~750** (in between)

### 2. "Wheat 28, Paddy 32" (Angle)
**Angle of repose:**
- Wheat: ~**28°** (rounder, flows better)
- Paddy: ~**32°** (elongated, less flowable)

### 3. "R = D/4" (for cylinder)
**Hydraulic radius** = Quarter of diameter
- Easy to remember: **R-adius = D/4**

### 4. "0.01 to 0.02 to Maintain" (Aeration)
**Maintenance aeration:** **0.01-0.02** m³/(min·t)
- Most common question answer
- Not for drying! (too low airflow)

### 5. "Low O₂, High CO₂" (CAS)
**Controlled Atmosphere:**
- **O₂ ↓** to 2-5% (one-tenth of normal)
- **CO₂ ↑** to 10-20% (hundreds times normal)
- Kills insects without chemicals

### 6. "Janssen Plateau"
At large depth, pressure **plateaus** (doesn't increase linearly)
- Due to wall friction
- Pv,max = γR/(kμ)

### 7. "k for Kick, μ for Move"
- **k** (lateral ratio): How much pressure **kicks** sideways (0.3-0.6)
- **μ** (friction): How hard to **move** grain on wall (0.25-0.40)

---

## ⚠️ Common Mistakes

### Mistake 1: Confusing bin and silo
❌ **Wrong:** Bin H/D > 2, Silo H/D < 2
✅ **Correct:** **Bin H/D < 2** (squat), **Silo H/D > 2** (tall)

### Mistake 2: Linear pressure assumption
❌ **Wrong:** Pv = γh (hydrostatic, linear)
✅ **Correct:** Janssen's equation (plateaus due to wall friction)

### Mistake 3: Aeration for drying
❌ **Wrong:** Aeration rate 0.01-0.02 m³/(min·t) can dry grain
✅ **Correct:** This is for **cooling/maintenance** only, NOT drying (too low)

### Mistake 4: CAS composition
❌ **Wrong:** CAS has high O₂ and low CO₂
✅ **Correct:** **Low O₂ (2-5%), High CO₂ (10-20%)**

### Mistake 5: Bulk density order
❌ **Wrong:** Rice lighter than paddy
✅ **Correct:** **Paddy** (with husk) **lighter** (~600), **Rice** (no husk) **heavier** (~850)

---

## 🎯 Pre-Exam Checklist

### Formulas to Write First:
```
1. Pv = (γR/kμ) × [1-exp(-kμh/R)]
2. Ph = k × Pv
3. R = D/4 (cylinder)
4. Q = m × q (aeration)
```

### Values to Memorize:
- **Bulk density:** Paddy 550-600, Wheat 750-800 kg/m³
- **Angle:** Wheat 25-30°, Paddy 30-35°
- **k:** ~0.4, **μ:** ~0.3
- **Aeration:** 0.01-0.02 m³/(min·t)
- **CAS:** O₂ 2-5%, CO₂ 10-20%

### Quick Checks:
- ✅ Janssen: Pressure plateaus (not linear)
- ✅ Lateral Ph = k × Pv (k always <1)
- ✅ Bulk density: Rice > Wheat > Paddy
- ✅ Angle: Paddy > Wheat (worse flow)
- ✅ CAS: Low O₂, High CO₂

---

## 📊 Exam Strategy

### Time Allocation:
- **Bulk density value:** 15 seconds
- **Angle of repose:** 15 seconds
- **Lateral pressure (Ph=kPv):** 30 seconds
- **Aeration rate:** 15 seconds
- **CAS composition:** 15 seconds
- **Janssen's full calculation:** 3-4 minutes

### Priority Topics:
1. 🔥🔥🔥 **Janssen's equation** (complex but frequent)
2. 🔥🔥 **Bulk density values** (easy marks)
3. 🔥🔥 **Aeration rate** (0.01-0.02)
4. 🔥 **CAS concept** (Low O₂, High CO₂)
5. **Angle of repose**
6. **Bin vs silo**

### If Short on Time:
1. Memorize bulk densities (Paddy 600, Wheat 750)
2. Aeration rate: 0.01-0.02
3. CAS: Low O₂, High CO₂
4. Ph = k × Pv
5. R = D/4

---

## 🚀 Last-Minute Tips

### Write on entry:
```
Pv = (γR/kμ)[1-exp(-kμh/R)], Ph=kPv, R=D/4
Paddy 600, Wheat 750 kg/m³
Angle: Wheat 28°, Paddy 32°
Aeration: 0.01-0.02 m³/(min·t)
CAS: Low O₂ (2-5%), High CO₂ (10-20%)
```

### Mental checklist:
- [ ] Janssen's equation ready?
- [ ] Bulk densities memorized?
- [ ] Aeration rate known?
- [ ] CAS composition clear?
- [ ] R = D/4 for cylinder?

### During exam:
1. **Janssen:** Write full equation first, then substitute step-by-step
2. **Bulk density:** Paddy lightest (~600), Rice heaviest (~850)
3. **Aeration:** 0.01-0.02 is "maintenance" not drying
4. **CAS:** Always "Low O₂, High CO₂" together
5. **Lateral pressure:** Always Ph = k × Pv (simple!)

### Common question patterns:
- "Bulk density of wheat?" → **750-800 kg/m³**
- "Aeration rate for storage?" → **0.01-0.02 m³/(min·t)**
- "CAS gas composition?" → **Low O₂ (2-5%), High CO₂ (10-20%)**
- "Calculate lateral pressure (Pv given)?" → **Ph = k × Pv**
- "Major storage loss cause in India?" → **Insects/pests**

---

*[Theory](./README.md) | [Solutions](./Solutions.md) | [Section Home](../README.md)*
