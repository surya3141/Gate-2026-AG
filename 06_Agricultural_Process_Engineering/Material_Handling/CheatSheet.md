# 🚜 Material Handling - CheatSheet

> **Quick Reference for GATE 2026**

---

## 🔥 Critical Formulas (MUST MEMORIZE)

### Belt Conveyor Capacity
```
Q = 3.6 × A × v × ρ  (tonnes/hr)

A = cross-sectional area (m²)
v = belt velocity (m/s)
ρ = bulk density (t/m³)
```

### Screw Conveyor Capacity
```
Q = (π/4) × D² × p × N × η  (m³/hr)

D = diameter (m)
p = pitch (m)
N = speed (rpm)
η = efficiency (0.30-0.40)
```

### Belt Power (Horizontal)
```
P = (Q × L × f × g) / 3600  (kW)

Q = capacity (t/hr)
L = length (m)
f = friction (~0.03)
```

### Angle of Surcharge
```
θ_surcharge = θ_repose - (5° to 10°)
```

---

## 📋 Must-Know Values

### Belt Conveyor

**Typical velocities (m/s):**
- Fine powder: 0.8-1.5
- Grain: 1.5-2.5
- Coarse: 2.0-3.5

**Friction coefficient:** 0.02-0.04 (typically **0.03**)

**Angle of surcharge:** 5-10° less than repose
- Wheat: θr = 28° → θs ≈ **20°**

### Screw Conveyor

**Loading efficiency (η):** 
- Free-flowing: 0.40-0.45
- Average: **0.30-0.35** ← Most common
- Sticky: 0.15-0.25

**Never more than 45%!** (material needs space to tumble)

**Standard pitch:** p = D (pitch equals diameter)

### Bucket Elevator

**Speed:**
- Centrifugal: 100-150 m/min (fast)
- Continuous: 30-60 m/min (slow)

**Best for:** **Vertical transport** (THE key point)

### Pneumatic Conveying 🔥

**Air velocity:**
- **Dilute phase:** **15-30 m/s** ← MOST ASKED
- Dense phase: 3-10 m/s

**Solid:air ratio:**
- Dilute: < 15
- Dense: > 15

---

## 🎯 Quick Calculation Steps

### Problem Type 1: Belt Capacity (1 minute)

**Given:** A = 0.02 m², v = 1.5 m/s, ρ = 800 kg/m³ = 0.8 t/m³

**Steps:**
1. Write: Q = 3.6 × A × v × ρ
2. Substitute: = 3.6 × 0.02 × 1.5 × 0.8
3. Calculate: = 3.6 × 0.024 = 0.0864
4. Convert: = 0.0864 t/min = **86.4 t/hr**

**Key:** Factor 3.6 converts m³/s to t/hr (with density)

### Problem Type 2: Belt Power (1-2 minutes)

**Given:** Q = 100 t/hr, L = 50 m, f = 0.03, horizontal

**Steps:**
1. Write: P = (Q × L × f × g) / 3600
2. g = 10 m/s² (approximation)
3. Calculate: = (100 × 50 × 0.03 × 10) / 3600
4. = 1500 / 3600 = **0.417 kW**

### Problem Type 3: Screw Capacity (2 minutes)

**Given:** D = 150 mm = 0.15 m, p = 200 mm = 0.2 m, N = 60 rpm, η = 0.40

**Steps:**
1. Write: Q = (π/4) × D² × p × N × η
2. Calculate D²: = 0.15² = 0.0225 m²
3. Calculate: = (3.14/4) × 0.0225 × 0.2 × 60 × 0.40
4. = 0.785 × 0.0225 × 0.2 × 60 × 0.40
5. = 0.785 × 0.108 = **0.0848 m³/min**
6. Or: × 60 = **5.09 m³/hr**

### Problem Type 4: Equipment Selection (15 seconds)

**Question:** "For vertical transport?"
**Answer:** **Bucket elevator**

**Question:** "Most versatile, general purpose?"
**Answer:** **Belt conveyor**

**Question:** "Enclosed, horizontal, short distance?"
**Answer:** **Screw conveyor**

### Problem Type 5: Pneumatic Velocity (15 seconds)

**Question:** "Typical air velocity in dilute phase pneumatic conveying?"
**Answer:** **15-30 m/s**

---

## 💡 Memory Techniques

### 1. "3.6 for Belt"
**Belt capacity** formula has factor **3.6**
- Q = **3.6** × A × v × ρ
- Converts volume flow to mass flow per hour

### 2. "Screw 30-40"
**Screw efficiency:** **30-40%** (0.30-0.40)
- Can't be higher (material needs space)
- Free-flowing max 45%, average 30-35%
- "Screw is **30-40** efficient"

### 3. "Bucket Goes Up"
**Bucket elevator** = **Vertical** transport
- Name says it! "Elevator" goes UP
- Best for lifting grains
- Not for horizontal

### 4. "15-30 for Air"
**Pneumatic dilute phase:** **15-30 m/s**
- High velocity (material suspended)
- Lower than 15 → settling (saltation)
- "**15 to 30** for air to fly"

### 5. "Surcharge 5-10 Less"
**Angle of surcharge** = Repose - (5 to 10)°
- Moving belt → less stable than static pile
- Vibration reduces angle
- "Surcharge **5-10 less**"

### 6. "Q-A-V-Rho" (Belt)
**Belt capacity** components:
- **Q** (capacity) = A × v × ρ (with 3.6 factor)
- **A**rea × **V**elocity × **Rho**(density)
- "Q from A-V-Rho"

---

## ⚠️ Common Mistakes

### Mistake 1: Belt capacity units
❌ **Wrong:** Using wrong density units (kg vs t)
✅ **Correct:** ρ in **t/m³** (tonnes per cubic meter), or divide by 1000

### Mistake 2: Screw efficiency
❌ **Wrong:** Using η = 1.0 or η = 0.8
✅ **Correct:** η = **0.30-0.40** (never >0.45 for screws)

### Mistake 3: Vertical transport selection
❌ **Wrong:** Choosing belt or screw for vertical lift
✅ **Correct:** **Bucket elevator** for vertical transport

### Mistake 4: Pneumatic velocity
❌ **Wrong:** 5-10 m/s for dilute phase
✅ **Correct:** **15-30 m/s** for dilute (high velocity!)

### Mistake 5: Angle of surcharge
❌ **Wrong:** Surcharge angle > repose angle
✅ **Correct:** Surcharge **less** than repose (by 5-10°)

---

## 🎯 Pre-Exam Checklist

### Formulas to Write First:
```
1. Belt: Q = 3.6 × A × v × ρ
2. Screw: Q = (π/4) × D² × p × N × η
3. Belt power: P = Q×L×f×g / 3600
4. Surcharge: θs = θr - (5 to 10)°
```

### Values to Memorize:
- **Belt velocity:** 1.5-2.5 m/s (grain)
- **Screw efficiency:** 0.30-0.40 (standard)
- **Pneumatic dilute:** 15-30 m/s
- **Friction (belt):** ~0.03
- **Bucket elevator:** Vertical transport

### Equipment Selection Table:
| Need | Equipment |
|------|-----------|
| Horizontal, long, high capacity | Belt |
| Horizontal, short, enclosed | Screw |
| **Vertical** | **Bucket elevator** |
| Any angle, flexible | Pneumatic |

### Quick Checks:
- ✅ Belt: Factor 3.6 in formula
- ✅ Screw: Efficiency 0.3-0.4 (low!)
- ✅ Vertical → Bucket elevator (always)
- ✅ Pneumatic: 15-30 m/s dilute phase
- ✅ Surcharge angle < repose angle

---

## 📊 Exam Strategy

### Time Allocation:
- **Equipment selection:** 15 seconds
- **Belt capacity (given A):** 1 minute
- **Screw capacity:** 2 minutes
- **Belt power:** 1-2 minutes
- **Pneumatic velocity:** 15 seconds
- **Surcharge angle:** 30 seconds

### Priority Topics:
1. 🔥🔥🔥 **Belt capacity formula** (Q = 3.6Avρ)
2. 🔥🔥 **Equipment selection** (Bucket = vertical!)
3. 🔥🔥 **Pneumatic velocity** (15-30 m/s)
4. 🔥 **Screw efficiency** (0.3-0.4)
5. **Surcharge angle** (5-10° less)
6. **Belt power**

### If Short on Time:
1. Belt: Q = 3.6 × A × v × ρ
2. Screw: η = 0.3-0.4
3. Bucket elevator = vertical
4. Pneumatic = 15-30 m/s
5. Surcharge 5-10° less than repose

---

## 🚀 Last-Minute Tips

### Write on entry:
```
Belt: Q = 3.6×A×v×ρ
Screw: Q = (π/4)D²pNη, η=0.3-0.4
Bucket: Vertical transport
Pneumatic: 15-30 m/s (dilute)
Surcharge = Repose - (5-10°)
```

### Mental checklist:
- [ ] Belt formula with 3.6 clear?
- [ ] Screw efficiency 0.3-0.4?
- [ ] Bucket elevator = vertical?
- [ ] Pneumatic velocity 15-30 m/s?
- [ ] Equipment selection criteria?

### During exam:
1. **Belt capacity:** Always use 3.6 factor, check density units
2. **Screw:** Efficiency MUST be 0.3-0.4 (never 1.0!)
3. **Vertical transport:** ALWAYS bucket elevator
4. **Pneumatic:** Dilute phase = 15-30 m/s (high!)
5. **Surcharge:** Always LESS than repose angle

### Common question patterns:
- "Belt capacity with A, v, ρ given?" → **Q = 3.6Avρ**
- "Screw loading efficiency?" → **0.30-0.40**
- "For vertical transport?" → **Bucket elevator**
- "Dilute phase pneumatic velocity?" → **15-30 m/s**
- "Angle of surcharge vs repose?" → **5-10° less**
- "Belt power horizontal?" → **P = QLfg/3600**

### Calculation tips:
- **Belt:** 3.6 is KEY factor (don't forget!)
- **Screw:** η around **0.35** if not specified
- **Power:** g = 10 m/s² (approximation OK)
- **Units:** Watch t vs kg, m vs mm

---

*[Theory](./README.md) | [Solutions](./Solutions.md) | [Section Home](../README.md)*
