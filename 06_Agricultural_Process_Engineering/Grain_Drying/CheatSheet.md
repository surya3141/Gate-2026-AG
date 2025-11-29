# 🌾 Grain Drying - CheatSheet

> **Quick Reference for GATE 2026**

---

## 🔥 Critical Formulas (MUST MEMORIZE)

### 1. Moisture Content Conversions
```
wb to db:  Mdb = Mwb/(100-Mwb) × 100
db to wb:  Mwb = Mdb/(100+Mdb) × 100
```

**Example:** 20% wb → Mdb = 20/80 × 100 = 25% db

**Memory:** "wb smaller denominator (100-M), db bigger denominator (100+M)"

### 2. Drying Rate (Newton's Law)
```
dM/dt = -K(M - Me)

Integrated: MR = exp(-Kt)
where MR = (M-Me)/(M₀-Me)
```

**Rearranged for time:**
```
t = -(1/K) × ln[MR]
```

### 3. Relative Humidity
```
RH = (Pactual / Psaturation) × 100%
```

### 4. Water Removal
```
Wremoved = Mi × (Mwb,i - Mwb,f) / (100 - Mwb,f)
```

---

## 📋 Must-Know Values

### Safe Storage Moisture Content (wb%)

| Grain | Safe MC | Critical MC | Memory Aid |
|-------|---------|-------------|------------|
| **Wheat** | **12-14%** | >15% | "12-14 for wheat indeed" |
| **Paddy** | **12-14%** | >16% | Same as wheat |
| **Rice** | **12-13%** | >14% | Slightly lower |
| **Maize** | **13-15%** | >16% | Bit higher |
| Pulses | 10-12% | >13% | Lower (oily) |
| Oilseeds | 7-9% | >10% | Lowest |

**General rule:** Most cereals 12-14% wb

### Saturation Vapor Pressure (kPa)

| Temp (°C) | Ps (kPa) | Memory |
|-----------|----------|--------|
| 20 | 2.34 | ~2 |
| 25 | 3.17 | ~3 |
| 30 | 4.24 | ~4 |
| 35 | 5.62 | ~5.5 |
| 40 | 7.38 | ~7 |

**Pattern:** Roughly +1 kPa per 5°C

### Dryer Selection

| Dryer | Best For | Capacity | Key Feature |
|-------|----------|----------|-------------|
| **LSU** | **Paddy** | High | Continuous column |
| Tray | Herbs | Very Low | Batch |
| Fluidized | Seeds | Medium | Fast |
| Bin | On-farm | Low | Storage + drying |

**GATE favorite:** LSU for paddy drying

---

## 🎯 Quick Calculation Steps

### Problem Type 1: MC Conversion (30 seconds)

**wb to db:**
1. Write: Mdb = Mwb/(100-Mwb) × 100
2. Substitute: Mdb = 20/(100-20) × 100
3. Calculate: = 20/80 × 100 = **25%**

**db to wb:**
1. Write: Mwb = Mdb/(100+Mdb) × 100
2. Substitute: Mwb = 25/(100+25) × 100
3. Calculate: = 25/125 × 100 = **20%**

### Problem Type 2: Drying Rate (1 minute)

**Given:** K = 0.5 hr⁻¹, M = 18% db, Me = 10% db

**Steps:**
1. Write: Rate = K(M-Me)
2. Substitute: = 0.5 × (18-10)
3. Calculate: = 0.5 × 8 = **4% db/hr**

### Problem Type 3: RH Calculation (30 seconds)

**Given:** Pa = 2.12 kPa, Ps = 4.24 kPa

**Steps:**
1. Write: RH = (Pa/Ps) × 100
2. Substitute: = (2.12/4.24) × 100
3. Calculate: = 0.5 × 100 = **50%**

### Problem Type 4: Water Removal (2 minutes)

**Given:** 1000 kg at 20% wb → 14% wb

**Steps:**
1. Find dry matter: DM = 1000 × (100-20)/100 = 800 kg
2. Final mass: Mf = 800/(100-14) × 100 = 930.2 kg
3. Water removed: = 1000 - 930.2 = **69.8 kg**

### Problem Type 5: Drying Time (2 minutes)

**Given:** K = 0.3 hr⁻¹, M₀ = 25%, Me = 12%, M = 15% (all db)

**Steps:**
1. Write: t = -(1/K) × ln[(M-Me)/(M₀-Me)]
2. Calculate MR: = (15-12)/(25-12) = 3/13 = 0.231
3. t = -(1/0.3) × ln(0.231) = -(-3.33) × 1.466
4. Result: = **4.88 hours**

---

## 💡 Memory Techniques

### 1. "PEKEG" Chain (Psychrometry)
- **P**ressure (vapor)
- **E**quilibrium
- **K** (drying constant)
- **E**MC
- **G**rain quality

### 2. "12-14 Rule"
Most cereals: **12-14% wb** safe storage
- Wheat ✓
- Paddy ✓
- Rice (12-13%, slightly lower)

### 3. "LSU for Paddy Please"
**LSU dryer** = **Louisiana State University**
- Primary use: **Paddy drying**
- Continuous column design
- Most common in Asia

### 4. "At 100% RH, Twins They Be"
**RH = 100%** → **DBT = WBT**
- No evaporation possible
- No wet bulb depression
- Air fully saturated

### 5. "wb Smaller, db Bigger"
- wb → db: divide by (100-M) [smaller denominator]
- db → wb: divide by (100+M) [bigger denominator]

### 6. "K Times the Gap"
**Drying rate** = K × (M - Me)
- Rate proportional to moisture **gap**
- Larger gap → faster drying
- At Me, rate = 0 (equilibrium)

---

## ⚠️ Common Mistakes

### Mistake 1: Confusing wb and db
❌ **Wrong:** Using wb value in db formula
✅ **Correct:** Check question carefully - "on wet basis" or "dry basis"

### Mistake 2: Negative sign in drying rate
❌ **Wrong:** Reporting negative rate when question asks magnitude
✅ **Correct:** dM/dt = -K(M-Me), but rate magnitude = K(M-Me)

### Mistake 3: Safe MC confusion
❌ **Wrong:** Wheat safe MC = 8-10%
✅ **Correct:** Wheat safe MC = 12-14% wb (most cereals)

### Mistake 4: RH = 100% conditions
❌ **Wrong:** At RH = 100%, DBT > WBT
✅ **Correct:** At RH = 100%, DBT = WBT (no depression)

### Mistake 5: Dryer selection
❌ **Wrong:** Tray dryer for large-scale paddy
✅ **Correct:** LSU dryer for large-scale paddy (continuous operation)

---

## 🎯 Pre-Exam Checklist

### Formulas to Write First on Rough Sheet:
```
1. Mdb = Mwb/(100-Mwb)×100
2. Mwb = Mdb/(100+Mdb)×100
3. dM/dt = -K(M-Me)
4. MR = exp(-Kt)
5. RH = Pa/Ps × 100
```

### Values to Remember:
- **Safe MC:** Wheat/Paddy 12-14%
- **Ps at 30°C:** ~4.24 kPa
- **RH 100%:** DBT = WBT
- **LSU dryer:** Paddy continuous

### Quick Checks:
- ✅ MC always: db > wb (for same moisture)
- ✅ Safe storage: 12-14% for cereals
- ✅ Drying constant K: units hr⁻¹
- ✅ RH range: 0-100% only

---

## 📊 Exam Strategy

### Time Allocation (per question):
- **MC conversion:** 30 seconds
- **Safe MC value:** 15 seconds
- **RH calculation:** 30 seconds
- **Drying rate:** 1 minute
- **Drying time:** 2-3 minutes
- **Water removal:** 2 minutes

### Priority Topics (likely to appear):
1. 🔥🔥🔥 **MC conversion** (EVERY year)
2. 🔥🔥 **Drying rate** (80% years)
3. 🔥 **Safe storage values**
4. 🔥 **Dryer selection**
5. **Psychrometry basics**

### If Short on Time:
1. Master MC conversions (guaranteed marks)
2. Memorize safe MC values
3. Learn drying rate formula
4. Practice RH calculations
5. Know LSU dryer for paddy

---

## 🚀 Last-Minute Tips (1 Hour Before Exam)

### Write these on entry:
```
Mdb = Mwb/(100-Mwb)×100
Safe MC = 12-14% (Wheat, Paddy)
dM/dt = K(M-Me)
RH 100% → DBT = WBT
LSU for Paddy
```

### Mental checklist:
- [ ] MC conversions practiced?
- [ ] Safe storage values memorized?
- [ ] Newton's law clear?
- [ ] RH formula ready?
- [ ] Dryer types known?

### During exam:
1. Read carefully: wb or db?
2. Write formula before substituting
3. Check units in answer
4. Verify: db > wb for same moisture?
5. For LSU questions: Answer "Paddy" confidently

---

*[Theory](./README.md) | [Solutions](./Solutions.md) | [Section Home](../README.md)*
